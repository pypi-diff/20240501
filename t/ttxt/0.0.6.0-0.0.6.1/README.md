# Comparing `tmp/ttxt-0.0.6.0.tar.gz` & `tmp/ttxt-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.6.0.tar", last modified: Thu Apr 11 11:59:37 2024, max compression
+gzip compressed data, was "ttxt-0.0.6.1.tar", last modified: Wed May  1 15:59:51 2024, max compression
```

## Comparing `ttxt-0.0.6.0.tar` & `ttxt-0.0.6.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.081111 ttxt-0.0.6.0/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.0/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-11 11:59:37.080955 ttxt-0.0.6.0/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.0/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-04-11 11:59:37.081189 ttxt-0.0.6.0/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-04-11 11:59:35.000000 ttxt-0.0.6.0/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.070288 ttxt-0.0.6.0/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-04-05 05:36:17.000000 ttxt-0.0.6.0/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.071681 ttxt-0.0.6.0/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.0/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.0/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.0/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.078888 ttxt-0.0.6.0/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.0/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11279 2024-04-06 07:37:14.000000 ttxt-0.0.6.0/ttxt/exchanges/ascendex.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.0/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.0/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.0/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.0/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.0/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.0/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    20701 2024-04-11 11:59:21.000000 ttxt-0.0.6.0/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.0/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.0/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.0/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.0/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.0/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.0/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.0/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.0/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.0/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.079071 ttxt-0.0.6.0/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.0/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9863 2024-04-06 07:37:14.000000 ttxt-0.0.6.0/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.079383 ttxt-0.0.6.0/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.0/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.0/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.080237 ttxt-0.0.6.0/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.0/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.0/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.0/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-11 11:59:37.071070 ttxt-0.0.6.0/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-11 11:59:37.000000 ttxt-0.0.6.0/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-04-11 11:59:37.000000 ttxt-0.0.6.0/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-04-11 11:59:37.000000 ttxt-0.0.6.0/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-04-11 11:59:37.000000 ttxt-0.0.6.0/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.365886 ttxt-0.0.6.1/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.1/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-01 15:59:51.365739 ttxt-0.0.6.1/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.1/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-01 15:59:51.365930 ttxt-0.0.6.1/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-01 15:59:41.000000 ttxt-0.0.6.1/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.355712 ttxt-0.0.6.1/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1040 2024-04-20 13:49:26.000000 ttxt-0.0.6.1/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.356713 ttxt-0.0.6.1/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.1/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.1/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.1/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.363596 ttxt-0.0.6.1/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.1/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.1/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.1/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.1/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.1/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.1/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.1/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    21581 2024-05-01 15:58:33.000000 ttxt-0.0.6.1/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.1/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.1/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.1/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.1/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.1/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.1/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.1/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.1/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.1/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.363800 ttxt-0.0.6.1/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.1/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10063 2024-05-01 15:36:07.000000 ttxt-0.0.6.1/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.364293 ttxt-0.0.6.1/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.1/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.1/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.364950 ttxt-0.0.6.1/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.1/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.1/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.1/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-01 15:59:51.356260 ttxt-0.0.6.1/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      844 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-01 15:59:51.000000 ttxt-0.0.6.1/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.6.0/LICENSE` & `ttxt-0.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/__init__.py` & `ttxt-0.0.6.1/ttxt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from ttxt.base import baseFuturesExchange, baseSpotExchange
-from ttxt.exchanges.ascendex import ascendex
 from ttxt.exchanges.gateFutures import gateFutures
 from ttxt.exchanges.bybitFutures import bybitFutures
 from ttxt.exchanges.bitgetFutures import bitgetFutures
 from ttxt.exchanges.bingx import bingx
 from ttxt.exchanges.biconomy import biconomy
 from ttxt.exchanges.mexc import mexc
 from ttxt.exchanges.gateio import gateio
