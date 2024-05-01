# Comparing `tmp/melobot-2.6.4.tar.gz` & `tmp/melobot-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melobot-2.6.4.tar", last modified: Sun Apr 28 19:19:57 2024, max compression
+gzip compressed data, was "melobot-2.6.5.tar", last modified: Wed May  1 10:00:39 2024, max compression
```

## Comparing `melobot-2.6.4.tar` & `melobot-2.6.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1545 2024-04-17 07:58:06.600008 melobot-2.6.4/LICENSE-BSD
--rw-r--r--   0        0        0    20137 2024-04-17 10:10:23.406233 melobot-2.6.4/LICENSE-CC
--rw-r--r--   0        0        0     6410 2024-04-27 07:25:12.715861 melobot-2.6.4/README.md
--rw-r--r--   0        0        0     2651 2024-04-28 19:19:57.597497 melobot-2.6.4/pyproject.toml
--rw-r--r--   0        0        0      899 2024-04-23 10:40:08.419597 melobot-2.6.4/src/melobot/__init__.py
--rw-r--r--   0        0        0      400 2024-04-25 06:54:57.347251 melobot-2.6.4/src/melobot/base/__init__.py
--rw-r--r--   0        0        0    14351 2024-04-28 18:21:14.153110 melobot-2.6.4/src/melobot/base/abc.py
--rw-r--r--   0        0        0     1905 2024-04-28 14:19:04.061972 melobot-2.6.4/src/melobot/base/exceptions.py
--rw-r--r--   0        0        0     1695 2024-04-28 14:08:21.015679 melobot-2.6.4/src/melobot/base/ioc.py
--rw-r--r--   0        0        0    19367 2024-04-28 12:16:36.012674 melobot-2.6.4/src/melobot/base/tools.py
--rw-r--r--   0        0        0     4335 2024-04-28 09:08:39.804077 melobot-2.6.4/src/melobot/base/typing.py
--rw-r--r--   0        0        0      275 2024-04-20 16:29:46.707838 melobot-2.6.4/src/melobot/bot/__init__.py
--rw-r--r--   0        0        0     1855 2024-04-28 09:16:39.055982 melobot-2.6.4/src/melobot/bot/hook.py
--rw-r--r--   0        0        0    17322 2024-04-28 19:09:12.714557 melobot-2.6.4/src/melobot/bot/init.py
--rw-r--r--   0        0        0     1295 2024-04-26 09:48:10.186044 melobot-2.6.4/src/melobot/context/__init__.py
--rw-r--r--   0        0        0    57163 2024-04-28 11:01:20.922336 melobot-2.6.4/src/melobot/context/action.py
--rw-r--r--   0        0        0    24509 2024-04-28 12:11:14.151158 melobot-2.6.4/src/melobot/context/session.py
--rw-r--r--   0        0        0        0 2024-04-12 17:28:27.040296 melobot-2.6.4/src/melobot/controller/__init__.py
--rw-r--r--   0        0        0     3825 2024-04-28 14:28:49.091222 melobot-2.6.4/src/melobot/controller/dispatcher.py
--rw-r--r--   0        0        0     2593 2024-04-28 12:19:06.360136 melobot-2.6.4/src/melobot/controller/responder.py
--rw-r--r--   0        0        0      168 2024-04-13 14:35:10.206863 melobot-2.6.4/src/melobot/io/__init__.py
--rw-r--r--   0        0        0    11389 2024-04-28 19:12:50.816409 melobot-2.6.4/src/melobot/io/duplex_http.py
--rw-r--r--   0        0        0     9583 2024-04-28 19:13:37.642713 melobot-2.6.4/src/melobot/io/forward_ws.py
--rw-r--r--   0        0        0     8997 2024-04-28 19:13:30.049440 melobot-2.6.4/src/melobot/io/reverse_ws.py
--rw-r--r--   0        0        0     3391 2024-04-28 19:18:34.343495 melobot-2.6.4/src/melobot/meta.py
--rw-r--r--   0        0        0      567 2024-04-21 07:13:00.995861 melobot-2.6.4/src/melobot/models/__init__.py
--rw-r--r--   0        0        0    24306 2024-04-28 11:01:58.152610 melobot-2.6.4/src/melobot/models/event.py
--rw-r--r--   0        0        0    15488 2024-04-28 11:24:27.335986 melobot-2.6.4/src/melobot/models/msg.py
--rw-r--r--   0        0        0       81 2024-04-12 17:28:27.040296 melobot-2.6.4/src/melobot/plugin/__init__.py
--rw-r--r--   0        0        0    11809 2024-04-28 18:48:15.870905 melobot-2.6.4/src/melobot/plugin/handler.py
--rw-r--r--   0        0        0    38803 2024-04-28 11:31:26.871233 melobot-2.6.4/src/melobot/plugin/init.py
--rw-r--r--   0        0        0     5637 2024-04-28 11:44:35.493368 melobot-2.6.4/src/melobot/plugin/ipc.py
--rw-r--r--   0        0        0      831 2024-04-23 10:35:17.904031 melobot-2.6.4/src/melobot/utils/__init__.py
--rw-r--r--   0        0        0    12163 2024-04-28 11:48:44.035284 melobot-2.6.4/src/melobot/utils/checker.py
--rw-r--r--   0        0        0    10622 2024-04-28 11:53:13.540736 melobot-2.6.4/src/melobot/utils/logger.py
--rw-r--r--   0        0        0     4171 2024-04-20 15:28:42.348446 melobot-2.6.4/src/melobot/utils/matcher.py
--rw-r--r--   0        0        0    12753 2024-04-28 14:16:06.137565 melobot-2.6.4/src/melobot/utils/parser.py
--rw-r--r--   0        0        0        0 2024-04-26 13:26:23.449222 melobot-2.6.4/tests/__init__.py
--rw-r--r--   0        0        0     7932 1970-01-01 00:00:00.000000 melobot-2.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1545 2024-04-17 07:58:06.600008 melobot-2.6.5/LICENSE-BSD
+-rw-r--r--   0        0        0    20137 2024-04-17 10:10:23.406233 melobot-2.6.5/LICENSE-CC
+-rw-r--r--   0        0        0     6410 2024-04-27 07:25:12.715861 melobot-2.6.5/README.md
+-rw-r--r--   0        0        0     2651 2024-05-01 10:00:39.421814 melobot-2.6.5/pyproject.toml
+-rw-r--r--   0        0        0      899 2024-04-23 10:40:08.419597 melobot-2.6.5/src/melobot/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-25 06:54:57.347251 melobot-2.6.5/src/melobot/base/__init__.py
+-rw-r--r--   0        0        0    14351 2024-04-28 18:21:14.153110 melobot-2.6.5/src/melobot/base/abc.py
+-rw-r--r--   0        0        0     1905 2024-04-28 14:19:04.061972 melobot-2.6.5/src/melobot/base/exceptions.py
+-rw-r--r--   0        0        0     1695 2024-04-28 14:08:21.015679 melobot-2.6.5/src/melobot/base/ioc.py
+-rw-r--r--   0        0        0    19367 2024-04-28 12:16:36.012674 melobot-2.6.5/src/melobot/base/tools.py
+-rw-r--r--   0        0        0     4336 2024-05-01 09:13:32.123131 melobot-2.6.5/src/melobot/base/typing.py
+-rw-r--r--   0        0        0      275 2024-04-20 16:29:46.707838 melobot-2.6.5/src/melobot/bot/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-28 09:16:39.055982 melobot-2.6.5/src/melobot/bot/hook.py
+-rw-r--r--   0        0        0    17396 2024-04-29 08:12:45.172671 melobot-2.6.5/src/melobot/bot/init.py
+-rw-r--r--   0        0        0     1295 2024-04-26 09:48:10.186044 melobot-2.6.5/src/melobot/context/__init__.py
+-rw-r--r--   0        0        0    57163 2024-04-28 11:01:20.922336 melobot-2.6.5/src/melobot/context/action.py
+-rw-r--r--   0        0        0    24509 2024-04-28 12:11:14.151158 melobot-2.6.5/src/melobot/context/session.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:28:27.040296 melobot-2.6.5/src/melobot/controller/__init__.py
+-rw-r--r--   0        0        0     3825 2024-04-28 14:28:49.091222 melobot-2.6.5/src/melobot/controller/dispatcher.py
+-rw-r--r--   0        0        0     2593 2024-04-28 12:19:06.360136 melobot-2.6.5/src/melobot/controller/responder.py
+-rw-r--r--   0        0        0      168 2024-04-13 14:35:10.206863 melobot-2.6.5/src/melobot/io/__init__.py
+-rw-r--r--   0        0        0    11353 2024-04-29 07:44:55.379831 melobot-2.6.5/src/melobot/io/duplex_http.py
+-rw-r--r--   0        0        0     9704 2024-04-29 15:10:35.970263 melobot-2.6.5/src/melobot/io/forward_ws.py
+-rw-r--r--   0        0        0     8929 2024-04-29 15:10:40.843635 melobot-2.6.5/src/melobot/io/reverse_ws.py
+-rw-r--r--   0        0        0     3391 2024-05-01 09:59:49.951661 melobot-2.6.5/src/melobot/meta.py
+-rw-r--r--   0        0        0      567 2024-04-21 07:13:00.995861 melobot-2.6.5/src/melobot/models/__init__.py
+-rw-r--r--   0        0        0    24306 2024-04-28 11:01:58.152610 melobot-2.6.5/src/melobot/models/event.py
+-rw-r--r--   0        0        0    15488 2024-04-28 11:24:27.335986 melobot-2.6.5/src/melobot/models/msg.py
+-rw-r--r--   0        0        0       81 2024-04-12 17:28:27.040296 melobot-2.6.5/src/melobot/plugin/__init__.py
+-rw-r--r--   0        0        0    11839 2024-05-01 09:27:24.442756 melobot-2.6.5/src/melobot/plugin/handler.py
+-rw-r--r--   0        0        0    38803 2024-04-28 11:31:26.871233 melobot-2.6.5/src/melobot/plugin/init.py
+-rw-r--r--   0        0        0     5637 2024-04-28 11:44:35.493368 melobot-2.6.5/src/melobot/plugin/ipc.py
+-rw-r--r--   0        0        0      831 2024-04-23 10:35:17.904031 melobot-2.6.5/src/melobot/utils/__init__.py
+-rw-r--r--   0        0        0    12163 2024-04-28 11:48:44.035284 melobot-2.6.5/src/melobot/utils/checker.py
+-rw-r--r--   0        0        0    10634 2024-04-29 16:40:22.085816 melobot-2.6.5/src/melobot/utils/logger.py
+-rw-r--r--   0        0        0     4171 2024-04-20 15:28:42.348446 melobot-2.6.5/src/melobot/utils/matcher.py
+-rw-r--r--   0        0        0    12753 2024-04-28 14:16:06.137565 melobot-2.6.5/src/melobot/utils/parser.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:26:23.449222 melobot-2.6.5/tests/__init__.py
+-rw-r--r--   0        0        0     7932 1970-01-01 00:00:00.000000 melobot-2.6.5/PKG-INFO
```

### Comparing `melobot-2.6.4/LICENSE-BSD` & `melobot-2.6.5/LICENSE-BSD`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/LICENSE-CC` & `melobot-2.6.5/LICENSE-CC`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/README.md` & `melobot-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/pyproject.toml` & `melobot-2.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "2.6.4"
+version = "2.6.5"
 
 [project.license]
 text = "BSD"
 
 [project.urls]
 Homepage = "https://github.com/Meloland/melobot"
 Documentation = "https://docs.melobot.org"
