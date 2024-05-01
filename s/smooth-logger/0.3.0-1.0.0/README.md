# Comparing `tmp/smooth_logger-0.3.0.tar.gz` & `tmp/smooth_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smooth_logger-0.3.0.tar", last modified: Tue Apr 23 19:46:08 2024, max compression
+gzip compressed data, was "smooth_logger-1.0.0.tar", last modified: Wed May  1 11:42:06 2024, max compression
```

## Comparing `smooth_logger-0.3.0.tar` & `smooth_logger-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/
--rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-0.3.0/LICENSE
--rw-r--r--   0 murdo      (502) murdo      (502)     6638 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)     5671 2024-04-23 19:45:55.000000 smooth_logger-0.3.0/README.md
--rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/setup.cfg
--rw-r--r--   0 murdo      (502) murdo      (502)     1210 2024-04-23 19:36:03.000000 smooth_logger-0.3.0/setup.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.610517 smooth_logger-0.3.0/smooth_logger/
--rw-r--r--   0 murdo      (502) murdo      (502)      474 2024-02-27 11:04:48.000000 smooth_logger-0.3.0/smooth_logger/LogEntry.py
--rw-r--r--   0 murdo      (502) murdo      (502)    13305 2024-04-23 19:35:11.000000 smooth_logger-0.3.0/smooth_logger/Logger.py
--rw-r--r--   0 murdo      (502) murdo      (502)       88 2024-04-23 18:45:53.000000 smooth_logger-0.3.0/smooth_logger/__init__.py
--rw-r--r--   0 murdo      (502) murdo      (502)      233 2024-04-23 18:46:37.000000 smooth_logger-0.3.0/smooth_logger/enums.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/smooth_logger.egg-info/
--rw-r--r--   0 murdo      (502) murdo      (502)     6638 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)      309 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/SOURCES.txt
--rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/dependency_links.txt
--rw-r--r--   0 murdo      (502) murdo      (502)       22 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/requires.txt
--rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/top_level.txt
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/
+-rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-1.0.0/LICENSE
+-rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)     5878 2024-05-01 11:28:58.000000 smooth_logger-1.0.0/README.md
+-rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/setup.cfg
+-rw-r--r--   0 murdo      (502) murdo      (502)     1183 2024-05-01 11:29:32.000000 smooth_logger-1.0.0/setup.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.699392 smooth_logger-1.0.0/smooth_logger/
+-rw-r--r--   0 murdo      (502) murdo      (502)      470 2024-05-01 10:21:37.000000 smooth_logger-1.0.0/smooth_logger/LogEntry.py
+-rw-r--r--   0 murdo      (502) murdo      (502)    13010 2024-05-01 11:18:19.000000 smooth_logger-1.0.0/smooth_logger/Logger.py
+-rw-r--r--   0 murdo      (502) murdo      (502)       89 2024-05-01 10:24:22.000000 smooth_logger-1.0.0/smooth_logger/__init__.py
+-rw-r--r--   0 murdo      (502) murdo      (502)      376 2024-05-01 11:03:37.000000 smooth_logger-1.0.0/smooth_logger/enums.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-05-01 11:42:06.700392 smooth_logger-1.0.0/smooth_logger.egg-info/
+-rw-r--r--   0 murdo      (502) murdo      (502)     6813 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)      309 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)        6 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/requires.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-05-01 11:42:06.000000 smooth_logger-1.0.0/smooth_logger.egg-info/top_level.txt
```

### Comparing `smooth_logger-0.3.0/LICENSE` & `smooth_logger-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smooth_logger-0.3.0/PKG-INFO` & `smooth_logger-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 0.3.0
+Version: 1.0.0
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
@@ -14,40 +14,42 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plyer
-Requires-Dist: smooth_progress
 
 # smooth_logger
 
 A simple logger made primarily for my own personal use. Was made out of a combination of necessity and being so lazy that I overflowed into being productive and instead of searching for a library that suited my needs, I wrote my own.
 
 ## Installation
 
