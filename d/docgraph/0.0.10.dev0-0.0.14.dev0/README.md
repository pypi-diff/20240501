# Comparing `tmp/docgraph-0.0.10.dev0.tar.gz` & `tmp/docgraph-0.0.14.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docgraph-0.0.10.dev0.tar", last modified: Wed May  1 16:43:35 2024, max compression
+gzip compressed data, was "docgraph-0.0.14.dev0.tar", last modified: Wed May  1 18:51:36 2024, max compression
```

## Comparing `docgraph-0.0.10.dev0.tar` & `docgraph-0.0.14.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:43:35.711628 docgraph-0.0.10.dev0/
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1946 2024-05-01 16:43:35.710088 docgraph-0.0.10.dev0/PKG-INFO
--rw-r--r--   0 blarson   (1152) rnd      (10001)      942 2024-04-29 22:16:25.000000 docgraph-0.0.10.dev0/README.md
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:43:35.656361 docgraph-0.0.10.dev0/common/
--rw-rw-r--   0 blarson   (1152) rnd      (10001)       79 2024-04-29 17:22:28.000000 docgraph-0.0.10.dev0/common/__init__.py
--rw-rw-r--   0 blarson   (1152) rnd      (10001)      612 2024-04-29 17:22:28.000000 docgraph-0.0.10.dev0/common/logging_utils.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)    19884 2024-04-29 17:22:28.000000 docgraph-0.0.10.dev0/common/openapi.py
--rw-rw-r--   0 blarson   (1152) rnd      (10001)     6452 2024-04-29 17:22:28.000000 docgraph-0.0.10.dev0/common/utils.py
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:43:35.676747 docgraph-0.0.10.dev0/docgraph/
--rw-r--r--   0 blarson   (1152) rnd      (10001)        0 2024-04-29 20:53:16.000000 docgraph-0.0.10.dev0/docgraph/__init__.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1120 2024-04-29 23:08:23.000000 docgraph-0.0.10.dev0/docgraph/__main__.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)     2022 2024-04-29 17:22:28.000000 docgraph-0.0.10.dev0/docgraph/jsonutil.py
--rw-r--r--   0 blarson   (1152) rnd      (10001)      625 2024-04-29 23:25:39.000000 docgraph-0.0.10.dev0/docgraph/version.py
-drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 16:43:35.703566 docgraph-0.0.10.dev0/docgraph.egg-info/
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1946 2024-05-01 16:43:35.000000 docgraph-0.0.10.dev0/docgraph.egg-info/PKG-INFO
--rw-r--r--   0 blarson   (1152) rnd      (10001)      337 2024-05-01 16:43:35.000000 docgraph-0.0.10.dev0/docgraph.egg-info/SOURCES.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)        1 2024-05-01 16:43:35.000000 docgraph-0.0.10.dev0/docgraph.egg-info/dependency_links.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       29 2024-05-01 16:43:35.000000 docgraph-0.0.10.dev0/docgraph.egg-info/requires.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       16 2024-05-01 16:43:35.000000 docgraph-0.0.10.dev0/docgraph.egg-info/top_level.txt
--rw-r--r--   0 blarson   (1152) rnd      (10001)       38 2024-05-01 16:43:35.713079 docgraph-0.0.10.dev0/setup.cfg
--rw-r--r--   0 blarson   (1152) rnd      (10001)     1330 2024-05-01 16:42:39.000000 docgraph-0.0.10.dev0/setup.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 18:51:36.353371 docgraph-0.0.14.dev0/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     2685 2024-05-01 18:51:36.351611 docgraph-0.0.14.dev0/PKG-INFO
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1537 2024-05-01 18:48:15.000000 docgraph-0.0.14.dev0/README.md
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 18:51:36.288425 docgraph-0.0.14.dev0/common/
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)       79 2024-04-29 17:22:28.000000 docgraph-0.0.14.dev0/common/__init__.py
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)      612 2024-04-29 17:22:28.000000 docgraph-0.0.14.dev0/common/logging_utils.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)    19884 2024-04-29 17:22:28.000000 docgraph-0.0.14.dev0/common/openapi.py
+-rw-rw-r--   0 blarson   (1152) rnd      (10001)     6452 2024-04-29 17:22:28.000000 docgraph-0.0.14.dev0/common/utils.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 18:51:36.313741 docgraph-0.0.14.dev0/docgraph/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)        0 2024-04-29 20:53:16.000000 docgraph-0.0.14.dev0/docgraph/__init__.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1120 2024-04-29 23:08:23.000000 docgraph-0.0.14.dev0/docgraph/__main__.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     2022 2024-04-29 17:22:28.000000 docgraph-0.0.14.dev0/docgraph/jsonutil.py
+-rw-r--r--   0 blarson   (1152) rnd      (10001)      625 2024-04-29 23:25:39.000000 docgraph-0.0.14.dev0/docgraph/version.py
+drwxr-xr-x   0 blarson   (1152) rnd      (10001)        0 2024-05-01 18:51:36.344054 docgraph-0.0.14.dev0/docgraph.egg-info/
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     2685 2024-05-01 18:51:36.000000 docgraph-0.0.14.dev0/docgraph.egg-info/PKG-INFO
+-rw-r--r--   0 blarson   (1152) rnd      (10001)      337 2024-05-01 18:51:36.000000 docgraph-0.0.14.dev0/docgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)        1 2024-05-01 18:51:36.000000 docgraph-0.0.14.dev0/docgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       29 2024-05-01 18:51:36.000000 docgraph-0.0.14.dev0/docgraph.egg-info/requires.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       16 2024-05-01 18:51:36.000000 docgraph-0.0.14.dev0/docgraph.egg-info/top_level.txt
+-rw-r--r--   0 blarson   (1152) rnd      (10001)       38 2024-05-01 18:51:36.354905 docgraph-0.0.14.dev0/setup.cfg
+-rw-r--r--   0 blarson   (1152) rnd      (10001)     1330 2024-05-01 16:42:39.000000 docgraph-0.0.14.dev0/setup.py
```

### Comparing `docgraph-0.0.10.dev0/README.md` & `docgraph-0.0.14.dev0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -23,12 +23,30 @@
     py setup.py sdist bdist_wheel
     ```
 
 - Upload package to pipy
     ```cmd
     twine upload dist/*
 
+- pip install:
+    ```cmd
+    pip install --extra-index-url https://ha-us.dso.thermofisher.net/artifactory/api/pypi/sci-ai-pypi-internal-local/simple --trusted-host ha-us.dso.thermofisher.net docgraph==0.0.14-dev 
+    ```
+- reqiurements.txt install:
+    - in requirements.txt:
+        ```txt
+        --extra-index-url https://ha-us.dso.thermofisher.net/artifactory/api/pypi/sci-ai-pypi-internal-local/simple --trusted-host ha-us.dso.thermofisher.net
+        ...
+        docgraph==0.0.14-dev 
+        ```
+    - from the console:
+        ```
+        pip install -r requirements.txt
+        ```
+
+
+
 ## Constants
 
 ## Functions
 
 ## Classes
```

### Comparing `docgraph-0.0.10.dev0/common/logging_utils.py` & `docgraph-0.0.14.dev0/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/common/openapi.py` & `docgraph-0.0.14.dev0/common/openapi.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/common/utils.py` & `docgraph-0.0.14.dev0/common/utils.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/docgraph/__main__.py` & `docgraph-0.0.14.dev0/docgraph/__main__.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/docgraph/jsonutil.py` & `docgraph-0.0.14.dev0/docgraph/jsonutil.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/docgraph/version.py` & `docgraph-0.0.14.dev0/docgraph/version.py`

 * *Files identical despite different names*

### Comparing `docgraph-0.0.10.dev0/setup.py` & `docgraph-0.0.14.dev0/setup.py`

 * *Files identical despite different names*

