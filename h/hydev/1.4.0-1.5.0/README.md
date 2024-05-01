# Comparing `tmp/hydev-1.4.0.tar.gz` & `tmp/hydev-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydev-1.4.0.tar", max compression
+gzip compressed data, was "hydev-1.5.0.tar", max compression
```

## Comparing `hydev-1.4.0.tar` & `hydev-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      252 2023-02-27 08:27:16.470934 hydev-1.4.0/LICENSE
--rw-r--r--   0        0        0     2503 2023-12-05 10:37:55.905418 hydev-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       35 2022-12-21 17:54:52.089197 hydev-1.4.0/src/hydev/__init__.py
--rw-r--r--   0        0        0     1779 2022-12-21 17:54:52.089197 hydev-1.4.0/src/hydev/common_pyproject.toml
--rw-r--r--   0        0        0     7828 2023-08-09 19:44:44.227680 hydev-1.4.0/src/hydev/main.py
--rw-r--r--   0        0        0     2920 2023-03-22 13:29:08.269945 hydev-1.4.0/src/hydev/utils.py
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 hydev-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-05-01 07:45:10.622666 hydev-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2503 2024-05-01 07:52:08.452709 hydev-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-05-01 07:45:10.622666 hydev-1.5.0/src/hydev/__init__.py
+-rw-r--r--   0        0        0     1779 2024-05-01 07:45:10.622666 hydev-1.5.0/src/hydev/common_pyproject.toml
+-rw-r--r--   0        0        0     7828 2024-05-01 07:45:10.622666 hydev-1.5.0/src/hydev/main.py
+-rw-r--r--   0        0        0     2920 2024-05-01 07:45:10.622666 hydev-1.5.0/src/hydev/utils.py
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 hydev-1.5.0/PKG-INFO
```

### Comparing `hydev-1.4.0/pyproject.toml` & `hydev-1.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydev"
-version = "1.4.0"
+version = "1.5.0"
 description = "Common tooling and configuration for pythonic development"
 authors = ["hoverhell <hoverhell@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 hydautoflake = "hydev.main:Autoflake.run_cli"
 hydblack = "hydev.main:Black.run_cli"
@@ -14,59 +14,59 @@
 hydisort = "hydev.main:ISort.run_cli"
 hyd = "hydev.main:Fulltest.run_cli"
 hydmypy = "hydev.main:Mypy.run_cli"
 hydpytest = "hydev.main:Pytest.run_cli"
 hydtest = "hydev.main:Fulltest.run_cli"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 # Libs
 click = "^8.1.7"
 pyyaml = "^6.0.1"
 toml = "^0.10.2"
 # Tooling
-poetry = "^1.7.1"
-pre-commit = "^3.5.0"
+poetry = "^1.8.2"
+pre-commit = "^3.7.0"
 # Debug conveniences
 coloredlogs = "^15.0.1"
 ipdb = "^0.13.13"
 # Formatting
-autoflake = "^2.2.1"
-black = "^23.11.0"
-isort = "^5.12.0"
+autoflake = "^2.3.1"
+black = "^24.4.2"
+isort = "^5.13.2"
 # `flake8`
 flake8 = "^6.1.0"
 flake8-broken-line = "^1.0.0"
 flake8-debugger = "^4.1.2"
 flake8-mock-x2 = "^0.4.1"
 flake8-print = "^5.0.0"
-flake8-pytest-style = "^1.7.2"
+flake8-pytest-style = "^2.0.0"
 flake8-use-fstring = "^1.4"
 # `mypy`
-mypy = "^1.7.1"
+mypy = "^1.10.0"
 # `pytest`
-pytest = "^7.4.3"
+pytest = "^8.2.0"
 pytest-asyncio = "^0.23.2"
 pytest-blockage = "^0.2.4"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-env = "^1.1.3"
-pytest-timeout = "^2.2.0"
+pytest-timeout = "^2.3.1"
 # `django`
 django-coverage-plugin = {version = "^3.1.0", optional = true}
-django-debug-toolbar = {version = "^4.2.0", optional = true}
+django-debug-toolbar = {version = "^4.3.0", optional = true}
 django-extra-checks = {version = "^0.13.3", optional = true}
-django-migration-linter = {version = "^5.0.0", optional = true}
+django-migration-linter = {version = "^5.1.0", optional = true}
 django-querycount = {version = "^0.8.3", optional = true}
-django-split-settings = {version = "^1.2.0", optional = true}
-django-stubs = {version = "^4.2.6", optional = true}
-django-stubs-ext = {version = "^4.2.5", optional = true}
+django-split-settings = {version = "^1.3.1", optional = true}
+django-stubs = {version = "^5.0.0", optional = true}
+django-stubs-ext = {version = "^5.0.0", optional = true}
 django-test-migrations = {version = "^1.3.0", optional = true}
 flake8-django = {version = "^1.4", optional = true}
-pytest-django = {version = "^4.7.0", optional = true}
+pytest-django = {version = "^4.8.0", optional = true}
 # ...
 poetry-plugin-up = "^0.7.1"
 
 [tool.poetry.extras]
 django = [
   "django-coverage-plugin",
   "django-debug-toolbar",
```

### Comparing `hydev-1.4.0/src/hydev/common_pyproject.toml` & `hydev-1.5.0/src/hydev/common_pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydev-1.4.0/src/hydev/main.py` & `hydev-1.5.0/src/hydev/main.py`

 * *Files identical despite different names*

### Comparing `hydev-1.4.0/src/hydev/utils.py` & `hydev-1.5.0/src/hydev/utils.py`

 * *Files identical despite different names*

### Comparing `hydev-1.4.0/PKG-INFO` & `hydev-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: hydev
-Version: 1.4.0
+Version: 1.5.0
 Summary: Common tooling and configuration for pythonic development
 License: MIT
 Author: hoverhell
 Author-email: hoverhell@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: django
-Requires-Dist: autoflake (>=2.2.1,<3.0.0)
-Requires-Dist: black (>=23.11.0,<24.0.0)
+Requires-Dist: autoflake (>=2.3.1,<3.0.0)
+Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: django-coverage-plugin (>=3.1.0,<4.0.0) ; extra == "django"
-Requires-Dist: django-debug-toolbar (>=4.2.0,<5.0.0) ; extra == "django"
+Requires-Dist: django-debug-toolbar (>=4.3.0,<5.0.0) ; extra == "django"
 Requires-Dist: django-extra-checks (>=0.13.3,<0.14.0) ; extra == "django"
-Requires-Dist: django-migration-linter (>=5.0.0,<6.0.0) ; extra == "django"
+Requires-Dist: django-migration-linter (>=5.1.0,<6.0.0) ; extra == "django"
 Requires-Dist: django-querycount (>=0.8.3,<0.9.0) ; extra == "django"
-Requires-Dist: django-split-settings (>=1.2.0,<2.0.0) ; extra == "django"
-Requires-Dist: django-stubs (>=4.2.6,<5.0.0) ; extra == "django"
-Requires-Dist: django-stubs-ext (>=4.2.5,<5.0.0) ; extra == "django"
+Requires-Dist: django-split-settings (>=1.3.1,<2.0.0) ; extra == "django"
+Requires-Dist: django-stubs (>=5.0.0,<6.0.0) ; extra == "django"
+Requires-Dist: django-stubs-ext (>=5.0.0,<6.0.0) ; extra == "django"
 Requires-Dist: django-test-migrations (>=1.3.0,<2.0.0) ; extra == "django"
 Requires-Dist: flake8 (>=6.1.0,<7.0.0)
 Requires-Dist: flake8-broken-line (>=1.0.0,<2.0.0)
 Requires-Dist: flake8-debugger (>=4.1.2,<5.0.0)
 Requires-Dist: flake8-django (>=1.4,<2.0) ; extra == "django"
 Requires-Dist: flake8-mock-x2 (>=0.4.1,<0.5.0)
 Requires-Dist: flake8-print (>=5.0.0,<6.0.0)
-Requires-Dist: flake8-pytest-style (>=1.7.2,<2.0.0)
+Requires-Dist: flake8-pytest-style (>=2.0.0,<3.0.0)
 Requires-Dist: flake8-use-fstring (>=1.4,<2.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
-Requires-Dist: isort (>=5.12.0,<6.0.0)
-Requires-Dist: mypy (>=1.7.1,<2.0.0)
-Requires-Dist: poetry (>=1.7.1,<2.0.0)
+Requires-Dist: isort (>=5.13.2,<6.0.0)
+Requires-Dist: mypy (>=1.10.0,<2.0.0)
+Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: poetry-plugin-up (>=0.7.1,<0.8.0)
-Requires-Dist: pre-commit (>=3.5.0,<4.0.0)
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
+Requires-Dist: pre-commit (>=3.7.0,<4.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
 Requires-Dist: pytest-blockage (>=0.2.4,<0.3.0)
-Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
+Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytest-deadfixtures (>=2.2.1,<3.0.0)
-Requires-Dist: pytest-django (>=4.7.0,<5.0.0) ; extra == "django"
+Requires-Dist: pytest-django (>=4.8.0,<5.0.0) ; extra == "django"
 Requires-Dist: pytest-env (>=1.1.3,<2.0.0)
-Requires-Dist: pytest-timeout (>=2.2.0,<3.0.0)
+Requires-Dist: pytest-timeout (>=2.3.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

