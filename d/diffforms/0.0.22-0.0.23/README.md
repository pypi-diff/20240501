# Comparing `tmp/diffforms-0.0.22.tar.gz` & `tmp/diffforms-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffforms-0.0.22.tar", last modified: Mon Apr 29 22:16:25 2024, max compression
+gzip compressed data, was "diffforms-0.0.23.tar", last modified: Tue Apr 30 08:51:21 2024, max compression
```

## Comparing `diffforms-0.0.22.tar` & `diffforms-0.0.23.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.161721 diffforms-0.0.22/
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.22/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 22:16:25.160724 diffforms-0.0.22/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1540 2024-04-29 22:16:05.000000 diffforms-0.0.22/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.149290 diffforms-0.0.22/diffforms/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.22/diffforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20224 2024-04-29 22:12:09.000000 diffforms-0.0.22/diffforms/core.py
--rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-29 22:15:09.000000 diffforms-0.0.22/diffforms/release.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.159197 diffforms-0.0.22/diffforms.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.22/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 22:16:25.161811 diffforms-0.0.22/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.22/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 08:51:21.206788 diffforms-0.0.23/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.23/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-30 08:51:21.184448 diffforms-0.0.23/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1462 2024-04-29 22:24:18.000000 diffforms-0.0.23/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 08:51:21.180400 diffforms-0.0.23/diffforms/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.23/diffforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20759 2024-04-30 08:50:49.000000 diffforms-0.0.23/diffforms/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-30 08:51:10.000000 diffforms-0.0.23/diffforms/release.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 08:51:21.183896 diffforms-0.0.23/diffforms.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-30 08:51:21.000000 diffforms-0.0.23/diffforms.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-30 08:51:21.000000 diffforms-0.0.23/diffforms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-30 08:51:21.000000 diffforms-0.0.23/diffforms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-30 08:51:21.000000 diffforms-0.0.23/diffforms.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-30 08:51:21.000000 diffforms-0.0.23/diffforms.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.23/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-30 08:51:21.206920 diffforms-0.0.23/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.23/setup.py
```

### Comparing `diffforms-0.0.22/PKG-INFO` & `diffforms-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.22
+Version: 0.0.23
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.22/README.md` & `diffforms-0.0.23/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 General
 =======
