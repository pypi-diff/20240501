# Comparing `tmp/pysma_plus-0.1.5.tar.gz` & `tmp/pysma_plus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.1.5.tar", last modified: Sun Apr 14 07:30:36 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.0.tar", last modified: Wed May  1 08:31:51 2024, max compression
```

## Comparing `pysma_plus-0.1.5.tar` & `pysma_plus-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma_plus-0.1.5/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma_plus-0.1.5/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma_plus-0.1.5/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-14 07:30:28.000000 pysma_plus-0.1.5/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.475540 pysma_plus-0.1.5/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      981 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma_plus-0.1.5/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.471540 pysma_plus-0.1.5/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1225 2024-04-10 13:24:27.000000 pysma_plus-0.1.5/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6009 2024-04-10 16:37:53.000000 pysma_plus-0.1.5/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-04-08 19:36:48.000000 pysma_plus-0.1.5/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    13616 2024-04-14 05:54:46.000000 pysma_plus-0.1.5/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-04-11 08:50:06.000000 pysma_plus-0.1.5/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-04-10 13:24:57.000000 pysma_plus-0.1.5/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-04-10 16:40:01.000000 pysma_plus-0.1.5/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    11551 2024-04-14 07:26:35.000000 pysma_plus-0.1.5/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-04-10 14:31:01.000000 pysma_plus-0.1.5/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma_plus-0.1.5/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma_plus-0.1.5/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-04-10 19:19:27.000000 pysma_plus-0.1.5/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-14 07:30:28.000000 pysma_plus-0.1.5/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.472540 pysma_plus-0.1.5/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-04-08 20:09:20.000000 pysma_plus-0.1.5/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-04-10 14:29:16.000000 pysma_plus-0.1.5/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-04-09 20:11:50.000000 pysma_plus-0.1.5/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-04-11 15:05:50.000000 pysma_plus-0.1.5/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma_plus-0.1.5/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-04-10 14:26:59.000000 pysma_plus-0.1.5/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-04-10 19:09:44.000000 pysma_plus-0.1.5/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.474540 pysma_plus-0.1.5/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-04-11 10:21:03.000000 pysma_plus-0.1.5/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-04-11 10:20:59.000000 pysma_plus-0.1.5/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-04-09 19:24:27.000000 pysma_plus-0.1.5/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-04-09 13:01:16.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-04-03 12:07:59.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-04-09 13:09:32.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma_plus-0.2.0/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma_plus-0.2.0/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-01 08:31:48.000000 pysma_plus-0.2.0/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      981 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma_plus-0.2.0/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.862770 pysma_plus-0.2.0/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1225 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6009 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-04-08 19:36:48.000000 pysma_plus-0.2.0/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    13616 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-04-11 08:50:06.000000 pysma_plus-0.2.0/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-04-10 13:24:57.000000 pysma_plus-0.2.0/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-04-10 16:40:01.000000 pysma_plus-0.2.0/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    11551 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-04-10 14:31:01.000000 pysma_plus-0.2.0/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma_plus-0.2.0/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma_plus-0.2.0/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-04-10 19:19:27.000000 pysma_plus-0.2.0/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-01 08:31:48.000000 pysma_plus-0.2.0/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.864770 pysma_plus-0.2.0/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-04-08 20:09:20.000000 pysma_plus-0.2.0/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-04-10 14:29:16.000000 pysma_plus-0.2.0/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-04-09 20:11:50.000000 pysma_plus-0.2.0/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-04-11 15:05:50.000000 pysma_plus-0.2.0/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma_plus-0.2.0/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-04-10 14:26:59.000000 pysma_plus-0.2.0/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-04-10 19:09:44.000000 pysma_plus-0.2.0/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.867770 pysma_plus-0.2.0/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-04-11 10:21:03.000000 pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-04-11 10:20:59.000000 pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-04-09 19:24:27.000000 pysma_plus-0.2.0/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-04-09 13:01:16.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-04-03 12:07:59.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-04-09 13:09:32.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.1.5/LICENSE` & `pysma_plus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/PKG-INFO` & `pysma_plus-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.5
+Version: 0.2.0
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.5
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.0
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma_plus-0.1.5/README.md` & `pysma_plus-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pyproject.toml` & `pysma_plus-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.1.5"
+version = "0.2.0"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.1.5/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.0/pysma_plus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.5
+Version: 0.2.0
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.5
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.0
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma_plus-0.1.5/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.0/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/__init__.py` & `pysma_plus-0.2.0/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/const.py` & `pysma_plus-0.2.0/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.0/pysmaplus/const_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.0/pysmaplus/definitions_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.0/pysmaplus/definitions_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/device.py` & `pysma_plus-0.2.0/pysmaplus/device.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/device_em.py` & `pysma_plus-0.2.0/pysmaplus/device_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.0/pysmaplus/device_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.0/pysmaplus/device_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/helpers.py` & `pysma_plus-0.2.0/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/pysmaplus/sensor.py` & `pysma_plus-0.2.0/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/setup.py` & `pysma_plus-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.1.5"
+VERSION = "0.2.0"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.1.5/tests/__init__.py` & `pysma_plus-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/test_definitions.py` & `pysma_plus-0.2.0/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/test_em.py` & `pysma_plus-0.2.0/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/test_ennexos.py` & `pysma_plus-0.2.0/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/test_sensor.py` & `pysma_plus-0.2.0/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/test_webconnect.py` & `pysma_plus-0.2.0/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.0/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.0/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.0/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.1.5/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.0/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

