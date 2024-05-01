# Comparing `tmp/heatzypy-2.2.0.tar.gz` & `tmp/heatzypy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatzypy-2.2.0.tar", last modified: Fri Dec 22 11:03:59 2023, max compression
+gzip compressed data, was "heatzypy-2.5.0.tar", last modified: Wed May  1 13:52:55 2024, max compression
```

## Comparing `heatzypy-2.2.0.tar` & `heatzypy-2.5.0.tar`

### file list

```diff
@@ -1,20 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 11:03:59.384972 heatzypy-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-22 11:03:47.000000 heatzypy-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-22 11:03:47.000000 heatzypy-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-12-22 11:03:59.384972 heatzypy-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-22 11:03:47.000000 heatzypy-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 11:03:59.384972 heatzypy-2.2.0/heatzypy/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-22 11:03:47.000000 heatzypy-2.2.0/heatzypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-12-22 11:03:47.000000 heatzypy-2.2.0/heatzypy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-22 11:03:47.000000 heatzypy-2.2.0/heatzypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-22 11:03:47.000000 heatzypy-2.2.0/heatzypy/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-12-22 11:03:47.000000 heatzypy-2.2.0/heatzypy/heatzy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 11:03:59.384972 heatzypy-2.2.0/heatzypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-22 11:03:59.000000 heatzypy-2.2.0/heatzypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-22 11:03:53.000000 heatzypy-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 11:03:59.384972 heatzypy-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.899265 heatzypy-2.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 13:52:46.000000 heatzypy-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 13:52:46.000000 heatzypy-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 13:52:55.903265 heatzypy-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 13:52:46.000000 heatzypy-2.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-05-01 13:52:46.000000 heatzypy-2.5.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/heatzypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/heatzy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/heatzypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 13:52:46.000000 heatzypy-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 13:52:46.000000 heatzypy-2.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 13:52:46.000000 heatzypy-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:52:55.903265 heatzypy-2.5.0/setup.cfg
```

### Comparing `heatzypy-2.2.0/LICENSE` & `heatzypy-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heatzypy-2.2.0/PKG-INFO` & `heatzypy-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.2.0
-Summary: Provides asynchronous authentication and access to Heatzy module
+Version: 2.5.0
+Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
-Keywords: heatzy,async,climate
+Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
```

### Comparing `heatzypy-2.2.0/README.md` & `heatzypy-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `heatzypy-2.2.0/heatzypy/auth.py` & `heatzypy-2.5.0/heatzypy/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,119 @@
 """Authentication class."""
+
 from __future__ import annotations
 
 import asyncio
+from json import JSONDecodeError
 import logging
 import socket
 import time
-from json import JSONDecodeError
 from typing import Any
 
-from aiohttp import (  # pylint: disable=import-error
-    ClientError,
-    ClientResponseError,
-    ClientSession,
-)
+from aiohttp import ClientError, ClientResponseError, ClientSession
+from yarl import URL
 
-from .const import HEATZY_API_URL, HEATZY_APPLICATION_ID
+from .const import APPLICATION_ID, RETRY, URL_PATH
 from .exception import (
     AuthenticationFailed,
     CommandFailed,
     HttpRequestFailed,
     RetrieveFailed,
     TimeoutExceededError,
+    UnexpectedResponse,
 )
 
-_LOGGER = logging.getLogger(__name__)
-RETRY = 3
+logger = logging.getLogger(__name__)
 
 
 class Auth:
     """Class to make authenticated requests."""
 
     def __init__(
-        self, session: ClientSession | None, username: str, password: str, timeout: int
+        self,
+        session: ClientSession | None,
+        username: str,
+        password: str,
+        timeout: int,
+        host: str,
+        use_tls: bool = True,
     ):
         """Initialize the auth."""
         self._session = session or ClientSession()
         self._username = username
         self._password = password
         self._access_token: dict[str, Any] | None = None
         self._timeout: int = timeout
         self._retry = RETRY
+        self._host = host
+        self._scheme = "https" if use_tls else "http"
 
     async def request(
-        self, service: str, method: str = "GET", **kwargs: Any
+        self,
+        url: str | URL,
+        method: str = "get",
+        json: dict[str, Any] | None = None,
+        auth: bool = False,
     ) -> dict[str, Any]:
         """Make a request."""
-        headers = dict(
-            kwargs.pop("headers", {"X-Gizwits-Application-Id": HEATZY_APPLICATION_ID})
-        )
-        if kwargs.pop("auth", None) is None:
-            access_token = await self._async_get_token()
-            headers["X-Gizwits-User-Token"] = access_token
+        headers: dict[str, Any] = {"X-Gizwits-Application-Id": APPLICATION_ID}
+
+        if auth is False:
+            access_token = await self.async_get_token()
+            headers["X-Gizwits-User-Token"] = access_token.get("token")
 
         try:
-            _LOGGER.debug("METHOD:%s URL:%s", method, service)
-            _LOGGER.debug("DATA:%s", kwargs)
             async with asyncio.timeout(self._timeout):
+                url = URL.build(
+                    scheme=self._scheme, host=self._host, path=f"{URL_PATH}/{url}"
+                )
+                logger.debug("METHOD:%s URL:%s", method, url)
+                logger.debug("DATA:%s", json)
                 response = await self._session.request(
-                    method,
-                    f"{HEATZY_API_URL}/{service}",
-                    **kwargs,
-                    headers=headers,
+                    method, url, json=json, headers=headers
                 )
                 response.raise_for_status()
         except ClientResponseError as error:
-            if method == "GET":
-                raise RetrieveFailed(
-                    f"{service} not retrieved ({error.status})"
-                ) from error
-            if service == "login":
+            if method == "get":
+                raise RetrieveFailed(f"{url} not retrieved ({error.status})") from error
+            if url == "login":
                 raise AuthenticationFailed(
                     f"{error.message} ({error.status})"
                 ) from error
-            if method == "POST" and error.status in [400, 500, 502] and self._retry > 0:
+            if method == "post" and error.status in [400, 500, 502] and self._retry > 0:
                 self._retry -= 1
                 await asyncio.sleep(3)
-                await self.request(service, method, **kwargs)
+                return await self.request(url, method, json, auth)
             raise CommandFailed(
-                f"Cmd failed {service} with {kwargs} ({error.status} {error.message})"
+                f"Cmd failed {url} with {json} ({error.status} {error.message})"
             ) from error
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Heatzy."
             ) from error
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestFailed(
                 "Error occurred while communicating with Heatzy."
             ) from error
 
+        json_response: dict[str, Any] = {}
         try:
-            json_response: dict[str, Any] = {}
             if response.status != 204:
                 json_response = await response.json(content_type=None)
         except JSONDecodeError as error:
-            raise HttpRequestFailed(f"Error while deconding Json ({error})") from error
-        _LOGGER.debug(json_response)
+            raise UnexpectedResponse(f"Error while decoding Json ({error})") from error
+
+        logger.debug("RESPONSE: %s", json_response)
+
         return json_response
 
-    async def _async_get_token(self) -> str | None:
+    async def async_get_token(self) -> dict[str, Any]:
         """Get Token authentication."""
         if self._access_token is None or (
             (expire_at := self._access_token.get("expire_at"))
             and expire_at < time.time()
         ):
             payload = {"username": self._username, "password": self._password}
             self._access_token = await self.request(
-                "login", method="POST", json=payload, auth=True
+                "login", method="post", json=payload, auth=True
             )
-        return self._access_token.get("token")
-
-    async def async_close(self) -> None:
-        """Close session."""
-        await self._session.close()
+        return self._access_token
```

