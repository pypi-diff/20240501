# Comparing `tmp/jupyter_server_ydoc-1.0.0a0.tar.gz` & `tmp/jupyter_server_ydoc-1.0.0a1.tar.gz`

## Comparing `jupyter_server_ydoc-1.0.0a0.tar` & `jupyter_server_ydoc-1.0.0a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/setup.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter-config/jupyter_server_ydoc.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/_version.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/app.py
--rw-r--r--   0        0        0    15708 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/handlers.py
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/loaders.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/rooms.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/stores.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/utils.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/websocketserver.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/awareness.yaml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/session.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/__init__.py
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/conftest.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_app.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_documents.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_handlers.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_loaders.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_rooms.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/utils.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/LICENSE
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/README.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/setup.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter-config/jupyter_server_ydoc.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/_version.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/app.py
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/handlers.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/loaders.py
+-rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/rooms.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/stores.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/utils.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/websocketserver.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/awareness.yaml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/session.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/__init__.py
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/conftest.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_app.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_documents.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_handlers.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_loaders.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_rooms.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/README.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/PKG-INFO
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/app.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .stores import SQLiteYStore
 from .utils import (
     AWARENESS_EVENTS_SCHEMA_PATH,
     EVENTS_SCHEMA_PATH,
     encode_file_path,
     room_id_from_encoded_path,
 )
