# Comparing `tmp/antidupe-0.0.2.tar.gz` & `tmp/antidupe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.2.tar", last modified: Wed May  1 15:32:34 2024, max compression
+gzip compressed data, was "antidupe-0.0.3.tar", last modified: Wed May  1 16:56:49 2024, max compression
```

## Comparing `antidupe-0.0.2.tar` & `antidupe-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.514468 antidupe-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 15:32:28.000000 antidupe-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 15:32:34.514468 antidupe-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 15:32:28.000000 antidupe-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.510468 antidupe-0.0.2/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-01 15:32:28.000000 antidupe-0.0.2/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:32:34.514468 antidupe-0.0.2/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 15:32:34.000000 antidupe-0.0.2/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:32:34.514468 antidupe-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 15:32:28.000000 antidupe-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.349142 antidupe-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 16:56:45.000000 antidupe-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 16:56:49.345142 antidupe-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 16:56:45.000000 antidupe-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.345142 antidupe-0.0.3/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.345142 antidupe-0.0.3/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:56:49.349142 antidupe-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 16:56:45.000000 antidupe-0.0.3/setup.py
```

### Comparing `antidupe-0.0.2/LICENSE` & `antidupe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.2/PKG-INFO` & `antidupe-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.2/README.md` & `antidupe-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.2/antidupe/main.py` & `antidupe-0.0.3/antidupe/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 }
 
 
 class Antidupe:
     """
     Discover duplicate images.
     """
-    def __init__(self, limits: dict = DEFAULTS, device: str = 'cpu', debug: bool = False):  # noqa
+    def __init__(self, limits: dict = DEFAULTS, device: str = 'cpu', debug: bool = False, show_plots: bool = False):  # noqa
+        self.show_plots = show_plots
         self.device = device
         self.limits = limits
         self.debug = debug
         self.cnn = CNN(device=device)
 
     def d_print(self, *args, **kwargs):
         """
@@ -58,15 +59,15 @@
     def predict(self, images: [list, tuple], size: int = 512) -> bool:
         """
         Lets measure our images.
         """
         switch = False
         if self.device != 'cpu':
             switch = True
-        im_1, im_2 = resize_image(*images, size, show=self.debug)
+        im_1, im_2 = resize_image(*images, size, show=self.show_plots)
         ed = euclidean_distance(im_1, im_2)
         self.d_print(f'euclidean distance detected: {ed}')
         if ed == 0.0:
             self.d_print('euclidean distance found duplicate')
             return True
         else:
             ih = image_hash(im_1, im_2)
```

### Comparing `antidupe-0.0.2/antidupe/utilities.py` & `antidupe-0.0.3/antidupe/utilities.py`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.2/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.3/antidupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.2/setup.py` & `antidupe-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

