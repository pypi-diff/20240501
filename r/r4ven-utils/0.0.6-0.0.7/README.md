# Comparing `tmp/r4ven_utils-0.0.6.tar.gz` & `tmp/r4ven_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r4ven_utils-0.0.6.tar", last modified: Fri Apr 26 15:06:08 2024, max compression
+gzip compressed data, was "r4ven_utils-0.0.7.tar", last modified: Tue Apr 30 22:42:49 2024, max compression
```

## Comparing `r4ven_utils-0.0.6.tar` & `r4ven_utils-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/
--rw-rw-r--   0 victor    (1000) victor    (1000)    35149 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/LICENSE
--rw-r--r--   0 victor    (1000) victor    (1000)     3411 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)     2582 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/README.md
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.917448 r4ven_utils-0.0.6/r4ven_utils/
--rw-rw-r--   0 victor    (1000) victor    (1000)        0 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/r4ven_utils/__init__.py
--rw-rw-r--   0 victor    (1000) victor    (1000)     4373 2024-04-26 14:53:09.000000 r4ven_utils-0.0.6/r4ven_utils/log4me.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 15:06:08.917448 r4ven_utils-0.0.6/r4ven_utils.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)     3411 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/PKG-INFO
--rw-rw-r--   0 victor    (1000) victor    (1000)      222 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)        1 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)       12 2024-04-26 15:06:08.000000 r4ven_utils-0.0.6/r4ven_utils.egg-info/top_level.txt
--rw-rw-r--   0 victor    (1000) victor    (1000)      350 2024-04-26 15:06:08.921448 r4ven_utils-0.0.6/setup.cfg
--rw-rw-r--   0 victor    (1000) victor    (1000)     1454 2024-04-26 14:54:38.000000 r4ven_utils-0.0.6/setup.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-30 22:42:49.744818 r4ven_utils-0.0.7/
+-rw-rw-r--   0 victor    (1000) victor    (1000)    35149 2024-04-30 22:34:18.000000 r4ven_utils-0.0.7/LICENSE
+-rw-r--r--   0 victor    (1000) victor    (1000)     3405 2024-04-30 22:42:49.744818 r4ven_utils-0.0.7/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)     2582 2024-04-30 22:34:18.000000 r4ven_utils-0.0.7/README.md
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-30 22:42:49.744818 r4ven_utils-0.0.7/r4ven_utils/
+-rw-rw-r--   0 victor    (1000) victor    (1000)        0 2024-04-30 22:34:18.000000 r4ven_utils-0.0.7/r4ven_utils/__init__.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)     4816 2024-04-30 22:39:54.000000 r4ven_utils-0.0.7/r4ven_utils/log4me.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-30 22:42:49.744818 r4ven_utils-0.0.7/r4ven_utils.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)     3405 2024-04-30 22:42:49.000000 r4ven_utils-0.0.7/r4ven_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)      222 2024-04-30 22:42:49.000000 r4ven_utils-0.0.7/r4ven_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        1 2024-04-30 22:42:49.000000 r4ven_utils-0.0.7/r4ven_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)       12 2024-04-30 22:42:49.000000 r4ven_utils-0.0.7/r4ven_utils.egg-info/top_level.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)      350 2024-04-30 22:42:49.744818 r4ven_utils-0.0.7/setup.cfg
+-rw-rw-r--   0 victor    (1000) victor    (1000)     1440 2024-04-30 22:34:52.000000 r4ven_utils-0.0.7/setup.py
```

### Comparing `r4ven_utils-0.0.6/LICENSE` & `r4ven_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.6/PKG-INFO` & `r4ven_utils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: r4ven_utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: The companion that holds your grab-bag of utility functions and objects
 Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
-Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz
 Author: Victor Vinci Fantucci
 Author-email: victor.v.fantucci@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