```

### Comparing `melobot-2.6.4/src/melobot/__init__.py` & `melobot-2.6.5/src/melobot/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/base/abc.py` & `melobot-2.6.5/src/melobot/base/abc.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/base/exceptions.py` & `melobot-2.6.5/src/melobot/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/base/ioc.py` & `melobot-2.6.5/src/melobot/base/ioc.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/base/tools.py` & `melobot-2.6.5/src/melobot/base/tools.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/base/typing.py` & `melobot-2.6.5/src/melobot/base/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,9 +183,9 @@
             f"{func} 不是异步可调用对象（返回 Awaitable 的可调用对象）"
         )
 
     await_obj = func(*args, **kwargs)
     if inspect.isawaitable(await_obj):
         return await await_obj
     raise BotValidateError(
-        f"{func} 不是异步可调用对象（返回 Awaitable 的可调用对象），因为它的返回结果 {await_obj} 不可异步等待"
+        f"{func} 应该是异步函数，或其他异步可调用对象（返回 Awaitable 的可调用对象）。但它返回了：{await_obj}"
     )
```

### Comparing `melobot-2.6.4/src/melobot/bot/hook.py` & `melobot-2.6.5/src/melobot/bot/hook.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/bot/init.py` & `melobot-2.6.5/src/melobot/bot/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,19 +234,20 @@
 
                 life_tasks = [asyncio.create_task(self._life_ended.wait())]
                 if not self.connector.allow_reconn:
                     task = asyncio.create_task(self.connector._closed.wait())
                     life_tasks.append(task)
                 await asyncio.wait(life_tasks, return_when=asyncio.FIRST_COMPLETED)
 
