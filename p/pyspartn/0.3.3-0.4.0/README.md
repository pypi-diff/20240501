# Comparing `tmp/pyspartn-0.3.3.tar.gz` & `tmp/pyspartn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.3.3.tar", last modified: Tue Apr 30 06:32:39 2024, max compression
+gzip compressed data, was "pyspartn-0.4.0.tar", last modified: Wed May  1 09:03:42 2024, max compression
```

## Comparing `pyspartn-0.3.3.tar` & `pyspartn-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.909488 pyspartn-0.3.3/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.3.3/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.3.3/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    24126 2024-04-30 06:32:39.909196 pyspartn-0.3.3/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    20616 2024-04-30 06:27:38.000000 pyspartn-0.3.3/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-30 06:27:38.000000 pyspartn-0.3.3/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-30 06:32:39.909560 pyspartn-0.3.3/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.904943 pyspartn-0.3.3/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.906992 pyspartn-0.3.3/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     8957 2024-04-30 06:31:33.000000 pyspartn-0.3.3/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    18499 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    11595 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.3.3/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     9339 2024-04-29 14:57:05.000000 pyspartn-0.3.3/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    25860 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.908342 pyspartn-0.3.3/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    24126 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.908067 pyspartn-0.3.3/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.3.3/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     8670 2024-04-30 06:27:38.000000 pyspartn-0.3.3/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)   139331 2024-04-30 06:27:38.000000 pyspartn-0.3.3/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.523066 pyspartn-0.4.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.4.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.4.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24138 2024-05-01 09:03:42.522686 pyspartn-0.4.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    20628 2024-05-01 09:01:22.000000 pyspartn-0.4.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2446 2024-05-01 09:01:22.000000 pyspartn-0.4.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-01 09:03:42.523133 pyspartn-0.4.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.511465 pyspartn-0.4.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.514387 pyspartn-0.4.0/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.4.0/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     8987 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    18499 2024-04-30 06:27:38.000000 pyspartn-0.4.0/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)    11496 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.4.0/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     9370 2024-05-01 09:01:22.000000 pyspartn-0.4.0/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    25860 2024-04-30 06:27:38.000000 pyspartn-0.4.0/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.521522 pyspartn-0.4.0/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24138 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2024-05-01 09:03:42.000000 pyspartn-0.4.0/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-01 09:03:42.520675 pyspartn-0.4.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.4.0/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     8764 2024-05-01 09:01:22.000000 pyspartn-0.4.0/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   207798 2024-05-01 09:01:22.000000 pyspartn-0.4.0/tests/test_stream.py
```

### Comparing `pyspartn-0.3.3/LICENSE` & `pyspartn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/PKG-INFO` & `pyspartn-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.3
+Version: 0.4.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -209,15 +209,15 @@
 spr = SPARTNReader(stream)
 for (raw_data, parsed_data) in spr:
    print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
```

### Comparing `pyspartn-0.3.3/README.md` & `pyspartn-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 spr = SPARTNReader(stream)
 for (raw_data, parsed_data) in spr:
    print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
```

### Comparing `pyspartn-0.3.3/pyproject.toml` & `pyspartn-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "SPARTN protocol parser"
-version = "0.3.3"
+version = "0.4.0"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: MacOS X",
```

### Comparing `pyspartn-0.3.3/src/pyspartn/__init__.py` & `pyspartn-0.4.0/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn/exceptions.py` & `pyspartn-0.4.0/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn/socket_stream.py` & `pyspartn-0.4.0/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn/spartnhelpers.py` & `pyspartn-0.4.0/src/pyspartn/spartnhelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 # pylint: disable=invalid-name
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 from pyspartn.exceptions import SPARTNMessageError
 from pyspartn.spartntypes_core import FL, IN, SPARTN_DATA_FIELDS, TIMEBASE
 
 
@@ -241,15 +241,17 @@
     :returns: 32-bit gnssTimeTag
     :rtype: int
     """
 
     return int((date - TIMEBASE).total_seconds())
 
 
-def convert_timetag(timetag16: int, basedate: datetime = datetime.now()) -> int:
+def convert_timetag(
+    timetag16: int, basedate: datetime = datetime.now(timezone.utc)
+) -> int:
     """
     Convert 16-bit timetag to 32-bit format.
 
     32-bit timetag represents total seconds since 2010-01-01 00:00:00 (TIMEBASE).
 
     16-bit timetag represents seconds past 'base date' (the datetime the SPARTN
     message was originally sent, to the nearest half-day). It requires knowledge
```

### Comparing `pyspartn-0.3.3/src/pyspartn/spartnmessage.py` & `pyspartn-0.4.0/src/pyspartn/spartnmessage.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn/spartnreader.py` & `pyspartn-0.4.0/src/pyspartn/spartnreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 # pylint: disable=invalid-name too-many-instance-attributes
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from os import getenv
 from socket import socket
 
 from pyspartn.exceptions import (
     ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
@@ -72,15 +72,15 @@
     def __init__(
         self,
         datastream,
         validate: int = VALCRC,
         quitonerror: int = ERRLOG,
         decode: bool = False,
         key: str = None,
-        basedate: object = datetime.now(),
+        basedate: object = datetime.now(timezone.utc),
         bufsize: int = 4096,
         errorhandler: object = None,
     ):
         """Constructor.
 
         :param datastream stream: input data stream
         :param int validate: 0 = ignore invalid CRC, 1 = validate CRC (1)
@@ -102,22 +102,19 @@
         self._validate = validate
         self._quitonerror = quitonerror
         self._errorhandler = errorhandler
         self._decode = decode
         self._key = key
         # accumlated array of 32-bit gnssTimeTag from datastream
         self._timetags = {}
-        basedate = datetime.now() if basedate is None else basedate
+        basedate = datetime.now(timezone.utc) if basedate is None else basedate
         if isinstance(basedate, int):  # 32-bit gnssTimeTag
             self._basedate = timetag2date(basedate)
         else:  # datetime
             self._basedate = basedate
-        self._basedate = (
-            datetime.now() if basedate is None else basedate
-        )  # basedate for 16-bit gnssTimeTag
 
         if self._decode and self._key is None:
             raise ParameterError("Key must be provided if decoding is enabled")
 
     def __iter__(self):
         """Iterator."""
```

### Comparing `pyspartn-0.3.3/src/pyspartn/spartntables.py` & `pyspartn-0.4.0/src/pyspartn/spartntables.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn/spartntypes_core.py` & `pyspartn-0.4.0/src/pyspartn/spartntypes_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 (available in the public domain) © 2021 u-blox AG. All rights reserved.
 
 :author: semuadmin
 """
 
 # pylint: disable=line-too-long
 
-from datetime import datetime
+from datetime import datetime, timezone
 
-TIMEBASE = datetime(2010, 1, 1, 0, 0)
+TIMEBASE = datetime(2010, 1, 1, 0, 0, tzinfo=timezone.utc)
 ERRRAISE = 2
 ERRLOG = 1
 ERRIGNORE = 0
 VALNONE = 0
 VALCRC = 1
 VALMSGID = 2
 SPARTN_PRE = 0x73
```

### Comparing `pyspartn-0.3.3/src/pyspartn/spartntypes_get.py` & `pyspartn-0.4.0/src/pyspartn/spartntypes_get.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.4.0/src/pyspartn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.3
+Version: 0.4.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -209,15 +209,15 @@
 spr = SPARTNReader(stream)
 for (raw_data, parsed_data) in spr:
    print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
-Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now(timezone.utc)`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
 from serial import Serial
 from pyspartn import SPARTNReader
```

### Comparing `pyspartn-0.3.3/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.4.0/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/tests/test_socket.py` & `pyspartn-0.4.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.3/tests/test_static.py` & `pyspartn-0.4.0/tests/test_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 *** NB: must be saved in UTF-8 format ***
 
 @author: semuadmin
 """
 
 import os
 import unittest
-from datetime import datetime
+from datetime import datetime, timezone
 
 from pyspartn.exceptions import SPARTNMessageError
 from pyspartn.spartnhelpers import (
     att2idx,
     att2name,
     bitsval,
     convert_timetag,
@@ -126,20 +126,20 @@
         pt = decrypt(ct, key, iv, "CTR")
         self.assertEqual(msg, pt[0:-pad])
         ct, pad = encrypt(msg, key, iv, "CBC")
         pt = decrypt(ct, key, iv, "CBC")
         self.assertEqual(msg, pt[0:-pad])
 
     def testtimetag(self):
-        basedate_gps = datetime(2023, 6, 27, 23, 13, 0)
+        basedate_gps = datetime(2023, 6, 27, 23, 13, 0, tzinfo=timezone.utc)
         EXPECTED_RES_GPS = 425595780
         res = convert_timetag(32580, basedate_gps)
         self.assertEqual(res, EXPECTED_RES_GPS)
 
-        basedate_glo = datetime(2024, 4, 25, 11, 37, 0)
+        basedate_glo = datetime(2024, 4, 25, 11, 37, 0, tzinfo=timezone.utc)
         EXPECTED_RES_GLO = 451751822
         res = convert_timetag(9422, basedate_glo)
         self.assertEqual(res, EXPECTED_RES_GLO)
 
     def testiv(self):
         IV32 = "031800c03cb4306c2b40000000000001"
         IV16 = "001400c03cb4586c2580000000000001"
@@ -218,18 +218,18 @@
         res = enc2float(1332, 0.1, -90)
         self.assertAlmostEqual(res, 43.20000000000002, 6)
         res = enc2float(2033, 0.1, -180)
         self.assertAlmostEqual(res, 23.30000000000001, 6)
 
     def testtimetag2date(self):  # test timetag2date
         res = timetag2date(425595780)
-        self.assertEqual(res, datetime(2023, 6, 27, 21, 3, 0))
+        self.assertEqual(res, datetime(2023, 6, 27, 21, 3, 0, tzinfo=timezone.utc))
 
     def testdate2timetag(self):  # test date2timetag
-        res = date2timetag(datetime(2023, 6, 27, 21, 3, 0))
+        res = date2timetag(datetime(2023, 6, 27, 21, 3, 0, tzinfo=timezone.utc))
         self.assertEqual(res, 425595780)
 
     def testdatafields(self):  # check float datafields are correctly configured
         for _, value in SPARTN_DATA_FIELDS.items():
             if value[1] == FL:
                 self.assertTrue(
                     isinstance(value[3], (int, float))
```

### Comparing `pyspartn-0.3.3/tests/test_stream.py` & `pyspartn-0.4.0/tests/test_stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 @author: semuadmin
 """
 
 import os
 import sys
 import unittest
 from io import StringIO
-from datetime import datetime
+from datetime import datetime, timezone
 
 from pyspartn.exceptions import SPARTNMessageError, SPARTNParseError, ParameterError
 from pyspartn.spartnreader import SPARTNReader, SPARTNMessage
 from pyspartn.spartntypes_core import ERRRAISE, ERRIGNORE, ERRLOG
 
 SPARTN_KEY = "930d847b779b126863c8b3b2766ae7cc"
-SPARTN_BASEDATE = datetime(2024, 4, 18, 20, 48, 29, 977255)
+SPARTN_BASEDATE = datetime(2024, 4, 18, 20, 48, 29, 977255, tzinfo=timezone.utc)
 
 
 class StreamTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         self.dirname = os.path.dirname(__file__)
         self.streamSPARTN = open(os.path.join(self.dirname, "spartn_mqtt.log"), "rb")
@@ -319,15 +319,15 @@
             "rb",
         ) as stream:
             spr = SPARTNReader(
                 stream,
                 quitonerror=ERRRAISE,
                 decode=True,
                 key="930d847b779b126863c8b3b2766ae7cc",
-                basedate=datetime(2024, 4, 28, 23, 50, 40),
+                basedate=datetime(2024, 4, 28, 23, 50, 40, tzinfo=timezone.utc),
             )
 
             for raw, parsed in spr:
                 i += 1
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertTrue(0 <= parsed._padding <= 8)
@@ -354,11 +354,50 @@
                 i += 1
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertTrue(0 <= parsed._padding <= 8)
 
         self.assertEqual(i, 99)
 
