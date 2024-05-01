# Comparing `tmp/flask_super-0.2.6.tar.gz` & `tmp/flask_super-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_super-0.2.6.tar", max compression
+gzip compressed data, was "flask_super-0.2.7.tar", max compression
```

## Comparing `flask_super-0.2.6.tar` & `flask_super-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      583 2023-12-22 09:35:29.655002 flask_super-0.2.6/LICENSE
--rw-r--r--   0        0        0     3528 2024-01-23 08:18:35.284502 flask_super-0.2.6/README.md
--rw-r--r--   0        0        0     2829 2024-02-01 10:51:15.883619 flask_super-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      439 2024-01-04 14:33:21.423046 flask_super-0.2.6/src/flask_super/__init__.py
--rw-r--r--   0        0        0      882 2024-01-02 15:01:49.932857 flask_super-0.2.6/src/flask_super/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-12-22 10:48:27.656702 flask_super-0.2.6/src/flask_super/cli/commands/__init__.py
--rw-r--r--   0        0        0      722 2024-01-03 15:07:53.485191 flask_super-0.2.6/src/flask_super/cli/commands/config.py
--rw-r--r--   0        0        0     1790 2024-01-02 15:01:49.930837 flask_super-0.2.6/src/flask_super/cli/commands/inspect.py
--rw-r--r--   0        0        0      278 2024-01-02 12:32:58.764162 flask_super-0.2.6/src/flask_super/decorators.py
--rw-r--r--   0        0        0       62 2024-01-04 15:06:57.860423 flask_super-0.2.6/src/flask_super/initializers/__init__.py
--rw-r--r--   0        0        0     1218 2024-01-19 10:33:47.487018 flask_super-0.2.6/src/flask_super/initializers/logging.py
--rw-r--r--   0        0        0     2377 2024-01-03 19:10:11.780615 flask_super-0.2.6/src/flask_super/registry.py
--rw-r--r--   0        0        0      964 2024-01-19 15:20:48.074087 flask_super-0.2.6/src/flask_super/scanner.py
--rw-r--r--   0        0        0     1374 2024-01-03 19:10:11.773962 flask_super-0.2.6/src/flask_super/services.py
--rw-r--r--   0        0        0       41 2024-01-02 15:02:14.469401 flask_super-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      302 2024-01-02 15:37:23.851128 flask_super-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0      527 2024-01-03 15:16:19.378664 flask_super-0.2.6/tests/test_cli.py
--rw-r--r--   0        0        0     1266 2024-01-02 15:02:14.467108 flask_super-0.2.6/tests/test_services.py
--rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 flask_super-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      151 2023-12-22 09:35:29.665803 flask_super-0.2.7/AUTHORS.rst
+-rw-r--r--   0        0        0      583 2023-12-22 09:35:29.655002 flask_super-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3528 2024-01-23 08:18:35.284502 flask_super-0.2.7/README.md
+-rw-r--r--   0        0        0     2826 2024-05-01 14:09:07.830239 flask_super-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      439 2024-05-01 14:05:06.793428 flask_super-0.2.7/src/flask_super/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-01 14:05:06.793439 flask_super-0.2.7/src/flask_super/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-22 10:48:27.656702 flask_super-0.2.7/src/flask_super/cli/commands/__init__.py
+-rw-r--r--   0        0        0      722 2024-01-03 15:07:53.485191 flask_super-0.2.7/src/flask_super/cli/commands/config.py
+-rw-r--r--   0        0        0     1790 2024-01-02 15:01:49.930837 flask_super-0.2.7/src/flask_super/cli/commands/inspect.py
+-rw-r--r--   0        0        0      278 2024-05-01 14:05:06.793428 flask_super-0.2.7/src/flask_super/decorators.py
+-rw-r--r--   0        0        0       62 2024-01-04 15:06:57.860423 flask_super-0.2.7/src/flask_super/initializers/__init__.py
+-rw-r--r--   0        0        0     1218 2024-01-19 10:33:47.487018 flask_super-0.2.7/src/flask_super/initializers/logging.py
+-rw-r--r--   0        0        0     2377 2024-05-01 14:05:06.793724 flask_super-0.2.7/src/flask_super/registry.py
+-rw-r--r--   0        0        0      964 2024-01-19 15:20:48.074087 flask_super-0.2.7/src/flask_super/scanner.py
+-rw-r--r--   0        0        0     1374 2024-01-03 19:10:11.773962 flask_super-0.2.7/src/flask_super/services.py
+-rw-r--r--   0        0        0       41 2024-01-02 15:02:14.469401 flask_super-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0      302 2024-01-02 15:37:23.851128 flask_super-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0      527 2024-01-03 15:16:19.378664 flask_super-0.2.7/tests/test_cli.py
+-rw-r--r--   0        0        0     1266 2024-01-02 15:02:14.467108 flask_super-0.2.7/tests/test_services.py
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 flask_super-0.2.7/PKG-INFO
```

### Comparing `flask_super-0.2.6/LICENSE` & `flask_super-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/README.md` & `flask_super-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/pyproject.toml` & `flask_super-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Flask-Super"
-version = "0.2.6"
+version = "0.2.7"
 homepage = "https://github.com/abilian/flask-super"
 description = "Patterns and idioms for Flask applications."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.md"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -21,28 +21,28 @@
 
 [tool.poetry.dependencies]
 # We're uing pattern matching, so we need Python >=3.10
 python = ">=3.10,<4"
 
 flask = "^3.0.0"
 svcs = "^24.1.0"
