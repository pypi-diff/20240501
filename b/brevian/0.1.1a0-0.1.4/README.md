# Comparing `tmp/brevian-0.1.1a0.tar.gz` & `tmp/brevian-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevian-0.1.1a0.tar", max compression
+gzip compressed data, was "brevian-0.1.4.tar", max compression
```

## Comparing `brevian-0.1.1a0.tar` & `brevian-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,38 @@
--rw-r--r--   0        0        0     1065 2024-02-29 21:41:22.134348 brevian-0.1.1a0/LICENSE
--rw-r--r--   0        0        0      267 2024-02-29 21:52:31.053644 brevian-0.1.1a0/README.md
--rw-r--r--   0        0        0     1668 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/__init__.py
--rw-r--r--   0        0        0     6107 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/client.py
--rw-r--r--   0        0        0      519 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/api_error.py
--rw-r--r--   0        0        0     1273 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      299 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/errors/__init__.py
--rw-r--r--   0        0        0      300 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/errors/forbidden_error.py
--rw-r--r--   0        0        0      321 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/errors/internal_server_error.py
--rw-r--r--   0        0        0      326 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/errors/too_many_requests_error.py
--rw-r--r--   0        0        0     2315 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/__init__.py
--rw-r--r--   0        0        0     1067 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_request.py
--rw-r--r--   0        0        0      994 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_request_messages_item.py
--rw-r--r--   0        0        0      510 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_request_messages_item_role.py
--rw-r--r--   0        0        0     1205 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_response.py
--rw-r--r--   0        0        0     1027 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_response_choices_item.py
--rw-r--r--   0        0        0     1023 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_response_choices_item_message.py
--rw-r--r--   0        0        0      531 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_response_choices_item_message_role.py
--rw-r--r--   0        0        0     1098 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/chat_response_usage.py
--rw-r--r--   0        0        0      956 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/choice.py
--rw-r--r--   0        0        0      952 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/choice_message.py
--rw-r--r--   0        0        0      480 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/choice_message_role.py
--rw-r--r--   0        0        0      935 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/error_response.py
--rw-r--r--   0        0        0      940 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/forbidden_error_body.py
--rw-r--r--   0        0        0      945 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/internal_server_error_body.py
--rw-r--r--   0        0        0      927 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/message.py
--rw-r--r--   0        0        0      462 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/message_role.py
--rw-r--r--   0        0        0      474 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/message_role_enum.py
--rw-r--r--   0        0        0     1011 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_request_messages_item.py
--rw-r--r--   0        0        0      522 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_request_messages_item_role.py
--rw-r--r--   0        0        0     1235 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_response.py
--rw-r--r--   0        0        0     1044 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_response_choices_item.py
--rw-r--r--   0        0        0     1040 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_response_choices_item_message.py
--rw-r--r--   0        0        0      543 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_response_choices_item_message_role.py
--rw-r--r--   0        0        0     1102 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/post_chat_response_usage.py
--rw-r--r--   0        0        0      946 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0     1086 2024-03-01 02:48:02.000000 brevian-0.1.1a0/brevian/types/usage.py
--rw-r--r--   0        0        0      785 2024-02-29 21:58:01.959769 brevian-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 brevian-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-29 21:41:22.134348 brevian-0.1.4/LICENSE
+-rw-r--r--   0        0        0      267 2024-02-29 21:52:31.053644 brevian-0.1.4/README.md
+-rw-r--r--   0        0        0     1290 2024-04-30 22:51:54.390773 brevian-0.1.4/brevian/__init__.py
+-rw-r--r--   0        0        0     9782 2024-04-30 22:51:50.207197 brevian-0.1.4/brevian/client.py
+-rw-r--r--   0        0        0      519 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/api_error.py
+-rw-r--r--   0        0        0     1273 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      425 2024-04-30 22:51:50.207505 brevian-0.1.4/brevian/errors/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-30 22:51:50.207634 brevian-0.1.4/brevian/errors/bad_request_error.py
+-rw-r--r--   0        0        0      300 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/errors/forbidden_error.py
+-rw-r--r--   0        0        0      321 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/errors/internal_server_error.py
+-rw-r--r--   0        0        0      283 2024-04-30 22:51:50.207787 brevian-0.1.4/brevian/errors/not_found_error.py
+-rw-r--r--   0        0        0      326 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0     1595 2024-04-30 22:51:54.391219 brevian-0.1.4/brevian/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/chat_request.py
+-rw-r--r--   0        0        0      956 2024-04-30 22:51:54.391569 brevian-0.1.4/brevian/types/chat_request_messages_item.py
+-rw-r--r--   0        0        0      956 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/choice.py
+-rw-r--r--   0        0        0      946 2024-04-30 22:51:54.391956 brevian-0.1.4/brevian/types/choice_message.py
+-rw-r--r--   0        0        0      935 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/error_response.py
+-rw-r--r--   0        0        0      940 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/forbidden_error_body.py
+-rw-r--r--   0        0        0      945 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/internal_server_error_body.py
+-rw-r--r--   0        0        0      940 2024-04-30 22:51:54.392368 brevian-0.1.4/brevian/types/message.py
+-rw-r--r--   0        0        0      474 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/message_role_enum.py
+-rw-r--r--   0        0        0     1011 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/post_chat_request_messages_item.py
+-rw-r--r--   0        0        0      522 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/post_chat_request_messages_item_role.py
+-rw-r--r--   0        0        0     1148 2024-04-30 22:51:54.392693 brevian-0.1.4/brevian/types/post_chat_response.py
+-rw-r--r--   0        0        0     1044 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/post_chat_response_choices_item.py
+-rw-r--r--   0        0        0      967 2024-04-30 22:51:54.393052 brevian-0.1.4/brevian/types/post_chat_response_choices_item_message.py
+-rw-r--r--   0        0        0      936 2024-04-30 22:51:54.393359 brevian-0.1.4/brevian/types/post_chat_response_usage.py
+-rw-r--r--   0        0        0     1162 2024-04-30 22:51:50.208145 brevian-0.1.4/brevian/types/sub_query_metadata.py
+-rw-r--r--   0        0        0      946 2024-05-01 02:38:46.000000 brevian-0.1.4/brevian/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0     1135 2024-04-30 22:51:50.208279 brevian-0.1.4/brevian/types/unified_citation.py
+-rw-r--r--   0        0        0      920 2024-04-30 22:51:54.393668 brevian-0.1.4/brevian/types/usage.py
+-rw-r--r--   0        0        0      784 2024-04-30 22:52:06.762150 brevian-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brevian-0.1.4/PKG-INFO
```

### Comparing `brevian-0.1.1a0/LICENSE` & `brevian-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/core/__init__.py` & `brevian-0.1.4/brevian/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/core/client_wrapper.py` & `brevian-0.1.4/brevian/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/core/datetime_utils.py` & `brevian-0.1.4/brevian/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/core/jsonable_encoder.py` & `brevian-0.1.4/brevian/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/types/chat_request.py` & `brevian-0.1.4/brevian/types/chat_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ChatRequest(pydantic.BaseModel):
     messages: typing.List[ChatRequestMessagesItem]
