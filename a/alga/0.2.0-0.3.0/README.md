# Comparing `tmp/alga-0.2.0.tar.gz` & `tmp/alga-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alga-0.2.0.tar", max compression
+gzip compressed data, was "alga-0.3.0.tar", max compression
```

## Comparing `alga-0.2.0.tar` & `alga-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-12-20 08:38:20.327932 alga-0.2.0/LICENSE
--rw-r--r--   0        0        0      433 2024-01-06 19:56:28.339599 alga-0.2.0/README.md
--rw-r--r--   0        0        0     1343 2024-01-06 19:59:01.052410 alga-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-06 19:59:06.639361 alga-0.2.0/src/alga/__init__.py
--rw-r--r--   0        0        0      871 2024-01-06 19:54:46.432901 alga-0.2.0/src/alga/__main__.py
--rw-r--r--   0        0        0      323 2024-01-06 19:51:52.082648 alga-0.2.0/src/alga/cli_adhoc.py
--rw-r--r--   0        0        0     1350 2024-01-06 19:36:18.070232 alga-0.2.0/src/alga/cli_app.py
--rw-r--r--   0        0        0     1450 2023-12-20 22:35:45.232183 alga-0.2.0/src/alga/cli_channel.py
--rw-r--r--   0        0        0      708 2023-12-20 22:35:21.615505 alga-0.2.0/src/alga/cli_input.py
--rw-r--r--   0        0        0      536 2023-12-20 21:58:46.439810 alga-0.2.0/src/alga/cli_media.py
--rw-r--r--   0        0        0      275 2024-01-06 19:36:49.246127 alga-0.2.0/src/alga/cli_power.py
--rw-r--r--   0        0        0     1709 2024-01-06 19:54:26.549861 alga-0.2.0/src/alga/cli_setup.py
--rw-r--r--   0        0        0      467 2023-12-20 22:34:47.343308 alga-0.2.0/src/alga/cli_sound_output.py
--rw-r--r--   0        0        0      891 2023-12-20 22:34:28.042546 alga-0.2.0/src/alga/cli_volume.py
--rw-r--r--   0        0        0     1472 2023-12-20 23:01:23.886518 alga-0.2.0/src/alga/client.py
--rw-r--r--   0        0        0     4699 2024-01-01 15:59:01.471452 alga-0.2.0/src/alga/payloads.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 alga-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-12-20 08:38:20.327932 alga-0.3.0/LICENSE
+-rw-r--r--   0        0        0      433 2024-01-06 19:56:28.339599 alga-0.3.0/README.md
+-rw-r--r--   0        0        0     1673 2024-05-01 09:35:10.971358 alga-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-01-06 19:59:06.639361 alga-0.3.0/src/alga/__init__.py
+-rw-r--r--   0        0        0      871 2024-01-19 20:55:26.058493 alga-0.3.0/src/alga/__main__.py
+-rw-r--r--   0        0        0      323 2024-01-06 19:51:52.082648 alga-0.3.0/src/alga/cli_adhoc.py
+-rw-r--r--   0        0        0     1457 2024-04-30 19:40:42.019716 alga-0.3.0/src/alga/cli_app.py
+-rw-r--r--   0        0        0     1484 2024-02-22 22:19:49.614885 alga-0.3.0/src/alga/cli_channel.py
+-rw-r--r--   0        0        0      708 2024-04-30 19:46:20.165704 alga-0.3.0/src/alga/cli_input.py
+-rw-r--r--   0        0        0      536 2023-12-20 21:58:46.439810 alga-0.3.0/src/alga/cli_media.py
+-rw-r--r--   0        0        0      275 2024-01-06 19:36:49.246127 alga-0.3.0/src/alga/cli_power.py
+-rw-r--r--   0        0        0     1774 2024-05-01 09:30:32.111580 alga-0.3.0/src/alga/cli_setup.py
+-rw-r--r--   0        0        0      467 2023-12-20 22:34:47.343308 alga-0.3.0/src/alga/cli_sound_output.py
+-rw-r--r--   0        0        0      891 2023-12-20 22:34:28.042546 alga-0.3.0/src/alga/cli_volume.py
+-rw-r--r--   0        0        0     1524 2024-05-01 09:30:32.111596 alga-0.3.0/src/alga/client.py
+-rw-r--r--   0        0        0     4699 2024-01-01 15:59:01.471452 alga-0.3.0/src/alga/payloads.py
+-rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 alga-0.3.0/PKG-INFO
```

### Comparing `alga-0.2.0/LICENSE` & `alga-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/pyproject.toml` & `alga-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alga"
-version = "0.2.0"
+version = "0.3.0"
 description = "CLI for remote controlling LG webOS TVs"
 authors = ["Jeppe Fihl-Pearson <jeppe@tenzer.dk>"]
 license = "MIT"
 repository = "https://github.com/Tenzer/alga"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -22,38 +22,58 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 rich = "*"
 typer = {version = "*", extras = ["all"]}
 wakeonlan = "*"
 websocket-client = "*"
 
