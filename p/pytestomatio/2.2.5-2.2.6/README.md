# Comparing `tmp/pytestomatio-2.2.5.tar.gz` & `tmp/pytestomatio-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.2.5.tar", last modified: Wed May  1 12:35:32 2024, max compression
+gzip compressed data, was "pytestomatio-2.2.6.tar", last modified: Wed May  1 12:50:12 2024, max compression
```

## Comparing `pytestomatio-2.2.5.tar` & `pytestomatio-2.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.454958 pytestomatio-2.2.5/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 12:35:32.000000 pytestomatio-2.2.5/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:32.458958 pytestomatio-2.2.5/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 12:35:20.000000 pytestomatio-2.2.5/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_root.py
```

### Comparing `pytestomatio-2.2.5/LICENSE` & `pytestomatio-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/PKG-INFO` & `pytestomatio-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.5
+Version: 2.2.6
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.2.5/README.md` & `pytestomatio-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pyproject.toml` & `pytestomatio-2.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.2.5"
+version = "2.2.6"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>8.0.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
```

### Comparing `pytestomatio-2.2.5/pytestomatio/code_collector.py` & `pytestomatio-2.2.6/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/connector.py` & `pytestomatio-2.2.6/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/decorator_updater.py` & `pytestomatio-2.2.6/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/helper.py` & `pytestomatio-2.2.6/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/main.py` & `pytestomatio-2.2.6/pytestomatio/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,16 @@
             if key == 'title' and call.when == 'teardown':
                 continue
             if value is not None:
                 pytest.testomatio.test_run.status_request[item.nodeid][key] = value
 
 
 def pytest_runtest_logfinish(nodeid, location):
+    if not hasattr(pytest, 'testomatio_config_option'):
+        return
     if pytest.testomatio_config_option is None or pytest.testomatio_config_option != 'report':
         return
     elif not pytest.testomatio.test_run.test_run_id:
         return
 
     for nodeid, request in pytest.testomatio.test_run.status_request.items():
         if request['status']:
```

### Comparing `pytestomatio-2.2.5/pytestomatio/s3_connector.py` & `pytestomatio-2.2.6/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/testItem.py` & `pytestomatio-2.2.6/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/testRunConfig.py` & `pytestomatio-2.2.6/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio/testomatio.py` & `pytestomatio-2.2.6/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.2.6/pytestomatio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.5
+Version: 2.2.6
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.2.5/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.2.6/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.5/tests/test_root.py` & `pytestomatio-2.2.6/tests/test_root.py`

 * *Files identical despite different names*

