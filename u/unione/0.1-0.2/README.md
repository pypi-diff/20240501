# Comparing `tmp/unione-0.1.tar.gz` & `tmp/unione-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unione-0.1.tar", last modified: Mon Apr 29 13:24:23 2024, max compression
+gzip compressed data, was "unione-0.2.tar", last modified: Wed May  1 05:52:48 2024, max compression
```

## Comparing `unione-0.1.tar` & `unione-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-04-29 13:24:23.534012 unione-0.1/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-04-29 13:24:23.534012 unione-0.1/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-04-29 13:24:23.534012 unione-0.1/setup.cfg
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-04-29 13:23:46.000000 unione-0.1/setup.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-04-29 13:24:23.534012 unione-0.1/unilite/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.1/unilite/__init__.py
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)    98930 2024-04-29 13:16:09.000000 unione-0.1/unilite/contract_maker.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-04-29 13:24:23.534012 unione-0.1/unione.egg-info/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-04-29 13:24:23.000000 unione-0.1/unione.egg-info/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      203 2024-04-29 13:24:23.000000 unione-0.1/unione.egg-info/SOURCES.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-04-29 13:24:23.000000 unione-0.1/unione.egg-info/dependency_links.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-04-29 13:24:23.000000 unione-0.1/unione.egg-info/requires.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-04-29 13:24:23.000000 unione-0.1/unione.egg-info/top_level.txt
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 05:52:48.971328 unione-0.2/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-01 05:52:48.971328 unione-0.2/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-05-01 05:52:48.971328 unione-0.2/setup.cfg
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-05-01 05:48:50.000000 unione-0.2/setup.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 05:52:48.967995 unione-0.2/unilite/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.2/unilite/__init__.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)     3642 2024-05-01 05:46:51.000000 unione-0.2/unilite/constants.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)    98655 2024-05-01 05:48:21.000000 unione-0.2/unilite/contract_maker.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 05:52:48.971328 unione-0.2/unione.egg-info/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-01 05:52:48.000000 unione-0.2/unione.egg-info/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      224 2024-05-01 05:52:48.000000 unione-0.2/unione.egg-info/SOURCES.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-05-01 05:52:48.000000 unione-0.2/unione.egg-info/dependency_links.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-05-01 05:52:48.000000 unione-0.2/unione.egg-info/requires.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-05-01 05:52:48.000000 unione-0.2/unione.egg-info/top_level.txt
```

### Comparing `unione-0.1/unilite/contract_maker.py` & `unione-0.2/unilite/contract_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from web3 import Web3
 
-mainnet_rpc = 'https://eth.llamarpc.com'
-CONTRACT_ADDRESS = '0x9DAEa35A922492BE23941De2433D3FD88b3e7cAE'
-UNISWAP_V2_FACTORY = '0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f'
-UNISWAP_V2_ROUTER = '0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D'
-UNISWAP_V3_FACTORY = '0x1F98431c8aD98523631AE4a59f267346ea31F984'
-UNISWAP_V3_ROUTER = '0xE592427A0AEce92De3Edee1F18E0157C05861564'
+from unilite import constants
 
-w3 = Web3(Web3.HTTPProvider(mainnet_rpc))
+w3 = Web3(Web3.HTTPProvider(constants.ETH_MAINNET_RPC))
 
 contract_abi = [
     {
         "type": "constructor",
         "inputs": [],
         "stateMutability": "nonpayable"
     },
@@ -3783,34 +3778,32 @@
         "stateMutability": "view",
         "type": "function"
     }
 ]
 
 
 def get_uniswap_v2_factory():
-    return w3.eth.contract(address=UNISWAP_V2_FACTORY, abi=uniswap_v2_factory_abi)
+    return w3.eth.contract(address=constants.UNISWAP_V2_FACTORY, abi=uniswap_v2_factory_abi)
 
 
 def get_uniswap_v2_router():
-    return w3.eth.contract(address=UNISWAP_V2_ROUTER, abi=uniswap_v2_router_abi)
+    return w3.eth.contract(address=constants.UNISWAP_V2_ROUTER, abi=uniswap_v2_router_abi)
 
 
 def get_uniswap_v2_pool(address):
     return w3.eth.contract(address=address, abi=uniswap_v2_pool_abi)
 
 
 def get_uniswap_v3_factory():
-    return w3.eth.contract(address=UNISWAP_V3_FACTORY, abi=uniswap_v3_factory_abi)
+    return w3.eth.contract(address=constants.UNISWAP_V3_FACTORY, abi=uniswap_v3_factory_abi)
 
 
 def get_uniswap_v3_router():
-    return w3.eth.contract(address=UNISWAP_V3_ROUTER, abi=uniswap_v3_router_abi)
+    return w3.eth.contract(address=constants.UNISWAP_V3_ROUTER, abi=uniswap_v3_router_abi)
 
 
 def get_uniswap_v3_pool(address):
     return w3.eth.contract(address=address, abi=uniswap_v3_pool_abi)
 
 
 def get_bot_contract():
-    return w3.eth.contract(address=CONTRACT_ADDRESS, abi=contract_abi)
-
-
+    return w3.eth.contract(address=constants.CONTRACT_ADDRESS, abi=contract_abi)
```

