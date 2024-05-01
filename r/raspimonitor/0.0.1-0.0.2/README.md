# Comparing `tmp/raspimonitor-0.0.1.tar.gz` & `tmp/raspimonitor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspimonitor-0.0.1.tar", last modified: Mon Apr 15 14:56:54 2024, max compression
+gzip compressed data, was "raspimonitor-0.0.2.tar", last modified: Wed May  1 10:17:47 2024, max compression
```

## Comparing `raspimonitor-0.0.1.tar` & `raspimonitor-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:56:54.870294 raspimonitor-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 14:56:54.870294 raspimonitor-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:56:54.866294 raspimonitor-0.0.1/raspimonitor/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/raspimonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-15 14:56:46.000000 raspimonitor-0.0.1/raspimonitor/raspimonitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:56:54.866294 raspimonitor-0.0.1/raspimonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 14:56:54.000000 raspimonitor-0.0.1/raspimonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:56:54.870294 raspimonitor-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.222353 raspimonitor-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-01 10:17:47.222353 raspimonitor-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.218353 raspimonitor-0.0.2/raspimonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/raspimonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/raspimonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-01 10:17:41.000000 raspimonitor-0.0.2/raspimonitor/raspimonitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:17:47.218353 raspimonitor-0.0.2/raspimonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 10:17:47.000000 raspimonitor-0.0.2/raspimonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:17:47.222353 raspimonitor-0.0.2/setup.cfg
```

### Comparing `raspimonitor-0.0.1/LICENSE` & `raspimonitor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspimonitor-0.0.1/PKG-INFO` & `raspimonitor-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspimonitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Monitoring and alerting for your RaspberryPi 
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/raspimonitor
 Project-URL: Repository, https://github.com/w0rmr1d3r/raspimonitor
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/raspimonitor/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/raspimonitor
@@ -22,15 +22,15 @@
 Requires-Python: ~=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.0
 Provides-Extra: dev
 Requires-Dist: pip-tools~=7.0; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
-Requires-Dist: ruff==0.3.1; extra == "dev"
+Requires-Dist: ruff==0.3.7; extra == "dev"
 
 # raspimonitor
 
 Monitoring and alerting to your Discord server for your RaspberryPi
 
 ## Installation
```

### Comparing `raspimonitor-0.0.1/README.md` & `raspimonitor-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `raspimonitor-0.0.1/pyproject.toml` & `raspimonitor-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
 ]
 # Make this keywords match the ones in GitHub
 keywords = ["raspberry", "raspberrypi", "pi", "monitor"]
 
-version = "0.0.1"
+version = "0.0.2"
 # Minumum supported version
 # If supporting newer versions, update ->  CI and classifiers
 # If minimum supported version changes, update -> CI, release and classifiers.
 requires-python = "~=3.9.0"
 
 dependencies = [
     "requests~=2.0"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pip-tools~=7.0",
     "pytest~=8.0",
-    "ruff==0.3.1",
+    "ruff==0.3.7",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/w0rmr1d3r/raspimonitor"
 "Repository" = "https://github.com/w0rmr1d3r/raspimonitor"
 "Bug Tracker" = "https://github.com/w0rmr1d3r/raspimonitor/issues"
 "Documentation" = "https://github.com/w0rmr1d3r/raspimonitor"
```

### Comparing `raspimonitor-0.0.1/raspimonitor/raspimonitor.py` & `raspimonitor-0.0.2/raspimonitor/raspimonitor.py`

 * *Files identical despite different names*

### Comparing `raspimonitor-0.0.1/raspimonitor.egg-info/PKG-INFO` & `raspimonitor-0.0.2/raspimonitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspimonitor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Monitoring and alerting for your RaspberryPi 
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/raspimonitor
 Project-URL: Repository, https://github.com/w0rmr1d3r/raspimonitor
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/raspimonitor/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/raspimonitor
@@ -22,15 +22,15 @@
 Requires-Python: ~=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.0
 Provides-Extra: dev
 Requires-Dist: pip-tools~=7.0; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
-Requires-Dist: ruff==0.3.1; extra == "dev"
+Requires-Dist: ruff==0.3.7; extra == "dev"
 
 # raspimonitor
 
 Monitoring and alerting to your Discord server for your RaspberryPi
 
 ## Installation
```

