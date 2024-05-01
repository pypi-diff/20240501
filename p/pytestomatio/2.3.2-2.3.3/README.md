# Comparing `tmp/pytestomatio-2.3.2.tar.gz` & `tmp/pytestomatio-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.3.2.tar", last modified: Wed May  1 14:52:36 2024, max compression
+gzip compressed data, was "pytestomatio-2.3.3.tar", last modified: Wed May  1 15:36:27 2024, max compression
```

## Comparing `pytestomatio-2.3.2.tar` & `pytestomatio-2.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.757880 pytestomatio-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:52:36.757880 pytestomatio-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.753880 pytestomatio-2.3.2/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.753880 pytestomatio-2.3.2/pytestomatio/decor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/decor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/decor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/decor/pep8.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.757880 pytestomatio-2.3.2/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:52:36.000000 pytestomatio-2.3.2/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:52:36.757880 pytestomatio-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.753880 pytestomatio-2.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.753880 pytestomatio-2.3.2/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:36.757880 pytestomatio-2.3.2/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 14:52:31.000000 pytestomatio-2.3.2/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.450060 pytestomatio-2.3.3/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.450060 pytestomatio-2.3.3/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 15:36:27.000000 pytestomatio-2.3.3/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:27.454060 pytestomatio-2.3.3/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 15:36:21.000000 pytestomatio-2.3.3/tests/test_root.py
```

### Comparing `pytestomatio-2.3.2/LICENSE` & `pytestomatio-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/PKG-INFO` & `pytestomatio-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.2
+Version: 2.3.3
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE
 Requires-Dist: requests>=2.29.0
 Requires-Dist: pytest>7.2.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 Requires-Dist: autopep8>=2.1.0
+Requires-Dist: pytest-dotenv>=0.5.2
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
 # testomat.io plugin for pytest
 
 ## uses testomat.io API:
```

### Comparing `pytestomatio-2.3.2/README.md` & `pytestomatio-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/code_collector.py` & `pytestomatio-2.3.3/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/connector.py` & `pytestomatio-2.3.3/pytestomatio/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/decor/default.py` & `pytestomatio-2.3.3/pytestomatio/decor/default.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/decor/pep8.py` & `pytestomatio-2.3.3/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/decorator_updater.py` & `pytestomatio-2.3.3/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/helper.py` & `pytestomatio-2.3.3/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/main.py` & `pytestomatio-2.3.3/pytestomatio/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os, pytest, logging, json, re
 
-from pytest import Parser, Session, Config, Item, CallInfo
+from pytest import Parser, Session, Config, Item, CallInfo, fixture, FixtureRequest
 from .connector import Connector
 from .decorator_updater import update_tests
 from .testRunConfig import TestRunConfig
 from .testItem import TestItem
 from .s3_connector import S3Connector
 from .testomatio import Testomatio
 from .helper import add_and_enrich_tests, get_test_mapping, get_functions_source_by_name, collect_tests