-The Diffform python package implements differential forms and poly-forms from differential geometry. It includes some of the usual operations found in exterior calculus, include exterior product, differential operator. The main advatage of this package over other differential form packages ( e.g. [pycartan](https://github.com/TUD-RST/pycartan) ) is that it allows for polyforms and there is no dependence on basis forms. However, this removes some useful operations like insertion of vector fields.
+The Diffform python package implements differential forms and poly-forms from differential geometry. It includes some of the usual operations found in exterior calculus, include exterior product, differential operator. The main advatage of this package over other differential form packages ( e.g. [pycartan](https://github.com/TUD-RST/pycartan) ) is that it allows for polyforms and there is no dependence on basis forms.
 
 This package is a part-time project during my PhD so updates should be suspected to end eventually. Bugs and mistakes may (possibly will) be prevalent.
 
 Documentary will be implemented when I find the time, in the mean time I will try to provide comments in the code as a type of documentation.
 
 ToDo List
 =========
```

### Comparing `diffforms-0.0.22/diffforms/core.py` & `diffforms-0.0.23/diffforms/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         
     def __eq__(self,other): return (self.symbol == other.symbol) and (self.degree == other.degree)
     def __hash__(self): return hash((str(self.symbol),self.degree))
 
     def __mul__(self,other): return WedgeProduct(self,other)
     def __rmul__(self,other): return WedgeProduct(other,self)
     def __div__(self,other): return WedgeProduct(self,1/other)
+    def __truediv__(self,other): return WedgeProduct(self,1/other)
 
     def __add__(self,other):
         ret = DifferentialFormMul()
         if isinstance(other,AtomicExpr) or isinstance(other,float) or isinstance(other,int):
             ret.forms_list = [[self],[DifferentialForm(Integer(1),0)]]
             ret.factors = [1,other]
         elif isinstance(other,DifferentialForm):
@@ -176,14 +177,17 @@
     __repr__ = _repr_latex_
     _latex   = _repr_latex_
     _print   = _repr_latex_
     
     def __eq__(self,other):
         if isinstance(other,DifferentialForm):
             return str(self.symbol) == str(other.symbol) and self.degree == other.degree
+
+    def _eval_simplify(self, **kwargs):
+        return self
     
     def insert(self,vector:VectorField):
         if isinstance(vector,VectorField):
             if self.symbol == vector.symbol: return 1
             else: return 0
         else:
             raise NotImplementedError
@@ -192,17 +196,27 @@
     def d(self):
         if self.exact: return DifferentialForm(Number(0),self.degree+1,exact=True)
         elif isinstance(self.symbol,Number): return DifferentialForm(Number(0),self.degree+1,exact=True)
         else:
             dsymbol = symbols(r"d\left("+str(self.symbol)+r"\right)")
             return DifferentialForm(dsymbol,degree=self.degree+1,exact=True)
         raise NotImplementedError
-    
-    def _eval_simplify(self, **kwargs):
-        return self
+
+    def subs(self,target,sub=None):
+        if target == self: return sub
+        elif isinstance(target,DifferentialFormMul):
+            if len(target.factors) == 1 and target.forms_list == [[self]]:
+                return sub/target.factors[0]
+        elif isinstance(target,dict):
+            ret = DifferentialForm(self.symbol,self.degree)
+            ret.exact = self.exact
+            for t in target:
+                ret = ret.subs(t,target[t])
+            return ret
+
 
 class DifferentialFormMul():
 
     def __init__(self,form:DifferentialForm=None,factor:AtomicExpr=None):
         self.__sympy__ = True
         if form == None:
             self.forms_list = []
@@ -388,59 +402,59 @@
                         new_factors_list.append(ret.factors[i])
                 else:
                     new_forms_list+=[ret.forms_list[i]]
                     new_factors_list.append(ret.factors[i])
             ret.factors = new_factors_list
             ret.forms_list = new_forms_list
         elif isinstance(target,DifferentialFormMul):
-            if len(target.factors) > 1: raise NotImplementedError("Cannot match more than 1 term at a time")
+            if len(target.factors) > 1: raise NotImplementedError("Cannot replace more than 1 term at a time")
             new_forms_list = []
             new_factors_list = []
             for i in range(len(ret.forms_list)):
                 match_index = -1
                 for j in range(len(ret.forms_list[i])-len(target.forms_list[0])+1):
                     if ret.forms_list[i][j:j+len(target.forms_list[0])] == target.forms_list[0]:
                         match_index = j
                         break
                 if match_index != -1:
                     if isinstance(sub,DifferentialFormMul):
                         for k in range(len(sub.factors)):
                             s = sub.forms_list[k]
                             f = sub.factors[k]
-                            new_forms_list += [ret.forms_list[i][:match_index] + s + ret.forms_list[i][match_index+len(target.forms_list[0])+1:]]
+                            new_forms_list += [ret.forms_list[i][:match_index] + s + ret.forms_list[i][match_index+len(target.forms_list[0]):]]
                             new_factors_list.append(ret.factors[i]*f/target.factors[0])
                     elif isinstance(sub,DifferentialForm):
                         new_forms_list += [ret.forms_list[i][:match_index] + [sub] + ret.forms_list[i][match_index+len(target.forms_list[0]):]]
                         new_factors_list.append(ret.factors[i]/target.factors[0])
-                    elif isinstance(sub,float) or isinstance(sub,int) or isinstance(sub,AtomicExpr):
+                    elif isinstance(sub,(float,int,AtomicExpr,Expr)):
                         new_forms_list +=[ret.forms_list[i][:match_index] + ret.forms_list[i][match_index+len(target.forms_list[0]):]]
                         new_factors_list.append(ret.factors[i]*sub/target.factors[0])
                 else:
                     new_forms_list += [ret.forms_list[i]]
                     new_factors_list.append(ret.factors[i])
             ret.factors = new_factors_list
             ret.forms_list = new_forms_list
         elif isinstance(target,dict):
             for key in target:
                 ret = ret.subs(key,target[key])
-
-        if not isinstance(sub,DifferentialForm) and not isinstance(sub,DifferentialFormMul) and sub != None:
+        elif sub != None:
             for i in range(len(self.factors)):
-                    ret.factors[i] = ret.factors[i].subs(target,sub)
-
+                ret.factors[i] = ret.factors[i].subs(target,sub)
+        
         ret = simplify(ret)
         return ret
 
     def insert(self,vect:VectorField):
         ret = DifferentialFormMul()
         if isinstance(vect,VectorField):
             for i in range(len(self.factors)):
                 sign = 1
                 for j in range(len(self.forms_list[i])):
-                    if self.forms_list[i][j].symbol == vect.symbol:
+                    cur_symbol = self.forms_list[i][j].symbol
+                    if cur_symbol == vect.symbol or str(cur_symbol) == "d\\left("+str(vect.symbol)+"\\right)":
                         ret.forms_list += [self.forms_list[i][:j] + self.forms_list[i][j+1:]]
                         ret.factors += [self.factors[i]*sign]
                         break
                     else:
                         sign *= (-1)**self.forms_list[i][j].degree
         else:
             raise NotImplementedError
```

### Comparing `diffforms-0.0.22/diffforms.egg-info/PKG-INFO` & `diffforms-0.0.23/diffforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.22
+Version: 0.0.23
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.22/setup.py` & `diffforms-0.0.23/setup.py`

 * *Files identical despite different names*

