# Comparing `tmp/heatzypy-2.5.0.tar.gz` & `tmp/heatzypy-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatzypy-2.5.0.tar", last modified: Wed May  1 13:52:55 2024, max compression
+gzip compressed data, was "heatzypy-2.5.1.tar", last modified: Wed May  1 16:24:37 2024, max compression
```

## Comparing `heatzypy-2.5.0.tar` & `heatzypy-2.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.899265 heatzypy-2.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 13:52:46.000000 heatzypy-2.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 13:52:46.000000 heatzypy-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 13:52:46.000000 heatzypy-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 13:52:55.903265 heatzypy-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 13:52:46.000000 heatzypy-2.5.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1921 2024-05-01 13:52:46.000000 heatzypy-2.5.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/heatzypy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/heatzy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-01 13:52:46.000000 heatzypy-2.5.0/heatzypy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:52:55.903265 heatzypy-2.5.0/heatzypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 13:52:55.000000 heatzypy-2.5.0/heatzypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 13:52:46.000000 heatzypy-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 13:52:46.000000 heatzypy-2.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 13:52:46.000000 heatzypy-2.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:52:55.903265 heatzypy-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.334143 heatzypy-2.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 16:24:27.000000 heatzypy-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 16:24:27.000000 heatzypy-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 16:24:37.338143 heatzypy-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 16:24:27.000000 heatzypy-2.5.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2353 2024-05-01 16:24:27.000000 heatzypy-2.5.1/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/heatzypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/heatzy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/heatzypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 16:24:27.000000 heatzypy-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 16:24:27.000000 heatzypy-2.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 16:24:27.000000 heatzypy-2.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:24:37.338143 heatzypy-2.5.1/setup.cfg
```

### Comparing `heatzypy-2.5.0/.github/dependabot.yml` & `heatzypy-2.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.github/workflows/auto-approve.yml` & `heatzypy-2.5.1/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.github/workflows/lint.yml` & `heatzypy-2.5.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.github/workflows/pythonpublish.yml` & `heatzypy-2.5.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.github/workflows/release.yml` & `heatzypy-2.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.gitignore` & `heatzypy-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/.pre-commit-config.yaml` & `heatzypy-2.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/LICENSE` & `heatzypy-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/PKG-INFO` & `heatzypy-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.0
+Version: 2.5.1
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.0/README.md` & `heatzypy-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/example.py` & `heatzypy-2.5.1/example.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - Websocket mode by calling the websocket module
 """
 
 import asyncio
 import logging
 from typing import Any
 
-from heatzypy import HeatzyClient, HeatzyException
+from heatzypy import AuthenticationFailed, HeatzyClient, HeatzyException
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 # create console handler and set level to debug
 ch = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
@@ -48,18 +48,30 @@
         for uniqe_id, device in devices.items():
             # set all Pilot v2 devices to preset 'eco' mode.
             try:
                 # await api.async_control_device(uniqe_id, {"attrs": {"mode": "eco"}})
                 pass
             except HeatzyException as error:
                 logger.error(error)
+    except AuthenticationFailed as error:
+        logger.error("Auth failed (%s)", error)
     except HeatzyException as error:
         logger.error(str(error))
 
     # Listen Heatzy webscoket
+    api.websocket.register_callback(callback)
+    try:
+        await api.websocket.async_connect(auto_subscribe=True, all_devices=True)
+    except AuthenticationFailed as error:
+        logger.error("Auth failed (%s)", error)
+    except HeatzyException as error:
+        logger.error(str(error))
+
+    while api.websocket.is_connected:
+        await asyncio.sleep(1)
 
-    await api.websocket.async_listen(callback=callback, all_devices=True)
+    await api.async_close()
 
 
 if __name__ == "__main__":
     loop = asyncio.get_event_loop()
     loop.run_until_complete(async_main())
```

### Comparing `heatzypy-2.5.0/heatzypy/auth.py` & `heatzypy-2.5.1/heatzypy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,35 +45,35 @@
         self._timeout: int = timeout
         self._retry = RETRY
         self._host = host
         self._scheme = "https" if use_tls else "http"
 
     async def request(
         self,
-        url: str | URL,
+        url: str,
         method: str = "get",
         json: dict[str, Any] | None = None,
         auth: bool = False,
     ) -> dict[str, Any]:
         """Make a request."""
         headers: dict[str, Any] = {"X-Gizwits-Application-Id": APPLICATION_ID}
 
         if auth is False:
             access_token = await self.async_get_token()
             headers["X-Gizwits-User-Token"] = access_token.get("token")
 
         try:
             async with asyncio.timeout(self._timeout):
-                url = URL.build(
+                uri = URL.build(
                     scheme=self._scheme, host=self._host, path=f"{URL_PATH}/{url}"
                 )
-                logger.debug("METHOD:%s URL:%s", method, url)
+                logger.debug("METHOD:%s URL:%s", method, uri)
                 logger.debug("DATA:%s", json)
                 response = await self._session.request(
-                    method, url, json=json, headers=headers
+                    method, uri, json=json, headers=headers
                 )
                 response.raise_for_status()
         except ClientResponseError as error:
             if method == "get":
                 raise RetrieveFailed(f"{url} not retrieved ({error.status})") from error
             if url == "login":
                 raise AuthenticationFailed(
```

### Comparing `heatzypy-2.5.0/heatzypy/exception.py` & `heatzypy-2.5.1/heatzypy/exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,11 +31,7 @@
 
 class WebsocketError(HeatzyException):
     """Websocket exception."""
 
 
 class ConnectionFailed(WebsocketError):
     """Connection exception."""
-
-
-class ConnectionClosed(WebsocketError):
-    """Connection exception."""
```

### Comparing `heatzypy-2.5.0/heatzypy/heatzy.py` & `heatzypy-2.5.1/heatzypy/heatzy.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,19 +35,14 @@
             host = DFLT_API_URL
 
         self._auth = Auth(session, username, password, time_out, host, use_tls)
         self.websocket = Websocket(session, self._auth, WS_HOST, use_tls)
         self.session = session
         self.request = self._auth.request
 
-    @property
-    def is_connected(self) -> bool:
-        """Return if we are connect to the WebSocket."""
-        return self.websocket.is_connected
-
     async def async_bindings(self) -> dict[str, list[dict[str, Any]]]:
         """Fetch all configured devices."""
         return await self.request("bindings")
 
     async def async_get_devices(self) -> dict[str, Any]:
         """Fetch all configured devices."""
         response = await self.async_bindings()
```

### Comparing `heatzypy-2.5.0/heatzypy/websocket.py` & `heatzypy-2.5.1/heatzypy/websocket.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Class for websocket."""
 
 from __future__ import annotations
 
 import asyncio