+Project-URL: Download, https://github.com/VictorFantucci/r4ven_utils/releases/tag/alpha
 Keywords: r4ven_utils,utils,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `r4ven_utils-0.0.6/README.md` & `r4ven_utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.6/r4ven_utils/log4me.py` & `r4ven_utils-0.0.7/r4ven_utils/log4me.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 """
 This module contains all logging related functions.
 """
 
+# Import dependencies
 import os
+import sys
 import inspect
 import logging
 import time
 import functools
 
-def function_logger(file_mode: str = "w",
+# Getting the name of the directory where the this file is present.
+current_directory = os.path.dirname(os.path.realpath(__file__))
+
+# Getting the parent directory name where the current directory is present.
+parent_directory = os.path.dirname(current_directory)
+
+# Adding the parent directory to the sys.path.
+sys.path.append(parent_directory)
+
+def function_logger(script_name: str,
+                    file_mode: str = "w",
                     file_level: int = logging.INFO,
                     console_level: int = None) -> logging.Logger:
     """
     Creates a logger object specific to the function in which it's called.
 
     Args:
+        script_name (str): Name of the script/module in which the function is called.
+
         file_mode (str): A string that define which mode you want to open the log file.
         Defaults to "w" - Write - Opens a file for writing, creates the file if it does not exist.
 
         file_level (int): Logging level that will be written in the log file.
         Defaults to logging.INFO.
 
         console_level (int, optional): Logging level that will be displayed at the console.
         Defaults to None.
 
     Returns:
         logging.Logger: Logger object of the specific function in which this
         function is called.
     """
+
     create_logs_folder()
-    script_name = os.path.basename(__file__).removesuffix(".py")
     create_script_logs_folder(script_name)
 
     caller_frame = inspect.stack()[1]
 
     if caller_frame[3] == "<module>":
         # If the caller is the main module (<module>), get the main function name
         function_name = inspect.getmodulename(caller_frame[1])
@@ -70,28 +84,30 @@
     return logger
 
 def create_logs_folder() -> None:
     """
     Check if there's a logs folder (/logs) in the current directory,
     if there isn't, create it.
     """
+
     project_directory = os.getcwd()
     logs_directory = os.path.join(project_directory, "logs")
     if not os.path.exists(logs_directory):
         os.makedirs(logs_directory)
 
 def create_script_logs_folder(script_name: str) -> None:
     """
     Check if there's a log folder for the script that is running
     in the project directory (/logs/script_name), if there isn't, create it.
 
     Args:
         script_name (str): The name of the script that's calling the function
         function_logger.
     """
+
     project_directory = os.getcwd()
     script_logs_directory = os.path.join(project_directory, "logs")
     final_directory = os.path.join(script_logs_directory, script_name)
     if not os.path.exists(final_directory):
         os.makedirs(final_directory)
 
 def calculate_execution_time(logger: logging.Logger):
@@ -100,14 +116,15 @@
 
     Args:
         logger (logging.Logger): Logger object returned by the function function_logger.
 
     Returns:
         function: Decorated function.
     """
+
     def function_decorator(function):
         @functools.wraps(function)
         def wrapper(*args, **kwargs):
             """
             Wrapper function that calculates the execution time of the decorated function and logs it.
 
             Args:
```

### Comparing `r4ven_utils-0.0.6/r4ven_utils.egg-info/PKG-INFO` & `r4ven_utils-0.0.7/r4ven_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: r4ven_utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: The companion that holds your grab-bag of utility functions and objects
 Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
-Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz
 Author: Victor Vinci Fantucci
 Author-email: victor.v.fantucci@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
+Project-URL: Download, https://github.com/VictorFantucci/r4ven_utils/releases/tag/alpha
 Keywords: r4ven_utils,utils,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `r4ven_utils-0.0.6/setup.py` & `r4ven_utils-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # Package Information:
     name='r4ven_utils',
     packages=['r4ven_utils'], # Should match the package folder.
-    version='0.0.6',
+    version='0.0.7',
     license='GPLv3',
 
     # Description Information:
     description='The companion that holds your grab-bag of utility functions and objects',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
@@ -20,15 +20,16 @@
     author='Victor Vinci Fantucci',
     author_email='victor.v.fantucci@gmail.com',
     url='https://github.com/VictorFantucci/r4ven_utils_dev',
 
     # Project URLs:
     project_urls =
     {
-        "Bug Tracker": "https://github.com/VictorFantucci/r4ven_utils_dev/issues"
+        "Bug Tracker": "https://github.com/VictorFantucci/r4ven_utils_dev/issues",
+        "Download": "https://github.com/VictorFantucci/r4ven_utils/releases/tag/alpha"
     },
 
     # Project Requirements:
     install_requires=[],
 
     # Project Descriptive meta-data:
     keywords=['r4ven_utils', 'utils', 'logs'],
@@ -37,11 +38,9 @@
     classifiers=
     [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
-    ],
-
-    download_url="https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.6.tar.gz",
+    ]
 )
```

