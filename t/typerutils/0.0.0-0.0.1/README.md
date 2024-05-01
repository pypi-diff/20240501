# Comparing `tmp/typerutils-0.0.0.tar.gz` & `tmp/typerutils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerutils-0.0.0.tar", last modified: Fri Apr 26 22:51:02 2024, max compression
+gzip compressed data, was "typerutils-0.0.1.tar", last modified: Wed May  1 20:11:17 2024, max compression
```

## Comparing `typerutils-0.0.0.tar` & `typerutils-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 22:51:02.582988 typerutils-0.0.0/
--rw-r--r--   0 alex      (1000) alex      (1001)     1073 2024-04-23 20:54:27.000000 typerutils-0.0.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)     1607 2024-04-26 22:51:02.582988 typerutils-0.0.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      513 2024-04-26 22:50:28.000000 typerutils-0.0.0/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)     1361 2024-04-26 21:26:52.000000 typerutils-0.0.0/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-04-26 22:51:02.582988 typerutils-0.0.0/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 22:51:02.579655 typerutils-0.0.0/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 22:51:02.582988 typerutils-0.0.0/src/typerutils/
--rw-r--r--   0 alex      (1000) alex      (1001)      209 2024-04-26 21:24:35.000000 typerutils-0.0.0/src/typerutils/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)      409 2024-04-26 21:24:43.000000 typerutils-0.0.0/src/typerutils/create_app.py
--rw-r--r--   0 alex      (1000) alex      (1001)      200 2024-04-26 21:24:51.000000 typerutils-0.0.0/src/typerutils/groups.py
--rw-r--r--   0 alex      (1000) alex      (1001)      783 2024-04-26 21:24:59.000000 typerutils-0.0.0/src/typerutils/log_level.py
--rw-r--r--   0 alex      (1000) alex      (1001)       37 2024-04-26 21:25:43.000000 typerutils-0.0.0/src/typerutils/test_groups.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-26 22:51:02.582988 typerutils-0.0.0/src/typerutils.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     1607 2024-04-26 22:51:02.000000 typerutils-0.0.0/src/typerutils.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      360 2024-04-26 22:51:02.000000 typerutils-0.0.0/src/typerutils.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-04-26 22:51:02.000000 typerutils-0.0.0/src/typerutils.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)      234 2024-04-26 22:51:02.000000 typerutils-0.0.0/src/typerutils.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       11 2024-04-26 22:51:02.000000 typerutils-0.0.0/src/typerutils.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-01 20:11:17.570950 typerutils-0.0.1/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1073 2024-04-23 20:54:27.000000 typerutils-0.0.1/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-01 20:03:49.000000 typerutils-0.0.1/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1001)     1565 2024-05-01 20:11:17.570950 typerutils-0.0.1/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      533 2024-04-30 22:22:51.000000 typerutils-0.0.1/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)        6 2024-05-01 20:09:01.000000 typerutils-0.0.1/VERSION
+-rw-r--r--   0 alex      (1000) alex      (1001)     1325 2024-04-30 22:22:51.000000 typerutils-0.0.1/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-01 20:11:17.570950 typerutils-0.0.1/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-01 20:11:17.567617 typerutils-0.0.1/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-01 20:11:17.570950 typerutils-0.0.1/src/typerutils/
+-rw-r--r--   0 alex      (1000) alex      (1001)      209 2024-05-01 00:10:51.000000 typerutils-0.0.1/src/typerutils/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      744 2024-05-01 20:03:49.000000 typerutils-0.0.1/src/typerutils/create_app.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      186 2024-05-01 20:03:49.000000 typerutils-0.0.1/src/typerutils/groups.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      783 2024-04-26 21:24:59.000000 typerutils-0.0.1/src/typerutils/log_level.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      221 2024-05-01 20:03:49.000000 typerutils-0.0.1/src/typerutils/testing.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-01 20:11:17.570950 typerutils-0.0.1/src/typerutils.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1565 2024-05-01 20:11:17.000000 typerutils-0.0.1/src/typerutils.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      376 2024-05-01 20:11:17.000000 typerutils-0.0.1/src/typerutils.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-01 20:11:17.000000 typerutils-0.0.1/src/typerutils.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)      204 2024-05-01 20:11:17.000000 typerutils-0.0.1/src/typerutils.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       11 2024-05-01 20:11:17.000000 typerutils-0.0.1/src/typerutils.egg-info/top_level.txt
```

### Comparing `typerutils-0.0.0/LICENSE` & `typerutils-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typerutils-0.0.0/PKG-INFO` & `typerutils-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: typerutils
-Version: 0.0.0
+Version: 0.0.1
 Summary: Typer utility helpers
 Author-email: Alex Kwiatkowski <alex+pypi@fremantle.io>
 Project-URL: Homepage, https://github.com/rupurt/typerutils
 Project-URL: Issues, https://github.com/rupurt/typerutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer[all]~=0.9.0