+import json
 import logging
 import socket
 from typing import TYPE_CHECKING, Any, Callable, cast
 
 import aiohttp
+from aiohttp import ClientSession, ClientWebSocketResponse
 from yarl import URL as yurl
 
 from .const import APPLICATION_ID, WS_PING_INTERVAL, WS_PORT, WSS_PORT
 from .exception import AuthenticationFailed, ConnectionFailed, WebsocketError
 
 if TYPE_CHECKING:
     from .auth import Auth
@@ -19,275 +21,310 @@
 logger = logging.getLogger(__name__)
 
 
 class Websocket:
     """Heatzy websocket."""
 
     def __init__(
-        self,
-        session: aiohttp.ClientSession,
-        auth: Auth,
-        host: str,
-        use_tls: bool = True,
+        self, session: ClientSession, auth: Auth, host: str, use_tls: bool = True
     ) -> None:
         """Initialize."""
         self.session = session
         self._auth = auth
-        self._client: aiohttp.ClientWebSocketResponse = cast(
-            aiohttp.ClientWebSocketResponse, None
-        )
-        self.bindings: dict[str, Any] = {}
+        self.ws: ClientWebSocketResponse = cast(ClientWebSocketResponse, None)
+
         self.devices: dict[str, Any] = {}
+
         self._return_all: bool = False
         self._host = host
         self._scheme = "wss" if use_tls else "ws"
         self._port = WSS_PORT if use_tls else WS_PORT
 
