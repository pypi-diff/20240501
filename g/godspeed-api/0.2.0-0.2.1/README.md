# Comparing `tmp/godspeed_api-0.2.0.tar.gz` & `tmp/godspeed_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.2.0.tar", last modified: Wed May  1 16:40:30 2024, max compression
+gzip compressed data, was "godspeed_api-0.2.1.tar", last modified: Wed May  1 16:44:15 2024, max compression
```

## Comparing `godspeed_api-0.2.0.tar` & `godspeed_api-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:44:15.000000 godspeed_api-0.2.1/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 16:44:15.000000 godspeed_api-0.2.1/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:44:15.000000 godspeed_api-0.2.1/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 16:44:15.000000 godspeed_api-0.2.1/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 16:44:15.000000 godspeed_api-0.2.1/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:44:15.052101 godspeed_api-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-01 16:44:10.000000 godspeed_api-0.2.1/tests/test_api.py
```

### Comparing `godspeed_api-0.2.0/LICENSE` & `godspeed_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.2.0/PKG-INFO` & `godspeed_api-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `godspeed_api-0.2.0/README.md` & `godspeed_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.2.0/godspeed_api/api.py` & `godspeed_api-0.2.1/godspeed_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import json
 from typing import List, Optional
 from dacite import Config, from_dict
 import requests
 import datetime
 import logging
 
-from .Models.ListTasksResponse import ListTasksResponse
-from .Models.Status import Status
+from Models.ListTasksResponse import ListTasksResponse
+from Models.Status import Status
 
 
 class AuthError(Exception):
     def __init__(self):
         super().__init__("Failed to authenticate")
```

### Comparing `godspeed_api-0.2.0/godspeed_api.egg-info/PKG-INFO` & `godspeed_api-0.2.1/godspeed_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `godspeed_api-0.2.0/setup.py` & `godspeed_api-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="godspeed_api",
```

### Comparing `godspeed_api-0.2.0/tests/test_api.py` & `godspeed_api-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

