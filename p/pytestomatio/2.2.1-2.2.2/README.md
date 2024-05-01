# Comparing `tmp/pytestomatio-2.2.1.tar.gz` & `tmp/pytestomatio-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.2.1.tar", last modified: Wed Apr 17 14:42:12 2024, max compression
+gzip compressed data, was "pytestomatio-2.2.2.tar", last modified: Wed May  1 10:08:53 2024, max compression
```

## Comparing `pytestomatio-2.2.1.tar` & `pytestomatio-2.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.676660 pytestomatio-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-17 14:42:12.676660 pytestomatio-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.672660 pytestomatio-2.2.1/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.676660 pytestomatio-2.2.1/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 14:42:12.000000 pytestomatio-2.2.1/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:42:12.676660 pytestomatio-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.672660 pytestomatio-2.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.672660 pytestomatio-2.2.1/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:12.676660 pytestomatio-2.2.1/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 14:42:03.000000 pytestomatio-2.2.1/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 10:08:53.000000 pytestomatio-2.2.2/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.624867 pytestomatio-2.2.2/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:53.628867 pytestomatio-2.2.2/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 10:08:48.000000 pytestomatio-2.2.2/tests/test_root.py
```

### Comparing `pytestomatio-2.2.1/LICENSE` & `pytestomatio-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/PKG-INFO` & `pytestomatio-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
-Project-URL: Homepage, https://github.com/tikolakin/pytestomatio
-Project-URL: Bug Tracker, https://github.com/tikolakin/pytestomatio/issues
+Project-URL: Homepage, https://github.com/testomatio/pytestomatio
+Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,43 +27,15 @@
 
 - https://testomatio.github.io/check-tests/
 - https://testomatio.github.io/reporter/
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/tikolakin/pytestomatio.git@1.7#egg=pytestomatio
-```
-
-## configuration
-
-Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
-```bash
-export TESTOMATIO=<key>
-```
-
-Windows (cmd):
-
-```bash
-set TESTOMATIO=<key>
-```
-
-### Run groups parameter
-There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
-
-### pytest.ini
-In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
-testomat.io url in it
-
-```ini
-[pytest]
-testomatio_url = https://app.testomat.io
-
+pip install pytestomatio
 ```
 
 ## Usage
 
 Synchronize tests to testomat.io and get back test id.
 Tests will not be executed
 
@@ -87,14 +59,42 @@
 
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
+## configuration
+
+Create environment variable `TESTOMATIO` and set your testomat.io API key.
+Linux:
+
+```bash
+export TESTOMATIO=<key>
+```
+
+Windows (cmd):
+
+```bash
+set TESTOMATIO=<key>
+```
+
+### Run groups parameter
+There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
+
+### pytest.ini
+In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
+testomat.io url in it
+
+```ini
+[pytest]
+testomatio_url = https://app.testomat.io
+
+```
+
 ### Submitting Test Run Environment
 
 to configure test environment, you can use additional option:
 
 ```bash
 pytest --testomatio report --testRunEnv "windows11,chrome,1920x1080"
 ```
```

### Comparing `pytestomatio-2.2.1/README.md` & `pytestomatio-2.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,43 +6,15 @@
 
 - https://testomatio.github.io/check-tests/
 - https://testomatio.github.io/reporter/
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/tikolakin/pytestomatio.git@1.7#egg=pytestomatio
-```
-
-## configuration
-
-Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
-```bash
-export TESTOMATIO=<key>
-```
-
-Windows (cmd):
-
-```bash
-set TESTOMATIO=<key>
-```
-
-### Run groups parameter
-There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
-
-### pytest.ini
-In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
-testomat.io url in it
-
-```ini
-[pytest]
-testomatio_url = https://app.testomat.io
-
+pip install pytestomatio
 ```
 
 ## Usage
 
 Synchronize tests to testomat.io and get back test id.
 Tests will not be executed
 
@@ -66,14 +38,42 @@
 
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
+## configuration
+
+Create environment variable `TESTOMATIO` and set your testomat.io API key.
+Linux:
+
+```bash
+export TESTOMATIO=<key>
+```
+
+Windows (cmd):
+
+```bash
+set TESTOMATIO=<key>
+```
+
+### Run groups parameter
+There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
+
+### pytest.ini
+In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
+testomat.io url in it
+
+```ini
+[pytest]
+testomatio_url = https://app.testomat.io
+
+```
+
 ### Submitting Test Run Environment
 
 to configure test environment, you can use additional option:
 
 ```bash
 pytest --testomatio report --testRunEnv "windows11,chrome,1920x1080"
 ```
```

