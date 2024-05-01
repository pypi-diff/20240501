# Comparing `tmp/python_decorator-0.0.2.tar.gz` & `tmp/python_decorator-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_decorator-0.0.2.tar", max compression
+gzip compressed data, was "python_decorator-0.0.2.1.tar", max compression
```

## Comparing `python_decorator-0.0.2.tar` & `python_decorator-0.0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     8754 2024-04-30 13:16:34.567545 python_decorator-0.0.2/decorator0/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.2/decorator0/py.typed
--rwxr-xr-x   0        0        0     2527 2024-04-30 13:16:09.363535 python_decorator-0.0.2/decorator0/util.py
--rw-r--r--   0        0        0     1204 2024-04-30 13:16:24.878498 python_decorator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      201 2024-04-24 15:56:16.540240 python_decorator-0.0.2/readme.md
--rw-r--r--   0        0        0     1399 1970-01-01 00:00:00.000000 python_decorator-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     8913 2024-05-01 15:26:45.609821 python_decorator-0.0.2.1/decorator0/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.2.1/decorator0/py.typed
+-rwxr-xr-x   0        0        0     3102 2024-05-01 15:31:09.258372 python_decorator-0.0.2.1/decorator0/util.py
+-rw-r--r--   0        0        0     1193 2024-05-01 15:23:38.720958 python_decorator-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-01 15:23:48.559855 python_decorator-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 python_decorator-0.0.2.1/PKG-INFO
```

### Comparing `python_decorator-0.0.2/LICENSE` & `python_decorator-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_decorator-0.0.2/decorator0/__init__.py` & `python_decorator-0.0.2.1/decorator0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,34 @@
 """
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
 __version__ = (0, 0, 2)
 __all__ = ["decorated", "optional", "optional_args", "currying", "partialize"]
 
 from collections.abc import Callable
-from functools import partial, reduce, update_wrapper
+from functools import partial, reduce, update_wrapper as _update_wrapper
 from inspect import signature
 from typing import cast, overload, Any, Concatenate, Optional, ParamSpec, TypeVar
 
 from partial import ppartial
 from undefined import undefined
 
 
 Args = ParamSpec("Args")
 Args0 = ParamSpec("Args0")
 R = TypeVar("R")
 
 
+def update_wrapper(f, g, /, *args, **kwds):
+    if f is g:
+        return f
+    else:
+        return _update_wrapper(f, g, *args, **kwds)
+
+
 def decorated(
     f: Callable[Concatenate[Callable[Args, R], Args], R], 
     /, 
 ) -> Callable[[Callable[Args, R]], Callable[Args, R]]:
     """Transform the 2-layers decorator into 1-layer.
 
     @decorated
```

### Comparing `python_decorator-0.0.2/decorator0/util.py` & `python_decorator-0.0.2.1/decorator0/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["suppressed", "threaded", "timethis", "with_lock"]
+__all__ = ["suppressed", "threaded", "timethis", "with_lock", "with_cm"]
 
 from _thread import start_new_thread
 from asyncio import Lock as AsyncLock
 from concurrent.futures import Future
 from inspect import isawaitable, iscoroutinefunction
 from threading import Lock
 from time import perf_counter
+from typing import AsyncContextManager
 
 from undefined import undefined
 from . import decorated, optional
 
 
 @optional
 def suppressed(
@@ -86,7 +87,26 @@
         if lock is None:
             lock = Lock()
         async def wrapper(*args, **kwds):
             with lock:
                 return func(*args, **kwds)
     return wrapper
 
+
+@optional
+def with_cm(func, /, cm=None):
+    if cm is None:
+        return func
+    if iscoroutinefunction(func):
+        async def wrapper(*args, **kwds):
+            if isinstance(cm, AsyncContextManager):
+                async with cm:
+                    return await func(*args, **kwds)
+            else:
+                with cm:
+                    return await func(*args, **kwds)
+    else:
+        async def wrapper(*args, **kwds):
+            with cm:
+                return func(*args, **kwds)
+    return wrapper
+
```

### Comparing `python_decorator-0.0.2/pyproject.toml` & `python_decorator-0.0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "python-decorator"
-version = "0.0.2"
-description = "Python argument type."
+version = "0.0.2.1"
+description = "Python decorator."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
-keywords = ["file", "reverse", "iter"]
+keywords = ["decorator"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
@@ -23,15 +23,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-partial = "*"
+python-partial = "^0.0.4"
 python-undefined = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
```

### Comparing `python_decorator-0.0.2/PKG-INFO` & `python_decorator-0.0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-decorator
-Version: 0.0.2
-Summary: Python argument type.
+Version: 0.0.2.1
+Summary: Python decorator.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 License: MIT
-Keywords: file,reverse,iter
+Keywords: decorator
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: python-partial
+Requires-Dist: python-partial (>=0.0.4,<0.0.5)
 Requires-Dist: python-undefined
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 Description-Content-Type: text/markdown
 
 # Python decorator.
 
 ## Installation
```

