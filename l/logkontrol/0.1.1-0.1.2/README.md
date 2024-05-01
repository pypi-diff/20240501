# Comparing `tmp/logkontrol-0.1.1.tar.gz` & `tmp/logkontrol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkontrol-0.1.1.tar", last modified: Wed May  1 03:13:03 2024, max compression
+gzip compressed data, was "logkontrol-0.1.2.tar", last modified: Wed May  1 14:01:32 2024, max compression
```

## Comparing `logkontrol-0.1.1.tar` & `logkontrol-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/
--rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.1.1/LICENSE
--rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.1.1/LICENSE_PYYAML.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 03:13:03.220450 logkontrol-0.1.1/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 03:11:40.000000 logkontrol-0.1.1/README.md
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/logkontrol/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.1.1/logkontrol/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)    10220 2024-04-30 22:54:38.000000 logkontrol-0.1.1/logkontrol/logkontrol.py
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/logkontrol.egg-info/
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)      338 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/SOURCES.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/dependency_links.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/requires.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 03:13:03.000000 logkontrol-0.1.1/logkontrol.egg-info/top_level.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 03:12:53.000000 logkontrol-0.1.1/pyproject.toml
--rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 03:13:03.220450 logkontrol-0.1.1/setup.cfg
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 03:13:03.220450 logkontrol-0.1.1/tests/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.1/tests/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:45.000000 logkontrol-0.1.1/tests/test_log_kontrol.py
--rw-r--r--   0 rsp       (1000) wheel      (998)      198 2024-04-30 23:44:48.000000 logkontrol-0.1.1/tests/test_placeholder.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/
+-rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.1.2/LICENSE
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.1.2/LICENSE_PYYAML.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 14:01:32.812979 logkontrol-0.1.2/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 05:01:50.000000 logkontrol-0.1.2/README.md
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/logkontrol/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.1.2/logkontrol/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)    11283 2024-05-01 13:59:33.000000 logkontrol-0.1.2/logkontrol/logkontrol.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/logkontrol.egg-info/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)      552 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/requires.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/top_level.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 13:59:33.000000 logkontrol-0.1.2/pyproject.toml
+-rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 14:01:32.812979 logkontrol-0.1.2/setup.cfg
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/tests/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 13:22:37.000000 logkontrol-0.1.2/tests/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2522 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_init_logging.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2175 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_initialize_log_file.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1825 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_load_logging_config.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2702 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_function_call.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2932 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_json_content.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1900 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_message.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2533 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_variable.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_logkontrol.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)      833 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_truncate_string.py
```

### Comparing `logkontrol-0.1.1/LICENSE_PYYAML.txt` & `logkontrol-0.1.2/LICENSE_PYYAML.txt`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.1/PKG-INFO` & `logkontrol-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `logkontrol-0.1.1/README.md` & `logkontrol-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.1/logkontrol/logkontrol.py` & `logkontrol-0.1.2/logkontrol/logkontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,20 +288,46 @@
     log_entry += "\n"
 
     with open(log_file_path, "a") as log_file:
         log_file.write(log_entry)
 
 
 def load_logging_konfig(konfig_file_path: str):
+    """
+    Easter Egg function! Loads the logging configuration from a YAML file.
+
+    Args:
+        konfig_file_path (str): The path to the logging configuration file.
+
+    Returns:
+        dict: The loaded logging configuration.
+    """
     return load_logging_config(konfig_file_path)
 
 
 def log_funktion_kall(
     log_file_key: str, funktion_name: str, log_level: str = "DEBUG", **kwargs
 ):
+    """
+    Easter Egg function! Logs a function call with its arguments.
+
+    Args:
+        log_file_key (str): The key of the log file path in the logging configuration.
+        funktion_name (str): The name of the function being called.
+        log_level (str, optional): The log level of the function call. Defaults to "DEBUG".
+        **kwargs: Keyword arguments representing the function's arguments.
+    """
     return log_function_call(log_file_key, funktion_name, log_level, **kwargs)
 
 
 def log_json_kontent(
     log_file_key: str, json_kontent: dict | list[dict], log_level: str = "DEBUG"
 ):
+    """
+    Easter Egg function! Logs the content of a JSON object or a list of JSON objects in a pretty-printed format.
+
+    Args:
+        log_file_key (str): The key of the log file path in the logging configuration.
+        json_kontent (dict | list[dict]): The JSON object or list of JSON objects to log.
+        log_level (str, optional): The log level of the JSON content. Defaults to "DEBUG".
+    """
     return log_json_content(log_file_key, json_kontent, log_level)
```

### Comparing `logkontrol-0.1.1/logkontrol.egg-info/PKG-INFO` & `logkontrol-0.1.2/logkontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `logkontrol-0.1.1/pyproject.toml` & `logkontrol-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logkontrol"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "voidfemme", email = "rosemkatt@gmail.com" }
 ]
 description = "Custom file logging system for Python applications"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

