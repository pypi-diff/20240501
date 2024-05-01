# Comparing `tmp/tailucas_pylib-0.3.6.tar.gz` & `tmp/tailucas_pylib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.3.6.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.7.tar", max compression
```

## Comparing `tailucas_pylib-0.3.6.tar` & `tailucas_pylib-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.6/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.6/README.md
--rw-r--r--   0        0        0      537 2024-04-30 08:38:16.322013 tailucas_pylib-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.6/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.6/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.6/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.6/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.6/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.6/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.6/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.6/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.6/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.6/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9984 2024-04-30 08:38:32.802013 tailucas_pylib-0.3.6/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.6/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.6/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.7/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.7/README.md
+-rw-r--r--   0        0        0      557 2024-05-01 07:04:26.407556 tailucas_pylib-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.7/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.7/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.7/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.7/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.7/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.7/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     1503 2024-05-01 06:59:19.767564 tailucas_pylib-0.3.7/tailucas_pylib/device.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.7/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9984 2024-04-30 08:38:32.802013 tailucas_pylib-0.3.7/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.7/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.7/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12330 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.7/PKG-INFO
```

### Comparing `tailucas_pylib-0.3.6/LICENSE` & `tailucas_pylib-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/README.md` & `tailucas_pylib-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.7/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/app.py` & `tailucas_pylib-0.3.7/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.7/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.7/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.7/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.7/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/data.py` & `tailucas_pylib-0.3.7/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.7/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.7/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/process.py` & `tailucas_pylib-0.3.7/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.7/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.7/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.7/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.6/PKG-INFO` & `tailucas_pylib-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.93,<2.0.0)
 Requires-Dist: botoflow (>=0.8,<0.9)
 Requires-Dist: cronitor (>=4.7.1,<5.0.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (>=26.0.2,<27.0.0)
 Requires-Dist: sentry-sdk (>=2.0.1,<3.0.0)
 Requires-Dist: simplejson (>=3.19.2,<4.0.0)
 Description-Content-Type: text/markdown
```

