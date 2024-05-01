# Comparing `tmp/logkontrol-0.1.2.tar.gz` & `tmp/logkontrol-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkontrol-0.1.2.tar", last modified: Wed May  1 14:01:32 2024, max compression
+gzip compressed data, was "logkontrol-0.2.0.tar", last modified: Wed May  1 18:16:52 2024, max compression
```

## Comparing `logkontrol-0.1.2.tar` & `logkontrol-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/
--rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.1.2/LICENSE
--rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.1.2/LICENSE_PYYAML.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 14:01:32.812979 logkontrol-0.1.2/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 05:01:50.000000 logkontrol-0.1.2/README.md
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/logkontrol/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.1.2/logkontrol/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)    11283 2024-05-01 13:59:33.000000 logkontrol-0.1.2/logkontrol/logkontrol.py
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/logkontrol.egg-info/
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)      552 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/SOURCES.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/dependency_links.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/requires.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 14:01:32.000000 logkontrol-0.1.2/logkontrol.egg-info/top_level.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 13:59:33.000000 logkontrol-0.1.2/pyproject.toml
--rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 14:01:32.812979 logkontrol-0.1.2/setup.cfg
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:01:32.812979 logkontrol-0.1.2/tests/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 13:22:37.000000 logkontrol-0.1.2/tests/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2522 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_init_logging.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2175 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_initialize_log_file.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     1825 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_load_logging_config.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2702 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_function_call.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2932 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_json_content.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     1900 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_message.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2533 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_log_variable.py
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_logkontrol.py
--rw-r--r--   0 rsp       (1000) wheel      (998)      833 2024-05-01 13:59:33.000000 logkontrol-0.1.2/tests/test_truncate_string.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/
+-rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.2.0/LICENSE
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.2.0/LICENSE_PYYAML.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 18:16:52.826857 logkontrol-0.2.0/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 05:01:50.000000 logkontrol-0.2.0/README.md
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/logkontrol/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.2.0/logkontrol/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)    12915 2024-05-01 18:12:44.000000 logkontrol-0.2.0/logkontrol/logkontrol.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/logkontrol.egg-info/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)      534 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/requires.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/top_level.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 18:11:29.000000 logkontrol-0.2.0/pyproject.toml
+-rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 18:16:52.830190 logkontrol-0.2.0/setup.cfg
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/tests/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2603 2024-05-01 18:06:57.000000 logkontrol-0.2.0/tests/test_init_logging.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2305 2024-05-01 18:06:19.000000 logkontrol-0.2.0/tests/test_initialize_log_file.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1947 2024-05-01 18:07:21.000000 logkontrol-0.2.0/tests/test_load_logging_config.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2491 2024-05-01 18:07:58.000000 logkontrol-0.2.0/tests/test_log_function_call.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2624 2024-05-01 18:08:40.000000 logkontrol-0.2.0/tests/test_log_json_content.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2369 2024-05-01 18:09:13.000000 logkontrol-0.2.0/tests/test_log_message.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2328 2024-05-01 18:09:45.000000 logkontrol-0.2.0/tests/test_log_variable.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:26:29.000000 logkontrol-0.2.0/tests/test_logkontrol.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)      833 2024-05-01 18:09:53.000000 logkontrol-0.2.0/tests/test_truncate_string.py
```

### Comparing `logkontrol-0.1.2/LICENSE_PYYAML.txt` & `logkontrol-0.2.0/LICENSE_PYYAML.txt`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.2/PKG-INFO` & `logkontrol-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.2
+Version: 0.2.0
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `logkontrol-0.1.2/README.md` & `logkontrol-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `logkontrol-0.1.2/logkontrol/logkontrol.py` & `logkontrol-0.2.0/logkontrol/logkontrol.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,76 +5,125 @@
 import json
 from pathlib import Path
 from typing import Any
 import yaml
 from datetime import datetime
 
 
-logging_config = None
-
+class LogKonfig:
+    _instance = None
+    _logging_config = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+        return cls._instance
+
+    def init_logging(
+        self, config_file_path: str | None = None, log_directory: str = "logs"
+    ) -> None:
+        """
+        Initializes the logging configuration.
+
+        Args:
+            config_file_path (str | None, optional): The path to the logging configuration file.
+                If not provided, defaults to "logging_config.yaml".
+            log_directory (str, optional): The directory where log files will be stored.
+                Defaults to "logs".
+        """
+        if config_file_path is None:
+            config_file_path = "logging_config.yaml"
+
+        if not os.path.exists(config_file_path):
+            # Create the log directory if it doesn't exist
+            os.makedirs(log_directory, exist_ok=True)
+
+            # Generate a default YAML configuration
+            default_config = {
+                "log_file_paths": {
+                    "general": f"{log_directory}/general.log",
+                },
+                "log_format": "[{timestamp}] [{level}] {message}",
+                "timestamp_format": "%Y-%m-%d %H:%M:%S",
+                "log_level": "INFO",
+                "console_output": True,
+            }
+
+            # Write the default configuration to the YAML file
+            with open(config_file_path, "w") as config_file:
+                yaml.dump(default_config, config_file)
+
+        # Load the logging configuration from the YAML file
+        self._logging_config = self.load_logging_config(config_file_path)
+
+        # Initialize the log files if the logging configuration is loaded successfully
+        if self._logging_config is not None:
+            for log_file_key in self._logging_config["log_file_paths"]:
+                self.initialize_log_file(log_file_key)
+
+    def get_logging_config(self) -> dict | None:
+        return self._logging_config
+
+    def set_logging_config(self, config: dict) -> None:
+        self._logging_config = config
+
+    @staticmethod
+    def load_logging_config(config_file_path: str) -> dict:
+        """
+        Loads the logging configuration from a YAML file.
+
+        Args:
+            config_file_path (str): The path to the logging configuration file.
+
+        Returns:
+            dict: The loaded logging configuration.
+        """
+        config_path = Path(config_file_path)
+        with open(config_path, "r") as config_file:
+            config = yaml.safe_load(config_file)
+        return config
+
+    def initialize_log_file(self, log_file_key: str | None) -> None:
+        """
+        Initializes the log file by creating it if it doesn't exist and adding a header.
+
+        Args:
+            log_file_key (str): The key of the log file path in the logging configuration.
+        """
+        if self._logging_config is None:
+            raise ValueError(
+                "Logging configuration is not initialized. Please call init_logging() first"
+            )
+
+        # Check if log_file_key is not provided and if only one log path is configured
+        if log_file_key is None:
+            keys = list(self._logging_config["log_file_paths"].keys())
+            if len(keys) == 1:
+                log_file_key = keys[0]
+            else:
+                print("Multiple log files configured, please specify a log_file_key.")
+                return
 
-def init_logging(config_file_path: str | None = None, log_directory: str = "logs"):
-    """
-    Initializes the logging configuration.
+        log_file_path = self._logging_config["log_file_paths"][log_file_key]
+        if not os.path.exists(log_file_path):
+            with open(log_file_path, "w") as log_file:
+                log_file.write("Log File Initialized\n\n")
 
-    Args:
-        config_file_path (str | None, optional): The path to the logging configuration file.
-            If not provided, defaults to "logging_config.yaml".
-        log_directory (str, optional): The directory where log files will be stored.
-            Defaults to "logs".
-    """
-    global logging_config
-
-    if config_file_path is None:
-        config_file_path = "logging_config.yaml"
-
-    if not os.path.exists(config_file_path):
-        # Create the log directory if it doesn't exist
-        os.makedirs(log_directory, exist_ok=True)
-
-        # Generate a default YAML configuration
-        default_config = {
-            "log_file_paths": {
-                "general": f"{log_directory}/general.log",
-            },
-            "log_format": "[{timestamp}] [{level}] {message}",
-            "timestamp_format": "%Y-%m-%d %H:%M:%S",
-            "log_level": "INFO",
-            "console_output": True,
-        }
-
-        # Write the default configuration to the YAML file
-        with open(config_file_path, "w") as config_file:
-            yaml.dump(default_config, config_file)
-
-    # Load the logging configuration from the YAML file
-    logging_config = load_logging_config(config_file_path)
-
-    # Initialize the log files
-    for log_file_key in logging_config["log_file_paths"]:
-        initialize_log_file(log_file_key)
 
-
-def load_logging_config(config_file_path: str):
+def initialize_log_file(log_file_key: str | None) -> None:
     """
-    Loads the logging configuration from a YAML file.
+    Initializes the log file by creating it if it doesn't exist and adding a header.
 
     Args:
-        config_file_path (str): The path to the logging configuration file.
-
-    Returns:
-        dict: The loaded logging configuration.
+        log_file_key (str): The key of the log file path in the logging configuration.
     """
-    config_path = Path(config_file_path)
-    with open(config_path, "r") as config_file:
-        config = yaml.safe_load(config_file)
-    return config
+    pass
 
 
-def truncate_string(value: Any, max_length: int = 500):
+def truncate_string(value: Any, max_length: int = 500) -> str:
     """
     Truncates a string to a maximum length and appends "..." if truncated.
 
     Args:
         value: The value to truncate.
         max_length (int, optional): The maximum length of the truncated string.
 
@@ -88,26 +137,27 @@
 
 
 def log_message(
     log_file_key: str | None,
     message: str | None = None,
     variables: dict | None = None,
     log_level: str = "DEBUG",
-):
+) -> None:
     """
     Logs a message and/or variable values to a file.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         message (str, optional): The message to log. Defaults to None.
         variables (dict, optional): A dictionary of variables and their values to log.
             Defaults to None.
         log_level (str, optional): The log level of the message. Defaults to "DEBUG".
     """
 
+    logging_config = LogKonfig().get_logging_config()
     if logging_config is None:
         print(
             "Logging configuration is not initialized. Please call init_logging() first."
         )
         return
 
     # Check if log_file_key is not provided and if only one log path is configured
@@ -140,24 +190,25 @@
     else:
         with open(log_file_path, "a") as log_file:
             log_file.write(log_entry)
 
 
 def log_function_call(
     log_file_key: str | None, function_name: str, log_level: str = "DEBUG", **kwargs
-):
+) -> None:
     """
     Logs a function call with its arguments.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         function_name (str): The name of the function being called.
         log_level (str, optional): The log level of the function call. Defaults to "DEBUG".
         **kwargs: Keyword arguments representing the function's arguments.
     """
+    logging_config = LogKonfig().get_logging_config()
     if logging_config is None:
         print(
             "Logging configuration is not initialized. Please call init_logging() first."
         )
         return
 
     # Check if log_file_key is not provided and if only one log path is configured
@@ -178,24 +229,25 @@
 
 
 def log_variable(
     log_file_key: str | None,
     variable_name: str,
     variable_value: Any,
     log_level: str = "DEBUG",
-):
+) -> None:
     """
     Logs a variable and its value.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         variable_name (str): The name of the variable.
         variable_value: The value of the variable.
         log_level (str, optional): The log level of the variable. Defaults to "DEBUG".
     """
+    logging_config = LogKonfig().get_logging_config()
     if logging_config is None:
         print(
             "Logging configuration is not initialized. Please call init_logging() first."
         )
         return
 
     # Check if log_file_key is not provided and if only one log path is configured
@@ -210,53 +262,26 @@
     if log_level == "TRUNCATED":
         variable_value = truncate_string(variable_value)
     log_message(
         log_file_key, variables={variable_name: variable_value}, log_level=log_level
     )
 
 
-def initialize_log_file(log_file_key: str | None):
-    """
-    Initializes the log file by creating it if it doesn't exist and adding a header.
-
-    Args:
-        log_file_key (str): The key of the log file path in the logging configuration.
-    """
-    if logging_config is None:
-        print(
-            "Logging configuration is not initialized. Please call init_logging() first."
-        )
-        return
-
-    # Check if log_file_key is not provided and if only one log path is configured
-    if log_file_key is None:
-        keys = list(logging_config["log_file_paths"].keys())
-        if len(keys) == 1:
-            log_file_key = keys[0]
-        else:
-            print("Multiple log files configured, please specify a log_file_key.")
-            return
-
-    log_file_path = logging_config["log_file_paths"][log_file_key]
-    if not os.path.exists(log_file_path):
-        with open(log_file_path, "w") as log_file:
-            log_file.write("Log File Initialized\n\n")
-
-
 def log_json_content(
     log_file_key: str | None, json_content: dict | list[dict], log_level: str = "DEBUG"
-):
+) -> None:
     """
     Logs the content of a JSON object or a list of JSON objects in a pretty-printed format.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         json_content (dict | list[dict]): The JSON object or list of JSON objects to log.
         log_level (str, optional): The log level of the JSON content. Defaults to "DEBUG".
     """
+    logging_config = LogKonfig().get_logging_config()
     if logging_config is None:
         print(
             "Logging configuration is not initialized. Please call init_logging() first."
         )
         return
 
     # Check if log_file_key is not provided and if only one log path is configured
@@ -287,47 +312,60 @@
 
     log_entry += "\n"
 
     with open(log_file_path, "a") as log_file:
         log_file.write(log_entry)
 
 
-def load_logging_konfig(konfig_file_path: str):
+def load_logging_config(config_file_path: str) -> dict:
     """
-    Easter Egg function! Loads the logging configuration from a YAML file.
+    Loads the logging configuration from a YAML file.
+
+    Args:
+        config_file_path (str): The path to the logging configuration file.
+
+    Returns:
+        dict: The loaded logging configuration.
+    """
+    return LogKonfig.load_logging_config(config_file_path)
+
+
+def load_logging_konfig(konfig_file_path: str) -> dict:
+    """
+    Loads the logging configuration from a YAML file.
 
     Args:
         konfig_file_path (str): The path to the logging configuration file.
 
     Returns:
         dict: The loaded logging configuration.
     """
-    return load_logging_config(konfig_file_path)
+    return LogKonfig.load_logging_config(konfig_file_path)
 
 
 def log_funktion_kall(
     log_file_key: str, funktion_name: str, log_level: str = "DEBUG", **kwargs
-):
+) -> None:
     """
-    Easter Egg function! Logs a function call with its arguments.
+    Logs a function call with its arguments.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         funktion_name (str): The name of the function being called.
         log_level (str, optional): The log level of the function call. Defaults to "DEBUG".
         **kwargs: Keyword arguments representing the function's arguments.
     """
     return log_function_call(log_file_key, funktion_name, log_level, **kwargs)
 
 
 def log_json_kontent(
     log_file_key: str, json_kontent: dict | list[dict], log_level: str = "DEBUG"
-):
+) -> None:
     """
-    Easter Egg function! Logs the content of a JSON object or a list of JSON objects in a pretty-printed format.
+    Logs the content of a JSON object or a list of JSON objects in a pretty-printed format.
 
     Args:
         log_file_key (str): The key of the log file path in the logging configuration.
         json_kontent (dict | list[dict]): The JSON object or list of JSON objects to log.
         log_level (str, optional): The log level of the JSON content. Defaults to "DEBUG".
     """
     return log_json_content(log_file_key, json_kontent, log_level)
```

