# Comparing `tmp/beacon2-import-1.0.6.tar.gz` & `tmp/beacon2-import-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beacon2-import-1.0.6.tar", last modified: Fri Apr 19 17:27:42 2024, max compression
+gzip compressed data, was "dist/beacon2-import-1.0.7.tar", last modified: Wed May  1 11:38:58 2024, max compression
```

## Comparing `beacon2-import-1.0.6.tar` & `beacon2-import-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 17:27:42.950504 beacon2-import-1.0.6/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-19 17:27:42.950504 beacon2-import-1.0.6/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.6/README.md
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 17:27:42.946503 beacon2-import-1.0.6/beacon2_import/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.6/beacon2_import/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    16575 2024-04-08 11:19:40.000000 beacon2-import-1.0.6/beacon2_import/beacon2_import.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.6/beacon2_import/utils.py
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 17:27:42.946503 beacon2-import-1.0.6/beacon2_import.egg-info/
--rw-r--r--   0 khaled    (1000) khaled    (1000)      211 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/SOURCES.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/dependency_links.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      140 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/entry_points.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       47 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/requires.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-04-19 17:27:42.000000 beacon2-import-1.0.6/beacon2_import.egg-info/top_level.txt
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-19 17:27:42.950504 beacon2-import-1.0.6/beacon2_search/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.6/beacon2_search/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.6/beacon2_search/beacon2_search.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.6/beacon2_search/utils.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-04-19 17:27:42.950504 beacon2-import-1.0.6/setup.cfg
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      807 2024-04-19 17:27:07.000000 beacon2-import-1.0.6/setup.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2-import-1.0.6/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/top_level.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/SOURCES.txt
+-rw-r--r--   0 khaled    (1000) khaled    (1000)      258 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       47 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/requires.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      141 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/entry_points.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      258 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2-import-1.0.7/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.7/beacon2_import/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    16574 2024-05-01 11:30:19.000000 beacon2-import-1.0.7/beacon2_import/beacon2_import.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.7/beacon2_import/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/setup.cfg
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.7/README.md
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      807 2024-05-01 11:36:53.000000 beacon2-import-1.0.7/setup.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_search/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.7/beacon2_search/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.7/beacon2_search/beacon2_search.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.7/beacon2_search/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `beacon2-import-1.0.6/beacon2_import/beacon2_import.py` & `beacon2-import-1.0.7/beacon2_import/beacon2_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
             parser.print_help()
             sys.exit(1)
     
     # connect to beacon 
     client= connect_to_mongodb(args, parser)
     db = client[args.database]
     collection = db[args.collection]
-    #clear_collections(db, args)
+    clear_collections(db, args)
     
     
     
     # connect to Galaxy instance 
     if args.galaxy:
         # Check galaxy inputs to connect to Galaxy
         galaxy_args = ['galaxy_url', 'galaxy_key']
```

### Comparing `beacon2-import-1.0.6/beacon2_import/utils.py` & `beacon2-import-1.0.7/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.6/beacon2_search/beacon2_search.py` & `beacon2-import-1.0.7/beacon2_search/beacon2_search.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.6/beacon2_search/utils.py` & `beacon2-import-1.0.7/beacon2_import/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.6/setup.py` & `beacon2-import-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beacon2-import',
-    version='1.0.6',
+    version='1.0.7',
     author='Khaled Jumah',
     author_email='khalled.jooma@yahoo.com',
     description='Seamlessly import and query genomic variant data from a beacon',
     license = 'CC-BY-NC-4.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

### Comparing `beacon2-import-1.0.6/utils.py` & `beacon2-import-1.0.7/beacon2_search/utils.py`

 * *Files identical despite different names*