-        except Exception as e:
-            self.logger.error("bot 核心无法继续运行")
-            self.logger.exc(locals=locals())
+        except BaseException as e:
+            self.logger.exc("bot 核心无法继续运行，原因：", e, locals=locals())
 
         finally:
+            if not self._life_ended.is_set():
+                self._life_ended.set()
             await self._bot_bus.emit(BotLife.BEFORE_STOP, wait=True)
             self.logger.debug("BEFORE_STOP hook 已完成")
             self.logger.info("bot 已清理运行时资源")
 
             BOT_LOCAL._del_ctx(bot_token)
             self.__run_flag__ = False
```

### Comparing `melobot-2.6.4/src/melobot/context/__init__.py` & `melobot-2.6.5/src/melobot/context/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/context/action.py` & `melobot-2.6.5/src/melobot/context/action.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/context/session.py` & `melobot-2.6.5/src/melobot/context/session.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/controller/dispatcher.py` & `melobot-2.6.5/src/melobot/controller/dispatcher.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/controller/responder.py` & `melobot-2.6.5/src/melobot/controller/responder.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/io/duplex_http.py` & `melobot-2.6.5/src/melobot/io/duplex_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
         if self.secret is not None:
             sign = hmac.new(self.secret.encode(), data, "sha1").hexdigest()
             recv_sign = request.headers["X-Signature"][len("sha1=") :]
 
             if sign != recv_sign:
                 self.logger.error("OneBot 实现程序鉴权不通过，本次上报数据将不会被处理")
