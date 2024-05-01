# Comparing `tmp/icc_utils-0.1.61.tar.gz` & `tmp/icc_utils-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icc_utils-0.1.61.tar", last modified: Wed May  1 16:21:22 2024, max compression
+gzip compressed data, was "icc_utils-0.1.62.tar", last modified: Wed May  1 16:25:34 2024, max compression
```

## Comparing `icc_utils-0.1.61.tar` & `icc_utils-0.1.62.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:21:22.259581 icc_utils-0.1.61/
--rw-rw-rw-   0        0        0     1068 2024-05-01 16:10:12.000000 icc_utils-0.1.61/LICENSE
--rw-rw-rw-   0        0        0      883 2024-05-01 16:21:22.243954 icc_utils-0.1.61/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-01 16:10:12.000000 icc_utils-0.1.61/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 16:21:22.150205 icc_utils-0.1.61/icc_utils/
--rw-rw-rw-   0        0        0     5463 2024-03-01 06:14:57.000000 icc_utils-0.1.61/icc_utils/PandasUtils.py
--rw-rw-rw-   0        0        0     7021 2024-03-01 06:14:57.000000 icc_utils-0.1.61/icc_utils/SQLUtils.py
--rw-rw-rw-   0        0        0     2355 2024-05-01 16:17:29.000000 icc_utils-0.1.61/icc_utils/Scheduler.py
--rw-rw-rw-   0        0        0    13332 2024-05-01 16:06:56.000000 icc_utils-0.1.61/icc_utils/SystemUtils.py
--rw-rw-rw-   0        0        0      407 2024-05-01 16:10:18.000000 icc_utils-0.1.61/icc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:21:22.197080 icc_utils-0.1.61/icc_utils.egg-info/
--rw-rw-rw-   0        0        0      883 2024-05-01 16:21:22.000000 icc_utils-0.1.61/icc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-01 16:21:22.000000 icc_utils-0.1.61/icc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:21:22.000000 icc_utils-0.1.61/icc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-01 16:21:22.000000 icc_utils-0.1.61/icc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 16:21:22.000000 icc_utils-0.1.61/icc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 16:21:22.259581 icc_utils-0.1.61/setup.cfg
--rw-rw-rw-   0        0        0     1178 2024-05-01 16:21:18.000000 icc_utils-0.1.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.110279 icc_utils-0.1.62/
+-rw-rw-rw-   0        0        0     1068 2024-05-01 16:10:12.000000 icc_utils-0.1.62/LICENSE
+-rw-rw-rw-   0        0        0      883 2024-05-01 16:25:34.094653 icc_utils-0.1.62/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:10:12.000000 icc_utils-0.1.62/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.000905 icc_utils-0.1.62/icc_utils/
+-rw-rw-rw-   0        0        0     5463 2024-03-01 06:14:57.000000 icc_utils-0.1.62/icc_utils/PandasUtils.py
+-rw-rw-rw-   0        0        0     7021 2024-03-01 06:14:57.000000 icc_utils-0.1.62/icc_utils/SQLUtils.py
+-rw-rw-rw-   0        0        0     2698 2024-05-01 16:25:26.000000 icc_utils-0.1.62/icc_utils/Scheduler.py
+-rw-rw-rw-   0        0        0    12141 2024-05-01 16:25:26.000000 icc_utils-0.1.62/icc_utils/SystemUtils.py
+-rw-rw-rw-   0        0        0      407 2024-05-01 16:10:18.000000 icc_utils-0.1.62/icc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.047781 icc_utils-0.1.62/icc_utils.egg-info/
+-rw-rw-rw-   0        0        0      883 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:25:34.110279 icc_utils-0.1.62/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2024-05-01 16:25:31.000000 icc_utils-0.1.62/setup.py
```

### Comparing `icc_utils-0.1.61/LICENSE` & `icc_utils-0.1.62/LICENSE`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.61/PKG-INFO` & `icc_utils-0.1.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.61
+Version: 0.1.62
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `icc_utils-0.1.61/icc_utils/PandasUtils.py` & `icc_utils-0.1.62/icc_utils/PandasUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.61/icc_utils/SQLUtils.py` & `icc_utils-0.1.62/icc_utils/SQLUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.61/icc_utils/Scheduler.py` & `icc_utils-0.1.62/icc_utils/Scheduler.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 
     def add_task(self, func, trigger, *args, **kwargs):
         """
         Adds a task to the scheduler.
 
         Args:
             func: The function to schedule.
-            trigger: A dict containing the schedule type (e.g., 'daily', 'interval') and its parameters.
+            trigger: A dict containing the schedule type (e.g., 'daily', 'interval', 'minute', 'at') and its parameters.
             args, kwargs: Arguments and keyword arguments for the scheduled function.
         """
         if trigger['type'] == 'interval':
