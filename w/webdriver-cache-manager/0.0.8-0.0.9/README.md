# Comparing `tmp/webdriver_cache_manager-0.0.8.tar.gz` & `tmp/webdriver_cache_manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_cache_manager-0.0.8.tar", last modified: Wed May  1 00:43:40 2024, max compression
+gzip compressed data, was "webdriver_cache_manager-0.0.9.tar", last modified: Wed May  1 15:10:30 2024, max compression
```

## Comparing `webdriver_cache_manager-0.0.8.tar` & `webdriver_cache_manager-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.489214 webdriver_cache_manager-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/webdriver_cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:10:30.542810 webdriver_cache_manager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 15:10:23.000000 webdriver_cache_manager-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 15:10:30.542810 webdriver_cache_manager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 15:10:23.000000 webdriver_cache_manager-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 15:10:23.000000 webdriver_cache_manager-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:10:30.542810 webdriver_cache_manager-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:10:30.538810 webdriver_cache_manager-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:10:30.538810 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:10:23.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-01 15:10:23.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager/webdriver_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:10:30.538810 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 15:10:30.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-01 15:10:30.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:10:30.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 15:10:30.000000 webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/top_level.txt
```

### Comparing `webdriver_cache_manager-0.0.8/LICENSE` & `webdriver_cache_manager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.8/PKG-INFO` & `webdriver_cache_manager-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `webdriver_cache_manager-0.0.8/README.md` & `webdriver_cache_manager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.8/pyproject.toml` & `webdriver_cache_manager-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webdriver_cache_manager"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Muhammad Nawaz", email="MNawaz6935@gmail.com" },
 ]
 description = "Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/webdriver_cache_manager.py` & `webdriver_cache_manager-0.0.9/src/webdriver_cache_manager/webdriver_cache_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import threading
 import time
 import traceback
 import psutil
 
 CSV_FILE_PATH = os.path.join(os.path.expanduser("~"), ".wcm")
 os.makedirs(CSV_FILE_PATH, exist_ok=True)
-temp_file_path = os.path.join(CSV_FILE_PATH, "temp.csv")
-CSV_FILE_PATH = os.path.join(CSV_FILE_PATH, "pids.csv")
+temp_file_path = "temp.csv"#os.path.join(CSV_FILE_PATH, "temp.csv")
+CSV_FILE_PATH = "pids.csv"#os.path.join(CSV_FILE_PATH, "pids.csv")
 
 
 def save_pids_to_csv(file_path, chrome_driver_pid, chrome_pid):
     global CSV_FILE_PATH
     with open(CSV_FILE_PATH, 'a+', newline='') as csvfile:
         fieldnames = ['File Path', 'ChromeDriver PID', 'Chrome PID']
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
```

### Comparing `webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/PKG-INFO` & `webdriver_cache_manager-0.0.9/src/webdriver_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