-                self.logger.obj(data, "试图上报的数据：", level="ERROR")
+                self.logger.obj(data, "试图上报的数据", level="ERROR")
                 return
 
         self._pre_recv_time = time.time_ns()
         await self._ready_signal.wait()
 
         if not self._onebot_onlined.is_set():
             self._onebot_onlined.set()
@@ -240,16 +240,15 @@
                 self.logger.warning("OneBot 实现程序已掉线，正在等待它重新上线")
                 self._onebot_onlined.clear()
 
         except aiohttp.ContentTypeError:
             self.logger.error("连接器无法解析上报数据。可能是 access_token 未配置或错误")
 
         except Exception as e:
-            self.logger.error("bot 连接器发送任务抛出预期外的异常：")
-            self.logger.exc(locals=locals())
+            self.logger.exc("bot 连接器发送任务抛出预期外的异常", locals=locals())
 
     async def _watch_queue(self) -> None:
         """真正的发送方法。从 send_queue 提取 action 并按照一些处理步骤操作"""
         await self._ready_signal.wait()
 
         try:
             while True:
```

### Comparing `melobot-2.6.4/src/melobot/io/forward_ws.py` & `melobot-2.6.5/src/melobot/io/forward_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import time
 from itertools import count
 
 import websockets
 from websockets.exceptions import ConnectionClosed
 
 from ..base.abc import AbstractConnector, BotLife
