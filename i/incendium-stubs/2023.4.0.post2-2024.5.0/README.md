# Comparing `tmp/incendium-stubs-2023.4.0.post2.tar.gz` & `tmp/incendium_stubs-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incendium-stubs-2023.4.0.post2.tar", last modified: Thu Feb 22 18:34:32 2024, max compression
+gzip compressed data, was "incendium_stubs-2024.5.0.tar", last modified: Wed May  1 08:04:06 2024, max compression
```

## Comparing `incendium-stubs-2023.4.0.post2.tar` & `incendium_stubs-2024.5.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.071769 incendium-stubs-2023.4.0.post2/
--rw-rw-r--   0 root         (0) root         (0)     1070 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4823 2024-02-22 18:34:32.071769 incendium-stubs-2023.4.0.post2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2116 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/README.md
--rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 18:34:32.071769 incendium-stubs-2023.4.0.post2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.067769 incendium-stubs-2023.4.0.post2/stubs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.067769 incendium-stubs-2023.4.0.post2/stubs/incendium/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)      619 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/constants.pyi
--rw-rw-r--   0 root         (0) root         (0)      832 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/dataset.pyi
--rw-rw-r--   0 root         (0) root         (0)      183 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/date.pyi
--rw-rw-r--   0 root         (0) root         (0)     2579 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/db.pyi
--rw-rw-r--   0 root         (0) root         (0)      508 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/exceptions.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.067769 incendium-stubs-2023.4.0.post2/stubs/incendium/helper/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/helper/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/helper/py.typed
--rw-rw-r--   0 root         (0) root         (0)      320 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/helper/types.pyi
--rw-rw-r--   0 root         (0) root         (0)      395 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/net.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/py.typed
--rw-rw-r--   0 root         (0) root         (0)      259 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/tag.pyi
--rw-rw-r--   0 root         (0) root         (0)     1227 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/user.pyi
--rw-rw-r--   0 root         (0) root         (0)      561 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/util.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/version.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.071769 incendium-stubs-2023.4.0.post2/stubs/incendium/vision/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/vision/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)     1011 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/vision/gui.pyi
--rw-rw-r--   0 root         (0) root         (0)      276 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/vision/nav.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-22 18:32:19.000000 incendium-stubs-2023.4.0.post2/stubs/incendium/vision/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:34:32.071769 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4823 2024-02-22 18:34:32.000000 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2024-02-22 18:34:32.000000 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 18:34:32.000000 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-22 18:34:32.000000 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-22 18:34:32.000000 incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.161965 incendium_stubs-2024.5.0/
+-rw-rw-r--   0 root         (0) root         (0)     1070 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4773 2024-05-01 08:04:06.161965 incendium_stubs-2024.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2118 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1557 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 08:04:06.161965 incendium_stubs-2024.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.153965 incendium_stubs-2024.5.0/stubs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.157965 incendium_stubs-2024.5.0/stubs/incendium/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/__version__.pyi
+-rw-rw-r--   0 root         (0) root         (0)      670 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/constants.pyi
+-rw-rw-r--   0 root         (0) root         (0)      832 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/dataset.pyi
+-rw-rw-r--   0 root         (0) root         (0)      183 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/date.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2579 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/db.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1048 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/exceptions.pyi
+-rw-rw-r--   0 root         (0) root         (0)      299 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/gui.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.157965 incendium_stubs-2024.5.0/stubs/incendium/helper/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/helper/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/helper/py.typed
+-rw-rw-r--   0 root         (0) root         (0)      320 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/helper/types.pyi
+-rw-rw-r--   0 root         (0) root         (0)       91 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/l10n.pyi
+-rw-rw-r--   0 root         (0) root         (0)      395 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/net.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/py.typed
+-rw-rw-r--   0 root         (0) root         (0)      259 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/tag.pyi
+-rw-rw-r--   0 root         (0) root         (0)      195 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/time.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1227 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/user.pyi
+-rw-rw-r--   0 root         (0) root         (0)      561 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/util.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/version.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.157965 incendium_stubs-2024.5.0/stubs/incendium/vision/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/vision/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1187 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/vision/gui.pyi
+-rw-rw-r--   0 root         (0) root         (0)      276 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/vision/nav.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-01 08:02:15.000000 incendium_stubs-2024.5.0/stubs/incendium/vision/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 08:04:06.161965 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4773 2024-05-01 08:04:06.000000 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      910 2024-05-01 08:04:06.000000 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 08:04:06.000000 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-01 08:04:06.000000 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-01 08:04:06.000000 incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/top_level.txt
```

### Comparing `incendium-stubs-2023.4.0.post2/LICENSE` & `incendium_stubs-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.4.0.post2/PKG-INFO` & `incendium_stubs-2024.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: incendium-stubs
-Version: 2023.4.0.post2
+Version: 2024.5.0
 Summary: incendium stubs package