-            # Schedule a task that runs at a regular interval
+            # Schedule a task that runs at a regular interval in seconds
             schedule.every(trigger['interval']).seconds.do(func, *args, **kwargs)
-        elif trigger['type'] == 'daily':
+        elif trigger['type'] == 'daily' and 'time' in trigger:
             # Schedule a task that runs once a day at a specific time
             schedule.every().day.at(trigger['time']).do(func, *args, **kwargs)
         elif trigger['type'] == 'minute':
             # Schedule a task that runs every 'X' minutes
             schedule.every(trigger['interval']).minutes.do(func, *args, **kwargs)
+        elif trigger['type'] == 'at' and 'time' in trigger:
+            # Schedule a task that runs at a specific time
+            schedule.every().day.at(trigger['time']).do(func, *args, **kwargs)
         else:
-            raise ValueError("Unsupported trigger type")
+            raise ValueError("Unsupported trigger type or missing parameters")
+
+        # Keep track of tasks if needed for later use or management
         self.tasks.append((func, trigger, args, kwargs))
 
     @staticmethod
     def run_continuously(interval=1):
         cease_continuous_run = threading.Event()
 
         class ScheduleThread(threading.Thread):
```

### Comparing `icc_utils-0.1.61/icc_utils/SystemUtils.py` & `icc_utils-0.1.62/icc_utils/SystemUtils.py`

 * *Files 7% similar despite different names*

```diff
@@ -337,34 +337,7 @@
                 subprocess.run(close_cmd, check=True)
 
             # Execute the launch command
             subprocess.run(launch_cmd, check=True)
         except subprocess.CalledProcessError as ex:
             print(f"Command failed with error: {ex}")
 
-    @staticmethod
-    def run_continuously(interval=1):
-        cease_continuous_run = threading.Event()
-
-        class ScheduleThread(threading.Thread):
-            @classmethod
-            def run(cls):
-                while not cease_continuous_run.is_set():
-                    try:
-                        schedule.run_pending()
-                        time.sleep(interval)
-                    except (KeyboardInterrupt, SystemExit):
-                        cease_continuous_run.set()  # Signal to stop the loop
-                        schedule.clear()  # Clear all scheduled tasks
-
-        continuous_thread = ScheduleThread()
-        continuous_thread.start()
-
-        try:
-            while continuous_thread.is_alive():
-                continuous_thread.join(timeout=1)  # Wait for the thread to finish unless interrupted
-        except (KeyboardInterrupt, SystemExit):
-            cease_continuous_run.set()  # Ensure that the event is set to stop the thread in case of interruption
-            continuous_thread.join()  # Wait for the thread to properly finish
-
-        print("Scheduler stopped and exited cleanly.")
-        return cease_continuous_run
```

### Comparing `icc_utils-0.1.61/icc_utils.egg-info/PKG-INFO` & `icc_utils-0.1.62/icc_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.61
+Version: 0.1.62
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `icc_utils-0.1.61/setup.py` & `icc_utils-0.1.62/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='icc_utils',
-    version='0.1.61',
+    version='0.1.62',
     packages=find_packages(),
     description='Package used to handle common functions at ICC',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jordan Bradley',
     author_email='jbradley@internationalcybernetics.com',
     url='https://github.com/jbradleyicc/icc_utils',
```

