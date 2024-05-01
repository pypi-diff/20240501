# Comparing `tmp/webdriver_cache_manager-0.0.7.tar.gz` & `tmp/webdriver_cache_manager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_cache_manager-0.0.7.tar", last modified: Mon Apr 29 16:57:13 2024, max compression
+gzip compressed data, was "webdriver_cache_manager-0.0.8.tar", last modified: Wed May  1 00:43:40 2024, max compression
```

## Comparing `webdriver_cache_manager-0.0.7.tar` & `webdriver_cache_manager-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.033099 webdriver_cache_manager-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:57:13.033099 webdriver_cache_manager-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/webdriver_cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.489214 webdriver_cache_manager-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-05-01 00:43:29.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager/webdriver_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:40.493214 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 00:43:40.000000 webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/top_level.txt
```

### Comparing `webdriver_cache_manager-0.0.7/LICENSE` & `webdriver_cache_manager-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.7/PKG-INFO` & `webdriver_cache_manager-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `webdriver_cache_manager-0.0.7/README.md` & `webdriver_cache_manager-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.7/pyproject.toml` & `webdriver_cache_manager-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webdriver_cache_manager"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Muhammad Nawaz", email="MNawaz6935@gmail.com" },
 ]
 description = "Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/PKG-INFO` & `webdriver_cache_manager-0.0.8/src/webdriver_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

