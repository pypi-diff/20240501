# Comparing `tmp/botocore-a-la-carte-neptune-1.34.93.tar.gz` & `tmp/botocore-a-la-carte-neptune-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-neptune-1.34.93.tar", last modified: Sat Apr 27 01:00:58 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-neptune-1.34.94.tar", last modified: Tue Apr 30 01:01:37 2024, max compression
```

## Comparing `botocore-a-la-carte-neptune-1.34.93.tar` & `botocore-a-la-carte-neptune-1.34.94.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.821250 botocore-a-la-carte-neptune-1.34.93/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 01:00:58.821250 botocore-a-la-carte-neptune-1.34.93/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.817250 botocore-a-la-carte-neptune-1.34.93/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.817250 botocore-a-la-carte-neptune-1.34.93/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.817250 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.821250 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   330869 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/service-2.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-27 01:00:34.000000 botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:00:58.821250 botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:00:58.821250 botocore-a-la-carte-neptune-1.34.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 01:00:58.000000 botocore-a-la-carte-neptune-1.34.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   330869 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/service-2.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-30 01:01:14.000000 botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:01:37.259296 botocore-a-la-carte-neptune-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 01:01:37.000000 botocore-a-la-carte-neptune-1.34.94/setup.py
```

### Comparing `botocore-a-la-carte-neptune-1.34.93/LICENSE.txt` & `botocore-a-la-carte-neptune-1.34.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/PKG-INFO` & `botocore-a-la-carte-neptune-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-neptune
-Version: 1.34.93
+Version: 1.34.94
 Summary: neptune data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/paginators-1.json` & `botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/service-2.json` & `botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/service-2.sdk-extras.json` & `botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/service-2.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore/data/neptune/2014-10-31/waiters-2.json` & `botocore-a-la-carte-neptune-1.34.94/botocore/data/neptune/2014-10-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/PKG-INFO` & `botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-neptune
-Version: 1.34.93
+Version: 1.34.94
 Summary: neptune data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-neptune-1.34.93/botocore_a_la_carte_neptune.egg-info/SOURCES.txt` & `botocore-a-la-carte-neptune-1.34.94/botocore_a_la_carte_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-neptune-1.34.93/setup.py` & `botocore-a-la-carte-neptune-1.34.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-neptune',
-    version="1.34.93",
+    version="1.34.94",
     description='neptune data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/neptune/*/*.json'],
```

