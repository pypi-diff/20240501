# Comparing `tmp/liveflask-1.0.1.tar.gz` & `tmp/liveflask-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.1.tar", last modified: Wed May  1 20:13:02 2024, max compression
+gzip compressed data, was "liveflask-1.0.2.tar", last modified: Wed May  1 20:18:05 2024, max compression
```

## Comparing `liveflask-1.0.1.tar` & `liveflask-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.917877 liveflask-1.0.1/
--rw-rw-rw-   0        0        0     1342 2024-05-01 20:13:02.915878 liveflask-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.872877 liveflask-1.0.1/liveflask/
--rw-rw-rw-   0        0        0     5778 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.883876 liveflask-1.0.1/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.884876 liveflask-1.0.1/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.898877 liveflask-1.0.1/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0      872 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     8446 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.902877 liveflask-1.0.1/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      284 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.914877 liveflask-1.0.1/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/__init__.py
--rw-rw-rw-   0        0        0     2042 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_snapshots.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.881876 liveflask-1.0.1/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 20:13:02.917877 liveflask-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-05-01 20:12:56.000000 liveflask-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.510434 liveflask-1.0.2/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 20:18:05.508346 liveflask-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.475435 liveflask-1.0.2/liveflask/
+-rw-rw-rw-   0        0        0     5778 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.483347 liveflask-1.0.2/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.484347 liveflask-1.0.2/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.494397 liveflask-1.0.2/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1566 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0      872 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     8446 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.497348 liveflask-1.0.2/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      284 2024-05-01 18:57:08.000000 liveflask-1.0.2/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.507386 liveflask-1.0.2/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/__init__.py
+-rw-rw-rw-   0        0        0     2042 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 20:12:56.000000 liveflask-1.0.2/liveflask/traits/has_snapshots.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:18:05.481384 liveflask-1.0.2/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 20:18:05.000000 liveflask-1.0.2/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2024-05-01 20:18:05.000000 liveflask-1.0.2/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:18:05.000000 liveflask-1.0.2/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 20:18:05.000000 liveflask-1.0.2/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 20:18:05.000000 liveflask-1.0.2/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:18:05.510434 liveflask-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-01 20:18:03.000000 liveflask-1.0.2/setup.py
```

### Comparing `liveflask-1.0.1/PKG-INFO` & `liveflask-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.1
+Version: 1.0.2
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.1/liveflask/__init__.py` & `liveflask-1.0.2/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/attributes/__init__.py` & `liveflask-1.0.2/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/liveflask/action.js` & `liveflask-1.0.2/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.2/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/liveflask/model.js` & `liveflask-1.0.2/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/liveflask/polling.js` & `liveflask-1.0.2/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/liveflask/utils.js` & `liveflask-1.0.2/liveflask/static/liveflask/utils.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/static/lodash.min.js` & `liveflask-1.0.2/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/traits/has_actions.py` & `liveflask-1.0.2/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/traits/has_props.py` & `liveflask-1.0.2/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/traits/has_renders.py` & `liveflask-1.0.2/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask/traits/has_snapshots.py` & `liveflask-1.0.2/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.2/liveflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.1
+Version: 1.0.2
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.1/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.2/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.1/setup.py` & `liveflask-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.1",
+    version="1.0.2",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

