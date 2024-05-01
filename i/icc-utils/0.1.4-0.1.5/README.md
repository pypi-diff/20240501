# Comparing `tmp/icc_utils-0.1.4.tar.gz` & `tmp/icc_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icc_utils-0.1.4.tar", last modified: Thu Feb 29 23:22:16 2024, max compression
+gzip compressed data, was "icc_utils-0.1.5.tar", last modified: Wed May  1 16:10:23 2024, max compression
```

## Comparing `icc_utils-0.1.4.tar` & `icc_utils-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 23:22:16.461337 icc_utils-0.1.4/
--rw-rw-rw-   0        0        0      859 2024-02-29 23:22:16.460320 icc_utils-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-29 21:15:05.000000 icc_utils-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 23:22:16.448094 icc_utils-0.1.4/icc_utils/
--rw-rw-rw-   0        0        0     5463 2024-02-29 22:35:18.000000 icc_utils-0.1.4/icc_utils/PandasUtils.py
--rw-rw-rw-   0        0        0     7021 2024-02-29 22:09:57.000000 icc_utils-0.1.4/icc_utils/SQLUtils.py
--rw-rw-rw-   0        0        0    12091 2024-02-29 22:48:24.000000 icc_utils-0.1.4/icc_utils/SystemUtils.py
--rw-rw-rw-   0        0        0      407 2024-02-29 21:39:44.000000 icc_utils-0.1.4/icc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 23:22:16.458286 icc_utils-0.1.4/icc_utils.egg-info/
--rw-rw-rw-   0        0        0      859 2024-02-29 23:22:16.000000 icc_utils-0.1.4/icc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-02-29 23:22:16.000000 icc_utils-0.1.4/icc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 23:22:16.000000 icc_utils-0.1.4/icc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-02-29 23:22:16.000000 icc_utils-0.1.4/icc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-29 23:22:16.000000 icc_utils-0.1.4/icc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 23:22:16.461337 icc_utils-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-02-29 22:44:24.000000 icc_utils-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:10:23.879388 icc_utils-0.1.5/
+-rw-rw-rw-   0        0        0     1068 2024-05-01 16:10:12.000000 icc_utils-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      882 2024-05-01 16:10:23.879388 icc_utils-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:10:12.000000 icc_utils-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:10:23.332498 icc_utils-0.1.5/icc_utils/
+-rw-rw-rw-   0        0        0     5463 2024-03-01 06:14:57.000000 icc_utils-0.1.5/icc_utils/PandasUtils.py
+-rw-rw-rw-   0        0        0     7021 2024-03-01 06:14:57.000000 icc_utils-0.1.5/icc_utils/SQLUtils.py
+-rw-rw-rw-   0        0        0    13332 2024-05-01 16:06:56.000000 icc_utils-0.1.5/icc_utils/SystemUtils.py
+-rw-rw-rw-   0        0        0      407 2024-05-01 16:10:18.000000 icc_utils-0.1.5/icc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:10:23.816885 icc_utils-0.1.5/icc_utils.egg-info/
+-rw-rw-rw-   0        0        0      882 2024-05-01 16:10:22.000000 icc_utils-0.1.5/icc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-01 16:10:22.000000 icc_utils-0.1.5/icc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:10:22.000000 icc_utils-0.1.5/icc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-01 16:10:22.000000 icc_utils-0.1.5/icc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 16:10:22.000000 icc_utils-0.1.5/icc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:10:23.895008 icc_utils-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-05-01 16:06:58.000000 icc_utils-0.1.5/setup.py
```

### Comparing `icc_utils-0.1.4/PKG-INFO` & `icc_utils-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: sqlalchemy>=2.0.27
 Requires-Dist: pyodbc>=5.1.0
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: tqdm>=4.66.2
```

### Comparing `icc_utils-0.1.4/icc_utils/PandasUtils.py` & `icc_utils-0.1.5/icc_utils/PandasUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.4/icc_utils/SQLUtils.py` & `icc_utils-0.1.5/icc_utils/SQLUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.4/icc_utils/SystemUtils.py` & `icc_utils-0.1.5/icc_utils/SystemUtils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import ctypes
 import socket
 from pathlib import Path
 import random
 from tqdm import tqdm
 import shutil
 import subprocess
+import threading
+import time
+import schedule
 
 
 class SystemUtils:
 
     @staticmethod
     def get_env_variable(var_name, default=None):
         """
@@ -333,7 +336,35 @@
             if result.stdout.strip():
                 subprocess.run(close_cmd, check=True)
 
             # Execute the launch command
             subprocess.run(launch_cmd, check=True)
         except subprocess.CalledProcessError as ex:
             print(f"Command failed with error: {ex}")
+
+    @staticmethod
+    def run_continuously(interval=1):
+        cease_continuous_run = threading.Event()
+
+        class ScheduleThread(threading.Thread):
+            @classmethod
+            def run(cls):
+                while not cease_continuous_run.is_set():
+                    try:
+                        schedule.run_pending()
+                        time.sleep(interval)
+                    except (KeyboardInterrupt, SystemExit):
+                        cease_continuous_run.set()  # Signal to stop the loop
+                        schedule.clear()  # Clear all scheduled tasks
+
+        continuous_thread = ScheduleThread()
+        continuous_thread.start()
+
+        try:
+            while continuous_thread.is_alive():
+                continuous_thread.join(timeout=1)  # Wait for the thread to finish unless interrupted
+        except (KeyboardInterrupt, SystemExit):
+            cease_continuous_run.set()  # Ensure that the event is set to stop the thread in case of interruption
+            continuous_thread.join()  # Wait for the thread to properly finish
+
+        print("Scheduler stopped and exited cleanly.")
+        return cease_continuous_run
```

### Comparing `icc_utils-0.1.4/icc_utils.egg-info/PKG-INFO` & `icc_utils-0.1.5/icc_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: sqlalchemy>=2.0.27
 Requires-Dist: pyodbc>=5.1.0
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: tqdm>=4.66.2
```

### Comparing `icc_utils-0.1.4/setup.py` & `icc_utils-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='icc_utils',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     description='Package used to handle common functions at ICC',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jordan Bradley',
     author_email='jbradley@internationalcybernetics.com',
     url='https://github.com/jbradleyicc/icc_utils',
```