### Comparing `logkontrol-0.1.2/logkontrol.egg-info/PKG-INFO` & `logkontrol-0.2.0/logkontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.1.2
+Version: 0.2.0
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `logkontrol-0.1.2/logkontrol.egg-info/SOURCES.txt` & `logkontrol-0.2.0/logkontrol.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 logkontrol/__init__.py
 logkontrol/logkontrol.py
 logkontrol.egg-info/PKG-INFO
 logkontrol.egg-info/SOURCES.txt
 logkontrol.egg-info/dependency_links.txt
 logkontrol.egg-info/requires.txt
 logkontrol.egg-info/top_level.txt
-tests/__init__.py
 tests/test_init_logging.py
 tests/test_initialize_log_file.py
 tests/test_load_logging_config.py
 tests/test_log_function_call.py
 tests/test_log_json_content.py
 tests/test_log_message.py
 tests/test_log_variable.py
```

### Comparing `logkontrol-0.1.2/pyproject.toml` & `logkontrol-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logkontrol"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     { name = "voidfemme", email = "rosemkatt@gmail.com" }
 ]
 description = "Custom file logging system for Python applications"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `logkontrol-0.1.2/tests/test_init_logging.py` & `logkontrol-0.2.0/tests/test_init_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import unittest
 from unittest.mock import patch
 from logkontrol import logkontrol
 
 
 class TestInitLogging(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = logkontrol.LogKonfig()
         self.default_config_path = "logging_config.yaml"
         self.default_log_directory = "logs"
         self.custom_config_path = "custom_config.yaml"
         self.custom_log_directory = "custom_logs"
 
     def tearDown(self):
         # Clean up generated files and directories after each test
@@ -26,34 +27,34 @@
         if os.path.exists(self.custom_log_directory):
             for file in os.listdir(self.custom_log_directory):
                 os.remove(os.path.join(self.custom_log_directory, file))
             os.rmdir(self.custom_log_directory)
 
     def test_default_config_creation(self):
         # Test case: Configuration file doesn't exist
-        logkontrol.init_logging()
+        self.log_konfig.init_logging()
         self.assertTrue(os.path.exists(self.default_config_path))
         self.assertTrue(os.path.exists(self.default_log_directory))
 
-    @patch("logkontrol.logkontrol.load_logging_config")
+    @patch.object(logkontrol.LogKonfig, "load_logging_config")
     def test_existing_config_loading(self, mock_load_config):
         # Test case: Configuration file exists
         with open(self.default_config_path, "w") as file:
             file.write("# Existing configuration")
-        logkontrol.init_logging()
+        self.log_konfig.init_logging()
         mock_load_config.assert_called_once_with(self.default_config_path)
 
     def test_custom_config_path(self):
         # Test case: Custom configuration file path
-        logkontrol.init_logging(config_file_path=self.custom_config_path)
+        self.log_konfig.init_logging(config_file_path=self.custom_config_path)
         self.assertTrue(os.path.exists(self.custom_config_path))
 
     def test_custom_log_directory(self):
         # Test case: Custom log directory
-        logkontrol.init_logging(log_directory=self.custom_log_directory)
+        self.log_konfig.init_logging(log_directory=self.custom_log_directory)
         self.assertTrue(os.path.exists(self.custom_log_directory))
 
     @patch("builtins.open", side_effect=IOError("Failed to open file"))
     def test_invalid_config_file(self, mock_open):
         # Test case: Invalid configuration file
         with self.assertRaises(IOError):
-            logkontrol.init_logging()
+            self.log_konfig.init_logging()
```

