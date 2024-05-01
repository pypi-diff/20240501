# Comparing `tmp/llamascript-0.0.3.tar.gz` & `tmp/llamascript-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.0.3.tar", last modified: Tue Apr 30 23:20:56 2024, max compression
+gzip compressed data, was "llamascript-0.1.0.tar", last modified: Tue Apr 30 23:53:03 2024, max compression
```

## Comparing `llamascript-0.0.3.tar` & `llamascript-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 23:20:56.253934 llamascript-0.0.3/
--rw-rw-rw-   0        0        0    11525 2024-04-30 21:46:58.000000 llamascript-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1208 2024-04-30 23:20:56.252932 llamascript-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      752 2024-04-30 23:13:49.000000 llamascript-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 23:20:56.226408 llamascript-0.0.3/llamascript/
--rw-rw-rw-   0        0        0     2650 2024-04-30 23:20:36.000000 llamascript-0.0.3/llamascript/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 23:20:56.249934 llamascript-0.0.3/llamascript.egg-info/
--rw-rw-rw-   0        0        0     1208 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 23:20:55.000000 llamascript-0.0.3/llamascript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 23:20:56.253934 llamascript-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      763 2024-04-30 23:20:45.000000 llamascript-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:53:03.071162 llamascript-0.1.0/
+-rw-rw-rw-   0        0        0    11525 2024-04-30 21:46:58.000000 llamascript-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1208 2024-04-30 23:53:03.070159 llamascript-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2024-04-30 23:13:49.000000 llamascript-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 23:53:03.045643 llamascript-0.1.0/llamascript/
+-rw-rw-rw-   0        0        0     3254 2024-04-30 23:49:41.000000 llamascript-0.1.0/llamascript/__init__.py
+-rw-rw-rw-   0        0        0      668 2024-04-30 23:50:30.000000 llamascript-0.1.0/llamascript/test.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:53:03.067162 llamascript-0.1.0/llamascript.egg-info/
+-rw-rw-rw-   0        0        0     1208 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 23:53:02.000000 llamascript-0.1.0/llamascript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 23:53:03.071162 llamascript-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-04-30 23:52:18.000000 llamascript-0.1.0/setup.py
```

### Comparing `llamascript-0.0.3/LICENSE` & `llamascript-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.0.3/PKG-INFO` & `llamascript-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.0.3
+Version: 0.1.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.0.3/README.md` & `llamascript-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `llamascript-0.0.3/llamascript.egg-info/PKG-INFO` & `llamascript-0.1.0/llamascript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.0.3
+Version: 0.1.0
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.0.3/setup.py` & `llamascript-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="llamascript", 
-    version="0.0.3",
+    version="0.1.0",
     author="WolfTheDev",
     author_email="wolfthedev@gmail.com",
     description="No-code AI chatbot using Ollama.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/WolfTheDeveloper/llamascript",
     packages=setuptools.find_packages(),
```

