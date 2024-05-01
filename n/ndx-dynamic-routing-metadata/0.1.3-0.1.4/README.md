# Comparing `tmp/ndx_dynamic_routing_metadata-0.1.3.tar.gz` & `tmp/ndx_dynamic_routing_metadata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.3.tar", last modified: Tue Apr 30 23:16:03 2024, max compression
+gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.4.tar", last modified: Tue Apr 30 23:28:27 2024, max compression
```

## Comparing `ndx_dynamic_routing_metadata-0.1.3.tar` & `ndx_dynamic_routing_metadata-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-30 23:16:01.000000 ndx_dynamic_routing_metadata-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-30 23:15:58.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-30 23:28:25.000000 ndx_dynamic_routing_metadata-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.533454 ndx_dynamic_routing_metadata-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.533454 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/pynwb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 23:28:27.000000 ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:28:27.537454 ndx_dynamic_routing_metadata-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 23:28:03.000000 ndx_dynamic_routing_metadata-0.1.4/tests/test_core.py
```

### Comparing `ndx_dynamic_routing_metadata-0.1.3/LICENSE` & `ndx_dynamic_routing_metadata-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/LICENSE.txt` & `ndx_dynamic_routing_metadata-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.3
+Version: 0.1.4
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.3/README.md` & `ndx_dynamic_routing_metadata-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.3
+Version: 0.1.4
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.3/pyproject.toml` & `ndx_dynamic_routing_metadata-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "nwb-extension",
     "ndx-extension",
 ]
 dependencies = [
     "pynwb>=2.6.0",
     "hdmf>=3.13.0",
 ]
-version = "0.1.3"
+version = "0.1.4"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
@@ -45,21 +45,21 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = [
     "src",
-    "spec/ndx-dynamic-routing-metadata.extensions.yaml",
-    "spec/ndx-dynamic-routing-metadata.namespace.yaml",
 ]
 
 [tool.setuptools.package-data]
 ndx_dynamic_routing_metadata = [
     "py.typed",
+    "spec/ndx-dynamic-routing-metadata.extensions.yaml",
+    "spec/ndx-dynamic-routing-metadata.namespace.yaml",
 ]
 
 [tool.black]
 target-version = [
     "py39",
     "py310",
     "py311",
```

### Comparing `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/__init__.py` & `ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/__init__.py` & `ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/pynwb/__init__.py`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py` & `ndx_dynamic_routing_metadata-0.1.4/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.3/tests/test_core.py` & `ndx_dynamic_routing_metadata-0.1.4/tests/test_core.py`

 * *Files identical despite different names*

