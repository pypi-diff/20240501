# Comparing `tmp/PyLauncherMPI-0.1.0.tar.gz` & `tmp/PyLauncherMPI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLauncherMPI-0.1.0.tar", last modified: Wed May  1 12:26:44 2024, max compression
+gzip compressed data, was "PyLauncherMPI-0.1.1.tar", last modified: Wed May  1 12:33:30 2024, max compression
```

## Comparing `PyLauncherMPI-0.1.0.tar` & `PyLauncherMPI-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:26:44.958343 PyLauncherMPI-0.1.0/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.0/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:26:44.955010 PyLauncherMPI-0.1.0/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:26:44.955010 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      250 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:26:44.000000 PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.0/README.md
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:26:44.958343 PyLauncherMPI-0.1.0/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1169 2024-05-01 12:23:53.000000 PyLauncherMPI-0.1.0/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.1/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      250 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.1/README.md
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1169 2024-05-01 12:33:01.000000 PyLauncherMPI-0.1.1/setup.py
```

### Comparing `PyLauncherMPI-0.1.0/LICENSE` & `PyLauncherMPI-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.0/PKG-INFO` & `PyLauncherMPI-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.0/PyLauncherMPI.egg-info/PKG-INFO` & `PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.0/setup.py` & `PyLauncherMPI-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.0',
+    version='0.1.1',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description='A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ioannis-vm/PyLauncherMPI',
     packages=find_packages(),
```

