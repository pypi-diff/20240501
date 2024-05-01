# Comparing `tmp/automvs-0.0.5.tar.gz` & `tmp/automvs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.5.tar", last modified: Wed May  1 15:55:21 2024, max compression
+gzip compressed data, was "automvs-0.0.6.tar", last modified: Wed May  1 16:01:00 2024, max compression
```

## Comparing `automvs-0.0.5.tar` & `automvs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.5/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 15:55:21.707338 automvs-0.0.5/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.5/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    19906 2024-05-01 15:55:15.000000 automvs-0.0.5/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 15:55:21.707338 automvs-0.0.5/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-01 15:55:17.000000 automvs-0.0.5/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 16:01:00.969718 automvs-0.0.6/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.6/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 16:01:00.969718 automvs-0.0.6/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.6/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 16:01:00.969718 automvs-0.0.6/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    19908 2024-05-01 16:00:55.000000 automvs-0.0.6/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 16:01:00.969718 automvs-0.0.6/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 16:01:00.000000 automvs-0.0.6/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 16:01:00.000000 automvs-0.0.6/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 16:01:00.000000 automvs-0.0.6/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 16:01:00.000000 automvs-0.0.6/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 16:01:00.969718 automvs-0.0.6/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-01 16:00:47.000000 automvs-0.0.6/setup.py
```

### Comparing `automvs-0.0.5/LICENSE` & `automvs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.5/PKG-INFO` & `automvs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.5/README.md` & `automvs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.5/automvs/__init__.py` & `automvs-0.0.6/automvs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This library allows the use of MVS/CE in an automated fashion. This can
     be used for deploying XMI files, pushing out updates, building software,
     creating custom MVS deployments.
 
     Using this library requires a recent version of hercules SDL and MVS/CE.
 """
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -276,15 +276,15 @@
                                     "exitcode": j[10]
                                 }
                   maxcc=j[10]
                   stepname = j[2]
 
                   if j[3] != "-":
                       log = logmsg.format(j[1],j[2],j[3],j[11])
-                    step_status = {
+                      step_status = {
                                         "jobname:" : j[1],
                                         "procname": j[2],
                                         "stepname": j[3],
                                         "exitcode": j[11]
                                     }
                       stepname = j[3]
                       maxcc=j[11]
```

### Comparing `automvs-0.0.5/automvs.egg-info/PKG-INFO` & `automvs-0.0.6/automvs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.5/setup.py` & `automvs-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.5',    
+    version='0.0.6',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