@@ -13,15 +12,14 @@
 from ttxt.exchanges.bitmart import bitmart
 from ttxt.exchanges.cryptocom import cryptocom
 from ttxt.exchanges.bitget import bitget
 from ttxt.exchanges.binance import binance
 from ttxt.exchanges.kucoin import kucoin
 
 exchanges = [
-    "ascendex",
     "biconomy",
     "binance",
     "bingx",
     "bitgetFutures",
     "bitget",
     "bybitFutures",
     "gateFutures",
```

### Comparing `ttxt-0.0.6.0/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.6.1/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.6.1/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/ascendex.py` & `ttxt-0.0.6.1/ttxt/exchanges/bitget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,268 +1,308 @@
-from ast import parse
+from email import header
 import hmac
 import base64
 import hashlib
 import json
-import re
 import time
+from wsgiref import headers
 import requests
 from urllib.parse import urlencode
 from ttxt.utils import general
-from ttxt.base import baseFuturesExchange
+from ttxt.base import baseSpotExchange
 from ttxt.types import baseTypes
 
-# password is account group, which is required for private api calls and private wss
-# naming it "password" to keep creds standard
-class ascendex(baseFuturesExchange.BaseFuturesExchange):
+
+class bitget(baseSpotExchange.BaseSpotExchange):
     def __init__(self, key, secret, password, **kwargs):
         super().__init__(key, secret, **kwargs)
-        self.group = password
-        self.category = kwargs["category"] if "category" in kwargs else "cash"  # can also be "margin"
-        self.domain_url = "https://ascendex.com"
-        self.prefix = "api/pro/v1"
+        self.domain_url = "https://api.bitget.com"
+        self.password = password
+        self.success_sode = '00000'
         
-    ## Auth
-    def hmac_sha256(self, secret, pre_hash_msg):
-        return hmac.new(secret.encode('utf-8'), pre_hash_msg.encode('utf-8'), hashlib.sha256).digest()
-
-    def sign(self, msg, secret):
-        msg = bytearray(msg.encode("utf-8"))
-        hmac_key = base64.b64decode(secret)
-        signature = hmac.new(hmac_key, msg, hashlib.sha256)
-        signature_b64 = base64.b64encode(signature.digest()).decode("utf-8")
-        return signature_b64
+    def _getSymbol(self, symbol):
+        return symbol.replace("/", "")
     
-    def utc_timestamp(self):
-        return int(round(time.time() * 1e3))
-
-    def make_auth_headers(self, timestamp, preHashString, apikey, secret):
-        # convert timestamp to string   
-        if isinstance(timestamp, bytes):
-            timestamp = timestamp.decode("utf-8")
-        elif isinstance(timestamp, int):
-            timestamp = str(timestamp)
-        header = {
-            "x-auth-key": apikey,
-            "x-auth-signature": self.sign(f"{timestamp}+{preHashString}", secret),
-            "x-auth-timestamp": timestamp,
-        }
-        return header
+    def _getUserSymbol(self, symbol):
+        raise NotImplementedError("method not implemented")
     
-    def _signedRequest(self, request_path, method, preHashString, params=None, body=None):
-        ts = self.utc_timestamp()
-        headers = self.make_auth_headers(ts, preHashString, self.key, self.secret)
-        url = f"{self.domain_url}/{self.group}/{self.prefix}/{request_path}"
+    ## Auth 
+    def sign(self, message):
+        mac = hmac.new(bytes(self.secret, encoding='utf-8'), bytes(message, encoding='utf-8'), digestmod='sha256')
+        d = mac.digest()
+        return base64.b64encode(d)
+    
+    def pre_hash(self, timestamp, method, request_path, queryString, body=None):
+        if not body:
+            return str(timestamp) + str.upper(method) + request_path + queryString
+        return str(timestamp) + str.upper(method) + request_path + body
+    
+    def parse_params_to_str(self, params):
+        params = [(key, val) for key, val in params.items()]
+        params.sort(key=lambda x:x[0])
+        url = "?" + urlencode(params)
+        if url == '?':
+            return ''
+        return url
+    
+    def generate_timestamp(self):
+        return int(time.time() * 10**3)
+    
+    def _signedRequest(self, method, request_path, queryString, body):
+        timeMs = self.generate_timestamp()
+        if method == "POST":
+            body = json.dumps(body)
+            queryString = json.dumps(queryString) if queryString is not None else ''
+            signature = self.sign(self.pre_hash(timeMs, method, request_path, queryString ,body))
+            headers = {"ACCESS-KEY": self.key, "ACCESS-SIGN": signature, "ACCESS-PASSPHRASE": self.password, "ACCESS-TIMESTAMP": str(timeMs), "locale": "en-US", "Content-Type": "application/json"}
+            url = self.domain_url+request_path
+            try:
+                response = requests.post(url, headers=headers, data=body)
+                return response.json()
+            except Exception as e:
+                raise e
         if method == "GET":
+            params = queryString
+            body = ""
+            request_path = request_path + self.parse_params_to_str(params)
+            signature = self.sign(self.pre_hash(timeMs, "GET", request_path, str(body)))
+            headers = {"ACCESS-KEY": self.key, "ACCESS-SIGN": signature, "ACCESS-PASSPHRASE": self.password, "ACCESS-TIMESTAMP": str(timeMs), "locale": "en-US", "Content-Type": "application/json"}
+            url = self.domain_url+request_path
             try:
-                response = requests.get(url, headers=headers, params=params)
+                response = requests.get(url, headers=headers)
                 return response.json()
             except Exception as e:
                 raise e
-        # elif method == "POST":
-        else:
+    
+    def _unsignedRequest(self, method, apiUrl, params):
+        url = self.domain_url + apiUrl
+        if method == 'GET':
             try:
-                response = requests.request(method, url, headers=headers, json=body)
+                response = requests.request('get', url, params=params)
                 return response.json()
             except Exception as e:
                 raise e
+        else:
+            raise Exception(f"{method} Method not supported for unsigned calls")
     
     ## parsers
     def _parseBalance(self, balData):
         parsedBal = {"free": {}, "total": {}}
-        if balData['code'] != 0: raise Exception(balData['message'])
+        if balData['code'] != '00000': 
+            raise Exception(balData['msg'])
         data = balData.get("data", None)
         if data is not None:
             for element in data:
-                parsedBal['total'][element["asset"]] = element.get('totalBalance', None)
-                parsedBal['free'][element["asset"]] = element.get('availableBalance', None)
+                parsedBal["free"][element["coin"]] = element.get("available", None)
+                parsedBal["total"][element["coin"]] = str(float(element['available'])+float(element['frozen']))
         return parsedBal
-
-    def _parseCreateOrder(self, order):
-        parsedOrder = {}
-        if order['code'] != 0: raise Exception(order['message'])
-        if "data" in order and "info" in order["data"]:
-            parsedOrder["id"] = order['data']["info"]["orderId"]
-        elif "id" in order:
-            parsedOrder["id"] = order['id']
-        parsedOrder["symbol"] = None
-        parsedOrder["price"] = None
-        parsedOrder["amount"] = None
-        parsedOrder["side"] = None
-        parsedOrder["timestamp"] = None
-        parsedOrder["status"] = None
-        parsedOrder["orderJson"] = json.dumps(order)
-        return parsedOrder
     
-    def _parseCancelorder(self, order):
+    def _parseCreateorder(self, order):
+        if order['code'] != '00000': 
+            raise Exception(order['msg'])
         parsedOrder = {'id': None, "symbol": None, "amount": None, "side": None, "timestamp": None, "status": None, "orderJson": None}
-        if order['code'] != 0: raise Exception(order['message'])
-        if 'data' in order and 'info' in order['data']:
-            element = order['data']['info']
-            parsedOrder['id'] = element.get("orderId",None)
-            parsedOrder['symbol'] = element.get("symbol",None)
-            parsedOrder['timestamp'] = element.get("timestamp",None)
-            parsedOrder["orderJson"] = json.dumps(element) if element else None
+        if "data" in order and order["data"] != {}:
+            parsedOrder['id'] = order['data']['orderId']
+            parsedOrder["orderJson"] = json.dumps(order)
         return parsedOrder
-        
-    def _parseOpenOrders(self, order):
-        parsedOrderList = []
-        if order['code'] != 0: raise Exception(order['message'])
-        if "data" in order:
-            for element in order['data']:
-                parsedOrderList.append(self._parseOrder(element))
+    
+    def _parseOpenOrders(self, orderjson):
+        if orderjson['code'] != '00000': 
+            raise Exception(orderjson['msg'])
+        parsedOrderList = []    
+        if "data" in orderjson and orderjson['data'] != {}:
+            for order in orderjson["data"]:
+                order['price'] = order['priceAvg']
+                parsedOrderList.append(self._parseOrder(order))
         return parsedOrderList
     
     def _parseOrder(self, order):
         parsedOrder = {}
         parsedOrder["id"] = order.get('orderId', None)
         parsedOrder["symbol"] = order.get('symbol', None)
         parsedOrder["price"] = float(order["price"]) if "price" in order else None 
-        parsedOrder["amount"] = float(order["orderQty"]) if "orderQty" in order else None
+        parsedOrder["amount"] = float(order["size"]) if "size" in order else None
         parsedOrder["side"] = order['side'].lower() if "side" in order else None
-        parsedOrder["timestamp"] = int(order["lastExecTime"]) if "lastExecTime" in order else None
+        parsedOrder["timestamp"] = int(order["cTime"]) if "cTime" in order else None
         parsedOrder["status"] = order.get("status", None)
         parsedOrder["orderJson"] = json.dumps(order) if order else None 
         return parsedOrder
-        
-    def _parseFetchOrder(self, order):
-        if order['code'] != 0: raise Exception(order['message'])
+    
+    def _parseFetchOrder(self, data):
         parsedOrder = {"id": None, "symbol": None, "price": None, "amount": None, "takerOrMaker": None, "datetime": None, "fee": None, "fee_currency": None,
                        "side": None, "timestamp": None, "status": None}
-        if "data" in order and order["data"] != {}:
-            order = order['data']
+        if "data" in data and data["data"] != {}:
+            order = data['data']
+            if type(order) == list:
+                order = order[0]
             parsedOrder["id"] = order["orderId"]
+            parsedOrder["tradeId"] = order.get("tradeId", None)
             parsedOrder["symbol"] = order["symbol"]
-            parsedOrder["price"] = float(order["price"])
+            if "price" in order:
+                parsedOrder["price"] = float(order["price"])
+            else:
+                parsedOrder["price"] = float(order["priceAvg"])
             parsedOrder['takerOrMaker'] = order.get('tradeScope', None)
-            parsedOrder["amount"] = float(order["orderQty"])
+            parsedOrder["amount"] = float(order["size"])
             parsedOrder["side"] = order["side"].lower()
-            parsedOrder["timestamp"] = int(order["lastExecTime"])
+            parsedOrder["timestamp"] = int(order["uTime"])
             parsedOrder["datetime"] = general.ts_to_datetime(parsedOrder["timestamp"])
             parsedOrder["status"] = order.get('status', None)
-            parsedOrder["fee_currency"] = order["feeAsset"]
+            parsedOrder['fee'] = order.get("feeDetail", None).get('totalFee', None) if order.get("feeDetail", None) is not None else None
+            parsedOrder["fee_currency"] = order["feeDetail"].get('feeCoin', None)
         return parsedOrder
-        
-        
-    def _parseFetchTrades(self, order):
-        if order['code'] != 0: raise Exception(order['message'])
+    
+    def _parseFetchTrades(self, orderjson):
+        if orderjson['code'] != '00000': 
+            raise Exception(orderjson['msg'])
         parsedTradesList = []
-        if "data" in order and order["data"] != []:
-            for element in order['data']:
-                parsedTradesList.append(self._parseOrder({'data': element}))
+        if "data" in orderjson and orderjson["data"] != []:
+            for order in orderjson["data"]:
+                parsedTradesList.append(self._parseFetchOrder({'data': order}))
         return parsedTradesList
-        
-    ## Exchange functions
+    
+    def _parseCancelorder(self, order):
+        if order['code'] != '00000': 
+            raise Exception(order['msg'])
+        parsedOrder = {'id': None, "symbol": None, "amount": None, "side": None, "timestamp": None, "status": None, "orderJson": None}
+        if "data" in order and order["data"] != {}:
+            parsedOrder['id'] = order['data']['orderId']
+        return parsedOrder
+    
+    ## Exchange functions 
     def fetch_ticker(self, symbol):
         raise NotImplementedError("method not implemented")
     
     def fetch_balance(self, params={}) -> baseTypes.Balances:
-        apiUrl = f'{self.category}/balance'
-        params = {"showAll": False}
-        preHashString = "balance"
+        apiUrl = "/api/v2/spot/account/assets"
         try:
-            resp = self._signedRequest(method="GET", request_path=apiUrl, preHashString=preHashString ,params=params)
+            resp = self._signedRequest('GET', apiUrl, params, '')
             return self._parseBalance(resp)
         except Exception as e:
             raise e
-    
-    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
-        apiUrl = f'{self.category}/order/hist/current'
-        preHashString = "order/hist/current"
-        params = {
-            "symbol": symbol
-        }
-        if limit:
-            params['n'] = limit
+        
+    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}): 
+        apiUrl = "/api/v2/spot/trade/fills"
         try:
