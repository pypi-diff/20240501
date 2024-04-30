# Comparing `tmp/spiceai-0.2.2.tar.gz` & `tmp/spiceai-0.3.0.tar.gz`

## Comparing `spiceai-0.2.2.tar` & `spiceai-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.2.2/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.2.2/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.2.2/scripts/prompt.txt
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.2.2/scripts/run.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/errors.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/models.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/providers.py
--rw-r--r--   0        0        0    30497 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/spice_message.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/utils.py
--rw-r--r--   0        0        0    18407 2020-02-02 00:00:00.000000 spiceai-0.2.2/spice/wrapped_clients.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.2.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.2.2/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.2.2/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 spiceai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 spiceai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.3.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/prompt.txt
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/run.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/errors.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/models.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/providers.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/spice_message.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.0/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 spiceai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 spiceai-0.3.0/PKG-INFO
```

### Comparing `spiceai-0.2.2/.github/workflows/ruff.yml` & `spiceai-0.3.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/scripts/run.py` & `spiceai-0.3.0/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/errors.py` & `spiceai-0.3.0/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/models.py` & `spiceai-0.3.0/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/providers.py` & `spiceai-0.3.0/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/spice.py` & `spiceai-0.3.0/spice/spice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 import dataclasses
 import glob
 import json
+from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from json import JSONDecodeError
 from pathlib import Path
 from timeit import default_timer as timer
 from typing import Any, AsyncIterator, Callable, Collection, Dict, List, Optional, cast
 
 import httpx
 from jinja2 import Environment
 from openai.types.chat.completion_create_params import ResponseFormat
 
 from spice.errors import InvalidModelError, UnknownModelError
 from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
-from spice.spice_message import MessagesEncoder, SpiceMessage, SpiceMessages
+from spice.spice_message import MessagesEncoder, SpiceMessage
 from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
 
 @dataclass
 class SpiceCallArgs:
     model: str
@@ -232,20 +233,41 @@
 
         # TODO: Should we validate model aliases?
         self._model_aliases = model_aliases
 
         self._total_cost: float = 0
         self._prompts: Dict[str, str] = {}
 
-        if logging_dir is not None:
-            logging_dir = Path(logging_dir).expanduser().resolve()
-            timestamp = datetime.now().strftime("%m%d%y_%H%M%S")
-            self._log_file = logging_dir / f"spice_{timestamp}.json"
-        else:
-            self._log_file = None
+        self.logging_dir = logging_dir
+        self.new_run("spice")
+
+    def new_run(self, name: str):
+        """
+        Create a new run. All llm calls will be logged in a folder with the run name and a timestamp.
+        """
+        timestamp = datetime.now().strftime("%m%d%y_%H%M%S")
+        self._cur_run = f"{name}_{timestamp}"
+        self._cur_logged_names = defaultdict(int)
+
+    def _log_response(self, response: SpiceResponse, name: Optional[str] = None):
+        if self.logging_dir is not None:
+            response_dict = dataclasses.asdict(response)
+            if name is None:
+                name = "spice"
+            if self._cur_logged_names[name] != 0:
+                name += f"_{self._cur_logged_names[name]}"
+            self._cur_logged_names[name] += 1
+            name += ".json"
+
+            response_json = json.dumps(response_dict, cls=MessagesEncoder)
+
+            logging_dir = Path(self.logging_dir).expanduser() / self._cur_run
+            logging_dir.mkdir(exist_ok=True, parents=True)
+            with (logging_dir / name).open("w") as file:
+                file.write(f"{response_json}\n")
 
     @property
     def total_cost(self) -> float:
         """The total cost in cents of all api calls made through this Spice client."""
         return self._total_cost
 
     def load_provider(self, provider: Provider | str):
@@ -313,31 +335,23 @@
             messages=messages,
             stream=stream,
             temperature=temperature,
             max_tokens=max_tokens,
             response_format=response_format,
         )
 
