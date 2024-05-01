# Comparing `tmp/avanza_api-9.1.0.tar.gz` & `tmp/avanza_api-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avanza_api-9.1.0.tar", last modified: Mon Apr 15 19:47:49 2024, max compression
+gzip compressed data, was "avanza_api-9.1.1.tar", last modified: Mon Apr 22 19:49:38 2024, max compression
```

## Comparing `avanza_api-9.1.0.tar` & `avanza_api-9.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 19:47:41.000000 avanza_api-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-15 19:47:49.941053 avanza_api-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-15 19:47:41.000000 avanza_api-9.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/avanza/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101813 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/avanza.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/avanza_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/avanza_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:47:49.941053 avanza_api-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-15 19:47:41.000000 avanza_api-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:49:38.702611 avanza_api-9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-22 19:49:30.000000 avanza_api-9.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-22 19:49:38.702611 avanza_api-9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-22 19:49:30.000000 avanza_api-9.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:49:38.702611 avanza_api-9.1.1/avanza/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 19:49:30.000000 avanza_api-9.1.1/avanza/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101831 2024-04-22 19:49:30.000000 avanza_api-9.1.1/avanza/avanza.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-22 19:49:30.000000 avanza_api-9.1.1/avanza/avanza_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-22 19:49:30.000000 avanza_api-9.1.1/avanza/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-22 19:49:30.000000 avanza_api-9.1.1/avanza/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:49:38.702611 avanza_api-9.1.1/avanza_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-22 19:49:38.000000 avanza_api-9.1.1/avanza_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 19:49:38.000000 avanza_api-9.1.1/avanza_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:49:38.000000 avanza_api-9.1.1/avanza_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 19:49:38.000000 avanza_api-9.1.1/avanza_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 19:49:38.000000 avanza_api-9.1.1/avanza_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:49:38.702611 avanza_api-9.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-22 19:49:30.000000 avanza_api-9.1.1/setup.py
```

### Comparing `avanza_api-9.1.0/LICENSE` & `avanza_api-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avanza_api-9.1.0/PKG-INFO` & `avanza_api-9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avanza-api
-Version: 9.1.0
+Version: 9.1.1
 Summary: A Python library for the unofficial Avanza API
 Home-page: https://github.com/Qluxzz/avanza
 Author: André Andersson
 Author-email: andre.eric.andersson@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `avanza_api-9.1.0/README.md` & `avanza_api-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `avanza_api-9.1.0/avanza/avanza.py` & `avanza_api-9.1.1/avanza/avanza.py`

 * *Files 0% similar despite different names*

```diff
@@ -2213,24 +2213,24 @@
             HttpMethod.POST,
             Route.ORDER_PLACE_STOP_LOSS_PATH.value,
             {
                 'parentStopLossId': parent_stop_loss_id,
                 'accountId': account_id,
                 'orderBookId': order_book_id,
                 'stopLossTrigger': {
-                    'type': stop_loss_trigger.type,
+                    'type': stop_loss_trigger.type.value,
                     'value': stop_loss_trigger.value,
                     'validUntil': stop_loss_trigger.valid_until.isoformat()
                 },
                 'stopLossOrderEvent': {
-                    'type': stop_loss_order_event.type,
+                    'type': stop_loss_order_event.type.value,
                     'price': stop_loss_order_event.price,
                     'volume': stop_loss_order_event.volume,
                     'validDays': stop_loss_order_event.valid_days,
-                    'priceType': stop_loss_order_event.price_type,
+                    'priceType': stop_loss_order_event.price_type.value,
                     'shortSellingAllowed': stop_loss_order_event.short_selling_allowed
                 }
             }
         )
 
     def edit_order(
         self,
```

### Comparing `avanza_api-9.1.0/avanza/avanza_socket.py` & `avanza_api-9.1.1/avanza/avanza_socket.py`

 * *Files identical despite different names*

### Comparing `avanza_api-9.1.0/avanza/constants.py` & `avanza_api-9.1.1/avanza/constants.py`

 * *Files identical despite different names*

### Comparing `avanza_api-9.1.0/avanza/entities.py` & `avanza_api-9.1.1/avanza/entities.py`

 * *Files identical despite different names*

### Comparing `avanza_api-9.1.0/avanza_api.egg-info/PKG-INFO` & `avanza_api-9.1.1/avanza_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avanza-api
-Version: 9.1.0
+Version: 9.1.1
 Summary: A Python library for the unofficial Avanza API
 Home-page: https://github.com/Qluxzz/avanza
 Author: André Andersson
 Author-email: andre.eric.andersson@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `avanza_api-9.1.0/setup.py` & `avanza_api-9.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'avanza-api'
 DESCRIPTION = 'A Python library for the unofficial Avanza API'
 URL = 'https://github.com/Qluxzz/avanza'
 EMAIL = 'andre.eric.andersson@gmail.com'
 AUTHOR = 'André Andersson'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '9.1.0'
+VERSION = '9.1.1'
 
 REQUIRED = [
     'requests>=2',
     'pyotp>=2',
     'websockets>=8'
 ]
```