+        self.logged_in: bool = False
+        self.subscribed_devices: list[str] = []
         self.last_invalid_msg: dict[str, Any] | None = None
 
+        self._event: asyncio.Event | None = None
+        self._callbacks: list[Callable[..., None]] = []
+
     @property
     def is_connected(self) -> bool:
         """Return if we are connect to the WebSocket."""
-        return self._client is not None and not self._client.closed
+        return self.ws is not None and not self.ws.closed
 
-    async def async_bindings(self) -> None:
+    async def async_fetch_binding_devices(self) -> None:
         """Return bindings devices."""
         bindings = await self._auth.request("bindings")
-        self.bindings = {
-            device["did"]: device for device in bindings.get("devices", {})
-        }
-
-    async def async_get_device(self, device_id: str) -> dict[str, Any] | None:
-        """Return device data while listen connection."""
-        if not self._client or not self.is_connected:
-            msg = "Not connected to a Heatzy WebSocket"
-            raise WebsocketError(msg)
-
-        c2s = {"cmd": "c2s_read", "data": {"did": device_id}}
-        logger.debug("WEBSOCKET >>> %s", c2s)
-        await self._client.send_json(c2s)
-
-        return self.bindings.get(device_id)
+        for info in bindings.get("devices", {}):
+            self.devices.update({info["did"]: info})
 
     async def async_get_devices(self) -> dict[str, Any]:
         """Return all devices data while listen connection."""
-        if not self._client or not self.is_connected:
-            msg = "Not connected to a Heatzy WebSocket"
-            raise WebsocketError(msg)
-
-        for did in self.bindings:
-            c2s = {"cmd": "c2s_read", "data": {"did": did}}
-            logger.debug("WEBSOCKET >>> %s", c2s)
-            await self._client.send_json(c2s)
-
-        return self.bindings
+        for did in self.devices:
+            payload = {"cmd": "c2s_read", "data": {"did": did}}
+            await self._send_cmd(payload)
+        return self.devices
 
     async def async_control_device(
         self, device_id: str, payload: dict[str, dict[str, Any]]
     ) -> None:
         """Send command to device.
 
         Args:
         ----
             - payload: raw or attrs dictionary containing the actions dictionary
              {"raw": [1,1,3]} or {"attrs": {"mode": "cft"} }
         """
-        if not self._client or not self.is_connected:
-            msg = "Not connected to a Heatzy WebSocket"
-            raise WebsocketError(msg)
-
         cmd = "c2s_raw" if payload.get("raw") else "c2s_write"
-        c2s = {"cmd": cmd, "data": {"did": device_id, **payload}}
-        logger.debug("WEBSOCKET >>> %s", c2s)
-        await self._client.send_json(c2s)
+        control = {"cmd": cmd, "data": {"did": device_id, **payload}}
+        await self._send_cmd(control)
 
     async def _async_heartbeat(self) -> None:
         """Heatbeat websocket."""
-        while not self._client.closed:
-            c2s = {"cmd": "ping"}
-            logger.debug("WEBSOCKET >>> %s", c2s)
-            await self._client.send_json(c2s)
+        while not self.ws.closed:
+            await self.async_ping()
             await asyncio.sleep(WS_PING_INTERVAL)
 
