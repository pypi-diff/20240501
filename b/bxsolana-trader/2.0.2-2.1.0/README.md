# Comparing `tmp/bxsolana_trader-2.0.2.tar.gz` & `tmp/bxsolana-trader-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana_trader-2.0.2.tar", last modified: Wed May  1 01:45:02 2024, max compression
+gzip compressed data, was "bxsolana-trader-2.1.0.tar", last modified: Mon Mar 18 18:52:17 2024, max compression
```

## Comparing `bxsolana_trader-2.0.2.tar` & `bxsolana-trader-2.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.103468 bxsolana_trader-2.0.2/bxsolana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.103468 bxsolana_trader-2.0.2/bxsolana/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      670 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/examples/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      718 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/examples/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/examples/order_lifecycle.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9198 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/examples/order_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14302 2024-05-01 01:43:37.000000 bxsolana_trader-2.0.2/bxsolana/examples/request_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5282 2024-05-01 01:43:37.000000 bxsolana_trader-2.0.2/bxsolana/examples/stream_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5194 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/examples/transaction_request_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/bxsolana/provider/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-04-23 19:58:33.000000 bxsolana_trader-2.0.2/bxsolana/provider/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1290 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2809 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/grpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32922 2024-05-01 01:43:37.000000 bxsolana_trader-2.0.2/bxsolana/provider/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/http_error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/jsonrpc_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/package_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4955 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/provider/ws.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/bxsolana/transaction/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/transaction/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/transaction/memo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/transaction/private_txs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2402 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/bxsolana/transaction/signing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-05-01 01:45:02.000000 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2024-05-01 01:45:02.000000 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-01 01:45:02.000000 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      145 2024-05-01 01:45:02.000000 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-05-01 01:45:02.000000 bxsolana_trader-2.0.2/bxsolana_trader.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      677 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/test/integration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/private.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/public.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      852 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/test_grpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/test_http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      664 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/integration/test_ws.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/test/unit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/unit/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 01:45:02.107468 bxsolana_trader-2.0.2/test/unit/transaction/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/unit/transaction/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      834 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/unit/transaction/test_memo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4629 2024-04-23 18:43:17.000000 bxsolana_trader-2.0.2/test/unit/transaction/test_signing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/examples/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      670 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      718 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/order_lifecycle.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9198 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/order_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14230 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/request_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4603 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/stream_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5194 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/examples/transaction_request_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/provider/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1290 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2809 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/grpc.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32775 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/http.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/http_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/jsonrpc_patch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      127 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/package_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4955 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/provider/ws.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana/transaction/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      535 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/memo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/private_txs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2402 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/bxsolana/transaction/signing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4618 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      145 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-03-18 18:52:17.000000 bxsolana-trader-2.1.0/bxsolana_trader.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      677 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/integration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/private.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/public.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      852 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/stream.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      701 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_grpc.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_http.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      664 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/integration/test_ws.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/unit/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:17.955932 bxsolana-trader-2.1.0/test/unit/transaction/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      834 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/test_memo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4629 2024-03-18 18:52:02.000000 bxsolana-trader-2.1.0/test/unit/transaction/test_signing.py
```

### Comparing `bxsolana_trader-2.0.2/LICENSE` & `bxsolana-trader-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/PKG-INFO` & `bxsolana-trader-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: aiohttp==3.8.1
 Requires-Dist: grpclib==0.4.3
 Requires-Dist: aiounittest==1.4.1
 Requires-Dist: base58==2.1.1
 Requires-Dist: solana==0.31.0
 Requires-Dist: solders==0.19.0
 Requires-Dist: bx-jsonrpc-py==0.2.0
-Requires-Dist: bxsolana-trader-proto==0.0.66
+Requires-Dist: bxsolana-trader-proto==0.0.63
 
 # Solana Trader Python Client
 
 Provides a Python SDK for bloXroute's Solana Trader API.
 
 ## Installation
