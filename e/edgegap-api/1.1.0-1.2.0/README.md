# Comparing `tmp/edgegap_api-1.1.0.tar.gz` & `tmp/edgegap_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_api-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_api-1.2.0.tar", max compression
```

## Comparing `edgegap_api-1.1.0.tar` & `edgegap_api-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/LICENSE
--rw-r--r--   0        0        0     2171 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/edgegap_api/BUILD
--rw-r--r--   0        0        0      132 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/edgegap_api/__init__.py
--rw-r--r--   0        0        0      626 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/edgegap_api/_configuration.py
--rw-r--r--   0        0        0     4163 2024-04-30 16:04:37.491396 edgegap_api-1.1.0/edgegap_api/_helper.py
--rw-r--r--   0        0        0      536 2024-04-30 16:04:58.407573 edgegap_api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2171 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/edgegap_api/BUILD
+-rw-r--r--   0        0        0      132 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/edgegap_api/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/edgegap_api/_configuration.py
+-rw-r--r--   0        0        0     3990 2024-05-01 17:52:18.959014 edgegap_api-1.2.0/edgegap_api/_helper.py
+-rw-r--r--   0        0        0      763 2024-05-01 17:52:24.627153 edgegap_api-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.2.0/PKG-INFO
```

### Comparing `edgegap_api-1.1.0/LICENSE` & `edgegap_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.1.0/README.md` & `edgegap_api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.1.0/edgegap_api/_configuration.py` & `edgegap_api-1.2.0/edgegap_api/_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from pydantic import BaseModel, HttpUrl, Field
-
+from pydantic import BaseModel, Field, HttpUrl
 from pytimeparse import parse
 
 
 class ApiConfiguration(BaseModel):
-    base_url: HttpUrl = Field(..., description="The Base URL to use in the API calls.")
-    default_headers: dict[str, str] = Field(default={}, description="The default Headers to append to all requests.")
-    timeout: str = Field(default="10s", description="The timeout in annotation to wait for the request to complete")
+    base_url: HttpUrl = Field(..., description='The Base URL to use in the API calls.')
+    default_headers: dict[str, str] = Field(default={}, description='The default Headers to append to all requests.')
+    timeout: str = Field(
+        default='10s',
+        description='The timeout in annotation to wait for the request to complete',
+    )
 
     @property
     def timeout_in_ms(self) -> int:
         return self.timeout_in_seconds * 1000
 
     @property
     def timeout_in_seconds(self) -> int:
```

### Comparing `edgegap_api-1.1.0/edgegap_api/_helper.py` & `edgegap_api-1.2.0/edgegap_api/_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,140 +1,147 @@
 from contextlib import asynccontextmanager
-from typing import Callable, AsyncIterator
+from typing import AsyncIterator, Callable
 
 import aiohttp
 from aiohttp import ClientResponse
 from aiohttp.client import ClientSession
 
 from ._configuration import ApiConfiguration
 
 
 class ApiHelper:
     def __init__(self, configuration: ApiConfiguration):
-        if isinstance(configuration.base_url, str) and configuration.base_url.endswith("/"):
-            configuration.base_url = configuration.base_url[:-1]
-
         self.__configuration = configuration
 
     def __get_headers(self, extra_headers: dict = None) -> dict:
         headers = self.__configuration.default_headers
 
         if headers is None:
             headers = {}
 
         if isinstance(extra_headers, dict):
             headers.update(extra_headers)
 
         return headers
 
     def __get_url(self, endpoint: str) -> str:
-        if endpoint.startswith("/"):
+        base_url = str(self.__configuration.base_url)
+
+        if base_url.endswith('/'):
+            base_url = base_url[:-1]
+
+        if endpoint.startswith('/'):
             endpoint = endpoint[1:]
 
-        return f"{self.__configuration.base_url}/{endpoint}"
+        return f'{base_url}/{endpoint}'
 
     @asynccontextmanager
     async def __request(
-            self,
-            method: Callable,
-            endpoint: str,
-            headers: dict = None,
-            params: dict = None,
-            body: dict = None
+        self,
+        method: Callable,
+        endpoint: str,
+        headers: dict = None,
+        params: dict = None,
+        body: dict = None,
     ) -> AsyncIterator[ClientResponse]:
