# Comparing `tmp/PyLauncherMPI-0.1.1.tar.gz` & `tmp/PyLauncherMPI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLauncherMPI-0.1.1.tar", last modified: Wed May  1 12:33:30 2024, max compression
+gzip compressed data, was "PyLauncherMPI-0.1.2.tar", last modified: Wed May  1 12:44:03 2024, max compression
```

## Comparing `PyLauncherMPI-0.1.1.tar` & `PyLauncherMPI-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.1/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/PKG-INFO
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      250 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/requires.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:33:30.000000 PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.1/README.md
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:33:30.697770 PyLauncherMPI-0.1.1/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1169 2024-05-01 12:33:01.000000 PyLauncherMPI-0.1.1/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.043734 PyLauncherMPI-0.1.2/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1081 2024-05-01 12:21:07.000000 PyLauncherMPI-0.1.2/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      101 2024-05-01 12:43:22.000000 PyLauncherMPI-0.1.2/MANIFEST.in
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/PKG-INFO
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      949 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      284 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       58 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        7 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/requires.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2024-05-01 12:44:02.000000 PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      110 2024-05-01 12:25:07.000000 PyLauncherMPI-0.1.2/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2024-05-01 12:44:03.040400 PyLauncherMPI-0.1.2/pylaunchermpi/
+-rw-------   0 john_vm   (1000) john_vm   (1000)     3173 2024-05-01 12:22:15.000000 PyLauncherMPI-0.1.2/pylaunchermpi/main.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2024-05-01 12:44:03.043734 PyLauncherMPI-0.1.2/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)     1200 2024-05-01 12:44:00.000000 PyLauncherMPI-0.1.2/setup.py
```

### Comparing `PyLauncherMPI-0.1.1/LICENSE` & `PyLauncherMPI-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLauncherMPI-0.1.1/PKG-INFO` & `PyLauncherMPI-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.1/PyLauncherMPI.egg-info/PKG-INFO` & `PyLauncherMPI-0.1.2/PyLauncherMPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLauncherMPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.
 Home-page: https://github.com/ioannis-vm/PyLauncherMPI
 Author: John Vouvakis Manousakis
 Author-email: ioannis_vm@berkeley.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `PyLauncherMPI-0.1.1/setup.py` & `PyLauncherMPI-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLauncherMPI',
-    version='0.1.1',
+    version='0.1.2',
     author='John Vouvakis Manousakis',
     author_email='ioannis_vm@berkeley.edu',
     description='A simple MPI-based task scheduler for dynamically distributing commands across MPI processes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ioannis-vm/PyLauncherMPI',
     packages=find_packages(),
+    include_package_data=True,
     install_requires=[
         'mpi4py',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
@@ -23,11 +24,11 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
-            'pylaunchermpi=PyLauncherMPI.main:main',  # Adjust the path as necessary
+            'pylaunchermpi=pylaunchermpi.main:main',  # Adjust the path as necessary
         ],
     },
 )
```

