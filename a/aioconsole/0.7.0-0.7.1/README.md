# Comparing `tmp/aioconsole-0.7.0.tar.gz` & `tmp/aioconsole-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioconsole-0.7.0.tar", last modified: Sat Dec  9 17:38:33 2023, max compression
+gzip compressed data, was "aioconsole-0.7.1.tar", last modified: Wed May  1 15:37:59 2024, max compression
```

## Comparing `aioconsole-0.7.0.tar` & `aioconsole-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:38:33.176160 aioconsole-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-12-09 17:38:32.000000 aioconsole-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-12-09 17:38:33.176160 aioconsole-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2023-12-09 17:38:32.000000 aioconsole-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:38:33.176160 aioconsole-0.7.0/aioconsole/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/apython.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/rlwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2023-12-09 17:38:32.000000 aioconsole-0.7.0/aioconsole/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:38:33.176160 aioconsole-0.7.0/aioconsole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-12-09 17:38:33.000000 aioconsole-0.7.0/aioconsole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-09 17:38:33.000000 aioconsole-0.7.0/aioconsole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:38:33.000000 aioconsole-0.7.0/aioconsole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-09 17:38:33.000000 aioconsole-0.7.0/aioconsole.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-09 17:38:33.000000 aioconsole-0.7.0/aioconsole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-09 17:38:33.176160 aioconsole-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-12-09 17:38:32.000000 aioconsole-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:59.700665 aioconsole-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-01 15:37:58.000000 aioconsole-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-01 15:37:59.700665 aioconsole-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-01 15:37:58.000000 aioconsole-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:59.696665 aioconsole-0.7.1/aioconsole/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/apython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/rlwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-01 15:37:58.000000 aioconsole-0.7.1/aioconsole/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:37:59.700665 aioconsole-0.7.1/aioconsole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-01 15:37:59.000000 aioconsole-0.7.1/aioconsole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-01 15:37:59.000000 aioconsole-0.7.1/aioconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:37:59.000000 aioconsole-0.7.1/aioconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 15:37:59.000000 aioconsole-0.7.1/aioconsole.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 15:37:59.000000 aioconsole-0.7.1/aioconsole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-01 15:37:59.700665 aioconsole-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-01 15:37:58.000000 aioconsole-0.7.1/setup.py
```

### Comparing `aioconsole-0.7.0/LICENSE` & `aioconsole-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/PKG-INFO` & `aioconsole-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioconsole
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous console and interfaces for asyncio
 Home-page: https://github.com/vxgmichel/aioconsole
 Download-URL: https://pypi.org/project/aioconsole/
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
@@ -17,33 +17,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 
 aioconsole
 ==========
 
-.. image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
-   :target: http://aioconsole.readthedocs.io/
-   :alt:
+|docs-badge| |cov-badge| |ci-badge| |version-badge| |pyversion-badge|
 
-.. image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
-   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amaster
-   :alt:
-
-.. image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/vxgmichel/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/v/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
 
 Asynchronous console and interfaces for asyncio
 
 aioconsole_ provides:
 
 * asynchronous equivalents to `input`_, `print`_, `exec`_ and `code.interact`_
 * an interactive loop running the asynchronous python console
@@ -61,15 +44,15 @@
 Installation
 ------------
 
 aioconsole_ is available on PyPI_ and GitHub_.
 Both of the following commands install the ``aioconsole`` package
 and the ``apython`` script.
 
-.. sourcecode:: console
+.. code:: console
 
     $ pip3 install aioconsole   # from PyPI
     $ python3 setup.py install  # or from the sources
     $ apython -h
     usage: apython [-h] [--serve [HOST:] PORT] [--no-readline]
                    [--banner BANNER] [--locals LOCALS]
                    [-m MODULE | FILE] ...
@@ -94,27 +77,27 @@
 
 
 Simple usage
 ------------
 
 The following example demonstrates the use of ``await`` inside the console:
 
-.. sourcecode:: console
+.. code:: console
 
     $ apython
     Python 3.5.0 (default, Sep 7 2015, 14:12:03)
     [GCC 4.8.4] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     ---
     This console is running in an asyncio event loop.
     It allows you to wait for coroutines using the 'await' syntax.
     Try: await asyncio.sleep(1, result=3, loop=loop)
     ---
 
-.. sourcecode:: python3
+.. code:: python3
 
     >>> await asyncio.sleep(1, result=3)
     # Wait one second...
     3
     >>>
 
 
@@ -142,12 +125,32 @@
 .. _GitHub: https://github.com/vxgmichel/aioconsole
 .. _input: https://docs.python.org/3/library/functions.html#input
 .. _print: https://docs.python.org/3/library/functions.html#print
 .. _exec: https://docs.python.org/3/library/functions.html#exec
 .. _code.interact: https://docs.python.org/3/library/code.html#code.interact
 .. _argparse: https://docs.python.org/dev/library/argparse.html
 .. _stream: https://docs.python.org/3/library/asyncio-stream.html
