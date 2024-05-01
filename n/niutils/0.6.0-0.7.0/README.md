# Comparing `tmp/niutils-0.6.0.tar.gz` & `tmp/niutils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/niutils-0.6.0.tar", last modified: Mon Mar 20 15:20:27 2023, max compression
+gzip compressed data, was "dist/niutils-0.7.0.tar", last modified: Wed May  1 09:18:52 2024, max compression
```

## Comparing `niutils-0.6.0.tar` & `niutils-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:27.000000 niutils-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1346 2023-03-20 15:20:18.000000 niutils-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2361 2023-03-20 15:20:27.000000 niutils-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1538 2023-03-20 15:20:27.000000 niutils-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      374 2023-03-20 15:20:18.000000 niutils-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:27.000000 niutils-0.6.0/niutils/
--rw-r--r--   0 runner    (1001) docker     (116)      497 2023-03-20 15:20:27.000000 niutils-0.6.0/niutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    15666 2023-03-20 15:20:18.000000 niutils-0.6.0/niutils/niutils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:27.000000 niutils-0.6.0/niutils/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:18.000000 niutils-0.6.0/niutils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      123 2023-03-20 15:20:18.000000 niutils-0.6.0/niutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:27.000000 niutils-0.6.0/niutils/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:18.000000 niutils-0.6.0/niutils/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 15:20:27.000000 niutils-0.6.0/niutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2361 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      249 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       51 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      355 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-20 15:20:26.000000 niutils-0.6.0/niutils.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:52.000000 niutils-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:38.000000 niutils-0.7.0/niutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 09:18:38.000000 niutils-0.7.0/niutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:38.000000 niutils-0.7.0/niutils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-05-01 09:18:38.000000 niutils-0.7.0/niutils/niutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-01 09:18:38.000000 niutils-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 09:18:52.000000 niutils-0.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-01 09:18:52.000000 niutils-0.7.0/niutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-01 09:18:52.000000 niutils-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-01 09:18:38.000000 niutils-0.7.0/setup.py
```

### Comparing `niutils-0.6.0/README.md` & `niutils-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `niutils-0.6.0/PKG-INFO` & `niutils-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niutils
-Version: 0.6.0
+Version: 0.7.0
 Summary: Various utilities to fast-track some boring python coding.
 Home-page: https://github.com/smoia/niutils
 Author: niutils developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/smoia/niutils
@@ -47,7 +47,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Provides: niutils
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: style
+Provides-Extra: dev
+Provides-Extra: clustering
```

### Comparing `niutils-0.6.0/setup.cfg` & `niutils-0.7.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -29,23 +29,29 @@
 	pytest >=3.6
 test_suite = pytest
 zip_safe = False
 packages = find:
 include_package_data = True
 
 [options.extras_require]
+clustering = 
+	scipy
+	scikit-learn
+	scikit-image
 style = 
 	flake8 >=3.7
 	flake8-docstrings >=1.5
 test = 
 	pytest >=5.3
 	pytest-cov
 	%(style)s
 all = 
-	%(style)s
+	%(clustering)s
+dev = 
+	%(all)s
 	%(test)s
 
 [options.entry_points]
 console_scripts = 
 	niutils=niutils.niutils:_main
 
 [flake8]
```

### Comparing `niutils-0.6.0/niutils/niutils.py` & `niutils-0.7.0/niutils/niutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 import os
 from copy import deepcopy
 from itertools import tee
 
 import matplotlib.pyplot as plt
 import nibabel as nib
 import numpy as np
-from scipy.optimize import linear_sum_assignment
-from scipy.stats import zscore
-from sklearn.metrics import confusion_matrix
 
 
 SUB_LIST = ['001', '002', '003', '004', '007', '008', '009']
 LAST_SES = 10  # 10
 
 KCLUSLIST = [f"{i:02d}" for i in list(range(2, 51))]
 
@@ -175,15 +172,15 @@
     Unmask 1D or 2D into an nD based on shape or asdata
     """
     if asdata is not None:
         if shape is not None:
             print('Both shape and asdata were defined. '
                   f'Overwriting shape {shape} with asdata {asdata.shape}')
         shape = asdata.shape
-    elif shape == '':
+    elif shape == '' or shape is None:
         raise ValueError('Both shape and asdata are empty. '
                          'Must specify at least one')
 
     if data.shape[0] != mask.sum():
         raise ValueError('Cannot unmask data with first dimension '
                          f'{data.shape[0]} using mask with shape '
                          f'{mask.shape} ({np.prod(mask.shape)} entries)')
@@ -243,14 +240,17 @@
     if return_pca:
         return clus+1, pca
     else:
         return clus+1
 
 
 def relabel(prefix, kclus=KCLUSLIST, offset=9000):
+    from scipy.optimize import linear_sum_assignment
+    from sklearn.metrics import confusion_matrix
+
     # Prepare data
     # kclus = [f"{i:02d}" for i in list(kclus)]
 
     data = {}
     data2d = {}
     hungdist = np.zeros(len(kclus)-1)
```

### Comparing `niutils-0.6.0/niutils.egg-info/PKG-INFO` & `niutils-0.7.0/niutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niutils
-Version: 0.6.0
+Version: 0.7.0
 Summary: Various utilities to fast-track some boring python coding.
 Home-page: https://github.com/smoia/niutils
 Author: niutils developers
 Maintainer: Stefano Moia
 Maintainer-email: s.moia@bcbl.eu
 License: Apache-2.0
 Download-URL: https://github.com/smoia/niutils
@@ -47,7 +47,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Provides: niutils
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: style
+Provides-Extra: dev
+Provides-Extra: clustering
```

