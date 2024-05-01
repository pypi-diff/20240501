# Comparing `tmp/PyLauncherMPI-0.1.3.tar.gz` & `tmp/PyLauncherMPI-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLauncherMPI-0.1.3.tar", last modified: Wed May  1 12:49:29 2024, max compression
+gzip compressed data, was "PyLauncherMPI-0.1.4.tar", last modified: Wed May  1 13:10:02 2024, max compression
```

## Comparing `PyLauncherMPI-0.1.3.tar` & `PyLauncherMPI-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.3/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       43 2024-05-01 12:49:18.000000 PyLauncherMPI-0.1.3/MANIFEST.in
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      284 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:49:29.000000 PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.3/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/pylaunchermpi/
--rw-------   0 john_vm   (1000) john_vm   (1000)     3173 2024-05-01 12:22:15.000000 PyLauncherMPI-0.1.3/pylaunchermpi/main.py
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:49:29.885167 PyLauncherMPI-0.1.3/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1200 2024-05-01 12:48:06.000000 PyLauncherMPI-0.1.3/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:10:02.055578 PyLauncherMPI-0.1.4/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.4/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 13:10:02.055578 PyLauncherMPI-0.1.4/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:10:02.052245 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 13:10:01.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      298 2024-05-01 13:10:02.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 13:10:01.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 13:10:01.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 13:10:01.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       14 2024-05-01 13:10:01.000000 PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.4/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:10:02.052245 PyLauncherMPI-0.1.4/pylaunchermpi/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 13:09:05.000000 PyLauncherMPI-0.1.4/pylaunchermpi/__init__.py
+-rw-------   0 john_vm   (1000) john_vm   (1000)     3173 2024-05-01 12:22:15.000000 PyLauncherMPI-0.1.4/pylaunchermpi/main.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 13:10:02.055578 PyLauncherMPI-0.1.4/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1168 2024-05-01 13:09:57.000000 PyLauncherMPI-0.1.4/setup.py
```

### Comparing `PyLauncherMPI-0.1.3/LICENSE` & `PyLauncherMPI-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.3/PKG-INFO` & `PyLauncherMPI-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.3/PyLauncherMPI.egg-info/PKG-INFO` & `PyLauncherMPI-0.1.4/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.3/pylaunchermpi/main.py` & `PyLauncherMPI-0.1.4/pylaunchermpi/main.py`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.3/setup.py` & `PyLauncherMPI-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.3',
+    version='0.1.4',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description='A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ioannis-vm/PyLauncherMPI',
     packages=find_packages(),
@@ -24,11 +24,11 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
-            'pylaunchermpi=pylaunchermpi.main:main',  # Adjust the path as necessary
+            'pylaunchermpi=pylaunchermpi.main:main',
         ],
     },
 )
```

