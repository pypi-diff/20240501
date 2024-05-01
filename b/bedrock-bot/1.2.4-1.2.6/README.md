# Comparing `tmp/bedrock_bot-1.2.4.tar.gz` & `tmp/bedrock_bot-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.2.4.tar", max compression
+gzip compressed data, was "bedrock_bot-1.2.6.tar", max compression
```

## Comparing `bedrock_bot-1.2.4.tar` & `bedrock_bot-1.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/README.md
--rw-r--r--   0        0        0      120 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     4018 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/cli.py
--rw-r--r--   0        0        0      143 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/models/__init__.py
--rw-r--r--   0        0        0     2146 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/models/base_model.py
--rw-r--r--   0        0        0     1475 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/models/claude.py
--rw-r--r--   0        0        0     1149 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/models/mistral.py
--rw-r--r--   0        0        0      175 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/bedrock_bot/util.py
--rw-r--r--   0        0        0      468 2024-04-25 06:31:37.674951 bedrock_bot-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/LICENSE
+-rw-r--r--   0        0        0     4039 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/README.md
+-rw-r--r--   0        0        0      120 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     4619 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/cli.py
+-rw-r--r--   0        0        0      143 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/base_model.py
+-rw-r--r--   0        0        0     1610 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/claude.py
+-rw-r--r--   0        0        0     1326 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/models/mistral.py
+-rw-r--r--   0        0        0      188 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/bedrock_bot/util.py
+-rw-r--r--   0        0        0      633 2024-05-01 02:13:58.771954 bedrock_bot-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 bedrock_bot-1.2.6/PKG-INFO
```

### Comparing `bedrock_bot-1.2.4/LICENSE` & `bedrock_bot-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.4/bedrock_bot/cli.py` & `bedrock_bot-1.2.6/bedrock_bot/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,88 @@
+from __future__ import annotations
+
 import logging
 import sys
+from typing import TYPE_CHECKING
 
 import boto3
 import click
 from botocore.config import Config
 
 from . import model_list
 from .util import formatted_print
 
-CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])
+if TYPE_CHECKING:
+    from io import TextIOWrapper
+
+    from bedrock_bot.models.base_model import _BedrockModel
+
+CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}
 LOG_FORMATTER = logging.Formatter(
     "%(asctime)s - %(levelname)s - %(module)s - %(message)s",
     "%Y-%m-%d %H:%M:%S",
 )
 log = None
 
 
-def configure_logger(verbose):
-    global log
+def configure_logger(*, verbose: bool) -> None:
+    global log  # noqa: PLW0603
     log_level = logging.ERROR
     if verbose:
         log_level = logging.INFO
 
     logging.basicConfig(level=log_level)
     log = logging.getLogger()
     log.handlers[0].setFormatter(LOG_FORMATTER)
     log.info(f"Log level set to {logging.getLevelName(log_level)}")
 
 
-def available_models():
+def available_models() -> list[str]:
     return [x.name for x in model_list]
 
 
-def model_class_from_input(value):
+def model_class_from_input(value: str) -> type[_BedrockModel]:
     try:
-        return [x for x in model_list if x.name.lower() == value.lower()][0]
-    except IndexError:
-        raise click.BadParameter(
-            f"Invalid value: {value}. Allowed values are: {available_models}"
-        )
+        return next(x for x in model_list if x.name.lower() == value.lower())
+    except StopIteration as err:
+        msg = f"Invalid value: {value}. Allowed values are: {available_models}"
+        raise click.BadParameter(msg) from err
 
 
-def generate_boto_config(region):
+def generate_boto_config(region: str) -> Config:
     boto_config = Config()
     if region:
         boto_config = Config(region_name=region)
     elif boto3.setup_default_session() and not boto3.DEFAULT_SESSION.region_name:
         boto_config = Config(region_name="us-east-1")
     return boto_config
 
 
-def get_user_input(instance, args):
+def get_user_input(instance: _BedrockModel, args: list[str]) -> str:
     if instance.messages == [] and not sys.stdin.isatty():
         user_input = sys.stdin.read()
