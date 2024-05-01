# Comparing `tmp/lhs-0.4.1-py3-none-any.whl.zip` & `tmp/lhs-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,9 @@
-Zip file size: 9390 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     4474 b- defN 23-Jan-20 04:38 lhs/__init__.py
--rw-rw-r--  2.0 unx     6182 b- defN 23-Jan-20 04:33 lhs/dist.py
--rw-rw-r--  2.0 unx     6433 b- defN 22-Dec-23 03:53 lhs/sample.py
--rw-rw-r--  2.0 unx     1497 b- defN 23-Jan-20 04:38 lhs-0.4.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4175 b- defN 23-Jan-20 04:38 lhs-0.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-20 04:38 lhs-0.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-Jan-20 04:38 lhs-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Aug-19 02:37 lhs-0.4.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      657 b- defN 23-Jan-20 04:38 lhs-0.4.1.dist-info/RECORD
-9 files, 23515 bytes uncompressed, 8272 bytes compressed:  64.8%
+Zip file size: 9098 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4503 b- defN 20-Feb-02 00:00 lhs/__init__.py
+-rw-r--r--  2.0 unx     6216 b- defN 20-Feb-02 00:00 lhs/dist.py
+-rw-r--r--  2.0 unx     6416 b- defN 20-Feb-02 00:00 lhs/sample.py
+?rw-r--r--  2.0 unx     4269 b- defN 20-Feb-02 00:00 lhs-0.4.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lhs-0.4.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1497 b- defN 20-Feb-02 00:00 lhs-0.4.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      497 b- defN 20-Feb-02 00:00 lhs-0.4.2.dist-info/RECORD
+7 files, 23485 bytes uncompressed, 8236 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,26 +3,20 @@
 
 Filename: lhs/dist.py
 Comment: 
 
 Filename: lhs/sample.py
 Comment: 
 
-Filename: lhs-0.4.1.dist-info/LICENSE
+Filename: lhs-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: lhs-0.4.1.dist-info/METADATA
+Filename: lhs-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: lhs-0.4.1.dist-info/WHEEL
+Filename: lhs-0.4.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: lhs-0.4.1.dist-info/top_level.txt
-Comment: 
-
-Filename: lhs-0.4.1.dist-info/zip-safe
-Comment: 
-
-Filename: lhs-0.4.1.dist-info/RECORD
+Filename: lhs-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lhs/__init__.py

```diff
@@ -71,19 +71,21 @@
     # Collect the independent and dependent parameter names.
     indep_names = list(params.keys())
     dep_names = list(dep_params.keys())
 
     # Collect the details for each parameter in turn.
     param_shapes = []
     for name in indep_names:
-        param_shapes.append((name, params[name].get('shape'),
-                             params[name].get('broadcast')))
+        shape = params[name].get('shape')
+        broadcast = params[name].get('broadcast')
+        param_shapes.append((name, shape, broadcast))
     for name in dep_names:
-        param_shapes.append((name, dep_params[name].get('shape'),
-                             dep_params[name].get('broadcast')))
+        shape = dep_params[name].get('shape')
+        broadcast = dep_params[name].get('broadcast')
+        param_shapes.append((name, shape, broadcast))
 
     # Draw subspace samples for each parameter.
     subspace_samples = sample.sample_subspaces(rng, n, param_shapes)
 
     # Obtain sample values for each independent parameter.
     if values is None:
         values = {}
@@ -100,12 +102,13 @@
         # Ensure that the expected distributions have been defined.
         expect_dists = set(dep_params.keys())
         actual_dists = set(dep_dists.keys())
         if expect_dists != actual_dists:
             raise ValueError('Inconsistent dependent parameters')
 
         # Obtain sample values for each dependent parameter in turn.
-        for (name, dist) in dep_dists.items():
-            values[name] = sample.lhs_values(name, dist,
-                                             subspace_samples[name])
+        for name, dist in dep_dists.items():
+            values[name] = sample.lhs_values(
+                name, dist, subspace_samples[name]
+            )
 
     return values
```

