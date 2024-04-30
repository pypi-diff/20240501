# Comparing `tmp/ndx_dynamic_routing_metadata-0.1.1.tar.gz` & `tmp/ndx_dynamic_routing_metadata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.1.tar", last modified: Mon Apr 29 19:21:37 2024, max compression
+gzip compressed data, was "ndx_dynamic_routing_metadata-0.1.2.tar", last modified: Tue Apr 30 18:50:02 2024, max compression
```

## Comparing `ndx_dynamic_routing_metadata-0.1.1.tar` & `ndx_dynamic_routing_metadata-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-29 19:21:35.000000 ndx_dynamic_routing_metadata-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.767141 ndx_dynamic_routing_metadata-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 19:21:32.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.767141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/ndx_dynamic_routing_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 19:21:32.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/ndx_dynamic_routing_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 19:21:32.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/tests/test_dynamic_routing_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-29 19:21:32.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 19:21:37.000000 ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:21:37.771141 ndx_dynamic_routing_metadata-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 19:21:13.000000 ndx_dynamic_routing_metadata-0.1.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 18:50:02.000000 ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-30 18:50:00.000000 ndx_dynamic_routing_metadata-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.402775 ndx_dynamic_routing_metadata-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:50:02.406775 ndx_dynamic_routing_metadata-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 18:49:39.000000 ndx_dynamic_routing_metadata-0.1.2/tests/test_core.py
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/LICENSE` & `ndx_dynamic_routing_metadata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.1/LICENSE.txt` & `ndx_dynamic_routing_metadata-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.1/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/README.md` & `ndx_dynamic_routing_metadata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.1/pyproject.toml` & `ndx_dynamic_routing_metadata-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "nwb-extension",
     "ndx-extension",
 ]
 dependencies = [
     "pynwb>=2.6.0",
     "hdmf>=3.13.0",
 ]