+    def testspartnntrip(
+        self,
+    ):  # test decryption of datastream from SPARTN NTRIP caster containing unencrypted messages (eaf=0)
+        EXPECTED_RESULT = [
+            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=369, eaf=0, crcType=2, frameCrc=14, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=4347676, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF094_01=32768, SF055_01_01=1, SF056_01_01=1, SF060_01_01=8.960000000000036, SF061a_01_01=0.1599999999999966, SF061b_01_01=0.3999999999999915, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, SF055_02_01=3, SF056_02_01=1, SF060_02_01=9.800000000000011, SF061a_02_01=-0.38400000000000034, SF061b_02_01=-0.4399999999999977, SF055_02_02=4, SF056_02_02=1, SF060_02_02=28.480000000000018, SF061a_02_02=-0.4720000000000084, SF061b_02_02=0.37599999999999056, SF055_02_03=3, SF056_02_03=1, SF060_02_03=3.5200000000000387, SF061a_02_03=-0.24800000000000466, SF061b_02_03=0.0799999999999983, SF055_02_04=4, SF056_02_04=1, SF060_02_04=27.640000000000043, SF061a_02_04=-1.0080000000000098, SF061b_02_04=0.3359999999999985, SF055_02_05=2, SF056_02_05=1, SF060_02_05=22.319999999999993, SF061a_02_05=0.37599999999999056, SF061b_02_05=-0.6080000000000041, SF055_02_06=4, SF056_02_06=1, SF060_02_06=15.760000000000048, SF061a_02_06=0.1039999999999992, SF061b_02_06=0.22399999999998954, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=1, SF094_03=184550404, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.28000000000003, SF061a_03_01=-0.4480000000000075, SF061b_03_01=-0.26400000000001, SF055_03_02=5, SF056_03_02=1, SF060_03_02=30.52000000000004, SF061a_03_02=0.07199999999998852, SF061b_03_02=0.30400000000000205, SF055_03_03=1, SF056_03_03=1, SF060_03_03=3.5600000000000023, SF061a_03_03=-0.0799999999999983, SF061b_03_03=-0.03200000000001069, SF055_03_04=2, SF056_03_04=1, SF060_03_04=17.319999999999993, SF061a_03_04=0.30400000000000205, SF061b_03_04=-0.6159999999999997, SF055_03_05=1, SF056_03_05=1, SF060_03_05=17.760000000000048, SF061a_03_05=0.28000000000000114, SF061b_03_05=0.3359999999999985, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=1, SF094_04=50335748, SF055_04_01=4, SF056_04_01=1, SF060_04_01=28.08000000000004, SF061a_04_01=0.02400000000000091, SF061b_04_01=-1.784000000000006, SF055_04_02=4, SF056_04_02=1, SF060_04_02=13.480000000000018, SF061a_04_02=0.35199999999998965, SF061b_04_02=-2.3600000000000065, SF055_04_03=5, SF056_04_03=1, SF060_04_03=32.160000000000025, SF061a_04_03=-0.2560000000000002, SF061b_04_03=-1.7360000000000042, SF055_04_04=4, SF056_04_04=1, SF060_04_04=20.480000000000018, SF061a_04_04=0.5519999999999925, SF061b_04_04=-1.9680000000000035, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=1, SF094_05=50335748, SF055_05_01=1, SF056_05_01=1, SF060_05_01=19.439999999999998, SF061a_05_01=1.3119999999999976, SF061b_05_01=-0.35999999999999943, SF055_05_02=1, SF056_05_02=1, SF060_05_02=3.080000000000041, SF061a_05_02=1.583999999999989, SF061b_05_02=-0.9680000000000035, SF055_05_03=4, SF056_05_03=1, SF060_05_03=23.760000000000048, SF061a_05_03=0.8239999999999981, SF061b_05_03=-0.48799999999999955, SF055_05_04=3, SF056_05_04=1, SF060_05_04=10.720000000000027, SF061a_05_04=1.7920000000000016, SF061b_05_04=-0.7120000000000033, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF094_06=98304, SF055_06_01=5, SF056_06_01=1, SF060_06_01=32.44, SF061a_06_01=-0.0799999999999983, SF061b_06_01=0.5759999999999934, SF055_06_02=1, SF056_06_02=1, SF060_06_02=8.640000000000043, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.24799999999999045, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=1, SF094_07=184550404, SF055_07_01=1, SF056_07_01=1, SF060_07_01=12.04000000000002, SF061a_07_01=1.0959999999999894, SF061b_07_01=-0.2400000000000091, SF055_07_02=1, SF056_07_02=1, SF060_07_02=32.04000000000002, SF061a_07_02=0.5919999999999987, SF061b_07_02=0.6400000000000006, SF055_07_03=1, SF056_07_03=1, SF060_07_03=6.240000000000009, SF061a_07_03=1.2719999999999914, SF061b_07_03=0.19999999999998863, SF055_07_04=4, SF056_07_04=1, SF060_07_04=21.640000000000043, SF061a_07_04=1.176000000000002, SF061b_07_04=0.14399999999999125, SF055_07_05=2, SF056_07_05=1, SF060_07_05=18.480000000000018, SF061a_07_05=1.3519999999999897, SF061b_07_05=0.15200000000000102, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=1, SF094_08=184550404, SF055_08_01=2, SF056_08_01=1, SF060_08_01=11.520000000000039, SF061a_08_01=1.024000000000001, SF061b_08_01=0.015999999999991132, SF055_08_02=2, SF056_08_02=1, SF060_08_02=35.879999999999995, SF061a_08_02=0.5360000000000014, SF061b_08_02=0.9119999999999919, SF055_08_03=2, SF056_08_03=1, SF060_08_03=7.160000000000025, SF061a_08_03=1.1039999999999992, SF061b_08_03=0.16799999999999216, SF055_08_04=4, SF056_08_04=1, SF060_08_04=20.480000000000018, SF061a_08_04=0.7599999999999909, SF061b_08_04=-0.6480000000000103, SF055_08_05=1, SF056_08_05=1, SF060_08_05=20.04000000000002, SF061a_08_05=1.5360000000000014, SF061b_08_05=0.5600000000000023, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF094_09=98304, SF055_09_01=3, SF056_09_01=1, SF060_09_01=34.04000000000002, SF061a_09_01=-0.2960000000000065, SF061b_09_01=0.21599999999999397, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.840000000000032, SF061a_09_02=0.32799999999998875, SF061b_09_02=0.30400000000000205, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=1, SF094_10=184550404, SF055_10_01=1, SF056_10_01=1, SF060_10_01=7.8799999999999955, SF061a_10_01=1.2800000000000011, SF061b_10_01=0.08799999999999386, SF055_10_02=1, SF056_10_02=1, SF060_10_02=30.200000000000045, SF061a_10_02=1.063999999999993, SF061b_10_02=0.9119999999999919, SF055_10_03=1, SF056_10_03=1, SF060_10_03=2.0400000000000205, SF061a_10_03=1.2959999999999923, SF061b_10_03=0.4159999999999968, SF055_10_04=1, SF056_10_04=1, SF060_10_04=16.0, SF061a_10_04=1.519999999999996, SF061b_10_04=-0.6800000000000068, SF055_10_05=1, SF056_10_05=1, SF060_10_05=14.400000000000034, SF061a_10_05=1.2079999999999984, SF061b_10_05=0.5039999999999907)>",
+            "<SPARTN(SPARTN-1X-HPAC-BEI, msgType=1, nData=101, eaf=0, crcType=2, frameCrc=7, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=3165361, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=1, SF094_01=184554500, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-9.680000000000007, SF061a_01_01=-0.7920000000000016, SF061b_01_01=-0.5679999999999978, SF055_01_02=2, SF056_01_02=1, SF060_01_02=15.560000000000002, SF061a_01_02=-0.5120000000000005, SF061b_01_02=0.1839999999999975, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-12.079999999999984, SF061a_01_03=-0.43200000000000216, SF061b_01_03=-0.24800000000000466, SF055_01_04=3, SF056_01_04=1, SF060_01_04=10.360000000000014, SF061a_01_04=-1.5360000000000014, SF061b_01_04=-0.1600000000000108, SF055_01_05=1, SF056_01_05=1, SF060_01_05=5.1200000000000045, SF061a_01_05=0.27199999999999136, SF061b_01_05=-0.8640000000000043, SF055_01_06=1, SF056_01_06=1, SF060_01_06=3.8799999999999955, SF061a_01_06=-0.06400000000000716, SF061b_01_06=0.1599999999999966, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=1, SF094_02=184554500, SF055_02_01=1, SF056_02_01=1, SF060_02_01=-11.560000000000002, SF061a_02_01=-0.632000000000005, SF061b_02_01=-0.5440000000000111, SF055_02_02=3, SF056_02_02=1, SF060_02_02=14.360000000000014, SF061a_02_02=-0.6400000000000006, SF061b_02_02=0.16799999999999216, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-13.239999999999952, SF061a_02_03=-0.45600000000000307, SF061b_02_03=-0.2880000000000109, SF055_02_04=2, SF056_02_04=1, SF060_02_04=7.0, SF061a_02_04=-1.4639999999999986, SF061b_02_04=-0.08800000000000807, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.8799999999999955, SF061a_02_05=-0.008000000000009777, SF061b_02_05=-0.847999999999999, SF055_02_06=1, SF056_02_06=1, SF060_02_06=3.7200000000000273, SF061a_02_06=-0.1600000000000108, SF061b_02_06=0.1039999999999992)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=536, eaf=0, crcType=2, frameCrc=14, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=4199949, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.15200000000000002, SF049a_01=-0.0020000000000000018, SF049b_01=-0.0040000000000000036, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412539457, SF055_01_01=1, SF056_01_01=1, SF060_01_01=3.160000000000025, SF061a_01_01=0.43200000000000216, SF061b_01_01=0.1599999999999966, SF055_01_02=2, SF056_01_02=1, SF060_01_02=0.6800000000000068, SF061a_01_02=0.19199999999999307, SF061b_01_02=0.08799999999999386, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-0.7999999999999545, SF061a_01_03=1.0480000000000018, SF061b_01_03=0.1039999999999992, SF055_01_04=1, SF056_01_04=1, SF060_01_04=7.360000000000014, SF061a_01_04=1.4959999999999951, SF061b_01_04=-0.1360000000000099, SF055_01_05=3, SF056_01_05=1, SF060_01_05=-0.3599999999999568, SF061a_01_05=0.23999999999999488, SF061b_01_05=-0.1600000000000108, SF055_01_06=4, SF056_01_06=1, SF060_01_06=17.04000000000002, SF061a_01_06=-0.38400000000000034, SF061b_01_06=-0.6240000000000094, SF055_01_07=4, SF056_01_07=1, SF060_01_07=24.80000000000001, SF061a_01_07=-1.0480000000000018, SF061b_01_07=-0.32800000000000296, SF055_01_08=4, SF056_01_08=1, SF060_01_08=13.680000000000007, SF061a_01_08=0.847999999999999, SF061b_01_08=0.4479999999999933, SF031_02=1, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0, SF044_02=1, SF048_02=-0.128, SF049a_02=0.0010000000000000009, SF049b_02=-0.0030000000000000027, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412539457, SF055_02_01=5, SF056_02_01=1, SF060_02_01=-1.2399999999999523, SF061a_02_01=2.3359999999999985, SF061b_02_01=0.0, SF055_02_02=4, SF056_02_02=1, SF060_02_02=-2.839999999999975, SF061a_02_02=2.128, SF061b_02_02=-0.1600000000000108, SF055_02_03=4, SF056_02_03=1, SF060_02_03=-3.7199999999999704, SF061a_02_03=0.2079999999999984, SF061b_02_03=0.14399999999999125, SF055_02_04=5, SF056_02_04=1, SF060_02_04=2.4399999999999977, SF061a_02_04=2.304000000000002, SF061b_02_04=-0.35999999999999943, SF055_02_05=4, SF056_02_05=1, SF060_02_05=-1.5600000000000023, SF061a_02_05=0.4959999999999951, SF061b_02_05=-0.04800000000000182, SF055_02_06=1, SF056_02_06=1, SF060_02_06=20.400000000000034, SF061a_02_06=0.14399999999999125, SF061b_02_06=-0.35200000000000387, SF055_02_07=5, SF056_02_07=1, SF060_02_07=27.120000000000005, SF061a_02_07=0.19999999999998863, SF061b_02_07=0.04800000000000182, SF055_02_08=4, SF056_02_08=1, SF060_02_08=10.680000000000007, SF061a_02_08=0.19199999999999307, SF061b_02_08=0.3999999999999915, SF031_03=2, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=1, SF043_03=0.0, SF044_03=1, SF048_03=-0.14800000000000002, SF049a_03=-0.015000000000000013, SF049b_03=0.0010000000000000009, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412539457, SF055_03_01=5, SF056_03_01=1, SF060_03_01=-0.5600000000000023, SF061a_03_01=2.7039999999999935, SF061b_03_01=0.0799999999999983, SF055_03_02=5, SF056_03_02=1, SF060_03_02=-2.0399999999999636, SF061a_03_02=2.1999999999999886, SF061b_03_02=0.08799999999999386, SF055_03_03=4, SF056_03_03=1, SF060_03_03=-1.3999999999999773, SF061a_03_03=0.1039999999999992, SF061b_03_03=0.03999999999999204, SF055_03_04=5, SF056_03_04=1, SF060_03_04=1.6400000000000432, SF061a_03_04=1.3119999999999976, SF061b_03_04=-0.03200000000001069, SF055_03_05=5, SF056_03_05=1, SF060_03_05=-2.0, SF061a_03_05=0.27199999999999136, SF061b_03_05=-0.08800000000000807, SF055_03_06=4, SF056_03_06=1, SF060_03_06=14.400000000000034, SF061a_03_06=0.2879999999999967, SF061b_03_06=-0.7680000000000007, SF055_03_07=4, SF056_03_07=1, SF060_03_07=26.80000000000001, SF061a_03_07=-0.7280000000000086, SF061b_03_07=-0.2079999999999984, SF055_03_08=1, SF056_03_08=1, SF060_03_08=13.760000000000048, SF061a_03_08=0.07199999999998852, SF061b_03_08=0.367999999999995, SF031_04=3, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.0, SF044_04=1, SF048_04=-0.124, SF049a_04=0.0030000000000000027, SF049b_04=-0.0010000000000000009, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412539457, SF055_04_01=4, SF056_04_01=1, SF060_04_01=1.3600000000000136, SF061a_04_01=-1.480000000000004, SF061b_04_01=0.2079999999999984, SF055_04_02=4, SF056_04_02=1, SF060_04_02=-1.599999999999966, SF061a_04_02=-1.328000000000003, SF061b_04_02=0.24799999999999045, SF055_04_03=4, SF056_04_03=1, SF060_04_03=-4.359999999999957, SF061a_04_03=2.7920000000000016, SF061b_04_03=0.3359999999999985, SF055_04_04=4, SF056_04_04=1, SF060_04_04=9.920000000000016, SF061a_04_04=0.1039999999999992, SF061b_04_04=0.15200000000000102, SF055_04_05=4, SF056_04_05=1, SF060_04_05=-0.9199999999999591, SF061a_04_05=3.1119999999999948, SF061b_04_05=0.0799999999999983, SF055_04_06=5, SF056_04_06=1, SF060_04_06=27.80000000000001, SF061a_04_06=1.3199999999999932, SF061b_04_06=-0.784000000000006, SF055_04_07=5, SF056_04_07=1, SF060_04_07=29.439999999999998, SF061a_04_07=0.4959999999999951, SF061b_04_07=0.8399999999999892, SF055_04_08=3, SF056_04_08=1, SF060_04_08=11.879999999999995, SF061a_04_08=1.1359999999999957, SF061b_04_08=0.5999999999999943, SF031_05=4, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.0, SF044_05=1, SF048_05=-0.14, SF049a_05=0.0020000000000000018, SF049b_05=-0.0010000000000000009, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412539457, SF055_05_01=4, SF056_05_01=1, SF060_05_01=6.1200000000000045, SF061a_05_01=-0.1039999999999992, SF061b_05_01=0.37599999999999056, SF055_05_02=5, SF056_05_02=1, SF060_05_02=1.4399999999999977, SF061a_05_02=-1.6720000000000041, SF061b_05_02=0.21599999999999397, SF055_05_03=4, SF056_05_03=1, SF060_05_03=0.040000000000020464, SF061a_05_03=2.5519999999999925, SF061b_05_03=0.4239999999999924, SF055_05_04=2, SF056_05_04=1, SF060_05_04=10.319999999999993, SF061a_05_04=0.46399999999999864, SF061b_05_04=0.04800000000000182, SF055_05_05=3, SF056_05_05=1, SF060_05_05=1.0, SF061a_05_05=3.087999999999994, SF061b_05_05=0.24799999999999045, SF055_05_06=5, SF056_05_06=1, SF060_05_06=20.720000000000027, SF061a_05_06=1.3599999999999994, SF061b_05_06=-0.2560000000000002, SF055_05_07=4, SF056_05_07=1, SF060_05_07=35.0, SF061a_05_07=0.4719999999999942, SF061b_05_07=0.367999999999995, SF055_05_08=3, SF056_05_08=1, SF060_05_08=20.28000000000003, SF061a_05_08=1.5360000000000014, SF061b_05_08=0.6239999999999952, SF031_06=5, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.0, SF044_06=1, SF048_06=-0.08799999999999997, SF049a_06=-0.01899999999999999, SF049b_06=-0.0020000000000000018, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538881, SF055_06_01=2, SF056_06_01=1, SF060_06_01=5.600000000000023, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.28000000000000114, SF055_06_02=3, SF056_06_02=1, SF060_06_02=3.2000000000000455, SF061a_06_02=0.24799999999999045, SF061b_06_02=0.29599999999999227, SF055_06_03=4, SF056_06_03=1, SF060_06_03=0.20000000000004547, SF061a_06_03=-0.7439999999999998, SF061b_06_03=0.35999999999999943, SF055_06_04=2, SF056_06_04=1, SF060_06_04=12.360000000000014, SF061a_06_04=0.2639999999999958, SF061b_06_04=-0.02400000000000091, SF055_06_05=4, SF056_06_05=1, SF060_06_05=0.5600000000000023, SF061a_06_05=-1.720000000000006, SF061b_06_05=0.23999999999999488, SF055_06_06=4, SF056_06_06=1, SF060_06_06=8.720000000000027, SF061a_06_06=1.2239999999999895, SF061b_06_06=0.43200000000000216, SF031_07=6, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.0, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=-0.015999999999999986, SF049b_07=-0.006000000000000005, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538881, SF055_07_01=3, SF056_07_01=1, SF060_07_01=7.319999999999993, SF061a_07_01=-0.03200000000001069, SF061b_07_01=0.19999999999998863, SF055_07_02=1, SF056_07_02=1, SF060_07_02=5.0, SF061a_07_02=0.11999999999999034, SF061b_07_02=0.24799999999999045, SF055_07_03=2, SF056_07_03=1, SF060_07_03=2.2000000000000455, SF061a_07_03=-0.480000000000004, SF061b_07_03=0.3359999999999985, SF055_07_04=1, SF056_07_04=1, SF060_07_04=12.760000000000048, SF061a_07_04=0.13599999999999568, SF061b_07_04=0.055999999999997385, SF055_07_05=2, SF056_07_05=1, SF060_07_05=2.080000000000041, SF061a_07_05=-0.9920000000000044, SF061b_07_05=0.015999999999991132, SF055_07_06=4, SF056_07_06=1, SF060_07_06=13.160000000000025, SF061a_07_06=0.9919999999999902, SF061b_07_06=0.6319999999999908, SF031_08=7, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.0, SF044_08=1, SF048_08=-0.14, SF049a_08=-0.023999999999999994, SF049b_08=-0.0010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=117571585, SF055_08_01=3, SF056_08_01=1, SF060_08_01=-8.839999999999975, SF061a_08_01=-0.7199999999999989, SF061b_08_01=-0.23199999999999932, SF055_08_02=4, SF056_08_02=1, SF060_08_02=-10.759999999999991, SF061a_08_02=-1.5520000000000067, SF061b_08_02=-0.1039999999999992, SF055_08_03=1, SF056_08_03=1, SF060_08_03=-2.8799999999999955, SF061a_08_03=-0.4960000000000093, SF061b_08_03=-0.3760000000000048, SF055_08_04=4, SF056_08_04=1, SF060_08_04=-12.479999999999961, SF061a_08_04=-1.240000000000009, SF061b_08_04=-0.1839999999999975, SF055_08_05=2, SF056_08_05=1, SF060_08_05=4.360000000000014, SF061a_08_05=0.5919999999999987, SF061b_08_05=0.3359999999999985, SF031_09=8, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.0040000000000000036, SF044_09=1, SF048_09=-0.14400000000000002, SF049a_09=0.0010000000000000009, SF049b_09=0.0, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.400000000000034, SF061a_09_01=-0.2400000000000091, SF061b_09_01=0.09599999999998943, SF055_09_02=2, SF056_09_02=1, SF060_09_02=11.520000000000039, SF061a_09_02=-0.35200000000000387, SF061b_09_02=-0.016000000000005343, SF055_09_03=1, SF056_09_03=1, SF060_09_03=8.0, SF061a_09_03=-0.5440000000000111, SF061b_09_03=0.14399999999999125, SF055_09_04=2, SF056_09_04=1, SF060_09_04=22.640000000000043, SF061a_09_04=-0.08800000000000807, SF061b_09_04=-0.2880000000000109, SF055_09_05=2, SF056_09_05=1, SF060_09_05=11.640000000000043, SF061a_09_05=-1.4000000000000057, SF061b_09_05=-0.1600000000000108, SF055_09_06=4, SF056_09_06=1, SF060_09_06=20.0, SF061a_09_06=-3.8160000000000025, SF061b_09_06=0.015999999999991132, SF031_10=9, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=1, SF043_10=0.0040000000000000036, SF044_10=1, SF048_10=-0.09199999999999997, SF049a_10=0.007000000000000006, SF049b_10=-0.0010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538881, SF055_10_01=2, SF056_10_01=1, SF060_10_01=9.160000000000025, SF061a_10_01=-0.30400000000000205, SF061b_10_01=-0.17600000000000193, SF055_10_02=2, SF056_10_02=1, SF060_10_02=6.720000000000027, SF061a_10_02=-0.4960000000000093, SF061b_10_02=-0.20000000000000284, SF055_10_03=2, SF056_10_03=1, SF060_10_03=4.8799999999999955, SF061a_10_03=-0.6159999999999997, SF061b_10_03=-0.15200000000000102, SF055_10_04=2, SF056_10_04=1, SF060_10_04=14.240000000000009, SF061a_10_04=0.031999999999996476, SF061b_10_04=-0.416000000000011, SF055_10_05=1, SF056_10_05=1, SF060_10_05=5.800000000000011, SF061a_10_05=-0.7120000000000033, SF061b_10_05=-0.38400000000000034, SF055_10_06=2, SF056_10_06=1, SF060_10_06=17.24000000000001, SF061a_10_06=-2.896000000000008, SF061b_10_06=-0.3119999999999976)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=465, eaf=0, crcType=2, frameCrc=0, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=8229442, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=10, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.0040000000000000036, SF044_01=1, SF048_01=-0.11199999999999999, SF049a_01=0.016000000000000014, SF049b_01=-0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538881, SF055_01_01=3, SF056_01_01=1, SF060_01_01=-2.5600000000000023, SF061a_01_01=-0.8719999999999999, SF061b_01_01=-0.14400000000000546, SF055_01_02=2, SF056_01_02=1, SF060_01_02=-5.639999999999986, SF061a_01_02=-0.7520000000000095, SF061b_01_02=-0.21600000000000819, SF055_01_03=4, SF056_01_03=1, SF060_01_03=-6.0, SF061a_01_03=-0.9519999999999982, SF061b_01_03=-0.09600000000000364, SF055_01_04=1, SF056_01_04=1, SF060_01_04=-0.4399999999999977, SF061a_01_04=-0.5600000000000023, SF061b_01_04=-0.35200000000000387, SF055_01_05=2, SF056_01_05=1, SF060_01_05=-8.599999999999966, SF061a_01_05=-0.8320000000000078, SF061b_01_05=-0.3119999999999976, SF055_01_06=5, SF056_01_06=1, SF060_01_06=5.720000000000027, SF061a_01_06=-1.6640000000000015, SF061b_01_06=0.35199999999998965, SF031_02=11, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.0040000000000000036, SF044_02=1, SF048_02=-0.18799999999999994, SF049a_02=0.013000000000000012, SF049b_02=-0.0050000000000000044, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538881, SF055_02_01=2, SF056_02_01=1, SF060_02_01=14.319999999999993, SF061a_02_01=-0.3440000000000083, SF061b_02_01=0.03999999999999204, SF055_02_02=2, SF056_02_02=1, SF060_02_02=13.080000000000041, SF061a_02_02=-0.416000000000011, SF061b_02_02=0.055999999999997385, SF055_02_03=1, SF056_02_03=1, SF060_02_03=9.840000000000032, SF061a_02_03=-0.5600000000000023, SF061b_02_03=0.14399999999999125, SF055_02_04=2, SF056_02_04=1, SF060_02_04=24.319999999999993, SF061a_02_04=-0.3680000000000092, SF061b_02_04=-0.2560000000000002, SF055_02_05=1, SF056_02_05=1, SF060_02_05=18.0, SF061a_02_05=-1.2319999999999993, SF061b_02_05=-0.20000000000000284, SF055_02_06=5, SF056_02_06=1, SF060_02_06=31.80000000000001, SF061a_02_06=-1.9920000000000044, SF061b_02_06=0.06399999999999295, SF031_03=12, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.008000000000000007, SF044_03=1, SF048_03=-0.14, SF049a_03=0.008000000000000007, SF049b_03=0.016000000000000014, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4378984449, SF055_03_01=5, SF056_03_01=1, SF060_03_01=13.960000000000036, SF061a_03_01=0.43200000000000216, SF061b_03_01=0.43200000000000216, SF055_03_02=5, SF056_03_02=1, SF060_03_02=12.439999999999998, SF061a_03_02=0.19999999999998863, SF061b_03_02=0.40800000000000125, SF055_03_03=3, SF056_03_03=1, SF060_03_03=22.80000000000001, SF061a_03_03=-0.43200000000000216, SF061b_03_03=-0.2560000000000002, SF055_03_04=3, SF056_03_04=1, SF060_03_04=16.160000000000025, SF061a_03_04=-1.2240000000000038, SF061b_03_04=-0.3920000000000101, SF055_03_05=4, SF056_03_05=1, SF060_03_05=33.04000000000002, SF061a_03_05=-2.5120000000000076, SF061b_03_05=0.055999999999997385, SF031_04=13, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=1, SF043_04=0.008000000000000007, SF044_04=1, SF048_04=-0.09599999999999997, SF049a_04=0.0020000000000000018, SF049b_04=-0.0030000000000000027, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, SF055_04_01=1, SF056_04_01=1, SF060_04_01=11.080000000000041, SF061a_04_01=-0.3680000000000092, SF061b_04_01=-0.16800000000000637, SF055_04_02=1, SF056_04_02=1, SF060_04_02=9.200000000000045, SF061a_04_02=-0.4399999999999977, SF061b_04_02=-0.20000000000000284, SF055_04_03=2, SF056_04_03=1, SF060_04_03=7.560000000000002, SF061a_04_03=-0.5760000000000076, SF061b_04_03=-0.08800000000000807, SF055_04_04=1, SF056_04_04=1, SF060_04_04=16.80000000000001, SF061a_04_04=-0.0799999999999983, SF061b_04_04=-0.480000000000004, SF055_04_05=2, SF056_04_05=1, SF060_04_05=10.600000000000023, SF061a_04_05=-0.8719999999999999, SF061b_04_05=-0.3440000000000083, SF055_04_06=4, SF056_04_06=1, SF060_04_06=28.879999999999995, SF061a_04_06=-2.608000000000004, SF061b_04_06=-0.5600000000000023, SF031_05=14, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=1, SF043_05=0.008000000000000007, SF044_05=1, SF048_05=-0.12, SF049a_05=0.006000000000000005, SF049b_05=0.0, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, SF055_05_01=4, SF056_05_01=1, SF060_05_01=10.28000000000003, SF061a_05_01=-0.43200000000000216, SF061b_05_01=-0.16800000000000637, SF055_05_02=2, SF056_05_02=1, SF060_05_02=7.960000000000036, SF061a_05_02=-0.2960000000000065, SF061b_05_02=-0.2079999999999984, SF055_05_03=1, SF056_05_03=1, SF060_05_03=6.8799999999999955, SF061a_05_03=-0.6000000000000085, SF061b_05_03=-0.09600000000000364, SF055_05_04=1, SF056_05_04=1, SF060_05_04=13.920000000000016, SF061a_05_04=-0.03200000000001069, SF061b_05_04=-0.4720000000000084, SF055_05_05=1, SF056_05_05=1, SF060_05_05=8.0, SF061a_05_05=-0.8400000000000034, SF061b_05_05=-0.5919999999999987, SF055_05_06=4, SF056_05_06=1, SF060_05_06=25.879999999999995, SF061a_05_06=-2.6400000000000077, SF061b_05_06=-0.6240000000000094, SF031_06=15, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.008000000000000007, SF044_06=1, SF048_06=-0.15200000000000002, SF049a_06=0.009000000000000008, SF049b_06=-0.007000000000000006, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, SF055_06_01=1, SF056_06_01=1, SF060_06_01=7.28000000000003, SF061a_06_01=0.14399999999999125, SF061b_06_01=0.3199999999999932, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.400000000000034, SF061a_06_02=0.09599999999998943, SF061b_06_02=0.21599999999999397, SF055_06_03=2, SF056_06_03=1, SF060_06_03=4.160000000000025, SF061a_06_03=-0.35999999999999943, SF061b_06_03=0.38400000000000034, SF055_06_04=2, SF056_06_04=1, SF060_06_04=9.120000000000005, SF061a_06_04=0.35199999999998965, SF061b_06_04=0.16799999999999216, SF055_06_05=2, SF056_06_05=1, SF060_06_05=2.319999999999993, SF061a_06_05=-0.19200000000000728, SF061b_06_05=0.04800000000000182, SF031_07=16, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=1, SF043_07=0.008000000000000007, SF044_07=1, SF048_07=-0.15200000000000002, SF049a_07=0.0020000000000000018, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4546756608, SF055_07_01=1, SF056_07_01=1, SF060_07_01=19.439999999999998, SF061a_07_01=-1.024000000000001, SF061b_07_01=-0.6480000000000103, SF055_07_02=4, SF056_07_02=1, SF060_07_02=62.24000000000001, SF061a_07_02=0.22399999999998954, SF061b_07_02=-0.20000000000000284, SF055_07_03=1, SF056_07_03=1, SF060_07_03=18.08000000000004, SF061a_07_03=-1.1039999999999992, SF061b_07_03=-0.6720000000000113, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.920000000000016, SF061a_07_04=-1.240000000000009, SF061b_07_04=-0.4480000000000075, SF055_07_05=1, SF056_07_05=1, SF060_07_05=27.480000000000018, SF061a_07_05=-0.8800000000000097, SF061b_07_05=-0.9840000000000089, SF055_07_06=1, SF056_07_06=1, SF060_07_06=23.360000000000014, SF061a_07_06=-1.6800000000000068, SF061b_07_06=-1.0, SF031_08=17, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=2, SF043_08=0.008000000000000007, SF044_08=1, SF048_08=-0.11599999999999999, SF049a_08=-0.0040000000000000036, SF049b_08=0.006000000000000005, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4546756608, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.120000000000005, SF061a_08_01=-0.9519999999999982, SF061b_08_01=-0.6159999999999997, SF055_08_02=1, SF056_08_02=1, SF060_08_02=59.960000000000036, SF061a_08_02=0.28000000000000114, SF061b_08_02=-0.3760000000000048, SF055_08_03=1, SF056_08_03=1, SF060_08_03=13.640000000000043, SF061a_08_03=-0.9519999999999982, SF061b_08_03=-0.6640000000000015, SF055_08_04=1, SF056_08_04=1, SF060_08_04=12.240000000000009, SF061a_08_04=-1.088000000000008, SF061b_08_04=-0.5919999999999987, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.08000000000004, SF061a_08_05=-0.7920000000000016, SF061b_08_05=-0.9759999999999991, SF055_08_06=1, SF056_08_06=1, SF060_08_06=16.52000000000004, SF061a_08_06=-1.5840000000000032, SF061b_08_06=-0.9759999999999991, SF031_09=18, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.008000000000000007, SF044_09=1, SF048_09=-0.132, SF049a_09=0.006000000000000005, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=8.879999999999995, SF061a_09_01=0.3119999999999976, SF061b_09_01=0.5759999999999934, SF055_09_02=1, SF056_09_02=1, SF060_09_02=7.0400000000000205, SF061a_09_02=0.21599999999999397, SF061b_09_02=0.4719999999999942, SF055_09_03=1, SF056_09_03=1, SF060_09_03=6.28000000000003, SF061a_09_03=-0.3119999999999976, SF061b_09_03=0.5999999999999943, SF055_09_04=1, SF056_09_04=1, SF060_09_04=12.360000000000014, SF061a_09_04=0.5759999999999934, SF061b_09_04=0.23199999999999932, SF055_09_05=2, SF056_09_05=1, SF060_09_05=8.600000000000023, SF061a_09_05=-0.016000000000005343, SF061b_09_05=0.1599999999999966, SF055_09_06=2, SF056_09_06=1, SF060_09_06=31.0, SF061a_09_06=-1.9200000000000017, SF061b_09_06=0.35199999999998965, SF031_10=19, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.008000000000000007, SF044_10=1, SF048_10=-0.15200000000000002, SF049a_10=0.0030000000000000027, SF049b_10=-0.0030000000000000027, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538880, SF055_10_01=1, SF056_10_01=1, SF060_10_01=6.560000000000002, SF061a_10_01=0.1839999999999975, SF061b_10_01=0.30400000000000205, SF055_10_02=1, SF056_10_02=1, SF060_10_02=3.9600000000000364, SF061a_10_02=0.11999999999999034, SF061b_10_02=0.2560000000000002, SF055_10_03=1, SF056_10_03=1, SF060_10_03=4.560000000000002, SF061a_10_03=-0.12000000000000455, SF061b_10_03=0.37599999999999056, SF055_10_04=1, SF056_10_04=1, SF060_10_04=8.080000000000041, SF061a_10_04=0.3199999999999932, SF061b_10_04=0.16799999999999216, SF055_10_05=1, SF056_10_05=1, SF060_10_05=2.8799999999999955, SF061a_10_05=-0.28000000000000114, SF061b_10_05=0.007999999999995566)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=459, eaf=0, crcType=2, frameCrc=15, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=10010485, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=20, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.14800000000000002, SF049a_01=-0.0010000000000000009, SF049b_01=0.007000000000000006, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4546756608, SF055_01_01=1, SF056_01_01=1, SF060_01_01=21.08000000000004, SF061a_01_01=-0.8239999999999981, SF061b_01_01=-0.6720000000000113, SF055_01_02=5, SF056_01_02=1, SF060_01_02=62.08000000000004, SF061a_01_02=-0.06400000000000716, SF061b_01_02=-0.5280000000000058, SF055_01_03=1, SF056_01_03=1, SF060_01_03=19.840000000000032, SF061a_01_03=-0.8960000000000008, SF061b_01_03=-0.6880000000000024, SF055_01_04=1, SF056_01_04=1, SF060_01_04=18.360000000000014, SF061a_01_04=-1.0799999999999983, SF061b_01_04=-0.5840000000000032, SF055_01_05=1, SF056_01_05=1, SF060_01_05=28.28000000000003, SF061a_01_05=-0.6640000000000015, SF061b_01_05=-0.9840000000000089, SF055_01_06=1, SF056_01_06=1, SF060_01_06=26.160000000000025, SF061a_01_06=-1.3840000000000003, SF061b_01_06=-1.0160000000000053, SF031_02=21, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.124, SF049a_02=0.010000000000000009, SF049b_02=-0.009000000000000008, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4546756608, SF055_02_01=1, SF056_02_01=1, SF060_02_01=16.960000000000036, SF061a_02_01=-0.847999999999999, SF061b_02_01=-0.6640000000000015, SF055_02_02=1, SF056_02_02=1, SF060_02_02=59.44, SF061a_02_02=-0.02400000000000091, SF061b_02_02=-0.22400000000000375, SF055_02_03=1, SF056_02_03=1, SF060_02_03=15.520000000000039, SF061a_02_03=-0.8560000000000088, SF061b_02_03=-0.7280000000000086, SF055_02_04=1, SF056_02_04=1, SF060_02_04=14.680000000000007, SF061a_02_04=-1.13600000000001, SF061b_02_04=-0.48799999999999955, SF055_02_05=1, SF056_02_05=1, SF060_02_05=22.08000000000004, SF061a_02_05=-0.5600000000000023, SF061b_02_05=-1.1280000000000001, SF055_02_06=1, SF056_02_06=1, SF060_02_06=19.720000000000027, SF061a_02_06=-1.4399999999999977, SF061b_02_06=-1.088000000000008, SF031_03=22, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=3, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.14400000000000002, SF049a_03=0.0050000000000000044, SF049b_03=-0.0030000000000000027, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4345430017, SF055_03_01=1, SF056_03_01=1, SF060_03_01=7.640000000000043, SF061a_03_01=0.24799999999999045, SF061b_03_01=0.5519999999999925, SF055_03_02=1, SF056_03_02=1, SF060_03_02=6.080000000000041, SF061a_03_02=-0.1360000000000099, SF061b_03_02=0.6319999999999908, SF055_03_03=1, SF056_03_03=1, SF060_03_03=10.800000000000011, SF061a_03_03=0.47999999999998977, SF061b_03_03=0.24799999999999045, SF055_03_04=1, SF056_03_04=1, SF060_03_04=8.680000000000007, SF061a_03_04=-0.12000000000000455, SF061b_03_04=0.21599999999999397, SF055_03_05=2, SF056_03_05=1, SF060_03_05=35.64000000000004, SF061a_03_05=-1.9120000000000061, SF061b_03_05=0.17600000000000193, SF031_04=23, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=2, SF043_04=0.01200000000000001, SF044_04=1, SF048_04=-0.14, SF049a_04=-0.0040000000000000036, SF049b_04=0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538881, SF055_04_01=1, SF056_04_01=1, SF060_04_01=10.680000000000007, SF061a_04_01=0.30400000000000205, SF061b_04_01=0.5120000000000005, SF055_04_02=1, SF056_04_02=1, SF060_04_02=8.600000000000023, SF061a_04_02=0.21599999999999397, SF061b_04_02=0.3999999999999915, SF055_04_03=1, SF056_04_03=1, SF060_04_03=9.760000000000048, SF061a_04_03=-0.15200000000000102, SF061b_04_03=0.6079999999999899, SF055_04_04=1, SF056_04_04=1, SF060_04_04=12.360000000000014, SF061a_04_04=0.38400000000000034, SF061b_04_04=0.3359999999999985, SF055_04_05=1, SF056_04_05=1, SF060_04_05=9.640000000000043, SF061a_04_05=-0.1360000000000099, SF061b_04_05=0.15200000000000102, SF055_04_06=3, SF056_04_06=1, SF060_04_06=37.76000000000005, SF061a_04_06=-1.7280000000000015, SF061b_04_06=0.519999999999996, SF031_05=24, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=2, SF043_05=0.01200000000000001, SF044_05=1, SF048_05=-0.124, SF049a_05=-0.01999999999999999, SF049b_05=-0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538880, SF055_05_01=2, SF056_05_01=1, SF060_05_01=6.400000000000034, SF061a_05_01=0.46399999999999864, SF061b_05_01=0.2079999999999984, SF055_05_02=1, SF056_05_02=1, SF060_05_02=4.1200000000000045, SF061a_05_02=0.367999999999995, SF061b_05_02=0.09599999999998943, SF055_05_03=3, SF056_05_03=1, SF060_05_03=5.240000000000009, SF061a_05_03=0.08799999999999386, SF061b_05_03=0.1599999999999966, SF055_05_04=1, SF056_05_04=1, SF060_05_04=7.319999999999993, SF061a_05_04=0.7039999999999935, SF061b_05_04=-0.04000000000000625, SF055_05_05=1, SF056_05_05=1, SF060_05_05=3.6000000000000227, SF061a_05_05=-0.008000000000009777, SF061b_05_05=-0.22400000000000375, SF031_06=25, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=2, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.14, SF049a_06=-0.032, SF049b_06=-0.0030000000000000027, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4412538880, SF055_06_01=1, SF056_06_01=1, SF060_06_01=6.800000000000011, SF061a_06_01=0.3199999999999932, SF061b_06_01=0.13599999999999568, SF055_06_02=1, SF056_06_02=1, SF060_06_02=4.0400000000000205, SF061a_06_02=0.2560000000000002, SF061b_06_02=0.055999999999997385, SF055_06_03=1, SF056_06_03=1, SF060_06_03=6.080000000000041, SF061a_06_03=-0.17600000000000193, SF061b_06_03=0.16799999999999216, SF055_06_04=1, SF056_06_04=1, SF060_06_04=6.319999999999993, SF061a_06_04=0.4719999999999942, SF061b_06_04=-0.008000000000009777, SF055_06_05=1, SF056_06_05=1, SF060_06_05=2.5200000000000387, SF061a_06_05=-0.17600000000000193, SF061b_06_05=-0.14400000000000546, SF031_07=26, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=3, SF043_07=0.01200000000000001, SF044_07=1, SF048_07=-0.124, SF049a_07=-0.0020000000000000018, SF049b_07=0.014000000000000012, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.240000000000009, SF061a_07_01=0.4239999999999924, SF061b_07_01=-1.9120000000000061, SF055_07_02=1, SF056_07_02=1, SF060_07_02=14.720000000000027, SF061a_07_02=0.32799999999998875, SF061b_07_02=-1.960000000000008, SF055_07_03=2, SF056_07_03=1, SF060_07_03=13.400000000000034, SF061a_07_03=0.04800000000000182, SF061b_07_03=-1.8320000000000078, SF055_07_04=1, SF056_07_04=1, SF060_07_04=23.920000000000016, SF061a_07_04=0.3199999999999932, SF061b_07_04=-2.328000000000003, SF055_07_05=2, SF056_07_05=1, SF060_07_05=26.439999999999998, SF061a_07_05=-0.6720000000000113, SF061b_07_05=-2.4000000000000057, SF031_08=27, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=3, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.14800000000000002, SF049a_08=-0.0020000000000000018, SF049b_08=0.010000000000000009, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538881, SF055_08_01=1, SF056_08_01=1, SF060_08_01=14.240000000000009, SF061a_08_01=1.4080000000000013, SF061b_08_01=-0.1839999999999975, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.319999999999993, SF061a_08_02=1.3519999999999897, SF061b_08_02=-0.26400000000001, SF055_08_03=2, SF056_08_03=1, SF060_08_03=12.879999999999995, SF061a_08_03=1.0719999999999885, SF061b_08_03=-0.008000000000009777, SF055_08_04=1, SF056_08_04=1, SF060_08_04=20.400000000000034, SF061a_08_04=1.5279999999999916, SF061b_08_04=-0.6720000000000113, SF055_08_05=2, SF056_08_05=1, SF060_08_05=21.600000000000023, SF061a_08_05=0.8160000000000025, SF061b_08_05=-0.6800000000000068, SF055_08_06=4, SF056_08_06=1, SF060_08_06=47.24000000000001, SF061a_08_06=-0.1600000000000108, SF061b_08_06=0.03999999999999204, SF031_09=28, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=2, SF043_09=0.01200000000000001, SF044_09=1, SF048_09=-0.09199999999999997, SF049a_09=-0.0040000000000000036, SF049b_09=0.015000000000000013, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4412538881, SF055_09_01=1, SF056_09_01=1, SF060_09_01=13.760000000000048, SF061a_09_01=1.3279999999999887, SF061b_09_01=-0.16800000000000637, SF055_09_02=1, SF056_09_02=1, SF060_09_02=12.439999999999998, SF061a_09_02=1.2879999999999967, SF061b_09_02=-0.23199999999999932, SF055_09_03=1, SF056_09_03=1, SF060_09_03=13.0, SF061a_09_03=1.024000000000001, SF061b_09_03=-0.008000000000009777, SF055_09_04=1, SF056_09_04=1, SF060_09_04=17.80000000000001, SF061a_09_04=1.543999999999997, SF061b_09_04=-0.6880000000000024, SF055_09_05=1, SF056_09_05=1, SF060_09_05=18.879999999999995, SF061a_09_05=0.7680000000000007, SF061b_09_05=-0.695999999999998, SF055_09_06=3, SF056_09_06=1, SF060_09_06=46.960000000000036, SF061a_09_06=-0.32800000000000296, SF061b_09_06=-0.04000000000000625, SF031_10=29, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=2, SF043_10=0.01200000000000001, SF044_10=1, SF048_10=-0.14, SF049a_10=0.016000000000000014, SF049b_10=0.010000000000000009, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4546756608, SF055_10_01=1, SF056_10_01=1, SF060_10_01=13.680000000000007, SF061a_10_01=0.5519999999999925, SF061b_10_01=-0.19200000000000728, SF055_10_02=3, SF056_10_02=1, SF060_10_02=56.68000000000001, SF061a_10_02=0.8399999999999892, SF061b_10_02=0.7999999999999972, SF055_10_03=1, SF056_10_03=1, SF060_10_03=12.04000000000002, SF061a_10_03=0.4719999999999942, SF061b_10_03=-0.3119999999999976, SF055_10_04=1, SF056_10_04=1, SF060_10_04=13.080000000000041, SF061a_10_04=-0.2560000000000002, SF061b_10_04=-0.04000000000000625, SF055_10_05=2, SF056_10_05=1, SF060_10_05=16.439999999999998, SF061a_10_05=0.8160000000000025, SF061b_10_05=-0.4720000000000084, SF055_10_06=1, SF056_10_06=1, SF060_10_06=16.640000000000043, SF061a_10_06=-0.1600000000000108, SF061b_10_06=-0.3440000000000083)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=448, eaf=0, crcType=2, frameCrc=13, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=7076377, SF005=354, SF068=1, SF069=0, SF030=9, SF031_01=30, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=3, SF043_01=0.01200000000000001, SF044_01=1, SF048_01=-0.16800000000000004, SF049a_01=-0.0010000000000000009, SF049b_01=-0.015999999999999986, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, SF055_01_01=2, SF056_01_01=1, SF060_01_01=12.920000000000016, SF061a_01_01=0.5039999999999907, SF061b_01_01=-0.19200000000000728, SF055_01_02=2, SF056_01_02=1, SF060_01_02=11.160000000000025, SF061a_01_02=0.4239999999999924, SF061b_01_02=-0.22400000000000375, SF055_01_03=2, SF056_01_03=1, SF060_01_03=12.800000000000011, SF061a_01_03=0.19999999999998863, SF061b_01_03=0.055999999999997385, SF055_01_04=1, SF056_01_04=1, SF060_01_04=14.720000000000027, SF061a_01_04=0.6079999999999899, SF061b_01_04=-0.3680000000000092, SF055_01_05=4, SF056_01_05=1, SF060_01_05=13.920000000000016, SF061a_01_05=0.055999999999997385, SF061b_01_05=-0.6159999999999997, SF031_02=31, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=2, SF043_02=0.01200000000000001, SF044_02=1, SF048_02=-0.10399999999999998, SF049a_02=0.0020000000000000018, SF049b_02=0.007000000000000006, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, SF055_02_01=2, SF056_02_01=1, SF060_02_01=5.080000000000041, SF061a_02_01=0.28000000000000114, SF061b_02_01=0.1839999999999975, SF055_02_02=2, SF056_02_02=1, SF060_02_02=3.1200000000000045, SF061a_02_02=0.23199999999999932, SF061b_02_02=0.0799999999999983, SF055_02_03=4, SF056_02_03=1, SF060_02_03=5.080000000000041, SF061a_02_03=-0.06400000000000716, SF061b_02_03=0.13599999999999568, SF055_02_04=3, SF056_02_04=1, SF060_02_04=5.760000000000048, SF061a_02_04=0.5039999999999907, SF061b_02_04=-0.04800000000000182, SF055_02_05=2, SF056_02_05=1, SF060_02_05=4.240000000000009, SF061a_02_05=-0.1280000000000001, SF061b_02_05=-0.2560000000000002, SF031_03=32, SF039_03=0, SF040T_03=1, SF040I_03=1, SF041_03=1, SF042_03=2, SF043_03=0.01200000000000001, SF044_03=1, SF048_03=-0.09599999999999997, SF049a_03=-0.033, SF049b_03=-0.009000000000000008, SF054_03=1, SatBitmaskLen_03=0, SF093_03=4412538880, SF055_03_01=1, SF056_03_01=1, SF060_03_01=5.960000000000036, SF061a_03_01=0.48799999999999955, SF061b_03_01=0.11199999999999477, SF055_03_02=2, SF056_03_02=1, SF060_03_02=3.4399999999999977, SF061a_03_02=0.30400000000000205, SF061b_03_02=0.055999999999997385, SF055_03_03=4, SF056_03_03=1, SF060_03_03=5.640000000000043, SF061a_03_03=1.9279999999999973, SF061b_03_03=0.2639999999999958, SF055_03_04=1, SF056_03_04=1, SF060_03_04=5.0400000000000205, SF061a_03_04=0.7599999999999909, SF061b_03_04=-0.02400000000000091, SF055_03_05=1, SF056_03_05=1, SF060_03_05=2.5600000000000023, SF061a_03_05=0.09599999999998943, SF061b_03_05=-0.1360000000000099, SF031_04=33, SF039_04=0, SF040T_04=1, SF040I_04=1, SF041_04=1, SF042_04=3, SF043_04=0.016000000000000014, SF044_04=1, SF048_04=-0.09999999999999998, SF049a_04=0.0010000000000000009, SF049b_04=-0.0050000000000000044, SF054_04=1, SatBitmaskLen_04=0, SF093_04=4412538880, SF055_04_01=1, SF056_04_01=1, SF060_04_01=14.480000000000018, SF061a_04_01=0.13599999999999568, SF061b_04_01=-2.0320000000000036, SF055_04_02=2, SF056_04_02=1, SF060_04_02=14.080000000000041, SF061a_04_02=0.15200000000000102, SF061b_04_02=-2.0960000000000036, SF055_04_03=1, SF056_04_03=1, SF060_04_03=13.560000000000002, SF061a_04_03=0.09599999999998943, SF061b_04_03=-1.9200000000000017, SF055_04_04=3, SF056_04_04=1, SF060_04_04=23.720000000000027, SF061a_04_04=-0.008000000000009777, SF061b_04_04=-2.504000000000005, SF055_04_05=2, SF056_04_05=1, SF060_04_05=29.160000000000025, SF061a_04_05=-0.35999999999999943, SF061b_04_05=-2.608000000000004, SF031_05=34, SF039_05=0, SF040T_05=1, SF040I_05=1, SF041_05=1, SF042_05=3, SF043_05=0.016000000000000014, SF044_05=1, SF048_05=-0.132, SF049a_05=-0.0040000000000000036, SF049b_05=0.01100000000000001, SF054_05=1, SatBitmaskLen_05=0, SF093_05=4412538881, SF055_05_01=2, SF056_05_01=1, SF060_05_01=7.600000000000023, SF061a_05_01=1.5519999999999925, SF061b_05_01=-0.20000000000000284, SF055_05_02=2, SF056_05_02=1, SF060_05_02=6.760000000000048, SF061a_05_02=1.5519999999999925, SF061b_05_02=-0.2560000000000002, SF055_05_03=3, SF056_05_03=1, SF060_05_03=7.520000000000039, SF061a_05_03=1.2879999999999967, SF061b_05_03=0.0, SF055_05_04=2, SF056_05_04=1, SF060_05_04=13.439999999999998, SF061a_05_04=1.4399999999999977, SF061b_05_04=-0.5760000000000076, SF055_05_05=3, SF056_05_05=1, SF060_05_05=17.400000000000034, SF061a_05_05=0.73599999999999, SF061b_05_05=-0.9440000000000026, SF055_05_06=4, SF056_05_06=1, SF060_05_06=47.84000000000003, SF061a_05_06=0.02400000000000091, SF061b_05_06=0.14399999999999125, SF031_06=35, SF039_06=0, SF040T_06=1, SF040I_06=1, SF041_06=1, SF042_06=3, SF043_06=0.01200000000000001, SF044_06=1, SF048_06=-0.17200000000000004, SF049a_06=0.0020000000000000018, SF049b_06=-0.013000000000000012, SF054_06=1, SatBitmaskLen_06=0, SF093_06=4546756608, SF055_06_01=1, SF056_06_01=1, SF060_06_01=11.080000000000041, SF061a_06_01=0.45599999999998886, SF061b_06_01=-0.23199999999999932, SF055_06_02=4, SF056_06_02=1, SF060_06_02=60.68000000000001, SF061a_06_02=0.4719999999999942, SF061b_06_02=0.519999999999996, SF055_06_03=1, SF056_06_03=1, SF060_06_03=9.400000000000034, SF061a_06_03=0.519999999999996, SF061b_06_03=-0.26400000000001, SF055_06_04=2, SF056_06_04=1, SF060_06_04=11.800000000000011, SF061a_06_04=0.3359999999999985, SF061b_06_04=-0.17600000000000193, SF055_06_05=1, SF056_06_05=1, SF060_06_05=12.080000000000041, SF061a_06_05=0.7199999999999989, SF061b_06_05=-0.4399999999999977, SF055_06_06=2, SF056_06_06=1, SF060_06_06=12.680000000000007, SF061a_06_06=0.2560000000000002, SF061b_06_06=-0.6159999999999997, SF031_07=36, SF039_07=0, SF040T_07=1, SF040I_07=1, SF041_07=1, SF042_07=2, SF043_07=0.016000000000000014, SF044_07=1, SF048_07=-0.11599999999999999, SF049a_07=0.0010000000000000009, SF049b_07=0.0020000000000000018, SF054_07=1, SatBitmaskLen_07=0, SF093_07=4412538880, SF055_07_01=1, SF056_07_01=1, SF060_07_01=15.720000000000027, SF061a_07_01=1.039999999999992, SF061b_07_01=-0.09600000000000364, SF055_07_02=1, SF056_07_02=1, SF060_07_02=13.720000000000027, SF061a_07_02=1.024000000000001, SF061b_07_02=-0.09600000000000364, SF055_07_03=1, SF056_07_03=1, SF060_07_03=17.04000000000002, SF061a_07_03=0.8799999999999955, SF061b_07_03=-0.1280000000000001, SF055_07_04=1, SF056_07_04=1, SF060_07_04=15.319999999999993, SF061a_07_04=1.0719999999999885, SF061b_07_04=-0.21600000000000819, SF055_07_05=1, SF056_07_05=1, SF060_07_05=15.120000000000005, SF061a_07_05=0.8079999999999927, SF061b_07_05=-0.45600000000000307, SF031_08=37, SF039_08=0, SF040T_08=1, SF040I_08=1, SF041_08=1, SF042_08=1, SF043_08=0.01200000000000001, SF044_08=1, SF048_08=-0.07199999999999995, SF049a_08=0.006000000000000005, SF049b_08=0.016000000000000014, SF054_08=1, SatBitmaskLen_08=0, SF093_08=4412538880, SF055_08_01=1, SF056_08_01=1, SF060_08_01=15.520000000000039, SF061a_08_01=1.0559999999999974, SF061b_08_01=-0.03200000000001069, SF055_08_02=1, SF056_08_02=1, SF060_08_02=13.080000000000041, SF061a_08_02=1.0, SF061b_08_02=-0.16800000000000637, SF055_08_03=1, SF056_08_03=1, SF060_08_03=16.52000000000004, SF061a_08_03=0.8559999999999945, SF061b_08_03=-0.1039999999999992, SF055_08_04=1, SF056_08_04=1, SF060_08_04=14.160000000000025, SF061a_08_04=1.1039999999999992, SF061b_08_04=-0.2560000000000002, SF055_08_05=1, SF056_08_05=1, SF060_08_05=13.28000000000003, SF061a_08_05=0.671999999999997, SF061b_08_05=-0.30400000000000205, SF031_09=38, SF039_09=0, SF040T_09=1, SF040I_09=1, SF041_09=1, SF042_09=1, SF043_09=0.016000000000000014, SF044_09=1, SF048_09=-0.17600000000000005, SF049a_09=-0.01899999999999999, SF049b_09=-0.006000000000000005, SF054_09=1, SatBitmaskLen_09=0, SF093_09=4546756608, SF055_09_01=1, SF056_09_01=1, SF060_09_01=9.0, SF061a_09_01=0.5600000000000023, SF061b_09_01=-0.1600000000000108, SF055_09_02=3, SF056_09_02=1, SF060_09_02=61.160000000000025, SF061a_09_02=-0.480000000000004, SF061b_09_02=0.6640000000000015, SF055_09_03=1, SF056_09_03=1, SF060_09_03=7.080000000000041, SF061a_09_03=0.671999999999997, SF061b_09_03=-0.28000000000000114, SF055_09_04=2, SF056_09_04=1, SF060_09_04=10.160000000000025, SF061a_09_04=0.4959999999999951, SF061b_09_04=-0.1280000000000001, SF055_09_05=2, SF056_09_05=1, SF060_09_05=9.360000000000014, SF061a_09_05=0.6559999999999917, SF061b_09_05=-0.5600000000000023, SF055_09_06=2, SF056_09_06=1, SF060_09_06=10.520000000000039, SF061a_09_06=0.6400000000000006, SF061b_09_06=-0.6480000000000103, SF031_10=39, SF039_10=0, SF040T_10=1, SF040I_10=1, SF041_10=1, SF042_10=3, SF043_10=0.016000000000000014, SF044_10=1, SF048_10=-0.124, SF049a_10=0.010000000000000009, SF049b_10=0.0020000000000000018, SF054_10=1, SatBitmaskLen_10=0, SF093_10=4412538888, SF055_10_01=1, SF056_10_01=1, SF060_10_01=12.080000000000041, SF061a_10_01=0.9200000000000017, SF061b_10_01=-0.11200000000000898, SF055_10_02=1, SF056_10_02=1, SF060_10_02=10.160000000000025, SF061a_10_02=0.9039999999999964, SF061b_10_02=-0.08800000000000807, SF055_10_03=1, SF056_10_03=1, SF060_10_03=13.640000000000043, SF061a_10_03=0.8239999999999981, SF061b_10_03=-0.2079999999999984, SF055_10_04=1, SF056_10_04=1, SF060_10_04=11.560000000000002, SF061a_10_04=0.8319999999999936, SF061b_10_04=-0.2560000000000002, SF055_10_05=1, SF056_10_05=1, SF060_10_05=11.400000000000034, SF061a_10_05=0.9839999999999947, SF061b_10_05=-0.3359999999999985, SF055_10_06=5, SF056_10_06=1, SF060_10_06=68.76000000000005, SF061a_10_06=-4.496000000000002, SF061b_10_06=-3.5520000000000067)>",
+            "<SPARTN(SPARTN-1X-HPAC-GAL, msgType=1, nData=87, eaf=0, crcType=2, frameCrc=2, msgSubtype=2, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=5702700, SF005=354, SF068=1, SF069=0, SF030=1, SF031_01=40, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.008000000000000007, SF044_01=1, SF048_01=-0.15600000000000003, SF049a_01=-0.008000000000000007, SF049b_01=0.0, SF054_01=1, SatBitmaskLen_01=0, SF093_01=4412538880, SF055_01_01=2, SF056_01_01=1, SF060_01_01=-4.0, SF061a_01_01=0.24799999999999045, SF061b_01_01=-0.20000000000000284, SF055_01_02=1, SF056_01_02=1, SF060_01_02=-6.9599999999999795, SF061a_01_02=0.1839999999999975, SF061b_01_02=-0.2400000000000091, SF055_01_03=1, SF056_01_03=1, SF060_01_03=-5.639999999999986, SF061a_01_03=-0.06400000000000716, SF061b_01_03=-0.26400000000001, SF055_01_04=2, SF056_01_04=1, SF060_01_04=-4.0, SF061a_01_04=0.5759999999999934, SF061b_01_04=-0.3359999999999985, SF055_01_05=1, SF056_01_05=1, SF060_01_05=-9.439999999999998, SF061a_01_05=-0.07200000000000273, SF061b_01_05=-0.4720000000000084, SF031_02=41, SF039_02=0, SF040T_02=1, SF040I_02=1, SF041_02=1, SF042_02=1, SF043_02=0.008000000000000007, SF044_02=1, SF048_02=-0.16400000000000003, SF049a_02=-0.0010000000000000009, SF049b_02=0.0010000000000000009, SF054_02=1, SatBitmaskLen_02=0, SF093_02=4412538880, SF055_02_01=2, SF056_02_01=1, SF060_02_01=-3.599999999999966, SF061a_02_01=0.19999999999998863, SF061b_02_01=-0.20000000000000284, SF055_02_02=1, SF056_02_02=1, SF060_02_02=-6.839999999999975, SF061a_02_02=0.09599999999998943, SF061b_02_02=-0.30400000000000205, SF055_02_03=1, SF056_02_03=1, SF060_02_03=-6.079999999999984, SF061a_02_03=-0.1360000000000099, SF061b_02_03=-0.27200000000000557, SF055_02_04=1, SF056_02_04=1, SF060_02_04=-3.1200000000000045, SF061a_02_04=0.45599999999998886, SF061b_02_04=-0.35999999999999943, SF055_02_05=1, SF056_02_05=1, SF060_02_05=-9.879999999999995, SF061a_02_05=-0.03200000000001069, SF061b_02_05=-0.480000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=180, eaf=0, crcType=2, frameCrc=4, msgSubtype=0, timeTagtype=1, gnssTimeTag=452200860, solutionId=5, solutionProcId=11, crc=736926, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF016=0, SatBitmaskLen=0, SF011=882933762, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF018_01=45, SF020R_01=0.13599999999999923, SF020A_01=-1.426000000000002, SF020C_01=0.045999999999999375, SF022_01=7, SF020CK_01=6.782, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF025_01=60, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.6660000000000004, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.6660000000000004, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.6359999999999992, CodeBiasBitmaskLen_01=0, SF027_01=60, SF029_01_01=-2.280000000000001, SF029_01_02=-0.35999999999999943, SF029_01_03=-0.240000000000002, SF029_01_04=-2.4800000000000004, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF018_02=189, SF020R_02=-0.652000000000001, SF020A_02=-0.07000000000000028, SF020C_02=0.1039999999999992, SF022_02=7, SF020CK_02=3.041999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF025_02=60, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=1.5879999999999974, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=1.5879999999999974, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=1.6039999999999992, CodeBiasBitmaskLen_02=0, SF027_02=60, SF029_02_01=-3.1400000000000006, SF029_02_02=-2.280000000000001, SF029_02_03=-2.460000000000001, SF029_02_04=-1.1999999999999993, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF018_03=48, SF020R_03=-0.23200000000000287, SF020A_03=1.9899999999999984, SF020C_03=-0.0020000000000024443, SF022_03=7, SF020CK_03=1.8399999999999999, SF024_03=1, PhaseBiasBitmaskLen_03=0, SF025_03=60, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=-0.23799999999999955, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=-0.23799999999999955, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=-0.272000000000002, CodeBiasBitmaskLen_03=0, SF027_03=60, SF029_03_01=0.5999999999999979, SF029_03_02=2.84, SF029_03_03=3.099999999999998, SF029_03_04=0.9199999999999982, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF018_04=5, SF020R_04=0.14399999999999835, SF020A_04=0.27399999999999736, SF020C_04=0.2759999999999998, SF022_04=7, SF020CK_04=2.8959999999999972, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF025_04=60, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.17800000000000082, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.17800000000000082, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=-0.1620000000000026, CodeBiasBitmaskLen_04=0, SF027_04=60, SF029_04_01=0.16000000000000014, SF029_04_02=1.4400000000000013, SF029_04_03=1.2800000000000011, SF029_04_04=-0.6000000000000014, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=6, SF018_05=108, SF020R_05=-0.7500000000000018, SF020A_05=-0.6400000000000006, SF020C_05=0.2560000000000002, SF022_05=6, SF020CK_05=-1.7180000000000017, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF025_05=60, SF023_05_01=1, SF015_05_01=6, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=6, SF020PB_05_02=0.27199999999999847, SF023_05_03=1, SF015_05_03=6, SF020PB_05_03=0.27199999999999847, SF023_05_04=1, SF015_05_04=6, SF020PB_05_04=0.6219999999999999, CodeBiasBitmaskLen_05=0, SF027_05=60, SF029_05_01=-0.120000000000001, SF029_05_02=-0.08000000000000185, SF029_05_03=-0.1999999999999993, SF029_05_04=1.5399999999999991, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF018_06=44, SF020R_06=-0.18599999999999994, SF020A_06=0.6459999999999972, SF020C_06=-0.24399999999999977, SF022_06=7, SF020CK_06=-1.3300000000000018, SF024_06=3, PhaseBiasBitmaskLen_06=0, SF025_06=56, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=-0.03400000000000247, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=-0.03400000000000247, CodeBiasBitmaskLen_06=0, SF027_06=56, SF029_06_01=0.16000000000000014, SF029_06_02=-0.7800000000000011, SF029_06_03=-0.8399999999999999, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF018_07=32, SF020R_07=0.11199999999999832, SF020A_07=-0.48600000000000065, SF020C_07=0.4659999999999975, SF022_07=7, SF020CK_07=-1.474000000000002, SF024_07=1, PhaseBiasBitmaskLen_07=0, SF025_07=56, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=0.2579999999999991, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=0.2579999999999991, CodeBiasBitmaskLen_07=0, SF027_07=56, SF029_07_01=-0.9200000000000017, SF029_07_02=-2.0199999999999996, SF029_07_03=-1.9800000000000004)>",
+            "<SPARTN(SPARTN-1X-OCB-GLO, msgType=0, nData=152, eaf=0, crcType=2, frameCrc=15, msgSubtype=1, timeTagtype=1, gnssTimeTag=452211642, solutionId=5, solutionProcId=11, crc=7233776, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF017=0, SatBitmaskLen=0, SF012=8618373, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF019_01=89, SF020R_01=0.2839999999999989, SF020A_01=2.2779999999999987, SF020C_01=-1.910000000000002, SF022_01=7, SF020CK_01=-3.4040000000000017, SF024_01=2, PhaseBiasBitmaskLen_01=0, SF026_01=24, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=-0.5800000000000018, CodeBiasBitmaskLen_01=0, SF028_01=24, SF029_01_01=1.120000000000001, SF029_01_02=1.9199999999999982, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF019_02=89, SF020R_02=0.129999999999999, SF020A_02=0.6459999999999972, SF020C_02=0.8780000000000001, SF022_02=7, SF020CK_02=-0.7900000000000009, SF024_02=2, PhaseBiasBitmaskLen_02=0, SF026_02=24, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.4480000000000004, CodeBiasBitmaskLen_02=0, SF028_02=24, SF029_02_01=-0.6799999999999997, SF029_02_02=-0.5599999999999987, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF019_03=89, SF020R_03=-0.013999999999999346, SF020A_03=3.0159999999999982, SF020C_03=0.8580000000000005, SF022_03=7, SF020CK_03=4.366, SF024_03=2, PhaseBiasBitmaskLen_03=0, SF026_03=24, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.34199999999999875, CodeBiasBitmaskLen_03=0, SF028_03=24, SF029_03_01=-1.6000000000000014, SF029_03_02=-2.400000000000002, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF019_04=89, SF020R_04=0.7519999999999989, SF020A_04=6.013999999999999, SF020C_04=-3.1860000000000017, SF022_04=7, SF020CK_04=5.2940000000000005, SF024_04=2, PhaseBiasBitmaskLen_04=0, SF026_04=24, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=0.19399999999999906, CodeBiasBitmaskLen_04=0, SF028_04=24, SF029_04_01=-0.5599999999999987, SF029_04_02=-0.9600000000000009, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF019_05=89, SF020R_05=0.01799999999999713, SF020A_05=-5.796000000000001, SF020C_05=-0.1460000000000008, SF022_05=7, SF020CK_05=1.1119999999999983, SF024_05=2, PhaseBiasBitmaskLen_05=0, SF026_05=24, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=-0.1460000000000008, CodeBiasBitmaskLen_05=0, SF028_05=24, SF029_05_01=-0.5199999999999996, SF029_05_02=-0.10000000000000142, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=6, SF019_06=89, SF020R_06=0.5339999999999989, SF020A_06=-0.5640000000000018, SF020C_06=0.6739999999999995, SF022_06=6, SF020CK_06=-1.838000000000001, SF024_06=1, PhaseBiasBitmaskLen_06=0, SF026_06=24, SF023_06_01=1, SF015_06_01=6, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=6, SF020PB_06_02=-0.15000000000000213, CodeBiasBitmaskLen_06=0, SF028_06=24, SF029_06_01=0.03999999999999915, SF029_06_02=-0.03999999999999915, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF019_07=89, SF020R_07=1.4540000000000006, SF020A_07=-1.5180000000000007, SF020C_07=-1.200000000000001, SF022_07=7, SF020CK_07=-2.694000000000001, SF024_07=4, PhaseBiasBitmaskLen_07=0, SF026_07=24, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.7660000000000018, CodeBiasBitmaskLen_07=0, SF028_07=24, SF029_07_01=2.919999999999998, SF029_07_02=2.1799999999999997, SF013_08=0, SF014O_08=1, SF014C_08=1, SF014B_08=1, SF015_08=7, SF019_08=89, SF020R_08=0.597999999999999, SF020A_08=0.15399999999999991, SF020C_08=0.5239999999999974, SF022_08=7, SF020CK_08=-1.6560000000000006, SF024_08=2, PhaseBiasBitmaskLen_08=0, SF026_08=24, SF023_08_01=1, SF015_08_01=7, SF020PB_08_01=0.0, SF023_08_02=1, SF015_08_02=7, SF020PB_08_02=-0.5660000000000007, CodeBiasBitmaskLen_08=0, SF028_08=24, SF029_08_01=1.379999999999999, SF029_08_02=1.259999999999998)>",
+            "<SPARTN(SPARTN-1X-OCB-BEI, msgType=0, nData=193, eaf=0, crcType=2, frameCrc=3, msgSubtype=3, timeTagtype=1, gnssTimeTag=452200846, solutionId=5, solutionProcId=11, crc=6801214, SF005=354, SF010=0, SF069=0, SF008=0, SF009=0, SF097=0, SatBitmaskLen=1, SF094=184555012, SF013_01=0, SF014O_01=1, SF014C_01=1, SF014B_01=1, SF015_01=7, SF100_01=95, SF020R_01=0.24599999999999866, SF020A_01=0.20599999999999952, SF020C_01=-0.28000000000000114, SF022_01=7, SF020CK_01=2.9399999999999977, SF024_01=3, PhaseBiasBitmaskLen_01=0, SF103_01=232, SF023_01_01=1, SF015_01_01=7, SF020PB_01_01=0.0, SF023_01_02=1, SF015_01_02=7, SF020PB_01_02=0.7999999999999972, SF023_01_03=1, SF015_01_03=7, SF020PB_01_03=0.7799999999999976, SF023_01_04=1, SF015_01_04=7, SF020PB_01_04=0.0, CodeBiasBitmaskLen_01=0, SF106_01=232, SF029_01_01=-1.1799999999999997, SF029_01_02=-2.620000000000001, SF029_01_03=-2.620000000000001, SF029_01_04=-1.1799999999999997, SF013_02=0, SF014O_02=1, SF014C_02=1, SF014B_02=1, SF015_02=7, SF100_02=95, SF020R_02=0.3379999999999974, SF020A_02=-0.08200000000000074, SF020C_02=-0.4380000000000006, SF022_02=7, SF020CK_02=4.047999999999998, SF024_02=1, PhaseBiasBitmaskLen_02=0, SF103_02=232, SF023_02_01=1, SF015_02_01=7, SF020PB_02_01=0.0, SF023_02_02=1, SF015_02_02=7, SF020PB_02_02=0.7680000000000007, SF023_02_03=1, SF015_02_03=7, SF020PB_02_03=0.7479999999999976, SF023_02_04=1, SF015_02_04=7, SF020PB_02_04=0.0, CodeBiasBitmaskLen_02=0, SF106_02=232, SF029_02_01=-1.4000000000000021, SF029_02_02=-4.0, SF029_02_03=-4.0, SF029_02_04=-1.4000000000000021, SF013_03=0, SF014O_03=1, SF014C_03=1, SF014B_03=1, SF015_03=7, SF100_03=95, SF020R_03=-0.240000000000002, SF020A_03=0.029999999999997584, SF020C_03=-0.34800000000000253, SF022_03=7, SF020CK_03=4.07, SF024_03=3, PhaseBiasBitmaskLen_03=0, SF103_03=232, SF023_03_01=1, SF015_03_01=7, SF020PB_03_01=0.0, SF023_03_02=1, SF015_03_02=7, SF020PB_03_02=0.6899999999999977, SF023_03_03=1, SF015_03_03=7, SF020PB_03_03=0.6720000000000006, SF023_03_04=1, SF015_03_04=7, SF020PB_03_04=0.0, CodeBiasBitmaskLen_03=0, SF106_03=232, SF029_03_01=-1.0199999999999996, SF029_03_02=-5.32, SF029_03_03=-5.32, SF029_03_04=-1.0199999999999996, SF013_04=0, SF014O_04=1, SF014C_04=1, SF014B_04=1, SF015_04=7, SF100_04=95, SF020R_04=-0.1460000000000008, SF020A_04=0.2539999999999978, SF020C_04=0.347999999999999, SF022_04=7, SF020CK_04=-3.0100000000000016, SF024_04=1, PhaseBiasBitmaskLen_04=0, SF103_04=232, SF023_04_01=1, SF015_04_01=7, SF020PB_04_01=0.0, SF023_04_02=1, SF015_04_02=7, SF020PB_04_02=-0.1479999999999997, SF023_04_03=1, SF015_04_03=7, SF020PB_04_03=-0.1460000000000008, SF023_04_04=1, SF015_04_04=7, SF020PB_04_04=0.0, CodeBiasBitmaskLen_04=0, SF106_04=232, SF029_04_01=0.14000000000000057, SF029_04_02=-0.26000000000000156, SF029_04_03=-0.26000000000000156, SF029_04_04=0.14000000000000057, SF013_05=0, SF014O_05=1, SF014C_05=1, SF014B_05=1, SF015_05=7, SF100_05=95, SF020R_05=-0.15399999999999991, SF020A_05=-0.26399999999999935, SF020C_05=-0.2140000000000022, SF022_05=7, SF020CK_05=-5.328000000000001, SF024_05=1, PhaseBiasBitmaskLen_05=0, SF103_05=232, SF023_05_01=1, SF015_05_01=7, SF020PB_05_01=0.0, SF023_05_02=1, SF015_05_02=7, SF020PB_05_02=0.8580000000000005, SF023_05_03=1, SF015_05_03=7, SF020PB_05_03=0.8359999999999985, SF023_05_04=1, SF015_05_04=7, SF020PB_05_04=0.0, CodeBiasBitmaskLen_05=0, SF106_05=232, SF029_05_01=-0.40000000000000213, SF029_05_02=6.140000000000001, SF029_05_03=6.140000000000001, SF029_05_04=-0.40000000000000213, SF013_06=0, SF014O_06=1, SF014C_06=1, SF014B_06=1, SF015_06=7, SF100_06=95, SF020R_06=-0.38000000000000256, SF020A_06=-0.28800000000000026, SF020C_06=0.045999999999999375, SF022_06=7, SF020CK_06=-4.3580000000000005, SF024_06=2, PhaseBiasBitmaskLen_06=0, SF103_06=232, SF023_06_01=1, SF015_06_01=7, SF020PB_06_01=0.0, SF023_06_02=1, SF015_06_02=7, SF020PB_06_02=0.7880000000000003, SF023_06_03=1, SF015_06_03=7, SF020PB_06_03=0.7680000000000007, SF023_06_04=1, SF015_06_04=7, SF020PB_06_04=0.0, CodeBiasBitmaskLen_06=0, SF106_06=232, SF029_06_01=-1.4800000000000004, SF029_06_02=2.259999999999998, SF029_06_03=2.259999999999998, SF029_06_04=-1.4800000000000004, SF013_07=0, SF014O_07=1, SF014C_07=1, SF014B_07=1, SF015_07=7, SF100_07=95, SF020R_07=0.1319999999999979, SF020A_07=0.3739999999999988, SF020C_07=0.4259999999999984, SF022_07=7, SF020CK_07=-1.6240000000000006, SF024_07=3, PhaseBiasBitmaskLen_07=0, SF103_07=232, SF023_07_01=1, SF015_07_01=7, SF020PB_07_01=0.0, SF023_07_02=1, SF015_07_02=7, SF020PB_07_02=-0.0779999999999994, SF023_07_03=1, SF015_07_03=7, SF020PB_07_03=-0.07600000000000051, SF023_07_04=1, SF015_07_04=7, SF020PB_07_04=0.0, CodeBiasBitmaskLen_07=0, SF106_07=232, SF029_07_01=0.7800000000000011, SF029_07_02=0.33999999999999986, SF029_07_03=0.33999999999999986, SF029_07_04=0.7800000000000011)>",
+        ]
+        i = 0
+        with open(
+            os.path.join(self.dirname, "spartnntrip_20240430192807.log"),
+            "rb",
+        ) as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=True,
+                key="abcdef1234567890abcdef1234567890",  # key is arbitrary for unencrypted messages
+                basedate=datetime(
+                    2024, 1, 1, 1, 1, 1
+                ),  # basedate is arbitrary for unencrypted messages
+            )
+
+            for raw, parsed in spr:
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertEqual(str(parsed), EXPECTED_RESULT[i])
+                    self.assertTrue(0 <= parsed._padding <= 8)
+                    i += 1
+
+        self.assertEqual(i, 10)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

