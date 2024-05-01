# Comparing `tmp/arclet_entari-0.3.1.tar.gz` & `tmp/arclet_entari-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_entari-0.3.1.tar", last modified: Tue Apr 30 10:19:47 2024, max compression
+gzip compressed data, was "arclet_entari-0.3.2.tar", last modified: Wed May  1 13:07:27 2024, max compression
```

## Comparing `arclet_entari-0.3.1.tar` & `arclet_entari-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/LICENSE
--rw-r--r--   0        0        0      880 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/README.md
--rw-r--r--   0        0        0     2029 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/__init__.py
--rw-r--r--   0        0        0      110 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/__init__.py
--rw-r--r--   0        0        0      480 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/argv.py
--rw-r--r--   0        0        0     8556 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/main.py
--rw-r--r--   0        0        0     1142 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/model.py
--rw-r--r--   0        0        0      787 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/plugin.py
--rw-r--r--   0        0        0     5569 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/command/provider.py
--rw-r--r--   0        0        0     3442 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/core.py
--rw-r--r--   0        0        0     9705 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/event.py
--rw-r--r--   0        0        0     9783 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/message.py
--rw-r--r--   0        0        0     3295 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/plugin.py
--rw-r--r--   0        0        0    10061 2024-04-30 10:19:25.520823 arclet_entari-0.3.1/arclet/entari/session.py
--rw-r--r--   0        0        0     1821 2024-04-30 10:19:47.920649 arclet_entari-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 arclet_entari-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/LICENSE
+-rw-r--r--   0        0        0      880 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/README.md
+-rw-r--r--   0        0        0     2147 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/argv.py
+-rw-r--r--   0        0        0     8556 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/main.py
+-rw-r--r--   0        0        0     1142 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/model.py
+-rw-r--r--   0        0        0      787 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/plugin.py
+-rw-r--r--   0        0        0     5569 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/command/provider.py
+-rw-r--r--   0        0        0     3442 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/core.py
+-rw-r--r--   0        0        0    10124 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/event.py
+-rw-r--r--   0        0        0      950 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/filter.py
+-rw-r--r--   0        0        0     9684 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/message.py
+-rw-r--r--   0        0        0     3295 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/plugin.py
+-rw-r--r--   0        0        0    10061 2024-05-01 13:07:00.141449 arclet_entari-0.3.2/arclet/entari/session.py
+-rw-r--r--   0        0        0     1821 2024-05-01 13:07:27.481691 arclet_entari-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 arclet_entari-0.3.2/PKG-INFO
```

### Comparing `arclet_entari-0.3.1/LICENSE` & `arclet_entari-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/README.md` & `arclet_entari-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/__init__.py` & `arclet_entari-0.3.2/arclet/entari/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,12 +39,14 @@
 from satori.config import WebsocketsInfo as WebsocketsInfo
 
 from .command import AlconnaDispatcher as AlconnaDispatcher
 from .command import EntariCommands as EntariCommands
 from .core import Entari as Entari
 from .event import MessageCreatedEvent as MessageCreatedEvent
 from .event import MessageEvent as MessageEvent
+from .filter import is_direct_message as is_direct_message
+from .filter import is_public_message as is_public_message
 from .message import MessageChain as MessageChain
 from .plugin import Plugin as Plugin
 from .plugin import load_plugin as load_plugin
 from .plugin import load_plugins as load_plugins
 from .session import ContextSession as ContextSession
```

### Comparing `arclet_entari-0.3.1/arclet/entari/command/main.py` & `arclet_entari-0.3.2/arclet/entari/command/main.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/command/model.py` & `arclet_entari-0.3.2/arclet/entari/command/model.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/command/plugin.py` & `arclet_entari-0.3.2/arclet/entari/command/plugin.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/command/provider.py` & `arclet_entari-0.3.2/arclet/entari/command/provider.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/core.py` & `arclet_entari-0.3.2/arclet/entari/core.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/event.py` & `arclet_entari-0.3.2/arclet/entari/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         fs = fields(cls)
         attrs = {"account": account}
         for fd in fs:
             if not fd.init:
                 continue
             if attr := getattr(origin, fd.name, None):
                 attrs[fd.name] = attr
