# Comparing `tmp/pldag-0.7.7.tar.gz` & `tmp/pldag-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.7.tar", max compression
+gzip compressed data, was "pldag-0.7.8.tar", max compression
```

## Comparing `pldag-0.7.7.tar` & `pldag-0.7.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.7/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.7/README.md
--rw-r--r--   0        0        0    33037 2024-04-26 11:21:47.553528 pldag-0.7.7/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.7/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.7/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-26 11:21:55.153992 pldag-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.8/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.8/README.md
+-rw-r--r--   0        0        0    34855 2024-05-01 13:43:39.180071 pldag-0.7.8/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.8/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.8/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-01 13:44:02.390036 pldag-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.8/PKG-INFO
```

### Comparing `pldag-0.7.7/LICENSE` & `pldag-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.7/README.md` & `pldag-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.7/pldag/__init__.py` & `pldag-0.7.8/pldag/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         ).static_order()
     
     @staticmethod
     def _composite_id(children: list, bias: int, negate: bool = False) -> str:
         """
             Create a composite ID from a list of children.
         """
-        return sha1(("".join(sorted(set(children))) + str(negate) + str(bias)).encode()).hexdigest()
+        return sha1(("".join(map(lambda x: sha1(x.encode()).hexdigest(), sorted(set(children)))) + str(negate) + str(bias)).encode()).hexdigest()
     
     @property
     def primitives(self) -> np.ndarray:
         return self._col_vars[~self._cvec]
     
     @property
     def composites(self) -> np.ndarray:
@@ -704,76 +704,110 @@
         """
         return self.set_xor([
             self.set_and(references),
             self.set_not(references),
         ], alias)
     
     @lru_cache
-    def to_polyhedron(self, **fix: Dict[str, complex]) -> tuple:
+    def to_polyhedron(self, double_binding: bool = True, **assume: Dict[str, complex]) -> tuple:
 
         """
             Constructs a polyhedron of matrix A and bias vector b,
             such that A.dot(x) >= b, where x is the vector of variables.
             Every composite variable A is its own column in the matrix where
             A -> (A's composite proposition) is true. 
 
             Parameters
             ----------
-            fix : Dict[str, int]
-                A dictionary of variables to fix.
+            assume : Dict[str, int]
+                A dictionary of variables to assume tighter bounds.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
             >>> A, b = model.to_polyhedron()
             >>> np.array_equal(A, np.array([[1,1,1,-1]]))
             True
         """
 
+        # From a aux variable A such that A <-> X, and the constraint X: c*x + c*y + c*z >= d, where n is the number of terms on left hand side, we have the following constraints:
+        # `mx` is the maximum sum over the inner variables in a constraint X.
+        # For atleast constraints:
+        # 1) -dA + sum(+X) >= ±0             (-A v +X)
+        # 2) +mx*A + sum(-X) >= -(d-1)       (+A v -X)
+
+        # For atmost constraints:
+        # 1) (-mx-d)A + sum(-X) >= -mx       (-A v +X)
+        # 2) (-d+mn+1)A + sum(+X) >= (-d+1)     (+A v -X)
+
         # Create the matrix
-        A = np.zeros(self._amat.shape, dtype=np.int64)
+        A = np.zeros((self._amat.shape[0] * 2, self._amat.shape[1]), dtype=np.int64)
+        b = np.zeros(self._amat.shape[0] * 2, dtype=np.int64)
+
+        # Find max of inner bounds for each composite
+        ad = self._amat.dot(self._dvec)
+        mn = ad.real
+        mx = ad.imag
+
+        # Extract `d` vector from bias
+        d = -1 * self._bvec.real
 
         # Adjacent points
         adj_points = np.argwhere(self._amat == 1)
 
-        # Fill the matrix
-        A[adj_points.T[0], adj_points.T[1]] = 1
-
-        # Flip the once that are negated
-        A[self._nvec == 1] *= -1
+        # A -> X row indices
+        A_X_ri = adj_points.T[0]
+        A_X = np.unique(A_X_ri)
+        # X -> A row indices
+        X_A_ri = adj_points.T[0] + adj_points.T[0].max() + 1
+        X_A = np.unique(X_A_ri)
+
+        # Fill the matrix with adjacency points
+        A[A_X_ri, adj_points.T[1]] = -1
+        A[X_A_ri, adj_points.T[1]] = -1
+
+        # Assign 1 instead of -1 to the at least A -> X, and at most constraints for X -> A.
+        A[A_X[~self._nvec], :] *= -1
+        A[X_A[self._nvec], :] *= -1
 
         # Composite index in matrix
         cidx = np.array(list(self._imap.values()))[self._cvec]
 
-        # Fetch the inner bounds
-        inner_bounds = self._amat.dot(self._dvec)
-
-        # Flip those that are negated
-        inner_bounds[self._nvec == 1] = np.conj(inner_bounds[self._nvec == 1]) * -1j
-
-        # Add onto bias so the bounds are correct
-        eq_bounds = inner_bounds + self._bvec
-
-        # Fill the composite id's with the mx value
-        A[range(A.shape[0]), cidx] = eq_bounds.real
-
-        # Create the bias vector. The linear equation should be increased
-        # by the flipped minimum value
-        b = eq_bounds.real - self._bvec.real
+        # Set coef and bias for at least aux variable A->X
+        # 1) (-d+mn)A + sum(-X) >= mn            (-A v +X)
+        A[A_X[~self._nvec], cidx[~self._nvec]] = -d[~self._nvec]+mn[~self._nvec]
+        b[A_X[~self._nvec]] = mn[~self._nvec]
+
+        # Set coef and bias for at least aux var X->A
+        # 2) +mx*A + sum(-X) >= -(d-1)       (+A v -X)
+        if double_binding:
+            A[X_A[~self._nvec], cidx[~self._nvec]] = mx[~self._nvec]-(d[~self._nvec] - 1)
+            b[X_A[~self._nvec]] = -(d[~self._nvec] - 1)
+
+        # Set coef and bias for at most aux variable A->X
+        # 1) (-mx-d)A + sum(-X) >= -mx       (-A v +X)
+        A[A_X[self._nvec], cidx[self._nvec]] = -mx[self._nvec] - d[self._nvec]
+        b[A_X[self._nvec]] = -mx[self._nvec]
+
+        # Set coef and bias for at most aux var X->A
+        # 2) (-d-mn+1)A + sum(+X) >= (-d+1)     (+A v -X)
+        if double_binding:
+            A[X_A[self._nvec], cidx[self._nvec]] = -d[self._nvec] + 1 - mn[self._nvec]
+            b[X_A[self._nvec]] = -d[self._nvec] + 1
 
         # Fix constant variables
         for i, vs in groupby(
             sorted(
                 map(
                     lambda x: (x[0], int(x[1].real)), 
                     filter(
                         lambda x: x[1].real == x[1].imag, 
-                        fix.items()
+                        assume.items()
                     )
                 ),
                 key=lambda x: x[1] 
             ), 
             key=lambda x: x[1]
         ):
             v = list(map(lambda x: x[0], vs))
@@ -799,15 +833,15 @@
         d_imag = self._dvec.imag
 
         # Also, if fix has tighter bounds set we use them instead
         for i, bound in filter(
             lambda x: (x[1].real != x[1].imag), 
             starmap(
                 lambda k,v: (self._col(k), v),
-                fix.items()
+                assume.items()
             )
         ):
             if bound.real > d_real[i]:
                 d_real[i] = bound.real
             elif bound.imag < d_imag[i]:
                 d_imag[i] = bound.imag
         
@@ -900,25 +934,25 @@
                 break
             matching_variables.update(new_matching_variables)
 
         col_idxs = np.array(sorted(list(map(col_vars.index, matching_variables))))
         row_idxs = np.array(sorted(list(map(row_vars.index, filter(lambda v: v in self._row_vars, matching_variables)))))
         return self._from_indices(row_idxs, col_idxs)
     
-    def solve(self, objectives: List[Dict[str, int]], fix: Dict[str, complex], solver: Solver) -> List[Dict[str, complex]]:
+    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, complex], solver: Solver) -> List[Dict[str, complex]]:
         """
             Solves the model with the given objectives.
 
             Parameters
             ----------
             objectives : List[Dict[str, int]]
                 The objectives to solve for.
 
-            fix : Dict[str, complex]
-                The variables to fix.
+            assume : Dict[str, complex]
+                Assume new bounds for variables.
 
             solver : Solver
                 The solver to use.
 
             Examples
             --------
             >>> model = PLDAG()
@@ -928,15 +962,15 @@
             [{'x': 0j, 'y': 1+1j, 'z': 0j}]
 
             Returns
             -------
             List[Dict[str, complex]]
                 The solutions for the objectives.
         """
-        A, b = self.to_polyhedron(**fix)
+        A, b = self.to_polyhedron(**assume)
         variables = self._col_vars
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
```

### Comparing `pldag-0.7.7/pldag/solver/glpk_solver.py` & `pldag-0.7.8/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.7.7/PKG-INFO` & `pldag-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.7
+Version: 0.7.8
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

