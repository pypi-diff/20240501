# Comparing `tmp/seamm_widgets-2022.7.29.tar.gz` & `tmp/seamm_widgets-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_widgets-2022.7.29.tar", last modified: Fri Jul 29 18:44:28 2022, max compression
+gzip compressed data, was "seamm_widgets-2024.5.1.tar", last modified: Wed May  1 09:27:43 2024, max compression
```

## Comparing `seamm_widgets-2022.7.29.tar` & `seamm_widgets-2024.5.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.683380 seamm_widgets-2022.7.29/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6790 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8728 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6473 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/seamm_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/seamm_widgets/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    31375 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/check_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/seamm_widgets/data/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/data/checked.png
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/data/mixed.png
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/data/unchecked.png
--rw-r--r--   0 runner    (1001) docker     (121)    26835 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/html_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    20685 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/labeled_combobox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/labeled_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5576 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/labeled_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/mousewheel_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     9845 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    12760 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/property_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     6615 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/scrolled_columns.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/scrolled_frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/scrolled_labelframe.py
--rw-r--r--   0 runner    (1001) docker     (121)    18602 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/search_criteria.py
--rw-r--r--   0 runner    (1001) docker     (121)     5731 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/unit_combobox.py
--rw-r--r--   0 runner    (1001) docker     (121)     5562 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/seamm_widgets/unit_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/seamm_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-07-29 18:44:28.000000 seamm_widgets-2022.7.29/seamm_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-07-29 18:44:28.000000 seamm_widgets-2022.7.29/seamm_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 18:44:28.000000 seamm_widgets-2022.7.29/seamm_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-29 18:44:28.000000 seamm_widgets-2022.7.29/seamm_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-29 18:44:28.000000 seamm_widgets-2022.7.29/seamm_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 18:44:28.687380 seamm_widgets-2022.7.29/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/tests/test_seamm_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-07-29 18:44:18.000000 seamm_widgets-2022.7.29/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.765854 seamm_widgets-2024.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8728 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/seamm_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/seamm_widgets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31375 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/check_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/seamm_widgets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/data/checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/data/mixed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/data/unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26824 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/html_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/labeled_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/labeled_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/labeled_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/mousewheel_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/property_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/scrolled_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/scrolled_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/scrolled_labelframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/search_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/unit_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/seamm_widgets/unit_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/seamm_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-01 09:27:43.000000 seamm_widgets-2024.5.1/seamm_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-01 09:27:43.000000 seamm_widgets-2024.5.1/seamm_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:27:43.000000 seamm_widgets-2024.5.1/seamm_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 09:27:43.000000 seamm_widgets-2024.5.1/seamm_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 09:27:43.000000 seamm_widgets-2024.5.1/seamm_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:27:43.769853 seamm_widgets-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/tests/test_seamm_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-01 09:27:24.000000 seamm_widgets-2024.5.1/versioneer.py
```

### Comparing `seamm_widgets-2022.7.29/CONTRIBUTING.rst` & `seamm_widgets-2024.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/LICENSE` & `seamm_widgets-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/PKG-INFO` & `seamm_widgets-2024.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_widgets
-Version: 2022.7.29
+Version: 2024.5.1
 Summary: seamm_widgets
 Home-page: https://github.com/molssi-seam/seamm_widgets
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_widgets
 Platform: Linux
@@ -16,14 +16,17 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: pillow
+Requires-Dist: Pmw
+Requires-Dist: seamm-util
 
 =============
 SEAMM Widgets
 =============
 
 
 .. image:: https://img.shields.io/travis/molssi-seamm/seamm_widgets.svg
@@ -79,11 +82,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-0.1.0 (2019-04-02)
-------------------
+2024.5.1 -- Enhancement to ScrolledColumns
+    * Added optional separator columns for dividing sections of the table.
+      
+2022.10.28 -- Bugfix: problem deleting 2 or more keywords
+  There was a crash if you deleted a second keyword in the Keywords tab of
+  calculation.
 
