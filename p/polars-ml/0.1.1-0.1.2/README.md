# Comparing `tmp/polars_ml-0.1.1-cp38-abi3-win_amd64.whl.zip` & `tmp/polars_ml-0.1.2-cp38-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,19 @@
-Zip file size: 3118697 bytes, number of entries: 13
--rw-r--r--  4.6 unx     3317 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     1068 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      479 b- defN 24-Apr-12 11:32 polars_ml/nltk/functions.py
--rw-r--r--  4.6 unx      496 b- defN 24-Apr-12 11:32 polars_ml/nltk/nltk_namespace.py
--rw-r--r--  4.6 unx      109 b- defN 24-Apr-12 11:32 polars_ml/nltk/__init__.py
--rw-r--r--  4.6 unx       53 b- defN 24-Apr-12 11:32 polars_ml/sparse/constants.py
--rw-r--r--  4.6 unx     1174 b- defN 24-Apr-12 11:32 polars_ml/sparse/functions.py
--rw-r--r--  4.6 unx      502 b- defN 24-Apr-12 11:32 polars_ml/sparse/sparse_namespace.py
--rw-r--r--  4.6 unx      126 b- defN 24-Apr-12 11:32 polars_ml/sparse/__init__.py
--rw-r--r--  4.6 unx       48 b- defN 24-Apr-12 11:32 polars_ml/__init__.py
--rwxr-xr-x  4.6 unx 12606976 b- defN 24-Apr-12 11:32 polars_ml/polars_ml.pyd
--rw-r--r--  4.6 unx     1079 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/RECORD
-13 files, 12615521 bytes uncompressed, 3116889 bytes compressed:  75.3%
+Zip file size: 4509472 bytes, number of entries: 17
+-rw-r--r--  4.6 unx     5502 b- defN 24-May-01 06:56 polars_ml-0.1.2.dist-info/METADATA
+-rw-r--r--  4.6 unx      127 b- defN 24-May-01 06:56 polars_ml-0.1.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1068 b- defN 24-May-01 06:56 polars_ml-0.1.2.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      107 b- defN 24-May-01 06:56 polars_ml/nltk/__init__.py
+-rw-r--r--  4.6 unx      463 b- defN 24-May-01 06:56 polars_ml/nltk/functions.py
+-rw-r--r--  4.6 unx      481 b- defN 24-May-01 06:56 polars_ml/nltk/nltk_namespace.py
+-rw-r--r--  4.6 unx       50 b- defN 24-May-01 06:56 polars_ml/sparse/constants.py
+-rw-r--r--  4.6 unx      123 b- defN 24-May-01 06:56 polars_ml/sparse/__init__.py
+-rw-r--r--  4.6 unx     1143 b- defN 24-May-01 06:56 polars_ml/sparse/functions.py
+-rw-r--r--  4.6 unx      487 b- defN 24-May-01 06:56 polars_ml/sparse/sparse_namespace.py
+-rw-r--r--  4.6 unx       69 b- defN 24-May-01 06:56 polars_ml/__init__.py
+-rw-r--r--  4.6 unx      107 b- defN 24-May-01 06:56 polars_ml/graph/__init__.py
+-rw-r--r--  4.6 unx      484 b- defN 24-May-01 06:56 polars_ml/graph/graph_namespace.py
+-rw-r--r--  4.6 unx     3533 b- defN 24-May-01 06:56 polars_ml/graph/node2vec_function.py
+-rw-r--r--  4.6 unx       55 b- defN 24-May-01 06:56 polars_ml/graph/functions.py
+-rwxr-xr-x  4.6 unx 19228192 b- defN 24-May-01 06:56 polars_ml/polars_ml.abi3.so
+-rw-r--r--  4.6 unx     1433 b- defN 24-May-01 06:56 polars_ml-0.1.2.dist-info/RECORD
+17 files, 19243424 bytes uncompressed, 4507102 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -1,40 +1,52 @@
-Filename: polars_ml-0.1.1.dist-info/METADATA
+Filename: polars_ml-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: polars_ml-0.1.1.dist-info/WHEEL
+Filename: polars_ml-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: polars_ml-0.1.1.dist-info/license_files/LICENSE.txt
+Filename: polars_ml-0.1.2.dist-info/license_files/LICENSE.txt
+Comment: 
+
+Filename: polars_ml/nltk/__init__.py
 Comment: 
 
 Filename: polars_ml/nltk/functions.py
 Comment: 
 
 Filename: polars_ml/nltk/nltk_namespace.py
 Comment: 
 