## lhs/dist.py

```diff
@@ -29,15 +29,16 @@
         final_period = dist_name.rfind('.')
         if final_period < 0:
             # No period, look for a function in this module.
             fn = getattr(sys.modules[__name__], dist_name)
         else:
             # Also support fully-qualified function names.
             module_name = dist_name[:final_period]
-            value_name = dist_name[final_period + 1:]
+            name_ix = final_period + 1
+            value_name = dist_name[name_ix:]
             module = importlib.import_module(module_name)
             fn = getattr(module, value_name)
     except (AttributeError, ModuleNotFoundError):
         return scipy_stats_dist(samples, dist_name, dist_kwargs)
 
     if not callable(fn):
         name = __name__ + '.' + dist_name
@@ -157,11 +158,11 @@
     :param dist_kwargs: The (distribution-specific) shape parameters.
     :returns: The sample values as a ``numpy.ndarray`` that has the same shape
         as ``samples``.
     :raises ValueError: if the distribution ``dist_name`` is not defined.
     """
     try:
         dist_class = getattr(scipy.stats, dist_name)
-    except AttributeError:
-        raise ValueError('Unknown distribution "{}"'.format(dist_name))
+    except AttributeError as e:
+        raise ValueError(f'Unknown distribution "{dist_name}"') from e
     dist_obj = dist_class(**dist_kwargs)
     return dist_obj.ppf(samples)
```

## lhs/sample.py

```diff
@@ -70,16 +70,15 @@
             index = (slice(None, None), *ixs)
             # Select a random sample ordering for this index.
             samples[index] = (rng.permutation(n) + rng.random(size=n)) / n
 
     # Broadcast the samples to the desired output shape (if any).
     if broadcast is not None:
         # Construct the indexing slice.
-        index = [None if b > 0 else slice(None, None)
-                 for b in broadcast]
+        index = [None if b > 0 else slice(None, None) for b in broadcast]
         index.insert(0, slice(None, None))
         index = tuple(index)
 
         # Determine the output shape.
         shape_out = [n]
         shape_ix = 1
         for b in broadcast:
```

## Comparing `lhs-0.4.1.dist-info/LICENSE` & `lhs-0.4.2.dist-info/licenses/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-23, Rob Moss
+Copyright (c) 2020-24, Rob Moss
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

## Comparing `lhs-0.4.1.dist-info/METADATA` & `lhs-0.4.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lhs
-Version: 0.4.1
+Version: 0.4.2
 Summary: Latin hypercube sampler for scenario modelling
+Project-URL: homepage, https://bitbucket.org/robmoss/latin-hypercube-sampler/
+Project-URL: repository, https://bitbucket.org/robmoss/latin-hypercube-sampler/
+Project-URL: documentation, https://lhs.readthedocs.io/en/latest/
+Project-URL: changelog, https://lhs.readthedocs.io/en/latest/changelog.html
 Author-email: Rob Moss <rgmoss@unimelb.edu.au>
 Maintainer-email: Rob Moss <rgmoss@unimelb.edu.au>
-License: Copyright (c) 2020-23, Rob Moss
+License: Copyright (c) 2020-24, Rob Moss
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -27,31 +31,29 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: homepage, https://bitbucket.org/robmoss/latin-hypercube-sampling/
-Project-URL: repository, https://bitbucket.org/robmoss/latin-hypercube-sampling/
-Project-URL: documentation, https://lhs.readthedocs.io/en/latest/
-Project-URL: changelog, https://lhs.readthedocs.io/en/latest/changelog.html
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
+Requires-Dist: numpy>=1.17
+Requires-Dist: scipy~=1.4
+Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov~=4.0; extra == 'tests'
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: numpy (~=1.17)
-Requires-Dist: scipy (~=1.4)
 
 Latin hypercube sampler for scenario modelling
 ==================================================
 
 |version| |docs| |tests| |coverage|
 
 Description
```