-    def _log_response(self, response: SpiceResponse):
-        if self._log_file is not None:
-            response_json = json.dumps(dataclasses.asdict(response), cls=MessagesEncoder)
-
-            # TODO: This unfortunately isn't a valid json file (since it has multiple objects) but it's the easiest way to keep all requests from one client together
-            with self._log_file.open("a") as file:
-                file.write(response_json)
-                file.write("\n")
-
     async def get_response(
         self,
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
+        name: Optional[str] = None,
     ) -> SpiceResponse:
         """
         Asynchronously retrieves a chat completion response.
 
         Args:
             messages: The list of messages given as context for the completion.
             Will raise an ImageError if any invalid images are given.
@@ -351,14 +365,16 @@
 
             temperature: The temperature to give the model.
 
             max_tokens: The maximum tokens the model can output.
 
             response_format: For valid models, will set the response format to 'text' or 'json'.
             If the provider/model does not support response_format, this argument will be ignored.
+
+            name: If given, will be given this name when logged.
         """
 
         text_model = self._get_text_model(model)
         client = self._get_client(text_model, provider)
         call_args = self._fix_call_args(messages, text_model, False, temperature, max_tokens, response_format)
 
         start_time = timer()
@@ -368,25 +384,26 @@
         text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
 
         cost = text_request_cost(text_model, input_tokens, output_tokens)
         if cost is not None:
             self._total_cost += cost
 
         response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
-        self._log_response(response)
+        self._log_response(response, name)
         return response
 
     async def stream_response(
         self,
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
+        name: Optional[str] = None,
     ) -> StreamingSpiceResponse:
         """
         Asynchronously retrieves a chat completion stream that can be iterated over asynchronously.
 
         Args:
             messages: The list of messages given as context for the completion.
             Will raise an ImageError if any invalid images are given.
@@ -400,29 +417,32 @@
 
             temperature: The temperature to give the model.
 
             max_tokens: The maximum tokens the model can output.
 
             response_format: For valid models, will set the response format to 'text' or 'json'.
             If the provider/model does not support response_format, this argument will be ignored.
+
+            name: If given, will be given this name when logged.
         """
 
         text_model = self._get_text_model(model)
         client = self._get_client(text_model, provider)
         call_args = self._fix_call_args(messages, text_model, True, temperature, max_tokens, response_format)
 
         with client.catch_and_convert_errors():
             stream = await client.get_chat_completion_or_stream(call_args)
         stream = cast(AsyncIterator, stream)
 
         def callback(response: SpiceResponse, cache: List[float] = [0]):
             if response.cost is not None:
                 self._total_cost += response.cost - cache[0]
                 cache[0] = response.cost
-            self._log_response(response)
+            # TODO: Do we want to log multiple times? Our old log might be incomplete, which is why this is still in, but probably not necessary.
+            self._log_response(response, name)
 
         return StreamingSpiceResponse(text_model, call_args, client, stream, callback)
 
     def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel:
         if model is None:
             if self._default_embeddings_model is None:
                 raise InvalidModelError("Model is required when default embeddings model is not set at initialization")
@@ -742,38 +762,49 @@
             )
             if str(file_path).endswith(".toml"):
                 if use_toml:
                     self._load_toml_dict(tomllib.loads(prompt), name)  # pyright: ignore[reportPossiblyUnboundVariable]
             elif str(file_path).endswith(".txt"):
                 self.store_prompt(prompt, name)
 
-    def load_url(self, url: str):
+    def load_url(self, url: str, name: str):
         """
-        Loads a prompt from the given url. Will send a GET request to the url and expects a response with the following schema:
+        Loads a prompt from the given url. Will send a GET request to the url and expects a response with either the following schema or a toml file (.toml only available for Python 3.11 and onwards):
         ```
         {
             "prompts": [
                 {
                     "name": "<prompt_name>",
                     "prompt": "<prompt>"
                 }, ...
             ]
         }
         ```
+        TOML will only be loaded if the url points to a .toml file.
+        All prompt names will be prefixed with `name.`
         If any name collides with the name of a previously loaded prompt, the previous prompt will be overwritten.
 
         Args:
             url: The url.
+
+            name: The name to prefix the prompts with.
         """
 
-        raw_json = httpx.get(url).content.decode("utf-8")
-        try:
-            prompts = json.loads(raw_json)
-        except JSONDecodeError:
-            raise
+        response = httpx.get(url).content.decode("utf-8")
+        if url.endswith(".toml"):
+            import tomllib
+
+            try:
+                prompts = tomllib.loads(response)
+            except tomllib.TOMLDecodeError:
+                raise
+            self._load_toml_dict(prompts, name)
+
+        else:
+            try:
+                prompts = json.loads(response)
+            except JSONDecodeError:
+                raise
 
-        try:
             for prompt_object in prompts["prompts"]:
                 name, prompt = prompt_object["name"], prompt_object["prompt"]
                 self.store_prompt(prompt, name)
