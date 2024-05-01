# Comparing `tmp/pysma_plus-0.2.0.tar.gz` & `tmp/pysma_plus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.0.tar", last modified: Wed May  1 08:31:51 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.1.tar", last modified: Wed May  1 08:48:05 2024, max compression
```

## Comparing `pysma_plus-0.2.0.tar` & `pysma_plus-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,30 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma_plus-0.2.0/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma_plus-0.2.0/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-01 08:31:48.000000 pysma_plus-0.2.0/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      981 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-01 08:31:51.000000 pysma_plus-0.2.0/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma_plus-0.2.0/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.862770 pysma_plus-0.2.0/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1225 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6009 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-04-08 19:36:48.000000 pysma_plus-0.2.0/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    13616 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-04-11 08:50:06.000000 pysma_plus-0.2.0/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-04-10 13:24:57.000000 pysma_plus-0.2.0/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-04-10 16:40:01.000000 pysma_plus-0.2.0/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    11551 2024-05-01 08:30:27.000000 pysma_plus-0.2.0/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-04-10 14:31:01.000000 pysma_plus-0.2.0/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma_plus-0.2.0/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma_plus-0.2.0/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-04-10 19:19:27.000000 pysma_plus-0.2.0/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 08:31:51.870770 pysma_plus-0.2.0/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-01 08:31:48.000000 pysma_plus-0.2.0/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.864770 pysma_plus-0.2.0/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-04-08 20:09:20.000000 pysma_plus-0.2.0/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-04-10 14:29:16.000000 pysma_plus-0.2.0/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-04-09 20:11:50.000000 pysma_plus-0.2.0/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-04-11 15:05:50.000000 pysma_plus-0.2.0/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma_plus-0.2.0/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-04-10 14:26:59.000000 pysma_plus-0.2.0/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-04-10 19:09:44.000000 pysma_plus-0.2.0/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:31:51.867770 pysma_plus-0.2.0/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-04-11 10:21:03.000000 pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-04-11 10:20:59.000000 pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-04-09 19:24:27.000000 pysma_plus-0.2.0/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-04-09 13:01:16.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-04-03 12:07:59.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-04-09 13:09:32.000000 pysma_plus-0.2.0/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-05-01 08:48:02.000000 pysma_plus-0.2.1/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3509 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      674 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.1/pysma_plus.egg-info/zip-safe
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-01 08:48:02.000000 pysma_plus-0.2.1/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.674802 pysma_plus-0.2.1/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.1/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.1/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-01 08:48:05.675803 pysma_plus-0.2.1/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.1/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.0/LICENSE` & `pysma_plus-0.2.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+The webconnect Interface was created by kellerza.
+Later Engery-Meter and EnnexOS Support was added by little.yoda.
+Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
+was added to this Library and modified by little.yoda
+
 The MIT License (MIT)
 
 Copyright (c) 2016 kellerza
+Copyright (c) 2021 Garth Berry
+Copyright (c) 2024 little.yoda
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,7 +22,9 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+
```

### Comparing `pysma_plus-0.2.0/PKG-INFO` & `pysma_plus-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.0
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
-License: The MIT License (MIT)
+License: The webconnect Interface was created by kellerza.
+        Later Engery-Meter and EnnexOS Support was added by little.yoda.
+        Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
+        was added to this Library and modified by little.yoda
+        
+        The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
+        Copyright (c) 2021 Garth Berry
+        Copyright (c) 2024 little.yoda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -24,14 +31,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+        
+        
 Project-URL: Homepage, https://github.com/littleyoda/pysma
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pysma_plus-0.2.0/README.md` & `pysma_plus-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/pyproject.toml` & `pysma_plus-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.0/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.1/pysma_plus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.0
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.1
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
-License: The MIT License (MIT)
+License: The webconnect Interface was created by kellerza.
+        Later Engery-Meter and EnnexOS Support was added by little.yoda.
+        Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
+        was added to this Library and modified by little.yoda
+        
+        The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
+        Copyright (c) 2021 Garth Berry
+        Copyright (c) 2024 little.yoda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -24,14 +31,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+        
+        
 Project-URL: Homepage, https://github.com/littleyoda/pysma
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pysma_plus-0.2.0/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.1/pysma_plus.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,14 @@
 setup.py
 pysma_plus.egg-info/PKG-INFO
 pysma_plus.egg-info/SOURCES.txt
 pysma_plus.egg-info/dependency_links.txt
 pysma_plus.egg-info/requires.txt
 pysma_plus.egg-info/top_level.txt
 pysma_plus.egg-info/zip-safe
-pysmaplus/__init__.py
-pysmaplus/const.py
-pysmaplus/const_webconnect.py
-pysmaplus/definitions_ennexos.py
-pysmaplus/definitions_webconnect.py
-pysmaplus/device.py
-pysmaplus/device_em.py
-pysmaplus/device_ennexos.py
-pysmaplus/device_webconnect.py
-pysmaplus/exceptions.py
-pysmaplus/helpers.py
-pysmaplus/sensor.py
 tests/__init__.py
 tests/test_definitions.py
 tests/test_em.py
 tests/test_ennexos.py
 tests/test_helpers.py
 tests/test_sensor.py
 tests/test_webconnect.py
```

### Comparing `pysma_plus-0.2.0/setup.py` & `pysma_plus-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.0/tests/__init__.py` & `pysma_plus-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/test_definitions.py` & `pysma_plus-0.2.1/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/test_em.py` & `pysma_plus-0.2.1/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/test_ennexos.py` & `pysma_plus-0.2.1/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/test_sensor.py` & `pysma_plus-0.2.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/test_webconnect.py` & `pysma_plus-0.2.1/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.1/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.1/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.1/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.1/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.0/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.1/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*