### Comparing `logkontrol-0.1.2/tests/test_initialize_log_file.py` & `logkontrol-0.2.0/tests/test_initialize_log_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 # tests/test_initialize_log_file.py
 
 import os
 import unittest
-from unittest.mock import patch, mock_open
-from logkontrol.logkontrol import initialize_log_file
+from unittest.mock import patch
+from logkontrol.logkontrol import LogKonfig
 
 
 class TestInitializeLogFile(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = LogKonfig()
         self.log_file_key = "test_log"
         self.log_file_path = "test_log.log"
 
     def tearDown(self):
         if os.path.exists(self.log_file_path):
             os.remove(self.log_file_path)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
-    def test_initialize_log_file(self):
-        initialize_log_file(self.log_file_key)
+    def test_initialize_log_file_with_log_konfig(self):
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
+        self.log_konfig.initialize_log_file(self.log_file_key)
         self.assertTrue(os.path.exists(self.log_file_path))
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertEqual(log_content, "Log File Initialized\n\n")
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
-    def test_initialize_existing_log_file(self):
+    def test_initialize_existing_log_file_with_log_konfig(self):
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
         with open(self.log_file_path, "w") as log_file:
             log_file.write("Existing log content\n")
-        initialize_log_file(self.log_file_key)
+        self.log_konfig.initialize_log_file(self.log_file_key)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertEqual(log_content, "Existing log content\n")
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
-    def test_initialize_log_file_without_log_file_key(self):
-        initialize_log_file(None)
+    def test_initialize_log_file_without_log_file_key_with_log_konfig(self):
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
+        self.log_konfig.initialize_log_file(None)
         self.assertTrue(os.path.exists(self.log_file_path))
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertEqual(log_content, "Log File Initialized\n\n")
 
-    @patch("logkontrol.logkontrol.logging_config", None)
-    def test_initialize_log_file_without_logging_config(self):
-        with patch("builtins.print") as mock_print:
-            initialize_log_file(self.log_file_key)
-            mock_print.assert_called_with(
-                "Logging configuration is not initialized. Please call init_logging() first."
-            )
+    def test_initialize_log_file_without_logging_config_with_log_konfig(self):
+        self.log_konfig.set_logging_config(None)  # type: ignore
+        with self.assertRaises(ValueError) as cm:
+            self.log_konfig.initialize_log_file(self.log_file_key)
+        self.assertEqual(
+            str(cm.exception),
+            "Logging configuration is not initialized. Please call init_logging() first",
+        )
```

### Comparing `logkontrol-0.1.2/tests/test_load_logging_config.py` & `logkontrol-0.2.0/tests/test_load_logging_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from unittest.mock import patch, mock_open
 from logkontrol import logkontrol
 import yaml
 
 
 class TestLoadLoggingConfig(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = logkontrol.LogKonfig()
         self.valid_config_path = "valid_config.yaml"
         self.invalid_config_path = "invalid_config.yaml"
         self.nonexistent_config_path = "nonexistent_config.yaml"
 
     def tearDown(self):
         # Clean up generated files after each test
         if os.path.exists(self.valid_config_path):
@@ -26,21 +27,22 @@
             "log_file_paths": {"general": "logs/general.log"},
             "log_format": "[{timestamp}] [{level}] {message}",
             "timestamp_format": "%Y-%m-%d %H:%M:%S",
             "log_level": "INFO",
             "console_output": True,
         }
         with patch("builtins.open", mock_open(read_data=yaml.dump(valid_config))):
-            loaded_config = logkontrol.load_logging_config(self.valid_config_path)
+            loaded_config = self.log_konfig.load_logging_config(self.valid_config_path)
+        self.log_konfig.set_logging_config(loaded_config)
         self.assertEqual(loaded_config, valid_config)
 
     def test_invalid_yaml_config(self):
         # Test case: Invalid YAML configuration file
         invalid_yaml = "invalid: yaml: format"
         with patch("builtins.open", mock_open(read_data=invalid_yaml)):
             with self.assertRaises(yaml.YAMLError):
-                logkontrol.load_logging_config(self.invalid_config_path)
+                self.log_konfig.load_logging_config(self.invalid_config_path)
 
     def test_nonexistent_config_file(self):
         # Test case: Non-existent configuration file
         with self.assertRaises(FileNotFoundError):
-            logkontrol.load_logging_config(self.nonexistent_config_path)
+            self.log_konfig.load_logging_config(self.nonexistent_config_path)
```

### Comparing `logkontrol-0.1.2/tests/test_log_function_call.py` & `logkontrol-0.2.0/tests/test_log_function_call.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 # tests/test_log_function_call.py
 
 import os
 import unittest
-from unittest.mock import patch, mock_open
-from logkontrol.logkontrol import log_function_call, truncate_string
+from unittest.mock import patch
+from logkontrol.logkontrol import LogKonfig, log_function_call, truncate_string
 
 
 class TestLogFunctionCall(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = LogKonfig()
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
         self.log_file_key = "test_log"
         self.log_file_path = "test_log.log"
         self.function_name = "test_function"
         self.log_level = "DEBUG"
         self.kwargs = {"arg1": "value1", "arg2": 123}
 
     def tearDown(self):
         if os.path.exists(self.log_file_path):
             os.remove(self.log_file_path)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_function_call(self):
         log_function_call(self.log_file_key, self.function_name, **self.kwargs)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(f"Function Call: {self.function_name}()", log_content)
         for arg_name, arg_value in self.kwargs.items():
             self.assertIn(f"  {arg_name}: {arg_value}", log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_function_call_with_truncated_level(self):
         long_arg_value = "This is a very long argument value that will be truncated."
         kwargs = {"long_arg": long_arg_value}
         log_function_call(
             self.log_file_key, self.function_name, log_level="TRUNCATED", **kwargs
         )
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(f"Function Call: {self.function_name}()", log_content)
         self.assertIn(f"  long_arg: {truncate_string(long_arg_value)}", log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_function_call_without_log_file_key(self):
         log_function_call(None, self.function_name, **self.kwargs)
         self.assertTrue(os.path.exists(self.log_file_path))
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(f"Function Call: {self.function_name}()", log_content)
 
-    @patch("logkontrol.logkontrol.logging_config", None)
     def test_log_function_call_without_logging_config(self):
+        self.log_konfig.set_logging_config(None)  # type: ignore
         with patch("builtins.print") as mock_print:
             log_function_call(self.log_file_key, self.function_name, **self.kwargs)
             mock_print.assert_called_with(
                 "Logging configuration is not initialized. Please call init_logging() first."
             )
```

### Comparing `logkontrol-0.1.2/tests/test_log_json_content.py` & `logkontrol-0.2.0/tests/test_log_json_content.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 # tests/test_log_json_content.py
 
 import os
 import unittest
 from unittest.mock import patch, mock_open
-from logkontrol.logkontrol import log_json_content
+from logkontrol.logkontrol import LogKonfig, log_json_content
 
 
 class TestLogJsonContent(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = LogKonfig()
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
         self.log_file_key = "test_log"
         self.log_file_path = "test_log.log"
         self.json_object = {"key1": "value1", "key2": {"nested_key": "nested_value"}}
         self.json_list = [{"item1": "value1"}, {"item2": "value2"}]
         self.log_level = "DEBUG"
 
     def tearDown(self):
         if os.path.exists(self.log_file_path):
             os.remove(self.log_file_path)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_json_object(self):
         log_json_content(self.log_file_key, self.json_object)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn("JSON Content:", log_content)
         self.assertIn('"key1": "value1"', log_content)
         self.assertIn('"key2": {', log_content)
         self.assertIn('"nested_key": "nested_value"', log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_json_list(self):
         log_json_content(self.log_file_key, self.json_list)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn("JSON Content:", log_content)
         self.assertIn('"item1": "value1"', log_content)
         self.assertIn('"item2": "value2"', log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_invalid_json_content(self):
         invalid_json = "invalid_json_content"
-        log_json_content(self.log_file_key, invalid_json)
+        log_json_content(self.log_file_key, invalid_json)  # type: ignore
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn("JSON Content:", log_content)
         self.assertIn(invalid_json, log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_json_content_without_log_file_key(self):
         log_json_content(None, self.json_object)
         self.assertTrue(os.path.exists(self.log_file_path))
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn("JSON Content:", log_content)
 
-    @patch("logkontrol.logkontrol.logging_config", None)
     def test_log_json_content_without_logging_config(self):
+        self.log_konfig.set_logging_config(None)  # type: ignore
         with patch("builtins.print") as mock_print:
             log_json_content(self.log_file_key, self.json_object)
             mock_print.assert_called_with(
                 "Logging configuration is not initialized. Please call init_logging() first."
             )
```

### Comparing `logkontrol-0.1.2/tests/test_log_message.py` & `logkontrol-0.2.0/tests/test_log_message.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 # tests/test_log_message.py
 
 import os
 import unittest
-from unittest.mock import patch, mock_open
-from logkontrol.logkontrol import log_message, truncate_string
+from unittest.mock import patch
+from logkontrol.logkontrol import LogKonfig, log_message, truncate_string
 
 
 class TestLogMessage(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = LogKonfig()
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
         self.log_file_key = "test_log"
         self.log_file_path = "test_log.log"
         self.message = "Test log message"
         self.variables = {"var1": "value1", "var2": "value2"}
         self.log_level = "DEBUG"
 
     def tearDown(self):
         if os.path.exists(self.log_file_path):
             os.remove(self.log_file_path)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_message_to_file(self):
         log_message(self.log_file_key, self.message)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(self.message, log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_message_with_variables(self):
         log_message(self.log_file_key, variables=self.variables)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         for variable_name, variable_value in self.variables.items():
             self.assertIn(f"{variable_name}: {variable_value}", log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_message_with_truncated_level(self):
-        long_message = "This is a very long message that will be truncated."
+        long_message = "This is a very long message that will be truncated." * 100
         log_message(self.log_file_key, long_message, log_level="TRUNCATED")
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(truncate_string(long_message), log_content)
+
+    def test_log_message_without_log_file_key(self):
+        log_message(None, self.message)
+        self.assertTrue(os.path.exists(self.log_file_path))
+        with open(self.log_file_path, "r") as log_file:
+            log_content = log_file.read()
+        self.assertIn(self.message, log_content)
+
+    def test_log_message_without_logging_config(self):
+        self.log_konfig.set_logging_config(None)  # type: ignore
+        with patch("builtins.print") as mock_print:
+            log_message(self.log_file_key, self.message)
+            mock_print.assert_called_with(
+                "Logging configuration is not initialized. Please call init_logging() first."
+            )
```

### Comparing `logkontrol-0.1.2/tests/test_log_variable.py` & `logkontrol-0.2.0/tests/test_log_variable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,60 @@
 # tests/test_log_variable.py
 
 import os
 import unittest
-from unittest.mock import patch, mock_open
-from logkontrol.logkontrol import log_variable, truncate_string
+from unittest.mock import patch
+from logkontrol.logkontrol import LogKonfig, log_variable, truncate_string
 
 
 class TestLogVariable(unittest.TestCase):
     def setUp(self):
+        self.log_konfig = LogKonfig()
+        self.log_konfig.set_logging_config(
+            {"log_file_paths": {"test_log": "test_log.log"}}
+        )
         self.log_file_key = "test_log"
         self.log_file_path = "test_log.log"
         self.variable_name = "test_variable"
         self.variable_value = "test_value"
         self.log_level = "DEBUG"
 
     def tearDown(self):
         if os.path.exists(self.log_file_path):
             os.remove(self.log_file_path)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_variable(self):
         log_variable(self.log_file_key, self.variable_name, self.variable_value)
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(f"{self.variable_name}: {self.variable_value}", log_content)
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_variable_with_truncated_level(self):
         long_variable_value = (
-            "This is a very long variable value that will be truncated."
+            "This is a very long variable value that will be truncated." * 100
         )
         log_variable(
             self.log_file_key,
             self.variable_name,
             long_variable_value,
             log_level="TRUNCATED",
         )
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(
             f"{self.variable_name}: {truncate_string(long_variable_value)}", log_content
         )
 
-    @patch(
-        "logkontrol.logkontrol.logging_config",
-        {"log_file_paths": {"test_log": "test_log.log"}},
-    )
     def test_log_variable_without_log_file_key(self):
         log_variable(None, self.variable_name, self.variable_value)
         self.assertTrue(os.path.exists(self.log_file_path))
         with open(self.log_file_path, "r") as log_file:
             log_content = log_file.read()
         self.assertIn(f"{self.variable_name}: {self.variable_value}", log_content)
 
-    @patch("logkontrol.logkontrol.logging_config", None)
     def test_log_variable_without_logging_config(self):
+        self.log_konfig.set_logging_config(None)  # type: ignore
         with patch("builtins.print") as mock_print:
             log_variable(self.log_file_key, self.variable_name, self.variable_value)
             mock_print.assert_called_with(
                 "Logging configuration is not initialized. Please call init_logging() first."
             )
```

### Comparing `logkontrol-0.1.2/tests/test_truncate_string.py` & `logkontrol-0.2.0/tests/test_truncate_string.py`

 * *Files identical despite different names*

