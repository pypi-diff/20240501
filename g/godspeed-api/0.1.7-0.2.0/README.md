# Comparing `tmp/godspeed_api-0.1.7.tar.gz` & `tmp/godspeed_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godspeed_api-0.1.7.tar", last modified: Wed Apr  3 15:33:55 2024, max compression
+gzip compressed data, was "godspeed_api-0.2.0.tar", last modified: Wed May  1 16:40:30 2024, max compression
```

## Comparing `godspeed_api-0.1.7.tar` & `godspeed_api-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.931861 godspeed_api-0.1.7/godspeed_api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/godspeed_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/godspeed_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/godspeed_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 15:33:55.000000 godspeed_api-0.1.7/godspeed_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:55.935861 godspeed_api-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 15:33:51.000000 godspeed_api-0.1.7/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/godspeed_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/godspeed_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/godspeed_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/godspeed_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 16:40:30.000000 godspeed_api-0.2.0/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:40:30.814738 godspeed_api-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-01 16:40:24.000000 godspeed_api-0.2.0/tests/test_api.py
```

### Comparing `godspeed_api-0.1.7/LICENSE` & `godspeed_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.1.7/PKG-INFO` & `godspeed_api-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: godspeed_api
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Godspeed task manager API wrapper
 Author: Artem Trubacheev
 Author-email: almaz5200@gmail.com
 Keywords: python,godspeed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: dacite
 
 # Godspeed-API
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A Python API package for [Godspeed](https://godspeedapp.com/). The package implements basic authentication and task creation functionalities, this will be extended as the API is documented more.
-
+A Python API wrapper for [Godspeed](https://godspeedapp.com/). 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Godspeed-API.
 
 ```bash
 pip install godspeed-api
 ```
 
+## Features
+
+- Task creation (`create_task`)
+- Task modification (`update_task`)
+- Paginated task query (`list_tasks`)
+
 ## Usage
 ```python
 from godspeed_api import API
 
 api = API("your-username", "your-password")
 
 # to create a task
```

### Comparing `godspeed_api-0.1.7/README.md` & `godspeed_api-0.2.0/godspeed_api.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,45 @@
+Metadata-Version: 2.1
+Name: godspeed_api
+Version: 0.2.0
+Summary: A Godspeed task manager API wrapper
+Author: Artem Trubacheev
+Author-email: almaz5200@gmail.com
+Keywords: python,godspeed
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: dacite
+
 # Godspeed-API
 
 [![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/downloads/release/python-390/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-A Python API package for [Godspeed](https://godspeedapp.com/). The package implements basic authentication and task creation functionalities, this will be extended as the API is documented more.
-
+A Python API wrapper for [Godspeed](https://godspeedapp.com/). 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Godspeed-API.
 
 ```bash
 pip install godspeed-api
 ```
 
+## Features
+
+- Task creation (`create_task`)
+- Task modification (`update_task`)
+- Paginated task query (`list_tasks`)
+
 ## Usage
 ```python
 from godspeed_api import API
 
 api = API("your-username", "your-password")
 
 # to create a task
```

### Comparing `godspeed_api-0.1.7/setup.py` & `godspeed_api-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.1.7"
+VERSION = "0.2.0"
 DESCRIPTION = "A Godspeed task manager API wrapper"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="godspeed_api",
@@ -14,14 +14,15 @@
     author_email="almaz5200@gmail.com",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "requests",
+        "dacite",
     ],
     keywords=["python", "godspeed"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
```

### Comparing `godspeed_api-0.1.7/tests/test_api.py` & `godspeed_api-0.2.0/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import json
 import logging
 from os import environ
 import godspeed_api
 import unittest
 
 
 class TestAPI(unittest.TestCase):
@@ -24,7 +25,27 @@
         api.create_task(
             "Test task for testing",
             notes="This is a test task",
             due_at=due_at,
             # TODO: Uncomment after api either allows for new tags here or returns an error
             # label_names=["test"],
         )
+
+    def test_list_tasks(self):
+        api = godspeed_api.API(self.login, self.password)
+
+        result = api.list_tasks()
+
+        for task in result.tasks:
+            print(task.title)
+
+    def test_update_task(self):
+        api = godspeed_api.API(self.login, self.password)
+
+        result = api.list_tasks().tasks[0]
+
+        print(f"Updating task {result.title}")
+        api.update_task(
+            result.id,
+            title=result.title + " [Upd]",
+            due_at=datetime.datetime.now() + datetime.timedelta(days=1),
+        )
```