-[tool.poetry.scripts]
-alga = "alga.__main__:app"
-
 [tool.poetry.group.dev.dependencies]
+coverage = "*"
+faker = "*"
 mypy = "*"
+pytest = "*"
+pytest-cov = "*"
+
+[tool.poetry.scripts]
+alga = "alga.__main__:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py312"
+
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "I",  # isort
     "PL",  # Pylint
     "UP",  # pyupgrade
 ]
 ignore = [
     "E501",  # Line too long
     "UP007",  # Use `X | Y` for type annotations"
 ]
 
-[tool.ruff.format]
-skip-magic-trailing-comma = true
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
+known-first-party = ["alga"]
 lines-after-imports = 2
 split-on-trailing-comma = false
+
+[tool.ruff.format]
+skip-magic-trailing-comma = true
+
+[tool.pytest.ini_options]
+addopts = """
+    --cov
+    --cov-fail-under=100
+    --cov-report=term-missing:skip-covered
+    --no-cov-on-fail
+"""
+
+[tool.coverage.report]
+exclude_also = [
+    "if __name__ == .__main__.:",
+]
```

### Comparing `alga-0.2.0/src/alga/__main__.py` & `alga-0.3.0/src/alga/__main__.py`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/src/alga/cli_app.py` & `alga-0.3.0/src/alga/cli_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Annotated, Optional
 
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from typer import Argument, Typer
 
@@ -17,36 +18,39 @@
         "ssap://com.webos.applicationManager/getForegroundAppInfo"
     )
     print(f"The current app is [bold]{response['appId']}[/bold]")
 
 
 @app.command()
 def close(app_id: Annotated[str, Argument()]) -> None:
-    client.request("ssap://system.launcher/close")
+    client.request("ssap://system.launcher/close", {"id": app_id})
 
 
 @app.command()
 def launch(
     app_id: Annotated[str, Argument()],
-    content: Annotated[Optional[str], Argument()] = None,
+    data: Annotated[Optional[str], Argument()] = None,
 ) -> None:
-    client.request("ssap://system.launcher/launch", {"id": app_id})
+    payload = {"id": app_id}
+    if data:
+        payload.update(json.loads(data))
+    client.request("ssap://system.launcher/launch", payload)
 
 
 @app.command()
 def list() -> None:
     response = client.request("ssap://com.webos.applicationManager/listApps")
 
     table = Table()
     table.add_column("Name")
     table.add_column("ID")
 
     all_apps = []
-    for a in response["apps"]:
-        all_apps.append([a["title"], a["id"]])
+    for app in response["apps"]:
+        all_apps.append([app["title"], app["id"]])
 
     for row in sorted(all_apps):
         table.add_row(*row)
 
     console = Console()
     console.print(table)
```

### Comparing `alga-0.2.0/src/alga/cli_channel.py` & `alga-0.3.0/src/alga/cli_channel.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,23 +41,23 @@
     table = Table()
     table.add_column("Type")
     table.add_column("Number")
     table.add_column("Name")
 
     all_channels = []
     type_to_emoji = {1: "📺", 2: "📻"}