```

### Comparing `bxsolana_trader-2.0.2/README.md` & `bxsolana-trader-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/constants.py` & `bxsolana-trader-2.1.0/bxsolana/examples/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/order_lifecycle.py` & `bxsolana-trader-2.1.0/bxsolana/examples/order_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/order_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/order_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/request_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/request_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
         (
             await api.get_jupiter_quotes(
                 get_jupiter_quotes_request=proto.GetJupiterQuotesRequest(
                     in_token="EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v",
                     out_token="So11111111111111111111111111111111111111112",
                     in_amount=0.01,
                     slippage=10,
-                    fast_mode=True,
                 )
             )
         ).to_json()
     )
 
     # trade API
     print("fetching open orders for account")
@@ -423,15 +422,14 @@
             await api.post_jupiter_swap(
                 post_jupiter_swap_request=proto.PostJupiterSwapRequest(
                     owner_address=public_key,
                     in_token="So11111111111111111111111111111111111111112",
                     in_amount=0.01,
                     out_token="EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v",
                     slippage=0.01,
-                    fast_mode=True,
                 )
             )
         )
     )
 
     print("generate route swap")
     step = proto.RouteStep(
```

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/stream_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/stream_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 from bxsolana_trader_proto import api as proto
 from .. import provider
 
 
 async def do_stream(api: provider.Provider, run_slow: bool = False):
     item_count = 0
-    print("streaming market depth updates...")
-    async for response in api.get_market_depths_stream(
-        get_market_depths_request=proto.GetMarketDepthsRequest(
-            markets=["SOLUSDC"], limit=10, project=proto.Project.P_OPENBOOK
-        )
-    ):
-        print(response.to_json())
-        item_count += 1
-        if item_count == 1:
-            item_count = 0
-            break
-
-    print("streaming orderbook updates...")
-    async for response in api.get_orderbooks_stream(
-        get_orderbooks_request=proto.GetOrderbooksRequest(
-            markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
-        )
-    ):
-        print(response.to_json())
-        item_count += 1
-        if item_count == 1:
-            item_count = 0
-            break
+
+    if run_slow:
+        print("streaming orderbook updates...")
+        async for response in api.get_orderbooks_stream(
+            get_orderbooks_request=proto.GetOrderbooksRequest(
+                markets=["SOLUSDC"], project=proto.Project.P_OPENBOOK
+            )
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 1:
+                item_count = 0
+                break
 
     if run_slow:
         print("streaming ticker updates...")
         async for response in api.get_tickers_stream(
             get_tickers_stream_request=proto.GetTickersStreamRequest(
                 markets=[
                     "BONK/SOL",
@@ -138,18 +128,7 @@
             get_priority_fee_request=proto.GetPriorityFeeRequest()
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
-
-    if run_slow:
-        print("streaming bundle tip updates...")
-        async for response in api.get_bundle_tip_stream(
-            get_bundle_tip_request=proto.GetBundleTipRequest()
-        ):
-            print(response.to_json())
-            item_count += 1
-            if item_count == 1:
-                item_count = 0
-                break
```

### Comparing `bxsolana_trader-2.0.2/bxsolana/examples/transaction_request_utils.py` & `bxsolana-trader-2.1.0/bxsolana/examples/transaction_request_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/base.py` & `bxsolana-trader-2.1.0/bxsolana/provider/base.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/constants.py` & `bxsolana-trader-2.1.0/bxsolana/provider/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/grpc.py` & `bxsolana-trader-2.1.0/bxsolana/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/http.py` & `bxsolana-trader-2.1.0/bxsolana/provider/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,22 +152,19 @@
         self,
         get_jupiter_quotes_request: proto.GetJupiterQuotesRequest,
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> proto.GetJupiterQuotesResponse:
-        url = (
+        async with self._session.get(
             f"{self._endpoint_v2}/jupiter/quotes?inToken={get_jupiter_quotes_request.in_token}&"
             f"outToken={get_jupiter_quotes_request.out_token}&inAmount={get_jupiter_quotes_request.in_amount}&"
             f"slippage={get_jupiter_quotes_request.slippage}"
-        )
-        if get_jupiter_quotes_request.fast_mode is not None:
-            url += f"&fastMode={get_jupiter_quotes_request.fast_mode}"
-        async with self._session.get(url) as res:
+        ) as res:
             return await map_response(res, proto.GetJupiterQuotesResponse())
 
     async def get_raydium_prices(
         self,
         get_raydium_prices_request: proto.GetRaydiumPricesRequest,
         *,
         timeout: Optional[float] = None,
@@ -551,15 +548,15 @@
         get_account_balance_request: proto.GetAccountBalanceRequest,
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> proto.GetAccountBalanceResponse:
         async with self._session.get(
-            f"{self._endpoint_v2}/balance?ownerAddress={get_account_balance_request.owner_address}"
+            f"{self._endpoint}/account/balance?ownerAddress={get_account_balance_request.owner_address}"
         ) as res:
             return await map_response(res, proto.GetAccountBalanceResponse())
 
     async def get_token_accounts(
         self,
         get_token_accounts_request: proto.GetTokenAccountsRequest,
         *,
```

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/http_error.py` & `bxsolana-trader-2.1.0/bxsolana/provider/http_error.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/jsonrpc_patch.py` & `bxsolana-trader-2.1.0/bxsolana/provider/jsonrpc_patch.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/provider/ws.py` & `bxsolana-trader-2.1.0/bxsolana/provider/ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/transaction/__init__.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/transaction/memo.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/transaction/private_txs.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/private_txs.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana/transaction/signing.py` & `bxsolana-trader-2.1.0/bxsolana/transaction/signing.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/bxsolana_trader.egg-info/PKG-INFO` & `bxsolana-trader-2.1.0/bxsolana_trader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: aiohttp==3.8.1
 Requires-Dist: grpclib==0.4.3
 Requires-Dist: aiounittest==1.4.1
 Requires-Dist: base58==2.1.1
 Requires-Dist: solana==0.31.0
 Requires-Dist: solders==0.19.0
 Requires-Dist: bx-jsonrpc-py==0.2.0
-Requires-Dist: bxsolana-trader-proto==0.0.66
+Requires-Dist: bxsolana-trader-proto==0.0.63
 
 # Solana Trader Python Client
 
 Provides a Python SDK for bloXroute's Solana Trader API.
 
 ## Installation
```

### Comparing `bxsolana_trader-2.0.2/bxsolana_trader.egg-info/SOURCES.txt` & `bxsolana-trader-2.1.0/bxsolana_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/setup.cfg` & `bxsolana-trader-2.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bxsolana-trader
-version = 2.0.2
+version = 2.1.0
 description = Python SDK for bloXroute's Solana Trader API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = bloXroute Labs
 author_email = support@bloxroute.com
 url = https://github.com/bloXroute-Labs/solana-trader-client-python
 keywords = serum, solana, blockchain, trader, grpc, stream
@@ -16,13 +16,13 @@
 	aiohttp==3.8.1
 	grpclib==0.4.3
 	aiounittest==1.4.1
 	base58==2.1.1
 	solana==0.31.0
 	solders==0.19.0
 	bx-jsonrpc-py==0.2.0
-	bxsolana-trader-proto==0.0.66
+	bxsolana-trader-proto==0.0.63
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bxsolana_trader-2.0.2/test/integration/private.py` & `bxsolana-trader-2.1.0/test/integration/private.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/integration/public.py` & `bxsolana-trader-2.1.0/test/integration/public.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/integration/stream.py` & `bxsolana-trader-2.1.0/test/integration/stream.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/integration/test_grpc.py` & `bxsolana-trader-2.1.0/test/integration/test_grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/integration/test_http.py` & `bxsolana-trader-2.1.0/test/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/integration/test_ws.py` & `bxsolana-trader-2.1.0/test/integration/test_ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/unit/transaction/test_memo.py` & `bxsolana-trader-2.1.0/test/unit/transaction/test_memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana_trader-2.0.2/test/unit/transaction/test_signing.py` & `bxsolana-trader-2.1.0/test/unit/transaction/test_signing.py`

 * *Files identical despite different names*

