# Comparing `tmp/xarray_treeview-1.2.0.tar.gz` & `tmp/xarray_treeview-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_treeview-1.2.0.tar", last modified: Tue Apr 30 21:47:09 2024, max compression
+gzip compressed data, was "xarray_treeview-1.2.1.tar", last modified: Tue Apr 30 22:56:15 2024, max compression
```

## Comparing `xarray_treeview-1.2.0.tar` & `xarray_treeview-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.0/LICENSE
--rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.0/README.md
--rw-r--r--   0        0        0     1256 2024-04-30 21:47:09.910923 xarray_treeview-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7671 2024-04-24 22:17:08.019833 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeItem.py
--rw-r--r--   0        0        0     5999 2024-03-08 22:47:30.993487 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeModel.py
--rw-r--r--   0        0        0    10664 2024-04-26 15:47:20.923676 xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeView.py
--rw-r--r--   0        0        0      195 2024-02-08 22:49:32.523681 xarray_treeview-1.2.0/src/xarray_treeview/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 xarray_treeview-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.1/LICENSE
+-rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.1/README.md
+-rw-r--r--   0        0        0     1261 2024-04-30 22:56:15.940983 xarray_treeview-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7671 2024-04-24 22:17:08.019833 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeItem.py
+-rw-r--r--   0        0        0     5999 2024-03-08 22:47:30.993487 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeModel.py
+-rw-r--r--   0        0        0    10664 2024-04-26 15:47:20.923676 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeView.py
+-rw-r--r--   0        0        0      195 2024-02-08 22:49:32.523681 xarray_treeview-1.2.1/src/xarray_treeview/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 xarray_treeview-1.2.1/PKG-INFO
```

### Comparing `xarray_treeview-1.2.0/LICENSE` & `xarray_treeview-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.0/pyproject.toml` & `xarray_treeview-1.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 authors = [
     { name = "Marcel Goldschen-Ohm", email = "goldschen-ohm@utexas.edu" },
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy>=1.26.2",
     "xarray>=2023.12.0",
-    "xarray-tree>=0.1.0",
     "qtpy>=2.4.1",
     "qtawesome>=1.3.0",
     "pyqt-ext>=1.1.0",
+    "xarray-datatree>=0.0.14",
 ]
 readme = "README.md"
 keywords = [
     "PyQt",
     "PySide",
     "xarray",
     "tree",
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.0"
+version = "1.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
```

### Comparing `xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeItem.py` & `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeItem.py`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeModel.py` & `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeModel.py`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.0/src/xarray_treeview/XarrayTreeView.py` & `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeView.py`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.0/PKG-INFO` & `xarray_treeview-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-treeview
-Version: 1.2.0
+Version: 1.2.1
 Summary: PyQt/PySide model/view for tree of Xarray datasets.
 Keywords: PyQt,PySide,xarray,tree
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-treeview
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Project-URL: Homepage, https://github.com/marcel-goldschen-ohm/xarray-treeview
 Project-URL: Repository, https://github.com/marcel-goldschen-ohm/xarray-treeview
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: xarray>=2023.12.0
-Requires-Dist: xarray-tree>=0.1.0
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: qtawesome>=1.3.0
 Requires-Dist: pyqt-ext>=1.1.0
+Requires-Dist: xarray-datatree>=0.0.14
 Description-Content-Type: text/markdown
 
 # xarray-treeview
 PyQt/PySide model/view for tree of Xarray datasets.
 
 :construction:
```

