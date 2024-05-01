# Comparing `tmp/pytestomatio-2.2.2.tar.gz` & `tmp/pytestomatio-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.2.2.tar", last modified: Wed May  1 10:08:53 2024, max compression
+gzip compressed data, was "pytestomatio-2.2.3.tar", last modified: Wed May  1 11:11:52 2024, max compression
```

## Comparing `pytestomatio-2.2.2.tar` & `pytestomatio-2.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/test_root.py
```

### Comparing `pytestomatio-2.2.2/LICENSE` & `pytestomatio-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/PKG-INFO` & `pytestomatio-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.2
+Version: 2.2.3
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.29.0
-Requires-Dist: pytest<8.0.0,>=7.3.1
+Requires-Dist: pytest>8.0.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
 # testomat.io plugin for pytest
```

### Comparing `pytestomatio-2.2.2/README.md` & `pytestomatio-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pyproject.toml` & `pytestomatio-2.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.2.2"
+version = "2.2.3"
 
 dependencies = [
     "requests>=2.29.0",
-    "pytest<8.0.0,>=7.3.1",
+    "pytest>8.0.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1"]
 
 authors = [
     { name = "Oleksii Ostapov" },
     { name = "TikoQA" },
```

### Comparing `pytestomatio-2.2.2/pytestomatio/code_collector.py` & `pytestomatio-2.2.3/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/connector.py` & `pytestomatio-2.2.3/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/decorator_updater.py` & `pytestomatio-2.2.3/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/helper.py` & `pytestomatio-2.2.3/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/main.py` & `pytestomatio-2.2.3/pytestomatio/main.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/s3_connector.py` & `pytestomatio-2.2.3/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/testItem.py` & `pytestomatio-2.2.3/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/testRunConfig.py` & `pytestomatio-2.2.3/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio/testomatio.py` & `pytestomatio-2.2.3/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.2.3/pytestomatio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.2
+Version: 2.2.3
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.29.0
-Requires-Dist: pytest<8.0.0,>=7.3.1
+Requires-Dist: pytest>8.0.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
 # testomat.io plugin for pytest
```

### Comparing `pytestomatio-2.2.2/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.2.3/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.2/tests/test_root.py` & `pytestomatio-2.2.3/tests/test_root.py`

 * *Files identical despite different names*