-.. _example directory: https://github.com/vxgmichel/aioconsole/blob/master/example
+.. _example directory: https://github.com/vxgmichel/aioconsole/blob/main/example
 .. _documentation: http://aioconsole.readthedocs.io/
 .. _PyPI: aioconsole_
 .. _IPython: https://ipython.readthedocs.io
 .. _ptpython: https://github.com/prompt-toolkit/ptpython
+
+.. |docs-badge| image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
+   :target: http://aioconsole.readthedocs.io/
+   :alt:
+
+.. |ci-badge| image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
+   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amain
+   :alt:
+
+.. |cov-badge| image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/vxgmichel/aioconsole
+   :alt:
+
+.. |version-badge| image:: https://img.shields.io/pypi/v/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
+
+.. |pyversion-badge| image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
```

### Comparing `aioconsole-0.7.0/README.rst` & `aioconsole-0.7.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,12 @@
 aioconsole
 ==========
 
-.. image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
-   :target: http://aioconsole.readthedocs.io/
-   :alt:
+|docs-badge| |cov-badge| |ci-badge| |version-badge| |pyversion-badge|
 
-.. image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
-   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amaster
-   :alt:
-
-.. image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/vxgmichel/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/v/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
 
 Asynchronous console and interfaces for asyncio
 
 aioconsole_ provides:
 
 * asynchronous equivalents to `input`_, `print`_, `exec`_ and `code.interact`_
 * an interactive loop running the asynchronous python console
@@ -41,15 +24,15 @@
 Installation
 ------------
 
 aioconsole_ is available on PyPI_ and GitHub_.
 Both of the following commands install the ``aioconsole`` package
 and the ``apython`` script.
 
-.. sourcecode:: console
+.. code:: console
 
     $ pip3 install aioconsole   # from PyPI
     $ python3 setup.py install  # or from the sources
     $ apython -h
     usage: apython [-h] [--serve [HOST:] PORT] [--no-readline]
                    [--banner BANNER] [--locals LOCALS]
                    [-m MODULE | FILE] ...
@@ -74,27 +57,27 @@
 
 
 Simple usage
 ------------
 
 The following example demonstrates the use of ``await`` inside the console:
 
-.. sourcecode:: console
+.. code:: console
 
     $ apython
     Python 3.5.0 (default, Sep 7 2015, 14:12:03)
     [GCC 4.8.4] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     ---
     This console is running in an asyncio event loop.
     It allows you to wait for coroutines using the 'await' syntax.
     Try: await asyncio.sleep(1, result=3, loop=loop)
     ---
 
-.. sourcecode:: python3
+.. code:: python3
 
     >>> await asyncio.sleep(1, result=3)
     # Wait one second...
     3
     >>>
 
 
@@ -122,12 +105,32 @@
 .. _GitHub: https://github.com/vxgmichel/aioconsole
 .. _input: https://docs.python.org/3/library/functions.html#input
 .. _print: https://docs.python.org/3/library/functions.html#print
 .. _exec: https://docs.python.org/3/library/functions.html#exec
 .. _code.interact: https://docs.python.org/3/library/code.html#code.interact
 .. _argparse: https://docs.python.org/dev/library/argparse.html
 .. _stream: https://docs.python.org/3/library/asyncio-stream.html
-.. _example directory: https://github.com/vxgmichel/aioconsole/blob/master/example
+.. _example directory: https://github.com/vxgmichel/aioconsole/blob/main/example
 .. _documentation: http://aioconsole.readthedocs.io/
 .. _PyPI: aioconsole_
 .. _IPython: https://ipython.readthedocs.io
 .. _ptpython: https://github.com/prompt-toolkit/ptpython
+
+.. |docs-badge| image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
+   :target: http://aioconsole.readthedocs.io/
+   :alt:
+
+.. |ci-badge| image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
+   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amain
+   :alt:
+
+.. |cov-badge| image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/vxgmichel/aioconsole
+   :alt:
+
+.. |version-badge| image:: https://img.shields.io/pypi/v/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
+
+.. |pyversion-badge| image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
```

### Comparing `aioconsole-0.7.0/aioconsole/__init__.py` & `aioconsole-0.7.1/aioconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/apython.py` & `aioconsole-0.7.1/aioconsole/apython.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/command.py` & `aioconsole-0.7.1/aioconsole/command.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/console.py` & `aioconsole-0.7.1/aioconsole/console.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/events.py` & `aioconsole-0.7.1/aioconsole/events.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/execute.py` & `aioconsole-0.7.1/aioconsole/execute.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/rlwrap.py` & `aioconsole-0.7.1/aioconsole/rlwrap.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/server.py` & `aioconsole-0.7.1/aioconsole/server.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.7.0/aioconsole/stream.py` & `aioconsole-0.7.1/aioconsole/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 from collections import deque
 from threading import Thread
 from concurrent.futures import Future
 
 from . import compat
 
 
