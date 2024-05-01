# Comparing `tmp/pytestomatio-2.2.6.tar.gz` & `tmp/pytestomatio-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.2.6.tar", last modified: Wed May  1 12:50:12 2024, max compression
+gzip compressed data, was "pytestomatio-2.3.0.tar", last modified: Wed May  1 14:22:56 2024, max compression
```

## Comparing `pytestomatio-2.2.6.tar` & `pytestomatio-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 12:50:12.000000 pytestomatio-2.2.6/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:12.076480 pytestomatio-2.2.6/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 12:50:07.000000 pytestomatio-2.2.6/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:22:56.000000 pytestomatio-2.3.0/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.565033 pytestomatio-2.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:56.569033 pytestomatio-2.3.0/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 14:22:52.000000 pytestomatio-2.3.0/tests/test_root.py
```

### Comparing `pytestomatio-2.2.6/LICENSE` & `pytestomatio-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/PKG-INFO` & `pytestomatio-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.6
+Version: 2.3.0
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
-Requires-Dist: pytest>8.0.0
+Requires-Dist: pytest>7.2.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 Requires-Dist: autopep8>=2.1.0
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
@@ -61,28 +61,27 @@
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
 ## configuration
-
 Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
 ```bash
-export TESTOMATIO=<key>
+TESTOMATIO=<key>
 ```
-
-Windows (cmd):
-
+Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
+If you are not sure, don't set this variable. Default value is 'default'
 ```bash
-set TESTOMATIO=<key>
+TESTOMATIO_CODE_STYLE=pep8
 ```
 
+```bash
+
+
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
 
 ### pytest.ini
 In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
 testomat.io url in it
```

### Comparing `pytestomatio-2.2.6/README.md` & `pytestomatio-2.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,28 +39,27 @@
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
 ## configuration
-
 Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
 ```bash
-export TESTOMATIO=<key>
+TESTOMATIO=<key>
 ```
-
-Windows (cmd):
-
+Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
+If you are not sure, don't set this variable. Default value is 'default'
 ```bash
-set TESTOMATIO=<key>
+TESTOMATIO_CODE_STYLE=pep8
 ```
 
+```bash
+
+
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
 
 ### pytest.ini
 In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
 testomat.io url in it
```

### Comparing `pytestomatio-2.2.6/pyproject.toml` & `pytestomatio-2.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.2.6"
+version = "2.3.0"
 
 dependencies = [
     "requests>=2.29.0",
-    "pytest>8.0.0",
+    "pytest>7.2.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
     "autopep8>=2.1.0"]
 
 authors = [
     { name = "Oleksii Ostapov" },
@@ -33,14 +33,18 @@
 classifiers = [
     "Framework :: Pytest",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[tool.pytest.ini_options]
+minversion = "7.0"
+pytest_plugins = ["dotenv"]
+
 [project.urls]
 "Testomat.io" = "https://testomat.io/"
 "Homepage" = "https://github.com/testomatio/pytestomatio"
 "Bug Tracker" = "https://github.com/testomatio/pytestomatio/issues"
 
 [project.entry-points.pytest11]
 pytestomatio = "pytestomatio.main"
```

### Comparing `pytestomatio-2.2.6/pytestomatio/code_collector.py` & `pytestomatio-2.3.0/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/connector.py` & `pytestomatio-2.3.0/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/decorator_updater.py` & `pytestomatio-2.3.0/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/helper.py` & `pytestomatio-2.3.0/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/main.py` & `pytestomatio-2.3.0/pytestomatio/main.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/s3_connector.py` & `pytestomatio-2.3.0/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/testItem.py` & `pytestomatio-2.3.0/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/testRunConfig.py` & `pytestomatio-2.3.0/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio/testomatio.py` & `pytestomatio-2.3.0/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.6/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.3.0/pytestomatio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.6
+Version: 2.3.0
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
-Requires-Dist: pytest>8.0.0
+Requires-Dist: pytest>7.2.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 Requires-Dist: autopep8>=2.1.0
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
@@ -61,28 +61,27 @@
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
 ## configuration
-
 Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
 ```bash
-export TESTOMATIO=<key>
+TESTOMATIO=<key>
 ```
-
-Windows (cmd):
-
+Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
+If you are not sure, don't set this variable. Default value is 'default'
 ```bash
-set TESTOMATIO=<key>
+TESTOMATIO_CODE_STYLE=pep8
 ```
 
+```bash
+
+
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
 
 ### pytest.ini
 In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
 testomat.io url in it
```

### Comparing `pytestomatio-2.2.6/tests/test_root.py` & `pytestomatio-2.3.0/tests/test_root.py`

 * *Files identical despite different names*

