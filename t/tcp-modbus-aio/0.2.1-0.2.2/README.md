# Comparing `tmp/tcp_modbus_aio-0.2.1.tar.gz` & `tmp/tcp_modbus_aio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.2.1.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.2.2.tar", max compression
```

## Comparing `tcp_modbus_aio-0.2.1.tar` & `tcp_modbus_aio-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/LICENSE
--rw-r--r--   0        0        0     1649 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/README.md
--rw-r--r--   0        0        0      857 2024-04-25 23:27:30.469780 tcp_modbus_aio-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-25 23:27:30.477780 tcp_modbus_aio-0.2.1/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    20152 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/client.py
--rw-r--r--   0        0        0      267 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1167 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-04-25 23:27:29.761787 tcp_modbus_aio-0.2.1/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1649 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/README.md
+-rw-r--r--   0        0        0      857 2024-05-01 21:34:44.383420 tcp_modbus_aio-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-01 21:34:44.391420 tcp_modbus_aio-0.2.2/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    20487 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/client.py
+-rw-r--r--   0        0        0      267 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1167 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.2/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.2.1/LICENSE` & `tcp_modbus_aio-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.1/README.md` & `tcp_modbus_aio-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.1/pyproject.toml` & `tcp_modbus_aio-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.2.1"
+version = "0.2.2"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tcp_modbus_aio-0.2.1/tcp_modbus_aio/client.py` & `tcp_modbus_aio-0.2.2/tcp_modbus_aio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 import logging
 import random
 import socket
 import struct
 import time
 import uuid
 from dataclasses import dataclass
-from types import TracebackType
-from typing import Any, ClassVar
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from cachetools import TTLCache
-from typing_extensions import Self
-from umodbus.functions import ModbusFunction
 
 from tcp_modbus_aio.exceptions import (
     ModbusCommunicationFailureError,
     ModbusNotConnectedError,
 )
 from tcp_modbus_aio.ping import ping_ip
 from tcp_modbus_aio.typed_functions import (
     ModbusFunctionT,
     ReadCoils,
     create_function_from_response_pdu,
 )
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from typing_extensions import Self
+    from umodbus.functions import ModbusFunction
+
 
 @dataclass
 class CoilWatchStatus:
     msg: ModbusFunction
 
     memo_key: Any
     expiry: float
@@ -304,15 +307,24 @@
         if self._writer is not None:
             if self.logger is not None:
                 self.logger.warning(
                     f"[{self}][clear_tcp_connection] closing TCP connection #{self._lifetime_tcp_connection_num}"
                 )
 
             self._writer.close()
-            await self._writer.wait_closed()
+
+            try:
+                await self._writer.wait_closed()
+            except TimeoutError:
+                if self.logger is not None:
+                    self.logger.warning(
+                        f"[{self}][clear_tcp_connection] connection close timed out, continuing anyway"
+                    )
+
+                pass
 
         self._reader = None
         self._writer = None
 
     async def test_connection(
         self, timeout: float | None = DEFAULT_MODBUS_TIMEOUT_SEC
     ) -> None:
```

### Comparing `tcp_modbus_aio-0.2.1/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.2.2/tcp_modbus_aio/ping.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.1/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.2.2/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.1/PKG-INFO` & `tcp_modbus_aio-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.2.1
+Version: 0.2.2
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

