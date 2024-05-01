# Comparing `tmp/skytable_py-0.0.2.tar.gz` & `tmp/skytable_py-0.1.0.tar.gz`

## Comparing `skytable_py-0.0.2.tar` & `skytable_py-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,20 @@
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 skytable_py-0.0.2/run_tests.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 skytable_py-0.0.2/src/skytable_py/__init__.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 skytable_py-0.0.2/src/skytable_py/connection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skytable_py-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 skytable_py-0.0.2/tests/test_config.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 skytable_py-0.0.2/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.0.2/LICENSE
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 skytable_py-0.0.2/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 skytable_py-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 skytable_py-0.1.0/run_tests.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 skytable_py-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/config.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/connection.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/exception.py
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/protocol.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/query.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 skytable_py-0.1.0/src/skytable_py/response.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_encoding.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_query.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 skytable_py-0.1.0/tests/test_response.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 skytable_py-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.1.0/LICENSE
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 skytable_py-0.1.0/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 skytable_py-0.1.0/PKG-INFO
```

### Comparing `skytable_py-0.0.2/src/skytable_py/connection.py` & `skytable_py-0.1.0/src/skytable_py/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,69 @@
-import asyncio
-from asyncio import StreamReader, StreamWriter
-
+# Copyright 2024, Sayan Nandan <nandansayan@outlook.com>
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-class ClientException(Exception):
-    """
-    An exception thrown by this client library
-    """
-    pass
+from asyncio import StreamReader, StreamWriter
+from .query import Query
+from .protocol import Protocol
+from .response import Response
 
 
 class Connection:
     """
     A database connection to a Skytable instance
     """
 
     def __init__(self, reader: StreamReader, writer: StreamWriter) -> None:
         self._reader = reader
         self._writer = writer
+        self._protocol = Protocol()
 
     async def _write_all(self, bytes: bytes):
         self._write(bytes)
         await self._flush()
 
     def _write(self, bytes: bytes) -> None:
         self._writer.write(bytes)
 
+    def __buffer(self) -> bytes:
+        return self.buffer[:self._cursor]
+
     async def _flush(self):
         await self._writer.drain()
 
     async def _read_exact(self, count) -> bytes:
         return await self._reader.readexactly(count)
 
     async def close(self):
         """
         Close this connection
         """
         self._writer.close()
         await self._writer.wait_closed()
 
-
-class Config:
-    def __init__(self, username: str, password: str, host: str = "127.0.0.1", port: int = 2003) -> None:
-        self._username = username
-        self._password = password
-        self._host = host
-        self._port = port
-
-    def get_username(self) -> str:
-        return self._username
-
-    def get_password(self) -> str:
-        return self._password
-
-    def get_host(self) -> str:
-        return self._host
-
-    def get_port(self) -> int:
-        return self._port
-
-    def __hs(self) -> bytes:
-        return f"H\0\0\0\0\0{len(self.get_username())}\n{len(self.get_password())}\n{self.get_username()}{self.get_password()}".encode()
-
-    async def connect(self) -> Connection:
-        """
-        Establish a connection to the database instance using the set configuration.
-
-        ## Exceptions
-        Exceptions are raised in the following scenarios:
-        - If the server responds with a handshake error
-        - If the server sends an unknown handshake (usually caused by version incompatibility)
-        """
-        reader, writer = await asyncio.open_connection(self.get_host(), self.get_port())
-        con = Connection(reader, writer)
-        await con._write_all(self.__hs())
-        resp = await con._read_exact(4)
-        a, b, c, d = resp[0], resp[1], resp[2], resp[3]
-        if resp == b"H\0\0\0":
-            return con
-        elif a == ord(b'H') and b == 0 and c == 1:
-            raise ClientException(f"handshake error {d}")
-        else:
-            raise ClientException("unknown handshake")
+    async def run_simple_query(self, query: Query) -> Response:
+        query_window_str = str(query._q_window)
+        total_packet_size = len(query_window_str) + 1 + len(query._buffer)
+        # write metaframe
+        metaframe = f"S{str(total_packet_size)}\n{query_window_str}\n"
+        await self._write_all(metaframe.encode())
+        # write dataframe
+        await self._write_all(query._buffer)
+        # read response
+        while True:
+            new_block = await self._reader.read(1024)
+            self._protocol.push_additional_bytes(new_block)
+            resp = self._protocol.parse()
+            if resp:
+                return resp
```

### Comparing `skytable_py-0.0.2/LICENSE` & `skytable_py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytable_py-0.0.2/README.md` & `skytable_py-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `skytable_py-0.0.2/pyproject.toml` & `skytable_py-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skytable-py"
-version = "0.0.2"
+version = "0.1.0"
 authors = [{ name = "Sayan Nandan", email = "nandansayan@outlook.com" }]
 description = "Official Skytable client library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `skytable_py-0.0.2/PKG-INFO` & `skytable_py-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skytable-py
-Version: 0.0.2
+Version: 0.1.0
 Summary: Official Skytable client library for Python
 Project-URL: Homepage, https://github.com/skytable/skytable-py
 Project-URL: Issues, https://github.com/skytable/skytable-py/issues
 Author-email: Sayan Nandan <nandansayan@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

