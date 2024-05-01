# Comparing `tmp/automvs-0.0.3.tar.gz` & `tmp/automvs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.3.tar", last modified: Tue Apr 30 16:17:49 2024, max compression
+gzip compressed data, was "automvs-0.0.4.tar", last modified: Wed May  1 05:50:09 2024, max compression
```

## Comparing `automvs-0.0.3.tar` & `automvs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.3/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-04-30 16:17:49.364480 automvs-0.0.3/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.3/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    19020 2024-04-30 16:16:50.000000 automvs-0.0.3/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-30 16:17:49.364480 automvs-0.0.3/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-04-30 16:16:55.000000 automvs-0.0.3/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.4/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 05:50:09.675153 automvs-0.0.4/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.4/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    19039 2024-05-01 05:48:13.000000 automvs-0.0.4/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 05:50:09.675153 automvs-0.0.4/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-01 05:48:06.000000 automvs-0.0.4/setup.py
```

### Comparing `automvs-0.0.3/LICENSE` & `automvs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.3/PKG-INFO` & `automvs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.3/README.md` & `automvs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.3/automvs/__init__.py` & `automvs-0.0.4/automvs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This library allows the use of MVS/CE in an automated fashion. This can
     be used for deploying XMI files, pushing out updates, building software,
     creating custom MVS deployments.
 
     Using this library requires a recent version of hercules SDL and MVS/CE.
 """
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -362,21 +362,21 @@
         '''
            Reads stdout queue waiting for expected response, default is
            to check STDOUT queue, set stderr=True to check stderr queue instead
            default timeout is 30 minutes
         '''
         time_started = time.time()
 
-        if not timeout:
-            timeout = TIMEOUT
-
         if not timeout and self.timeout:
             timeout=self.timeout
 
-        self.logger.debug("[AUTOMATION] Waiting for string to appear in hercules log: {}".format(string_to_waitfor))
+        if not timeout:
+            timeout = TIMEOUT
+
+        self.logger.debug("[AUTOMATION] Waiting {} seconds for string to appear in hercules log: {}".format(timeout,string_to_waitfor))
 
         while True:
             if time.time() > time_started + timeout:
                 exception = "Waiting for '{}' timed out after {} seconds".format(string_to_waitfor, timeout)
                 print("[AUTOMATION] {}".format(exception))
                 raise Exception(exception)
```

### Comparing `automvs-0.0.3/automvs.egg-info/PKG-INFO` & `automvs-0.0.4/automvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.3/setup.py` & `automvs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.3',    
+    version='0.0.4',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