-smooth_logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
+smooth_logger can be installed through pip. Either download the latest release from GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branch on the repository.
 
 smooth_logger is currently devloped using Python 3.11, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
 
-smooth_logger supports Linux, macOS and Windows.
+smooth_logger supports Linux, macOS and Windows and will be able to automatically create a folder for storing log files on these operating systems. Other operating systems are not officially supported, but you may still be able to use them by providing a custom config path. See the Initialisation section, below, for more.
+
+### Requirements
+
+- smooth_logger uses the `plyer` library to send desktop notifications.
 
 ## Usage
 
 Usage of smooth-logger is, as it should be, quite simple.
 
 The `Logger` model provides a number of methods for your use:
 
 - `Logger.add_scope()` adds a new scope.
 - `Logger.clean()` erases all log entries currently in memory.
 - `Logger.edit_scope()` modifies the category of an existing scope.
 - `Logger.get()` allows you to retrieve either the most recent log entry or all log entries, optionally filtered by scope.
-- `Logger.get_time()` returns the full date & time, or optionally just the date, in ISO-8601 formatting.
-- `Logger.init_bar()` initialises the `ProgressBar` model imported from the `smooth_progress` dependency.
+- `Logger.is_scope()` can be queried with a scope name to check if the scope exists, and optionally with a category to check if the scope is set to it.
 - `Logger.notify()` sends a desktop notification using the `plyer` dependency.
 - `Logger.new()` creates and, depending on scope, prints a new log entry.
 - `Logger.output()` saves all log entries of appropriate scope to the log file and cleans the log array for the next group of log entries. A new log file is created for each new day. This method only attempts to create or update the log file if there are entries of an appropriate scope to be written to it; if there are none, it just executes `Logger.clean()`.
 - `Logger.remove_scope()` removes an existing scope.
 
 ### Initialisation
 
@@ -76,25 +78,26 @@
 
 - DEBUG: Information for debugging the program.
 - ERROR: Errors that the program can recover from but impact functionality or performance.
 - FATAL: Errors that mean the program must continue; handled crashes.
 - INFO: General information for the user.
 - WARNING: Things that have no immediate impact to functionality but could cause errors later on.
 
-You can also use the value "NOSCOPE" to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
+You can also forgo passing a scope or pass a None value to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
 
 ### Categories
 
 When initialising the Logger, you can optionally provide categories to associate with each scope:
 
 - DISABLED (will not print to console or save to log file)
-- ENABLED (will print to console but not save to log file)
-- MAXIMUM (will print to console and save to log file)
+- PRINT    (will print to console but not save to log file)
+- SAVE     (will to log file but not save print to console)
+- MAXIMUM  (will print to console and save to log file)
 
-By default, the DEBUG scope is disabled, the INFO scope is enabled, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
+By default, the DEBUG scope is disabled, the INFO scope is set to print, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to save or maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
 
 Categories are accessed like so:
 
 ```py
 from smooth_logger.enums import Categories
 
 Categories.ENABLED
@@ -122,14 +125,10 @@
 
 ```py
 Log.remove_scope("DEBUG")
 ```
 
 It is recommended to be careful with this method. Removing scopes, like adding or editing them, is ephemeral and won't be hard-saved anywhere, but removing a scope during run-time will produce warnings if you attempt to use that scope anywhere in your program.
 
-## Roadmap
-
-- Rework `Logger.get()` to allow passing of a specific number of log values to be fetched. If these values exceed the number in the log, all matching log values should be returned, and a warning should be issued (but not returned).
-
-- Possibly replace some internal warnings with Exceptions so they can be more easily-handled by end-user programs.
+## Contributing
 
-- Add a category that saves to the log file but doesn't print to the console.
+I'm always happy to accept feature requests, bug reports, and any pull requests to improve the project. If you want to contribute, please explain clearly what your request or issue is so that I can provide solutions as swiftly as possible.
```

