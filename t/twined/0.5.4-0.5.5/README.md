# Comparing `tmp/twined-0.5.4.tar.gz` & `tmp/twined-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twined-0.5.4.tar", last modified: Thu Apr 25 15:59:06 2024, max compression
+gzip compressed data, was "twined-0.5.5.tar", last modified: Wed May  1 11:07:07 2024, max compression
```

## Comparing `twined-0.5.4.tar` & `twined-0.5.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 15:59:04.000000 twined-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-25 15:59:04.000000 twined-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-25 15:59:06.823912 twined-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 15:59:04.000000 twined-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 15:59:06.823912 twined-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 15:59:04.000000 twined-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_manifest_strands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_schema_strands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_twine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/twined/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 15:59:04.000000 twined-0.5.4/twined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-25 15:59:04.000000 twined-0.5.4/twined/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/twined/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-25 15:59:04.000000 twined-0.5.4/twined/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2174030 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/plotly_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/twine_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-25 15:59:04.000000 twined-0.5.4/twined/twine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/load_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.179858 twined-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-01 11:06:55.000000 twined-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 11:06:55.000000 twined-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-01 11:07:07.179858 twined-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-01 11:06:55.000000 twined-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 11:07:07.179858 twined-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-01 11:06:55.000000 twined-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.171858 twined-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_manifest_strands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_schema_strands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_twine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 11:06:55.000000 twined-0.5.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.171858 twined-0.5.5/twined/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 11:06:55.000000 twined-0.5.5/twined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-01 11:06:55.000000 twined-0.5.5/twined/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.175858 twined-0.5.5/twined/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-01 11:06:55.000000 twined-0.5.5/twined/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.175858 twined-0.5.5/twined/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:06:55.000000 twined-0.5.5/twined/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2174030 2024-05-01 11:06:55.000000 twined-0.5.5/twined/schema/plotly_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-01 11:06:55.000000 twined-0.5.5/twined/schema/twine_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-05-01 11:06:55.000000 twined-0.5.5/twined/twine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.179858 twined-0.5.5/twined/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 11:06:55.000000 twined-0.5.5/twined/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 11:06:55.000000 twined-0.5.5/twined/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-01 11:06:55.000000 twined-0.5.5/twined/utils/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-01 11:06:55.000000 twined-0.5.5/twined/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:07:07.179858 twined-0.5.5/twined.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-01 11:07:07.000000 twined-0.5.5/twined.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-01 11:07:07.000000 twined-0.5.5/twined.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:07:07.000000 twined-0.5.5/twined.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 11:07:07.000000 twined-0.5.5/twined.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 11:07:07.000000 twined-0.5.5/twined.egg-info/top_level.txt
```

### Comparing `twined-0.5.4/LICENSE` & `twined-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/PKG-INFO` & `twined-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twined
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library to help digital twins and data services talk to one another
 Home-page: https://www.github.com/octue/twined
 Author: Octue (github: octue)
 License: MIT
 Keywords: digital,twins,data,services,python,schema
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema~=4.4.0
+Requires-Dist: jsonschema<5,>=4
 Requires-Dist: python-dotenv
 
 # twined
 
 A library to help digital twins and data services talk to one another. Read more at [twined.readthedocs.io](https://twined.readthedocs.io)
 
 [![PyPI version](https://badge.fury.io/py/twined.svg)](https://badge.fury.io/py/twined)
```

### Comparing `twined-0.5.4/README.md` & `twined-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/setup.cfg` & `twined-0.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/setup.py` & `twined-0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,20 @@
     readme_text = f.read()
 
 with open("LICENSE") as f:
     license_text = f.read()
 
 setup(
     name="twined",
-    version="0.5.4",
+    version="0.5.5",
     py_modules=[],
-    install_requires=["jsonschema ~= 4.4.0", "python-dotenv"],
+    install_requires=[
+        "jsonschema>=4,<5",
+        "python-dotenv",
+    ],
     url="https://www.github.com/octue/twined",
     license="MIT",
     author="Octue (github: octue)",
     description="A library to help digital twins and data services talk to one another",
     long_description=readme_text,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests", "docs")),
```

### Comparing `twined-0.5.4/tests/test_children.py` & `twined-0.5.5/tests/test_children.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_credentials.py` & `twined-0.5.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_manifest_strands.py` & `twined-0.5.5/tests/test_manifest_strands.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_monitors.py` & `twined-0.5.5/tests/test_monitors.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_schema_strands.py` & `twined-0.5.5/tests/test_schema_strands.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_twine.py` & `twined-0.5.5/tests/test_twine.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/tests/test_utils.py` & `twined-0.5.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/exceptions.py` & `twined-0.5.5/twined/exceptions.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/schema/plotly_schema.json` & `twined-0.5.5/twined/schema/plotly_schema.json`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/schema/twine_schema.json` & `twined-0.5.5/twined/schema/twine_schema.json`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/twine.py` & `twined-0.5.5/twined/twine.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/utils/encoders.py` & `twined-0.5.5/twined/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined/utils/load_json.py` & `twined-0.5.5/twined/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.4/twined.egg-info/PKG-INFO` & `twined-0.5.5/twined.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twined
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library to help digital twins and data services talk to one another
 Home-page: https://www.github.com/octue/twined
 Author: Octue (github: octue)
 License: MIT
 Keywords: digital,twins,data,services,python,schema
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema~=4.4.0
+Requires-Dist: jsonschema<5,>=4
 Requires-Dist: python-dotenv
 
 # twined
 
 A library to help digital twins and data services talk to one another. Read more at [twined.readthedocs.io](https://twined.readthedocs.io)
 
 [![PyPI version](https://badge.fury.io/py/twined.svg)](https://badge.fury.io/py/twined)
```

### Comparing `twined-0.5.4/twined.egg-info/SOURCES.txt` & `twined-0.5.5/twined.egg-info/SOURCES.txt`

 * *Files identical despite different names*