-            resp = self._signedRequest(method="GET", request_path=apiUrl, preHashString=preHashString, params=params)
-            return self._parseFetchTrades(resp)
+            params = {
+                "symbol": self._getSymbol(symbol)
+            }
+            if since:
+                params["startTime"] = since
+            if 'endTime' in params and params['endTime']:
+                params['endTime'] = params['endTime']
+            if limit:
+                params['limit'] = limit
+            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
+            return self._parseFetchTrades(response)
         except Exception as e:
             raise e
     
     def create_order(self, symbol, side, amount, order_type, price=None, params={}): 
+        apiUrl = "/api/v2/spot/trade/place-order"
+        params = {
+            "symbol": self._getSymbol(symbol),
+            "force": "GTC",
+            "side": side.lower(),
+            "size": str(amount)
+        }
         try:
-            if order_type == "limit":
-                return self.create_limit_order(symbol, amount, side, price, params={})
-            elif order_type == "market":
-                return self.create_market_order(symbol, amount, side, params={})
+            if order_type == 'limit':
+                params["orderType"] = "limit"
+                params['price'] = str(price)
+            elif order_type == 'market':
+                params["orderType"] = "market"
+            params.update(params) 
+            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
+            return self._parseCreateorder(response)
         except Exception as e:
             raise e
     