+Requires-Dist: typer>=0.9.0
 Provides-Extra: test
 Requires-Dist: build>=1.2.1; extra == "test"
 Requires-Dist: twine>=5.0.0; extra == "test"
 Requires-Dist: ruff>=0.3.4; extra == "test"
 Requires-Dist: pip-tools>=7.4.1; extra == "test"
 Requires-Dist: pygments>=2.17.0; extra == "test"
 Requires-Dist: pyhamcrest>=2.1.0; extra == "test"
 Requires-Dist: pyright>=1.1.0; extra == "test"
 Requires-Dist: pytest>=8.1.0; extra == "test"
 Requires-Dist: pytest-cov>=5.0.0; extra == "test"
-Requires-Dist: pytest-recording>=0.13.1; extra == "test"
 Requires-Dist: pytest-unordered>=0.6.0; extra == "test"
 Requires-Dist: pytest-watcher>=0.4.0; extra == "test"
 
 # typerutils
 
-Typer utility helpers
+[Typer](https://typer.tiangolo.com/) utility helpers
 
 ## Usage
 
 Install the package from pypi
 
 ```console
 > pip install typerutils
@@ -52,13 +51,13 @@
 ```shell
 > make test
 ```
 
 ## Publish Package to PyPi
 
 ```shell
-> make distribution
+> make pypi
 ```
 
 ## License
 
-`pydanticutils` is released under the [MIT license](./LICENSE)
+`typerutils` is released under the [MIT license](./LICENSE)
```

### Comparing `typerutils-0.0.0/README.md` & `typerutils-0.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # typerutils
 
-Typer utility helpers
+[Typer](https://typer.tiangolo.com/) utility helpers
 
 ## Usage
 
 Install the package from pypi
 
 ```console
 > pip install typerutils
@@ -25,13 +25,13 @@
 ```shell
 > make test
 ```
 
 ## Publish Package to PyPi
 
 ```shell
-> make distribution
+> make pypi
 ```
 
 ## License
 
-`pydanticutils` is released under the [MIT license](./LICENSE)
+`typerutils` is released under the [MIT license](./LICENSE)
```

### Comparing `typerutils-0.0.0/pyproject.toml` & `typerutils-0.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 readme = "README.md"
 requires-python = ">= 3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent"
 ]
 dependencies = [
-  "typer[all] ~=0.9.0",
+  "typer >=0.9.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/rupurt/typerutils"
 Issues = "https://github.com/rupurt/typerutils/issues"
 
 [project.optional-dependencies]
@@ -32,15 +32,14 @@
   "ruff >=0.3.4",
   "pip-tools >=7.4.1",
   "pygments >=2.17.0",
   "pyhamcrest >=2.1.0",
   "pyright >=1.1.0",
   "pytest >=8.1.0",
   "pytest-cov >=5.0.0",
-  "pytest-recording >=0.13.1",
   "pytest-unordered >=0.6.0",
   "pytest-watcher >=0.4.0",
 ]
 
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
```

### Comparing `typerutils-0.0.0/src/typerutils/log_level.py` & `typerutils-0.0.1/src/typerutils/log_level.py`

 * *Files identical despite different names*

### Comparing `typerutils-0.0.0/src/typerutils.egg-info/PKG-INFO` & `typerutils-0.0.1/src/typerutils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: typerutils
-Version: 0.0.0
+Version: 0.0.1
 Summary: Typer utility helpers
 Author-email: Alex Kwiatkowski <alex+pypi@fremantle.io>
 Project-URL: Homepage, https://github.com/rupurt/typerutils
 Project-URL: Issues, https://github.com/rupurt/typerutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer[all]~=0.9.0
+Requires-Dist: typer>=0.9.0
 Provides-Extra: test
 Requires-Dist: build>=1.2.1; extra == "test"
 Requires-Dist: twine>=5.0.0; extra == "test"
 Requires-Dist: ruff>=0.3.4; extra == "test"
 Requires-Dist: pip-tools>=7.4.1; extra == "test"
 Requires-Dist: pygments>=2.17.0; extra == "test"
 Requires-Dist: pyhamcrest>=2.1.0; extra == "test"
 Requires-Dist: pyright>=1.1.0; extra == "test"
 Requires-Dist: pytest>=8.1.0; extra == "test"
 Requires-Dist: pytest-cov>=5.0.0; extra == "test"
-Requires-Dist: pytest-recording>=0.13.1; extra == "test"
 Requires-Dist: pytest-unordered>=0.6.0; extra == "test"
 Requires-Dist: pytest-watcher>=0.4.0; extra == "test"
 
 # typerutils
 
-Typer utility helpers
+[Typer](https://typer.tiangolo.com/) utility helpers
 
 ## Usage
 
 Install the package from pypi
 
 ```console
 > pip install typerutils
@@ -52,13 +51,13 @@
 ```shell
 > make test
 ```
 
 ## Publish Package to PyPi
 
 ```shell
-> make distribution
+> make pypi
 ```
 
 ## License
 
-`pydanticutils` is released under the [MIT license](./LICENSE)
+`typerutils` is released under the [MIT license](./LICENSE)
```

