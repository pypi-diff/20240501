# Comparing `tmp/PyVecs-0.0.6.tar.gz` & `tmp/pyvecs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVecs-0.0.6.tar", last modified: Tue Apr  9 22:19:04 2024, max compression
+gzip compressed data, was "pyvecs-0.0.7.tar", last modified: Wed May  1 19:33:49 2024, max compression
```

## Comparing `PyVecs-0.0.6.tar` & `pyvecs-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.335529 PyVecs-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 22:19:04.335529 PyVecs-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.331529 PyVecs-0.0.6/PyVecs/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 22:18:54.000000 PyVecs-0.0.6/PyVecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-09 22:18:54.000000 PyVecs-0.0.6/PyVecs/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:19:04.335529 PyVecs-0.0.6/PyVecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:19:04.000000 PyVecs-0.0.6/PyVecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 22:18:54.000000 PyVecs-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:19:04.335529 PyVecs-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 22:18:54.000000 PyVecs-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:33:49.157380 pyvecs-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 19:33:49.157380 pyvecs-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:33:49.157380 pyvecs-0.0.7/PyVecs/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 19:33:41.000000 pyvecs-0.0.7/PyVecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-01 19:33:41.000000 pyvecs-0.0.7/PyVecs/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:33:49.157380 pyvecs-0.0.7/PyVecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 19:33:49.000000 pyvecs-0.0.7/PyVecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 19:33:49.000000 pyvecs-0.0.7/PyVecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:33:49.000000 pyvecs-0.0.7/PyVecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:33:49.000000 pyvecs-0.0.7/PyVecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 19:33:41.000000 pyvecs-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:33:49.157380 pyvecs-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-01 19:33:41.000000 pyvecs-0.0.7/setup.py
```

### Comparing `PyVecs-0.0.6/PKG-INFO` & `pyvecs-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: PyVecs
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple 2D and 3D Vector class to Python.
 Author: Thales Rodrigues
 Author-email: thaleshend@gmail.com
 Project-URL: Github, https://github.com/Thales625/PyVecs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10,<=3.12.2
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyVecs
 Vector 2D and Vector 3D for Python
 
 ## Installation
```

### Comparing `PyVecs-0.0.6/PyVecs/main.py` & `pyvecs-0.0.7/PyVecs/main.py`

 * *Files identical despite different names*

### Comparing `PyVecs-0.0.6/PyVecs.egg-info/PKG-INFO` & `pyvecs-0.0.7/PyVecs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: PyVecs
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple 2D and 3D Vector class to Python.
 Author: Thales Rodrigues
 Author-email: thaleshend@gmail.com
 Project-URL: Github, https://github.com/Thales625/PyVecs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10,<=3.12.2
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyVecs
 Vector 2D and Vector 3D for Python
 
 ## Installation
```

### Comparing `PyVecs-0.0.6/setup.py` & `pyvecs-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 
 setup(
     name="PyVecs",
-    version="0.0.6",
+    version="0.0.7",
     author="Thales Rodrigues",
     author_email="thaleshend@gmail.com",
     description="A simple 2D and 3D Vector class to Python.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[],
@@ -18,9 +18,9 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Utilities"
     ],
-    python_requires=">=3.10,<=3.12.2"
+    python_requires=">=3.10"
 )
```