-    agent_id: str = pydantic.Field(alias="agentId")
+    agent_id: typing.Optional[str] = pydantic.Field(alias="agentId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_request_messages_item.py` & `brevian-0.1.4/brevian/types/chat_request_messages_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_request_messages_item_role import ChatRequestMessagesItemRole
+from .message_role_enum import MessageRoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ChatRequestMessagesItem(pydantic.BaseModel):
-    role: ChatRequestMessagesItemRole
+    role: MessageRoleEnum
     content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_response.py` & `brevian-0.1.4/brevian/types/post_chat_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_response_choices_item import ChatResponseChoicesItem
-from .chat_response_usage import ChatResponseUsage
+from .post_chat_response_choices_item import PostChatResponseChoicesItem
+from .post_chat_response_usage import PostChatResponseUsage
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatResponse(pydantic.BaseModel):
+class PostChatResponse(pydantic.BaseModel):
     id: str
-    conversation_id: str = pydantic.Field(alias="conversationId")
+    conversation_id: str
     created: str
     model: str
-    choices: typing.List[ChatResponseChoicesItem]
-    usage: ChatResponseUsage
+    choices: typing.List[PostChatResponseChoicesItem]
+    usage: PostChatResponseUsage
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_response_choices_item.py` & `brevian-0.1.4/brevian/types/post_chat_response_choices_item_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_response_choices_item_message import ChatResponseChoicesItemMessage
+from .message_role_enum import MessageRoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatResponseChoicesItem(pydantic.BaseModel):
-    index: int
-    finish_reason: str
-    message: ChatResponseChoicesItemMessage
+class PostChatResponseChoicesItemMessage(pydantic.BaseModel):
+    role: MessageRoleEnum
+    content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_response_choices_item_message.py` & `brevian-0.1.4/brevian/types/choice_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_response_choices_item_message_role import ChatResponseChoicesItemMessageRole
+from .message_role_enum import MessageRoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatResponseChoicesItemMessage(pydantic.BaseModel):
-    role: ChatResponseChoicesItemMessageRole
+class ChoiceMessage(pydantic.BaseModel):
+    role: MessageRoleEnum
     content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_response_choices_item_message_role.py` & `brevian-0.1.4/brevian/types/post_chat_request_messages_item_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class ChatResponseChoicesItemMessageRole(str, enum.Enum):
+class PostChatRequestMessagesItemRole(str, enum.Enum):
     USER = "user"
     ASSISTANT = "assistant"
 
     def visit(self, user: typing.Callable[[], T_Result], assistant: typing.Callable[[], T_Result]) -> T_Result:
-        if self is ChatResponseChoicesItemMessageRole.USER:
+        if self is PostChatRequestMessagesItemRole.USER:
             return user()
-        if self is ChatResponseChoicesItemMessageRole.ASSISTANT:
+        if self is PostChatRequestMessagesItemRole.ASSISTANT:
             return assistant()
```

### Comparing `brevian-0.1.1a0/brevian/types/chat_response_usage.py` & `brevian-0.1.4/brevian/types/error_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatResponseUsage(pydantic.BaseModel):
-    prompt_tokens: int = pydantic.Field(alias="promptTokens")
-    completion_tokens: int = pydantic.Field(alias="completionTokens")
-    total_tokens: int = pydantic.Field(alias="totalTokens")
+class ErrorResponse(pydantic.BaseModel):
+    error: str
+    path: typing.Optional[str]
+    status: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `brevian-0.1.1a0/brevian/types/choice.py` & `brevian-0.1.4/brevian/types/choice.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/types/choice_message.py` & `brevian-0.1.4/brevian/types/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .choice_message_role import ChoiceMessageRole
+from .message_role_enum import MessageRoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChoiceMessage(pydantic.BaseModel):
-    role: ChoiceMessageRole
+class Message(pydantic.BaseModel):
+    role: MessageRoleEnum
     content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `brevian-0.1.1a0/brevian/types/error_response.py` & `brevian-0.1.4/brevian/types/too_many_requests_error_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ErrorResponse(pydantic.BaseModel):
+class TooManyRequestsErrorBody(pydantic.BaseModel):
     error: str
     path: typing.Optional[str]
     status: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `brevian-0.1.1a0/brevian/types/forbidden_error_body.py` & `brevian-0.1.4/brevian/types/forbidden_error_body.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/types/internal_server_error_body.py` & `brevian-0.1.4/brevian/types/internal_server_error_body.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/types/message.py` & `brevian-0.1.4/brevian/types/sub_query_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .message_role import MessageRole
+from .unified_citation import UnifiedCitation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Message(pydantic.BaseModel):
-    role: MessageRole
-    content: str
+class SubQueryMetadata(pydantic.BaseModel):
+    message_id: typing.Optional[str]
+    conversation_id: typing.Optional[str]
+    sub_question: typing.Optional[str]
+    retrieval_type: typing.Optional[str]
+    sub_answer: typing.Optional[str]
+    citations: typing.Optional[typing.List[UnifiedCitation]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `brevian-0.1.1a0/brevian/types/post_chat_request_messages_item.py` & `brevian-0.1.4/brevian/types/post_chat_request_messages_item.py`

 * *Files identical despite different names*

### Comparing `brevian-0.1.1a0/brevian/types/post_chat_response.py` & `brevian-0.1.4/brevian/types/post_chat_response_choices_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .post_chat_response_choices_item import PostChatResponseChoicesItem
-from .post_chat_response_usage import PostChatResponseUsage
+from .post_chat_response_choices_item_message import PostChatResponseChoicesItemMessage
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PostChatResponse(pydantic.BaseModel):
-    id: str
-    conversation_id: str = pydantic.Field(alias="conversationId")
-    created: str
-    model: str
-    choices: typing.List[PostChatResponseChoicesItem]
-    usage: PostChatResponseUsage
+class PostChatResponseChoicesItem(pydantic.BaseModel):
+    index: int
+    finish_reason: str
+    message: PostChatResponseChoicesItemMessage
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `brevian-0.1.1a0/brevian/types/post_chat_response_choices_item.py` & `brevian-0.1.4/brevian/types/unified_citation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .post_chat_response_choices_item_message import PostChatResponseChoicesItemMessage
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PostChatResponseChoicesItem(pydantic.BaseModel):
-    index: int
-    finish_reason: str
-    message: PostChatResponseChoicesItemMessage
+class UnifiedCitation(pydantic.BaseModel):
+    structured_response: typing.Optional[typing.Dict[str, typing.Any]]
+    sql_query: typing.Optional[str]
+    type: typing.Optional[str]
+    url: typing.Optional[str]
+    source_index: typing.Optional[int]
+    name: typing.Optional[str]
+    page_content: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `brevian-0.1.1a0/brevian/types/post_chat_response_choices_item_message.py` & `brevian-0.1.4/brevian/types/post_chat_response_usage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .post_chat_response_choices_item_message_role import PostChatResponseChoicesItemMessageRole
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PostChatResponseChoicesItemMessage(pydantic.BaseModel):
-    role: PostChatResponseChoicesItemMessageRole
-    content: str
+class PostChatResponseUsage(pydantic.BaseModel):
+    prompt_tokens: int
+    completion_tokens: int
+    total_tokens: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `brevian-0.1.1a0/brevian/types/post_chat_response_usage.py` & `brevian-0.1.4/brevian/types/usage.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PostChatResponseUsage(pydantic.BaseModel):
-    prompt_tokens: int = pydantic.Field(alias="promptTokens")
-    completion_tokens: int = pydantic.Field(alias="completionTokens")
-    total_tokens: int = pydantic.Field(alias="totalTokens")
+class Usage(pydantic.BaseModel):
+    prompt_tokens: int
+    completion_tokens: int
+    total_tokens: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `brevian-0.1.1a0/pyproject.toml` & `brevian-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brevian"
-version = "0.1.1a"
+version = "0.1.4"
 description = "Python SDK for BREVIAN API"
 authors = ["BREVIAN Inc <engineering@brevian.ai>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/brevian-ai/brevian-python-sdk"
 repository = "https://github.com/brevian-ai/brevian-python-sdk"
 keywords = ["brevian", "sdk", "api", "ai", "machine-learning", "artificial-intelligence"]
```

### Comparing `brevian-0.1.1a0/PKG-INFO` & `brevian-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brevian
-Version: 0.1.1a0
+Version: 0.1.4
 Summary: Python SDK for BREVIAN API
 Home-page: https://github.com/brevian-ai/brevian-python-sdk
 License: MIT
 Keywords: brevian,sdk,api,ai,machine-learning,artificial-intelligence
 Author: BREVIAN Inc
 Author-email: engineering@brevian.ai
 Requires-Python: >=3.11,<3.12
```