-    def create_market_order(self, symbol, amount, side, params={}):
-        apiUrl = f"{self.category}/order"
-        preHashString = "order"
-        body = {    
-            'account-group': self.group,
-            'account-category': self.category,
-            'symbol': symbol,
-            'time': self.utc_timestamp(),
-            'orderQty': str(amount),    
-            'orderType': "market",
-            'side': side,  # buy or sell,
+    def create_market_order(self, symbol, side, amount, params={}):
+        apiUrl = "/api/v2/spot/trade/place-order"
+        params = {
+            "symbol": self._getSymbol(symbol),
+            "orderType": "market",
+            "side": side.lower(),
+            "size": str(amount)
         }
         try:
-            resp = self._signedRequest(method="POST", request_path=apiUrl, preHashString=preHashString, body=body)
-            return self._parseCreateOrder(resp)
+            params.update(params) 
+            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
+            return self._parseCreateorder(response)
         except Exception as e:
             raise e
     
-    def create_limit_order(self, symbol, amount, side, price, params={}):
-        apiUrl = f"{self.category}/order"
-        preHashString = "order"
-        body = {
-            'account-group': self.group,
-            'account-category': self.category,
-            'symbol': symbol,
-            'time': self.utc_timestamp(),
-            'orderQty': str(amount),
-            'orderPrice': str(price),
-            'orderType': "limit",
-            'side': side,  # buy or sell,
+    def create_limit_order(self, symbol, side, amount, price, params={}):
+        apiUrl = "/api/v2/spot/trade/place-order"
+        params = {
+            "symbol": self._getSymbol(symbol),
+            "orderType": "limit",
+            "force": "GTC",
+            "side": side.lower(),
+            "price": str(price),
+            "size": str(amount)
         }
         try:
-            resp = self._signedRequest(method="POST", request_path=apiUrl, preHashString=preHashString, body=body)
-            return self._parseCreateOrder(resp)
+            params.update(params) 
+            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
+            return self._parseCreateorder(response)
         except Exception as e:
             raise e
     
     def cancel_order(self, id=None, symbol=None, params={}):
-        apiUrl = f"{self.category}/order"
-        preHashString = "order"
+        apiUrl = "/api/v2/spot/trade/cancel-order"
+        ticker = self._getSymbol(symbol)
         try:
-            params = {
-                "orderId": id,
-                "time": self.utc_timestamp()
-            }
-            if symbol:
-                params['symbol'] = symbol
-            response = self._signedRequest(method='DELETE', request_path=apiUrl, preHashString=preHashString, body=params)
+            params={}
+            if id is not None:
+                params['orderId'] = id
+            if symbol is not None:
+                params['symbol'] = str(ticker)
+            params.update(params)
+            response = self._signedRequest('POST', request_path=apiUrl, queryString='',body=params)
             return self._parseCancelorder(response)
         except Exception as e:
             raise e
     
     def fetch_open_orders(self, symbol=None, kwargs=None):
-        apiUrl = f"{self.category}/order/open"
-        preHashString="order/open"
+        apiUrl = "/api/v2/spot/trade/unfilled-orders"
+        ticker = self._getSymbol(symbol)
         try:
-            params = {}
-            if symbol:
-                params['symbol'] = symbol
-            response = self._signedRequest(method='GET', request_path=apiUrl, preHashString=preHashString, params=None, body=None)
+            params = {
+                'symbol': ticker,
+                'endTime': self.generate_timestamp(),
+                'limit': 100,
+            }
+            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
             return self._parseOpenOrders(response)
         except Exception as e:
             raise e
     
     def fetch_order(self, id, symbol = None, params={}):
-        apiUrl = f"{self.category}/order/status"
-        preHashString="order/status"
+        apiUrl = "/api/v2/spot/trade/orderInfo"
         try:
             params = {
-                "orderId": id
+                'orderId': id
             }
-            response = self._signedRequest(method='GET', request_path=apiUrl, preHashString=preHashString, params=params, body=None)
+            params.update(params)
+            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
             return self._parseFetchOrder(response)
         except Exception as e:
             raise e
-        
-# https://ascendex.github.io/ascendex-pro-api/#generate-order-id
-# https://github.com/ascendex/ascendex-pro-api-demo/blob/main/signature_demo/python/signature.py
+
+    ## use case specifci request    
+    def sub_account_transfer(self, amount, fromUserId, toUserId, coin, fromType="spot", toType="spot"):
+        apiUrl = "/api/v2/spot/wallet/subaccount-transfer"
+        params = {
+            "fromType": fromType,
+            "toType": toType,
+            "amount": amount,
+            "coin": coin,
+            "fromUserId": fromUserId,
+            "toUserId": toUserId
+        }
+        try:
+            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
+            return response
+        except Exception as e:
+            raise e
```

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/biconomy.py` & `ttxt-0.0.6.1/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/binance.py` & `ttxt-0.0.6.1/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bingx.py` & `ttxt-0.0.6.1/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bitget.py` & `ttxt-0.0.6.1/ttxt/exchanges/okx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,308 +1,296 @@
-from email import header
 import hmac
 import base64
 import hashlib
 import json
 import time
-from wsgiref import headers
 import requests
-from urllib.parse import urlencode
-from ttxt.utils import general
+import datetime
 from ttxt.base import baseSpotExchange
 from ttxt.types import baseTypes
+from ttxt.utils import general
 
 
-class bitget(baseSpotExchange.BaseSpotExchange):
+class okx(baseSpotExchange.BaseSpotExchange):
     def __init__(self, key, secret, password, **kwargs):
         super().__init__(key, secret, **kwargs)
-        self.domain_url = "https://api.bitget.com"
         self.password = password
-        self.success_sode = '00000'
-        
+        self.domain = "https://www.okx.com"
+        ## constants
+        self.CONTENT_TYPE = 'Content-Type'
+        self.OK_ACCESS_KEY = 'OK-ACCESS-KEY'
+        self.OK_ACCESS_SIGN = 'OK-ACCESS-SIGN'
+        self.OK_ACCESS_TIMESTAMP = 'OK-ACCESS-TIMESTAMP'
+        self.OK_ACCESS_PASSPHRASE = 'OK-ACCESS-PASSPHRASE'
+        self.APPLICATION_JSON = 'application/json'
+        self.GET = "GET"
+        self.POST = "POST"
+
     def _getSymbol(self, symbol):
-        return symbol.replace("/", "")
+        return symbol.replace("/", "-")
     
     def _getUserSymbol(self, symbol):
-        raise NotImplementedError("method not implemented")
-    
+        return symbol.replace("-", "/")
+
     ## Auth 
     def sign(self, message):
-        mac = hmac.new(bytes(self.secret, encoding='utf-8'), bytes(message, encoding='utf-8'), digestmod='sha256')
+        mac = hmac.new(bytes(self.secret, encoding='utf8'), bytes(message, encoding='utf-8'), digestmod='sha256')
         d = mac.digest()
         return base64.b64encode(d)
-    
-    def pre_hash(self, timestamp, method, request_path, queryString, body=None):
-        if not body:
-            return str(timestamp) + str.upper(method) + request_path + queryString
+
+
+    def pre_hash(self, timestamp, method, request_path, body):
         return str(timestamp) + str.upper(method) + request_path + body
-    
+
+
+    def get_header(self, sign, timestamp):
+        header = dict()
+        header[self.CONTENT_TYPE] = self.APPLICATION_JSON
+        header[self.OK_ACCESS_KEY] = self.key
+        header[self.OK_ACCESS_SIGN] = sign
+        header[self.OK_ACCESS_TIMESTAMP] = str(timestamp)
+        header[self.OK_ACCESS_PASSPHRASE] = self.password
+        # header['x-simulated-trading'] = flag
+        return header
+
+    def get_header_no_sign(self):
+        header = dict()
+        header[self.CONTENT_TYPE] = self.APPLICATION_JSON
+        # header['x-simulated-trading'] = flag
+        return header
+
     def parse_params_to_str(self, params):
-        params = [(key, val) for key, val in params.items()]
-        params.sort(key=lambda x:x[0])
-        url = "?" + urlencode(params)
-        if url == '?':
-            return ''
+        url = '?'
+        for key, value in params.items():
+            if(value != ''):
+                url = url + str(key) + '=' + str(value) + '&'
+        url = url[0:-1]
         return url
-    
-    def generate_timestamp(self):
-        return int(time.time() * 10**3)
-    
-    def _signedRequest(self, method, request_path, queryString, body):
-        timeMs = self.generate_timestamp()
-        if method == "POST":
-            body = json.dumps(body)
-            queryString = json.dumps(queryString) if queryString is not None else ''
-            signature = self.sign(self.pre_hash(timeMs, method, request_path, queryString ,body))
-            headers = {"ACCESS-KEY": self.key, "ACCESS-SIGN": signature, "ACCESS-PASSPHRASE": self.password, "ACCESS-TIMESTAMP": str(timeMs), "locale": "en-US", "Content-Type": "application/json"}
-            url = self.domain_url+request_path
-            try:
-                response = requests.post(url, headers=headers, data=body)
-                return response.json()
-            except Exception as e:
-                raise e
+
+    def get_timestamp(self):
+        now = datetime.datetime.utcnow()
+        t = now.isoformat("T", "milliseconds")
+        return t + "Z"
+
+    def signature(self, timestamp, method, request_path, body):
+        if str(body) == '{}' or str(body) == 'None':
+            body = ''
+        message = str(timestamp) + str.upper(method) + request_path + str(body)
+
+        mac = hmac.new(bytes(self.secret, encoding='utf8'), bytes(message, encoding='utf-8'), digestmod='sha256')
+        d = mac.digest()
+
+        return base64.b64encode(d)
+
+    ## Requests 
+    def _signedRequest(self, method, request_path, params):
         if method == "GET":
-            params = queryString
-            body = ""
             request_path = request_path + self.parse_params_to_str(params)
-            signature = self.sign(self.pre_hash(timeMs, "GET", request_path, str(body)))
-            headers = {"ACCESS-KEY": self.key, "ACCESS-SIGN": signature, "ACCESS-PASSPHRASE": self.password, "ACCESS-TIMESTAMP": str(timeMs), "locale": "en-US", "Content-Type": "application/json"}
-            url = self.domain_url+request_path
-            try:
-                response = requests.get(url, headers=headers)
-                return response.json()
-            except Exception as e:
-                raise e
-    
-    def _unsignedRequest(self, method, apiUrl, params):
-        url = self.domain_url + apiUrl
-        if method == 'GET':
-            try:
-                response = requests.request('get', url, params=params)
-                return response.json()
-            except Exception as e:
-                raise e
+        timestamp = self.get_timestamp()
+        body = json.dumps(params) if method == "POST" else ""
+        if self.key != '-1':
+            sign = self.sign(self.pre_hash(timestamp, method, request_path, str(body)))
+            header = self.get_header(sign, timestamp)
         else:
-            raise Exception(f"{method} Method not supported for unsigned calls")
+            header = self.get_header_no_sign()
+        response = None
+        url = self.domain + request_path
+        if method == "GET":
+            response = requests.get(url, headers=header)
+        elif method == "POST":
+            response = requests.post(url, data=body, headers=header)
+        return response.json()
     
     ## parsers
     def _parseBalance(self, balData):
+        if balData['code'] != "0": raise Exception(balData["msg"])
         parsedBal = {"free": {}, "total": {}}
-        if balData['code'] != '00000': 
-            raise Exception(balData['msg'])
-        data = balData.get("data", None)
-        if data is not None:
-            for element in data:
-                parsedBal["free"][element["coin"]] = element.get("available", None)
-                parsedBal["total"][element["coin"]] = str(float(element['available'])+float(element['frozen']))
+        for bal in balData["data"][0]["details"]:
+            parsedBal["free"][bal["ccy"]] = bal.get("availBal", None)
+            parsedBal["total"][bal["ccy"]] = bal.get("eq", None)
         return parsedBal
     
-    def _parseCreateorder(self, order):
-        if order['code'] != '00000': 
-            raise Exception(order['msg'])
-        parsedOrder = {'id': None, "symbol": None, "amount": None, "side": None, "timestamp": None, "status": None, "orderJson": None}
-        if "data" in order and order["data"] != {}:
-            parsedOrder['id'] = order['data']['orderId']
-            parsedOrder["orderJson"] = json.dumps(order)
+    def _parseOrderbook(self, orderbookData):
+        parsedData = {}
+        parsedData["datetime"] = None
+        parsedData["timestamp"] = orderbookData.get("current", None)
+        parsedData["nonce"] = orderbookData.get("id", None)
+        if "bids" in orderbookData:
+            parsedData["bids"] = [[float(d[0]), float(d[1])] for d in orderbookData["bids"]]
+        else: parsedData["bids"] = []
+        if "asks" in orderbookData:
+            parsedData["asks"] = [[float(d[0]), float(d[1])] for d in orderbookData["asks"]]
+        else: parsedData["asks"] = []
+        return parsedData
+
+    def _parseCreateOrder(self, order):
+        parsedOrder = {}
+        if order['code'] != "0": raise Exception(order["msg"])
+        parsedOrder["id"] = order['data'][0]['ordId']
+        parsedOrder["symbol"] = None
+        parsedOrder["price"] = None
+        parsedOrder["amount"] = None
+        parsedOrder["side"] = None
+        parsedOrder["timestamp"] = float(order["outTime"]) if "outTime" in order else None
+        parsedOrder["status"] = None
+        parsedOrder["orderJson"] = json.dumps(order) if order else None 
         return parsedOrder
     
-    def _parseOpenOrders(self, orderjson):
-        if orderjson['code'] != '00000': 
-            raise Exception(orderjson['msg'])
-        parsedOrderList = []    
-        if "data" in orderjson and orderjson['data'] != {}:
-            for order in orderjson["data"]:
-                order['price'] = order['priceAvg']
-                parsedOrderList.append(self._parseOrder(order))
-        return parsedOrderList
-    
     def _parseOrder(self, order):
         parsedOrder = {}
-        parsedOrder["id"] = order.get('orderId', None)
-        parsedOrder["symbol"] = order.get('symbol', None)
-        parsedOrder["price"] = float(order["price"]) if "price" in order else None 
-        parsedOrder["amount"] = float(order["size"]) if "size" in order else None
-        parsedOrder["side"] = order['side'].lower() if "side" in order else None
-        parsedOrder["timestamp"] = int(order["cTime"]) if "cTime" in order else None
-        parsedOrder["status"] = order.get("status", None)
+        parsedOrder["id"] = order.get('ordId', None)
+        parsedOrder["symbol"] = self._getUserSymbol(order["instId"]) if "instId" in order else None
+        parsedOrder["price"] = float(order["px"]) if "px" in order else None 
+        parsedOrder["amount"] = float(order["sz"]) if "sz" in order else None
+        parsedOrder["side"] = order.get('side', None)
+        parsedOrder["timestamp"] = float(order["cTime"]) if "cTime" in order else None
+        parsedOrder["status"] = order["status"] if "status" in order else None
         parsedOrder["orderJson"] = json.dumps(order) if order else None 
         return parsedOrder
+
+    def _parseOpenOrders(self, orders):
+        parsedOrderList = []
+        if order['code'] != "0": raise Exception(order["msg"])
+        for order in orders['data']:
+            parsedOrderList.append(self._parseOrder(order))
+        return parsedOrderList
     
-    def _parseFetchOrder(self, data):
-        parsedOrder = {"id": None, "symbol": None, "price": None, "amount": None, "takerOrMaker": None, "datetime": None, "fee": None, "fee_currency": None,
-                       "side": None, "timestamp": None, "status": None}
-        if "data" in data and data["data"] != {}:
-            order = data['data']
-            if type(order) == list:
-                order = order[0]
-            parsedOrder["id"] = order["orderId"]
-            parsedOrder["tradeId"] = order.get("tradeId", None)
-            parsedOrder["symbol"] = order["symbol"]
-            if "price" in order:
-                parsedOrder["price"] = float(order["price"])
-            else:
-                parsedOrder["price"] = float(order["priceAvg"])
-            parsedOrder['takerOrMaker'] = order.get('tradeScope', None)
-            parsedOrder["amount"] = float(order["size"])
-            parsedOrder["side"] = order["side"].lower()
-            parsedOrder["timestamp"] = int(order["uTime"])
-            parsedOrder["datetime"] = general.ts_to_datetime(parsedOrder["timestamp"])
-            parsedOrder["status"] = order.get('status', None)
-            parsedOrder['fee'] = order.get("feeDetail", None).get('totalFee', None) if order.get("feeDetail", None) is not None else None
-            parsedOrder["fee_currency"] = order["feeDetail"].get('feeCoin', None)
-        return parsedOrder
-    
-    def _parseFetchTrades(self, orderjson):
-        if orderjson['code'] != '00000': 
-            raise Exception(orderjson['msg'])
-        parsedTradesList = []
-        if "data" in orderjson and orderjson["data"] != []:
-            for order in orderjson["data"]:
-                parsedTradesList.append(self._parseFetchOrder({'data': order}))
-        return parsedTradesList
-    
-    def _parseCancelorder(self, order):
-        if order['code'] != '00000': 
-            raise Exception(order['msg'])
-        parsedOrder = {'id': None, "symbol": None, "amount": None, "side": None, "timestamp": None, "status": None, "orderJson": None}
-        if "data" in order and order["data"] != {}:
-            parsedOrder['id'] = order['data']['orderId']
-        return parsedOrder
-    
+    def _parseTrades(self, trades):
+        def parseTrade(trade):
+            parsedTrade = {}
+            parsedTrade["symbol"] = trade.get('instId', None)
+            parsedTrade["id"] = trade.get("ordId", None)
+            parsedTrade["tradeId"] = trade.get("tradeId", None)
+            parsedTrade["side"] = trade.get("side", None)
+            parsedTrade["price"] = trade.get("fillPx", None)
+            parsedTrade["amount"] = trade.get("fillSz", None)
+            parsedTrade["takerOrMaker"] = "taker" if trade['execType'] == 'T' else "maker"
+            if "fillTime" in trade:
+                parsedTrade["timestamp"] = int(float(trade["fillTime"]))
+                parsedTrade["datetime"] = general.ts_to_datetime(parsedTrade["timestamp"])
+            else: 
+                parsedTrade["timestamp"] = None
+                parsedTrade["datetime"] = None
+            parsedTrade["feeCurrency"] = trade["feeCcy"]
+            parsedTrade["fee"] = trade["fee"]
+            return parsedTrade
+        parsedTradeList = []
+        if trades['code'] != "0": raise Exception(trades["msg"])
+        for trade in trades["data"]:
+            parsedTradeList.append(parseTrade(trade))
+        return parsedTradeList
+
     ## Exchange functions 
-    def fetch_ticker(self, symbol):
-        raise NotImplementedError("method not implemented")
-    
-    def fetch_balance(self, params={}) -> baseTypes.Balances:
-        apiUrl = "/api/v2/spot/account/assets"
+
+    def create_order(self, symbol, type, side, amount, price=None, params={}):
+        if type == "market":
+            body = {
+                "tdMode": "cash",
+                "instId": self._getSymbol(symbol),
+                "ordType": "market",
+                "side": side,
+                "iceberg": params["iceberg"] if "iceberg" in params else "0",
+                "sz": str(amount)
+            }
+        elif type == "limit":
+            body = {
+                "tdMode": "cash",
+                "instId": self._getSymbol(symbol),
+                "ordType": "limit",
+                "side": side,
+                "iceberg": params["iceberg"] if "iceberg" in params else "0",
+                "sz": str(amount),
+                "px": str(price)
+            }
+        apiUrl = f"/api/v5/trade/order"
         try:
-            resp = self._signedRequest('GET', apiUrl, params, '')
-            return self._parseBalance(resp)
+            response = self._signedRequest(method='POST', request_path=apiUrl, params=body)
+            return self._parseCreateOrder(response)
         except Exception as e:
             raise e
         
-    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}): 
-        apiUrl = "/api/v2/spot/trade/fills"
-        try:
-            params = {
-                "symbol": self._getSymbol(symbol)
-            }
-            if since:
-                params["startTime"] = since
-            if 'endTime' in params and params['endTime']:
-                params['endTime'] = params['endTime']
-            if limit:
-                params['limit'] = limit
-            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
-            return self._parseFetchTrades(response)
-        except Exception as e:
-            raise e
-    
-    def create_order(self, symbol, side, amount, order_type, price=None, params={}): 
-        apiUrl = "/api/v2/spot/trade/place-order"
-        params = {
-            "symbol": self._getSymbol(symbol),
-            "force": "GTC",
-            "side": side.lower(),
-            "size": str(amount)
+    def create_limit_order(self, symbol, amount, side, price, params={}):
+        body = {
+            "tdMode": "cash",
+            "instId": self._getSymbol(symbol),
+            "ordType": "limit",
+            "side": side,
+            "iceberg": params["iceberg"] if "iceberg" in params else "0",
+            "sz": str(amount),
+            "px": str(price)
         }
+        apiUrl = f"/api/v5/trade/order"
         try:
-            if order_type == 'limit':
-                params["orderType"] = "limit"
-                params['price'] = str(price)
-            elif order_type == 'market':
-                params["orderType"] = "market"
-            params.update(params) 
-            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
-            return self._parseCreateorder(response)
+            response = self._signedRequest(method='POST', request_path=apiUrl, params=body)
+            return self._parseCreateOrder(response)
         except Exception as e:
             raise e
-    
-    def create_market_order(self, symbol, side, amount, params={}):
-        apiUrl = "/api/v2/spot/trade/place-order"
-        params = {
-            "symbol": self._getSymbol(symbol),
-            "orderType": "market",
-            "side": side.lower(),
-            "size": str(amount)
+
+    def create_market_order(self, symbol, amount, side, params={}):
+        body = {
+            "tdMode": "cash",
+            "instId": self._getSymbol(symbol),
+            "ordType": "market",
+            "side": side,
+            "iceberg": params["iceberg"] if "iceberg" in params else "0",
+            "sz": str(amount)
         }
+        apiUrl = f"/api/v5/trade/order"
         try:
-            params.update(params) 
-            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
-            return self._parseCreateorder(response)
+            response = self._signedRequest(method='POST', request_path=apiUrl, params=body)
+            return self._parseCreateOrder(response)
         except Exception as e:
             raise e
     
-    def create_limit_order(self, symbol, side, amount, price, params={}):
-        apiUrl = "/api/v2/spot/trade/place-order"
-        params = {
-            "symbol": self._getSymbol(symbol),
-            "orderType": "limit",
-            "force": "GTC",
-            "side": side.lower(),
-            "price": str(price),
-            "size": str(amount)
-        }
+    def fetch_order(self, id, symbol=None):
+        raise NotImplementedError("method not implemented")
+
+    def fetch_open_orders(self, symbol=None,  kwargs=None):
+        apiUrl = "/api/v5/trade/orders-pending"
+        params = {"instId": self._getSymbol(symbol), "instType": "SPOT"}
         try:
-            params.update(params) 
-            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
-            return self._parseCreateorder(response)
+            response = self._signedRequest(method='GET', request_path=apiUrl, params=params)
+            return self._parseOpenOrders(response)
         except Exception as e:
             raise e
-    
-    def cancel_order(self, id=None, symbol=None, params={}):
-        apiUrl = "/api/v2/spot/trade/cancel-order"
-        ticker = self._getSymbol(symbol)
+        
+    def cancel_order(self, id, symbol=None):
+        apiUrl = "/api/v5/trade/cancel-order"
+        params = {"instId": self._getSymbol(symbol), "ordId": id}
         try:
-            params={}
-            if id is not None:
-                params['orderId'] = id
-            if symbol is not None:
-                params['symbol'] = str(ticker)
-            params.update(params)
-            response = self._signedRequest('POST', request_path=apiUrl, queryString='',body=params)
-            return self._parseCancelorder(response)
+            response = self._signedRequest(method='POST', request_path=apiUrl, params=params)
+            return self._parseCreateOrder(response)
         except Exception as e:
             raise e
+
+    def fetch_ticker(self, symbol: str, params={}) -> baseTypes.Ticker:
+        raise NotImplementedError("method not implemented")
     
-    def fetch_open_orders(self, symbol=None, kwargs=None):
-        apiUrl = "/api/v2/spot/trade/unfilled-orders"
-        ticker = self._getSymbol(symbol)
+    def fetch_balance(self, params={}) -> baseTypes.Balances:
+        apiUrl = '/api/v5/account/balance'
         try:
-            params = {
-                'symbol': ticker,
-                'endTime': self.generate_timestamp(),
-                'limit': 100,
-            }
-            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
-            return self._parseOpenOrders(response)
+            resp = self._signedRequest(method='GET', request_path=apiUrl, params=params)
+            return self._parseBalance(resp)
         except Exception as e:
             raise e
     
-    def fetch_order(self, id, symbol = None, params={}):
-        apiUrl = "/api/v2/spot/trade/orderInfo"
+    # for extra params: https://www.okx.com/docs-v5/en/#order-book-trading-trade-get-transaction-details-last-3-months
+    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
+        apiUrl = '/api/v5/trade/fills-history'
+        if symbol:
+            params['instType'] = "SPOT"
+        if limit:
+            params['limit'] = limit
+        if since:
+            params['begin'] = int(since)
         try:
-            params = {
-                'orderId': id
-            }
-            params.update(params)
-            response = self._signedRequest('GET', request_path=apiUrl, queryString=params, body='')
-            return self._parseFetchOrder(response)
+            resp = self._signedRequest(method='GET', request_path=apiUrl, params=params)
+            return self._parseTrades(resp)
         except Exception as e:
             raise e
-
-    ## use case specifci request    
-    def sub_account_transfer(self, amount, fromUserId, toUserId, coin, fromType="spot", toType="spot"):
-        apiUrl = "/api/v2/spot/wallet/subaccount-transfer"
-        params = {
-            "fromType": fromType,
-            "toType": toType,
-            "amount": amount,
-            "coin": coin,
-            "fromUserId": fromUserId,
-            "toUserId": toUserId
-        }
-        try:
-            response = self._signedRequest('POST', request_path=apiUrl, body=params, queryString='')
-            return response
-        except Exception as e:
-            raise e
+        
+    def fetch_order_book(self, symbol: str, limit=None, params={}) -> baseTypes.OrderBook:
+        raise NotImplementedError("method not implemented")
+    
+    # parsed OHLCV = [[ts_ms, o, h ,l ,c, v],[]]
+    def fetch_ohlcv(self, symbol: str, timeframe='1m', since = None, limit = None, params={}):
+        raise NotImplementedError("method not implemented")
```

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.6.1/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bitmart.py` & `ttxt-0.0.6.1/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bybit.py` & `ttxt-0.0.6.1/ttxt/exchanges/bybit.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,17 @@
             return parsedTrade
         parsedTradeList = []
         if trades['retCode'] != 0: raise Exception(trades['retMsg'])
         for trade in trades['result']['list']:
             parsedTradeList.append(parseTrade(trade))
         return parsedTradeList
 
+    def _parseAccountInfo(self, accountData):
+        if accountData['retCode'] != 0: raise Exception(accountData['retMsg'])
+        return accountData['result']
 
     ## Exchange functions 
 
     # https://www.gate.io/docs/developers/apiv4/en/#create-a-futures-order
     def create_order(self, symbol, type, side, amount, price=None, params={}):
         try:
             ticker = self._getSymbol(symbol)
@@ -465,17 +468,24 @@
         try:
             resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams)
             return resp # parse this response into Ticker
         except Exception as e:
             raise e
     
     def fetch_balance(self, params={}) -> baseTypes.Balances:
-        apiUrl = '/v5/account/wallet-balance'
         queryParams = {"accountType": self.account_type}
         try:
+            accountInfo = self.fetch_account_info()
+            if accountInfo['unifiedMarginStatus'] == 1:
+                queryParams = {"accountType": "SPOT"}
+                apiUrl = "/v5/asset/transfer/query-account-coins-balance"
+            elif accountInfo['marginMode'] != 'REGULAR_MARGIN':
+                apiUrl = "/v5/spot-cross-margin-trade/account"
+            else:
+                apiUrl = '/v5/account/wallet-balance'
             resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams, auth=True)
             return self._parseBalance(resp)
         except WrongAccountType as e:
             apiUrl = "/v5/asset/transfer/query-account-coins-balance"
             queryParams = {"accountType": "SPOT"}
             try:
                 resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams, auth=True)