-* First release on PyPI.
+0.1.0 (2019-04-02)
+  * First release on PyPI.
```

### Comparing `seamm_widgets-2022.7.29/README.rst` & `seamm_widgets-2024.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/docs/Makefile` & `seamm_widgets-2024.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/docs/conf.py` & `seamm_widgets-2024.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/docs/index.rst` & `seamm_widgets-2024.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/docs/installation.rst` & `seamm_widgets-2024.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/docs/make.bat` & `seamm_widgets-2024.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/check_tree.py` & `seamm_widgets-2024.5.1/seamm_widgets/check_tree.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/data/mixed.png` & `seamm_widgets-2024.5.1/seamm_widgets/data/mixed.png`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/data/unchecked.png` & `seamm_widgets-2024.5.1/seamm_widgets/data/unchecked.png`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/html_widgets.py` & `seamm_widgets-2024.5.1/seamm_widgets/html_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,15 @@
                 setattr(self, m, getattr(self.frame, m))
 
     def __str__(self):
         return str(self.frame)
 
 
 class HTMLScrolledText(_ScrolledText):
-
-    """
-    HTML scrolled text widget
-    """
+    """HTML scrolled text widget"""
 
     def __init__(self, *args, html=None, **kwargs):
         super().__init__(*args, **kwargs)
         self._w_init(kwargs)
         self.html_parser = HTMLTextParser()
         if isinstance(html, str):
             self.set_html(html)
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/keywords.py` & `seamm_widgets-2024.5.1/seamm_widgets/keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,25 +159,42 @@
             row += 1
             keyword = d["keyword"]
             if "widgets" not in d:
                 widgets = d["widgets"] = {}
             else:
                 widgets = d["widgets"]
 
-            if "remove" not in widgets:
-                # The button to remove a row...
+            # The button to remove a row...
+            if "remove" in widgets:
+                widgets["remove"].configure(
+                    command=lambda row=row: self.remove_keyword(row)
+                )
+            else:
                 widgets["remove"] = ttk.Button(
                     frame,
                     text="-",
                     width=2,
                     command=lambda row=row: self.remove_keyword(row),
                     takefocus=True,
                 )
 
-            if "entry" not in widgets:
+            if "entry" in widgets:
+                widgets["entry"].configure(
+                    validatecommand=(
+                        self.keyword_cb,
+                        keyword,
+                        row,
+                        "%W",
+                        "%P",
+                        "%s",
+                        "%d",
+                        "%S",
+                    )
+                )
+            else:
                 # the name of the keyword
                 widgets["entry"] = ttk.Entry(
                     frame,
                     width=self._max_width,
                     validate="key",
                     validatecommand=(
                         self.keyword_cb,
@@ -188,19 +205,19 @@
                         "%s",
                         "%d",
                         "%S",
                     ),
                     takefocus=True,
                     style="Red.TEntry",
                 )
-                widgets["entry"].bind(
-                    "<KeyPress-Tab>",
-                    lambda event=None, row=row: self.handle_tab(event, row),
-                )
                 widgets["entry"].insert("end", keyword)
+            widgets["entry"].bind(
+                "<KeyPress-Tab>",
+                lambda event=None, row=row: self.handle_tab(event, row),
+            )
 
             self.logger.debug("  widgets: " + str(widgets))
             widgets["remove"].grid(row=row, column=0, sticky=tk.W)
             col = 1
             widgets["entry"].grid(row=row, column=col, stick=tk.EW)
             col += 1
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/labeled_combobox.py` & `seamm_widgets-2024.5.1/seamm_widgets/labeled_combobox.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/labeled_entry.py` & `seamm_widgets-2024.5.1/seamm_widgets/labeled_entry.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/labeled_widget.py` & `seamm_widgets-2024.5.1/seamm_widgets/labeled_widget.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/mousewheel_support.py` & `seamm_widgets-2024.5.1/seamm_widgets/mousewheel_support.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/periodic_table.py` & `seamm_widgets-2024.5.1/seamm_widgets/periodic_table.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/property_table.py` & `seamm_widgets-2024.5.1/seamm_widgets/property_table.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/scrolled_columns.py` & `seamm_widgets-2024.5.1/seamm_widgets/scrolled_columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
         # list (vector) of the header widgets, _ncolumns long
         self._header_widgets = []
 
         # list of lists (row x column) of widgets in the table
         self._widgets = []
 
