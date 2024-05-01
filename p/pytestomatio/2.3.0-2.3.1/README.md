# Comparing `tmp/pytestomatio-2.3.0.tar.gz` & `tmp/pytestomatio-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.3.0.tar", last modified: Wed May  1 14:22:56 2024, max compression
+gzip compressed data, was "pytestomatio-2.3.1.tar", last modified: Wed May  1 14:46:46 2024, max compression
```

## Comparing `pytestomatio-2.3.0.tar` & `pytestomatio-2.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/pytestomatio/decor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/pep8.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.473676 pytestomatio-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:46:46.473676 pytestomatio-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.469676 pytestomatio-2.3.1/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.469676 pytestomatio-2.3.1/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.473676 pytestomatio-2.3.1/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:46:46.000000 pytestomatio-2.3.1/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:46:46.473676 pytestomatio-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.469676 pytestomatio-2.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.469676 pytestomatio-2.3.1/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:46.473676 pytestomatio-2.3.1/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 14:46:41.000000 pytestomatio-2.3.1/tests/test_root.py
```

### Comparing `pytestomatio-2.3.0/LICENSE` & `pytestomatio-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/PKG-INFO` & `pytestomatio-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.3.0/README.md` & `pytestomatio-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pyproject.toml` & `pytestomatio-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.3.0"
+version = "2.3.1"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>7.2.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
```

### Comparing `pytestomatio-2.3.0/pytestomatio/code_collector.py` & `pytestomatio-2.3.1/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/connector.py` & `pytestomatio-2.3.1/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/decor/default.py` & `pytestomatio-2.3.1/pytestomatio/decor/default.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/decor/pep8.py` & `pytestomatio-2.3.1/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/decorator_updater.py` & `pytestomatio-2.3.1/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/helper.py` & `pytestomatio-2.3.1/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/main.py` & `pytestomatio-2.3.1/pytestomatio/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,16 @@
                     create=config.getoption('create'),
                     directory=config.getoption('directory')
                 )
                 testomatio_tests = pytest.testomatio.connector.get_tests(meta)
                 add_and_enrich_tests(meta, test_files, test_names, testomatio_tests, decorator_name)
                 pytest.testomatio.session = "sync"
                 print(f'Found {len(items)} test. {len(meta)} unique test functions data collected and updated.')
+                print('Test sync with testomat.io finished')
+                pytest.exit('Exit without test execution')
             case 'remove':
                 mapping = get_test_mapping(meta)
                 for test_file in test_files:
                     update_tests(test_file, mapping, test_names, decorator_name, remove=True)
                 pytest.exit(
                     f'{len(items)} found. tests ids removed. Exit without test execution')
             case 'report':
```

### Comparing `pytestomatio-2.3.0/pytestomatio/s3_connector.py` & `pytestomatio-2.3.1/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/testItem.py` & `pytestomatio-2.3.1/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/testRunConfig.py` & `pytestomatio-2.3.1/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio/testomatio.py` & `pytestomatio-2.3.1/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.3.1/pytestomatio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.3.0/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.3.1/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.0/tests/test_root.py` & `pytestomatio-2.3.1/tests/test_root.py`

 * *Files identical despite different names*

