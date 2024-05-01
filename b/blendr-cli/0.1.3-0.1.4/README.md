# Comparing `tmp/blendr_cli-0.1.3.tar.gz` & `tmp/blendr_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendr_cli-0.1.3.tar", last modified: Tue Apr 30 15:23:08 2024, max compression
+gzip compressed data, was "blendr_cli-0.1.4.tar", last modified: Tue Apr 30 15:25:22 2024, max compression
```

## Comparing `blendr_cli-0.1.3.tar` & `blendr_cli-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.015129 blendr_cli-0.1.3/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3134 2024-04-30 15:23:08.014868 blendr_cli-0.1.3/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.3/README.md
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.010820 blendr_cli-0.1.3/blendr/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.3/blendr/__init__.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.011414 blendr_cli-0.1.3/blendr/auth/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.3/blendr/auth/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1923 2024-04-30 07:06:02.000000 blendr_cli-0.1.3/blendr/auth/authenticate.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1917 2024-04-30 07:02:44.000000 blendr_cli-0.1.3/blendr/cli.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.012276 blendr_cli-0.1.3/blendr/config/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.3/blendr/config/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      158 2024-04-30 13:58:05.000000 blendr_cli-0.1.3/blendr/config/settings.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     6119 2024-04-30 14:25:22.000000 blendr_cli-0.1.3/blendr/config/setup.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.012787 blendr_cli-0.1.3/blendr/gpu_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.3/blendr/gpu_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.3/blendr/gpu_manager/detect.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.013270 blendr_cli-0.1.3/blendr/task_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.3/blendr/task_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.3/blendr/task_manager/listen.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.014600 blendr_cli-0.1.3/blendr_cli.egg-info/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3134 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/entry_points.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       71 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/requires.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/top_level.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-30 15:23:08.015175 blendr_cli-0.1.3/setup.cfg
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      844 2024-04-30 15:22:52.000000 blendr_cli-0.1.3/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.964002 blendr_cli-0.1.4/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3157 2024-04-30 15:25:22.963775 blendr_cli-0.1.4/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.4/README.md
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.960038 blendr_cli-0.1.4/blendr/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.4/blendr/__init__.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.960479 blendr_cli-0.1.4/blendr/auth/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.4/blendr/auth/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1923 2024-04-30 07:06:02.000000 blendr_cli-0.1.4/blendr/auth/authenticate.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1917 2024-04-30 07:02:44.000000 blendr_cli-0.1.4/blendr/cli.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.961144 blendr_cli-0.1.4/blendr/config/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.4/blendr/config/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      158 2024-04-30 13:58:05.000000 blendr_cli-0.1.4/blendr/config/settings.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     6119 2024-04-30 14:25:22.000000 blendr_cli-0.1.4/blendr/config/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.961663 blendr_cli-0.1.4/blendr/gpu_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.4/blendr/gpu_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.4/blendr/gpu_manager/detect.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.962255 blendr_cli-0.1.4/blendr/task_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.4/blendr/task_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.4/blendr/task_manager/listen.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:25:22.963524 blendr_cli-0.1.4/blendr_cli.egg-info/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3157 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       94 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/requires.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-30 15:25:22.000000 blendr_cli-0.1.4/blendr_cli.egg-info/top_level.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-30 15:25:22.964045 blendr_cli-0.1.4/setup.cfg
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      878 2024-04-30 15:25:19.000000 blendr_cli-0.1.4/setup.py
```

### Comparing `blendr_cli-0.1.3/PKG-INFO` & `blendr_cli-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
 Requires-Dist: GPUtil
 Requires-Dist: psutil
 Requires-Dist: keyring
 Requires-Dist: speedtest-cli
-Requires-Dist: py-cpuinfo
+Requires-Dist: py-cpuinfopython-socketio[client]
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.3/README.md` & `blendr_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.3/blendr/auth/authenticate.py` & `blendr_cli-0.1.4/blendr/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.3/blendr/cli.py` & `blendr_cli-0.1.4/blendr/cli.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.3/blendr/config/setup.py` & `blendr_cli-0.1.4/blendr/config/setup.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.3/blendr/task_manager/listen.py` & `blendr_cli-0.1.4/blendr/task_manager/listen.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.3/blendr_cli.egg-info/PKG-INFO` & `blendr_cli-0.1.4/blendr_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
 Requires-Dist: GPUtil
 Requires-Dist: psutil
 Requires-Dist: keyring
 Requires-Dist: speedtest-cli
-Requires-Dist: py-cpuinfo
+Requires-Dist: py-cpuinfopython-socketio[client]
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.3/setup.py` & `blendr_cli-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='blendr-cli',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'click',      
         'requests',  
         'colorama',
         'GPUtil',
         'psutil',
         'keyring',
         'speedtest-cli',
         'py-cpuinfo'
+        'python-socketio[client]'
     ],
     entry_points={
         'console_scripts': [
             'blendr=blendr.cli:main'
         ]
     },
     author='Blendr Network',
```

