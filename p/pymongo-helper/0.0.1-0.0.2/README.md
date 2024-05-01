# Comparing `tmp/pymongo_helper-0.0.1.tar.gz` & `tmp/pymongo_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongo_helper-0.0.1.tar", last modified: Thu Apr 25 17:49:41 2024, max compression
+gzip compressed data, was "pymongo_helper-0.0.2.tar", last modified: Wed May  1 18:54:19 2024, max compression
```

## Comparing `pymongo_helper-0.0.1.tar` & `pymongo_helper-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:49:41.950230 pymongo_helper-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:49:37.000000 pymongo_helper-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 17:49:41.950230 pymongo_helper-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 17:49:37.000000 pymongo_helper-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 17:49:37.000000 pymongo_helper-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 17:49:41.950230 pymongo_helper-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:49:41.950230 pymongo_helper-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:49:41.950230 pymongo_helper-0.0.1/src/pymongo_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 17:49:41.000000 pymongo_helper-0.0.1/src/pymongo_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 17:49:41.000000 pymongo_helper-0.0.1/src/pymongo_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:49:41.000000 pymongo_helper-0.0.1/src/pymongo_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:49:41.000000 pymongo_helper-0.0.1/src/pymongo_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:54:19.453991 pymongo_helper-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 18:54:15.000000 pymongo_helper-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-01 18:54:19.453991 pymongo_helper-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 18:54:15.000000 pymongo_helper-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 18:54:15.000000 pymongo_helper-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-01 18:54:19.453991 pymongo_helper-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:54:19.449991 pymongo_helper-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:54:19.453991 pymongo_helper-0.0.2/src/pymongo_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-01 18:54:19.000000 pymongo_helper-0.0.2/src/pymongo_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 18:54:19.000000 pymongo_helper-0.0.2/src/pymongo_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:54:19.000000 pymongo_helper-0.0.2/src/pymongo_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:54:19.000000 pymongo_helper-0.0.2/src/pymongo_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:54:19.453991 pymongo_helper-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-01 18:54:15.000000 pymongo_helper-0.0.2/tests/test_mongodb_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:54:15.000000 pymongo_helper-0.0.2/tests/test_pymongo_helper.py
```

### Comparing `pymongo_helper-0.0.1/LICENSE` & `pymongo_helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongo_helper-0.0.1/PKG-INFO` & `pymongo_helper-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongo-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: The pymongo helper package is a Python library designed to simplify and streamline interactions with MongoDB databases using the PyMongo driver.
 Home-page: https://github.com/ambroisehdn/pymongo-helper
 Author: ambroisehdn
 Author-email: contact@ambroisehdn.me
 Project-URL: Bug Tracker, https://github.com/ambroisehdn/pymongo-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pymongo_helper-0.0.1/setup.cfg` & `pymongo_helper-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymongo-helper
-version = 0.0.1
+version = 0.0.2
 author = ambroisehdn
 author_email = contact@ambroisehdn.me
 description = The pymongo helper package is a Python library designed to simplify and streamline interactions with MongoDB databases using the PyMongo driver.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ambroisehdn/pymongo-helper
 project_urls = 
@@ -19,13 +19,14 @@
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 install_requires = 
-	pymongo
+	pymongo==4.7.0
+	pytest==8.2.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pymongo_helper-0.0.1/src/pymongo_helper.egg-info/PKG-INFO` & `pymongo_helper-0.0.2/src/pymongo_helper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongo-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: The pymongo helper package is a Python library designed to simplify and streamline interactions with MongoDB databases using the PyMongo driver.
 Home-page: https://github.com/ambroisehdn/pymongo-helper
 Author: ambroisehdn
 Author-email: contact@ambroisehdn.me
 Project-URL: Bug Tracker, https://github.com/ambroisehdn/pymongo-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