-Author-email: César Román <cesar@thecesrom.dev>
+Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,18 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Funding, https://github.com/sponsors/thecesrom
-Project-URL: Homepage, https://thecesrom.dev/incendium-stubs
-Project-URL: Source, https://github.com/thecesrom/incendium-stubs
-Project-URL: Tracker, https://github.com/thecesrom/incendium-stubs/issues
+Project-URL: Funding, https://github.com/sponsors/cesarcoatl
+Project-URL: Source, https://github.com/ignition-incendium/incendium-stubs
+Project-URL: Tracker, https://github.com/ignition-incendium/incendium-stubs/issues
 Keywords: hmi,ignition,inductive automation,scada
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -52,25 +51,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ignition-api-stubs>=8.1
 
 # incendium-stubs
 
 <!--- Badges --->
-![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/thecesrom/incendium-stubs/main)
-[![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
+![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/cesarcoatl/incendium-stubs/main)
+[![GitHub contributors](https://img.shields.io/github/contributors/cesarcoatl/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
 [![Downloads](https://pepy.tech/badge/incendium-stubs)](https://pepy.tech/project/incendium-stubs)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ignition-incendium/stubs/main.svg)](https://results.pre-commit.ci/latest/github/ignition-incendium/stubs/main)
 [![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-incendium/incendium/discussions)
 
 This package contains a collection of [stubs](https://www.python.org/dev/peps/pep-484/) for [`ignition-incendium/incendium`](https://github.com/ignition-incendium/incendium). These files were generated using `mypy`'s [`stubgen`](https://coatl-mypy.readthedocs.io/en/v0.971/stubgen.html).
 
 ## Installation and usage
 
-To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.11.
+To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.12.
 
 ```sh
 python -m pip install incendium-stubs
 ```
 
 To run `mypy` against your code, execute the following command passing the source directory (typically `src`) or a single file:
```

### Comparing `incendium-stubs-2023.4.0.post2/README.md` & `incendium_stubs-2024.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # incendium-stubs
 
 <!--- Badges --->
-![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/thecesrom/incendium-stubs/main)
-[![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
+![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/cesarcoatl/incendium-stubs/main)
+[![GitHub contributors](https://img.shields.io/github/contributors/cesarcoatl/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
 [![Downloads](https://pepy.tech/badge/incendium-stubs)](https://pepy.tech/project/incendium-stubs)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ignition-incendium/stubs/main.svg)](https://results.pre-commit.ci/latest/github/ignition-incendium/stubs/main)
 [![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-incendium/incendium/discussions)
 
 This package contains a collection of [stubs](https://www.python.org/dev/peps/pep-484/) for [`ignition-incendium/incendium`](https://github.com/ignition-incendium/incendium). These files were generated using `mypy`'s [`stubgen`](https://coatl-mypy.readthedocs.io/en/v0.971/stubgen.html).
 
 ## Installation and usage
 
-To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.11.
+To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.12.
 
 ```sh
 python -m pip install incendium-stubs
 ```
 
 To run `mypy` against your code, execute the following command passing the source directory (typically `src`) or a single file:
```

### Comparing `incendium-stubs-2023.4.0.post2/pyproject.toml` & `incendium_stubs-2024.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "incendium-stubs"
-version = "2023.4.0.post2"
+version = "2024.5.0"
 description = "incendium stubs package"
 readme = "README.md"
 keywords = [
   "hmi",
   "ignition",
   "inductive automation",
   "scada",
 ]
 license = {file = "LICENSE"}
-authors = [{name = "César Román", email = "cesar@thecesrom.dev"}]
+authors = [{name = "César Román", email = "cesar@coatl.dev"}]
 requires-python = ">=3.7, <3.13"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: Manufacturing",
   "License :: OSI Approved :: MIT License",
@@ -38,18 +38,17 @@
   "Typing :: Stubs Only",
   "Typing :: Typed",
 ]
 dependencies = [
   "ignition-api-stubs>=8.1",
 ]
 [project.urls]
-Funding = "https://github.com/sponsors/thecesrom"
-Homepage = "https://thecesrom.dev/incendium-stubs"
-Source = "https://github.com/thecesrom/incendium-stubs"
-Tracker = "https://github.com/thecesrom/incendium-stubs/issues"
+Funding = "https://github.com/sponsors/cesarcoatl"
+Source = "https://github.com/ignition-incendium/incendium-stubs"
+Tracker = "https://github.com/ignition-incendium/incendium-stubs/issues"
 
 [tool.setuptools]
 include-package-data = true
 package-dir = {"" = "stubs"}
 
 [tool.setuptools.package-data]
 "*" = ["*.pyi", "py.typed"]
```

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/constants.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/constants.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -23,7 +23,9 @@
 PROCEED_WITH_SAVING_CHANGES: str
 PROCEED_WITHOUT_SAVING_CHANGES: str
 SUCCESS_WINDOW_TITLE: str
 TABBED_LINE: str
 UNEXPECTED_ERROR: str
 UNEXPECTED_ERROR_CAUSED_BY: str
 WARNING_WINDOW_TITLE: str
+GATEWAY_EXCEPTION: str
+MSSQL_SERVER_EXCEPTION: str
```

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/dataset.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/dataset.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/db.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/db.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/user.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/user.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/util.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/util.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Optional, Tuple, Union
 
 from incendium.helper.types import AnyStr, Number
 from incendium.user import IncendiumUser
 from java.util import Date
 
 def get_function_name() -> AnyStr: ...
-def get_timestamp(value: int) -> AnyStr: ...
 def get_timer(date: Union[Date, long]) -> AnyStr: ...
+def get_timestamp(value: int) -> AnyStr: ...
 def set_locale(user: IncendiumUser) -> None: ...
 def validate_form(
     strings: Optional[Dict[AnyStr, AnyStr]] = ...,
     numbers: Optional[Dict[AnyStr, Number]] = ...,
     collections: Optional[Dict[AnyStr, Number]] = ...,
 ) -> Tuple[bool, AnyStr]: ...
```

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium/vision/gui.pyi` & `incendium_stubs-2024.5.0/stubs/incendium/vision/gui.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -13,17 +13,26 @@
 CURSOR_N_RESIZE: int
 CURSOR_S_RESIZE: int
 CURSOR_W_RESIZE: int
 CURSOR_E_RESIZE: int
 CURSOR_HAND: int
 CURSOR_MOVE: int
 
-def authentication(auth_profile: AnyStr = ..., title: AnyStr = ...) -> bool: ...
+def authentication(
+    auth_profile: AnyStr = ...,
+    title: AnyStr = ...,
+    username_label_text: AnyStr = ...,
+    password_label_text: AnyStr = ...,
+) -> bool: ...
 def authorization(
-    role: AnyStr, auth_profile: AnyStr = ..., title: AnyStr = ...
+    role: AnyStr,
+    auth_profile: AnyStr = ...,
+    title: AnyStr = ...,
+    username_label_text: AnyStr = ...,
+    password_label_text: AnyStr = ...,
 ) -> bool: ...
 def confirm(
     message: AnyStr, title: AnyStr = ..., show_cancel: bool = ...
 ) -> Optional[bool]: ...
 def error(
     message: AnyStr, title: AnyStr = ..., detail: Optional[AnyStr] = ...
 ) -> None: ...
```

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/PKG-INFO` & `incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: incendium-stubs
-Version: 2023.4.0.post2
+Version: 2024.5.0
 Summary: incendium stubs package
-Author-email: César Román <cesar@thecesrom.dev>
+Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,18 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Funding, https://github.com/sponsors/thecesrom
-Project-URL: Homepage, https://thecesrom.dev/incendium-stubs
-Project-URL: Source, https://github.com/thecesrom/incendium-stubs
-Project-URL: Tracker, https://github.com/thecesrom/incendium-stubs/issues
+Project-URL: Funding, https://github.com/sponsors/cesarcoatl
+Project-URL: Source, https://github.com/ignition-incendium/incendium-stubs
+Project-URL: Tracker, https://github.com/ignition-incendium/incendium-stubs/issues
 Keywords: hmi,ignition,inductive automation,scada
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -52,25 +51,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ignition-api-stubs>=8.1
 
 # incendium-stubs
 
 <!--- Badges --->
-![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/thecesrom/incendium-stubs/main)
-[![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
+![GitHub last commit (stubs)](https://img.shields.io/github/last-commit/cesarcoatl/incendium-stubs/main)
+[![GitHub contributors](https://img.shields.io/github/contributors/cesarcoatl/incendium-stubs)](https://github.com/ignition-incendium/incendium-stubs/graphs/contributors)
 [![Downloads](https://pepy.tech/badge/incendium-stubs)](https://pepy.tech/project/incendium-stubs)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ignition-incendium/stubs/main.svg)](https://results.pre-commit.ci/latest/github/ignition-incendium/stubs/main)
 [![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-incendium/incendium/discussions)
 
 This package contains a collection of [stubs](https://www.python.org/dev/peps/pep-484/) for [`ignition-incendium/incendium`](https://github.com/ignition-incendium/incendium). These files were generated using `mypy`'s [`stubgen`](https://coatl-mypy.readthedocs.io/en/v0.971/stubgen.html).
 
 ## Installation and usage
 
-To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.11.
+To use `incendium-stubs`, you may install it with `pip`. It requires Python 3.7 through 3.12.
 
 ```sh
 python -m pip install incendium-stubs
 ```
 
 To run `mypy` against your code, execute the following command passing the source directory (typically `src`) or a single file:
```

### Comparing `incendium-stubs-2023.4.0.post2/stubs/incendium_stubs.egg-info/SOURCES.txt` & `incendium_stubs-2024.5.0/stubs/incendium_stubs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 stubs/incendium/__init__.pyi
+stubs/incendium/__version__.pyi
 stubs/incendium/constants.pyi
 stubs/incendium/dataset.pyi
 stubs/incendium/date.pyi
 stubs/incendium/db.pyi
 stubs/incendium/exceptions.pyi
+stubs/incendium/gui.pyi
+stubs/incendium/l10n.pyi
 stubs/incendium/net.pyi
 stubs/incendium/py.typed
 stubs/incendium/tag.pyi
+stubs/incendium/time.pyi
 stubs/incendium/user.pyi
 stubs/incendium/util.pyi
 stubs/incendium/version.pyi
 stubs/incendium/helper/__init__.pyi
 stubs/incendium/helper/py.typed
 stubs/incendium/helper/types.pyi
 stubs/incendium/vision/__init__.pyi
```

