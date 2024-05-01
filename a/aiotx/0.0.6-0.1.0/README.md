# Comparing `tmp/aiotx-0.0.6.tar.gz` & `tmp/aiotx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.0.6.tar", last modified: Tue Apr 30 06:30:09 2024, max compression
+gzip compressed data, was "aiotx-0.1.0.tar", last modified: Wed May  1 20:25:51 2024, max compression
```

## Comparing `aiotx-0.0.6.tar` & `aiotx-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.364729 aiotx-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.364729 aiotx-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 06:30:04.000000 aiotx-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-30 06:30:04.000000 aiotx-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 06:30:04.000000 aiotx-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-30 06:30:09.368729 aiotx-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 06:30:04.000000 aiotx-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 06:30:04.000000 aiotx-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 06:30:09.368729 aiotx-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-30 06:30:04.000000 aiotx-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-01 20:25:44.000000 aiotx-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 20:25:44.000000 aiotx-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-01 20:25:44.000000 aiotx-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 20:25:51.036228 aiotx-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-01 20:25:44.000000 aiotx-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 20:25:44.000000 aiotx-0.1.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-01 20:25:51.000000 aiotx-0.1.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 20:25:50.000000 aiotx-0.1.0/aiotx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-01 20:25:44.000000 aiotx-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 20:25:44.000000 aiotx-0.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 20:25:51.036228 aiotx-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-01 20:25:44.000000 aiotx-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.032228 aiotx-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/confest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.028228 aiotx-0.1.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:25:51.036228 aiotx-0.1.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-01 20:25:44.000000 aiotx-0.1.0/tests/test_bsc_client.py
```

### Comparing `aiotx-0.0.6/.github/workflows/python-publish.yml` & `aiotx-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.0.6/.gitignore` & `aiotx-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.0.6/PKG-INFO` & `aiotx-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.6
+Version: 0.1.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,25 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
+Requires-Dist: eth_keys
+Requires-Dist: eth_utils
+Requires-Dist: eth_account
 Provides-Extra: test
-Requires-Dist: black; extra == "test"
-Requires-Dist: flake8; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: isort; extra == "test"
-Requires-Dist: mypy>=0.910; extra == "test"
+Requires-Dist: ruff; extra == "test"
 Requires-Dist: pyproj; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: build; extra == "test"
+Requires-Dist: vcrpy; extra == "test"
 
 ## AioTx
 
 AioTx is an asynchronous library for interacting with various cryptocurrencies and blockchains. It aims to provide a lightweight and efficient solution for developers to integrate cryptocurrency functionalities into their projects without relying on heavy dependencies like web3.js or bitcoin-lib.
 Features
 
 - Asynchronous and non-blocking design for high performance
@@ -52,24 +54,27 @@
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
     
     # Create a new wallet
-    wallet = await bsc_client.create_wallet()
-    print(f"Wallet address: {wallet.address}")
+    address, private_key = await bsc_client.generate_address()
     
     # Retrieve the wallet balance
-    balance = await bsc_client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
+    # Send transaction
+    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    print(f"Your tx: {tx_id}")
+
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
 # Contributing
```

### Comparing `aiotx-0.0.6/README.md` & `aiotx-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
     
     # Create a new wallet
-    wallet = await bsc_client.create_wallet()
-    print(f"Wallet address: {wallet.address}")
+    address, private_key = await bsc_client.generate_address()
     
     # Retrieve the wallet balance
-    balance = await bsc_client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
+    # Send transaction
+    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    print(f"Your tx: {tx_id}")
+
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
 # Contributing
```

### Comparing `aiotx-0.0.6/aiotx.egg-info/PKG-INFO` & `aiotx-0.1.0/aiotx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.6
+Version: 0.1.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,25 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
+Requires-Dist: eth_keys
+Requires-Dist: eth_utils
+Requires-Dist: eth_account
 Provides-Extra: test
-Requires-Dist: black; extra == "test"
-Requires-Dist: flake8; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: isort; extra == "test"
-Requires-Dist: mypy>=0.910; extra == "test"
+Requires-Dist: ruff; extra == "test"
 Requires-Dist: pyproj; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: build; extra == "test"
+Requires-Dist: vcrpy; extra == "test"
 
 ## AioTx
 
 AioTx is an asynchronous library for interacting with various cryptocurrencies and blockchains. It aims to provide a lightweight and efficient solution for developers to integrate cryptocurrency functionalities into their projects without relying on heavy dependencies like web3.js or bitcoin-lib.
 Features
 
 - Asynchronous and non-blocking design for high performance
@@ -52,24 +54,27 @@
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
     
     # Create a new wallet
-    wallet = await bsc_client.create_wallet()
-    print(f"Wallet address: {wallet.address}")
+    address, private_key = await bsc_client.generate_address()
     
     # Retrieve the wallet balance
-    balance = await bsc_client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
+    # Send transaction
+    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    print(f"Your tx: {tx_id}")
+
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
 # Contributing
```

### Comparing `aiotx-0.0.6/setup.py` & `aiotx-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import find_packages, setup
 
 
 extras_test = (
     [
-        "black",
-        "flake8",
         "hypothesis",
-        "isort",
-        "mypy>=0.910",
+        "ruff",
         "pyproj",
         "pytest",
         "pytest-cov",
+        "pytest-asyncio",
         "tox",
-        "build"
+        "build",
+        "vcrpy"
     ]
 )
 
 setup(
     name="aiotx",
     keywords=[
         "cryptocurrency",
@@ -39,14 +38,17 @@
         "aiotx": ["py.typed"],
     },
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=[
         "aiohttp",
+        "eth_keys",
+        "eth_utils",
+        "eth_account"
     ],
     extras_require={
         "test": extras_test,
     },
     url="https://github.com/Grommash9/aiotx",
     author="Oleksandr Prudnikov",
     author_email="prudnikov21@icloud.com",
```

