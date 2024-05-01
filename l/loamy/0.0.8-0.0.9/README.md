# Comparing `tmp/loamy-0.0.8.tar.gz` & `tmp/loamy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loamy-0.0.8.tar", max compression
+gzip compressed data, was "loamy-0.0.9.tar", max compression
```

## Comparing `loamy-0.0.8.tar` & `loamy-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-27 20:39:31.899984 loamy-0.0.8/LICENSE
--rw-r--r--   0        0        0     2972 2024-04-27 20:39:31.899984 loamy-0.0.8/README.md
--rw-r--r--   0        0        0     1450 2024-04-27 20:39:31.899984 loamy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/__init__.py
--rw-r--r--   0        0        0       93 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/py.typed
--rw-r--r--   0        0        0    10583 2024-04-27 20:39:31.899984 loamy-0.0.8/src/loamy/session.py
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 loamy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-01 01:46:21.837996 loamy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2972 2024-05-01 01:46:21.837996 loamy-0.0.9/README.md
+-rw-r--r--   0        0        0     1450 2024-05-01 01:46:21.837996 loamy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 01:46:21.837996 loamy-0.0.9/src/loamy/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-01 01:46:21.841996 loamy-0.0.9/src/loamy/py.typed
+-rw-r--r--   0        0        0    11408 2024-05-01 01:46:21.841996 loamy-0.0.9/src/loamy/session.py
+-rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 loamy-0.0.9/PKG-INFO
```

### Comparing `loamy-0.0.8/LICENSE` & `loamy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loamy-0.0.8/README.md` & `loamy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `loamy-0.0.8/pyproject.toml` & `loamy-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loamy"
-version = "0.0.8"
+version = "0.0.9"
 description = "This project allows you to execute a list of http operations asynchronously from within a synchronous context."
 authors = ["Zach Fuller <zach.fuller1222@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fullerzz/loamy"
 packages = [{include = "loamy", from = "src"}]
```

### Comparing `loamy-0.0.8/src/loamy/session.py` & `loamy-0.0.9/src/loamy/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 import asyncio
-import sys
 from json import JSONDecodeError
 from typing import Literal
 
 import aiohttp
 import msgspec
 from loguru import logger
 
-logger.add(
-    sys.stdout,
-    format="{time} {level} {message}",
-    filter="loamy",
-    level="DEBUG",
-)
-
+# Disable the logger. If a consuming app wishes to see loamy's logs, they can enable() it again.
+logger.disable("loamy")
+# https://loguru.readthedocs.io/en/stable/overview.html#suitable-for-scripts-and-libraries
 try:
     import uvloop
 
     async_run = uvloop.run
     logger.debug("Using uvloop for async operations")
 except ModuleNotFoundError:
     async_run = asyncio.run  # type: ignore
     logger.debug("Using asyncio for async operations")
 
 
 class RequestMap(msgspec.Struct):
+    """
+    Class containing information about a single HTTP request to be sent.
+    """
+
     url: str
     http_op: Literal["GET", "POST", "PUT", "PATCH", "OPTIONS", "DELETE"]
     body: dict | None = None
     query_params: dict[str, str] | None = None
     headers: dict[str, str] | None = None
 
 
 class RequestResponse(msgspec.Struct):
+    """
+    Class containing information about the result of an HTTP request.
+    """
+
     request_map: RequestMap
     status_code: int
     body: dict | None = None
+    headers: dict[str, str] | None = None
     error: BaseException | None = None
 
 
 class Clump:
+    """
+    Class for sending multiple HTTP requests concurrently.
+    """
+
     def __init__(self, requests: list[RequestMap]) -> None:
         self._requestMaps: list[RequestMap] = requests
         logger.debug(f"Clump created with {len(self._requestMaps)} requests")
 
     def send_requests(self, return_exceptions: bool = False) -> list[RequestResponse]:
         logger.info(
             f"Sending {len(self._requestMaps)!s} requests with {return_exceptions=!s}"
@@ -115,22 +123,26 @@
         ) as resp:
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             status_code: int = resp.status
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
 
     async def _send_post_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         async with session.post(
@@ -141,22 +153,26 @@
         ) as resp:
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             status_code: int = resp.status
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
 
     async def _send_put_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         async with session.put(
@@ -167,22 +183,26 @@
         ) as resp:
             status_code: int = resp.status
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
 
     async def _send_patch_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         async with session.patch(
@@ -193,22 +213,26 @@
         ) as resp:
             status_code: int = resp.status
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
 
     async def _send_options_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         async with session.options(
@@ -219,22 +243,26 @@
         ) as resp:
             status_code: int = resp.status
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
 
     async def _send_delete_request(
         self, req_map: RequestMap, session: aiohttp.ClientSession
     ) -> RequestResponse:
         async with session.delete(
@@ -245,17 +273,21 @@
         ) as resp:
             status_code: int = resp.status
             error: aiohttp.ContentTypeError | JSONDecodeError | None = None
             logger.debug(f"{resp.url} returned {status_code}")
             try:
                 body = await resp.json()
             except (aiohttp.ContentTypeError, JSONDecodeError) as e:
-                logger.exception(f"Failed to decode JSON response from {resp.url}")
+                logger.error(f"Failed to decode JSON response from {resp.url}")
                 error = e
                 logger.trace("Attempting to read response as text")
                 text: str = await resp.text()
                 logger.trace("Successfully read response as text")
                 body = {"text": text}
         response = RequestResponse(
-            request_map=req_map, status_code=status_code, body=body, error=error
+            request_map=req_map,
+            status_code=status_code,
+            body=body,
+            headers=dict(resp.headers),
+            error=error,
         )
         return response
```

### Comparing `loamy-0.0.8/PKG-INFO` & `loamy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loamy
-Version: 0.0.8
+Version: 0.0.9
 Summary: This project allows you to execute a list of http operations asynchronously from within a synchronous context.
 Home-page: https://github.com/fullerzz/loamy
 License: MIT
 Author: Zach Fuller
 Author-email: zach.fuller1222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

