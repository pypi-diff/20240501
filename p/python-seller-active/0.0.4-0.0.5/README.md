# Comparing `tmp/python_seller_active-0.0.4.tar.gz` & `tmp/python_seller_active-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_seller_active-0.0.4.tar", last modified: Wed Apr 19 07:16:08 2023, max compression
+gzip compressed data, was "python_seller_active-0.0.5.tar", last modified: Wed May  1 13:56:43 2024, max compression
```

## Comparing `python_seller_active-0.0.4.tar` & `python_seller_active-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/python_seller_active.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 07:16:08.000000 python_seller_active-0.0.4/python_seller_active.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/bundles/bundles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/inventory/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/locations/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/locations/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/orders/orders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.654428 python_seller_active-0.0.4/seller_active/api/rate_limit_status/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/rate_limit_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/api/rate_limit_status/rate_limit_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/seller_active/base/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/seller_active/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 07:16:08.658428 python_seller_active-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-19 07:15:51.000000 python_seller_active-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.074941 python_seller_active-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-01 13:56:43.074941 python_seller_active-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/python_seller_active.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-01 13:56:43.000000 python_seller_active-0.0.5/python_seller_active.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-01 13:56:43.000000 python_seller_active-0.0.5/python_seller_active.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:56:43.000000 python_seller_active-0.0.5/python_seller_active.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:56:43.000000 python_seller_active-0.0.5/python_seller_active.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:56:43.000000 python_seller_active-0.0.5/python_seller_active.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/bundles/bundles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/inventory/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/locations/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/orders/orders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/api/rate_limit_status/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/rate_limit_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/api/rate_limit_status/rate_limit_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:56:43.070941 python_seller_active-0.0.5/seller_active/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/seller_active/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 13:56:43.074941 python_seller_active-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-01 13:56:35.000000 python_seller_active-0.0.5/setup.py
```

### Comparing `python_seller_active-0.0.4/LICENSE` & `python_seller_active-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/PKG-INFO` & `python_seller_active-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: python_seller_active
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper around SellerActive.com API
 Home-page: https://github.com/yberezkin/python_seller_active
 Author: Yan Berezkin
 Author-email: yan.berezkin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yberezkin/python_seller_active/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # SELLER-ACTIVE-API Python Wrapper
 
 [![CodeFactor](https://www.codefactor.io/repository/github/yberezkin/python_seller_active/badge)](https://www.codefactor.io/repository/github/yberezkin/python_seller_active)
 
 This project provides a Python wrapper for interacting with the [rest.selleractive.com](https://rest.selleractive.com/) API, allowing developers to easily integrate the API's functionality into their Python applications.
```

### Comparing `python_seller_active-0.0.4/README.md` & `python_seller_active-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/python_seller_active.egg-info/PKG-INFO` & `python_seller_active-0.0.5/python_seller_active.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: python-seller-active
-Version: 0.0.4
+Name: python_seller_active
+Version: 0.0.5
 Summary: Wrapper around SellerActive.com API
 Home-page: https://github.com/yberezkin/python_seller_active
 Author: Yan Berezkin
 Author-email: yan.berezkin@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yberezkin/python_seller_active/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # SELLER-ACTIVE-API Python Wrapper
 
 [![CodeFactor](https://www.codefactor.io/repository/github/yberezkin/python_seller_active/badge)](https://www.codefactor.io/repository/github/yberezkin/python_seller_active)
 
 This project provides a Python wrapper for interacting with the [rest.selleractive.com](https://rest.selleractive.com/) API, allowing developers to easily integrate the API's functionality into their Python applications.
```

### Comparing `python_seller_active-0.0.4/python_seller_active.egg-info/SOURCES.txt` & `python_seller_active-0.0.5/python_seller_active.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/api/bundles/bundles.py` & `python_seller_active-0.0.5/seller_active/api/bundles/bundles.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/api/inventory/inventory.py` & `python_seller_active-0.0.5/seller_active/api/inventory/inventory.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/api/locations/locations.py` & `python_seller_active-0.0.5/seller_active/api/locations/locations.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/api/orders/orders.py` & `python_seller_active-0.0.5/seller_active/api/orders/orders.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/base/api_response.py` & `python_seller_active-0.0.5/seller_active/base/api_response.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/seller_active/base/base.py` & `python_seller_active-0.0.5/seller_active/base/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .helpers import params_override
 
 logger = logging.getLogger(__name__)
 
 
 class BaseClient:
     SCHEME = "https://"
-    HOST = "rest.selleractive.com"
+    HOST = "legacy.api.channels.cart.com"
     API_VERSION = "api"
     USER_AGENT = f"{__package_name__}-{__version__}"
 
     def __init__(self, seller_id: str, api_key: str):
         self.seller_id = seller_id
         self.api_key = api_key
```

### Comparing `python_seller_active-0.0.4/seller_active/base/helpers.py` & `python_seller_active-0.0.5/seller_active/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python_seller_active-0.0.4/setup.py` & `python_seller_active-0.0.5/setup.py`

 * *Files identical despite different names*

