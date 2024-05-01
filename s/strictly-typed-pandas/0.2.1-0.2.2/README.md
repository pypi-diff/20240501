# Comparing `tmp/strictly_typed_pandas-0.2.1.tar.gz` & `tmp/strictly_typed_pandas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictly_typed_pandas-0.2.1.tar", last modified: Tue Feb  6 21:42:24 2024, max compression
+gzip compressed data, was "strictly_typed_pandas-0.2.2.tar", last modified: Mon Feb 26 08:27:39 2024, max compression
```

## Comparing `strictly_typed_pandas-0.2.1.tar` & `strictly_typed_pandas-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.999789 strictly_typed_pandas-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-06 21:42:23.999789 strictly_typed_pandas-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 21:42:23.999789 strictly_typed_pandas-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.995789 strictly_typed_pandas-0.2.1/strictly_typed_pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.995789 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.995789 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/
--rw-r--r--   0 runner    (1001) docker     (127)    49186 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/create_empty_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/typeguard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.999789 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 21:42:23.000000 strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 21:42:23.999789 strictly_typed_pandas-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/tests/test_indexed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-06 21:42:13.000000 strictly_typed_pandas-0.2.1/tests/test_type_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.854357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (127)    49186 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/create_empty_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/typeguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 08:27:39.000000 strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:27:39.858357 strictly_typed_pandas-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_indexed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-26 08:27:27.000000 strictly_typed_pandas-0.2.2/tests/test_type_validation.py
```

### Comparing `strictly_typed_pandas-0.2.1/LICENSE` & `strictly_typed_pandas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/PKG-INFO` & `strictly_typed_pandas-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.2.1
+Version: 0.2.2
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy<=1.26.4
-Requires-Dist: pandas<=2.2.0
-Requires-Dist: pandas-stubs<=2.1.4.231227
+Requires-Dist: pandas<=2.2.1
+Requires-Dist: pandas-stubs<=2.2.0.240218
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
 
 I love Pandas! But in production code I’m always a bit wary when I see:
```

### Comparing `strictly_typed_pandas-0.2.1/README.rst` & `strictly_typed_pandas-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/setup.py` & `strictly_typed_pandas-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/__init__.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/importhook.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/importhook.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/_vendor/typeguard/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/create_empty_dataframe.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/create_empty_dataframe.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/dataset.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/dataset.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/immutable.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/immutable.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/pandas_types.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/pandas_types.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/pytest_plugin.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/typeguard.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/typeguard.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas/validate_schema.py` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas/validate_schema.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/PKG-INFO` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.2.1
+Version: 0.2.2
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy<=1.26.4
-Requires-Dist: pandas<=2.2.0
-Requires-Dist: pandas-stubs<=2.1.4.231227
+Requires-Dist: pandas<=2.2.1
+Requires-Dist: pandas-stubs<=2.2.0.240218
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
 
 I love Pandas! But in production code I’m always a bit wary when I see:
```

### Comparing `strictly_typed_pandas-0.2.1/strictly_typed_pandas.egg-info/SOURCES.txt` & `strictly_typed_pandas-0.2.2/strictly_typed_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/tests/test_dataset.py` & `strictly_typed_pandas-0.2.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/tests/test_indexed_dataset.py` & `strictly_typed_pandas-0.2.2/tests/test_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.2.1/tests/test_type_validation.py` & `strictly_typed_pandas-0.2.2/tests/test_type_validation.py`

 * *Files identical despite different names*

