# Comparing `tmp/cerbernetix.toolbox-0.9.0.tar.gz` & `tmp/cerbernetix.toolbox-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbernetix.toolbox-0.9.0.tar", last modified: Fri Oct 27 06:51:32 2023, max compression
+gzip compressed data, was "cerbernetix.toolbox-0.9.1.tar", last modified: Fri Oct 27 07:33:27 2023, max compression
```

## Comparing `cerbernetix.toolbox-0.9.0.tar` & `cerbernetix.toolbox-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.634350 cerbernetix.toolbox-0.9.0/
--rw-r--r--   0 jsc        (501) staff       (20)     1078 2023-09-04 19:25:21.000000 cerbernetix.toolbox-0.9.0/LICENSE
--rw-r--r--   0 jsc        (501) staff       (20)     3833 2023-10-27 06:51:32.634153 cerbernetix.toolbox-0.9.0/PKG-INFO
--rw-r--r--   0 jsc        (501) staff       (20)     2974 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/README.md
--rw-r--r--   0 jsc        (501) staff       (20)     1222 2023-10-26 15:59:37.000000 cerbernetix.toolbox-0.9.0/pyproject.toml
--rw-r--r--   0 jsc        (501) staff       (20)       38 2023-10-27 06:51:32.634381 cerbernetix.toolbox-0.9.0/setup.cfg
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.629119 cerbernetix.toolbox-0.9.0/src/
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.629171 cerbernetix.toolbox-0.9.0/src/cerbernetix/
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.630802 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/
--rw-r--r--   0 jsc        (501) staff       (20)       96 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/__init__.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.631226 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/
--rw-r--r--   0 jsc        (501) staff       (20)     1460 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)    19716 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/config.py
--rw-r--r--   0 jsc        (501) staff       (20)    13292 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/config_option.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.631636 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/
--rw-r--r--   0 jsc        (501) staff       (20)     2008 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)     3367 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/mappers.py
--rw-r--r--   0 jsc        (501) staff       (20)     5833 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/value_extractor.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.632501 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/
--rw-r--r--   0 jsc        (501) staff       (20)     3812 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)    26559 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/csv_file.py
--rw-r--r--   0 jsc        (501) staff       (20)     9743 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/file.py
--rw-r--r--   0 jsc        (501) staff       (20)    21117 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/file_manager.py
--rw-r--r--   0 jsc        (501) staff       (20)     7677 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/json_file.py
--rw-r--r--   0 jsc        (501) staff       (20)     6817 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/path.py
--rw-r--r--   0 jsc        (501) staff       (20)    15068 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/pickle_file.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.632857 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/
--rw-r--r--   0 jsc        (501) staff       (20)     1258 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)     2228 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/config.py
--rw-r--r--   0 jsc        (501) staff       (20)    16009 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/log_file.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.633119 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/math/
--rw-r--r--   0 jsc        (501) staff       (20)      640 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/math/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)     3120 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/math/combination.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.633483 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/
--rw-r--r--   0 jsc        (501) staff       (20)     1018 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)     2734 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/decorators.py
--rw-r--r--   0 jsc        (501) staff       (20)     3568 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/test_case.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.633695 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/time/
--rw-r--r--   0 jsc        (501) staff       (20)     1112 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/time/__init__.py
--rw-r--r--   0 jsc        (501) staff       (20)    10784 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/time/weekday.py
-drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 06:51:32.630669 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/
--rw-r--r--   0 jsc        (501) staff       (20)     3833 2023-10-27 06:51:32.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 jsc        (501) staff       (20)     1288 2023-10-27 06:51:32.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 jsc        (501) staff       (20)        1 2023-10-27 06:51:32.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 jsc        (501) staff       (20)      117 2023-10-27 06:51:32.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/requires.txt
--rw-r--r--   0 jsc        (501) staff       (20)       12 2023-10-27 06:51:32.000000 cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.974124 cerbernetix.toolbox-0.9.1/
+-rw-r--r--   0 jsc        (501) staff       (20)     1078 2023-09-04 19:25:21.000000 cerbernetix.toolbox-0.9.1/LICENSE
+-rw-r--r--   0 jsc        (501) staff       (20)     4456 2023-10-27 07:33:27.973921 cerbernetix.toolbox-0.9.1/PKG-INFO
+-rw-r--r--   0 jsc        (501) staff       (20)     3597 2023-10-27 07:32:53.000000 cerbernetix.toolbox-0.9.1/README.md
+-rw-r--r--   0 jsc        (501) staff       (20)     1222 2023-10-27 07:33:10.000000 cerbernetix.toolbox-0.9.1/pyproject.toml
+-rw-r--r--   0 jsc        (501) staff       (20)       38 2023-10-27 07:33:27.974162 cerbernetix.toolbox-0.9.1/setup.cfg
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.968389 cerbernetix.toolbox-0.9.1/src/
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.968436 cerbernetix.toolbox-0.9.1/src/cerbernetix/
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.970145 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/
+-rw-r--r--   0 jsc        (501) staff       (20)       96 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/__init__.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.970653 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/
+-rw-r--r--   0 jsc        (501) staff       (20)     1460 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)    19716 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/config.py
+-rw-r--r--   0 jsc        (501) staff       (20)    13292 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/config_option.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.971142 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/
+-rw-r--r--   0 jsc        (501) staff       (20)     2008 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)     3367 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/mappers.py
+-rw-r--r--   0 jsc        (501) staff       (20)     5833 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/value_extractor.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.972108 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/
+-rw-r--r--   0 jsc        (501) staff       (20)     3812 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)    26559 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/csv_file.py
+-rw-r--r--   0 jsc        (501) staff       (20)     9743 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/file.py
+-rw-r--r--   0 jsc        (501) staff       (20)    21117 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/file_manager.py
+-rw-r--r--   0 jsc        (501) staff       (20)     7677 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/json_file.py
+-rw-r--r--   0 jsc        (501) staff       (20)     6817 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/path.py
+-rw-r--r--   0 jsc        (501) staff       (20)    15068 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/pickle_file.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.972474 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/
+-rw-r--r--   0 jsc        (501) staff       (20)     1258 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)     2228 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/config.py
+-rw-r--r--   0 jsc        (501) staff       (20)    16009 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/log_file.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.972746 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/math/
+-rw-r--r--   0 jsc        (501) staff       (20)      640 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/math/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)     3120 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/math/combination.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.973134 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/
+-rw-r--r--   0 jsc        (501) staff       (20)     1018 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)     2734 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/decorators.py
+-rw-r--r--   0 jsc        (501) staff       (20)     3568 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/test_case.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.973361 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/time/
+-rw-r--r--   0 jsc        (501) staff       (20)     1112 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/time/__init__.py
+-rw-r--r--   0 jsc        (501) staff       (20)    10784 2023-10-26 15:59:15.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/time/weekday.py
+drwxr-xr-x   0 jsc        (501) staff       (20)        0 2023-10-27 07:33:27.969948 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/
+-rw-r--r--   0 jsc        (501) staff       (20)     4456 2023-10-27 07:33:27.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 jsc        (501) staff       (20)     1288 2023-10-27 07:33:27.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 jsc        (501) staff       (20)        1 2023-10-27 07:33:27.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 jsc        (501) staff       (20)      117 2023-10-27 07:33:27.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/requires.txt
+-rw-r--r--   0 jsc        (501) staff       (20)       12 2023-10-27 07:33:27.000000 cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/top_level.txt
```

### Comparing `cerbernetix.toolbox-0.9.0/LICENSE` & `cerbernetix.toolbox-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/PKG-INFO` & `cerbernetix.toolbox-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbernetix.toolbox
-Version: 0.9.0
+Version: 0.9.1
 Summary: A set of utilities for Python projects
 Author-email: Jean-Sébastien CONAN <jsconan@gmail.com>
 Project-URL: Homepage, https://github.com/cerbernetix/py-toolbox
 Project-URL: Bug Tracker, https://github.com/cerbernetix/py-toolbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,15 @@
 
 -   [Requirements](#Requirements)
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Development](#Development)
     -   [Code style](#Codestyle)
     -   [Testing](#Testing)
+    -   [Document](#Document)
 -   [License](#License)
 
 <!-- vscode-markdown-toc-config
 	numbering=false
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
@@ -45,30 +46,38 @@
 
 The toolbox has been written in **`Python 3`**, and it needs version `3.7`.
 
 The dependencies are managed by `pip` using the file `requirements.txt`.
 
 ## <a name='Installation'></a>Installation
 
-To add `py-toolbox` to your project, run the following command:
+To add `py-toolbox` to your project, run the following command. This will add the last released version to you project:
 
 ```sh
-pip install git+https://github.com/cerbernetix/py-toolbox.git
+pip install --upgrade cerbernetix.toolbox
+```
+
+For getting the last unstable version, the package needs to be installed from the source code. The following command will grab the last develop version:
+
+```sh
+pip install --upgrade git+https://github.com/cerbernetix/py-toolbox.git@develop
+```
+
+If you prefer using ssh:
+
+```sh
+pip install --upgrade git+ssh://git@github.com/cerbernetix/py-toolbox.git@develop
 ```
 
 ## <a name='Usage'></a>Usage
 
 `py-toolbox` offers several utilities per domain.
 
 Please refer to the [documentation](./docs/README.md) for more information.
 
-The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
-
-The script `./pydoc.sh` can be used to regenerate it.
-
 ## <a name='Development'></a>Development
 
 Check out the repository:
 
 ```sh
 git clone git@github.com:cerbernetix/py-toolbox.git
 ```
@@ -123,11 +132,19 @@
 
 Unit tests are made using `unittest`. To run them:
 
 ```sh
 python3 -m unittest
 ```
 
+### <a name='Document'></a>Document
+
+Docstrings are written following the [Google docstrings format](https://github.com/google/styleguide/blob/gh-pages/pyguide.md#38-comments-and-docstrings).
+
+The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
+
+The script `./pydoc.sh` can be used to regenerate it.
+
 ## <a name='License'></a>License
 
 Copyright (c) 2023 Jean-Sébastien CONAN
 Distributed under the MIT License (See LICENSE file or copy at [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)).
```

### Comparing `cerbernetix.toolbox-0.9.0/README.md` & `cerbernetix.toolbox-0.9.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 -   [Requirements](#Requirements)
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Development](#Development)
     -   [Code style](#Codestyle)
     -   [Testing](#Testing)
+    -   [Document](#Document)
 -   [License](#License)
 
 <!-- vscode-markdown-toc-config
 	numbering=false
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
@@ -22,30 +23,38 @@
 
 The toolbox has been written in **`Python 3`**, and it needs version `3.7`.
 
 The dependencies are managed by `pip` using the file `requirements.txt`.
 
 ## <a name='Installation'></a>Installation
 
-To add `py-toolbox` to your project, run the following command:
+To add `py-toolbox` to your project, run the following command. This will add the last released version to you project:
 
 ```sh
-pip install git+https://github.com/cerbernetix/py-toolbox.git
+pip install --upgrade cerbernetix.toolbox
+```
+
+For getting the last unstable version, the package needs to be installed from the source code. The following command will grab the last develop version:
+
+```sh
+pip install --upgrade git+https://github.com/cerbernetix/py-toolbox.git@develop
+```
+
+If you prefer using ssh:
+
+```sh
+pip install --upgrade git+ssh://git@github.com/cerbernetix/py-toolbox.git@develop
 ```
 
 ## <a name='Usage'></a>Usage
 
 `py-toolbox` offers several utilities per domain.
 
 Please refer to the [documentation](./docs/README.md) for more information.
 
-The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
-
-The script `./pydoc.sh` can be used to regenerate it.
-
 ## <a name='Development'></a>Development
 
 Check out the repository:
 
 ```sh
 git clone git@github.com:cerbernetix/py-toolbox.git
 ```
@@ -100,11 +109,19 @@
 
 Unit tests are made using `unittest`. To run them:
 
 ```sh
 python3 -m unittest
 ```
 
+### <a name='Document'></a>Document
+
+Docstrings are written following the [Google docstrings format](https://github.com/google/styleguide/blob/gh-pages/pyguide.md#38-comments-and-docstrings).
+
+The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
+
+The script `./pydoc.sh` can be used to regenerate it.
+
 ## <a name='License'></a>License
 
 Copyright (c) 2023 Jean-Sébastien CONAN
 Distributed under the MIT License (See LICENSE file or copy at [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)).
```

### Comparing `cerbernetix.toolbox-0.9.0/pyproject.toml` & `cerbernetix.toolbox-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cerbernetix.toolbox"
-version = "0.9.0"
+version = "0.9.1"
 authors = [{ name = "Jean-Sébastien CONAN", email = "jsconan@gmail.com" }]
 description = "A set of utilities for Python projects"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["requests>=2.31.0"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/config.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/config.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/config/config_option.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/config/config_option.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/mappers.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/mappers.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/data/value_extractor.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/data/value_extractor.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/csv_file.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/csv_file.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/file.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/file.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/file_manager.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/file_manager.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/json_file.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/json_file.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/path.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/path.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/files/pickle_file.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/files/pickle_file.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/config.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/config.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/logging/log_file.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/logging/log_file.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/math/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/math/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/math/combination.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/math/combination.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/decorators.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/testing/test_case.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/time/__init__.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/time/__init__.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix/toolbox/time/weekday.py` & `cerbernetix.toolbox-0.9.1/src/cerbernetix/toolbox/time/weekday.py`

 * *Files identical despite different names*

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/PKG-INFO` & `cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbernetix.toolbox
-Version: 0.9.0
+Version: 0.9.1
 Summary: A set of utilities for Python projects
 Author-email: Jean-Sébastien CONAN <jsconan@gmail.com>
 Project-URL: Homepage, https://github.com/cerbernetix/py-toolbox
 Project-URL: Bug Tracker, https://github.com/cerbernetix/py-toolbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,15 @@
 
 -   [Requirements](#Requirements)
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Development](#Development)
     -   [Code style](#Codestyle)
     -   [Testing](#Testing)
+    -   [Document](#Document)
 -   [License](#License)
 
 <!-- vscode-markdown-toc-config
 	numbering=false
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
@@ -45,30 +46,38 @@
 
 The toolbox has been written in **`Python 3`**, and it needs version `3.7`.
 
 The dependencies are managed by `pip` using the file `requirements.txt`.
 
 ## <a name='Installation'></a>Installation
 
-To add `py-toolbox` to your project, run the following command:
+To add `py-toolbox` to your project, run the following command. This will add the last released version to you project:
 
 ```sh
-pip install git+https://github.com/cerbernetix/py-toolbox.git
+pip install --upgrade cerbernetix.toolbox
+```
+
+For getting the last unstable version, the package needs to be installed from the source code. The following command will grab the last develop version:
+
+```sh
+pip install --upgrade git+https://github.com/cerbernetix/py-toolbox.git@develop
+```
+
+If you prefer using ssh:
+
+```sh
+pip install --upgrade git+ssh://git@github.com/cerbernetix/py-toolbox.git@develop
 ```
 
 ## <a name='Usage'></a>Usage
 
 `py-toolbox` offers several utilities per domain.
 
 Please refer to the [documentation](./docs/README.md) for more information.
 
-The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
-
-The script `./pydoc.sh` can be used to regenerate it.
-
 ## <a name='Development'></a>Development
 
 Check out the repository:
 
 ```sh
 git clone git@github.com:cerbernetix/py-toolbox.git
 ```
@@ -123,11 +132,19 @@
 
 Unit tests are made using `unittest`. To run them:
 
 ```sh
 python3 -m unittest
 ```
 
+### <a name='Document'></a>Document
+
+Docstrings are written following the [Google docstrings format](https://github.com/google/styleguide/blob/gh-pages/pyguide.md#38-comments-and-docstrings).
+
+The documentation is generated using [lazydocs](https://github.com/ml-tooling/lazydocs).
+
+The script `./pydoc.sh` can be used to regenerate it.
+
 ## <a name='License'></a>License
 
 Copyright (c) 2023 Jean-Sébastien CONAN
 Distributed under the MIT License (See LICENSE file or copy at [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)).
```

### Comparing `cerbernetix.toolbox-0.9.0/src/cerbernetix.toolbox.egg-info/SOURCES.txt` & `cerbernetix.toolbox-0.9.1/src/cerbernetix.toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