### Comparing `heatzypy-2.2.0/heatzypy/heatzy.py` & `heatzypy-2.5.0/heatzypy/heatzy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 """Heatzy API."""
+
 from __future__ import annotations
 
 import logging
-from typing import Any
+from typing import Any, Self
 
-from aiohttp import ClientSession  # pylint: disable=import-error
+from aiohttp import ClientSession
 
 from .auth import Auth
+from .const import DFLT_API_URL, EU_API_URL, TIMEOUT, US_API_URL, WS_HOST
+from .websocket import Websocket
 
-_LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class HeatzyClient:
     """Heatzy Client data."""
 
     def __init__(
         self,
         username: str,
         password: str,
-        session: ClientSession | None = None,
-        time_out: int = 120,
+        session: ClientSession = ClientSession(),
+        time_out: int = TIMEOUT,
+        region: str = "EU",
+        use_tls: bool = True,
     ) -> None:
         """Load parameters."""
-        self._auth = Auth(session, username, password, time_out)
+        if region == "EU":
+            host = EU_API_URL
+        elif region == "US":
+            host = US_API_URL
+        else:
+            host = DFLT_API_URL
+
+        self._auth = Auth(session, username, password, time_out, host, use_tls)
+        self.websocket = Websocket(session, self._auth, WS_HOST, use_tls)
+        self.session = session
         self.request = self._auth.request
 
