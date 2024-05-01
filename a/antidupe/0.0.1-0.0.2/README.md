# Comparing `tmp/antidupe-0.0.1.tar.gz` & `tmp/antidupe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.1.tar", last modified: Tue Apr 30 21:59:18 2024, max compression
+gzip compressed data, was "antidupe-0.0.2.tar", last modified: Wed May  1 15:32:34 2024, max compression
```

## Comparing `antidupe-0.0.1.tar` & `antidupe-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:59:18.507625 antidupe-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 21:59:14.000000 antidupe-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-30 21:59:18.507625 antidupe-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 21:59:14.000000 antidupe-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:59:18.503625 antidupe-0.0.1/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 21:59:14.000000 antidupe-0.0.1/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-30 21:59:14.000000 antidupe-0.0.1/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-30 21:59:14.000000 antidupe-0.0.1/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:59:18.507625 antidupe-0.0.1/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-30 21:59:18.000000 antidupe-0.0.1/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 21:59:18.000000 antidupe-0.0.1/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:59:18.000000 antidupe-0.0.1/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 21:59:18.000000 antidupe-0.0.1/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 21:59:18.000000 antidupe-0.0.1/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:59:18.507625 antidupe-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-30 21:59:14.000000 antidupe-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.514468 antidupe-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 15:32:28.000000 antidupe-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 15:32:34.514468 antidupe-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 15:32:28.000000 antidupe-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.510468 antidupe-0.0.2/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.514468 antidupe-0.0.2/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:32:34.514468 antidupe-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 15:32:28.000000 antidupe-0.0.2/setup.py
```

### Comparing `antidupe-0.0.1/LICENSE` & `antidupe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.1/PKG-INFO` & `antidupe-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: SSIM-PIL
 Requires-Dist: matplotlib
 Requires-Dist: imagehash
 Requires-Dist: efficientnet_pytorch
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
```

### Comparing `antidupe-0.0.1/README.md` & `antidupe-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.1/antidupe/main.py` & `antidupe-0.0.2/antidupe/main.py`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.1/antidupe/utilities.py` & `antidupe-0.0.2/antidupe/utilities.py`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.1/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.2/antidupe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: SSIM-PIL
 Requires-Dist: matplotlib
 Requires-Dist: imagehash
 Requires-Dist: efficientnet_pytorch
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
```

### Comparing `antidupe-0.0.1/setup.py` & `antidupe-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     from install_preserve import preserve
 except ImportError:
     import pip  # noqa
     pip.main(['install', 'install-preserve'])
     from install_preserve import preserve  # noqa
 
 install_requires = [
+    'SSIM-PIL',
     'matplotlib',
     'imagehash',
     'efficientnet_pytorch',
     'numpy',
     'Pillow',
     'torch>=2.0.0',
     'torchvision>=0.17.0',
@@ -26,15 +27,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