-from .websocketserver import JupyterWebsocketServer, RoomNotFound
+from .websocketserver import JupyterWebsocketServer, RoomNotFound, exception_logger
 
 
 class YDocExtension(ExtensionApp):
     name = "jupyter_server_ydoc"
     app_name = "Collaboration"
     description = """
     Enables Real Time Collaboration in JupyterLab
@@ -103,14 +103,17 @@
         for k, v in self.config.get(self.ystore_class.__name__, {}).items():
             setattr(self.ystore_class, k, v)
 
         self.ywebsocket_server = JupyterWebsocketServer(
             rooms_ready=False,
             auto_clean_rooms=False,
             ystore_class=self.ystore_class,
+            # Log exceptions, because we don't want the websocket server
+            # to _ever_ crash permanently in a live jupyter_server.
+            exception_handler=exception_logger,
             log=self.log,
         )
 
         # self.settings is local to the ExtensionApp but here we need
         # the global app settings in which the file id manager will register
         # itself maybe at a later time.
         self.file_loaders = FileLoaderMapping(
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/handlers.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 from __future__ import annotations
 
 import asyncio
 import json
 import time
 import uuid
+from logging import Logger
 from typing import Any
 
 from jupyter_server.auth import authorized
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
+from jupyter_server.utils import ensure_async
 from jupyter_ydoc import ydocs as YDOCS
 from pycrdt_websocket.websocket_server import YRoom
 from pycrdt_websocket.ystore import BaseYStore
 from pycrdt_websocket.yutils import YMessageType, write_var_uint
 from tornado import web
 from tornado.websocket import WebSocketHandler
 
@@ -66,25 +68,41 @@
 
     def create_task(self, aw):
         task = asyncio.create_task(aw)
         self._background_tasks.add(task)
         task.add_done_callback(self._background_tasks.discard)
 
     async def prepare(self):
+        await ensure_async(super().prepare())
         if not self._websocket_server.started.is_set():
             self.create_task(self._websocket_server.start())
             await self._websocket_server.started.wait()
 
         # Get room
         self._room_id: str = room_id_from_encoded_path(self.request.path)
 
         async with self._room_lock(self._room_id):
             if self._websocket_server.room_exists(self._room_id):
                 self.room: YRoom = await self._websocket_server.get_room(self._room_id)
             else:
+                # Logging exceptions, instead of raising them here to ensure
+                # that the y-rooms stay alive even after an exception is seen.
+                def exception_logger(exception: Exception, log: Logger) -> bool:
+                    """A function that catches any exceptions raised in the websocket
+                    server and logs them.
+
+                    The protects the y-room's task group from cancelling
+                    anytime an exception is raised.
+                    """
+                    log.error(
+                        f"Document Room Exception, (room_id={self._room_id or 'unknown'}): ",
+                        exc_info=exception,
+                    )
+                    return True
+
                 if self._room_id.count(":") >= 2:
                     # DocumentRoom
                     file_format, file_type, file_id = decode_file_path(self._room_id)
                     if file_id in self._file_loaders:
                         self._emit(
                             LogLevel.WARNING,
                             None,
@@ -98,28 +116,47 @@
                         self._room_id,
                         file_format,
                         file_type,
                         file,
                         self.event_logger,
                         ystore,
                         self.log,
-                        self._document_save_delay,
+                        exception_handler=exception_logger,
+                        save_delay=self._document_save_delay,
                     )
 
                 else:
                     # TransientRoom
                     # it is a transient document (e.g. awareness)
-                    self.room = TransientRoom(self._room_id, self.log)
+                    self.room = TransientRoom(
+                        self._room_id,
+                        log=self.log,
+                        exception_handler=exception_logger,
+                    )
 
-            await self._websocket_server.start_room(self.room)
-            self._websocket_server.add_room(self._room_id, self.room)
+            try:
+                await self._websocket_server.start_room(self.room)
+            except Exception as e:
+                self.log.error("Room %s failed to start on websocket server", self._room_id)
+                # Clean room
+                await self.room.stop()
+                self.log.info("Room %s deleted", self._room_id)
+                self._emit(LogLevel.INFO, "clean", "Room deleted.")
 
-        res = super().prepare()
-        if res is not None:
-            return await res
+                # Clean the file loader in file loader mapping if there are not any rooms using it
+                _, _, file_id = decode_file_path(self._room_id)
+                file = self._file_loaders[file_id]
+                if file.number_of_subscriptions == 0 or (
+                    file.number_of_subscriptions == 1 and self._room_id in file._subscriptions
+                ):
+                    self.log.info("Deleting file %s", file.path)
+                    await self._file_loaders.remove(file_id)
+                    self._emit(LogLevel.INFO, "clean", "file loader removed.")
+                raise e
+            self._websocket_server.add_room(self._room_id, self.room)
 
     def initialize(
         self,
         ywebsocket_server: JupyterWebsocketServer,
         file_loaders: FileLoaderMapping,
         ystore_class: type[BaseYStore],
         document_cleanup_delay: float | None = 60.0,
@@ -130,14 +167,16 @@
         self._file_id_manager = self.settings["file_id_manager"]
         self._file_loaders = file_loaders
         self._ystore_class = ystore_class
         self._cleanup_delay = document_cleanup_delay
         self._document_save_delay = document_save_delay
         self._websocket_server = ywebsocket_server
         self._message_queue = asyncio.Queue()
+        self._room_id = ""
+        self.room = None
 
     @property
     def path(self):
         """
         Returns the room id. It needs to be called 'path' for compatibility with
         the WebsocketServer (websocket.path).
         """
@@ -201,15 +240,16 @@
                 # Close websocket and propagate error.
                 if isinstance(e, web.HTTPError):
                     self.log.error(f"File {file.path} not found.\n{e!r}", exc_info=e)
                     self.close(1004, f"File {file.path} not found.")
                 else:
                     self.log.error(f"Error initializing: {file.path}\n{e!r}", exc_info=e)
                     self.close(
-                        1003, f"Error initializing: {file.path}. You need to close the document."
+                        1003,
+                        f"Error initializing: {file.path}. You need to close the document.",
                     )
 
                 # Clean up the room and delete the file loader
                 if len(self.room.clients) == 0 or self.room.clients == [self]:
                     self._message_queue.put_nowait(b"")
                     self._cleanup_delay = 0
                     await self._clean_room()
@@ -223,15 +263,15 @@
         """
         Send a message to the client.
         """
         # needed to be compatible with WebsocketServer (websocket.send)
         try:
             self.write_message(message, binary=True)
         except Exception as e:
-            self.log.debug("Failed to write message", exc_info=e)
+            self.log.error("Failed to write message", exc_info=e)
 
     async def recv(self):
         """
         Receive a message from the client.
         """
         message = await self._message_queue.get()
         return message
@@ -268,15 +308,19 @@
                 return skip
 
         if message_type == MessageType.CHAT:
             msg = message[2:].decode("utf-8")
 
             user = self.current_user
             data = json.dumps(
-                {"sender": user.username, "timestamp": time.time(), "content": json.loads(msg)}
+                {
+                    "sender": user.username,
+                    "timestamp": time.time(),
+                    "content": json.loads(msg),
+                }
             ).encode("utf8")
 
             for client in self.room.clients:
                 if client != self:
                     task = asyncio.create_task(
                         client.send(bytes([MessageType.CHAT]) + write_var_uint(len(data)) + data)
                     )
@@ -337,15 +381,15 @@
             return
 
         await asyncio.sleep(self._cleanup_delay)
 
         async with self._room_lock(self._room_id):
             # Remove the room from the websocket server
             self.log.info("Deleting Y document from memory: %s", self._room_id)
-            self._websocket_server.delete_room(room=self.room)
+            await self._websocket_server.delete_room(room=self.room)
 
             # Clean room
             del self.room
             self.log.info("Room %s deleted", self._room_id)
             self._emit(LogLevel.INFO, "clean", "Room deleted.")
 
             # Clean the file loader if there are not rooms using it
@@ -383,25 +427,35 @@
         file_id_manager = self.settings["file_id_manager"]
 
         idx = file_id_manager.get_id(path)
         if idx is not None:
             # index already exists
             self.log.info("Request for Y document '%s' with room ID: %s", path, idx)
             data = json.dumps(
-                {"format": format, "type": content_type, "fileId": idx, "sessionId": SERVER_SESSION}
+                {
+                    "format": format,
+                    "type": content_type,
+                    "fileId": idx,
+                    "sessionId": SERVER_SESSION,
+                }
             )
             self.set_status(200)
             return self.finish(data)
 
         # try indexing
         idx = file_id_manager.index(path)
         if idx is None:
             # file does not exists
             raise web.HTTPError(404, f"File {path!r} does not exist")
 
         # index successfully created
         self.log.info("Request for Y document '%s' with room ID: %s", path, idx)
         data = json.dumps(
-            {"format": format, "type": content_type, "fileId": idx, "sessionId": SERVER_SESSION}
+            {
+                "format": format,
+                "type": content_type,
+                "fileId": idx,
+                "sessionId": SERVER_SESSION,
+            }
         )
         self.set_status(201)
         return self.finish(data)
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/loaders.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,18 @@
         Clean up the file.
 
         Stops the watch task.
         """
         if self._watcher is not None:
             if not self._watcher.cancelled():
                 self._watcher.cancel()