### Comparing `smooth_logger-0.3.0/README.md` & `smooth_logger-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # smooth_logger
 
 A simple logger made primarily for my own personal use. Was made out of a combination of necessity and being so lazy that I overflowed into being productive and instead of searching for a library that suited my needs, I wrote my own.
 
 ## Installation
 
-smooth_logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
+smooth_logger can be installed through pip. Either download the latest release from GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branch on the repository.
 
 smooth_logger is currently devloped using Python 3.11, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
 
-smooth_logger supports Linux, macOS and Windows.
+smooth_logger supports Linux, macOS and Windows and will be able to automatically create a folder for storing log files on these operating systems. Other operating systems are not officially supported, but you may still be able to use them by providing a custom config path. See the Initialisation section, below, for more.
+
+### Requirements
+
+- smooth_logger uses the `plyer` library to send desktop notifications.
 
 ## Usage
 
 Usage of smooth-logger is, as it should be, quite simple.
 
 The `Logger` model provides a number of methods for your use:
 
 - `Logger.add_scope()` adds a new scope.
 - `Logger.clean()` erases all log entries currently in memory.
 - `Logger.edit_scope()` modifies the category of an existing scope.
 - `Logger.get()` allows you to retrieve either the most recent log entry or all log entries, optionally filtered by scope.
-- `Logger.get_time()` returns the full date & time, or optionally just the date, in ISO-8601 formatting.
-- `Logger.init_bar()` initialises the `ProgressBar` model imported from the `smooth_progress` dependency.
+- `Logger.is_scope()` can be queried with a scope name to check if the scope exists, and optionally with a category to check if the scope is set to it.
 - `Logger.notify()` sends a desktop notification using the `plyer` dependency.
 - `Logger.new()` creates and, depending on scope, prints a new log entry.
 - `Logger.output()` saves all log entries of appropriate scope to the log file and cleans the log array for the next group of log entries. A new log file is created for each new day. This method only attempts to create or update the log file if there are entries of an appropriate scope to be written to it; if there are none, it just executes `Logger.clean()`.
 - `Logger.remove_scope()` removes an existing scope.
 
 ### Initialisation
 
@@ -54,25 +57,26 @@
 
 - DEBUG: Information for debugging the program.
 - ERROR: Errors that the program can recover from but impact functionality or performance.
 - FATAL: Errors that mean the program must continue; handled crashes.
 - INFO: General information for the user.
 - WARNING: Things that have no immediate impact to functionality but could cause errors later on.
 
-You can also use the value "NOSCOPE" to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
+You can also forgo passing a scope or pass a None value to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
 
 ### Categories
 
 When initialising the Logger, you can optionally provide categories to associate with each scope:
 
 - DISABLED (will not print to console or save to log file)
-- ENABLED (will print to console but not save to log file)
-- MAXIMUM (will print to console and save to log file)
+- PRINT    (will print to console but not save to log file)
+- SAVE     (will to log file but not save print to console)
+- MAXIMUM  (will print to console and save to log file)
 
-By default, the DEBUG scope is disabled, the INFO scope is enabled, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
+By default, the DEBUG scope is disabled, the INFO scope is set to print, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to save or maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
 
 Categories are accessed like so:
 
 ```py
 from smooth_logger.enums import Categories
 
 Categories.ENABLED
@@ -100,14 +104,10 @@
 
 ```py
 Log.remove_scope("DEBUG")
 ```
 
 It is recommended to be careful with this method. Removing scopes, like adding or editing them, is ephemeral and won't be hard-saved anywhere, but removing a scope during run-time will produce warnings if you attempt to use that scope anywhere in your program.
 
-## Roadmap
-
-- Rework `Logger.get()` to allow passing of a specific number of log values to be fetched. If these values exceed the number in the log, all matching log values should be returned, and a warning should be issued (but not returned).
-
-- Possibly replace some internal warnings with Exceptions so they can be more easily-handled by end-user programs.
+## Contributing
 
-- Add a category that saves to the log file but doesn't print to the console.
+I'm always happy to accept feature requests, bug reports, and any pull requests to improve the project. If you want to contribute, please explain clearly what your request or issue is so that I can provide solutions as swiftly as possible.
```

