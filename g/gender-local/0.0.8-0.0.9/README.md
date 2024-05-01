# Comparing `tmp/gender_local-0.0.8.tar.gz` & `tmp/gender_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender_local-0.0.8.tar", last modified: Fri Apr 19 10:04:52 2024, max compression
+gzip compressed data, was "gender_local-0.0.9.tar", last modified: Fri Apr 19 10:07:55 2024, max compression
```

## Comparing `gender_local-0.0.8.tar` & `gender_local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:52.633689 gender_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 10:04:52.633689 gender_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 10:04:29.000000 gender_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:52.629689 gender_local-0.0.8/gender_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:52.633689 gender_local-0.0.8/gender_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:29.000000 gender_local-0.0.8/gender_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 10:04:29.000000 gender_local-0.0.8/gender_local/src/constants_gender_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 10:04:29.000000 gender_local-0.0.8/gender_local/src/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 10:04:29.000000 gender_local-0.0.8/gender_local/src/gender_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:52.633689 gender_local-0.0.8/gender_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 10:04:52.000000 gender_local-0.0.8/gender_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 10:04:52.000000 gender_local-0.0.8/gender_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:04:52.000000 gender_local-0.0.8/gender_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 10:04:52.000000 gender_local-0.0.8/gender_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 10:04:52.000000 gender_local-0.0.8/gender_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 10:04:29.000000 gender_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:04:52.633689 gender_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 10:04:29.000000 gender_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:55.230233 gender_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 10:07:55.230233 gender_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 10:07:38.000000 gender_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:55.226233 gender_local-0.0.9/gender_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:55.230233 gender_local-0.0.9/gender_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:38.000000 gender_local-0.0.9/gender_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 10:07:38.000000 gender_local-0.0.9/gender_local/src/constants_gender_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 10:07:38.000000 gender_local-0.0.9/gender_local/src/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 10:07:38.000000 gender_local-0.0.9/gender_local/src/gender_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:55.230233 gender_local-0.0.9/gender_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 10:07:55.000000 gender_local-0.0.9/gender_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 10:07:55.000000 gender_local-0.0.9/gender_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:07:55.000000 gender_local-0.0.9/gender_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 10:07:55.000000 gender_local-0.0.9/gender_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 10:07:55.000000 gender_local-0.0.9/gender_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 10:07:38.000000 gender_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:07:55.230233 gender_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 10:07:38.000000 gender_local-0.0.9/setup.py
```

### Comparing `gender_local-0.0.8/PKG-INFO` & `gender_local-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gender-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles gender-local Local/Remote Python
 Home-page: https://github.com/circles-zone/gender-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `gender_local-0.0.8/README.md` & `gender_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gender_local-0.0.8/gender_local/src/constants_gender_local.py` & `gender_local-0.0.9/gender_local/src/constants_gender_local.py`

 * *Files identical despite different names*

### Comparing `gender_local-0.0.8/gender_local/src/gender.py` & `gender_local-0.0.9/gender_local/src/gender.py`

 * *Files identical despite different names*

### Comparing `gender_local-0.0.8/gender_local.egg-info/PKG-INFO` & `gender_local-0.0.9/gender_local.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gender-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles gender-local Local/Remote Python
 Home-page: https://github.com/circles-zone/gender-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `gender_local-0.0.8/pyproject.toml` & `gender_local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gender_local-0.0.8/setup.py` & `gender_local-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "gender-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/gender-local/
+    version='0.0.9',  # https://pypi.org/project/gender-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles gender-local Local/Remote Python",
     long_description="This is a package for sharing common CRUD operation of gender to the database",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

