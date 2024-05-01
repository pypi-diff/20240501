# Comparing `tmp/livekit-plugins-openai-0.3.dev0.tar.gz` & `tmp/livekit_plugins_openai-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-openai-0.3.dev0.tar", last modified: Thu Apr 11 22:03:54 2024, max compression
+gzip compressed data, was "livekit_plugins_openai-0.4.dev0.tar", last modified: Wed May  1 00:22:29 2024, max compression
```

## Comparing `livekit-plugins-openai-0.3.dev0.tar` & `livekit_plugins_openai-0.4.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.637794 livekit_plugins_openai-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.637794 livekit_plugins_openai-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:29.000000 livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:29.641794 livekit_plugins_openai-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 00:22:25.000000 livekit_plugins_openai-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-openai-0.3.dev0/PKG-INFO` & `livekit_plugins_openai-0.4.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/llm.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,36 +19,39 @@
     model: str | ChatModels
 
 
 class LLM(llm.LLM):
     def __init__(
         self,
         *,
-        model: str | ChatModels = "gpt-4-1106-preview",
+        model: str | ChatModels = "gpt-4-turbo",
         client: openai.AsyncClient | None = None,
     ) -> None:
         self._opts = LLMOptions(model=model)
         self._client = client or openai.AsyncClient()
         self._running_fncs: MutableSet[asyncio.Task] = set()
 
     async def chat(
         self,
         history: llm.ChatContext,
         fnc_ctx: llm.FunctionContext | None = None,
         temperature: float | None = None,
         n: int | None = None,
     ) -> "LLMStream":
-        tools = to_openai_tools(fnc_ctx) if fnc_ctx else openai.NOT_GIVEN
+        opts = dict()
+        if fnc_ctx:
+            opts["tools"] = to_openai_tools(fnc_ctx)
+
         cmp = await self._client.chat.completions.create(
             messages=to_openai_ctx(history),
             model=self._opts.model,
             n=n,
-            tools=tools,
             temperature=temperature,
             stream=True,
+            **opts,
         )
 
         return LLMStream(cmp, fnc_ctx)
 
 
 class LLMStream(llm.LLMStream):
     def __init__(
@@ -168,19 +171,22 @@
                 return
 
             if issubclass(arg.type, enum.Enum) and args[arg.name] not in arg.type:
                 logger.error(f"invalid arg {arg.name} for ai_callable {name}")
                 return
 
         logger.debug(f"calling function {name} with arguments {args}")
+        self._called_functions.append(
+            llm.CalledFunction(fnc_name=name, fnc=fnc.fnc, args=args)
+        )
         func = functools.partial(fnc.fnc, **args)
         if asyncio.iscoroutinefunction(fnc.fnc):
-            task = asyncio.ensure_future(func())
+            task = asyncio.create_task(func())
         else:
-            task = asyncio.ensure_future(asyncio.to_thread(func))
+            task = asyncio.create_task(asyncio.to_thread(func))
 
         def _task_done(task: asyncio.Task) -> None:
             if not task.cancelled() and task.exception():
                 logger.error("ai_callable task failed", exc_info=task.exception())
             self._running_fncs.discard(task)
 
         task.add_done_callback(_task_done)
@@ -206,14 +212,15 @@
     ]
 
 
 def to_openai_tools(fnc_ctx: llm.FunctionContext):
     tools = []
     for fnc in fnc_ctx.ai_functions.values():
         plist = {}
+        required = []
         for arg_name, arg in fnc.args.items():
             p: Dict[str, Any] = {}
             if arg.desc:
                 p["description"] = arg.desc
 
             if arg.type is str:
                 p["type"] = "string"
@@ -225,22 +232,26 @@
                 p["type"] = "boolean"
             elif issubclass(arg.type, enum.Enum):
                 p["type"] = "string"
                 p["enum"] = [e.value for e in arg.type]
 
             plist[arg_name] = p
 
+            if arg.default is inspect.Parameter.empty:
+                required.append(arg_name)
+
         tools.append(
             {
                 "type": "function",
                 "function": {
                     "name": fnc.metadata.name,
                     "description": fnc.metadata.desc,
                     "parameters": {
                         "type": "object",
                         "properties": plist,
+                        "required": required,
                     },
                 },
             }
         )
 
     return tools
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/models.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import Literal
 
 WhisperModels = Literal["whisper-1"]
 TTSModels = Literal["tts-1", "tts-1-hd"]
 TTSVoices = Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"]
 DalleModels = Literal["dall-e-2", "dall-e-3"]
 ChatModels = Literal[
-    "gpt-4-1106-preview",
+    "gpt-4-turbo",
+    "gpt-4-turbo-2024-04-09",
+    "gpt-4-turbo-preview",
+    "gpt-4-0125-preview" "gpt-4-1106-preview",
     "gpt-4-vision-preview",
+    "gpt-4-1106-vision-preview",
     "gpt-4",
     "gpt-4-0314",
     "gpt-4-0613",
     "gpt-4-32k",
     "gpt-4-32k-0314",
     "gpt-4-32k-0613",
     "gpt-3.5-turbo",
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/stt.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/tts.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/tts.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 OPENAI_ENPOINT = "https://api.openai.com/v1/audio/speech"
 
 
 class TTS(tts.TTS):
     def __init__(
         self, model: TTSModels, voice: TTSVoices, api_key: Optional[str] = None
     ) -> None:
-        super().__init__(streaming_supported=False)
+        super().__init__(
+            streaming_supported=False,
+            sample_rate=OPENAI_TTS_SAMPLE_RATE,
+            num_channels=OPENAI_TTS_CHANNELS,
+        )
         api_key = api_key or os.environ.get("OPENAI_API_KEY")
         if not api_key:
             raise ValueError("OPENAI_API_KEY must be set")
 
         # TODO: we want to reuse aiohttp sessions
         # for improved latency but doing so doesn't
         # give us a clean way to close the session.
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py` & `livekit_plugins_openai-0.4.dev0/livekit/plugins/openai/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.dev0"
+__version__ = "0.4.dev0"
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO` & `livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
```

### Comparing `livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/SOURCES.txt` & `livekit_plugins_openai-0.4.dev0/livekit_plugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit-plugins-openai-0.3.dev0/setup.py` & `livekit_plugins_openai-0.4.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
-        "livekit ~= 0.9",
-        "livekit-agents~=0.5.dev0",
+        "livekit ~= 0.11",
+        "livekit-agents~=0.6.dev0",
         "openai >= 1.0.0",
         "requests >= 2, < 3",
     ],
     package_data={
         "livekit.plugins.openai": ["py.typed"],
     },
     project_urls={
```