-            await self._watcher
+            try:
+                await self._watcher
+            except asyncio.CancelledError:
+                self._log.info(f"file watcher for '{self.file_id}' is cancelled now")
 
     def observe(self, id: str, callback: Callable[[], Coroutine[Any, Any, None]]) -> None:
         """
         Subscribe to the file to get notified about out-of-band file changes.
 
             Parameters:
                     id (str): Room ID
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/rooms.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/rooms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 from __future__ import annotations
 
 import asyncio
 from logging import Logger
-from typing import Any
+from typing import Any, Callable
 
 from jupyter_events import EventLogger
 from jupyter_ydoc import ydocs as YDOCS
 from pycrdt_websocket.websocket_server import YRoom
 from pycrdt_websocket.ystore import BaseYStore, YDocNotFound
 
 from .loaders import FileLoader
@@ -27,16 +27,17 @@
         file_format: str,
         file_type: str,
         file: FileLoader,
         logger: EventLogger,
         ystore: BaseYStore | None,
         log: Logger | None,
         save_delay: float | None = None,
+        exception_handler: Callable[[Exception, Logger], bool] | None = None,
     ):
-        super().__init__(ready=False, ystore=ystore, log=log)
+        super().__init__(ready=False, ystore=ystore, exception_handler=exception_handler, log=log)
 
         self._room_id: str = room_id
         self._file_format: str = file_format
         self._file_type: str = file_type
         self._file: FileLoader = file
         self._document = YDOCS.get(self._file_type, YFILE)(self.ydoc)
 
@@ -119,27 +120,31 @@
                     pass
 
             if not read_from_source:
                 # if YStore updates and source file are out-of-sync, resync updates with source
                 if self._document.source != model["content"]:
                     # TODO: Delete document from the store.
                     self._emit(
-                        LogLevel.INFO, "initialize", "The file is out-of-sync with the ystore."
+                        LogLevel.INFO,
+                        "initialize",
+                        "The file is out-of-sync with the ystore.",
                     )
                     self.log.info(
                         "Content in file %s is out-of-sync with the ystore %s",
                         self._file.path,
                         self.ystore.__class__.__name__,
                     )
                     read_from_source = True
 
             if read_from_source:
                 self._emit(LogLevel.INFO, "load", "Content loaded from disk.")
                 self.log.info(
-                    "Content in room %s loaded from file %s", self._room_id, self._file.path
+                    "Content in room %s loaded from file %s",
+                    self._room_id,
+                    self._file.path,
                 )
                 self._document.source = model["content"]
 
                 if self.ystore:
                     await self.ystore.encode_state_as_update(self.ydoc)
 
             self._document.dirty = False
@@ -151,21 +156,24 @@
         if action:
             data["action"] = action
         if msg:
             data["msg"] = msg
 
         self._logger.emit(schema_id=JUPYTER_COLLABORATION_EVENTS_URI, data=data)
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """
         Stop the room.
 
         Cancels the save task and unsubscribes from the file.
         """
-        super().stop()
+        try:
+            await super().stop()
+        except RuntimeError:
+            pass
         # TODO: Should we cancel or wait ?
         if self._saving_document:
             self._saving_document.cancel()
 
         self._document.unobserve()
         self._file.unobserve(self.room_id)
 
@@ -277,16 +285,21 @@
             self.log.error(msg, exc_info=e)
             self._emit(LogLevel.ERROR, None, msg)
 
 
 class TransientRoom(YRoom):
     """A Y room for sharing state (e.g. awareness)."""
 
-    def __init__(self, room_id: str, log: Logger | None):
-        super().__init__(log=log)
+    def __init__(
+        self,
+        room_id: str,
+        log: Logger | None = None,
+        exception_handler: Callable[[Exception, Logger], bool] | None = None,
+    ):
+        super().__init__(log=log, exception_handler=exception_handler)
 
         self._room_id = room_id
 
     @property
     def room_id(self) -> str:
         """
         The room ID.