### Comparing `smooth_logger-0.3.0/setup.py` & `smooth_logger-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 
 def readme():
     return open('README.md', 'r').read()
 
 
 setup(
     name="smooth_logger",
-    version="0.3.0",
+    version="1.0.0",
     author="Murdo Maclachlan",
     author_email="murdomaclachlan@duck.com",
     description=(
         "A simple logger made primarily for my own personal use. Made from a combination of"
         + " necessity and so much sloth that it overflowed into productivity."
     ),
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/MurdoMaclachlan/smooth_logger",
     packages=find_packages(),
     install_requires=[
-        "plyer",
-        "smooth_progress"
+        "plyer"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `smooth_logger-0.3.0/smooth_logger/Logger.py` & `smooth_logger-1.0.0/smooth_logger/Logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 from datetime import datetime
 from os import environ, makedirs
 from os.path import expanduser, isdir
 from plyer import notification
 from plyer.facades import Notification
-from smooth_progress import ProgressBar
 from time import time
 from typing_extensions import Union
 
 from .enums import Categories
 from .LogEntry import LogEntry
 
 
 class Logger:
     """
     Class for controlling the entirety of logging. The logging works on a scope-based system where
     (almost) every message has a defined scope, and the scopes are each associated with a specific
-    category between 0 and 2 inclusive. The meanings of the categories are as follows:
+    category defined by the smooth_logger.enums.Categories class. The categories' meanings are as
+    follows:
 
-    0: disabled, do not print to console or save to log file
-    1: enabled, print to console but do not save to log file
-    2: maximum, print to console and save to log file
+    Categories.DISABLED: do not print to console or save to log file
+    Categories.PRINT: print to console but do not save to log file
+    Categories.SAVE:  save to log file but do not print to console
+    Categories.MAXIMUM: print to console and save to log file
+
+    Note that the old Categories.ENABLED category is deprecated and its functionality has been
+    replaced with Categories.PRINT. It will be removed in a later version.
     """
     def __init__(self,
                  program_name: str,
                  config_path: str = None,
                  debug: int = Categories.DISABLED,
                  error: int = Categories.MAXIMUM,
                  fatal: int = Categories.MAXIMUM,
-                 info: int = Categories.ENABLED,
+                 info: int = Categories.PRINT,
                  warning: int = Categories.MAXIMUM) -> None:
-        self.bar: ProgressBar = ProgressBar()
-        self.__is_empty: bool = True
-        self.__log: list[LogEntry] = []
-        self.__notifier: Notification = notification
-        self.__program_name: str = program_name
-        self.__scopes: dict[str, int] = {
+        self.is_empty: bool = True
+        self.program_name: str = program_name
+        self._log: list[LogEntry] = []
+        self._scopes: dict[str, int] = {
             "DEBUG":   debug,   # information for debugging the program
             "ERROR":   error,   # errors the program can recover from
             "FATAL":   fatal,   # errors that mean the program cannot continue
             "INFO":    info,    # general information for the user
             "WARNING": warning  # things that could cause errors later on
         }
+        self.__notifier: Notification = notification
         self.__write_logs = False
-        self.__output_path: str = (
+
+        self._output_path: str = (
             self.__define_output_path()
             if config_path is None else 
             f"{config_path}/logs"
         )
-        self.__create_log_folder()
+        self._create_folder(self._output_path)
 
     def __create_log_entry(self, message: str, output: bool, scope: str) -> LogEntry:
         """
         Creates a new log entry from given settings and appends it to the log.
 
         :param message: the log message
         :param output: whether the message should be output to the log file
         :param scope: the scope of the message
 
         :returns: the created log entry
         """
-        entry: LogEntry = LogEntry(message, output, scope, self.__get_time())
-        self.__log.append(entry)
+        entry: LogEntry = LogEntry(message, output, scope, self._get_time())
+        self._log.append(entry)
         return entry
 
-    def __create_log_folder(self) -> None:
-        """
-        Creates the folder that will contain the log files.
-        """
-        if not isdir(self.__output_path):
-            print(f"Making path: {self.__output_path}")
-            makedirs(self.__output_path, exist_ok=True)
-
     def __define_output_path(self) -> str:
         """
         Defines the appropriate output path for the log file, automatically detecting the user's
         config folder and using the given program name. If the detected operating system is not
         supported, exits.
 
         Supported operating systems are: Linux, MacOS, Windows. Users of an unsupported operating
@@ -87,67 +83,67 @@
         /home/{user}/.config/test
         """
         from sys import platform
 
         os: str = "".join(list(platform)[:3])
         if os in ["dar", "lin", "win"]:
             path: str = (
-                environ["APPDATA"] + f"\\{self.__program_name}\logs"
+                environ["APPDATA"] + f"\\{self.program_name}\logs"
                 if os == "win" else
-                f"{expanduser('~')}/.config/{self.__program_name}/logs"
+                f"{expanduser('~')}/.config/{self.program_name}/logs"
             )
-            if not isdir(path):
-                print(f"INFO: Making path: {path}")
-                makedirs(path, exist_ok=True)
             return path
         else:
-            print(
-                f"FATAL: Could not automatically create output folder for operating system: {os}."
-                + "You will need to manually pass a pre-defined config_path."
+            raise OSError(
+                f"Could not automatically create output folder for operating system: {os}. You"
+                + " will need to pass a manually-defined config_path."
             )
-            exit()
     
     def __display_log_entry(self,
                             entry: LogEntry,
                             scope: str,
                             notify: bool,
-                            is_bar: bool,
                             print_to_console: bool = True) -> None:
         """
         Displays a given log entry as appropriate using further given settings.
 
         :param entry: the entry to display
         :param scope: the scope of the entry
         :param notify: whether to show a desktop notification for the entry
-        :param is_bar: whether the progress bar is active
-        :param console: whether the message should be printed to the console
+        :param print_to_console: whether the message should be printed to the console
         """
-        if scope == "NOSCOPE" or (self.__scopes[scope] != Categories.DISABLED and print_to_console):
+        if scope is None or (
+                self._scopes[scope] in [Categories.MAXIMUM, Categories.PRINT, Categories.ENABLED]
+                and print_to_console
+        ):
             print(entry.rendered)
-        if is_bar:
-            print(self.bar.state, end="\r", flush=True)
         if notify:
             self.notify(entry.message)
 
-    def __get_time(self, method: str = "time") -> str:
+    def _create_folder(self, path: str) -> None:
+        """
+        Creates a folder at a given path. Intended for the creation of configuration and and log
+        folders.
+        """
+        if not isdir(path):
+            print(f"Making path: {path}")
+            makedirs(path, exist_ok=True)
+
+    def _get_time(self, date_only: bool = False) -> str:
         """
         Gets the current time and parses it to a human-readable format; either
         'YYYY-MM-DD HH:MM:SS' or 'YYYY-MM-DD'.
 
-        :param method: the format of the timestamp; either 'time' or 'date'.
-
-        :returns: a single date string
+        :param date_only: optional; whether the timestamp should include only the date or the time
+                          as well; defaults to False
+        :returns: a single datetime string
         """
-        if method in ["time", "date"]:
-            return datetime.fromtimestamp(time()).strftime(
-                ("%Y-%m-%d", "%Y-%m-%d %H:%M:%S")[method == "time"]
-            )
-        else:
-            self.new("Bad method passed to Logger.get_time().", "ERROR")
-            return ""
+        return datetime.fromtimestamp(time()).strftime(
+            ("%Y-%m-%d %H:%M:%S", "%Y-%m-%d")[date_only]
+        )
 
     def add_scope(self, name: str, category: int) -> bool:
         """
         Adds a new logging scope for use with log entries. Users should be careful when doing this;
         custom scopes would be best added immediately following initialisation. If a 'Logger.new()'
         call is made before the scope it uses is added, it will generate a warning.
 
@@ -155,53 +151,53 @@
         Custom scopes are instance specific and not hard saved.
 
         :param name: the name of the new scope
         :param category: the default category of the new scope (0-2)
 
         :return: a boolean sucess status
         """
-        if name in self.__scopes.keys():
+        if name in self._scopes.keys():
             self.new(
                 f"Attempt was made to add new scope with name {name}, but scope with this name "
                 + "already exists.",
                 "WARNING"
             )
         else:
             if category in set(item for item in Categories):
-                self.__scopes[name] = category
+                self._scopes[name] = category
                 return True
             else:
                 self.new(
                     f"Attempt was made to add new scope with category {category}, but this is not "
                     + "a valid category.",
                     "WARNING"
                 )
         return False
 
     def clean(self) -> None:
         """
         Empties log array. Any log entries not saved to the output file will be lost.
         """
-        del self.__log[:]
-        self.__is_empty = True
+        del self._log[:]
+        self.is_empty = True
         self.__write_logs = False
 
     def edit_scope(self, name: str, category: int) -> bool:
         """
         Edits an existing scope's category, if the scope exists. Edited categories are instance
         specific and not hard saved.
 
         :param name: the name of the scope to edit
         :param category: the new category of the scope (0-2)
 
         :returns: a boolean success status
         """
-        if name in self.__scopes.keys():
+        if name in self._scopes.keys():
             if category in set(item for item in Categories):
-                self.__scopes[name] = category
+                self._scopes[name] = category
                 return True
             else:
                 self.new(
                     f"Attempt was made to change category of scope {name} to {category}, but this "
                     + "is not a valid category.",
                     "WARNING"
                 )
@@ -209,132 +205,128 @@
             self.new(
                 f"Attempt was made to edit a scope with name {name}, but no scope with this name "
                 + "exists.",
                 "WARNING"
             )
         return False
 
-    def get(self, mode: str = "all", scope: str = None) -> Union[list[LogEntry], LogEntry, None]:
+    def get(self,
+            number: int = 1,
+            recent: bool = True,
+            scope: str = None) -> Union[list[LogEntry], LogEntry, None]:
         """
         Returns item(s) in the log. The entries returned can be controlled by passing optional
         arguments.
 
         If no entries match the query, nothing will be returned.
 
-        :param mode: optional; 'all' for all log entries or 'recent' for only the most recent one
-        :param scope: optional; if passed, only entries matching its category will be returned
-
+        :param number: the number of entries to be returned; defaults to 1
+        :param recent: whether to return starting at the most recent entry (True) or the earliest
+                       (False); defaults to True
+        :param scope: if passed, only entries matching its category will be returned
         :returns: a single log entry or list of log entries, or nothing
         """
-        if self.__is_empty:
-            pass
-        elif scope is None:
-            return (self.__log, self.__log[-1])[mode == "recent"]
+        if self.is_empty:
+            return None
         else:
-            # return all log entries matching the query
-            if mode == "all":
-                data: list[LogEntry] = []
-                for entry in self.__log:
-                    if scope is None or entry.scope == scope:
-                        data.append(entry)
-                if data:
-                    return data
-            # iterate through the log in reverse to find the most recent entry matching the query
-            elif mode == "recent":
-                for entry in reversed(self.__log):
-                    if scope is None or entry.scope == scope:
-                        return entry
-            else:
-                self.new("Unknown mode passed to Logger.get().", "WARNING")
-
-    def init_bar(self, limit: int) -> None:
-        """
-        Initiate and open the progress bar.
-
-        :param limit: the number of increments it should take to fill the bar
-        """
-        self.bar = ProgressBar(limit=limit)
-        self.bar.open()
+            data: list[LogEntry] = []
+            entries: list[LogEntry] = (self._log, reversed(self._log))[recent]
+            for entry in entries:
+                if len(data) < number and (scope is None or entry.scope == scope):
+                    data.append(entry)
+            if data:
+                return data
+
+    def is_scope(self, scope: str, category: Categories = None) -> bool:
+        """
+        Queries a given scope to check if it exists, and optionally if it matches a given category.
+
+        If no category is given, will return true if the scope exists. If a category is given, will
+        return true if and only if the scope exists and matches the given category.
+
+        :param scope: the scope to check
+        :param category: optional; the category to check for
+        :return: whether the scope exists and optionally matches the category
+        """
+        scope_exists: bool = scope in self._scopes
+        if category is None:
+            return scope_exists
+        else:
+            return scope_exists and self._scopes[scope] == category
 
     def new(self,
             message: str,
             scope: str,
             print_to_console: bool = True,
             notify: bool = False) -> bool:
         """
         Initiates a new log entry and prints it to the console. Optionally, if do_not_print is
         passed as True, it will only save the log and will not print anything (unless the scope is
-        'NOSCOPE'; these messages are always printed).
+        None; these messages are always printed).
 
         :param message: the log message
         :param scope: the scope of the message
         :param print_to_console: optional, default True; whether the message should be printed to
                                  the console
         :param notify: optional, default False; whether the message should be displayed as a
                        desktop notification
 
         :returns: a boolean success status
         """
-        if scope in self.__scopes or scope == "NOSCOPE":
+        if scope in self._scopes or scope is None:
             output: bool = (
-                (self.__scopes[scope] == Categories.MAXIMUM)
-                if scope != "NOSCOPE" else
                 False
+                if scope is None else
+                self._scopes[scope] in [Categories.MAXIMUM, Categories.SAVE]
             )
-            is_bar: bool = (self.bar is not None) and self.bar.opened
-
-            # if the progress bar is enabled, append any necessary empty characters to the message
-            # to completely overwrite it upon output
-            if is_bar and len(message) < len(self.bar.state):
-                message += " " * (len(self.bar.state) - len(message))
             
             entry: LogEntry = self.__create_log_entry(message, output, scope)
             self.__display_log_entry(entry, scope, notify, is_bar, print_to_console)
 
             self.__write_logs = self.__write_logs or output
-            self.__is_empty = False
+            self.is_empty = False
 
             return True
         else:
             self.new("Unknown scope passed to Logger.new()", "WARNING")
         return False
 
     def notify(self, message: str) -> None:
         """
         Displays a desktop notification with a given message.
 
         :param message: the message to display
         """
-        self.__notifier.notify(title=self.__program_name, message=message)
+        self._notifier.notify(title=self.program_name, message=message)
 
     def output(self) -> None:
         """
         Writes all log entries with appropriate scopes to the log file. If the output path for the
         log file does not exist, it is created.
 
         Log files are marked with the date, so each new day, a new file will be created.
         """
         if self.__write_logs:
-            with open(f"{self.__output_path}/log-{self.__get_time(method='date')}.txt",
+            with open(f"{self._output_path}/log-{self._get_time(date_only=True)}.txt",
                       "at+") as log_file:
-                for line in self.__log:
+                for line in self._log:
                     if line.output:
                         log_file.write(line.rendered + "\n")
         self.clean()
 
     def remove_scope(self, name: str) -> bool:
         """
         Removes an existing scope if it exists.
 
         :param name: the name of the scope to remove
 
         :returns: a boolean success status
         """
-        if name in self.__scopes.keys():
-            del self.__scopes[name]
+        if name in self._scopes.keys():
+            del self._scopes[name]
             return True
         else:
             self.new(
                 f"Attempt was made to remove a scope with name {name}, but no scope with this "
                 + "name exists.",
                 "WARNING"
             )
```

### Comparing `smooth_logger-0.3.0/smooth_logger.egg-info/PKG-INFO` & `smooth_logger-1.0.0/smooth_logger.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 0.3.0
+Version: 1.0.0
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
@@ -14,40 +14,42 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plyer
-Requires-Dist: smooth_progress
 
 # smooth_logger
 
 A simple logger made primarily for my own personal use. Was made out of a combination of necessity and being so lazy that I overflowed into being productive and instead of searching for a library that suited my needs, I wrote my own.
 
 ## Installation
 
-smooth_logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
+smooth_logger can be installed through pip. Either download the latest release from GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branch on the repository.
 
 smooth_logger is currently devloped using Python 3.11, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
 
-smooth_logger supports Linux, macOS and Windows.
+smooth_logger supports Linux, macOS and Windows and will be able to automatically create a folder for storing log files on these operating systems. Other operating systems are not officially supported, but you may still be able to use them by providing a custom config path. See the Initialisation section, below, for more.
+
+### Requirements
+
+- smooth_logger uses the `plyer` library to send desktop notifications.
 
 ## Usage
 
 Usage of smooth-logger is, as it should be, quite simple.
 
 The `Logger` model provides a number of methods for your use:
 
 - `Logger.add_scope()` adds a new scope.
 - `Logger.clean()` erases all log entries currently in memory.
 - `Logger.edit_scope()` modifies the category of an existing scope.
 - `Logger.get()` allows you to retrieve either the most recent log entry or all log entries, optionally filtered by scope.
-- `Logger.get_time()` returns the full date & time, or optionally just the date, in ISO-8601 formatting.
-- `Logger.init_bar()` initialises the `ProgressBar` model imported from the `smooth_progress` dependency.
+- `Logger.is_scope()` can be queried with a scope name to check if the scope exists, and optionally with a category to check if the scope is set to it.
 - `Logger.notify()` sends a desktop notification using the `plyer` dependency.
 - `Logger.new()` creates and, depending on scope, prints a new log entry.
 - `Logger.output()` saves all log entries of appropriate scope to the log file and cleans the log array for the next group of log entries. A new log file is created for each new day. This method only attempts to create or update the log file if there are entries of an appropriate scope to be written to it; if there are none, it just executes `Logger.clean()`.
 - `Logger.remove_scope()` removes an existing scope.
 
 ### Initialisation
 
@@ -76,25 +78,26 @@
 
 - DEBUG: Information for debugging the program.
 - ERROR: Errors that the program can recover from but impact functionality or performance.
 - FATAL: Errors that mean the program must continue; handled crashes.
 - INFO: General information for the user.
 - WARNING: Things that have no immediate impact to functionality but could cause errors later on.
 
-You can also use the value "NOSCOPE" to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
+You can also forgo passing a scope or pass a None value to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
 
 ### Categories
 
 When initialising the Logger, you can optionally provide categories to associate with each scope:
 
 - DISABLED (will not print to console or save to log file)
-- ENABLED (will print to console but not save to log file)
-- MAXIMUM (will print to console and save to log file)
+- PRINT    (will print to console but not save to log file)
+- SAVE     (will to log file but not save print to console)
+- MAXIMUM  (will print to console and save to log file)
 
-By default, the DEBUG scope is disabled, the INFO scope is enabled, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
+By default, the DEBUG scope is disabled, the INFO scope is set to print, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to save or maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
 
 Categories are accessed like so:
 
 ```py
 from smooth_logger.enums import Categories
 
 Categories.ENABLED
@@ -122,14 +125,10 @@
 
 ```py
 Log.remove_scope("DEBUG")
 ```
 
 It is recommended to be careful with this method. Removing scopes, like adding or editing them, is ephemeral and won't be hard-saved anywhere, but removing a scope during run-time will produce warnings if you attempt to use that scope anywhere in your program.
 
-## Roadmap
-
-- Rework `Logger.get()` to allow passing of a specific number of log values to be fetched. If these values exceed the number in the log, all matching log values should be returned, and a warning should be issued (but not returned).
-
-- Possibly replace some internal warnings with Exceptions so they can be more easily-handled by end-user programs.
+## Contributing
 
-- Add a category that saves to the log file but doesn't print to the console.
+I'm always happy to accept feature requests, bug reports, and any pull requests to improve the project. If you want to contribute, please explain clearly what your request or issue is so that I can provide solutions as swiftly as possible.
```

