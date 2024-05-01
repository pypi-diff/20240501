# Comparing `tmp/ml_project_tracker-0.0.1.tar.gz` & `tmp/ml_project_tracker-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.1.tar", last modified: Thu Apr 25 21:15:28 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.2.dev1.tar", last modified: Wed May  1 21:45:19 2024, max compression
```

## Comparing `ml_project_tracker-0.0.1.tar` & `ml_project_tracker-0.0.2.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-04-25 21:15:28.169722 ml_project_tracker-0.0.1/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      569 2024-04-25 21:15:28.169722 ml_project_tracker-0.0.1/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.1/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-04-25 21:15:28.169722 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      569 2024-04-25 21:15:28.000000 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      227 2024-04-25 21:15:28.000000 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-04-25 21:15:28.000000 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       30 2024-04-25 21:15:28.000000 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-04-25 21:15:28.000000 ml_project_tracker-0.0.1/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-04-25 21:15:28.169722 ml_project_tracker-0.0.1/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      905 2024-04-25 21:07:05.000000 ml_project_tracker-0.0.1/setup.py
+drwxrwxr-x   0 lilia     (1000) lilia     (1000)        0 2024-05-01 21:45:19.379073 ml_project_tracker-0.0.2.dev1/
+-rw-r--r--   0 lilia     (1000) lilia     (1000)      597 2024-05-01 21:45:19.379073 ml_project_tracker-0.0.2.dev1/PKG-INFO
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)       12 2024-05-01 17:28:52.000000 ml_project_tracker-0.0.2.dev1/README.md
+drwxrwxr-x   0 lilia     (1000) lilia     (1000)        0 2024-05-01 21:45:19.379073 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/
+-rw-r--r--   0 lilia     (1000) lilia     (1000)      597 2024-05-01 21:45:19.000000 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)      227 2024-05-01 21:45:19.000000 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)        1 2024-05-01 21:45:19.000000 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)       38 2024-05-01 21:45:19.000000 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)        1 2024-05-01 21:45:19.000000 ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)       38 2024-05-01 21:45:19.379073 ml_project_tracker-0.0.2.dev1/setup.cfg
+-rw-rw-r--   0 lilia     (1000) lilia     (1000)      930 2024-05-01 21:33:47.000000 ml_project_tracker-0.0.2.dev1/setup.py
```

### Comparing `ml_project_tracker-0.0.1/PKG-INFO` & `ml_project_tracker-0.0.2.dev1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.1
+Version: 0.0.2.dev1
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: wandb
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
+Requires-Dist: neptune
 
 # ML-Tracker
```

### Comparing `ml_project_tracker-0.0.1/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.2.dev1/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.1
+Version: 0.0.2.dev1
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: wandb
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: torch
+Requires-Dist: neptune
 
 # ML-Tracker
```

### Comparing `ml_project_tracker-0.0.1/setup.py` & `ml_project_tracker-0.0.2.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.1',
+    version='0.0.2.dev1',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
     keywords=['Deep Learning', 'Machine Learning', 'Wandb', 'Neptune'],
     install_requires=[
         'wandb',
         'numpy',
         'torchvision',
-        'torch'
+        'torch', 
+        "neptune"
         # Add any other dependencies here
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