### Comparing `pytestomatio-2.2.1/pyproject.toml` & `pytestomatio-2.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.2.1"
+version = "2.2.2"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest<8.0.0,>=7.3.1",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1"]
@@ -34,12 +34,12 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Testomat.io" = "https://testomat.io/"
-"Homepage" = "https://github.com/tikolakin/pytestomatio"
-"Bug Tracker" = "https://github.com/tikolakin/pytestomatio/issues"
+"Homepage" = "https://github.com/testomatio/pytestomatio"
+"Bug Tracker" = "https://github.com/testomatio/pytestomatio/issues"
 
 [project.entry-points.pytest11]
 pytestomatio = "pytestomatio.main"
```

### Comparing `pytestomatio-2.2.1/pytestomatio/code_collector.py` & `pytestomatio-2.2.2/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/connector.py` & `pytestomatio-2.2.2/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/decorator_updater.py` & `pytestomatio-2.2.2/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/helper.py` & `pytestomatio-2.2.2/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/main.py` & `pytestomatio-2.2.2/pytestomatio/main.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/s3_connector.py` & `pytestomatio-2.2.2/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/testItem.py` & `pytestomatio-2.2.2/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/testRunConfig.py` & `pytestomatio-2.2.2/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio/testomatio.py` & `pytestomatio-2.2.2/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.2.2/pytestomatio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
-Project-URL: Homepage, https://github.com/tikolakin/pytestomatio
-Project-URL: Bug Tracker, https://github.com/tikolakin/pytestomatio/issues
+Project-URL: Homepage, https://github.com/testomatio/pytestomatio
+Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,43 +27,15 @@
 
 - https://testomatio.github.io/check-tests/
 - https://testomatio.github.io/reporter/
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/tikolakin/pytestomatio.git@1.7#egg=pytestomatio
-```
-
-## configuration
-
-Create environment variable `TESTOMATIO` and set your testomat.io API key.
-Linux:
-
-```bash
-export TESTOMATIO=<key>
-```
-
-Windows (cmd):
-
-```bash
-set TESTOMATIO=<key>
-```
-
-### Run groups parameter
-There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
-
-### pytest.ini
-In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
-testomat.io url in it
-
-```ini
-[pytest]
-testomatio_url = https://app.testomat.io
-
+pip install pytestomatio
 ```
 
 ## Usage
 
 Synchronize tests to testomat.io and get back test id.
 Tests will not be executed
 
@@ -87,14 +59,42 @@
 
 Run pytest with debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --testomatio debug
 ```
 
+## configuration
+
+Create environment variable `TESTOMATIO` and set your testomat.io API key.
+Linux:
+
+```bash
+export TESTOMATIO=<key>
+```
+
+Windows (cmd):
+
+```bash
+set TESTOMATIO=<key>
+```
+
+### Run groups parameter
+There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
+
+### pytest.ini
+In case you are using private testomat.io service, create `pytest.ini` file in your project root directory. Specify
+testomat.io url in it
+
+```ini
+[pytest]
+testomatio_url = https://app.testomat.io
+
+```
+
 ### Submitting Test Run Environment
 
 to configure test environment, you can use additional option:
 
 ```bash
 pytest --testomatio report --testRunEnv "windows11,chrome,1920x1080"
 ```
```

### Comparing `pytestomatio-2.2.1/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.2.2/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.1/tests/test_root.py` & `pytestomatio-2.2.2/tests/test_root.py`

 * *Files identical despite different names*