@@ -295,7 +308,16 @@
 
     async def _broadcast_updates(self):
         # FIXME should be upstreamed
         try:
             await super()._broadcast_updates()
         except asyncio.CancelledError:
             pass
+
+    async def stop(self) -> None:
+        """
+        Stop the room.
+        """
+        try:
+            await super().stop()
+        except RuntimeError:
+            pass
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/stores.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/stores.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/utils.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/websocketserver.py` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/websocketserver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 from __future__ import annotations
 
 import asyncio
 from logging import Logger
-from typing import Any
+from typing import Any, Callable
 
 from pycrdt_websocket.websocket_server import WebsocketServer, YRoom
 from pycrdt_websocket.ystore import BaseYStore
 from tornado.websocket import WebSocketHandler
 
 
 class RoomNotFound(LookupError):
     pass
 
 
+def exception_logger(exception: Exception, log: Logger) -> bool:
+    """A function that catches any exceptions raised in the websocket
+    server and logs them.
+
+    This protects the websocket server's task group from cancelling
+    anytime an exception is raised.
+    """
+    log.error("Jupyter Websocket Server: ", exc_info=exception)
+    return True
+
+
 class JupyterWebsocketServer(WebsocketServer):
     """Ypy websocket server.
 
     It communicates the document updates to all clients for each room.
     """
 
     ypatch_nb: int
     connected_user: dict[int, str]
 
     def __init__(
         self,
         ystore_class: BaseYStore,
         rooms_ready: bool = True,
         auto_clean_rooms: bool = True,
+        exception_handler: Callable[[Exception, Logger], bool] | None = None,
         log: Logger | None = None,
     ):
-        super().__init__(rooms_ready, auto_clean_rooms, log)
+        super().__init__(
+            rooms_ready=rooms_ready,
+            auto_clean_rooms=auto_clean_rooms,
+            exception_handler=exception_handler,
+            log=log,
+        )
         self.ystore_class = ystore_class
         self.ypatch_nb = 0
         self.connected_users: dict[Any, Any] = {}
         # Async loop is not yet ready at the object instantiation
         self.monitor_task: asyncio.Task | None = None
 
     async def clean(self):
@@ -54,15 +71,15 @@
         # if room_tasks:
         #     _, pending = await asyncio.wait(room_tasks, timeout=3)
         #     if pending:
         #         msg = f"{len(pending)} room task(s) are pending."
         #         self.log.warning(msg)
         #         self.log.debug("Pending tasks: %r", pending)
 
-        self.stop()
+        await self.stop()
         tasks = []
         if self.monitor_task is not None:
             self.monitor_task.cancel()
             tasks.append(self.monitor_task)
 
         if tasks:
             _, pending = await asyncio.wait(tasks, timeout=3)
```

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/awareness.yaml` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/awareness.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/session.yaml` & `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/session.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/conftest.py` & `jupyter_server_ydoc-1.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/test_app.py` & `jupyter_server_ydoc-1.0.0a1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/test_documents.py` & `jupyter_server_ydoc-1.0.0a1/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/test_loaders.py` & `jupyter_server_ydoc-1.0.0a1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/test_rooms.py` & `jupyter_server_ydoc-1.0.0a1/tests/test_rooms.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/tests/utils.py` & `jupyter_server_ydoc-1.0.0a1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/.gitignore` & `jupyter_server_ydoc-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/LICENSE` & `jupyter_server_ydoc-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a0/pyproject.toml` & `jupyter_server_ydoc-1.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 authors = [
     { name = "Jupyter Development Team", email = "jupyter@googlegroups.com" },
 ]
 dependencies = [
     "jupyter_server>=2.4.0,<3.0.0",
     "jupyter_ydoc>=2.0.0,<3.0.0",
-    "pycrdt-websocket>=0.12.5,<0.13.0",
+    "pycrdt-websocket>=0.13.1,<0.14.0",
     "jupyter_events>=0.10.0",
     "jupyter_server_fileid>=0.7.0,<1",
     "jsonschema>=4.18.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

### Comparing `jupyter_server_ydoc-1.0.0a0/PKG-INFO` & `jupyter_server_ydoc-1.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-server-ydoc
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: jupyter-server extension integrating collaborative shared models.
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
         (also known as New or Revised or 3-Clause BSD), as follows:
         
@@ -76,15 +76,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: jsonschema>=4.18.0
 Requires-Dist: jupyter-events>=0.10.0
 Requires-Dist: jupyter-server-fileid<1,>=0.7.0
 Requires-Dist: jupyter-server<3.0.0,>=2.4.0
 Requires-Dist: jupyter-ydoc<3.0.0,>=2.0.0
-Requires-Dist: pycrdt-websocket<0.13.0,>=0.12.5
+Requires-Dist: pycrdt-websocket<0.14.0,>=0.13.1
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: importlib-metadata>=4.8.3; (python_version < '3.10') and extra == 'test'
 Requires-Dist: jupyter-server-fileid[test]; extra == 'test'
 Requires-Dist: jupyter-server[test]>=2.4.0; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
```