-    for c in response["channelList"]:
+    for channel in response["channelList"]:
         # The first item is for sorting
         all_channels.append(
             [
-                int(c["channelNumber"]),
-                type_to_emoji.get(c["channelTypeId"], "❓"),
-                c["channelNumber"],
-                c["channelName"],
+                int(channel["channelNumber"]),
+                type_to_emoji.get(channel["channelTypeId"], "❓"),
+                channel["channelNumber"],
+                channel["channelName"],
             ]
         )
 
     for row in sorted(all_channels):
-        table.add_row(*row)
+        table.add_row(*row[1:])
 
     console = Console()
     console.print(table)
```

### Comparing `alga-0.2.0/src/alga/cli_input.py` & `alga-0.3.0/src/alga/cli_input.py`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/src/alga/cli_media.py` & `alga-0.3.0/src/alga/cli_media.py`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/src/alga/cli_setup.py` & `alga-0.3.0/src/alga/cli_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from ipaddress import ip_address
 from socket import gaierror, getaddrinfo
 from typing import Annotated
 
 from rich import print
-from typer import Argument
+from typer import Argument, Exit
 
 from alga import client
 from alga.payloads import get_hello_data
 
 
 def _ip_from_hostname(hostname: str) -> str | None:
     try:
@@ -26,26 +26,29 @@
         ip = ip_address(hostname).compressed
     except ValueError:
         ip = _ip_from_hostname(hostname)
         if not ip:
             print(
                 f"[red]Could not find any host by the name '{hostname}'.[/red] Is the TV on and connected to the network?"
             )
-            return
+            raise Exit(code=1)
 
-    with client.new(perform_handshake=False, timeout=60) as connection:
+    with client.new(
+        perform_handshake=False, timeout=60
+    ) as connection:  # pragma: no cover
         connection.send(json.dumps(get_hello_data()))
         response = json.loads(connection.recv())
         assert response == {
             "id": "register_0",
             "payload": {"pairingType": "PROMPT", "returnValue": True},
             "type": "response",
         }, "Unexpected response received"
         print("Please approve the connection request on the TV now...")
 
         response = json.loads(connection.recv())
         if "client-key" not in response["payload"]:
             print("[red]Setup failed![/red]")
-            return
+            raise Exit(code=1)
+
         print(
             f"Got key: {response['payload']['client-key']}. Please put this in the `ALGA_KEY` environment variable"
         )
```

### Comparing `alga-0.2.0/src/alga/cli_volume.py` & `alga-0.3.0/src/alga/cli_volume.py`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/src/alga/client.py` & `alga-0.3.0/src/alga/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 
 HOSTNAME = getenv("ALGA_HOST", "lgwebostv")
 KEY = getenv("ALGA_KEY", "")
 
 
 @contextmanager
-def new(perform_handshake: bool = True, timeout: int = 3) -> Iterator[WebSocket]:
+def new(
+    perform_handshake: bool = True, timeout: int = 3
+) -> Iterator[WebSocket]:  # pragma: no cover
     connection = WebSocket(sslopt={"cert_reqs": ssl.CERT_NONE})
     connection.connect(f"wss://{HOSTNAME}:3001/", suppress_origin=True, timeout=timeout)  # type: ignore[no-untyped-call]
 
     if perform_handshake:
         connection.send(json.dumps(get_hello_data(KEY)))
         response = json.loads(connection.recv())
         if "client-key" not in response["payload"]:
@@ -29,15 +31,17 @@
 
     try:
         yield connection
     finally:
         connection.close()
 
 
-def request(uri: str, data: dict[str, Any] | None = None) -> dict[str, Any]:
+def request(
+    uri: str, data: dict[str, Any] | None = None
+) -> dict[str, Any]:  # pragma: no cover
     with new() as connection:
         request: dict[str, Any] = {"type": "request", "uri": uri}
 
         if data:
             request.update(payload=data)
 
         connection.send(json.dumps(request))
```

### Comparing `alga-0.2.0/src/alga/payloads.py` & `alga-0.3.0/src/alga/payloads.py`

 * *Files identical despite different names*

### Comparing `alga-0.2.0/PKG-INFO` & `alga-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alga
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI for remote controlling LG webOS TVs
 Home-page: https://github.com/Tenzer/alga
 License: MIT
 Author: Jeppe Fihl-Pearson
 Author-email: jeppe@tenzer.dk
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

