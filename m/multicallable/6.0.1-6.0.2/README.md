# Comparing `tmp/multicallable-6.0.1.tar.gz` & `tmp/multicallable-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmp98vfcn28/multicallable-6.0.1.tar", last modified: Sun Sep 17 14:17:34 2023, max compression
+gzip compressed data, was "multicallable-6.0.2.tar", last modified: Wed May  1 15:22:51 2024, max compression
```

## Comparing `multicallable-6.0.1.tar` & `multicallable-6.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-09-17 14:17:34.000000 multicallable-6.0.1/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-6.0.1/LICENCE
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4037 2023-09-17 14:17:34.000000 multicallable-6.0.1/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3488 2023-08-31 16:09:12.000000 multicallable-6.0.1/README.md
--rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-6.0.1/pyproject.toml
--rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2023-09-17 14:17:34.000000 multicallable-6.0.1/setup.cfg
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      476 2023-09-17 14:17:05.000000 multicallable-6.0.1/src/multicallable/__init__.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     5373 2023-08-31 16:30:15.000000 multicallable-6.0.1/src/multicallable/async_multicallable.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable/multicall/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      172 2023-08-31 16:09:12.000000 multicallable-6.0.1/src/multicallable/multicall/__init__.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     5318 2023-09-17 14:13:49.000000 multicallable-6.0.1/src/multicallable/multicall/async_multicall.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     7598 2023-08-12 14:14:55.000000 multicallable-6.0.1/src/multicallable/multicall/constants.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4979 2023-09-17 14:16:08.000000 multicallable-6.0.1/src/multicallable/multicall/multicall.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3610 2023-08-31 16:09:12.000000 multicallable-6.0.1/src/multicallable/multicallable.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     1162 2023-08-31 16:09:12.000000 multicallable-6.0.1/src/multicallable/utils.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable.egg-info/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4037 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable.egg-info/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)      508 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable.egg-info/SOURCES.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable.egg-info/dependency_links.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2023-09-17 14:17:34.000000 multicallable-6.0.1/src/multicallable.egg-info/top_level.txt
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2024-05-01 15:22:51.474564 multicallable-6.0.2/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-6.0.2/LICENCE
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4037 2024-05-01 15:22:51.474564 multicallable-6.0.2/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     3488 2023-08-31 16:09:12.000000 multicallable-6.0.2/README.md
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-6.0.2/pyproject.toml
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2024-05-01 15:22:51.474564 multicallable-6.0.2/setup.cfg
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2024-05-01 15:22:51.470564 multicallable-6.0.2/src/
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2024-05-01 15:22:51.472564 multicallable-6.0.2/src/multicallable/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      476 2024-05-01 15:19:57.000000 multicallable-6.0.2/src/multicallable/__init__.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     5373 2023-08-31 16:30:15.000000 multicallable-6.0.2/src/multicallable/async_multicallable.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2024-05-01 15:22:51.473564 multicallable-6.0.2/src/multicallable/multicall/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      172 2023-08-31 16:09:12.000000 multicallable-6.0.2/src/multicallable/multicall/__init__.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     5318 2023-09-17 14:13:49.000000 multicallable-6.0.2/src/multicallable/multicall/async_multicall.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     7598 2023-08-12 14:14:55.000000 multicallable-6.0.2/src/multicallable/multicall/constants.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     5433 2024-05-01 15:16:47.000000 multicallable-6.0.2/src/multicallable/multicall/multicall.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     3610 2023-08-31 16:09:12.000000 multicallable-6.0.2/src/multicallable/multicallable.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     1162 2023-08-31 16:09:12.000000 multicallable-6.0.2/src/multicallable/utils.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2024-05-01 15:22:51.473564 multicallable-6.0.2/src/multicallable.egg-info/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4037 2024-05-01 15:22:51.000000 multicallable-6.0.2/src/multicallable.egg-info/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      508 2024-05-01 15:22:51.000000 multicallable-6.0.2/src/multicallable.egg-info/SOURCES.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2024-05-01 15:22:51.000000 multicallable-6.0.2/src/multicallable.egg-info/dependency_links.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2024-05-01 15:22:51.000000 multicallable-6.0.2/src/multicallable.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `multicallable-6.0.1/LICENCE` & `multicallable-6.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/PKG-INFO` & `multicallable-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 6.0.1
+Version: 6.0.2
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multicallable-6.0.1/README.md` & `multicallable-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/setup.cfg` & `multicallable-6.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multicallable
-version = 6.0.1
+version = 6.0.2
 author = Hassan Abbasi, Mojtaba Farokhi
 author_email = hassan.abbp@gmail.com
 description = Easy way to work with Multicall package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deusfinance/multicallable
 project_urls =
```

### Comparing `multicallable-6.0.1/src/multicallable/async_multicallable.py` & `multicallable-6.0.2/src/multicallable/async_multicallable.py`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/src/multicallable/multicall/async_multicall.py` & `multicallable-6.0.2/src/multicallable/multicall/async_multicall.py`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/src/multicallable/multicall/constants.py` & `multicallable-6.0.2/src/multicallable/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/src/multicallable/multicall/multicall.py` & `multicallable-6.0.2/src/multicallable/multicall/multicall.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 """
 
 from typing import List, Union
 
 from eth_abi import decode
 from web3 import Web3
 from web3.contract import Contract
+from web3.exceptions import BadFunctionCallOutput
 
 from .constants import MULTICALL_ABI, MULTICALL_ADDRESS, CHAIN_NANE, DEFAULT_MAKER_DAO_MULTICALL_ADDRESS
 from ..utils import get_type
 
 
 class Call:
     """
@@ -133,26 +134,32 @@
             kwargs = dict(block_identifier=block_identifier)
         else:
             kwargs = dict()
         block_number, block_hash, return_data = self.contract.functions.tryBlockAndAggregate(
             require_success, [(call.target, call.call_data) for call in calls]).call(**kwargs)
 
         outputs = []
-        for call, result in zip(calls, return_data):
-            success, data = result
-            if not success or not data:
+        for call, (success, data) in zip(calls, return_data):
+            if not success:
                 try:
-                    error_message = ''.join(chr(c) for c in data[-32:] if c)
+                    error_message = ''.join(chr(c) for c in data if chr(c).isprintable())
                 except:
                     error_message = 'Error'
                 outputs.append(ValueError(error_message))
                 continue
             for item in call.abi:
                 if item.get('name') == call.fn_name:
                     out_types = tuple(get_type(schema) for schema in item['outputs'])
+                    if out_types and not data:
+                        if require_success:
+                            raise BadFunctionCallOutput("Could not call contract function for a Call. "
+                                                        "Check Call's contract address correctness.")
+                        else:
+                            outputs.append(BadFunctionCallOutput())
+                            break
                     decoded_output = decode(out_types, data)
                     if len(item['outputs']) == 1:
                         decoded_output = decoded_output[0]
                     outputs.append(decoded_output)
                     break
 
         return block_number, block_hash, outputs
```

### Comparing `multicallable-6.0.1/src/multicallable/multicallable.py` & `multicallable-6.0.2/src/multicallable/multicallable.py`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/src/multicallable/utils.py` & `multicallable-6.0.2/src/multicallable/utils.py`

 * *Files identical despite different names*

### Comparing `multicallable-6.0.1/src/multicallable.egg-info/PKG-INFO` & `multicallable-6.0.2/src/multicallable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 6.0.1
+Version: 6.0.2
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