-    async def async_connect(self, auto_subscribe: bool = True) -> None:
+    async def async_ping(self) -> None:
+        """Send ping."""
+        await self._send_cmd({"cmd": "ping"})
+
+    async def async_connect(
+        self,
+        auto_subscribe: bool = True,
+        all_devices: bool = False,
+        event: asyncio.Event | None = None,
+    ) -> None:
         """Connect to the WebSocket.
 
         Args:
         ---
             - auto_subscribe set True the server automatically subscribes to all the bound devices
             if false, you need to select the devices to be subscribed to through the following async_subscribe
         """
         if self.is_connected:
             return
 
         if not self.session:
             raise WebsocketError("Session not found")
 
-        if not self.bindings:
-            await self.async_bindings()
+        if not self.devices:
+            await self.async_fetch_binding_devices()
+
+        self._return_all = all_devices is True
 
         try:
             url = yurl.build(
                 scheme=self._scheme, host=self._host, port=self._port, path="/ws/app/v1"
             )
-            self._client = await self.session.ws_connect(url=url)
+            self.ws = await self.session.ws_connect(url=url)
             logger.debug("WEBSOCKET Connected to a %s Websocket", url)
+
+            # Create a background task to receive messages
+            asyncio.ensure_future(self.async_listen(self.ws))
+
         except (
             aiohttp.WSServerHandshakeError,
             aiohttp.ClientConnectionError,
             socket.gaierror,
         ) as exception:
-            msg = (
+            raise ConnectionFailed(
                 f"Error occurred while communicating with device on WebSocket at {url}"
-            )
-            raise ConnectionFailed(msg) from exception
+            ) from exception
 
         try:
             await self.async_login(auto_subscribe)
         except WebsocketError as error:
             raise AuthenticationFailed(error) from error
 
+        try:
+            if self._return_all:
+                await self.async_get_devices()
+        except WebsocketError as error:
+            raise AuthenticationFailed(error) from error
+
     async def async_login(self, auto_subscribe: bool = True) -> None:
         """Login to websocket."""
-        if not self._client or not self.is_connected:
-            msg = "Not connected to a Heatzy WebSocket"
-            raise WebsocketError(msg)
 
         token_data = await self._auth.async_get_token()
 