+class ProtectedPipe:
+    """Wrapper to protect a pipe from being closed."""
+
+    def __init__(self, pipe):
+        self.pipe = pipe
+
+    def fileno(self):
+        return self.pipe.fileno()
+
+    def close(self):
+        pass
+
+
 def is_pipe_transport_compatible(pipe):
     if compat.platform == "win32":
         return False
     try:
         fileno = pipe.fileno()
     except (OSError, AttributeError):
         return False
@@ -61,25 +74,14 @@
     Thread(target=daemon, daemon=True).start()
     try:
         return await asyncio.wrap_future(future)
     except BaseExceptionWrapper as exc:
         raise exc.args[0]
 
 
-def protect_standard_streams(stream):
-    if stream._transport is None:
-        return
-    try:
-        fileno = stream._transport.get_extra_info("pipe").fileno()
-    except (ValueError, OSError):
-        return
-    if fileno < 3:
-        stream._transport._pipe = None
-
-
 class StandardStreamReaderProtocol(asyncio.StreamReaderProtocol):
     def connection_made(self, transport):
         # The connection is already made
         if self._stream_reader._transport is not None:
             return
         # Make the connection
         super().connection_made(transport)
@@ -90,16 +92,14 @@
         # Call the parent
         super().connection_lost(exc)
         # Restore the inner state
         self.__dict__.update(state)
 
 
 class StandardStreamReader(asyncio.StreamReader):
-    __del__ = protect_standard_streams
-
     async def readuntil(self, separator=b"\n"):
         # Re-implement `readuntil` to work around self._limit.
         # The limit is still useful to prevent the internal buffer
         # from growing too large when it's not necessary, but it
         # needs to be disabled when the user code is purposely
         # reading from stdin.
         while True:
@@ -111,15 +111,26 @@
                     del self._buffer[: e.consumed + len(separator)]
                     self._maybe_resume_transport()
                     return bytes(chunk)
                 await self._wait_for_data("readuntil")
 
 
 class StandardStreamWriter(asyncio.StreamWriter):
-    __del__ = protect_standard_streams
+    def __del__(self):
+        # No `__del__` method for StreamWriter in Python 3.10 and before
+        try:
+            parent_del = super().__del__
+        except AttributeError:
+            return
+        # Do not attempt to close the transport if the loop is closed
+        try:
+            asyncio.get_running_loop()
+        except RuntimeError:
+            return
+        parent_del()
 
     def write(self, data):
         if isinstance(data, str):
             data = data.encode()
         super().write(data)
 
 
@@ -220,24 +231,26 @@
 async def open_standard_pipe_connection(pipe_in, pipe_out, pipe_err, *, loop=None):
     if loop is None:
         loop = asyncio.get_event_loop()
 
     # Reader
     in_reader = StandardStreamReader(loop=loop)
     protocol = StandardStreamReaderProtocol(in_reader, loop=loop)
-    await loop.connect_read_pipe(lambda: protocol, pipe_in)
+    await loop.connect_read_pipe(lambda: protocol, ProtectedPipe(pipe_in))
 
     # Out writer
-    out_write_connect = loop.connect_write_pipe(lambda: protocol, pipe_out)
-    out_transport, _ = await out_write_connect
+    out_transport, _ = await loop.connect_write_pipe(
+        lambda: protocol, ProtectedPipe(pipe_out)
+    )
     out_writer = StandardStreamWriter(out_transport, protocol, in_reader, loop)
 
     # Err writer
-    err_write_connect = loop.connect_write_pipe(lambda: protocol, pipe_err)
-    err_transport, _ = await err_write_connect
+    err_transport, _ = await loop.connect_write_pipe(
+        lambda: protocol, ProtectedPipe(pipe_err)
+    )
     err_writer = StandardStreamWriter(err_transport, protocol, in_reader, loop)
 
     # Set the write buffer limits to zero
     # This way, `await stream.drain()` can be used to make sure the buffer is flushed
     out_transport.set_write_buffer_limits(high=0, low=0)
     err_transport.set_write_buffer_limits(high=0, low=0)
```

### Comparing `aioconsole-0.7.0/aioconsole.egg-info/PKG-INFO` & `aioconsole-0.7.1/aioconsole.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioconsole
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous console and interfaces for asyncio
 Home-page: https://github.com/vxgmichel/aioconsole
 Download-URL: https://pypi.org/project/aioconsole/
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
@@ -17,33 +17,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 
 aioconsole
 ==========
 