-Filename: polars_ml/nltk/__init__.py
+Filename: polars_ml/sparse/constants.py
 Comment: 
 
-Filename: polars_ml/sparse/constants.py
+Filename: polars_ml/sparse/__init__.py
 Comment: 
 
 Filename: polars_ml/sparse/functions.py
 Comment: 
 
 Filename: polars_ml/sparse/sparse_namespace.py
 Comment: 
 
-Filename: polars_ml/sparse/__init__.py
+Filename: polars_ml/__init__.py
 Comment: 
 
-Filename: polars_ml/__init__.py
+Filename: polars_ml/graph/__init__.py
+Comment: 
+
+Filename: polars_ml/graph/graph_namespace.py
+Comment: 
+
+Filename: polars_ml/graph/node2vec_function.py
+Comment: 
+
+Filename: polars_ml/graph/functions.py
 Comment: 
 
-Filename: polars_ml/polars_ml.pyd
+Filename: polars_ml/polars_ml.abi3.so
 Comment: 
 
-Filename: polars_ml-0.1.1.dist-info/RECORD
+Filename: polars_ml-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## polars_ml/nltk/functions.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-import os.path
-import polars as pl
-from polars.utils.udfs import _get_shared_lib_location
-from polars.plugins import register_plugin_function
-
-
-_lib = _get_shared_lib_location(os.path.dirname(__file__))
-
-
-def snowball_stem(expr: pl.Expr, *, language: str) -> pl.Expr:
-    return register_plugin_function(
-        args=[expr],
-        plugin_path=_lib,
-        function_name='snowball_stem',
-        is_elementwise=True,
-        kwargs={'language': language}
+import os.path
+import polars as pl
+from polars.utils.udfs import _get_shared_lib_location
+from polars.plugins import register_plugin_function
+
+
+_lib = _get_shared_lib_location(os.path.dirname(__file__))
+
+
+def snowball_stem(expr: pl.Expr, *, language: str) -> pl.Expr:
+    return register_plugin_function(
+        args=[expr],
+        plugin_path=_lib,
+        function_name='snowball_stem',
+        is_elementwise=True,
+        kwargs={'language': language}
     )
```

## polars_ml/nltk/nltk_namespace.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, Callable
-import polars as pl
-from polars_ml.nltk import functions
-
-
-@pl.api.register_expr_namespace("nltk")
-class NltkNamespace:
-    def __init__(self, expr: pl.Expr):
-        self._expr = expr
-
-    def __getattr__(self, function_name: str) -> Callable[[Any], pl.Expr]:
-        def func(*args: Any, **kwargs: Any) -> pl.Expr:
-            return getattr(functions, function_name)(
-                self._expr, *args, **kwargs
-            )
+from typing import Any, Callable
+import polars as pl
+from polars_ml.nltk import functions
+
+
+@pl.api.register_expr_namespace("nltk")
+class NltkNamespace:
+    def __init__(self, expr: pl.Expr):
+        self._expr = expr
+
+    def __getattr__(self, function_name: str) -> Callable[[Any], pl.Expr]:
+        def func(*args: Any, **kwargs: Any) -> pl.Expr:
+            return getattr(functions, function_name)(
+                self._expr, *args, **kwargs
+            )
         return func
```

## polars_ml/nltk/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-from polars_ml.nltk.nltk_namespace import NltkNamespace
-from polars_ml.nltk.functions import snowball_stem
+from polars_ml.nltk.nltk_namespace import NltkNamespace
+from polars_ml.nltk.functions import snowball_stem
```

## polars_ml/sparse/constants.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-DIM = 'dim'
-INDICES = 'indices'
-VALUES = 'values'
+DIM = 'dim'
+INDICES = 'indices'
+VALUES = 'values'
```

## polars_ml/sparse/functions.py

 * *Ordering differences only*

```diff
@@ -1,31 +1,31 @@
-import os.path
-import polars as pl
-from polars.utils.udfs import _get_shared_lib_location
-from polars.plugins import register_plugin_function
-from polars_ml.sparse.constants import DIM, INDICES, VALUES
-
-
-_lib = _get_shared_lib_location(os.path.dirname(__file__))
-
-
-def from_list(expr: pl.Expr) -> pl.expr:
-    output_name = expr.meta.output_name()
-    return pl.struct(pl.when(expr.is_null()).then(None).otherwise(expr.list.len().alias(DIM)),
-                     expr.list.eval(pl.arg_where(pl.element() != 0)).alias(INDICES),
-                     expr.list.eval(pl.element().filter(pl.element() != 0)).alias(VALUES)).alias(output_name)
-
-
-def normalize(expr: pl.Expr,  *, how: str = 'vertical', p: float = 2.0) -> pl.Expr:
-    # validate params
-    if how not in ['vertical']:
-        raise ValueError(f'Illegal how = {how}, only vertical is supported.')
-    if p < 1.0:
-        raise ValueError(f'p must be greater or equals to 1.0, {p} was given.')
-
-    return register_plugin_function(
-        args=[expr],
-        plugin_path=_lib,
-        function_name='normalize',
-        is_elementwise=True,
-        kwargs={'how': how, 'p': p}
-    )
+import os.path
+import polars as pl
+from polars.utils.udfs import _get_shared_lib_location
+from polars.plugins import register_plugin_function
+from polars_ml.sparse.constants import DIM, INDICES, VALUES
+
+
+_lib = _get_shared_lib_location(os.path.dirname(__file__))
+
+
+def from_list(expr: pl.Expr) -> pl.expr:
+    output_name = expr.meta.output_name()
+    return pl.struct(pl.when(expr.is_null()).then(None).otherwise(expr.list.len().alias(DIM)),
+                     expr.list.eval(pl.arg_where(pl.element() != 0)).alias(INDICES),
+                     expr.list.eval(pl.element().filter(pl.element() != 0)).alias(VALUES)).alias(output_name)
+
+
+def normalize(expr: pl.Expr,  *, how: str = 'vertical', p: float = 2.0) -> pl.Expr:
+    # validate params
+    if how not in ['vertical']:
+        raise ValueError(f'Illegal how = {how}, only vertical is supported.')
+    if p < 1.0:
+        raise ValueError(f'p must be greater or equals to 1.0, {p} was given.')
+
+    return register_plugin_function(
+        args=[expr],
+        plugin_path=_lib,
+        function_name='normalize',
+        is_elementwise=True,
+        kwargs={'how': how, 'p': p}
+    )
```

## polars_ml/sparse/sparse_namespace.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, Callable
-import polars as pl
-from polars_ml.sparse import functions
-
-
-@pl.api.register_expr_namespace("sparse")
-class SparseNamespace:
-    def __init__(self, expr: pl.Expr):
-        self._expr = expr
-
-    def __getattr__(self, function_name: str) -> Callable[[Any], pl.Expr]:
-        def func(*args: Any, **kwargs: Any) -> pl.Expr:
-            return getattr(functions, function_name)(
-                self._expr, *args, **kwargs
-            )
+from typing import Any, Callable
+import polars as pl
+from polars_ml.sparse import functions
+
+
+@pl.api.register_expr_namespace("sparse")
+class SparseNamespace:
+    def __init__(self, expr: pl.Expr):
+        self._expr = expr
+
+    def __getattr__(self, function_name: str) -> Callable[[Any], pl.Expr]:
+        def func(*args: Any, **kwargs: Any) -> pl.Expr:
+            return getattr(functions, function_name)(
+                self._expr, *args, **kwargs
+            )
         return func
```

## polars_ml/sparse/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-from polars_ml.sparse.sparse_namespace import SparseNamespace
-from polars_ml.sparse.functions import from_list, normalize
-
+from polars_ml.sparse.sparse_namespace import SparseNamespace
+from polars_ml.sparse.functions import from_list, normalize
+
```

## polars_ml/__init__.py

```diff
@@ -1,2 +1,3 @@
-import polars_ml.nltk
-import polars_ml.sparse
+import polars_ml.nltk
+import polars_ml.sparse
+import polars_ml.graph
```

## Comparing `polars_ml-0.1.1.dist-info/license_files/LICENSE.txt` & `polars_ml-0.1.2.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

