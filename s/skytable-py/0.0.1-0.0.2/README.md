# Comparing `tmp/skytable_py-0.0.1.tar.gz` & `tmp/skytable_py-0.0.2.tar.gz`

## Comparing `skytable_py-0.0.1.tar` & `skytable_py-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 skytable_py-0.0.1/src/skytable_py/__init__.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 skytable_py-0.0.1/src/skytable_py/connection.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 skytable_py-0.0.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.0.1/LICENSE
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 skytable_py-0.0.1/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 skytable_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 skytable_py-0.0.2/run_tests.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 skytable_py-0.0.2/src/skytable_py/__init__.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 skytable_py-0.0.2/src/skytable_py/connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skytable_py-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 skytable_py-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 skytable_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.0.2/LICENSE
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 skytable_py-0.0.2/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 skytable_py-0.0.2/PKG-INFO
```

### Comparing `skytable_py-0.0.1/src/skytable_py/connection.py` & `skytable_py-0.0.2/src/skytable_py/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     """
     An exception thrown by this client library
     """
     pass
 
 
 class Connection:
+    """
+    A database connection to a Skytable instance
+    """
+
     def __init__(self, reader: StreamReader, writer: StreamWriter) -> None:
         self._reader = reader
         self._writer = writer
 
     async def _write_all(self, bytes: bytes):
         self._write(bytes)
         await self._flush()
@@ -24,14 +28,17 @@
     async def _flush(self):
         await self._writer.drain()
 
     async def _read_exact(self, count) -> bytes:
         return await self._reader.readexactly(count)
 
     async def close(self):
+        """
+        Close this connection
+        """
         self._writer.close()
         await self._writer.wait_closed()
 
 
 class Config:
     def __init__(self, username: str, password: str, host: str = "127.0.0.1", port: int = 2003) -> None:
         self._username = username
@@ -52,30 +59,25 @@
         return self._port
 
     def __hs(self) -> bytes:
         return f"H\0\0\0\0\0{len(self.get_username())}\n{len(self.get_password())}\n{self.get_username()}{self.get_password()}".encode()
 
     async def connect(self) -> Connection:
         """
-        Establish a connection to the database instance using the set configuration
+        Establish a connection to the database instance using the set configuration.
+
+        ## Exceptions
+        Exceptions are raised in the following scenarios:
+        - If the server responds with a handshake error
+        - If the server sends an unknown handshake (usually caused by version incompatibility)
         """
         reader, writer = await asyncio.open_connection(self.get_host(), self.get_port())
         con = Connection(reader, writer)
         await con._write_all(self.__hs())
         resp = await con._read_exact(4)
         a, b, c, d = resp[0], resp[1], resp[2], resp[3]
         if resp == b"H\0\0\0":
             return con
         elif a == ord(b'H') and b == 0 and c == 1:
             raise ClientException(f"handshake error {d}")
         else:
             raise ClientException("unknown handshake")
-
-
-async def main():
-    cfg = Config("root", "Ai5WVhl03zPigkrN")
-    print("establishing...")
-    connection = await cfg.connect()
-    print("connected")
-
-if __name__ == "__main__":
-    asyncio.run(main())
```

### Comparing `skytable_py-0.0.1/LICENSE` & `skytable_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skytable_py-0.0.1/pyproject.toml` & `skytable_py-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skytable-py"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Sayan Nandan", email = "nandansayan@outlook.com" }]
 description = "Official Skytable client library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `skytable_py-0.0.1/PKG-INFO` & `skytable_py-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skytable-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Official Skytable client library for Python
 Project-URL: Homepage, https://github.com/skytable/skytable-py
 Project-URL: Issues, https://github.com/skytable/skytable-py/issues
 Author-email: Sayan Nandan <nandansayan@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,20 +13,41 @@
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Skytable Python Client
 
+> **Note**: This library is currently in alpha
+
 This is an alpha version of Skytable's official connector for Python 3.X.
 
+
 ## Example
 
+Install the dependency:
+
+```sh
+pip install skytable-py
+```
+
+Use in your code:
 ```python
 import asyncio
-from skytable import Config
+from skytable_py import Config
 
 c = Config(username="root", password="password")
-db = await c.connect()
 
-# ... use the db
+
+async def main():
+    db = await c.connect()
+    # ... use the db
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+
 ```
+
+## License
+
+This client library is distributed under the [Apache-2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
```

