# Comparing `tmp/mongo_vconnect-0.0.3.tar.gz` & `tmp/mongo_vconnect-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_vconnect-0.0.3.tar", last modified: Mon Apr 29 14:14:51 2024, max compression
+gzip compressed data, was "mongo_vconnect-0.0.6.tar", last modified: Wed May  1 07:53:27 2024, max compression
```

## Comparing `mongo_vconnect-0.0.3.tar` & `mongo_vconnect-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:51.305942 mongo_vconnect-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:14:51.305942 mongo_vconnect-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-29 14:14:30.000000 mongo_vconnect-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 14:14:30.000000 mongo_vconnect-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-29 14:14:51.305942 mongo_vconnect-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-29 14:14:30.000000 mongo_vconnect-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:51.301942 mongo_vconnect-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:51.301942 mongo_vconnect-0.0.3/src/MongoDBConnect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:30.000000 mongo_vconnect-0.0.3/src/MongoDBConnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 14:14:30.000000 mongo_vconnect-0.0.3/src/MongoDBConnect/mongo_crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:51.305942 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:14:51.000000 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-29 14:14:51.000000 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:14:51.000000 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 14:14:51.000000 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 14:14:51.000000 mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:53:27.849267 mongo_vconnect-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 07:53:27.849267 mongo_vconnect-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-01 07:53:03.000000 mongo_vconnect-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 07:53:03.000000 mongo_vconnect-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 07:53:27.849267 mongo_vconnect-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 07:53:03.000000 mongo_vconnect-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:53:27.845267 mongo_vconnect-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:53:27.849267 mongo_vconnect-0.0.6/src/MongoDBConnect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:53:03.000000 mongo_vconnect-0.0.6/src/MongoDBConnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-01 07:53:03.000000 mongo_vconnect-0.0.6/src/MongoDBConnect/mongo_crud1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:53:27.849267 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 07:53:27.000000 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 07:53:27.000000 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:53:27.000000 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 07:53:27.000000 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 07:53:27.000000 mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/top_level.txt
```

### Comparing `mongo_vconnect-0.0.3/PKG-INFO` & `mongo_vconnect-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_Vconnect
-Version: 0.0.3
+Version: 0.0.6
 Summary: A python package for connecting with database.
 Home-page: https://github.com/21Vijeth/Mlops_MongoDB
 Author: 21Vijeth
 Author-email: vijethfernandes21@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/21Vijeth/Mlops_MongoDB/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mongo_vconnect-0.0.3/README.md` & `mongo_vconnect-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mongo_vconnect-0.0.3/setup.cfg` & `mongo_vconnect-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mongo_vconnect-0.0.3/setup.py` & `mongo_vconnect-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from typing import List
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
    
 
-__version__ = "0.0.3"
+__version__ = "0.0.6"
 REPO_NAME = "Mlops_MongoDB"
 PKG_NAME= "mongo_Vconnect"
 AUTHOR_USER_NAME = "21Vijeth"
 AUTHOR_EMAIL = "vijethfernandes21@gmail.com"
 
 setup(
     name=PKG_NAME,
```

### Comparing `mongo_vconnect-0.0.3/src/MongoDBConnect/mongo_crud.py` & `mongo_vconnect-0.0.6/src/MongoDBConnect/mongo_crud1.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 import os
 import pandas as pd
 from pymongo.mongo_client import MongoClient
 import json
 from ensure import ensure_annotations
 
 
-class mongo_operation:
+class mongodb_operation:
     __collection=None # here i have created a private/protected variable
     __database=None
     
     def __init__(self,client_url: str, database_name: str, collection_name: str=None):
         self.client_url=client_url
         self.database_name=database_name
         self.collection_name=collection_name
        
     def create_mongo_client(self,collection=None):
         client=MongoClient(self.client_url)
         return client
     
     def create_database(self,collection=None):
-        if mongo_operation.__database==None:
+        if mongodb_operation.__database==None:
             client=self.create_mongo_client(collection)
             self.database=client[self.database_name]
         return self.database 
     
     def create_collection(self,collection=None):
-        if mongo_operation.__collection==None:
+        if mongodb_operation.__collection==None:
             database=self.create_database(collection)
             self.collection=database[self.collection_name]
-            mongo_operation.__collection=collection
+            mongodb_operation.__collection=collection
         
-        if mongo_operation.__collection!=collection:
+        if mongodb_operation.__collection!=collection:
             database=self.create_database(collection)
             self.collection=database[self.collection_name]
-            mongo_operation.__collection=collection
+            mongodb_operation.__collection=collection
             
         return self.collection
     
     def insert_record(self,record: dict, collection_name: str) -> Any:
         if type(record) == list:
             for data in record:
                 if type(data) != dict:
```

### Comparing `mongo_vconnect-0.0.3/src/mongo_Vconnect.egg-info/PKG-INFO` & `mongo_vconnect-0.0.6/src/mongo_Vconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_Vconnect
-Version: 0.0.3
+Version: 0.0.6
 Summary: A python package for connecting with database.
 Home-page: https://github.com/21Vijeth/Mlops_MongoDB
 Author: 21Vijeth
 Author-email: vijethfernandes21@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/21Vijeth/Mlops_MongoDB/issues
 Classifier: Programming Language :: Python :: 3.7
```

