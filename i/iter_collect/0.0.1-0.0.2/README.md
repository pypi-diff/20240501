# Comparing `tmp/iter_collect-0.0.1.tar.gz` & `tmp/iter_collect-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iter_collect-0.0.1.tar", max compression
+gzip compressed data, was "iter_collect-0.0.2.tar", max compression
```

## Comparing `iter_collect-0.0.1.tar` & `iter_collect-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iter_collect-0.0.1/LICENSE
--rw-r--r--   0        0        0     7129 2024-04-21 15:34:30.962282 iter_collect-0.0.1/iter_collect/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iter_collect-0.0.1/iter_collect/py.typed
--rw-r--r--   0        0        0     1137 2024-04-21 15:35:24.098271 iter_collect-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-21 15:22:53.442652 iter_collect-0.0.1/readme.md
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 iter_collect-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iter_collect-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     7878 2024-05-01 12:26:54.623510 iter_collect-0.0.2/iter_collect/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iter_collect-0.0.2/iter_collect/py.typed
+-rw-r--r--   0        0        0     1137 2024-05-01 12:26:51.439090 iter_collect-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-21 15:22:53.442652 iter_collect-0.0.2/readme.md
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 iter_collect-0.0.2/PKG-INFO
```

### Comparing `iter_collect-0.0.1/LICENSE` & `iter_collect-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iter_collect-0.0.1/iter_collect/__init__.py` & `iter_collect-0.0.2/iter_collect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = [
     "collect_as_mapping", "group", "uniq", "dups", "iter_dups", "iter_keyed_dups", 
 ]
 
 from collections.abc import Iterable, Iterator, MutableMapping
 from typing import cast, overload, Any, Callable, Literal, Optional, Protocol, TypeVar
 
@@ -145,81 +145,94 @@
 
 
 @overload
 def dups(
     it: Iterable[V], 
     /, 
     key: None = None, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> MutableMapping[V, list[V]]:
     ...
 @overload
 def dups(
     it: Iterable[tuple[K, V]], 
     /, 
     key: Literal[True] = True, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> MutableMapping[K, list[V]]:
     ...
 @overload
 def dups(
     it: Iterable[V], 
     /, 
     key: Callable[[V], K], 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> MutableMapping[K, list[V]]:
     ...
 def dups(
     it: Iterable, 
     /, 
     key: None | Literal[True] | Callable = None, 
-    keep_first: bool | Callable[..., SupportsLT] = True, 
+    keep_first: None | bool | Callable[..., SupportsLT] = True, 
 ) -> dict[Any, list]:
     return collect_as_mapping(iter_keyed_dups(it, key, keep_first=keep_first))
 
 
 @overload
 def iter_dups(
     it: Iterable[V], 
     /, 
     key: None = None, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[V]:
     ...
 @overload
 def iter_dups(
     it: Iterable[tuple[K, V]], 
     /, 
     key: Literal[True] = True, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[V]:
     ...
 @overload
 def iter_dups(
     it: Iterable[V], 
     /, 
     key: Callable[[V], K], 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[V]:
     ...
 def iter_dups(
     it: Iterable, 
     /, 
     key: None | Literal[True] | Callable = None, 
-    keep_first: bool | Callable[..., SupportsLT] = True, 
+    keep_first: None | bool | Callable[..., SupportsLT] = True, 
 ) -> Iterator:
     items: Iterable[tuple[Any, Any]]
     if key is None:
         items = ((e, e) for e in it)
     elif key is True:
         items = it
     else:
         items = ((key(e), e) for e in it)
-    if keep_first is True:
+    if keep_first is None:
         s: set = set()
+        cached: dict = {}
+        add = s.add
+        for k, v in items:
+            if k in s:
+                yield v
+            elif k in cached:
+                yield cached.pop(k)
+                yield v
+                add(k)
+            else:
+                cached[k] = v
+    elif keep_first is True:
+        s = set()
         add = s.add
         for k, v in items:
             if k in s:
                 yield v
             else:
                 add(k)
     elif keep_first is False:
@@ -243,48 +256,61 @@
 
 
 @overload
 def iter_keyed_dups(
     it: Iterable[V], 
     /, 
     key: None = None, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[tuple[Any, V]]:
     ...
 @overload
 def iter_keyed_dups(
     it: Iterable[tuple[K, V]], 
     /, 
     key: Literal[True] = True, 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[tuple[Any, V]]:
     ...
 @overload
 def iter_keyed_dups(
     it: Iterable[V], 
     /, 
     key: Callable[[V], K], 
-    keep_first: bool | Callable[[V], SupportsLT] = True, 
+    keep_first: None | bool | Callable[[V], SupportsLT] = True, 
 ) -> Iterator[tuple[Any, V]]:
     ...
 def iter_keyed_dups(
     it: Iterable, 
     /, 
     key: None | Literal[True] | Callable = None, 
-    keep_first: bool | Callable[..., SupportsLT] = True, 
+    keep_first: None | bool | Callable[..., SupportsLT] = True, 
 ) -> Iterator:
     items: Iterable[tuple[Any, Any]]
     if key is None:
         items = ((e, e) for e in it)
     elif key is True:
         items = it
     else:
         items = ((key(e), e) for e in it)
-    if keep_first is True:
+    if keep_first is None:
         s: set = set()
+        cached: dict = {}
+        add = s.add
+        for k, v in items:
+            if k in s:
+                yield k, v
+            elif k in cached:
+                yield k, cached.pop(k)
+                yield k, v
+                add(k)
+            else:
+                cached[k] = v
+    elif keep_first is True:
+        s = set()
         add = s.add
         for k, v in items:
             if k in s:
                 yield k, v
             else:
                 add(k)
     elif keep_first is False:
```

### Comparing `iter_collect-0.0.1/pyproject.toml` & `iter_collect-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iter_collect"
-version = "0.0.1"
+version = "0.0.2"
 description = "iter_collect."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iter_collect"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iter_collect"
 keywords = ["iterate", "collect"]
```

### Comparing `iter_collect-0.0.1/PKG-INFO` & `iter_collect-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iter_collect
-Version: 0.0.1
+Version: 0.0.2
 Summary: iter_collect.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iter_collect
 License: MIT
 Keywords: iterate,collect
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