-.. image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
-   :target: http://aioconsole.readthedocs.io/
-   :alt:
+|docs-badge| |cov-badge| |ci-badge| |version-badge| |pyversion-badge|
 
-.. image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
-   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amaster
-   :alt:
-
-.. image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/vxgmichel/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/v/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
-
-.. image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
-   :target: https://pypi.python.org/pypi/aioconsole
-   :alt:
 
 Asynchronous console and interfaces for asyncio
 
 aioconsole_ provides:
 
 * asynchronous equivalents to `input`_, `print`_, `exec`_ and `code.interact`_
 * an interactive loop running the asynchronous python console
@@ -61,15 +44,15 @@
 Installation
 ------------
 
 aioconsole_ is available on PyPI_ and GitHub_.
 Both of the following commands install the ``aioconsole`` package
 and the ``apython`` script.
 
-.. sourcecode:: console
+.. code:: console
 
     $ pip3 install aioconsole   # from PyPI
     $ python3 setup.py install  # or from the sources
     $ apython -h
     usage: apython [-h] [--serve [HOST:] PORT] [--no-readline]
                    [--banner BANNER] [--locals LOCALS]
                    [-m MODULE | FILE] ...
@@ -94,27 +77,27 @@
 
 
 Simple usage
 ------------
 
 The following example demonstrates the use of ``await`` inside the console:
 
-.. sourcecode:: console
+.. code:: console
 
     $ apython
     Python 3.5.0 (default, Sep 7 2015, 14:12:03)
     [GCC 4.8.4] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     ---
     This console is running in an asyncio event loop.
     It allows you to wait for coroutines using the 'await' syntax.
     Try: await asyncio.sleep(1, result=3, loop=loop)
     ---
 
-.. sourcecode:: python3
+.. code:: python3
 
     >>> await asyncio.sleep(1, result=3)
     # Wait one second...
     3
     >>>
 
 
@@ -142,12 +125,32 @@
 .. _GitHub: https://github.com/vxgmichel/aioconsole
 .. _input: https://docs.python.org/3/library/functions.html#input
 .. _print: https://docs.python.org/3/library/functions.html#print
 .. _exec: https://docs.python.org/3/library/functions.html#exec
 .. _code.interact: https://docs.python.org/3/library/code.html#code.interact
 .. _argparse: https://docs.python.org/dev/library/argparse.html
 .. _stream: https://docs.python.org/3/library/asyncio-stream.html
-.. _example directory: https://github.com/vxgmichel/aioconsole/blob/master/example
+.. _example directory: https://github.com/vxgmichel/aioconsole/blob/main/example
 .. _documentation: http://aioconsole.readthedocs.io/
 .. _PyPI: aioconsole_
 .. _IPython: https://ipython.readthedocs.io
 .. _ptpython: https://github.com/prompt-toolkit/ptpython
+
+.. |docs-badge| image:: https://readthedocs.org/projects/aioconsole/badge/?version=latest
+   :target: http://aioconsole.readthedocs.io/
+   :alt:
+
+.. |ci-badge| image:: https://github.com/vxgmichel/aioconsole/workflows/CI/badge.svg
+   :target: https://github.com/vxgmichel/aioconsole/actions?query=branch%3Amain
+   :alt:
+
+.. |cov-badge| image:: https://codecov.io/gh/vxgmichel/aioconsole/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/vxgmichel/aioconsole
+   :alt:
+
+.. |version-badge| image:: https://img.shields.io/pypi/v/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
+
+.. |pyversion-badge| image:: https://img.shields.io/pypi/pyversions/aioconsole.svg
+   :target: https://pypi.python.org/pypi/aioconsole
+   :alt:
```

### Comparing `aioconsole-0.7.0/setup.py` & `aioconsole-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 Programming Language :: Python :: 3.11
 Programming Language :: Python :: 3.12
 Programming Language :: Python :: 3 :: Only
 """.splitlines()
 
 setup(
     name="aioconsole",
-    version="0.7.0",
+    version="0.7.1",
     packages=["aioconsole"],
     entry_points={"console_scripts": ["apython = aioconsole:run_apython"]},
     setup_requires=["pytest-runner" if TESTING else ""],
     tests_require=[
         "pytest",
         "pytest-asyncio",
         "pytest-cov",
         "pytest-repeat",
+        'uvloop; python_implementation != "PyPy" and sys_platform != "win32"',
     ],
     license="GPLv3",
     python_requires=">=3.8",
     classifiers=CLASSIFIERS,
     description="Asynchronous console and interfaces for asyncio",
     long_description=README,
     author="Vincent Michel",
```

