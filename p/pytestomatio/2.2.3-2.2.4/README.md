# Comparing `tmp/pytestomatio-2.2.3.tar.gz` & `tmp/pytestomatio-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.2.3.tar", last modified: Wed May  1 11:11:52 2024, max compression
+gzip compressed data, was "pytestomatio-2.2.4.tar", last modified: Wed May  1 12:14:43 2024, max compression
```

## Comparing `pytestomatio-2.2.3.tar` & `pytestomatio-2.2.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 11:11:52.000000 pytestomatio-2.2.3/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.817200 pytestomatio-2.2.3/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:52.821200 pytestomatio-2.2.3/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 11:11:48.000000 pytestomatio-2.2.3/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.384466 pytestomatio-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-01 12:14:43.384466 pytestomatio-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.380466 pytestomatio-2.2.4/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.384466 pytestomatio-2.2.4/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 12:14:43.000000 pytestomatio-2.2.4/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:14:43.384466 pytestomatio-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.380466 pytestomatio-2.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.380466 pytestomatio-2.2.4/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:43.384466 pytestomatio-2.2.4/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 12:14:33.000000 pytestomatio-2.2.4/tests/test_root.py
```

### Comparing `pytestomatio-2.2.3/LICENSE` & `pytestomatio-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/PKG-INFO` & `pytestomatio-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.3
+Version: 2.2.4
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -117,14 +117,16 @@
 You would need to decide when you want to upload your test artifacts to cloud storage
 
 1) Upload page screenshot when test fails, using fixtures [reference](https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures)
 
 ```python
 # content of conftest.py
 import pytest
+import random
+import os
 from typing import Dict
 from pytest import StashKey, CollectReport
 from playwright.sync_api import Page
 
 phase_report_key = StashKey[Dict[str, CollectReport]]()
 
 @pytest.hookimpl(wrapper=True, tryfirst=True)
@@ -173,18 +175,18 @@
 
 ## Example of test
 
 To make the experience more consistent, it uses standard pytest markers.  
 testomat.io test id is a string value that starts with `@T` and has 8 symbols after.
 
 ```python
-import pytest
+from pytest import mark
 
 
-@pytest.mark.testomatio('@T96c700e6')
+@mark.testomatio('@T96c700e6')
 def test_example():
     assert 2 + 2 == 4
 ```
 
 ### Compatibility table with [Testomatio check-tests](https://github.com/testomatio/check-tests)
 
 | Action |  Compatibility | Method |
```

### Comparing `pytestomatio-2.2.3/README.md` & `pytestomatio-2.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 You would need to decide when you want to upload your test artifacts to cloud storage
 
 1) Upload page screenshot when test fails, using fixtures [reference](https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures)
 
 ```python
 # content of conftest.py
 import pytest
+import random
+import os
 from typing import Dict
 from pytest import StashKey, CollectReport
 from playwright.sync_api import Page
 
 phase_report_key = StashKey[Dict[str, CollectReport]]()
 
 @pytest.hookimpl(wrapper=True, tryfirst=True)
@@ -152,18 +154,18 @@
 
 ## Example of test
 
 To make the experience more consistent, it uses standard pytest markers.  
 testomat.io test id is a string value that starts with `@T` and has 8 symbols after.
 
 ```python
-import pytest
+from pytest import mark
 
 
-@pytest.mark.testomatio('@T96c700e6')
+@mark.testomatio('@T96c700e6')
 def test_example():
     assert 2 + 2 == 4
 ```
 
 ### Compatibility table with [Testomatio check-tests](https://github.com/testomatio/check-tests)
 
 | Action |  Compatibility | Method |
```

### Comparing `pytestomatio-2.2.3/pyproject.toml` & `pytestomatio-2.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.2.3"
+version = "2.2.4"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>8.0.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1"]
```

### Comparing `pytestomatio-2.2.3/pytestomatio/code_collector.py` & `pytestomatio-2.2.4/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/connector.py` & `pytestomatio-2.2.4/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/helper.py` & `pytestomatio-2.2.4/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/main.py` & `pytestomatio-2.2.4/pytestomatio/main.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/s3_connector.py` & `pytestomatio-2.2.4/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/testItem.py` & `pytestomatio-2.2.4/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/testRunConfig.py` & `pytestomatio-2.2.4/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio/testomatio.py` & `pytestomatio-2.2.4/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.2.3/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.2.4/pytestomatio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.2.3
+Version: 2.2.4
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -117,14 +117,16 @@
 You would need to decide when you want to upload your test artifacts to cloud storage
 
 1) Upload page screenshot when test fails, using fixtures [reference](https://docs.pytest.org/en/latest/example/simple.html#making-test-result-information-available-in-fixtures)
 
 ```python
 # content of conftest.py
 import pytest
+import random
+import os
 from typing import Dict
 from pytest import StashKey, CollectReport
 from playwright.sync_api import Page
 
 phase_report_key = StashKey[Dict[str, CollectReport]]()
 
 @pytest.hookimpl(wrapper=True, tryfirst=True)
@@ -173,18 +175,18 @@
 
 ## Example of test
 
 To make the experience more consistent, it uses standard pytest markers.  
 testomat.io test id is a string value that starts with `@T` and has 8 symbols after.
 
 ```python
-import pytest
+from pytest import mark
 
 
-@pytest.mark.testomatio('@T96c700e6')
+@mark.testomatio('@T96c700e6')
 def test_example():
     assert 2 + 2 == 4
 ```
 
 ### Compatibility table with [Testomatio check-tests](https://github.com/testomatio/check-tests)
 
 | Action |  Compatibility | Method |
```

### Comparing `pytestomatio-2.2.3/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.2.4/pytestomatio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pytestomatio.egg-info/PKG-INFO
 pytestomatio.egg-info/SOURCES.txt
 pytestomatio.egg-info/dependency_links.txt
 pytestomatio.egg-info/entry_points.txt
 pytestomatio.egg-info/requires.txt
 pytestomatio.egg-info/top_level.txt
 tests/test_class_root.py
+tests/test_decorators.py
 tests/test_root.py
 tests/sub/__init__.py
 tests/sub/test_class_sub.py
 tests/sub/test_sub.py
 tests/sub/sub_mob/__init__.py
 tests/sub/sub_mob/sub_sub_class_test.py
 tests/sub/sub_mob/sub_sub_test.py
```

### Comparing `pytestomatio-2.2.3/tests/test_root.py` & `pytestomatio-2.2.4/tests/test_root.py`

 * *Files identical despite different names*

