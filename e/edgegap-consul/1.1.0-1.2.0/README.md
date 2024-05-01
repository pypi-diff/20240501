# Comparing `tmp/edgegap_consul-1.1.0.tar.gz` & `tmp/edgegap_consul-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_consul-1.2.0.tar", max compression
```

## Comparing `edgegap_consul-1.1.0.tar` & `edgegap_consul-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/LICENSE
--rw-r--r--   0        0        0     2152 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/edgegap_consul/BUILD
--rw-r--r--   0        0        0      256 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1298 2024-04-30 16:04:37.491396 edgegap_consul-1.1.0/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1471 2024-04-30 16:04:37.495396 edgegap_consul-1.1.0/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      519 2024-04-30 16:05:04.211621 edgegap_consul-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2152 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/BUILD
+-rw-r--r--   0        0        0      341 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2257 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1298 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1623 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      720 2024-05-01 17:52:31.791329 edgegap_consul-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.2.0/PKG-INFO
```

### Comparing `edgegap_consul-1.1.0/LICENSE` & `edgegap_consul-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.1.0/README.md` & `edgegap_consul-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.1.0/edgegap_consul/_client.py` & `edgegap_consul-1.2.0/edgegap_consul/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Asyncio adapter for python consul using aiohttp library"""
 
     def __init__(self, *args, loop=None, **kwargs):
         super().__init__(*args, **kwargs)
         self._loop = loop or asyncio.get_event_loop()
         connector = aiohttp.TCPConnector(
             loop=self._loop,
-            verify_ssl=self.verify
+            verify_ssl=self.verify,
         )
         self._session = aiohttp.ClientSession(connector=connector)
 
     async def _request(self, callback, method, uri, data=None):
         resp = await self._session.request(method, uri, data=data)
         body = await resp.text(encoding='utf-8')
 
@@ -26,49 +26,51 @@
 
         r = base.Response(resp.status, resp.headers, body)
 
         return callback(r)
 
     def __del__(self):
         if not self._session.closed:
-            warnings.warn("Unclosed connector in aio.Consul.HTTPClient", ResourceWarning)
+            warnings.warn('Unclosed connector in aio.Consul.HTTPClient', ResourceWarning)
             asyncio.ensure_future(self.close())
 
     async def get(self, callback, path, params=None):
         uri = self.uri(path, params)
+
         return await self._request(callback, 'GET', uri)
 
     async def put(self, callback, path, params=None, data=''):
         uri = self.uri(path, params)
+
         return await self._request(callback, 'PUT', uri, data=data)
 
     async def delete(self, callback, path, params=None):
         uri = self.uri(path, params)
+
         return await self._request(callback, 'DELETE', uri)
 
     async def post(self, callback, path, params=None, data=''):
         uri = self.uri(path, params)
+
         return await self._request(callback, 'POST', uri, data=data)
 
     async def close(self):
         await self._session.close()
 
 
 class AsyncConsul(base.Consul):
-
     def __init__(self, *args, loop=None, **kwargs):
         self._loop = loop or asyncio.get_event_loop()
         super().__init__(*args, **kwargs)
 
     def connect(self, host: str, port: int, scheme: str, verify: bool = True, cert=None):
         return AsyncClient(
             host,
             port,
             scheme,
             loop=self._loop,
             verify=verify,
-            cert=None
+            cert=None,
         )
 
     async def close(self):
-        """Close all opened http connections"""
         await self.http.close()
```

### Comparing `edgegap_consul-1.1.0/edgegap_consul/_factory.py` & `edgegap_consul-1.2.0/edgegap_consul/_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import re
 
 from ._configuration import ConsulConfiguration
-from ._reader import ConsulReader, AsyncConsulReader
+from ._reader import AsyncConsulReader, ConsulReader
 
 
 class ConsulReaderFactory:
-    __consul_pattern__ = r"\[h=(?P<host>[^\]]*),t=(?P<token>[^\]]*)\]"
+    __consul_pattern__ = r'\[h=(?P<host>[^\]]*),t=(?P<token>[^\]]*)\]'
 
     def __parse_old_syntax(self) -> ConsulConfiguration | None:
-        consul_values = os.environ.get("CONSUL", "[h=localhost,t=None]")
+        consul_values = os.environ.get('CONSUL', '[h=localhost,t=None]')
 
         if isinstance(consul_values, str):
             match = re.match(self.__consul_pattern__, consul_values)
 
             if match:
                 host = match.group('host')
                 token = match.group('token')
@@ -23,15 +23,15 @@
     def get_configuration(self) -> ConsulConfiguration:
         configuration = self.__parse_old_syntax()
 
         # implement a new syntax if needed
         # configuration = self.__parse()
 
         if configuration is None:
-            raise ValueError("Could not parse Consul Value, please set environment variables correctly")
+            raise ValueError('Could not parse Consul Value, please set environment variables correctly')
 
         return configuration
 
     def from_env(self) -> ConsulReader:
         configuration = self.get_configuration()
 
         return ConsulReader(configuration)
```

### Comparing `edgegap_consul-1.1.0/edgegap_consul/_reader.py` & `edgegap_consul-1.2.0/edgegap_consul/_reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,45 @@
+import logging
+
 import consul.aio
 
 from ._client import AsyncConsul
 from ._configuration import ConsulConfiguration
 
+logger = logging.getLogger('edgegap-consul.Reader')
+
 
 class ConsulReader:
     def __init__(self, configuration: ConsulConfiguration):
         self._configuration = configuration
         self._client = consul.Consul(**self._configuration.model_dump())
 
     @staticmethod
     def _parse(data: dict) -> tuple[bool, [str | None]]:
         value = None
         key_exists = False
+
         if isinstance(data, dict):
-            value = data.get("Value")
+            value = data.get('Value')
 
             if isinstance(value, bytes):
-                value = str(value, "utf-8")
+                value = str(value, 'utf-8')
 
             key_exists = True
+
         return key_exists, value
 
     def get(self, key: str) -> tuple[bool, [str | None]]:
         try:
             _, data = self._client.kv.get(key)
+
             return self._parse(data)
+
         except ConnectionError as e:
-            print(e)
+            logger.exception(f'Failed to get [{key}]: {e}')
 
     def check(self) -> bool:
         status = self._client.status.leader()
 
         return isinstance(status, str)
 
 
@@ -39,13 +47,14 @@
     def __init__(self, configuration: ConsulConfiguration):
         super().__init__(configuration)
         self._client = AsyncConsul(**self._configuration.model_dump())
 
     async def get(self, key: str) -> tuple[bool, [str | None]]:
         try:
             _, data = await self._client.kv.get(key)
+
             return self._parse(data)
 
         except ConnectionError as e:
-            print(e)
+            logger.exception(f'Failed to get [{key}]: {e}')
         finally:
             await self._client.close()
```

### Comparing `edgegap_consul-1.1.0/pyproject.toml` & `edgegap_consul-1.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "1.1.0"
+version = "1.2.0"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
 pydantic = "^2.7.1"
 python-consul = "^1.1.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest-cov = "^5.0.0"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-mock = "^3.14.0"
+ruff = "^0.4.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+extend = "../../../3rdparty/ruff/ruff.toml"
```

### Comparing `edgegap_consul-1.1.0/PKG-INFO` & `edgegap_consul-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