-version = "0.1.1"
+version = "0.1.2"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
@@ -45,14 +45,16 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = [
     "src",
+    "src/ndx_dynamic_routing_metadata/spec/ndx-dynamic-routing-metadata.extensions.yaml",
+    "src/ndx_dynamic_routing_metadata/spec/ndx-dynamic-routing-metadata.namespace.yaml",
 ]
 
 [tool.setuptools.package-data]
 ndx_dynamic_routing_metadata = [
     "py.typed",
 ]
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/__init__.py` & `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Type to store metadata for dynamic routing experiments at Allen Institute
 """
 
 import doctest
 import importlib.metadata
 import logging
 
-from ndx_dynamic_routing_metadata.pynwb.ndx_dynamic_routing_metadata import *
+from ndx_dynamic_routing_metadata.pynwb import *
 from ndx_dynamic_routing_metadata.spec import *
 
 # import functions from submodules here:
 # from ndx_dynamic_routing_metadata.utils import *
 
 logger = logging.getLogger(__name__)
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/ndx_dynamic_routing_metadata/__init__.py` & `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/pynwb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,19 @@
 except ImportError:
     # TODO: Remove when python 3.9 becomes the new minimum
     from importlib_resources import files
 
 # Get path to the namespace.yaml file with the expected location when installed not in editable mode
 __location_of_this_file = files(__name__)
 __spec_path = (
-    __location_of_this_file.parent.parent
+    __location_of_this_file.parent
     / "spec"
     / "ndx-dynamic-routing-metadata.namespace.yaml"
 )
 
-# If that path does not exist, we are likely running in editable mode. Use the local path instead
-if not os.path.exists(__spec_path):
-    __spec_path = (
-        __location_of_this_file.parent.parent.parent.parent
-        / "spec"
-        / "ndx-dynamic-routing-metadata.namespace.yaml"
-    )
-
 # Load the namespace
 load_namespaces(str(__spec_path))
 
 # TODO: Define your classes here to make them accessible at the package level.
 # Either have PyNWB generate a class from the spec using `get_class` as shown
 # below or write a custom class and register it using the class decorator
 # `@register_class("TetrodeSeries", "ndx-dynamic-routing-metadata")`
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/pynwb/tests/test_dynamic_routing_metadata.py` & `ndx_dynamic_routing_metadata-0.1.2/tests/test_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-"""Unit and integration tests for the DynamicRoutingMetadata extension neurodata type.
-
-TODO: Modify these tests to test your extension neurodata type.
-"""
+import ndx_dynamic_routing_metadata
 
 import os
 import unittest
 from datetime import datetime
-
 from pynwb import NWBHDF5IO, NWBFile
-
 from ndx_dynamic_routing_metadata import DynamicRoutingMetadataExtension
 
 
+def test_import_package():
+    pass
+
+"""Unit and integration tests for the DynamicRoutingMetadata extension neurodata type.
+
+TODO: Modify these tests to test your extension neurodata type.
+"""
+
 class DynamicRoutingMetaDataExtensionTest(unittest.TestCase):
     def setUp(self):
-        self.nwbfile = NWBFile("description", "id", datetime.now().astimezone())
+        self.nwbfile = NWBFile('description', 'id', datetime.now().astimezone())
 
     def test_add_lab_metadata(self):
         # Creates LabMetaData container
         self.setUp()
 
         lab_metadata_dict = dict(
-            name="DynamicRoutingMetadata",  # name of key in nwb
+            name='DynamicRoutingMetadata', # name of key in nwb 
             is_sync=True,
             is_ephys=True,
             is_task=True,
         )
 
         lab_metadata = DynamicRoutingMetadataExtension(**lab_metadata_dict)
 
         # Add to file
         self.nwbfile.add_lab_meta_data(lab_metadata)
 
-        filename = "test_labmetadata.nwb"
+        filename = 'test_labmetadata.nwb'
 
-        with NWBHDF5IO(filename, "w") as io:
+        with NWBHDF5IO(filename, 'w') as io:
             io.write(self.nwbfile)
 
-        with NWBHDF5IO(filename, mode="r", load_namespaces=True) as io:
+        with NWBHDF5IO(filename, mode='r', load_namespaces=True) as io:
             nwbfile = io.read()
 
             for metadata_key, metadata_value in lab_metadata_dict.items():
-                self.assertEqual(
-                    metadata_value,
-                    getattr(
-                        nwbfile.lab_meta_data["DynamicRoutingMetadata"], metadata_key
-                    ),
-                )
+                self.assertEqual(metadata_value, getattr(nwbfile.lab_meta_data['DynamicRoutingMetadata'], metadata_key))
 
         os.remove(filename)
 
-
-if __name__ == "__main__":
-    test = DynamicRoutingMetaDataExtensionTest()
-    test.test_add_lab_metadata()
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py` & `ndx_dynamic_routing_metadata-0.1.2/src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py`

 * *Files identical despite different names*

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/PKG-INFO` & `ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndx-dynamic-routing-metadata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Type to store metadata for dynamic routing experiments at Allen Institute
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>, Arjun Sridhar <arjun.sridhar@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/ndx-dynamic-routing-metadata/issues
 Keywords: NeurodataWithoutBorders,NWB,nwb-extension,ndx-extension
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ndx_dynamic_routing_metadata-0.1.1/src/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt` & `ndx_dynamic_routing_metadata-0.1.2/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 LICENSE
 LICENSE.txt
 README.md
 pyproject.toml
+ndx_dynamic_routing_metadata.egg-info/PKG-INFO
+ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
+ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
+ndx_dynamic_routing_metadata.egg-info/entry_points.txt
+ndx_dynamic_routing_metadata.egg-info/requires.txt
+ndx_dynamic_routing_metadata.egg-info/top_level.txt
 src/ndx_dynamic_routing_metadata/__init__.py
 src/ndx_dynamic_routing_metadata/py.typed
-src/ndx_dynamic_routing_metadata.egg-info/PKG-INFO
-src/ndx_dynamic_routing_metadata.egg-info/SOURCES.txt
-src/ndx_dynamic_routing_metadata.egg-info/dependency_links.txt
-src/ndx_dynamic_routing_metadata.egg-info/entry_points.txt
-src/ndx_dynamic_routing_metadata.egg-info/requires.txt
-src/ndx_dynamic_routing_metadata.egg-info/top_level.txt
-src/ndx_dynamic_routing_metadata/pynwb/ndx_dynamic_routing_metadata/__init__.py
-src/ndx_dynamic_routing_metadata/pynwb/tests/__init__.py
-src/ndx_dynamic_routing_metadata/pynwb/tests/test_dynamic_routing_metadata.py
+src/ndx_dynamic_routing_metadata/pynwb/__init__.py
 src/ndx_dynamic_routing_metadata/spec/create_extension_spec.py
 tests/test_core.py
```