-from ..base.exceptions import BotRuntimeError
-from ..base.typing import TYPE_CHECKING, Any, Optional, TracebackType, Type, Union, cast
+from ..base.typing import TYPE_CHECKING, Optional, TracebackType, Type, Union, cast
 from ..context.session import ActionResponse
 
 if TYPE_CHECKING:
     import websockets.client
 
     from ..base.abc import BotAction
     from ..models.event import MessageEvent, MetaEvent, NoticeEvent, RequestEvent
@@ -73,31 +72,40 @@
         if self.access_token is not None:
             headers = {"Authorization": f"Bearer {self.access_token}"}
 
         async with self._run_lock:
             self._closed.clear()
             ok_flag = False
             retry_iter = count(0) if self.max_retry < 0 else range(self.max_retry + 1)
+            first_try = True
 
             for _ in retry_iter:
+                if first_try:
+                    first_try = False
+                else:
+                    await asyncio.sleep(self.retry_delay)
+
                 try:
                     self.conn = await websockets.connect(self.url, extra_headers=headers)
                     ok_flag = True
                     break
 
                 except Exception as e:
                     self.logger.warning(
                         f"ws 连接建立失败，{self.retry_delay}s 后自动重试。错误：{e}"
                     )
                     if "403" in str(e):
                         self.logger.warning("403 错误可能是 access_token 未配置或无效")
-                    await asyncio.sleep(self.retry_delay)
 
             if not ok_flag:
-                raise BotRuntimeError("连接重试已达最大重试次数，已放弃建立连接")
+                self.logger.error("重试已达最大次数，已放弃建立连接")
+                self._close()
+                for task in asyncio.all_tasks():
+                    task.cancel()
+                return
 
             try:
                 self.logger.info("连接器与 OneBot 实现程序建立了 ws 连接")
                 self._conn_ready.set()
                 asyncio.create_task(self._listen())
                 await self._closed.wait()
             finally:
@@ -196,17 +204,14 @@
                     self.conn = cast(
                         "websockets.client.WebSocketClientProtocol", self.conn
                     )
                     raw = await self.conn.recv()
                     if self.logger._check_level("DEBUG"):
                         self.logger.obj(raw, "收到上报，未格式化的字符串")
 
