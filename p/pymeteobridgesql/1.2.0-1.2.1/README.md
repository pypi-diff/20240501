# Comparing `tmp/pymeteobridgesql-1.2.0.tar.gz` & `tmp/pymeteobridgesql-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.2.0.tar", last modified: Mon Apr 29 13:10:23 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.2.1.tar", last modified: Wed May  1 17:16:16 2024, max compression
```

## Comparing `pymeteobridgesql-1.2.0.tar` & `pymeteobridgesql-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:16:16.002991 pymeteobridgesql-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-01 17:16:16.002991 pymeteobridgesql-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:16:16.002991 pymeteobridgesql-1.2.1/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:16:16.002991 pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-01 17:16:15.000000 pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-01 17:16:15.000000 pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:16:15.000000 pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 17:16:15.000000 pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:16:16.002991 pymeteobridgesql-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 17:16:09.000000 pymeteobridgesql-1.2.1/setup.py
```

### Comparing `pymeteobridgesql-1.2.0/LICENSE` & `pymeteobridgesql-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.2.0/PKG-INFO` & `pymeteobridgesql-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.0
+Version: 1.2.1
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.0/pymeteobridgesql/api.py` & `pymeteobridgesql-1.2.1/pymeteobridgesql/api.py`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.2.0/pymeteobridgesql/data.py` & `pymeteobridgesql-1.2.1/pymeteobridgesql/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,14 +273,15 @@
     precipitation: float
     pressure: float
     sunriseepoch: int
     sunsetepoch: int
     wind_bearing: int
     wind_speed: float
     wind_gust: float
+    conditions: str
 
     def to_dict(self):
         return {
             "day_num": self.day_num,
             "datetime": self.datetime,
             "temperature": self.temperature,
             "temp_low": self.temp_low,
@@ -290,14 +291,15 @@
             "precipitation": self.precipitation,
             "pressure": self.pressure,
             "sunriseepoch": self.sunriseepoch,
             "sunsetepoch": self.sunsetepoch,
             "wind_bearing": self.wind_bearing,
             "wind_speed": self.wind_speed,
             "wind_gust": self.wind_gust,
+            "conditions": self.conditions,
         }
 
 @dataclass(frozen=True)
 class StationData:
     ID: str
     mb_ip: str
     mb_swversion: str
```

### Comparing `pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.2.1/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.2.0
+Version: 1.2.1
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.2.0/setup.py` & `pymeteobridgesql-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.2.0",
+    version="1.2.1",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

