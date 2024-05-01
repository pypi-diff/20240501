# Comparing `tmp/gosundpy-0.8.0.tar.gz` & `tmp/gosundpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gosundpy-0.8.0.tar", last modified: Sun Jul 16 23:17:37 2023, max compression
+gzip compressed data, was "gosundpy-0.9.0.tar", last modified: Wed May  1 03:36:06 2024, max compression
```

## Comparing `gosundpy-0.8.0.tar` & `gosundpy-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.264083 gosundpy-0.8.0/
--rw-r--r--   0 rabo       (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.8.0/LICENSE
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-16 23:17:37.263982 gosundpy-0.8.0/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.8.0/README.md
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.263287 gosundpy-0.8.0/gosundpy/
--rw-r--r--   0 rabo       (501) staff       (20)      715 2023-07-16 23:14:15.000000 gosundpy-0.8.0/gosundpy/__init__.py
--rw-r--r--   0 rabo       (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.8.0/gosundpy/device.py
--rw-r--r--   0 rabo       (501) staff       (20)      411 2023-07-16 23:14:12.000000 gosundpy-0.8.0/gosundpy/exceptions.py
--rw-r--r--   0 rabo       (501) staff       (20)     2621 2023-07-12 00:07:52.000000 gosundpy-0.8.0/gosundpy/gosund.py
--rw-r--r--   0 rabo       (501) staff       (20)     1047 2023-07-12 00:07:04.000000 gosundpy-0.8.0/gosundpy/utils.py
--rw-r--r--   0 rabo       (501) staff       (20)       18 2023-07-16 23:16:51.000000 gosundpy-0.8.0/gosundpy/version.py
-drwxr-xr-x   0 rabo       (501) staff       (20)        0 2023-07-16 23:17:37.263804 gosundpy-0.8.0/gosundpy.egg-info/
--rw-r--r--   0 rabo       (501) staff       (20)     2001 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/PKG-INFO
--rw-r--r--   0 rabo       (501) staff       (20)      305 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/SOURCES.txt
--rw-r--r--   0 rabo       (501) staff       (20)        1 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/dependency_links.txt
--rw-r--r--   0 rabo       (501) staff       (20)       23 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/requires.txt
--rw-r--r--   0 rabo       (501) staff       (20)        9 2023-07-16 23:17:37.000000 gosundpy-0.8.0/gosundpy.egg-info/top_level.txt
--rw-r--r--   0 rabo       (501) staff       (20)       38 2023-07-16 23:17:37.264119 gosundpy-0.8.0/setup.cfg
--rw-r--r--   0 rabo       (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.8.0/setup.py
+drwxr-xr-x   0 rey        (501) staff       (20)        0 2024-05-01 03:36:06.124409 gosundpy-0.9.0/
+-rw-r--r--   0 rey        (501) staff       (20)     1073 2022-10-16 07:49:52.000000 gosundpy-0.9.0/LICENSE
+-rw-r--r--   0 rey        (501) staff       (20)     2039 2024-05-01 03:36:06.124123 gosundpy-0.9.0/PKG-INFO
+-rw-r--r--   0 rey        (501) staff       (20)     1035 2022-11-27 06:20:19.000000 gosundpy-0.9.0/README.md
+drwxr-xr-x   0 rey        (501) staff       (20)        0 2024-05-01 03:36:06.122624 gosundpy-0.9.0/gosundpy/
+-rw-r--r--   0 rey        (501) staff       (20)      715 2023-07-16 23:14:15.000000 gosundpy-0.9.0/gosundpy/__init__.py
+-rw-r--r--   0 rey        (501) staff       (20)     3357 2023-01-18 01:29:44.000000 gosundpy-0.9.0/gosundpy/device.py
+-rw-r--r--   0 rey        (501) staff       (20)      411 2023-07-16 23:14:12.000000 gosundpy-0.9.0/gosundpy/exceptions.py
+-rw-r--r--   0 rey        (501) staff       (20)     2804 2024-05-01 03:30:43.000000 gosundpy-0.9.0/gosundpy/gosund.py
+-rw-r--r--   0 rey        (501) staff       (20)     1047 2023-07-12 00:07:04.000000 gosundpy-0.9.0/gosundpy/utils.py
+-rw-r--r--   0 rey        (501) staff       (20)       18 2024-05-01 03:36:02.000000 gosundpy-0.9.0/gosundpy/version.py
+drwxr-xr-x   0 rey        (501) staff       (20)        0 2024-05-01 03:36:06.123816 gosundpy-0.9.0/gosundpy.egg-info/
+-rw-r--r--   0 rey        (501) staff       (20)     2039 2024-05-01 03:36:06.000000 gosundpy-0.9.0/gosundpy.egg-info/PKG-INFO
+-rw-r--r--   0 rey        (501) staff       (20)      305 2024-05-01 03:36:06.000000 gosundpy-0.9.0/gosundpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rey        (501) staff       (20)        1 2024-05-01 03:36:06.000000 gosundpy-0.9.0/gosundpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rey        (501) staff       (20)       23 2024-05-01 03:36:06.000000 gosundpy-0.9.0/gosundpy.egg-info/requires.txt
+-rw-r--r--   0 rey        (501) staff       (20)        9 2024-05-01 03:36:06.000000 gosundpy-0.9.0/gosundpy.egg-info/top_level.txt
+-rw-r--r--   0 rey        (501) staff       (20)       38 2024-05-01 03:36:06.124469 gosundpy-0.9.0/setup.cfg
+-rw-r--r--   0 rey        (501) staff       (20)     1690 2022-10-16 07:49:52.000000 gosundpy-0.9.0/setup.py
```

### Comparing `gosundpy-0.8.0/LICENSE` & `gosundpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gosundpy-0.8.0/PKG-INFO` & `gosundpy-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tuya-iot-py-sdk==0.6.6
 
 # gosundpy
 
 [![PyPI version](https://badge.fury.io/py/gosundpy.svg)](https://badge.fury.io/py/gosundpy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gosundpy)
 
 Control your Gosund smart devices via python code.
```

### Comparing `gosundpy-0.8.0/README.md` & `gosundpy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gosundpy-0.8.0/gosundpy/__init__.py` & `gosundpy-0.9.0/gosundpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.8.0/gosundpy/device.py` & `gosundpy-0.9.0/gosundpy/device.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.8.0/gosundpy/gosund.py` & `gosundpy-0.9.0/gosundpy/gosund.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,21 @@
         if status is None:
             raise GosundException(
                 f'unable to find status for device with id "{device_id}"')
         return status
 
     def get_device_statuses(self):
         # limit 20 device_ids per api call
-        resp = self.manager.get_device_list_status(self._known_devices)
-        assert_response_success('get device statuses', resp)
-        return {device['id']: device['status'] for device in resp.get('result', [])}
+        results = []
+        known_devices = list(self._known_devices.keys())
+        for i in range(0, len(self._known_devices), 20):
+            resp = self.manager.get_device_list_status(known_devices[i:i+20])
+            assert_response_success('get device statuses', resp)
+            results.extend(resp.get('result') or [])
+        return {device['id']: device['status'] for device in results}
 
     def _add_known_device(self, device_id):
         self._known_devices[device_id] = True
         self._clear_statuses_cache()
 
     def _remove_known_device(self, device_id):
         del self._known_devices[device_id]
```

### Comparing `gosundpy-0.8.0/gosundpy/utils.py` & `gosundpy-0.9.0/gosundpy/utils.py`

 * *Files identical despite different names*

### Comparing `gosundpy-0.8.0/gosundpy.egg-info/PKG-INFO` & `gosundpy-0.9.0/gosundpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosundpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python API for controling Gosund smart devices
 Home-page: https://github.com/purple4reina/gosundpy
 Author: Rey Abolofia
 Author-email: purple4reina@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/purple4reina/gosundpy
 Project-URL: Bug Tracker, https://github.com/purple4reina/gosundpy/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tuya-iot-py-sdk==0.6.6
 
 # gosundpy
 
 [![PyPI version](https://badge.fury.io/py/gosundpy.svg)](https://badge.fury.io/py/gosundpy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gosundpy)
 
 Control your Gosund smart devices via python code.
```

### Comparing `gosundpy-0.8.0/setup.py` & `gosundpy-0.9.0/setup.py`

 * *Files identical despite different names*