-                    if raw == "":
-                        continue
-
                     event = self._event_builder.try_build(raw)
                     if event is None:
                         resp = ActionResponse(raw)
                         asyncio.create_task(self._resp_dispatcher.respond(resp))
                     else:
                         event = cast(
                             Union[
```

### Comparing `melobot-2.6.4/src/melobot/io/reverse_ws.py` & `melobot-2.6.5/src/melobot/io/reverse_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,14 @@
             while True:
                 try:
                     raw = await self._conn.recv()
 
                     if self.logger._check_level("DEBUG"):
                         self.logger.obj(raw, "收到上报，未格式化的字符串")
 
-                    if raw == "":
-                        continue
-
                     event = self._event_builder.try_build(raw)
                     if event is None:
                         resp = ActionResponse(raw)
                         asyncio.create_task(self._resp_dispatcher.respond(resp))
                     else:
                         event = cast(
                             Union[
```

### Comparing `melobot-2.6.4/src/melobot/meta.py` & `melobot-2.6.5/src/melobot/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         super(self.__class__, self).__setattr__(name, value)
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         setattr(self, "__setattr__", ReadOnly.__instance_setattr)
         return super().__call__(*args, **kwargs)
 
 
-__version__ = "2.6.4"
+__version__ = "2.6.5"
 
 
 class MetaInfo(metaclass=ReadOnly):
     """元信息类
 
     .. admonition:: 提示
        :class: tip
```

### Comparing `melobot-2.6.4/src/melobot/models/__init__.py` & `melobot-2.6.5/src/melobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/models/event.py` & `melobot-2.6.5/src/melobot/models/event.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/models/msg.py` & `melobot-2.6.5/src/melobot/models/msg.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/plugin/handler.py` & `melobot-2.6.5/src/melobot/plugin/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,16 @@
     ) -> tuple[bool, "BotSession"]:
         event = cast(MessageEvent, event)
         session = BotSessionManager.make_temp(event)
 
         if self.matcher is not None:
             _match = self.matcher.match(event.text)
             status = await self._run_on_ctx(_match, session)
-            return status, session
+            if not status:
+                return False, session
 
         if self.parser is not None:
             _parse = self.parser.parse(event.text)
             args = await self._run_on_ctx(_parse, session)
             if args is None:
                 return False, session
             else:
```

### Comparing `melobot-2.6.4/src/melobot/plugin/init.py` & `melobot-2.6.5/src/melobot/plugin/init.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/plugin/ipc.py` & `melobot-2.6.5/src/melobot/plugin/ipc.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/utils/__init__.py` & `melobot-2.6.5/src/melobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/utils/checker.py` & `melobot-2.6.5/src/melobot/utils/checker.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/utils/logger.py` & `melobot-2.6.5/src/melobot/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     return colored_str, _CONSOLE.export_text()
 
 
 _EXC_FORMATTER = ExceptionFormatter(colored=True)
 _NO_COLOR_EXC_FORMATTER = ExceptionFormatter(colored=False)
 
 
-def _get_fmtted_exc(e: Exception) -> str:
+def _get_fmtted_exc(e: BaseException) -> str:
     """返回生成更好的异常字符串"""
     return "".join(
         _NO_COLOR_EXC_FORMATTER.format_exception(e.__class__, e, e.__traceback__)
     )
 
 
 class ObjectFilter(logging.Filter):
@@ -257,30 +257,30 @@
     ) -> bool:
         """检查日志器是否可以输出指定日志等级的日志"""
         return BotLogger.LEVEL_MAP[level] >= self.__LEVEL_FLAG__
 
     def exc(
         self,
         prefix: str = "出现异常：",
-        e: Optional[Exception] = None,
+        e: Optional[BaseException] = None,
         locals: Optional[dict[str, Any]] = None,
     ) -> None:
         """更好的用于记录异常的方法
 
         :param prefix: 记录时的前缀信息
         :param e: 异常对象
         :param locals: 需要记录的局部变量，为空则不记录
         """
         _exc = sys.exc_info()[1] if e is None else e
         exc_str = f"[{_exc.__class__.__qualname__}] {str(_exc)}"
 
         if hasattr(self, "exception"):
             self.exception(f"{prefix}{exc_str}")
         else:
-            fmt_exc = _get_fmtted_exc(cast(Exception, _exc))
+            fmt_exc = _get_fmtted_exc(cast(BaseException, _exc))
             self.error(f"{prefix}{exc_str}\n{fmt_exc}")
 
         if locals is not None:
             self.obj(locals, "异常抛出点局部变量", level="ERROR")
 
     def obj(
         self,
```

### Comparing `melobot-2.6.4/src/melobot/utils/matcher.py` & `melobot-2.6.5/src/melobot/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/src/melobot/utils/parser.py` & `melobot-2.6.5/src/melobot/utils/parser.py`

 * *Files identical despite different names*

### Comparing `melobot-2.6.4/PKG-INFO` & `melobot-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melobot
-Version: 2.6.4
+Version: 2.6.5
 Summary: A bot framework with session control and plugin-supported.
 Keywords: qq,qq bot,onebot,bot framework,asyncio,coroutine,concurrency
 Author-Email: aicorein <melodyecho@glowmem.com>
 Maintainer-Email: aicorein <melodyecho@glowmem.com>
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: melobot Version: 2.6.4 Summary: A bot framework
+Metadata-Version: 2.1 Name: melobot Version: 2.6.5 Summary: A bot framework
 with session control and plugin-supported. Keywords: qq,qq bot,onebot,bot
 framework,asyncio,coroutine,concurrency Author-Email: aicorein
 glowmem.com> Maintainer-Email: aicorein
 glowmem.com> License: BSD Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