-    async def async_bindings(self) -> dict[str, dict[str, Any]]:
+    @property
+    def is_connected(self) -> bool:
+        """Return if we are connect to the WebSocket."""
+        return self.websocket.is_connected
+
+    async def async_bindings(self) -> dict[str, list[dict[str, Any]]]:
         """Fetch all configured devices."""
         return await self.request("bindings")
 
     async def async_get_devices(self) -> dict[str, Any]:
         """Fetch all configured devices."""
         response = await self.async_bindings()
-        devices = response.get("devices", {})
-        devices_with_datas = [
-            await self._async_merge_with_device_data(device)  # type: ignore
-            for device in devices
-        ]
-        dict_devices_with_datas = {
-            device["did"]: device for device in devices_with_datas
-        }
-        return dict_devices_with_datas
+        devices = {device["did"]: device for device in response.get("devices", {})}
+        for did, device in devices.items():
+            device_data = await self.async_get_device_data(did)
+            device_data["attrs"] = device_data.pop("attr", {})
+            device.update(**device_data)
+        return devices
 
     async def async_get_device(self, device_id: str) -> dict[str, Any]:
         """Fetch device with given id."""
         device = await self.request(f"devices/{device_id}")
-        return await self._async_merge_with_device_data(device)
-
-    async def _async_merge_with_device_data(
-        self, device: dict[str, Any]
-    ) -> dict[str, Any]:
-        """Fetch detailed data for device and merge it with the device information."""
-        device_data = await self.async_get_device_data(device["did"])
+        device_data = await self.async_get_device_data(device_id)
+        device_data["attrs"] = device_data.pop("attr", {})
         return {**device, **device_data}
 
     async def async_get_device_data(self, device_id: str) -> dict[str, Any]:
         """Fetch detailed data for device with given id."""
         return await self.request(f"devdata/{device_id}/latest")
 
     async def async_control_device(
         self, device_id: str, payload: dict[str, Any]
     ) -> None:
         """Control state of device with given id."""
-        await self.request(f"control/{device_id}", method="POST", json=payload)
+        await self.request(f"control/{device_id}", method="post", json=payload)
 
     async def async_close(self) -> None:
-        """Close session."""
-        await self._auth.async_close()
+        """Close open client (WebSocket) session."""
+        await self.websocket.async_disconnect()
+        if self.session:
+            await self.session.close()
+
+    async def __aenter__(self) -> Self:
+        """Async enter."""
+        return self
+
+    async def __aexit__(self, *_exc_info: object) -> None:
+        """Async exit."""
+        await self.async_close()
```

### Comparing `heatzypy-2.2.0/heatzypy.egg-info/PKG-INFO` & `heatzypy-2.5.0/heatzypy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.2.0
-Summary: Provides asynchronous authentication and access to Heatzy module
+Version: 2.5.0
+Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
-Keywords: heatzy,async,climate
+Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
```

