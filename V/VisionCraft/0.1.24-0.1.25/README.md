# Comparing `tmp/VisionCraft-0.1.24.tar.gz` & `tmp/VisionCraft-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.1.24.tar", last modified: Wed May  1 08:27:25 2024, max compression
+gzip compressed data, was "VisionCraft-0.1.25.tar", last modified: Wed May  1 08:52:51 2024, max compression
```

## Comparing `VisionCraft-0.1.24.tar` & `VisionCraft-0.1.25.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.214634 VisionCraft-0.1.24/
--rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.1.24/LICENSE
--rw-rw-rw-   0        0        0    17602 2024-05-01 08:27:25.214634 VisionCraft-0.1.24/PKG-INFO
--rw-rw-rw-   0        0        0    16590 2024-04-01 14:42:43.000000 VisionCraft-0.1.24/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.117949 VisionCraft-0.1.24/VisionCraft/
--rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.1.24/VisionCraft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.131832 VisionCraft-0.1.24/VisionCraft/craft/
--rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.1.24/VisionCraft/craft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.142750 VisionCraft-0.1.24/VisionCraft/help/
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.191190 VisionCraft-0.1.24/VisionCraft/help/Experiment/
--rw-rw-rw-   0        0        0  3004238 2024-04-18 03:58:39.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp1.ipynb
--rw-rw-rw-   0        0        0  2216233 2024-04-18 03:58:46.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp2.ipynb
--rw-rw-rw-   0        0        0  1201342 2024-04-18 04:05:06.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp3.ipynb
--rw-rw-rw-   0        0        0  1262767 2024-04-18 04:05:35.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp4.ipynb
--rw-rw-rw-   0        0        0   332016 2024-04-18 04:05:28.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp5.ipynb
--rw-rw-rw-   0        0        0   379367 2024-04-18 04:05:40.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp6.ipynb
--rw-rw-rw-   0        0        0  1423296 2024-04-18 04:06:03.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp7.ipynb
--rw-rw-rw-   0        0        0   517272 2024-04-18 04:12:36.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp8.ipynb
--rw-rw-rw-   0        0        0   287542 2024-04-18 04:12:40.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp9.ipynb
--rw-rw-rw-   0        0        0       41 2024-04-18 05:38:17.000000 VisionCraft-0.1.24/VisionCraft/help/Experiment/__init__.py
--rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.1.24/VisionCraft/help/__init__.py
--rw-rw-rw-   0        0        0    25401 2024-05-01 08:27:11.000000 VisionCraft-0.1.24/VisionCraft/help/exp2.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.211771 VisionCraft-0.1.24/VisionCraft/vision/
--rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.1.24/VisionCraft/vision/__init__.py
--rw-rw-rw-   0        0        0     9771 2024-04-09 15:52:59.000000 VisionCraft-0.1.24/VisionCraft/vision/filter.py
--rw-rw-rw-   0        0        0     2117 2024-05-01 08:19:30.000000 VisionCraft-0.1.24/VisionCraft/vision/huffman.py
--rw-rw-rw-   0        0        0     6836 2024-03-13 03:13:00.000000 VisionCraft-0.1.24/VisionCraft/vision/processing.py
--rw-rw-rw-   0        0        0     7996 2024-04-03 08:40:46.000000 VisionCraft-0.1.24/VisionCraft/vision/segmentation.py
--rw-rw-rw-   0        0        0     9901 2024-03-13 03:13:52.000000 VisionCraft-0.1.24/VisionCraft/vision/transform.py
--rw-rw-rw-   0        0        0     9303 2024-03-13 03:14:28.000000 VisionCraft-0.1.24/VisionCraft/vision/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:27:25.131832 VisionCraft-0.1.24/VisionCraft.egg-info/
--rw-rw-rw-   0        0        0    17602 2024-05-01 08:27:24.000000 VisionCraft-0.1.24/VisionCraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      917 2024-05-01 08:27:24.000000 VisionCraft-0.1.24/VisionCraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 08:27:24.000000 VisionCraft-0.1.24/VisionCraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-01 08:27:24.000000 VisionCraft-0.1.24/VisionCraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 08:27:24.000000 VisionCraft-0.1.24/VisionCraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 08:27:25.214634 VisionCraft-0.1.24/setup.cfg
--rw-rw-rw-   0        0        0     1280 2024-05-01 08:27:16.000000 VisionCraft-0.1.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.803967 VisionCraft-0.1.25/
+-rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.1.25/LICENSE
+-rw-rw-rw-   0        0        0    17602 2024-05-01 08:52:51.750570 VisionCraft-0.1.25/PKG-INFO
+-rw-rw-rw-   0        0        0    16590 2024-04-01 14:42:43.000000 VisionCraft-0.1.25/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.427580 VisionCraft-0.1.25/VisionCraft/
+-rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.1.25/VisionCraft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.454182 VisionCraft-0.1.25/VisionCraft/craft/
+-rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.1.25/VisionCraft/craft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.457991 VisionCraft-0.1.25/VisionCraft/help/
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.705453 VisionCraft-0.1.25/VisionCraft/help/Experiment/
+-rw-rw-rw-   0        0        0  3004238 2024-04-18 03:58:39.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp1.ipynb
+-rw-rw-rw-   0        0        0  2216233 2024-04-18 03:58:46.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp2.ipynb
+-rw-rw-rw-   0        0        0  1201342 2024-04-18 04:05:06.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp3.ipynb
+-rw-rw-rw-   0        0        0  1262767 2024-04-18 04:05:35.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp4.ipynb
+-rw-rw-rw-   0        0        0   332016 2024-04-18 04:05:28.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp5.ipynb
+-rw-rw-rw-   0        0        0   379367 2024-04-18 04:05:40.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp6.ipynb
+-rw-rw-rw-   0        0        0  1423296 2024-04-18 04:06:03.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp7.ipynb
+-rw-rw-rw-   0        0        0   517272 2024-04-18 04:12:36.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp8.ipynb
+-rw-rw-rw-   0        0        0   287542 2024-04-18 04:12:40.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp9.ipynb
+-rw-rw-rw-   0        0        0       41 2024-04-18 05:38:17.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.1.25/VisionCraft/help/__init__.py
+-rw-rw-rw-   0        0        0    25401 2024-05-01 08:27:11.000000 VisionCraft-0.1.25/VisionCraft/help/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.743547 VisionCraft-0.1.25/VisionCraft/vision/
+-rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.1.25/VisionCraft/vision/__init__.py
+-rw-rw-rw-   0        0        0     9771 2024-04-09 15:52:59.000000 VisionCraft-0.1.25/VisionCraft/vision/filter.py
+-rw-rw-rw-   0        0        0     2117 2024-05-01 08:19:30.000000 VisionCraft-0.1.25/VisionCraft/vision/huffman.py
+-rw-rw-rw-   0        0        0     6836 2024-03-13 03:13:00.000000 VisionCraft-0.1.25/VisionCraft/vision/processing.py
+-rw-rw-rw-   0        0        0     7996 2024-04-03 08:40:46.000000 VisionCraft-0.1.25/VisionCraft/vision/segmentation.py
+-rw-rw-rw-   0        0        0     9901 2024-03-13 03:13:52.000000 VisionCraft-0.1.25/VisionCraft/vision/transform.py
+-rw-rw-rw-   0        0        0     9303 2024-03-13 03:14:28.000000 VisionCraft-0.1.25/VisionCraft/vision/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.446164 VisionCraft-0.1.25/VisionCraft.egg-info/
+-rw-rw-rw-   0        0        0    17602 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2024-05-01 08:52:51.000000 VisionCraft-0.1.25/VisionCraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 08:52:51.804967 VisionCraft-0.1.25/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2024-05-01 08:52:28.000000 VisionCraft-0.1.25/setup.py
```

### Comparing `VisionCraft-0.1.24/LICENSE` & `VisionCraft-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/PKG-INFO` & `VisionCraft-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.1.24
+Version: 0.1.25
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.1.24/README.md` & `VisionCraft-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp1.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp1.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp2.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp2.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp3.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp3.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp4.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp4.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp5.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp5.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp6.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp6.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp7.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp7.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp8.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp8.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/Experiment/Exp9.ipynb` & `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp9.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/help/exp2.py` & `VisionCraft-0.1.25/VisionCraft/help/exp.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/__init__.py` & `VisionCraft-0.1.25/VisionCraft/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/filter.py` & `VisionCraft-0.1.25/VisionCraft/vision/filter.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/huffman.py` & `VisionCraft-0.1.25/VisionCraft/vision/huffman.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/processing.py` & `VisionCraft-0.1.25/VisionCraft/vision/processing.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/segmentation.py` & `VisionCraft-0.1.25/VisionCraft/vision/segmentation.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/transform.py` & `VisionCraft-0.1.25/VisionCraft/vision/transform.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft/vision/utils.py` & `VisionCraft-0.1.25/VisionCraft/vision/utils.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.24/VisionCraft.egg-info/PKG-INFO` & `VisionCraft-0.1.25/VisionCraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.1.24
+Version: 0.1.25
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.1.24/VisionCraft.egg-info/SOURCES.txt` & `VisionCraft-0.1.25/VisionCraft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 VisionCraft.egg-info/PKG-INFO
 VisionCraft.egg-info/SOURCES.txt
 VisionCraft.egg-info/dependency_links.txt
 VisionCraft.egg-info/requires.txt
 VisionCraft.egg-info/top_level.txt
 VisionCraft/craft/__init__.py
 VisionCraft/help/__init__.py
-VisionCraft/help/exp2.py
+VisionCraft/help/exp.py
 VisionCraft/help/Experiment/Exp1.ipynb
 VisionCraft/help/Experiment/Exp2.ipynb
 VisionCraft/help/Experiment/Exp3.ipynb
 VisionCraft/help/Experiment/Exp4.ipynb
 VisionCraft/help/Experiment/Exp5.ipynb
 VisionCraft/help/Experiment/Exp6.ipynb
 VisionCraft/help/Experiment/Exp7.ipynb
```

### Comparing `VisionCraft-0.1.24/setup.py` & `VisionCraft-0.1.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.24'
+VERSION = '0.1.25'
 DESCRIPTION = 'Computer Vision Library to help do CV much faster, Updated Filters'
 LONG_DESCRIPTION = 'Simplifying computer vision tasks with Python. Visualize, transform, and analyze images effortlessly. Ideal for students, researchers, and developers. Enhance your computer vision projects!'
 
 # Setting up    
 setup(
     name="VisionCraft",
     version=VERSION,
```

