# Comparing `tmp/ndx_dynamic_routing_metadata-0.1.2.tar.gz` & `tmp/ndx_dynamic_routing_metadata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.2.tar", last modified: Tue Apr 30 18:50:02 2024, max compression
+gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.3.tar", last modified: Tue Apr 30 23:16:03 2024, max compression
```

## Comparing `ndx_dynamic_routing_metadata-0.1.2.tar` & `ndx_dynamic_routing_metadata-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-30 18:50:00.000000 ndx_dynamic_routing_metadata-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.402775 ndx_dynamic_routing_metadata-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 23:16:03.000000 ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-30 23:16:01.000000 ndx_dynamic_routing_metadata-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:16:03.978082 ndx_dynamic_routing_metadata-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-30 23:15:58.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:16:03.974082 ndx_dynamic_routing_metadata-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 23:15:38.000000 ndx_dynamic_routing_metadata-0.1.3/tests/test_core.py
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/LICENSE` & `ndx_dynamic_routing_metadata-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.2/LICENSE.txt` & `ndx_dynamic_routing_metadata-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.2/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/README.md` & `ndx_dynamic_routing_metadata-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt` & `ndx_dynamic_routing_metadata-0.1.3/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.2/pyproject.toml` & `ndx_dynamic_routing_metadata-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "nwb-extension",
     "ndx-extension",
 ]
 dependencies = [
     "pynwb>=2.6.0",
     "hdmf>=3.13.0",
 ]
-version = "0.1.2"
+version = "0.1.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
@@ -45,16 +45,16 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = [
     "src",
-    "src/ndx_dynamic_routing_metadata/spec/ndx-dynamic-routing-metadata.extensions.yaml",
-    "src/ndx_dynamic_routing_metadata/spec/ndx-dynamic-routing-metadata.namespace.yaml",
+    "spec/ndx-dynamic-routing-metadata.extensions.yaml",
+    "spec/ndx-dynamic-routing-metadata.namespace.yaml",
 ]
 
 [tool.setuptools.package-data]
 ndx_dynamic_routing_metadata = [
     "py.typed",
 ]
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/__init__.py` & `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/__init__.py` & `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/pynwb/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,30 @@
     from importlib.resources import files
 except ImportError:
     # TODO: Remove when python 3.9 becomes the new minimum
     from importlib_resources import files
 
 # Get path to the namespace.yaml file with the expected location when installed not in editable mode
 __location_of_this_file = files(__name__)
-__spec_path = (
-    __location_of_this_file.parent
-    / "spec"
-    / "ndx-dynamic-routing-metadata.namespace.yaml"
+
+__spec_path = os.path.join(
+    __location_of_this_file.parent,
+    "spec",
+    "ndx-dynamic-routing-metadata.namespace.yaml",
 )
 
+
+if not os.path.exists(__spec_path):
+    __spec_path = (
+        __location_of_this_file.parent.parent.parent
+        / "spec"
+        / "ndx-dynamic-routing-metadata.namespace.yaml"
+    )
+
+
 # Load the namespace
 load_namespaces(str(__spec_path))
 
 # TODO: Define your classes here to make them accessible at the package level.
 # Either have PyNWB generate a class from the spec using `get_class` as shown
 # below or write a custom class and register it using the class decorator
 # `@register_class("TetrodeSeries", "ndx-dynamic-routing-metadata")`
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py` & `ndx_dynamic_routing_metadata-0.1.3/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         required=False,
     )
 
     # TODO: add more attributes/groups as needed
     new_data_types = [DynamicRoutingMetadataExtension]
 
     # export the spec to yaml files in the spec folder
-    output_dir = os.path.abspath(os.path.join(os.path.dirname(__file__)))
+    output_dir = os.path.abspath(
+        os.path.join(os.path.dirname(__file__), "..", "..", "..", "spec")
+    )
     export_spec(ns_builder, new_data_types, output_dir)
 
 
 if __name__ == "__main__":
     # usage: python create_extension_spec.py
     main()
```

### Comparing `ndx_dynamic_routing_metadata-0.1.2/tests/test_core.py` & `ndx_dynamic_routing_metadata-0.1.3/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import ndx_dynamic_routing_metadata
-
 import os
 import unittest
 from datetime import datetime
 from pynwb import NWBHDF5IO, NWBFile
 from ndx_dynamic_routing_metadata import DynamicRoutingMetadataExtension
```

