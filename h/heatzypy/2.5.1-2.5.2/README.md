# Comparing `tmp/heatzypy-2.5.1.tar.gz` & `tmp/heatzypy-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatzypy-2.5.1.tar", last modified: Wed May  1 16:24:37 2024, max compression
+gzip compressed data, was "heatzypy-2.5.2.tar", last modified: Wed May  1 17:27:21 2024, max compression
```

## Comparing `heatzypy-2.5.1.tar` & `heatzypy-2.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.334143 heatzypy-2.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 16:24:27.000000 heatzypy-2.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 16:24:27.000000 heatzypy-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 16:24:27.000000 heatzypy-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 16:24:37.338143 heatzypy-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 16:24:27.000000 heatzypy-2.5.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2353 2024-05-01 16:24:27.000000 heatzypy-2.5.1/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/heatzypy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/heatzy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-01 16:24:27.000000 heatzypy-2.5.1/heatzypy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:24:37.338143 heatzypy-2.5.1/heatzypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 16:24:37.000000 heatzypy-2.5.1/heatzypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 16:24:27.000000 heatzypy-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 16:24:27.000000 heatzypy-2.5.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 16:24:27.000000 heatzypy-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:24:37.338143 heatzypy-2.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.266373 heatzypy-2.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 17:27:12.000000 heatzypy-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 17:27:12.000000 heatzypy-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 17:27:21.266373 heatzypy-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 17:27:12.000000 heatzypy-2.5.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2353 2024-05-01 17:27:12.000000 heatzypy-2.5.2/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/heatzypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/heatzy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.266373 heatzypy-2.5.2/heatzypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:27:20.000000 heatzypy-2.5.2/heatzypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 17:27:12.000000 heatzypy-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 17:27:12.000000 heatzypy-2.5.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 17:27:12.000000 heatzypy-2.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:27:21.266373 heatzypy-2.5.2/setup.cfg
```

### Comparing `heatzypy-2.5.1/.github/dependabot.yml` & `heatzypy-2.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.github/workflows/auto-approve.yml` & `heatzypy-2.5.2/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.github/workflows/lint.yml` & `heatzypy-2.5.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.github/workflows/pythonpublish.yml` & `heatzypy-2.5.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.github/workflows/release.yml` & `heatzypy-2.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.gitignore` & `heatzypy-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/.pre-commit-config.yaml` & `heatzypy-2.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/LICENSE` & `heatzypy-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/PKG-INFO` & `heatzypy-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.1
+Version: 2.5.2
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.1/README.md` & `heatzypy-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/example.py` & `heatzypy-2.5.2/example.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/heatzypy/auth.py` & `heatzypy-2.5.2/heatzypy/auth.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/heatzypy/exception.py` & `heatzypy-2.5.2/heatzypy/exception.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/heatzypy/heatzy.py` & `heatzypy-2.5.2/heatzypy/heatzy.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/heatzypy/websocket.py` & `heatzypy-2.5.2/heatzypy/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ) -> None:
         """Initialize."""
         self.session = session
         self._auth = auth
         self.ws: ClientWebSocketResponse = cast(ClientWebSocketResponse, None)
 
         self.devices: dict[str, Any] = {}
+        self.is_all_updated = False
 
         self._return_all: bool = False
         self._host = host
         self._scheme = "wss" if use_tls else "ws"
         self._port = WSS_PORT if use_tls else WS_PORT
 
         self.logged_in: bool = False
@@ -47,14 +48,19 @@
         self._callbacks: list[Callable[..., None]] = []
 
     @property
     def is_connected(self) -> bool:
         """Return if we are connect to the WebSocket."""
         return self.ws is not None and not self.ws.closed
 
+    @property
+    def is_updated(self) -> bool:
+        """Return if all devices updated."""
+        return self.check_full(self.devices)
+
     async def async_fetch_binding_devices(self) -> None:
         """Return bindings devices."""
         bindings = await self._auth.request("bindings")
         for info in bindings.get("devices", {}):
             self.devices.update({info["did"]: info})
 
     async def async_get_devices(self) -> dict[str, Any]:
@@ -107,24 +113,25 @@
         if not self.session:
             raise WebsocketError("Session not found")
 
         if not self.devices:
             await self.async_fetch_binding_devices()
 
         self._return_all = all_devices is True
+        self._event = event
 
         try:
             url = yurl.build(
                 scheme=self._scheme, host=self._host, port=self._port, path="/ws/app/v1"
             )
             self.ws = await self.session.ws_connect(url=url)
             logger.debug("WEBSOCKET Connected to a %s Websocket", url)
 
             # Create a background task to receive messages
-            asyncio.ensure_future(self.async_listen(self.ws))
+            # asyncio.ensure_future(self.async_listen())
 
         except (
             aiohttp.WSServerHandshakeError,
             aiohttp.ClientConnectionError,
             socket.gaierror,
         ) as exception:
             raise ConnectionFailed(
@@ -157,36 +164,25 @@
                 "heartbeat_interval": WS_PING_INTERVAL,
                 "auto_subscribe": auto_subscribe,
             },
         }
         await self._send_cmd(payload)
         asyncio.create_task(self._async_heartbeat())
 
-    async def async_listen(
-        self, ws: ClientWebSocketResponse, event: asyncio.Event | None = None
-    ) -> None:
-        """Listen for events on the WebSocket.
+    async def async_listen(self) -> None:
+        """Listen for events on the WebSocket."""
 
-        Args:
-        ----
-            callback: Method to call when a state update is received from the device.
-            callbackChange: Method to call when the device is bound or unbound by the user.
-            callbackStatus: Method to call when the device goes online or offline.
-            all_devices: set True , returns all devices in the callback
-            instead of the device that performed the update
-            event: trigger Event.set()
-        """
-        while not ws.closed:
-            message = await ws.receive()
+        while not self.ws.closed:
+            message = await self.ws.receive()
 
-            if event:
-                event.set()
+            if self._event:
+                self._event.set()
 
             if message.type == aiohttp.WSMsgType.ERROR:
-                raise ConnectionFailed(ws.exception())
+                raise ConnectionFailed(self.ws.exception())
 
             if message.type == aiohttp.WSMsgType.BINARY:
                 pass
 
             if message.type == aiohttp.WSMsgType.TEXT:
                 try:
                     message_data = message.json()
```

### Comparing `heatzypy-2.5.1/heatzypy.egg-info/PKG-INFO` & `heatzypy-2.5.2/heatzypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.1
+Version: 2.5.2
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.1/heatzypy.egg-info/SOURCES.txt` & `heatzypy-2.5.2/heatzypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.1/pyproject.toml` & `heatzypy-2.5.2/pyproject.toml`

 * *Files identical despite different names*

