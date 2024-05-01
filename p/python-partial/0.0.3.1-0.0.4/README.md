# Comparing `tmp/python_partial-0.0.3.1.tar.gz` & `tmp/python_partial-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_partial-0.0.3.1.tar", max compression
+gzip compressed data, was "python_partial-0.0.4.tar", max compression
```

## Comparing `python_partial-0.0.3.1.tar` & `python_partial-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.3.1/LICENSE
--rw-r--r--   0        0        0      185 2024-04-29 15:21:28.593758 python_partial-0.0.3.1/partial/__init__.py
--rw-r--r--   0        0        0     5725 2024-04-30 10:56:29.752428 python_partial-0.0.3.1/partial/partial.py
--rwxr-xr-x   0        0        0      849 2024-04-22 15:23:50.704838 python_partial-0.0.3.1/partial/placeholder.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.3.1/partial/py.typed
--rw-r--r--   0        0        0     1176 2024-04-30 10:56:41.377597 python_partial-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0      212 2024-04-22 15:32:04.972596 python_partial-0.0.3.1/readme.md
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 python_partial-0.0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.4/LICENSE
+-rw-r--r--   0        0        0      185 2024-05-01 15:19:19.891864 python_partial-0.0.4/partial/__init__.py
+-rw-r--r--   0        0        0     4123 2024-05-01 15:17:54.496468 python_partial-0.0.4/partial/partial.py
+-rwxr-xr-x   0        0        0      906 2024-05-01 14:51:25.216682 python_partial-0.0.4/partial/placeholder.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.4/partial/py.typed
+-rw-r--r--   0        0        0     1179 2024-05-01 15:20:05.342493 python_partial-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-05-01 15:18:46.197231 python_partial-0.0.4/readme.md
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 python_partial-0.0.4/PKG-INFO
```

### Comparing `python_partial-0.0.3.1/LICENSE` & `python_partial-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_partial-0.0.3.1/partial/placeholder.py` & `python_partial-0.0.4/partial/placeholder.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from __future__ import annotations
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["Placeholder", "_"]
 
 from typing import final, Never
 
+from undefined import undefined
+
 
 @final
 class Placeholder:
     __slots__ = ()
     __instance__: Placeholder
 
     def __new__(cls, /) -> Placeholder:
@@ -21,14 +23,14 @@
             inst = cls.__instance__ = super().__new__(cls)
             return inst
 
     def __init_subclass__(cls, /, **kwargs) -> Never:
         raise TypeError("Subclassing is not allowed")
 
     __bool__ = staticmethod(lambda: False)
-    __eq__ = lambda self, other, /: self is other
+    __eq__ = lambda self, other, /: self is other or other is undefined
     __hash__ = staticmethod(lambda: 0) # type: ignore
     __repr__ = staticmethod(lambda: "_") # type: ignore
 
 
 _ = Placeholder()
```

### Comparing `python_partial-0.0.3.1/pyproject.toml` & `python_partial-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "python-partial"
-version = "0.0.3.1"
-description = "Python partial types."
+version = "0.0.4"
+description = "Python partial."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
-keywords = ["file", "reverse", "iter"]
+keywords = ["partial", "currying", "placeholder"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `python_partial-0.0.3.1/PKG-INFO` & `python_partial-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-partial
-Version: 0.0.3.1
-Summary: Python partial types.
+Version: 0.0.4
+Summary: Python partial.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial
 License: MIT
-Keywords: file,reverse,iter
+Keywords: partial,currying,placeholder
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,23 +21,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: python-undefined
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial
 Description-Content-Type: text/markdown
 
-# Python partial types.
+# Python partial.
 
 ## Installation
 
 You can install from [pypi](https://pypi.org/project/python-partial/)
 
 ```console
 pip install -U python-partial
 ```
 
 ## Usage
 
 ```python
-from partial import ppartial
+from partial import ppartial, currying
 ```
 
+
```