-sentry-sdk = "^1.39.1"
+sentry-sdk = "^2"
 loguru = "^0.7.2"
 
 
 [tool.poetry.group.dev.dependencies]
 ## Standard cruft
 abilian-devtools = ">=0.5.16"
 
 # Cruft (project templates management)
 cruft = "*"
 toml = "*"
 
 ## /standard cruft
-pyanalyze = "^0.11.0"
+# pyanalyze = "^0.11.0"
 devtools = "^0.12.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # ---
```

### Comparing `flask_super-0.2.6/src/flask_super/cli/__init__.py` & `flask_super-0.2.7/src/flask_super/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import click
 
 from flask_super.registry import lookup, register
 
-__all__ = ["register_commands", "command", "group"]
+__all__ = ["command", "group", "register_commands"]
 
 from flask_super.scanner import scan_package
 
 
 def command(*args, **kwargs):
     def decorator(func):
         module = func.__module__
```

### Comparing `flask_super-0.2.6/src/flask_super/cli/commands/config.py` & `flask_super-0.2.7/src/flask_super/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/src/flask_super/cli/commands/inspect.py` & `flask_super-0.2.7/src/flask_super/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/src/flask_super/initializers/logging.py` & `flask_super-0.2.7/src/flask_super/initializers/logging.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/src/flask_super/registry.py` & `flask_super-0.2.7/src/flask_super/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Any
 
 from attr import field, frozen
 
-__all__ = ["registry", "register", "lookup"]
+__all__ = ["lookup", "register", "registry"]
 
 
 @frozen
 class Metadata:
     name: str = ""
     module: str = ""
     tag: str = ""
```

### Comparing `flask_super-0.2.6/src/flask_super/scanner.py` & `flask_super-0.2.7/src/flask_super/scanner.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/src/flask_super/services.py` & `flask_super-0.2.7/src/flask_super/services.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/tests/test_cli.py` & `flask_super-0.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/tests/test_services.py` & `flask_super-0.2.7/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `flask_super-0.2.6/PKG-INFO` & `flask_super-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Flask-Super
-Version: 0.2.6
+Version: 0.2.7
 Summary: Patterns and idioms for Flask applications.
 Home-page: https://github.com/abilian/flask-super
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flask (>=3.0.0,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: sentry-sdk (>=1.39.1,<2.0.0)
+Requires-Dist: sentry-sdk (>=2,<3)
 Requires-Dist: svcs (>=24.1.0,<25.0.0)
 Description-Content-Type: text/markdown
 
 # Flask-Super
 
 [![image](https://img.shields.io/pypi/v/flask_super.svg)](https://pypi.python.org/pypi/flask_super)
```

