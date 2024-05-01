# Comparing `tmp/droneinterface-0.0.3.tar.gz` & `tmp/droneinterface-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droneinterface-0.0.3.tar", last modified: Mon Apr 22 17:19:20 2024, max compression
+gzip compressed data, was "droneinterface-0.0.4.tar", last modified: Wed May  1 10:00:26 2024, max compression
```

## Comparing `droneinterface-0.0.3.tar` & `droneinterface-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-04-22 17:19:20.105490 droneinterface-0.0.3/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 16:01:29.000000 droneinterface-0.0.3/LICENSE
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1836 2024-04-22 17:19:20.105490 droneinterface-0.0.3/PKG-INFO
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-04-22 17:19:20.101490 droneinterface-0.0.3/droneinterface/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      704 2024-04-22 17:18:42.000000 droneinterface-0.0.3/droneinterface/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2492 2024-02-21 07:30:26.000000 droneinterface-0.0.3/droneinterface/combinators.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2407 2024-04-22 17:18:42.000000 droneinterface-0.0.3/droneinterface/commands.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7159 2024-04-22 17:18:42.000000 droneinterface-0.0.3/droneinterface/connection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3919 2024-04-22 17:18:42.000000 droneinterface-0.0.3/droneinterface/last_message.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-04-22 17:19:20.105490 droneinterface-0.0.3/droneinterface/messages/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      189 2023-05-11 22:39:42.000000 droneinterface-0.0.3/droneinterface/messages/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      846 2024-02-21 07:30:26.000000 droneinterface-0.0.3/droneinterface/messages/definitions.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4004 2024-03-08 18:07:10.000000 droneinterface-0.0.3/droneinterface/messages/wrapper_factory.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6306 2024-03-05 18:26:25.000000 droneinterface-0.0.3/droneinterface/messages/wrappers.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    10878 2024-04-22 17:18:42.000000 droneinterface-0.0.3/droneinterface/vehicle.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-04-22 17:19:20.101490 droneinterface-0.0.3/droneinterface.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1836 2024-04-22 17:19:19.000000 droneinterface-0.0.3/droneinterface.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      663 2024-04-22 17:19:20.000000 droneinterface-0.0.3/droneinterface.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-04-22 17:19:19.000000 droneinterface-0.0.3/droneinterface.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       11 2024-04-22 17:19:19.000000 droneinterface-0.0.3/droneinterface.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2024-04-22 17:19:19.000000 droneinterface-0.0.3/droneinterface.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1515 2024-03-05 19:34:08.000000 droneinterface-0.0.3/readme.md
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      416 2024-04-22 17:19:20.105490 droneinterface-0.0.3/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       68 2023-03-28 16:01:29.000000 droneinterface-0.0.3/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-04-22 17:19:20.105490 droneinterface-0.0.3/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      282 2023-07-10 13:20:08.000000 droneinterface-0.0.3/tests/test_connection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1107 2023-07-10 13:20:08.000000 droneinterface-0.0.3/tests/test_last_message.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1237 2023-07-10 13:20:08.000000 droneinterface-0.0.3/tests/test_vehicle.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      208 2024-04-22 17:18:42.000000 droneinterface-0.0.3/tests/test_wp.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      669 2023-05-16 13:27:55.000000 droneinterface-0.0.3/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:00:26.759963 droneinterface-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-01 10:00:00.000000 droneinterface-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-01 10:00:26.759963 droneinterface-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:00:26.759963 droneinterface-0.0.4/droneinterface/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/last_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-01 10:00:00.000000 droneinterface-0.0.4/droneinterface/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:00:26.759963 droneinterface-0.0.4/droneinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-01 10:00:26.000000 droneinterface-0.0.4/droneinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-01 10:00:26.000000 droneinterface-0.0.4/droneinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:00:26.000000 droneinterface-0.0.4/droneinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 10:00:26.000000 droneinterface-0.0.4/droneinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 10:00:26.000000 droneinterface-0.0.4/droneinterface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-01 10:00:00.000000 droneinterface-0.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-01 10:00:26.759963 droneinterface-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 10:00:00.000000 droneinterface-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:00:26.759963 droneinterface-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-01 10:00:00.000000 droneinterface-0.0.4/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 10:00:00.000000 droneinterface-0.0.4/tests/test_last_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 10:00:00.000000 droneinterface-0.0.4/tests/test_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 10:00:00.000000 droneinterface-0.0.4/tests/test_wp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 10:00:00.000000 droneinterface-0.0.4/tests/test_wrappers.py
```

### Comparing `droneinterface-0.0.3/LICENSE` & `droneinterface-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/PKG-INFO` & `droneinterface-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: droneinterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tidy way to talk to a Drone through PyMavLink
 Home-page: https://github.com/PyFlightCoach/DroneInterface
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: setuptools
+Requires-Dist: pymavlink
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: flightdata>=0.2.6
 
 This project will contain an opinionated but tidy way to talk to a Drone through PyMavLink 
 using the PyFlightCoach Libraries
 
 
 #### Setup the connection:
 ```sh
```

### Comparing `droneinterface-0.0.3/droneinterface/__init__.py` & `droneinterface-0.0.4/droneinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface/combinators.py` & `droneinterface-0.0.4/droneinterface/combinators.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface/commands.py` & `droneinterface-0.0.4/droneinterface/commands.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface/connection.py` & `droneinterface-0.0.4/droneinterface/connection.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface/last_message.py` & `droneinterface-0.0.4/droneinterface/last_message.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface/vehicle.py` & `droneinterface-0.0.4/droneinterface/vehicle.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/droneinterface.egg-info/PKG-INFO` & `droneinterface-0.0.4/droneinterface.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: droneinterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tidy way to talk to a Drone through PyMavLink
 Home-page: https://github.com/PyFlightCoach/DroneInterface
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: setuptools
+Requires-Dist: pymavlink
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: flightdata>=0.2.6
 
 This project will contain an opinionated but tidy way to talk to a Drone through PyMavLink 
 using the PyFlightCoach Libraries
 
 
 #### Setup the connection:
 ```sh
```

### Comparing `droneinterface-0.0.3/readme.md` & `droneinterface-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/tests/test_last_message.py` & `droneinterface-0.0.4/tests/test_last_message.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/tests/test_vehicle.py` & `droneinterface-0.0.4/tests/test_vehicle.py`

 * *Files identical despite different names*

### Comparing `droneinterface-0.0.3/tests/test_wrappers.py` & `droneinterface-0.0.4/tests/test_wrappers.py`

 * *Files identical despite different names*

