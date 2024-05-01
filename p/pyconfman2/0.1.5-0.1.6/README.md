# Comparing `tmp/pyconfman2-0.1.5.tar.gz` & `tmp/pyconfman2-0.1.6.tar.gz`

## Comparing `pyconfman2-0.1.5.tar` & `pyconfman2-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/tests/test_schema_config.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/LICENSE
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyconfman2-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/tests/test_schema_config.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pyconfman2-0.1.6/PKG-INFO
```

### Comparing `pyconfman2-0.1.5/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.6/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.5/src/pyconfman2/Schema.py` & `pyconfman2-0.1.6/src/pyconfman2/Schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.5/tests/test_schema.py` & `pyconfman2-0.1.6/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.5/LICENSE` & `pyconfman2-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.5/README.md` & `pyconfman2-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.5/pyproject.toml` & `pyconfman2-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "yaml",
+]
 
 [project.urls]
 Homepage = "https://github.com/PhillypHenning/python-config-parser"
 Issues = "https://github.com/PhillypHenning/python-config-parser/issues"
```

### Comparing `pyconfman2-0.1.5/PKG-INFO` & `pyconfman2-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: yaml
 Description-Content-Type: text/markdown
 
 # pyconfman2
 
 pyconfman2 is designed to handle schema configurations by loading properties from a dictionary or a YAML configuration file. It provides methods for adding, getting, and removing properties from the schema.
 
 ## Installation
```

