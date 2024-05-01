# Comparing `tmp/snowflake_legacy-0.7.0.tar.gz` & `tmp/snowflake_legacy-0.8.0.tar.gz`

## Comparing `snowflake_legacy-0.7.0.tar` & `snowflake_legacy-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/snowflake.pth
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/snowflake/_legacy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/tests/test_legacy_api.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/.gitignore
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/README.md
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 snowflake_legacy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/snowflake.pth
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/snowflake/_legacy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/tests/test_legacy_api.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/PKG-INFO
```

### Comparing `snowflake_legacy-0.7.0/snowflake.pth` & `snowflake_legacy-0.8.0/snowflake.pth`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.7.0/snowflake/_legacy/__init__.py` & `snowflake_legacy-0.8.0/snowflake/_legacy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 
 
 from typing import Optional
 
 
 SNOWFLAKE_FILE = '/etc/snowflake'
```

### Comparing `snowflake_legacy-0.7.0/tests/test_legacy_api.py` & `snowflake_legacy-0.8.0/tests/test_legacy_api.py`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.7.0/.gitignore` & `snowflake_legacy-0.8.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -74,9 +74,9 @@
 
 ##############################
 ## Auto Summary
 ##############################
 docs/source/_autosummary/*
 
 .coverage
-/libs/*/coverage-3.*.xml
+/libs/*/coverage-*.xml
 /.github/workflows/parameters/connections.toml
```

### Comparing `snowflake_legacy-0.7.0/README.md` & `snowflake_legacy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.7.0/pyproject.toml` & `snowflake_legacy-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,31 +56,34 @@
     'data/snowflake.pth',
     'README.md',
     'tests/',
     'CHANGELOG.md',
     'pyproject.toml',
 ]
 
-[[tool.hatch.envs.test.matrix]]
+[tool.hatch.envs.test_all]
+template = 'test'
+
+[[tool.hatch.envs.test_all.matrix]]
 python = ['3.8', '3.9', '3.10', '3.11']
 
 [tool.hatch.envs.test]
 dependencies = [
     'coverage[toml]',
     'diff-cover',
     'pytest',
     'pytest-cov',
     'sybil',
 ]
 
 [tool.hatch.envs.test.scripts]
 check = [
-    'pytest --cov-report=xml:coverage-{matrix:python}.xml {args:tests}',
+    'pytest --cov-report=xml:coverage-{matrix:python:{env:PYTHON_VERSION:unset}}.xml {args:tests}',
     # The following is only useful in a git repository; thus errors are ignored.
-    '- diff-cover coverage-{matrix:python}.xml',
+    '- diff-cover coverage-{matrix:python:{env:PYTHON_VERSION:unset}}.xml',
 ]
 
 [tool.hatch.envs.precommit]
 dependencies = [
     'black',                    # 2023-08-08(bwarsaw): Change to `blue` in followup PR
     'mypy',
     'ruff',
```

### Comparing `snowflake_legacy-0.7.0/PKG-INFO` & `snowflake_legacy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake._legacy
-Version: 0.7.0
+Version: 0.8.0
 Summary: You should switch to the snowflake-uuid package
 Author-email: "Snowflake, Inc." <snowflake-python-libraries-dl@snowflake.com>
 License: Apache-2.0
 Keywords: Snowflake,analytics,cloud,database,db,warehouse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
```