+        # Columns that are separators
+        self._column_separators = set()
+
         # Create the two subframes, linking them both to the
         # horizontal scrollbar at the bottom
         # self.headers = ttk.Frame(self)
         self.table = sw.ScrolledFrame(
             self, scroll_vertically=True, borderwidth=2, relief=tk.SUNKEN
         )
         self.headers = sw.ScrolledFrame(
@@ -52,14 +55,16 @@
         self.rowconfigure(1, weight=1)
 
         # Put in the column titles if given
         col = 0
         header = self.headers.interior()
         for item in columns:
             if isinstance(item, str):
+                if item == "|":
+                    self._column_separators.add(col)
                 item = ttk.Label(header, text=item)
             item.grid(row=0, column=col)
             col += 1
             self._header_widgets.append(item)
 
     def cell(self, row, column, value=None):
         """Return or set the widget at the given cell"""
@@ -74,16 +79,23 @@
                 # pad the header and each row with None's
                 extra = [None] * (column - self.ncolumns + 1)
                 self._header_widgets.extend(extra)
                 for row_of_widgets in self._widgets:
                     row_of_widgets.extend(extra)
             if row >= self.nrows:
                 # add rows 'till we get there
-                extra = [None] * self.ncolumns
                 for i in range(self.nrows, row + 1):
+                    extra = []
+                    for col in range(self.ncolumns):
+                        if col in self._column_separators:
+                            tmp = ttk.Label(self.table.interior(), text="|")
+                            tmp.grid(row=i, column=col)
+                            extra.append(tmp)
+                        else:
+                            extra.append(None)
                     self._widgets.append(extra)
 
             if isinstance(value, str):
                 value = ttk.Label(self.table.interior(), text=value)
 
             value.grid(row=row, column=column)
             self._widgets[row][column] = value
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/scrolled_frame.py` & `seamm_widgets-2024.5.1/seamm_widgets/scrolled_frame.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/scrolled_labelframe.py` & `seamm_widgets-2024.5.1/seamm_widgets/scrolled_labelframe.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/search_criteria.py` & `seamm_widgets-2024.5.1/seamm_widgets/search_criteria.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/unit_combobox.py` & `seamm_widgets-2024.5.1/seamm_widgets/unit_combobox.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 The goal of these widgets is twofold: to make it easier for developers
 to implement dialogs with compound widgets, and to naturally
 standardize the user interface presented to the user.
 """
 
 import logging
-from seamm_util import Q_, units_class
+from seamm_util import Q_, units_class, default_units
 import seamm_widgets as sw
 import tkinter as tk
 import tkinter.ttk as ttk
 
 logger = logging.getLogger(__name__)
 
 options = {
@@ -102,15 +102,15 @@
                     if unit != "":
                         if Q_(unit).dimensionality != dimensionality:
                             self.units.configure(values=[])
                             current_units = []
                             break
 
             if len(current_units) == 0:
-                self.set_units([*sw.default_units[str(dimensionality)], ""])
+                self.set_units([*default_units(str(dimensionality)), ""])
                 self.units.set("{0.units:~}".format(value).replace(" ", ""))
         elif unit_string is not None:
             self.combobox.set(value)
 
             dimensionality = Q_(unit_string).dimensionality
             current_units = self.units.cget("values")
             if len(current_units) > 0:
@@ -118,15 +118,15 @@
                     if unit != "":
                         if Q_(unit).dimensionality != dimensionality:
                             self.units.configure(values=[])
                             current_units = []
                             break
 
             if len(current_units) == 0:
-                self.set_units([*sw.default_units[str(dimensionality)], ""])
+                self.set_units([*default_units(str(dimensionality)), ""])
                 self.units.set(unit_string)
         else:
             self.combobox.set(value)
             self.set_units("all")
             self.units.set("")
 
     def get(self):
@@ -146,20 +146,17 @@
                     return (value, unit)
             else:
                 return (value, unit)
 
     def set_units(self, values=None):
         if values is None:
             dimensionality = str(self.get().dimensionality)
-            self.units.config(values=sw.default_units[dimensionality])
+            self.units.config(values=[*default_units(dimensionality), ""])
         elif values == "all":
-            tmp = [""]
-            for key in sw.default_units:
-                tmp += sw.default_units[key]
-            self.units.config(values=tmp)
+            self.units.config(values=[*default_units("all"), ""])
         else:
             self.units.config(values=values)
 
     def config(self, **kwargs):
         """Set the configuration of the megawidget"""
         unitcombobox = options["unitcombobox"]
         units = options["units"]
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets/unit_entry.py` & `seamm_widgets-2024.5.1/seamm_widgets/unit_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 The goal of these widgets is twofold: to make it easier for developers
 to implement dialogs with compound widgets, and to naturally
 standardize the user interface presented to the user.
 """
 
 import logging
-from seamm_util import Q_, units_class
+from seamm_util import Q_, units_class, default_units
 import seamm_widgets as sw
 import tkinter as tk
 import tkinter.ttk as ttk
 
 logger = logging.getLogger(__name__)
 
 options = {
@@ -102,30 +102,30 @@
                 for unit in current_units:
                     if Q_(unit).dimensionality != dimensionality:
                         self.units.configure(values=[])
                         current_units = []
                         break
 
             if len(current_units) == 0:
-                self.set_units([*sw.default_units[str(dimensionality)], ""])
+                self.set_units([*default_units(str(dimensionality)), ""])
                 self.units.set("{0.units:~}".format(value).replace(" ", ""))
         elif unit_string:
             self.entry.insert(0, value)
 
             dimensionality = Q_(unit_string).dimensionality
             current_units = self.units.cget("values")
             if len(current_units) > 0:
                 for unit in current_units:
                     if unit != "" and Q_(unit).dimensionality != dimensionality:
                         self.units.configure(values=[])
                         current_units = []
                         break
 
             if len(current_units) == 0:
-                self.set_units([*sw.default_units[str(dimensionality)], ""])
+                self.set_units([*default_units(str(dimensionality)), ""])
                 self.units.set(unit_string)
         else:
             self.entry.insert(0, value)
             self.set_units("all")
             self.units.set("")
 
     def get(self):
@@ -143,20 +143,17 @@
         else:
             return (value, unit)
 
     def set_units(self, values=None):
         # logger.debug('set_units: ' + str(values))
         if values is None:
             dimensionality = str(self.get().dimensionality)
-            self.units.config(values=sw.default_units[dimensionality])
+            self.units.config(values=[*default_units(dimensionality), ""])
         elif values == "all":
-            tmp = [""]
-            for key in sw.default_units:
-                tmp += sw.default_units[key]
-            self.units.config(values=tmp)
+            self.units.config(values=[*default_units("all"), ""])
         else:
             self.units.config(values=values)
 
     def config(self, **kwargs):
         """Set the configuration of the megawidget"""
         unitentry = options["unitentry"]
         units = options["units"]
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets.egg-info/PKG-INFO` & `seamm_widgets-2024.5.1/seamm_widgets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seamm-widgets
-Version: 2022.7.29
+Name: seamm_widgets
+Version: 2024.5.1
 Summary: seamm_widgets
 Home-page: https://github.com/molssi-seam/seamm_widgets
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: seamm_widgets
 Platform: Linux
@@ -16,14 +16,17 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: pillow
+Requires-Dist: Pmw
+Requires-Dist: seamm-util
 
 =============
 SEAMM Widgets
 =============
 
 
 .. image:: https://img.shields.io/travis/molssi-seamm/seamm_widgets.svg
@@ -79,11 +82,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-0.1.0 (2019-04-02)
-------------------
+2024.5.1 -- Enhancement to ScrolledColumns
+    * Added optional separator columns for dividing sections of the table.
+      
+2022.10.28 -- Bugfix: problem deleting 2 or more keywords
+  There was a crash if you deleted a second keyword in the Keywords tab of
+  calculation.
 
-* First release on PyPI.
+0.1.0 (2019-04-02)
+  * First release on PyPI.
```

### Comparing `seamm_widgets-2022.7.29/seamm_widgets.egg-info/SOURCES.txt` & `seamm_widgets-2024.5.1/seamm_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/setup.py` & `seamm_widgets-2024.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/tests/test_seamm_widgets.py` & `seamm_widgets-2024.5.1/tests/test_seamm_widgets.py`

 * *Files identical despite different names*

### Comparing `seamm_widgets-2022.7.29/versioneer.py` & `seamm_widgets-2024.5.1/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,17 +335,17 @@
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
     cfg = VersioneerConfig()
```

