# Comparing `tmp/docgraph-0.0.6.dev0.tar.gz` & `tmp/docgraph-0.0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docgraph-0.0.6.dev0.tar", last modified: Wed May  1 16:11:26 2024, max compression
+gzip compressed data, was "docgraph-0.0.7.dev0.tar", last modified: Wed May  1 16:17:01 2024, max compression
```

## Comparing `docgraph-0.0.6.dev0.tar` & `docgraph-0.0.7.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:11:26.533927 docgraph-0.0.6.dev0/
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1861 2024-05-01 16:11:26.532399 docgraph-0.0.6.dev0/PKG-INFO
--rw-r--r--   0 blarson   (1152) rnd      (10001)      942 2024-04-29 22:16:25.000000 docgraph-0.0.6.dev0/README.md
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:11:26.479527 docgraph-0.0.6.dev0/common/
--rw-rw-r--   0 blarson   (1152) rnd      (10001)       79 2024-04-29 17:22:28.000000 docgraph-0.0.6.dev0/common/__init__.py
--rw-rw-r--   0 blarson   (1152) rnd      (10001)      612 2024-04-29 17:22:28.000000 docgraph-0.0.6.dev0/common/logging_utils.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)    19884 2024-04-29 17:22:28.000000 docgraph-0.0.6.dev0/common/openapi.py
--rw-rw-r--   0 blarson   (1152) rnd      (10001)     6452 2024-04-29 17:22:28.000000 docgraph-0.0.6.dev0/common/utils.py
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:11:26.498188 docgraph-0.0.6.dev0/docgraph/
--rw-r--r--   0 blarson   (1152) rnd      (10001)        0 2024-04-29 20:53:16.000000 docgraph-0.0.6.dev0/docgraph/__init__.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1120 2024-04-29 23:08:23.000000 docgraph-0.0.6.dev0/docgraph/__main__.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)     2022 2024-04-29 17:22:28.000000 docgraph-0.0.6.dev0/docgraph/jsonutil.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)      625 2024-04-29 23:25:39.000000 docgraph-0.0.6.dev0/docgraph/version.py
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:11:26.525239 docgraph-0.0.6.dev0/docgraph.egg-info/
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1861 2024-05-01 16:11:26.000000 docgraph-0.0.6.dev0/docgraph.egg-info/PKG-INFO
--rw-r--r--   0 blarson   (1152) rnd      (10001)      337 2024-05-01 16:11:26.000000 docgraph-0.0.6.dev0/docgraph.egg-info/SOURCES.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)        1 2024-05-01 16:11:26.000000 docgraph-0.0.6.dev0/docgraph.egg-info/dependency_links.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       29 2024-05-01 16:11:26.000000 docgraph-0.0.6.dev0/docgraph.egg-info/requires.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       16 2024-05-01 16:11:26.000000 docgraph-0.0.6.dev0/docgraph.egg-info/top_level.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       38 2024-05-01 16:11:26.535638 docgraph-0.0.6.dev0/setup.cfg
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1257 2024-05-01 16:08:20.000000 docgraph-0.0.6.dev0/setup.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:17:01.689906 docgraph-0.0.7.dev0/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1861 2024-05-01 16:17:01.688219 docgraph-0.0.7.dev0/PKG-INFO
+-rw-r--r--   0 blarson   (1152) rnd      (10001)      942 2024-04-29 22:16:25.000000 docgraph-0.0.7.dev0/README.md
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:17:01.627447 docgraph-0.0.7.dev0/common/
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)       79 2024-04-29 17:22:28.000000 docgraph-0.0.7.dev0/common/__init__.py
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)      612 2024-04-29 17:22:28.000000 docgraph-0.0.7.dev0/common/logging_utils.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)    19884 2024-04-29 17:22:28.000000 docgraph-0.0.7.dev0/common/openapi.py
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)     6452 2024-04-29 17:22:28.000000 docgraph-0.0.7.dev0/common/utils.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:17:01.650136 docgraph-0.0.7.dev0/docgraph/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)        0 2024-04-29 20:53:16.000000 docgraph-0.0.7.dev0/docgraph/__init__.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1120 2024-04-29 23:08:23.000000 docgraph-0.0.7.dev0/docgraph/__main__.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     2022 2024-04-29 17:22:28.000000 docgraph-0.0.7.dev0/docgraph/jsonutil.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)      625 2024-04-29 23:25:39.000000 docgraph-0.0.7.dev0/docgraph/version.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:17:01.680468 docgraph-0.0.7.dev0/docgraph.egg-info/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1861 2024-05-01 16:17:01.000000 docgraph-0.0.7.dev0/docgraph.egg-info/PKG-INFO
+-rw-r--r--   0 blarson   (1152) rnd      (10001)      337 2024-05-01 16:17:01.000000 docgraph-0.0.7.dev0/docgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)        1 2024-05-01 16:17:01.000000 docgraph-0.0.7.dev0/docgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       29 2024-05-01 16:17:01.000000 docgraph-0.0.7.dev0/docgraph.egg-info/requires.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       16 2024-05-01 16:17:01.000000 docgraph-0.0.7.dev0/docgraph.egg-info/top_level.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       38 2024-05-01 16:17:01.691573 docgraph-0.0.7.dev0/setup.cfg
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1257 2024-05-01 16:08:20.000000 docgraph-0.0.7.dev0/setup.py
```

### Comparing `docgraph-0.0.6.dev0/PKG-INFO` & `docgraph-0.0.7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docgraph
-Version: 0.0.6.dev0
+Version: 0.0.7.dev0
 Summary: Document Graph for LLM Embedding search and Completion context
 Home-page: https://ha-us.dso.thermofisher.net/artifactory/sci-ai-pypi-internal/docgraph
 Author: Brad Larson
 Author-email: <bhlarson@gmail.com>
 License: UNKNOWN
 Description: # Docgraph Python Library
```

### Comparing `docgraph-0.0.6.dev0/README.md` & `docgraph-0.0.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/common/logging_utils.py` & `docgraph-0.0.7.dev0/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/common/openapi.py` & `docgraph-0.0.7.dev0/common/openapi.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/common/utils.py` & `docgraph-0.0.7.dev0/common/utils.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/docgraph/__main__.py` & `docgraph-0.0.7.dev0/docgraph/__main__.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/docgraph/jsonutil.py` & `docgraph-0.0.7.dev0/docgraph/jsonutil.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/docgraph/version.py` & `docgraph-0.0.7.dev0/docgraph/version.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.6.dev0/docgraph.egg-info/PKG-INFO` & `docgraph-0.0.7.dev0/docgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docgraph
-Version: 0.0.6.dev0
+Version: 0.0.7.dev0
 Summary: Document Graph for LLM Embedding search and Completion context
 Home-page: https://ha-us.dso.thermofisher.net/artifactory/sci-ai-pypi-internal/docgraph
 Author: Brad Larson
 Author-email: <bhlarson@gmail.com>
 License: UNKNOWN
 Description: # Docgraph Python Library
```

### Comparing `docgraph-0.0.6.dev0/setup.py` & `docgraph-0.0.7.dev0/setup.py`

 * *Files identical despite different names*

