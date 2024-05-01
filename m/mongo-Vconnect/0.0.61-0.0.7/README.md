# Comparing `tmp/mongo_vconnect-0.0.61.tar.gz` & `tmp/mongo_vconnect-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_vconnect-0.0.61.tar", last modified: Wed May  1 08:24:59 2024, max compression
+gzip compressed data, was "mongo_vconnect-0.0.7.tar", last modified: Wed May  1 09:01:42 2024, max compression
```

## Comparing `mongo_vconnect-0.0.61.tar` & `mongo_vconnect-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:24:59.303650 mongo_vconnect-0.0.61/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-01 08:24:59.303650 mongo_vconnect-0.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-01 08:24:38.000000 mongo_vconnect-0.0.61/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 08:24:38.000000 mongo_vconnect-0.0.61/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 08:24:59.303650 mongo_vconnect-0.0.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-01 08:24:38.000000 mongo_vconnect-0.0.61/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:24:59.299650 mongo_vconnect-0.0.61/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:24:59.303650 mongo_vconnect-0.0.61/src/MongoDBConnect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:24:38.000000 mongo_vconnect-0.0.61/src/MongoDBConnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-01 08:24:38.000000 mongo_vconnect-0.0.61/src/MongoDBConnect/mongo_crud1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:24:59.303650 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-01 08:24:59.000000 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 08:24:59.000000 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:24:59.000000 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 08:24:59.000000 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 08:24:59.000000 mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:42.088922 mongo_vconnect-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-01 09:01:42.088922 mongo_vconnect-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-01 09:01:19.000000 mongo_vconnect-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 09:01:19.000000 mongo_vconnect-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 09:01:42.088922 mongo_vconnect-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-01 09:01:19.000000 mongo_vconnect-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:42.084922 mongo_vconnect-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:42.084922 mongo_vconnect-0.0.7/src/MongoDBConnect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:19.000000 mongo_vconnect-0.0.7/src/MongoDBConnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-01 09:01:19.000000 mongo_vconnect-0.0.7/src/MongoDBConnect/mongo_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:42.084922 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-01 09:01:42.000000 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 09:01:42.000000 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:01:42.000000 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 09:01:42.000000 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 09:01:42.000000 mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/top_level.txt
```

### Comparing `mongo_vconnect-0.0.61/PKG-INFO` & `mongo_vconnect-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: mongo_Vconnect
-Version: 0.0.61
+Version: 0.0.7
 Summary: A python package for connecting with database.
 Home-page: https://github.com/21Vijeth/Mlops_MongoDB
 Author: 21Vijeth
 Author-email: vijethfernandes21@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/21Vijeth/Mlops_MongoDB/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Requires-Dist: ensure==1.0.2
-Requires-Dist: py-youtube==1.1.7
+Requires-Dist: pymongo
+Requires-Dist: pymongo[srv]
+Requires-Dist: dnspython
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: ensure
+Requires-Dist: pytest
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
```

### Comparing `mongo_vconnect-0.0.61/README.md` & `mongo_vconnect-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mongo_vconnect-0.0.61/setup.cfg` & `mongo_vconnect-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mongo_vconnect-0.0.61/setup.py` & `mongo_vconnect-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from typing import List
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
    
 
-__version__ = "0.0.61"
+__version__ = "0.0.7"
 REPO_NAME = "Mlops_MongoDB"
 PKG_NAME= "mongo_Vconnect"
 AUTHOR_USER_NAME = "21Vijeth"
 AUTHOR_EMAIL = "vijethfernandes21@gmail.com"
 
 setup(
     name=PKG_NAME,
@@ -21,9 +21,17 @@
     long_description_content="text/markdown",
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    install_requirs=["pymongo","pymongo[srv]","dnspython","pandas","numpy","ensure","pytest"]
+    install_requires=[
+        "pymongo",
+        "pymongo[srv]",
+        "dnspython",
+        "pandas",
+        "numpy",
+        "ensure",
+        "pytest"
+    ]
     )
```

### Comparing `mongo_vconnect-0.0.61/src/MongoDBConnect/mongo_crud1.py` & `mongo_vconnect-0.0.7/src/MongoDBConnect/mongo_crud.py`

 * *Files identical despite different names*

### Comparing `mongo_vconnect-0.0.61/src/mongo_Vconnect.egg-info/PKG-INFO` & `mongo_vconnect-0.0.7/src/mongo_Vconnect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: mongo_Vconnect
-Version: 0.0.61
+Version: 0.0.7
 Summary: A python package for connecting with database.
 Home-page: https://github.com/21Vijeth/Mlops_MongoDB
 Author: 21Vijeth
 Author-email: vijethfernandes21@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/21Vijeth/Mlops_MongoDB/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Requires-Dist: ensure==1.0.2
-Requires-Dist: py-youtube==1.1.7
+Requires-Dist: pymongo
+Requires-Dist: pymongo[srv]
+Requires-Dist: dnspython
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: ensure
+Requires-Dist: pytest
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
```

