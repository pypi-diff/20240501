# Comparing `tmp/pysma_plus-0.2.1.tar.gz` & `tmp/pysma_plus-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.1.tar", last modified: Wed May  1 08:48:05 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.1.1.tar", last modified: Wed May  1 08:57:25 2024, max compression
```

## Comparing `pysma_plus-0.2.1.tar` & `pysma_plus-0.2.1.1.tar`

### file list

```diff
@@ -1,30 +1,45 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-01 08:48:02.000000 pysma_plus-0.2.1/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      674 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/zip-safe
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-01 08:48:02.000000 pysma_plus-0.2.1/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.674802 pysma_plus-0.2.1/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.1/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.1/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:57:25.384355 pysma_plus-0.2.1.1/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3513 2024-05-01 08:57:25.384355 pysma_plus-0.2.1.1/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      897 2024-05-01 08:57:20.000000 pysma_plus-0.2.1.1/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:57:25.383355 pysma_plus-0.2.1.1/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3513 2024-05-01 08:57:25.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1046 2024-05-01 08:57:25.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:57:25.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 08:57:25.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-01 08:57:25.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1.1/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:57:25.382355 pysma_plus-0.2.1.1/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1439 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    18648 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9266 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21918 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    11597 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19897 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.1.1/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.1.1/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 08:57:25.384355 pysma_plus-0.2.1.1/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      760 2024-05-01 08:57:20.000000 pysma_plus-0.2.1.1/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:57:25.383355 pysma_plus-0.2.1.1/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.1.1/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.1.1/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:57:25.383355 pysma_plus-0.2.1.1/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.1.1/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.1/LICENSE` & `pysma_plus-0.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/PKG-INFO` & `pysma_plus-0.2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.1/README.md` & `pysma_plus-0.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/pyproject.toml` & `pysma_plus-0.2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.1"
+version = "0.2.1.1"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.1/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.1.1/pysma_plus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.1/setup.py` & `pysma_plus-0.2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.1"
+VERSION = "0.2.1.1"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.1/tests/__init__.py` & `pysma_plus-0.2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/test_definitions.py` & `pysma_plus-0.2.1.1/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/test_em.py` & `pysma_plus-0.2.1.1/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/test_ennexos.py` & `pysma_plus-0.2.1.1/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/test_sensor.py` & `pysma_plus-0.2.1.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/test_webconnect.py` & `pysma_plus-0.2.1.1/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.1.1/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.1.1/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.1.1/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.1.1/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.1/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.1.1/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