-        c2s = {
+        payload = {
             "cmd": "login_req",
             "data": {
                 "appid": APPLICATION_ID,
                 "uid": token_data.get("uid"),
                 "token": token_data.get("token"),
                 "p0_type": "attrs_v4",
                 "heartbeat_interval": WS_PING_INTERVAL,
                 "auto_subscribe": auto_subscribe,
             },
         }
-        logger.debug("WEBSOCKET >>> %s", c2s)
-        await self._client.send_json(c2s)
+        await self._send_cmd(payload)
+        asyncio.create_task(self._async_heartbeat())
 
     async def async_listen(
-        self,
-        callback: Callable[..., None] | None = None,
-        callbackChange: Callable[..., None] | None = None,
-        callbackStatus: Callable[..., None] | None = None,
-        all_devices: bool = False,
-        event: asyncio.Event | None = None,
+        self, ws: ClientWebSocketResponse, event: asyncio.Event | None = None
     ) -> None:
         """Listen for events on the WebSocket.
 
         Args:
         ----
             callback: Method to call when a state update is received from the device.
             callbackChange: Method to call when the device is bound or unbound by the user.
             callbackStatus: Method to call when the device goes online or offline.
             all_devices: set True , returns all devices in the callback
             instead of the device that performed the update
             event: trigger Event.set()
         """
-        if not self._client or not self.is_connected:
-            logger.debug("WEBSOCKET Connect to the websocket")
-            await self.async_connect()
-
-        try:
-            if all_devices:
-                self._return_all = all_devices
-                await self.async_get_devices()
-        except WebsocketError as error:
-            raise WebsocketError("Fetch all devices failed (%s)", error) from error
-
-        asyncio.create_task(self._async_heartbeat())
-
-        while not self._client.closed:
-            message = await self._client.receive()
+        while not ws.closed:
+            message = await ws.receive()
 
             if event:
                 event.set()
 
             if message.type == aiohttp.WSMsgType.ERROR:
-                raise ConnectionFailed(self._client.exception())
+                raise ConnectionFailed(ws.exception())
+
+            if message.type == aiohttp.WSMsgType.BINARY:
+                pass
 
             if message.type == aiohttp.WSMsgType.TEXT:
-                message_data = message.json()
-                logger.debug("WEBSOCKET <<< %s", message_data)
-                data = message_data.get("data")
-                cmd = message_data.get("cmd")
-                self.last_invalid_msg = None
-                if isinstance(data, dict):
-                    match cmd:
-                        case "s2c_invalid_msg":
-                            self.last_invalid_msg = message_data
-                            logger.warn("Received invalid message (%s)", message_data)
-                        case "login_res":
-                            if message_data.get("data", {}).get("success") is False:
-                                raise AuthenticationFailed(message_data)
-                            logger.debug("WEBSOCKET Successfully authenticated")
-                        case "s2c_noti":
-                            if callback:
-                                if self._return_all is False:
-                                    callback(data)
-                                elif self.merge_data(self.bindings, data):
-                                    callback(self.bindings)
-                        case "s2c_binding_changed":
-                            await self.async_bindings()
-                            if (did := data.get("did")) and data.get("bind"):
-                                await self.async_get_device(did)
-                            if (did := data.get("did")) and (data.get("bind") is False):
-                                await self.bindings.pop(did, None)
-                            if callbackChange:
-                                callbackChange(data)
-                        case "s2c_online_status":
-                            if did := data.get("did"):
-                                await self.async_get_device(did)
-                            if callbackStatus:
-                                callbackStatus(data)
-                        case "pong":
-                            pass
+                try:
+                    message_data = message.json()
+                    logger.debug("WEBSOCKET <<< %s", message_data)
+                    data = message_data.get("data")
+                    cmd = message_data.get("cmd")
+                    if data and cmd:
+                        self.last_invalid_msg = None
+                        match cmd:
+                            case "login_res":
+                                await self._handle_login(data)
+                            case "subscribe_res":
+                                await self._handle_subscription(data)
+                            case "s2c_invalid_msg":
+                                await self._handle_invalid_msg(data)
+                            case "s2c_noti":
+                                await self._handle_notification(data)
+                            case "s2c_binding_changed":
+                                await self._handle_binding_change(data)
+                            case "s2c_online_status":
+                                await self._handle_status_change(data)
+                    elif cmd == "pong":
+                        await self._hand_pong(message_data)
+                    else:
+                        logger.warn(f"Received invalid message: {message}")
+                except json.JSONDecodeError:
+                    logger.error("Invalid JSON format for the received message.")
 
             if message.type in (
                 aiohttp.WSMsgType.CLOSE,
                 aiohttp.WSMsgType.CLOSED,
                 aiohttp.WSMsgType.CLOSING,
             ):
                 raise WebsocketError("Connection to the WebSocket has been closed")
 
     async def async_disconnect(self) -> None:
         """Disconnect from the WebSocket of a device."""
-        if not self._client or not self.is_connected:
+        if not self.ws or not self.is_connected:
             return
 
-        await self._client.close()
+        await self.ws.close()
 
     async def async_subscribe(self, device_ids: list[str]) -> None:
         """Subscribed to the bound device.
 
         This API only applies to scenarios where the connect or login parameter auto_subscribe is set to false
 
         Args:
         ----
             - device_ids : Array of did
         """
-        if not self._client or not self.is_connected:
-            msg = "Not connected to a Heatzy WebSocket"
-            raise WebsocketError(msg)
-
         dids = [{"did": did} for did in device_ids]
+        payload = {"cmd": "subscribe_req", "data": dids}
+        await self._send_cmd(payload)
+
+    async def _hand_pong(self, data: dict[str, Any]) -> None:
+        """Handle ping receive."""
+        pass
+
+    async def _handle_login(self, data: dict[str, Any]) -> None:
+        """Handle login response."""
+        if data.get("success") is False:
+            raise AuthenticationFailed(data)
+        logger.debug("WEBSOCKET Successfully authenticated")
+        self.logged_in = True
+
+    async def _handle_subscription(self, data: dict[str, Any]) -> None:
+        """Handle the response of subscription."""
+        devices = cast(list[Any], data.get("success"))
+        for device in devices:
+            if (did := device["did"]) not in self.subscribed_devices:
+                self.subscribed_devices.append(did)
+
+    async def _handle_notification(self, data: dict[str, Any]) -> None:
+        """Handle a notification receive by client."""
+        if did := data.get("did"):
+            device = self.devices.get(did)
+            if device and (attrs := data.get("attrs")):
+                device["attrs"] = attrs
+                if len(self._callbacks) > 0:
+                    if self._return_all:
+                        if self.check_full(self.devices):
+                            self._run_callbacks(self.devices)
+                    else:
+                        self._run_callbacks(device)
+
+    async def _handle_invalid_msg(self, data: dict[str, Any]) -> None:
+        """Handle a notification receive by client."""
+        logger.warn("Received invalid message: %s", data)
+        self.last_invalid_msg = data
+
+    async def _handle_binding_change(self, data: dict[str, Any]) -> None:
+        """Handle a new binding status."""
+        if (did := data.get("did")) and (data.get("bind") is False):
+            self.devices.pop(did, None)
+        elif did:
+            bindings = await self._auth.request("bindings")
+            if bindings and (data := bindings.get(did, {})):
+                self.devices.update({did: data})
+
+    async def _handle_status_change(self, data: dict[str, Any]) -> None:
+        """Handle a new status."""
+        if device := self.devices.get(data.get("did", "")):
+            await device.async_update(data)
+
+    async def _send_cmd(self, payload: dict[str, Any]) -> None:
+        """Send command to websocket."""
+        if not self.ws or not self.is_connected:
+            raise WebsocketError("Not connected to a Heatzy WebSocket")
 
-        c2s = {"cmd": "subscribe_req", "data": dids}
-        logger.debug("WEBSOCKET >>> %s", c2s)
-        await self._client.send_json(c2s)
+        logger.debug("WEBSOCKET >>> %s", payload)
+        await self.ws.send_json(payload)
 
     @staticmethod
-    def merge_data(bindings: dict[str, Any], data: dict[str, Any]) -> bool:
+    def check_full(devices: dict[str, Any]) -> bool:
         """Merge data."""
-        if bindings and (did := data.get("did")) and (device := bindings.get(did)):
-            device["attrs"] = data.get("attrs", {})
+        attrs_fills = [
+            device["did"] for device in devices.values() if device.get("attrs")
+        ]
+        return list(devices.keys()) == attrs_fills
 
-        n_devices = len(bindings.keys())
-        for binding in bindings.values():
-            if binding.get("attrs"):
-                n_devices -= 1
+    def register_callback(self, callback: Callable[..., None]) -> None:
+        """Register a data update callback.
+
+        :param func callback: Takes one function, which should be registered.
+        """
+        if callback not in self._callbacks:
+            self._callbacks.append(callback)
+
+    def unregister_callback(self, callback: Callable[..., None]) -> None:
+        """Unregister a data update callback.
+
+        :param func callback: Takes one function, which should be unregistered.
+        """
+        if callback in self._callbacks:
+            self._callbacks.remove(callback)
 
-        return n_devices == 0
+    def _run_callbacks(self, data: dict[str, Any]) -> None:
+        """Schedule a data callbacks."""
+        for fn in self._callbacks:
+            fn(data)
```

### Comparing `heatzypy-2.5.0/heatzypy.egg-info/PKG-INFO` & `heatzypy-2.5.1/heatzypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.0
+Version: 2.5.1
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.0/heatzypy.egg-info/SOURCES.txt` & `heatzypy-2.5.1/heatzypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.0/pyproject.toml` & `heatzypy-2.5.1/pyproject.toml`

 * *Files identical despite different names*

