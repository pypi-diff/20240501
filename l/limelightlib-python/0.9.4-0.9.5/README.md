# Comparing `tmp/limelightlib_python-0.9.4.tar.gz` & `tmp/limelightlib_python-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limelightlib_python-0.9.4.tar", last modified: Wed Apr 24 22:25:04 2024, max compression
+gzip compressed data, was "limelightlib_python-0.9.5.tar", last modified: Wed May  1 02:59:36 2024, max compression
```

## Comparing `limelightlib_python-0.9.4.tar` & `limelightlib_python-0.9.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:25:04.251174 limelightlib_python-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-24 22:25:04.251174 limelightlib_python-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 22:24:58.000000 limelightlib_python-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:25:04.251174 limelightlib_python-0.9.4/limelightlib-python/
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 22:24:58.000000 limelightlib_python-0.9.4/limelightlib-python/limelight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:25:04.251174 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-24 22:25:04.000000 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 22:25:04.000000 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:25:04.000000 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:25:04.000000 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 22:25:04.000000 limelightlib_python-0.9.4/limelightlib-python/limelightlib_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 22:24:58.000000 limelightlib_python-0.9.4/limelightlib-python/limelightresults.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:25:04.251174 limelightlib_python-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 22:24:58.000000 limelightlib_python-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:59:36.449719 limelightlib_python-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-01 02:59:36.449719 limelightlib_python-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-01 02:59:30.000000 limelightlib_python-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:59:36.449719 limelightlib_python-0.9.5/limelightlib-python/
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-05-01 02:59:30.000000 limelightlib_python-0.9.5/limelightlib-python/limelight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 02:59:36.449719 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-01 02:59:36.000000 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 02:59:36.000000 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 02:59:36.000000 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 02:59:36.000000 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 02:59:36.000000 limelightlib_python-0.9.5/limelightlib-python/limelightlib_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-01 02:59:30.000000 limelightlib_python-0.9.5/limelightlib-python/limelightresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 02:59:36.449719 limelightlib_python-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 02:59:30.000000 limelightlib_python-0.9.5/setup.py
```

### Comparing `limelightlib_python-0.9.4/limelightlib-python/limelightresults.py` & `limelightlib_python-0.9.5/limelightlib-python/limelightresults.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,13 @@
         self.class_id = classifier_data["classID"]
         self.confidence = classifier_data["conf"]
 
 
 def parse_results(json_data):
     start_time = time.time()
     if(json_data is not None):
-        results_data = json_data.get("Results", {})
-        parsed_result = GeneralResult(results_data)
+        parsed_result = GeneralResult(json_data)
         end_time = time.time()
         elapsed_time_ms = (end_time - start_time) * 1000
         parsed_result.parse_latency = elapsed_time_ms
         return parsed_result
-    return None
+    return None
```

### Comparing `limelightlib_python-0.9.4/setup.py` & `limelightlib_python-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
 name='limelightlib-python',
-version='0.9.4',
+version='0.9.5',
 url='https://limelightvision.io',
 author='Brandon Hjelstrom',
 author_email='brandon@limelightvision.io',
 description='Built to interface with any Limelight Smart Camera',
 long_description=long_description,
 long_description_content_type="text/markdown",
 py_modules=["limelight", "limelightresults"],
```