+        _headers = self.__get_headers(headers)
+        _url = self.__get_url(endpoint)
+
         async with aiohttp.ClientSession() as session:
             async with method(
-                    self=session,
-                    headers=self.__get_headers(headers),
-                    url=self.__get_url(endpoint),
-                    params=params,
-                    json=body,
-                    timeout=self.__configuration.timeout_in_ms
+                self=session,
+                headers=_headers,
+                url=_url,
+                params=params,
+                json=body,
+                timeout=self.__configuration.timeout_in_ms,
             ) as response:
                 yield response
 
     @staticmethod
     @asynccontextmanager
     async def session() -> AsyncIterator[ClientSession]:
         async with aiohttp.ClientSession() as session:
             yield session
 
     @asynccontextmanager
     async def get(
-            self,
-            endpoint: str,
-            params: dict = None,
-            headers: dict = None
+        self,
+        endpoint: str,
+        params: dict = None,
+        headers: dict = None,
     ) -> AsyncIterator[ClientResponse]:
         async with self.__request(
-                method=aiohttp.ClientSession.get,
-                endpoint=endpoint,
-                headers=headers,
-                params=params
+            method=aiohttp.ClientSession.get,
+            endpoint=endpoint,
+            headers=headers,
+            params=params,
         ) as response:
             yield response
 
     @asynccontextmanager
     async def delete(
-            self,
-            endpoint: str,
-            params: dict = None,
-            headers: dict = None
+        self,
+        endpoint: str,
+        params: dict = None,
+        body: dict = None,
+        headers: dict = None,
     ) -> AsyncIterator[ClientResponse]:
         async with self.__request(
-                method=aiohttp.ClientSession.delete,
-                endpoint=endpoint,
-                headers=headers,
-                params=params
+            method=aiohttp.ClientSession.delete,
+            endpoint=endpoint,
+            headers=headers,
+            params=params,
+            body=body,
         ) as response:
             yield response
 
     @asynccontextmanager
     async def post(
-            self,
-            endpoint: str,
-            params: dict = None,
-            body: dict = None,
-            headers: dict = None
+        self,
+        endpoint: str,
+        params: dict = None,
+        body: dict = None,
+        headers: dict = None,
     ) -> AsyncIterator[ClientResponse]:
         async with self.__request(
-                method=aiohttp.ClientSession.post,
-                endpoint=endpoint,
-                headers=headers,
-                params=params,
-                body=body
+            method=aiohttp.ClientSession.post,
+            endpoint=endpoint,
+            headers=headers,
+            params=params,
+            body=body,
         ) as response:
             yield response
 
     @asynccontextmanager
     async def patch(
-            self,
-            endpoint: str,
-            params: dict = None,
-            body: dict = None,
-            headers: dict = None
+        self,
+        endpoint: str,
+        params: dict = None,
+        body: dict = None,
+        headers: dict = None,
     ) -> AsyncIterator[ClientResponse]:
         async with self.__request(
-                method=aiohttp.ClientSession.patch,
-                endpoint=endpoint,
-                headers=headers,
-                params=params,
-                body=body
+            method=aiohttp.ClientSession.patch,
+            endpoint=endpoint,
+            headers=headers,
+            params=params,
+            body=body,
         ) as response:
             yield response
 
     @asynccontextmanager
     async def put(
-            self,
-            endpoint: str,
-            params: dict = None,
-            body: dict = None,
-            headers: dict = None
+        self,
+        endpoint: str,
+        params: dict = None,
+        body: dict = None,
+        headers: dict = None,
     ) -> AsyncIterator[ClientResponse]:
         async with self.__request(
-                method=aiohttp.ClientSession.put,
-                endpoint=endpoint,
-                headers=headers,
-                params=params,
-                body=body
+            method=aiohttp.ClientSession.put,
+            endpoint=endpoint,
+            headers=headers,
+            params=params,
+            body=body,
         ) as response:
             yield response
```

### Comparing `edgegap_api-1.1.0/PKG-INFO` & `edgegap_api-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

