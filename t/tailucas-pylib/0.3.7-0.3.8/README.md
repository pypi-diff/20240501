# Comparing `tmp/tailucas_pylib-0.3.7.tar.gz` & `tmp/tailucas_pylib-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.3.7.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.8.tar", max compression
```

## Comparing `tailucas_pylib-0.3.7.tar` & `tailucas_pylib-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.7/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.7/README.md
--rw-r--r--   0        0        0      557 2024-05-01 07:04:26.407556 tailucas_pylib-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.7/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.7/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.7/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.7/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.7/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.7/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     1503 2024-05-01 06:59:19.767564 tailucas_pylib-0.3.7/tailucas_pylib/device.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.7/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.7/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9984 2024-04-30 08:38:32.802013 tailucas_pylib-0.3.7/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.7/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.7/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12330 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.8/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.8/README.md
+-rw-r--r--   0        0        0      557 2024-05-01 08:26:15.897563 tailucas_pylib-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5980 2024-05-01 08:26:04.497563 tailucas_pylib-0.3.8/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.8/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.8/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.8/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.8/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.8/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.8/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.8/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     1503 2024-05-01 06:59:19.767564 tailucas_pylib-0.3.8/tailucas_pylib/device.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.8/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.8/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9984 2024-04-30 08:38:32.802013 tailucas_pylib-0.3.8/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.8/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.8/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12330 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.8/PKG-INFO
```

### Comparing `tailucas_pylib-0.3.7/LICENSE` & `tailucas_pylib-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/README.md` & `tailucas_pylib-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/pyproject.toml` & `tailucas_pylib-0.3.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.3.7"
+version = "0.3.8"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.8/tailucas_pylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         builtins.DEVICE_NAME = APP_NAME
         builtins.DEVICE_NAME_BASE = APP_NAME
     builtins.APP_CONFIG = app_config  # type: ignore
 
     # 1Password credentials
     creds = None
     app_creds_config = None
-    op_connect_server_env = 'OP_CONNECT_SERVER'
+    op_connect_server_env = 'OP_CONNECT_HOST'
     if op_connect_server_env in os.environ:
         if hasattr(builtins, 'creds_config'):
             try:
                 app_creds_config = builtins.creds_config
                 import onepasswordconnectsdk
                 from onepasswordconnectsdk.client import (
                     Client,
```

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/app.py` & `tailucas_pylib-0.3.8/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.8/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.8/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.8/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.8/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/data.py` & `tailucas_pylib-0.3.8/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.8/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/device.py` & `tailucas_pylib-0.3.8/tailucas_pylib/device.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.8/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/process.py` & `tailucas_pylib-0.3.8/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.8/tailucas_pylib/rabbit.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.8/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.8/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.7/PKG-INFO` & `tailucas_pylib-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.3.7
+Version: 0.3.8
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