-        except:
-            raise
```

### Comparing `spiceai-0.2.2/spice/spice_message.py` & `spiceai-0.3.0/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/utils.py` & `spiceai-0.3.0/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/spice/wrapped_clients.py` & `spiceai-0.3.0/spice/wrapped_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import base64
 import io
 import mimetypes
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, AsyncIterator, Collection, ContextManager, Dict, List, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Any, AsyncIterator, Collection, ContextManager, Dict, List, Optional, Tuple
 
 import anthropic
 import httpx
 import openai
 import tiktoken
 from anthropic import AsyncAnthropic
 from anthropic.types import Message, MessageParam, MessageStreamEvent, TextBlockParam
 from openai import AsyncAzureOpenAI, AsyncOpenAI, OpenAI
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 from PIL import Image
 from typing_extensions import override
 
-from spice.errors import APIConnectionError, APIError, AuthenticationError, ImageError, InvalidModelError, SpiceError
+from spice.errors import APIConnectionError, APIError, AuthenticationError, ImageError, InvalidModelError
 from spice.spice_message import VALID_MIMETYPES, SpiceMessage
 
 if TYPE_CHECKING:
     from spice.models import Model
     from spice.spice import SpiceCallArgs
 
 
@@ -85,15 +85,15 @@
         if call_args.max_tokens is None and "gpt-4" in call_args.model and "vision-preview" in call_args.model:
             max_tokens = 4096
         else:
             max_tokens = call_args.max_tokens
 
         return await self._client.chat.completions.create(
             model=call_args.model,
-            messages=call_args.messages,
+            messages=list(call_args.messages),
             stream=call_args.stream,
             temperature=call_args.temperature,
             max_tokens=max_tokens,
             **maybe_response_format_kwargs,
         )
 
     @override
@@ -206,15 +206,17 @@
         )
 
 
 class WrappedAnthropicClient(WrappedClient):
     def __init__(self, key):
         self._client = AsyncAnthropic(api_key=key)
 
-    def _convert_messages(self, messages: Collection[SpiceMessage]) -> Tuple[str, List[MessageParam]]:
+    def _convert_messages(
+        self, messages: Collection[SpiceMessage], add_json_brace: bool
+    ) -> Tuple[str, List[MessageParam]]:
         # Anthropic handles both images and system messages different from OpenAI, only allows alternating user / assistant messages,
         # and doesn't support tools / function calling (still in beta, and doesn't support streaming)
 
         system = ""
         converted_messages: List[MessageParam] = []
         start = True
         cur_role = ""
@@ -307,33 +309,40 @@
                 case "tool":
                     # Right now anthropic tool use is in beta and doesn't support some things like streaming, but once it releases we can modify this.
                     pass
                 case "function":
                     # Deprecated, nobody should use this
                     pass
 
+        if add_json_brace and converted_messages:
+            if converted_messages[-1]["role"] == "assistant" and not converted_messages[-1]["content"]:
+                converted_messages[-1]["content"] += "{"  # pyright: ignore
+            elif converted_messages[-1]["role"] == "user":
+                converted_messages.append({"role": "assistant", "content": "{"})
+
         return system, converted_messages
 
     @override
     async def get_chat_completion_or_stream(self, call_args: SpiceCallArgs):
-        if call_args.response_format is not None and call_args.response_format.get("type", "text") != "text":
-            raise InvalidModelError("response_format is not supported by Anthropic")
+        add_json_brace = (
+            call_args.response_format is not None and call_args.response_format.get("type", "text") == "json_object"
+        )
 
         # max_tokens is required by anthropic api
         if call_args.max_tokens is None:
             max_tokens = 4096
         else:
             max_tokens = call_args.max_tokens
 
         # temperature is optional but can't be None
         maybe_temperature_kwargs: dict[str, Any] = (
             {"temperature": call_args.temperature} if call_args.temperature is not None else {}
         )
 
-        system, converted_messages = self._convert_messages(call_args.messages)
+        system, converted_messages = self._convert_messages(call_args.messages, add_json_brace)
 
         return await self._client.messages.create(
             model=call_args.model,
             system=system,
             messages=converted_messages,
             stream=call_args.stream,
             max_tokens=max_tokens,
```

### Comparing `spiceai-0.2.2/LICENSE` & `spiceai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/README.md` & `spiceai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.2.2/pyproject.toml` & `spiceai-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.2.2"
+version = "0.3.0"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.2.2/PKG-INFO` & `spiceai-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