-        res = cls(**attrs)
+        res = cls(**attrs)  # type: ignore
         res._origin = origin
         return res
 
     async def gather(self, context: Contexts):
         context["$account"] = self.account
         context["$origin_event"] = self._origin
 
@@ -52,30 +52,40 @@
     class OperatorProvider(Provider[User]):
         priority = 10
 
         def validate(self, param: Param):
             return param.name == "operator" and super().validate(param)
 
         async def __call__(self, context: Contexts):
+            if "operator" in context:
+                return context["operator"]
             return context["$origin_event"].operator
 
     class UserProvider(Provider[User]):
         async def __call__(self, context: Contexts):
+            if "user" in context:
+                return context["user"]
             return context["$origin_event"].user
 
     class MessageProvider(Provider[MessageObject]):
         async def __call__(self, context: Contexts):
+            if "$message_origin" in context:
+                return context["$message_origin"]
             return context["$origin_event"].message
 
     class ChannelProvider(Provider[Channel]):
         async def __call__(self, context: Contexts):
+            if "channel" in context:
+                return context["channel"]
             return context["$origin_event"].channel
 
     class GuildProvider(Provider[Guild]):
         async def __call__(self, context: Contexts):
+            if "guild" in context:
+                return context["guild"]
             return context["$origin_event"].guild
 
 
 class NoticeEvent(Event):
     pass
```

### Comparing `arclet_entari-0.3.1/arclet/entari/message.py` & `arclet_entari-0.3.2/arclet/entari/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 TE = TypeVar("TE", bound=Element)
 TE1 = TypeVar("TE1", bound=Element)
 
 
 class MessageChain(list[TE]):
     """消息序列
 
-    参数:
+    Args:
         message: 消息内容
     """
 
     def __init__(
         self: MessageChain[Element],
         message: Iterable[str | TE] | str | TE | None = None,
     ):
@@ -97,62 +97,62 @@
             raise TypeError(f"Unsupported type {type(other)!r}")
         return self
 
     @overload
     def __getitem__(self, args: type[TE1]) -> MessageChain[TE1]:
         """获取仅包含指定消息段类型的消息
 
-        参数:
+        Args:
             args: 消息段类型
 
-        返回:
+        Return:
             所有类型为 `args` 的消息段
         """
 
     @overload
     def __getitem__(self, args: tuple[type[TE1], int]) -> TE1:
         """索引指定类型的消息段
 
-        参数:
+        Args:
             args: 消息段类型和索引
 
-        返回:
+        Return:
             类型为 `args[0]` 的消息段第 `args[1]` 个
         """
 
     @overload
     def __getitem__(self, args: tuple[type[TE1], slice]) -> MessageChain[TE1]:
         """切片指定类型的消息段
 
-        参数:
+        Args:
             args: 消息段类型和切片
 
-        返回:
+        Return:
             类型为 `args[0]` 的消息段切片 `args[1]`
         """
 
     @overload
     def __getitem__(self, args: int) -> TE:
         """索引消息段
 
-        参数:
+        Args:
             args: 索引
 
-        返回:
+        Return:
             第 `args` 个消息段
         """
 
     @overload
     def __getitem__(self, args: slice) -> Self:
         """切片消息段
 
-        参数:
+        Args:
             args: 切片
 
-        返回:
+        Return:
             消息切片 `args`
         """
 
     def __getitem__(
         self,
         args: type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice,
     ) -> TE | TE1 | MessageChain[TE1] | Self:
@@ -170,59 +170,58 @@
         if issubclass(arg1, Element) and isinstance(arg2, slice):
             return MessageChain([seg for seg in self if isinstance(seg, arg1)][arg2])
         raise ValueError("Incorrect arguments to slice")  # pragma: no cover
 
     def __contains__(self, value: str | Element | type[Element]) -> bool:
         """检查消息段是否存在
 
-        参数:
+        Args:
             value: 消息段或消息段类型
-        返回:
+        Return:
             消息内是否存在给定消息段或给定类型的消息段
         """
         if isinstance(value, type):
             return bool(next((seg for seg in self if isinstance(seg, value)), None))
         if isinstance(value, str):
             value = Text(value)
         return super().__contains__(value)
 
     def has(self, value: str | Element | type[Element]) -> bool:
-        """与 {ref}``__contains__` <nonebot.adapters.Message.__contains__>` 相同"""
         return value in self
 
     def index(self, value: str | Element | type[Element], *args: SupportsIndex) -> int:
         """索引消息段
 
-        参数:
+        Args:
             value: 消息段或者消息段类型
-            arg: start 与 end
+            args: start 与 end
 
-        返回:
+        Return:
             索引 index
 
-        异常:
+        Raise:
             ValueError: 消息段不存在
         """
         if isinstance(value, type):
             first_segment = next((seg for seg in self if isinstance(seg, value)), None)
             if first_segment is None:
                 raise ValueError(f"Element with type {value!r} is not in message")
             return super().index(first_segment, *args)
         if isinstance(value, str):
             value = Text(value)
         return super().index(value, *args)  # type: ignore
 
     def get(self, type_: type[TE], count: int | None = None) -> MessageChain[TE]:
         """获取指定类型的消息段
 
-        参数:
+        Args:
             type_: 消息段类型
             count: 获取个数
 
-        返回:
+        Return:
             构建的新消息
         """
         if count is None:
             return self[type_]
 
         iterator, filtered = (seg for seg in self if isinstance(seg, type_)), MessageChain()
         for _ in range(count):
@@ -231,50 +230,50 @@
                 break
             filtered.append(seg)
         return filtered
 
     def count(self, value: type[Element] | str | Element) -> int:
         """计算指定消息段的个数
 
-        参数:
+        Args:
             value: 消息段或消息段类型
 
-        返回:
+        Return:
             个数
         """
         if isinstance(value, str):
             value = Text(value)
         return (
             len(self[value])  # type: ignore
             if isinstance(value, type)
             else super().count(value)  # type: ignore
         )
 
     def only(self, value: type[Element] | str | Element) -> bool:
         """检查消息中是否仅包含指定消息段
 
-        参数:
+        Args:
             value: 指定消息段或消息段类型
 
-        返回:
+        Return:
             是否仅包含指定消息段
         """
         if isinstance(value, type):
             return all(isinstance(seg, value) for seg in self)
         if isinstance(value, str):
             value = Text(value)
         return all(seg == value for seg in self)
 
     def join(self, iterable: Iterable[TE1 | MessageChain[TE1]]) -> MessageChain[TE | TE1]:
         """将多个消息连接并将自身作为分割
 
-        参数:
+        Args:
             iterable: 要连接的消息
 
-        返回:
+        Return:
             连接后的消息
         """
         ret = MessageChain()
         for index, msg in enumerate(iterable):
             if index != 0:
                 ret.extend(self)
             if isinstance(msg, Element):
@@ -283,32 +282,32 @@
                 ret.extend(msg.copy())
         return ret
 
     def copy(self) -> MessageChain[TE]:
         """深拷贝消息"""
         return deepcopy(self)
 
-    def include(self, *types: type[Element]) -> Self:
+    def include(self, *types: type[Element]) -> MessageChain:
         """过滤消息
 
-        参数:
+        Args:
             types: 包含的消息段类型
 
-        返回:
+        Return:
             新构造的消息
         """
         return MessageChain(seg for seg in self if seg.__class__ in types)
 
-    def exclude(self, *types: type[Element]) -> Self:
+    def exclude(self, *types: type[Element]) -> MessageChain:
         """过滤消息
 
-        参数:
+        Args:
             types: 不包含的消息段类型
 
-        返回:
+        Return:
             新构造的消息
         """
         return MessageChain(seg for seg in self if seg.__class__ not in types)
 
     def extract_plain_text(self) -> str:
         """提取消息内纯文本消息"""
```

### Comparing `arclet_entari-0.3.1/arclet/entari/plugin.py` & `arclet_entari-0.3.2/arclet/entari/plugin.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/arclet/entari/session.py` & `arclet_entari-0.3.2/arclet/entari/session.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.1/pyproject.toml` & `arclet_entari-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-entari"
-version = "0.3.1"
+version = "0.3.2"
 description = "Simple IM Framework based on satori-python"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "arclet-letoderea>=0.9.2",
     "arclet-alconna>=1.8.11",
```

### Comparing `arclet_entari-0.3.1/PKG-INFO` & `arclet_entari-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-entari
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simple IM Framework based on satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

