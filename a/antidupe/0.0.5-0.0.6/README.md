# Comparing `tmp/antidupe-0.0.5.tar.gz` & `tmp/antidupe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidupe-0.0.5.tar", last modified: Wed May  1 19:39:22 2024, max compression
+gzip compressed data, was "antidupe-0.0.6.tar", last modified: Wed May  1 19:51:09 2024, max compression
```

## Comparing `antidupe-0.0.5.tar` & `antidupe-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.934507 antidupe-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 19:39:19.000000 antidupe-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:39:22.934507 antidupe-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 19:39:19.000000 antidupe-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.930507 antidupe-0.0.5/antidupe/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-01 19:39:19.000000 antidupe-0.0.5/antidupe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:39:22.934507 antidupe-0.0.5/antidupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 19:39:22.000000 antidupe-0.0.5/antidupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:39:22.934507 antidupe-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-01 19:39:19.000000 antidupe-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 19:50:58.000000 antidupe-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:51:09.219153 antidupe-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 19:50:58.000000 antidupe-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/antidupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-01 19:50:58.000000 antidupe-0.0.6/antidupe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.219153 antidupe-0.0.6/antidupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 19:51:09.000000 antidupe-0.0.6/antidupe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:51:09.219153 antidupe-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 19:50:58.000000 antidupe-0.0.6/setup.py
```

### Comparing `antidupe-0.0.5/LICENSE` & `antidupe-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.5/PKG-INFO` & `antidupe-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.5/README.md` & `antidupe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.5/antidupe/main.py` & `antidupe-0.0.6/antidupe/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
                 return True
             cnn = self.cnn.predict(im_1, im_2)
             self.d_print(f'cnn detected: {cnn}')
             if cnn < self.limits['cnn']:
                 self.d_print('cnn found duplicate')
                 return True
             dedup = self.dedup.predict(im_1, im_2)
+            self.d_print(f'dedup detected: {dedup}')
             if dedup < self.limits['dedup']:
                 self.d_print('dedup found duplicate')
                 return True
         return False
 
     def test(self, images: [list, tuple, None] = None):
         """
```

### Comparing `antidupe-0.0.5/antidupe/utilities.py` & `antidupe-0.0.6/antidupe/utilities.py`

 * *Files identical despite different names*

### Comparing `antidupe-0.0.5/antidupe.egg-info/PKG-INFO` & `antidupe-0.0.6/antidupe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidupe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Image deduplicator using CNN, Cosine Similarity, Image Hashing, Structural Similarity Index Measurement, and Euclidean Distance
 Home-page: https://github.com/manbehindthemadness/antidupe
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `antidupe-0.0.5/setup.py` & `antidupe-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='antidupe',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
@@ -48,8 +48,8 @@
     url='https://github.com/manbehindthemadness/antidupe',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.8',
-)
+)
```