@@ -29,23 +29,23 @@
     parser.addoption(f'--{testomatio}',
                      action='store',
                      help=help_text)
     parser.addoption(f'--testRunEnv',
                      action='store',
                      help=f'specify test run environment for testomat.io. Works only with --testomatio sync')
     parser.addoption(f'--create',
-                    action='store_true',
-                    default=False,
-                    dest="create",
-                    help="""
+                     action='store_true',
+                     default=False,
+                     dest="create",
+                     help="""
                         To import tests with Test IDs set in source code into a project use --create option.
                         In this case a project will be populated with the same Test IDs as in the code.
                         Use --testomatio sync together with --create option to enable this behavior.
                         """
-                    )
+                     )
     parser.addoption(f'--no-empty',
                      action='store_true',
                      default=False,
                      dest="no_empty",
                      help="""
                         Delete empty suites.
                         When tests are marked with IDs and imported to already created suites in Testomat.io newly imported suites may become empty.
@@ -67,15 +67,15 @@
                      action='store_true',
                      default=False,
                      dest="keep_structure",
                      help="""
                         Keep structure of source code. If suites are not created in Testomat.io they will be created based on the file structure.
                         Use --testomatio sync together with --structure option to enable this behaviour.
                         """
-                    )
+                     )
     parser.addoption('--directory',
                      default=None,
                      dest="directory",
                      help="""
                         Specify directory to use for test file structure, ex. --directory Windows\\smoke or --directory Linux/e2e
                         Use --testomatio sync together with --directory option to enable this behaviour.
                         Default is the root of the project.
@@ -85,43 +85,44 @@
     parser.addini('testomatio_url', 'testomat.io base url', default='https://app.testomat.io')
 
 
 def pytest_configure(config: Config):
     config.addinivalue_line(
         "markers", "testomatio(arg): built in marker to connect test case with testomat.io by unique id"
     )
-    
+
     pytest.testomatio = Testomatio()
     test_run_config = TestRunConfig(
         id=os.environ.get('TESTOMATIO_RUN'),
         title=os.environ.get('TESTOMATIO_TITLE'),
         group_title=os.environ.get('TESTOMATIO_RUNGROUP_TITLE'),
         environment=os.environ.get('TESTOMATIO_ENV'),
         shared_run=os.environ.get('TESTOMATIO_SHARED_RUN') in ['True', 'true', '1'],
         label=os.environ.get('TESTOMATIO_LABEL'),
     )
     pytest.testomatio.set_test_run(test_run_config)
-    pytest.s3_connector = pytest.testomatio.s3_connector # backward compatibility
+    pytest.s3_connector = pytest.testomatio.s3_connector  # backward compatibility
 
     if config.getoption(testomatio) in ('sync', 'report', 'remove'):
         url = config.getini('testomatio_url')
         project = os.environ.get('TESTOMATIO')
         if project is None:
             pytest.exit('TESTOMATIO env variable is not set')
         ## TODO: move connector tin testomatio
-        pytest.connector = Connector(url, project) # backward compatibility
+        pytest.connector = Connector(url, project)  # backward compatibility
         pytest.testomatio.connector = pytest.connector
         if config.getoption('testRunEnv'):
             pytest.testomatio.test_run.set_env(config.getoption('testRunEnv'))
 
-def pytest_runtestloop(session: Session):
-    if hasattr(pytest.testomatio, 'session'):
-        if pytest.testomatio.session == "sync":
-            print('Test sync with testomat.io finished')
-            pytest.exit('Exit without test execution')
+
+@fixture(autouse=True)
+def testomatio_skip_test_fixture(request: FixtureRequest):
+    if request.config.getoption(testomatio) in ['sync', 'remove']:
+        pytest.skip("Skipping this test because of some condition")
+
 
 def pytest_collection_modifyitems(session: Session, config: Config, items: list[Item]) -> None:
     if config.getoption(testomatio):
         meta, test_files, test_names = collect_tests(items)
         match config.getoption(testomatio):
             case 'sync':
                 pytest.testomatio.connector.load_tests(
@@ -132,45 +133,45 @@
                     create=config.getoption('create'),
                     directory=config.getoption('directory')
                 )
                 testomatio_tests = pytest.testomatio.connector.get_tests(meta)
                 add_and_enrich_tests(meta, test_files, test_names, testomatio_tests, decorator_name)
                 pytest.testomatio.session = "sync"
                 print(f'Found {len(items)} test. {len(meta)} unique test functions data collected and updated.')
-                print('Test sync with testomat.io finished')
-                pytest.skip('Skip all tests without execution')
             case 'remove':
                 mapping = get_test_mapping(meta)
                 for test_file in test_files:
                     update_tests(test_file, mapping, test_names, decorator_name, remove=True)
                 pytest.exit(
                     f'{len(items)} found. tests ids removed. Exit without test execution')
             case 'report':
                 if pytest.testomatio.test_run.test_run_id:
                     run_details = pytest.testomatio.connector.update_test_run(**pytest.testomatio.test_run.to_dict())
                 else:
                     run_details = pytest.testomatio.connector.create_test_run(**pytest.testomatio.test_run.to_dict())
                     pytest.testomatio.test_run.set_run_id(run_details['uid'])
-                
+
                 if run_details is None:
                     log.error('Test run failed to create. Reporting skipped')
                     return
 
                 if run_details.get('artifacts'):
                     s3_access_key = os.environ.get('ACCESS_KEY_ID') or run_details['artifacts'].get('ACCESS_KEY_ID')
-                    s3_secret_key = os.environ.get('SECRET_ACCESS_KEY') or run_details['artifacts'].get('SECRET_ACCESS_KEY')
+                    s3_secret_key = os.environ.get('SECRET_ACCESS_KEY') or run_details['artifacts'].get(
+                        'SECRET_ACCESS_KEY')
                     s3_endpoint = os.environ.get('ENDPOINT') or run_details['artifacts'].get('ENDPOINT')
                     s3_bucket = os.environ.get('BUCKET') or run_details['artifacts'].get('BUCKET')
                     if all((s3_access_key, s3_secret_key, s3_endpoint, s3_bucket)):
-                        pytest.testomatio.set_s3_connector(S3Connector(s3_access_key, s3_secret_key, s3_endpoint, s3_bucket))
+                        pytest.testomatio.set_s3_connector(
+                            S3Connector(s3_access_key, s3_secret_key, s3_endpoint, s3_bucket))
                         pytest.testomatio.s3_connector.login()
-                        pytest.s3_connector = pytest.testomatio.s3_connector # backward compatibility
+                        pytest.s3_connector = pytest.testomatio.s3_connector  # backward compatibility
                     else:
                         pytest.testomatio.set_s3_connector(S3Connector('', '', '', ''))
-                        pytest.s3_connector = pytest.testomatio.s3_connector # backward compatibility
+                        pytest.s3_connector = pytest.testomatio.s3_connector  # backward compatibility
             case 'debug':
                 with open(metadata_file, 'w') as file:
                     data = json.dumps([i.to_dict() for i in meta], indent=4)
                     file.write(data)
                 pytest.exit(
                     f'saved metadata to {metadata_file}. Exit without test execution')
             case _:
```

### Comparing `pytestomatio-2.3.2/pytestomatio/s3_connector.py` & `pytestomatio-2.3.3/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/testItem.py` & `pytestomatio-2.3.3/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/testRunConfig.py` & `pytestomatio-2.3.3/pytestomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio/testomatio.py` & `pytestomatio-2.3.3/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.3.3/pytestomatio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.2
+Version: 2.3.3
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE
 Requires-Dist: requests>=2.29.0
 Requires-Dist: pytest>7.2.0
 Requires-Dist: boto3>=1.28.28
 Requires-Dist: libcst==1.1.0
 Requires-Dist: commitizen>=3.18.1
 Requires-Dist: autopep8>=2.1.0
+Requires-Dist: pytest-dotenv>=0.5.2
 
 [![Support Ukraine Badge](https://bit.ly/support-ukraine-now)](https://github.com/support-ukraine/support-ukraine)
 
 # testomat.io plugin for pytest
 
 ## uses testomat.io API:
```

### Comparing `pytestomatio-2.3.2/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.3.3/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.2/tests/test_root.py` & `pytestomatio-2.3.3/tests/test_root.py`

 * *Files identical despite different names*

