# Comparing `tmp/PyLauncherMPI-0.1.2.tar.gz` & `tmp/PyLauncherMPI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLauncherMPI-0.1.2.tar", last modified: Wed May  1 12:44:03 2024, max compression
+gzip compressed data, was "PyLauncherMPI-0.1.3.tar", last modified: Wed May  1 12:49:29 2024, max compression
```

## Comparing `PyLauncherMPI-0.1.2.tar` & `PyLauncherMPI-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.043734 PyLauncherMPI-0.1.2/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.2/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      101 2024-05-01 12:43:22.000000 PyLauncherMPI-0.1.2/MANIFEST.in
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      284 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.2/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/pylaunchermpi/
--rw-------   0 john_vm   (1000) john_vm   (1000)     3173 2024-05-01 12:22:15.000000 PyLauncherMPI-0.1.2/pylaunchermpi/main.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:44:03.043734 PyLauncherMPI-0.1.2/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1200 2024-05-01 12:44:00.000000 PyLauncherMPI-0.1.2/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.3/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       43 2024-05-01 12:49:18.000000 PyLauncherMPI-0.1.3/MANIFEST.in
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      284 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.3/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/pylaunchermpi/
+-rw-------   0 john_vm   (1000) john_vm   (1000)     3173 2024-05-01 12:22:15.000000 PyLauncherMPI-0.1.3/pylaunchermpi/main.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1200 2024-05-01 12:48:06.000000 PyLauncherMPI-0.1.3/setup.py
```

### Comparing `PyLauncherMPI-0.1.2/LICENSE` & `PyLauncherMPI-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.2/PKG-INFO` & `PyLauncherMPI-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/PKG-INFO` & `PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.2/pylaunchermpi/main.py` & `PyLauncherMPI-0.1.3/pylaunchermpi/main.py`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.2/setup.py` & `PyLauncherMPI-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.2',
+    version='0.1.3',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description='A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ioannis-vm/PyLauncherMPI',
     packages=find_packages(),
```