@@ -511,8 +521,18 @@
         try:
             resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams)
             return self._parseOrderbook(resp)
         except Exception as e:
             raise e
         
     def fetch_ohlcv(self, symbol: str, timeframe='1m', since = None, limit = None, params={}):
-        raise NotImplementedError("Subclasses must implement this method")
+        raise NotImplementedError("Subclasses must implement this method")
+    
+    ## extra method 
+    def fetch_account_info(self):
+        apiUrl = '/v5/account/info'
+        queryParams = {}
+        try:
+            resp = self._signedRequest(method='GET', path=apiUrl, query=queryParams, auth=True)
+            return self._parseAccountInfo(resp)
+        except Exception as e:
+            raise e
```

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.6.1/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.6.1/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.6.1/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/gateio.py` & `ttxt-0.0.6.1/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/huobi.py` & `ttxt-0.0.6.1/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/kucoin.py` & `ttxt-0.0.6.1/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/exchanges/mexc.py` & `ttxt-0.0.6.1/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/tests/testExchange.py` & `ttxt-0.0.6.1/ttxt/tests/testExchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 DIR_NAME = os.path.dirname(os.path.abspath(__file__))
 root = os.path.dirname(os.path.dirname(DIR_NAME))
 sys.path.append(root)
 
 import ttxt
 
 def getTtxtExchange(exchangeName):
-    if exchangeName == "ascendex":
-        print('returned ascendex')
-        return ttxt.ascendex(key=os.getenv("KEY"), secret=os.getenv("SECRET"), password=os.getenv("PASSWORD"))
     if exchangeName == "gateFutures":
         print("returned gateFuture")
         return ttxt.gateFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bybitFutures":
         print("returned bybitFutures")
         return ttxt.bybitFutures(key=os.getenv("KEY"), secret=os.getenv("SECRET"))
     if exchangeName == "bitgetFutures":
@@ -81,23 +78,24 @@
             print(resp)
         except Exception as e:
             print("balance could not be fetched")
             print(e)
     if "createOrder" in params and params["createOrder"]:
         print("testing create order...")
         try:
-            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="market", amount="50", side="sell", price=0.3)
+            resp = ttxtExchange.create_order(symbol=tickerToTest, order_type="limit", amount="5", side="sell", price=5)
             print(f"createOrder response: {resp}")
         except Exception as e:
             print("order could not be created")
             print(e)
     if "createLimitOrder" in params and params["createLimitOrder"]:
         print("testing limit create order...")
         try:
-            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="buy", price=0.2)
+            params = {'timeInForce': 'PostOnly'}
+            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=100, side="buy", price=0.0494, params=params)
             print(f"createLimitOrder response: {resp}")
         except Exception as e:
             print("limit order could not be created")
             print(e)
     if "createMarketSellOrder" in params and params["createMarketSellOrder"]:
         print("testing market sell create order...")
         try:
@@ -113,31 +111,31 @@
             print(f"createMarketBuyOrder response: {resp}")
         except Exception as e:
             print("market buy order could not be created")
             print(e)
     if "create_market_order" in params and params["create_market_order"]:
         print("testing create market order...")
         try:
-            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=50)
+            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=1)
             print(f"create_market_order response: {resp}")
         except Exception as e:
             print("market order could not be created")
             print(e)
     if "fetchOrder" in params and params["fetchOrder"]:
         print("testing fetch order...")
         try:
-            resp = ttxtExchange.fetch_order(id="a18eae908f85U3317077942fPhjnp6nH", symbol=tickerToTest)
+            resp = ttxtExchange.fetch_order(id=45577069671, symbol=tickerToTest)
             print(f"fetchOrder response: {resp}")
         except Exception as e:
             print("order could not be fetched")
             print(e)
     if "cancelOrder" in params and params["cancelOrder"]:
         print("testing cancel order...")
         try:
-            resp = ttxtExchange.cancel_order(id="a18eaf2a165cU3317077942BKbakNWlN", symbol=tickerToTest)
+            resp = ttxtExchange.cancel_order(id=698922787, symbol=tickerToTest)
             print(f"cancelOrder response: {resp}")
         except Exception as e:
             print("order could not be canceled")
             print(e)
     if "fetchOpenOrders" in params and params["fetchOpenOrders"]:
         print("testing open orders...")
         try:
@@ -195,29 +193,37 @@
         print("testing myTrades...")
         try:
             resp = ttxtExchange.fetch_my_trades(symbol=tickerToTest, since=1710863600671)
             print(resp)
         except Exception as e:
             print("myTrades could not be fetched")
             print(e)
+    if "accountInfo" in params and params["accountInfo"]:  # only for bybit currently (not exposed to client)
+        print("testing account info...")
+        try:
+            resp = ttxtExchange.fetch_account_info()
+            print(resp)
+        except Exception as e:
+            print("account info could not be fetched")
+            print(e)
 
 
 if __name__ == "__main__":
-    tickerToTest = "OPUL/USDT"
+    tickerToTest = "GALA/USDT"
     testingParams = {"ticker": False, 
-                     "balance": False, 
+                     "balance": True, 
                      "ohlcv": False, 
                      "createOrder": False, 
                      "fetchOrder": False, 
                      "cancelOrder": False, 
                      "fetchOpenOrders": False, 
                      "setLeverage": False, 
                      "createLimitOrder": False,
                      "createMarketSellOrder": False, 
                      "createMarketBuyOrder": False, 
                      "orderbook": False, 
                      "candlestick": False,
                      "create_market_order": False, 
                      "cancelAllOrders": False, 
-                     "myTrades": True
-                    }
-    test(params=testingParams, exchangeName="ascendex")
+                     "myTrades": False,
+                     "accountInfo": False}
+    test(params=testingParams, exchangeName="bybit")
```

### Comparing `ttxt-0.0.6.0/ttxt/types/baseTypes.py` & `ttxt-0.0.6.1/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/utils/general.py` & `ttxt-0.0.6.1/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt/utils/xtUtils.py` & `ttxt-0.0.6.1/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.0/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.6.1/ttxt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 ttxt.egg-info/SOURCES.txt
 ttxt.egg-info/dependency_links.txt
 ttxt.egg-info/top_level.txt
 ttxt/base/__init__.py
 ttxt/base/baseFuturesExchange.py
 ttxt/base/baseSpotExchange.py
 ttxt/exchanges/__init__.py
-ttxt/exchanges/ascendex.py
 ttxt/exchanges/biconomy.py
 ttxt/exchanges/binance.py
 ttxt/exchanges/bingx.py
 ttxt/exchanges/bitget.py
 ttxt/exchanges/bitgetFutures.py
 ttxt/exchanges/bitmart.py
 ttxt/exchanges/bybit.py
```

