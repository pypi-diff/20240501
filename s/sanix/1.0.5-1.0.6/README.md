# Comparing `tmp/sanix-1.0.5.tar.gz` & `tmp/sanix-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanix-1.0.5.tar", last modified: Tue Feb 13 21:59:50 2024, max compression
+gzip compressed data, was "sanix-1.0.6.tar", last modified: Wed May  1 21:02:55 2024, max compression
```

## Comparing `sanix-1.0.5.tar` & `sanix-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:59:50.656731 sanix-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-13 21:59:41.000000 sanix-1.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-13 21:59:50.656731 sanix-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-13 21:59:41.000000 sanix-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-13 21:59:41.000000 sanix-1.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:59:50.656731 sanix-1.0.5/sanix/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-13 21:59:41.000000 sanix-1.0.5/sanix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-13 21:59:41.000000 sanix-1.0.5/sanix/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-13 21:59:41.000000 sanix-1.0.5/sanix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-13 21:59:41.000000 sanix-1.0.5/sanix/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:59:50.656731 sanix-1.0.5/sanix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-13 21:59:50.000000 sanix-1.0.5/sanix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-13 21:59:50.000000 sanix-1.0.5/sanix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 21:59:50.000000 sanix-1.0.5/sanix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-13 21:59:50.000000 sanix-1.0.5/sanix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-13 21:59:50.000000 sanix-1.0.5/sanix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 21:59:50.656731 sanix-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-13 21:59:41.000000 sanix-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:02:55.589110 sanix-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 21:02:51.000000 sanix-1.0.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 21:02:55.589110 sanix-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 21:02:51.000000 sanix-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 21:02:51.000000 sanix-1.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:02:55.589110 sanix-1.0.6/sanix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 21:02:51.000000 sanix-1.0.6/sanix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-01 21:02:51.000000 sanix-1.0.6/sanix/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-01 21:02:51.000000 sanix-1.0.6/sanix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-01 21:02:51.000000 sanix-1.0.6/sanix/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:02:55.589110 sanix-1.0.6/sanix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 21:02:55.000000 sanix-1.0.6/sanix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 21:02:55.000000 sanix-1.0.6/sanix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:02:55.000000 sanix-1.0.6/sanix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:02:55.000000 sanix-1.0.6/sanix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 21:02:55.000000 sanix-1.0.6/sanix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:02:55.589110 sanix-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-01 21:02:51.000000 sanix-1.0.6/setup.py
```

### Comparing `sanix-1.0.5/LICENCE` & `sanix-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `sanix-1.0.5/PKG-INFO` & `sanix-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanix
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python wrapper for getting measurements data from Sanix devices.
 Home-page: https://github.com/tomaszsluszniak/sanix_py
 Author: Tomasz Słuszniak
 Author-email: tomasz.sluszniak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sanix-1.0.5/sanix/__init__.py` & `sanix-1.0.6/sanix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Sanix API class."""
 import datetime
+import re
 from zoneinfo import ZoneInfo
 import requests
 
 from .const import (
     ATTR_API_BATTERY,
     ATTR_API_DEVICE_NO,
     ATTR_API_DISTANCE,
@@ -34,15 +35,15 @@
             resp.raise_for_status()
             _json = resp.json()
             return Measurement(
                 battery=_json[ATTR_API_BATTERY],
                 device_no=_json[ATTR_API_DEVICE_NO],
                 distance=_json[ATTR_API_DISTANCE],
                 fill_perc=_json[ATTR_API_FILL_PERC],
-                service_date=datetime.datetime.strptime(_json[ATTR_API_SERVICE_DATE], "%d.%m.%Y").date(),
+                service_date=datetime.datetime.strptime(_json[ATTR_API_SERVICE_DATE], "%d.%m.%Y").date() if re.match('\d{2}.\d{2}.\d{4}', _json[ATTR_API_SERVICE_DATE]) else None,
                 ssid=_json[ATTR_API_SSID],
                 status=_json[ATTR_API_STATUS],
                 time=datetime.datetime.strptime(_json[ATTR_API_TIME], "%d.%m.%Y %H:%M:%S").replace(tzinfo=ZoneInfo("Europe/Warsaw"))
             )
         except requests.HTTPError as err:
             if err.response is not None:
                 if err.response.status_code == 401:
```

### Comparing `sanix-1.0.5/sanix.egg-info/PKG-INFO` & `sanix-1.0.6/sanix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanix
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python wrapper for getting measurements data from Sanix devices.
 Home-page: https://github.com/tomaszsluszniak/sanix_py
 Author: Tomasz Słuszniak
 Author-email: tomasz.sluszniak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sanix-1.0.5/setup.py` & `sanix-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='sanix',
-    version='1.0.5',
+    version='1.0.6',
     description=
     'Python wrapper for getting measurements data from Sanix devices.',
     long_description=long_description,
     url='https://github.com/tomaszsluszniak/sanix_py',
     license='MIT',
     packages=['sanix'],
     install_requires=REQUIRES,
```

