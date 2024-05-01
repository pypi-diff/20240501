# Comparing `tmp/sideseeing_tools-0.2.1.tar.gz` & `tmp/sideseeing_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing_tools-0.2.1.tar", last modified: Wed Apr 24 23:40:11 2024, max compression
+gzip compressed data, was "sideseeing_tools-0.2.2.tar", last modified: Wed May  1 17:14:01 2024, max compression
```

## Comparing `sideseeing_tools-0.2.1.tar` & `sideseeing_tools-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:40:11.823863 sideseeing_tools-0.2.1/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.1/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11683 2024-04-24 23:40:11.819863 sideseeing_tools-0.2.1/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    10778 2024-04-24 23:29:33.000000 sideseeing_tools-0.2.1/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      894 2024-04-24 23:39:57.000000 sideseeing_tools-0.2.1/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-24 23:40:11.823863 sideseeing_tools-0.2.1/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:40:11.819863 sideseeing_tools-0.2.1/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:40:11.819863 sideseeing_tools-0.2.1/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-22 21:02:32.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2830 2024-04-24 21:04:42.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-22 21:11:00.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/plot.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     9507 2024-04-24 22:03:17.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8178 2024-04-24 22:11:35.000000 sideseeing_tools-0.2.1/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:40:11.819863 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11683 2024-04-24 23:40:11.000000 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      497 2024-04-24 23:40:11.000000 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-24 23:40:11.000000 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      145 2024-04-24 23:40:11.000000 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-24 23:40:11.000000 sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/top_level.txt
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 23:40:11.819863 sideseeing_tools-0.2.1/tests/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      114 2024-04-24 16:01:51.000000 sideseeing_tools-0.2.1/tests/test_media.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-05-01 17:14:01.215347 sideseeing_tools-0.2.2/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing_tools-0.2.2/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11623 2024-05-01 17:14:01.215347 sideseeing_tools-0.2.2/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    10778 2024-04-27 21:24:09.000000 sideseeing_tools-0.2.2/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      834 2024-05-01 17:11:43.000000 sideseeing_tools-0.2.2/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-05-01 17:14:01.215347 sideseeing_tools-0.2.2/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-05-01 17:14:01.207347 sideseeing_tools-0.2.2/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-05-01 17:14:01.215347 sideseeing_tools-0.2.2/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-11 19:11:31.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2830 2024-04-27 21:24:09.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-27 21:24:09.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/plot.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     9507 2024-04-27 21:24:09.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8178 2024-04-27 21:24:09.000000 sideseeing_tools-0.2.2/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-05-01 17:14:01.215347 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    11623 2024-05-01 17:14:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      477 2024-05-01 17:14:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-05-01 17:14:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       85 2024-05-01 17:14:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-05-01 17:14:01.000000 sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/top_level.txt
```

### Comparing `sideseeing_tools-0.2.1/LICENSE` & `sideseeing_tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/PKG-INFO` & `sideseeing_tools-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: folium~=0.13.0
-Requires-Dist: imageio~=2.5.0
-Requires-Dist: librosa~=0.10.0
+Requires-Dist: folium
+Requires-Dist: imageio
+Requires-Dist: librosa
 Requires-Dist: matplotlib
-Requires-Dist: moviepy~=1.0.3
-Requires-Dist: numpy~=1.25.0
-Requires-Dist: opencv-python~=4.7.0.68
-Requires-Dist: pandas~=2.0.3
-Requires-Dist: reverse-geocode==1.6
+Requires-Dist: moviepy
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: pandas
+Requires-Dist: reverse-geocode
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
```

### Comparing `sideseeing_tools-0.2.1/README.md` & `sideseeing_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/pyproject.toml` & `sideseeing_tools-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "sideseeing-tools"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-  "folium~=0.13.0",
-  "imageio~=2.5.0",
-  "librosa~=0.10.0",
+  "folium",
+  "imageio",
+  "librosa",
   "matplotlib",
-  "moviepy~=1.0.3",
-  "numpy~=1.25.0",
-  "opencv-python~=4.7.0.68",
-  "pandas~=2.0.3",
-  "reverse-geocode==1.6",
+  "moviepy",
+  "numpy",
+  "opencv-python",
+  "pandas",
+  "reverse-geocode",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
```

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools/constants.py` & `sideseeing_tools-0.2.2/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools/media.py` & `sideseeing_tools-0.2.2/src/sideseeing_tools/media.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools/plot.py` & `sideseeing_tools-0.2.2/src/sideseeing_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools/sideseeing.py` & `sideseeing_tools-0.2.2/src/sideseeing_tools/sideseeing.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools/utils.py` & `sideseeing_tools-0.2.2/src/sideseeing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.2.1/src/sideseeing_tools.egg-info/PKG-INFO` & `sideseeing_tools-0.2.2/src/sideseeing_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: folium~=0.13.0
-Requires-Dist: imageio~=2.5.0
-Requires-Dist: librosa~=0.10.0
+Requires-Dist: folium
+Requires-Dist: imageio
+Requires-Dist: librosa
 Requires-Dist: matplotlib
-Requires-Dist: moviepy~=1.0.3
-Requires-Dist: numpy~=1.25.0
-Requires-Dist: opencv-python~=4.7.0.68
-Requires-Dist: pandas~=2.0.3
-Requires-Dist: reverse-geocode==1.6
+Requires-Dist: moviepy
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: pandas
+Requires-Dist: reverse-geocode
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
```

