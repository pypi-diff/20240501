# Comparing `tmp/antidupe-0.0.3.tar.gz` & `tmp/antidupe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.3.tar", last modified: Wed May  1 16:56:49 2024, max compression
+gzip compressed data, was "antidupe-0.0.4.tar", last modified: Wed May  1 17:53:06 2024, max compression
```

## Comparing `antidupe-0.0.3.tar` & `antidupe-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.349142 antidupe-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 16:56:45.000000 antidupe-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 16:56:49.345142 antidupe-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 16:56:45.000000 antidupe-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.345142 antidupe-0.0.3/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-01 16:56:45.000000 antidupe-0.0.3/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:56:49.345142 antidupe-0.0.3/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 16:56:49.000000 antidupe-0.0.3/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:56:49.349142 antidupe-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 16:56:45.000000 antidupe-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.671077 antidupe-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:52:59.000000 antidupe-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 17:53:06.671077 antidupe-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 17:52:59.000000 antidupe-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.667077 antidupe-0.0.4/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-01 17:52:59.000000 antidupe-0.0.4/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:53:06.671077 antidupe-0.0.4/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 17:53:06.000000 antidupe-0.0.4/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:53:06.671077 antidupe-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-01 17:52:59.000000 antidupe-0.0.4/setup.py
```

### Comparing `antidupe-0.0.3/LICENSE` & `antidupe-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.3/PKG-INFO` & `antidupe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.3/README.md` & `antidupe-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.3/antidupe/main.py` & `antidupe-0.0.4/antidupe/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,23 @@
         return False
 
     def test(self, images: [list, tuple, None] = None):
         """
         Tests the prediction logic.
         """
         self.debug = True
+        self.show_plots = True
         if not images:
             im_1 = Image.open('images/unique_1.jpg')
             im_2 = Image.open('images/Bead_necklace_1.jpg')
             im_3 = Image.open('images/Bead_necklace_2.jpg')
         else:
             im_1, im_2, im_3 = images
         line = '------'
         print('testing unique')
         print(f"{line}duplicate? {self.predict((im_1, im_2))}")
         print('testing duplicates resized')
         print(f"{line}duplicate? {self.predict((im_2, im_3))}")
         print('testing identical duplicates')
         print(f"{line}duplicate? {self.predict((im_2, im_2))}")
         self.debug = False
+        self.show_plots = False
```

### Comparing `antidupe-0.0.3/antidupe/utilities.py` & `antidupe-0.0.4/antidupe/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,20 @@
     - channel_format: Desired channel format ('RGB' or 'L' for grayscale).
 
     Returns:
     - Resized and cropped versions of the input images.
     """
     if isinstance(image1, np.ndarray):
         image1 = Image.fromarray(image1)
+    else:
+        image1 = image1.copy()
     if isinstance(image2, np.ndarray):
         image2 = Image.fromarray(image2)
+    else:
+        image2 = image2.copy()
 
     aspect_ratio_1 = image1.width / image1.height
     aspect_ratio_2 = image2.width / image2.height
 
     if abs(aspect_ratio_1 - aspect_ratio_2) < 1e-6:
         image1 = resize_and_crop(image1, size, channel_format)
         image2 = resize_and_crop(image2, size, channel_format)
@@ -94,14 +98,16 @@
 
 def image_converter(image: [np.ndarray, Image.Image], size: int = 512, channel_format: str = 'RGB') -> Image.Image:
     """
     Converts a numpy array into an image object.
     """
     if isinstance(image, np.ndarray):
         image = Image.fromarray(image)
+    else:
+        image = image.copy()
     if image.size == (size, size) and image.mode == channel_format:
         return image
     image = image.resize((size, size))
     if image.mode != channel_format:
         image = image.convert(channel_format)
     return image
```

### Comparing `antidupe-0.0.3/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.4/antidupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.3/setup.py` & `antidupe-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