-        print(f"> {user_input}")
+        print(f"> {user_input}")  # noqa: T201
     elif instance.messages == [] and args:
         user_input = " ".join(args)
-        print(f"> {user_input}")
+        print(f"> {user_input}")  # noqa: T201
     elif not sys.stdin.isatty():
-        print(
-            "Note that you can only do one-shot requests when providing input via stdin"
+        print(  # noqa: T201
+            "Note that you can only do one-shot requests when providing input via stdin",
         )
-        exit()
+        sys.exit()
     else:
         user_input = input("> ")
 
     return user_input
 
 
-def handle_input_files(input_file) -> list:
+def handle_input_files(input_file: list[TextIOWrapper]) -> list:
     output = []
     if input_file:
-        for file in input_file:
-            output.append(f"File '{file.name}':\n" + file.read())
+        output = [f"File '{file.name}':\n{file.read()}" for file in input_file]
     return output
 
 
 @click.command()
 @click.argument("args", nargs=-1)
 @click.option(
     "-r",
@@ -101,50 +107,58 @@
 @click.option(
     "-i",
     "--input-file",
     multiple=True,
     type=click.File(),
     help="Read in file(s) to be used in your queries",
 )
-def main(model, region, raw_output, args, verbose, input_file):
-    configure_logger(verbose)
+def main(  # noqa: PLR0913
+    *,
+    model: str,
+    region: str,
+    raw_output: str,
+    args: list[str],
+    verbose: bool,
+    input_file: list[TextIOWrapper],
+) -> None:
+    configure_logger(verbose=verbose)
 
-    model = model_class_from_input(model)
+    model_class = model_class_from_input(model)
     boto_config = generate_boto_config(region)
-    instance = model(boto_config=boto_config)
+    instance = model_class(boto_config=boto_config)
 
-    print(
+    print(  # noqa: T201
         f"Hello! I am an AI assistant powered by Amazon Bedrock and using the model {instance.name}. Enter 'quit' or"
-        + " 'exit' at any time to exit. How may I help you today?"
+        " 'exit' at any time to exit. How may I help you today?",
     )
-    print(
-        "(You can clear existing context by starting a query with 'new>' or 'reset>')"
+    print(  # noqa: T201
+        "(You can clear existing context by starting a query with 'new>' or 'reset>')",
     )
 
     while True:
-        print()
+        print()  # noqa: T201
         user_input = get_user_input(instance, args)
 
         if not user_input:
             continue
         if user_input.lower() == "quit" or user_input.lower() == "exit":
-            print("\nGoodbye!")
+            print("\nGoodbye!")  # noqa: T201
             sys.exit()
         if user_input.lower().startswith("new>") or user_input.lower().startswith(
-            "reset>"
+            "reset>",
         ):
-            print("\nResetting...")
+            print("\nResetting...")  # noqa: T201
             instance.reset()
             continue
 
         if not instance.messages:
             user_input += "\n"
             user_input += "\n".join(handle_input_files(input_file))
 
         response = instance.invoke(user_input)
 
         if raw_output:
-            print(response)
+            print(response)  # noqa: T201
         else:
             formatted_print(response)
 
-        print()
+        print()  # noqa: T201
```

### Comparing `bedrock_bot-1.2.4/bedrock_bot/models/base_model.py` & `bedrock_bot-1.2.6/bedrock_bot/models/base_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import logging
 from enum import Enum
 
 import boto3
 from botocore.config import Config
 from rich.console import Console
@@ -11,68 +13,67 @@
 console = Console()
 
 
 class ConversationRole(Enum):
     USER = "user"
     ASSISTANT = "assistant"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.value
 
 
 class _BedrockModel:
-    """
-    Base class for all models. Usage:
+    """Base class for all models.
+
+    Usage:
     Add a message to the conversation and invoke the model with `model.invoke(message)`.
 
     Creating new implementations of this base model:
     - Define extra params to inject to the invoke call on self.model_params
     - Provide a model_id to `super().__init__()`
     - If your model needs a different body than the default, overwrite `self._create_invoke_body()`
     """
 
     name = "Base Model"
-    model_params = {}
+    model_params = {}  # noqa: RUF012
+    _model_id: str
 
     def __init__(
         self,
-        model_id: str,
-        boto_config=None,
-    ):
-        self._model_id = model_id
+        boto_config: None | Config = None,
+    ) -> None:
         if not boto_config:
             boto_config = Config()
         self._bedrock = boto3.client("bedrock-runtime", config=boto_config)
         self.messages = []
 
-    def reset(self):
+    def reset(self) -> None:
         self.messages = []
 
-    def append_message(self, role: ConversationRole, message: str):
+    def append_message(self, role: ConversationRole, message: str) -> None:
         self.messages.append({"role": role.value, "content": message})
 
-    def invoke(self, message: str):
+    def invoke(self, message: str) -> str:
         self.append_message(ConversationRole.USER, message)
 
         response = self._invoke()
         self.append_message(ConversationRole.ASSISTANT, response)
         return response
 
     def _create_invoke_body(self) -> dict:
         raise NotImplementedError
 
-    def _handle_response(self, body) -> str:
+    def _handle_response(self, body: dict) -> str:
         raise NotImplementedError
 
-    def _invoke(self):
+    def _invoke(self) -> str:
         body = self._create_invoke_body() | self.model_params
 
         with console.status("[bold green]Waiting for response..."):
             logger.info(f"Sending current messages to AI: {self.messages}")
             response = self._bedrock.invoke_model(
-                modelId=self._model_id, body=json.dumps(body)
+                modelId=self._model_id,
+                body=json.dumps(body),
             )
             body = json.loads(response["body"].read())
 
-            output = self._handle_response(body)
-
-        return output
+            return self._handle_response(body)
```

### Comparing `bedrock_bot-1.2.4/bedrock_bot/models/claude.py` & `bedrock_bot-1.2.6/bedrock_bot/models/claude.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,66 @@
+from __future__ import annotations
+
 import logging
+from typing import TYPE_CHECKING
 
 from rich.console import Console
 
 from .base_model import _BedrockModel
 
+if TYPE_CHECKING:
+    from botocore.config import Config
+
 logger = logging.getLogger()
 
 console = Console()
 
 
 class _Claude3(_BedrockModel):
-    model_params = {
+    model_params = {  # noqa: RUF012
         "max_tokens": 2000,
         "temperature": 1,
         "top_k": 250,
         "top_p": 0.999,
         "stop_sequences": ["\n\nHuman:"],
         "anthropic_version": "bedrock-2023-05-31",
     }
 
     def _create_invoke_body(self) -> dict:
-        body = {
+        return {
             "messages": self.messages,
         }
 
-        return body
-
-    def _handle_response(self, body) -> str:
+    def _handle_response(self, body: dict) -> str:
         response_message = body["content"][0]
 
         if response_message["type"] != "text":
-            raise RuntimeError(
-                "Unexpected response type to prompt: " + response_message["type"]
-            )
+            raise RuntimeError("Unexpected response type to prompt: " + response_message["type"])
 
         return response_message["text"]
 
-    def __init__(self, model_id: str, boto_config=None):
+    def __init__(self, boto_config: None | Config = None) -> None:
         super().__init__(
-            model_id=model_id,
             boto_config=boto_config,
         )
 
 
 class Claude3Sonnet(_Claude3):
     name = "Claude-3-Sonnet"
 
-    def __init__(self, boto_config=None):
+    def __init__(self, boto_config: None | Config = None) -> None:
+        self._model_id = "anthropic.claude-3-sonnet-20240229-v1:0"
+
         super().__init__(
-            model_id="anthropic.claude-3-sonnet-20240229-v1:0",
             boto_config=boto_config,
         )
 
 
 class Claude3Haiku(_Claude3):
     name = "Claude-3-Haiku"
 
-    def __init__(self, boto_config=None):
+    def __init__(self, boto_config: None | Config = None) -> None:
+        self._model_id = "anthropic.claude-3-haiku-20240307-v1:0"
+
         super().__init__(
-            model_id="anthropic.claude-3-haiku-20240307-v1:0",
             boto_config=boto_config,
         )
```

