# Comparing `tmp/logkontrol-0.1.0.tar.gz` & `tmp/logkontrol-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkontrol-0.1.0.tar", last modified: Tue Apr 30 23:28:56 2024, max compression
+gzip compressed data, was "logkontrol-0.1.1.tar", last modified: Wed May  1 03:13:03 2024, max compression
```

## Comparing `logkontrol-0.1.0.tar` & `logkontrol-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-04-30 23:28:56.010125 logkontrol-0.1.0/
--rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.1.0/LICENSE
--rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.1.0/LICENSE_PYYAML.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)     3695 2024-04-30 23:28:56.006791 logkontrol-0.1.0/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)     3101 2024-04-30 22:54:31.000000 logkontrol-0.1.0/README.md
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-04-30 23:28:56.006791 logkontrol-0.1.0/logkontrol/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.1.0/logkontrol/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)    10220 2024-04-30 22:54:38.000000 logkontrol-0.1.0/logkontrol/log_kontrol.py
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-04-30 23:28:56.006791 logkontrol-0.1.0/logkontrol.egg-info/
--rw-r--r--   0 rsp       (1000) wheel      (998)     3695 2024-04-30 23:28:56.000000 logkontrol-0.1.0/logkontrol.egg-info/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)      313 2024-04-30 23:28:56.000000 logkontrol-0.1.0/logkontrol.egg-info/SOURCES.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-04-30 23:28:56.000000 logkontrol-0.1.0/logkontrol.egg-info/dependency_links.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-04-30 23:28:56.000000 logkontrol-0.1.0/logkontrol.egg-info/requires.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-04-30 23:28:56.000000 logkontrol-0.1.0/logkontrol.egg-info/top_level.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-04-30 23:28:51.000000 logkontrol-0.1.0/pyproject.toml
--rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-04-30 23:28:56.010125 logkontrol-0.1.0/setup.cfg
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-04-30 23:28:56.006791 logkontrol-0.1.0/tests/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.0/tests/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.0/tests/test_log_kontrol.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/
+-rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.1.1/LICENSE
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.1.1/LICENSE_PYYAML.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 03:13:03.220450 logkontrol-0.1.1/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 03:11:40.000000 logkontrol-0.1.1/README.md
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/logkontrol/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.1.1/logkontrol/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)    10220 2024-04-30 22:54:38.000000 logkontrol-0.1.1/logkontrol/logkontrol.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/logkontrol.egg-info/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)      338 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/requires.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/top_level.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 03:12:53.000000 logkontrol-0.1.1/pyproject.toml
+-rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 03:13:03.220450 logkontrol-0.1.1/setup.cfg
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/tests/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.1/tests/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.1/tests/test_log_kontrol.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)      198 2024-04-30 23:44:48.000000 logkontrol-0.1.1/tests/test_placeholder.py
```

### Comparing `logkontrol-0.1.0/LICENSE_PYYAML.txt` & `logkontrol-0.1.1/LICENSE_PYYAML.txt`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.0/PKG-INFO` & `logkontrol-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.file_logger import init_logging, log_message
+from logkontrol.logkontrol import init_logging, log_message
 
 # Initialize the logging system
 init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
```

### Comparing `logkontrol-0.1.0/README.md` & `logkontrol-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.file_logger import init_logging, log_message
+from logkontrol.logkontrol import init_logging, log_message
 
 # Initialize the logging system
 init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
```

### Comparing `logkontrol-0.1.0/logkontrol/log_kontrol.py` & `logkontrol-0.1.1/logkontrol/logkontrol.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.0/logkontrol.egg-info/PKG-INFO` & `logkontrol-0.1.1/logkontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.file_logger import init_logging, log_message
+from logkontrol.logkontrol import init_logging, log_message
 
 # Initialize the logging system
 init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
```

### Comparing `logkontrol-0.1.0/pyproject.toml` & `logkontrol-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logkontrol"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "voidfemme", email = "rosemkatt@gmail.com" }
 ]
 description = "Custom file logging system for Python applications"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

