# Comparing `tmp/livekit-plugins-elevenlabs-0.3.dev0.tar.gz` & `tmp/livekit_plugins_elevenlabs-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-elevenlabs-0.3.dev0.tar", last modified: Thu Apr 11 22:03:31 2024, max compression
+gzip compressed data, was "livekit_plugins_elevenlabs-0.4.dev0.tar", last modified: Wed May  1 00:22:19 2024, max compression
```

## Comparing `livekit-plugins-elevenlabs-0.3.dev0.tar` & `livekit_plugins_elevenlabs-0.4.dev0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.896295 livekit_plugins_elevenlabs-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-01 00:22:19.892295 livekit_plugins_elevenlabs-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.892295 livekit_plugins_elevenlabs-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.892295 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.892295 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.892295 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-01 00:22:19.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 00:22:19.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:19.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:22:19.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:19.000000 livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:19.896295 livekit_plugins_elevenlabs-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-01 00:22:15.000000 livekit_plugins_elevenlabs-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO` & `livekit_plugins_elevenlabs-0.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
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
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py` & `livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py` & `livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/tts.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,54 +13,53 @@
 # limitations under the License.
 
 import asyncio
 import base64
 import contextlib
 import dataclasses
 import json
-import logging
 import os
 from dataclasses import dataclass
-from typing import Any, AsyncIterable, Dict, List, Optional
+from typing import AsyncIterable, List
 
 import aiohttp
 from livekit import rtc
-from livekit.agents import tts
+from livekit.agents import aio, tts
 
+from .log import logger
 from .models import TTSModels
 
 
 @dataclass
+class VoiceSettings:
+    stability: float  # [0.0 - 1.0]
+    similarity_boost: float  # [0.0 - 1.0]
+    style: float | None = None  # [0.0 - 1.0]
+    use_speaker_boost: bool | None = False
+
+
+@dataclass
 class Voice:
     id: str
     name: str
     category: str
-    settings: Optional["VoiceSettings"] = None
-
-
-@dataclass
-class VoiceSettings:
-    stability: float  # [0.0 - 1.0]
-    similarity_boost: float  # [0.0 - 1.0]
-    style: Optional[float] = None  # [0.0 - 1.0]
-    use_speaker_boost: Optional[bool] = False
+    settings: VoiceSettings | None = None
 
 
 DEFAULT_VOICE = Voice(
     id="EXAVITQu4vr4xnSDxMaL",
     name="Bella",
     category="premade",
     settings=VoiceSettings(
         stability=0.71, similarity_boost=0.5, style=0.0, use_speaker_boost=True
     ),
 )
 
 API_BASE_URL_V1 = "https://api.elevenlabs.io/v1"
 AUTHORIZATION_HEADER = "xi-api-key"
-STREAM_EOS = ""
 
 
 @dataclass
 class TTSOptions:
     api_key: str
     voice: Voice
     model_id: TTSModels
@@ -70,268 +69,317 @@
 
 
 class TTS(tts.TTS):
     def __init__(
         self,
         *,
         voice: Voice = DEFAULT_VOICE,
-        model_id: TTSModels = "eleven_multilingual_v2",
-        api_key: Optional[str] = None,
-        base_url: Optional[str] = None,
+        model_id: TTSModels = "eleven_turbo_v2",
+        api_key: str | None = None,
+        base_url: str | None = None,
         sample_rate: int = 24000,
-        latency: int = 2,
+        latency: int = 3,
     ) -> None:
-        super().__init__(streaming_supported=True)
+        super().__init__(
+            streaming_supported=True, sample_rate=sample_rate, num_channels=1
+        )
         api_key = api_key or os.environ.get("ELEVEN_API_KEY")
         if not api_key:
             raise ValueError("ELEVEN_API_KEY must be set")
 
         self._session = aiohttp.ClientSession()
-        self._config = TTSOptions(
+        self._opts = TTSOptions(
             voice=voice,
             model_id=model_id,
             api_key=api_key,
             base_url=base_url or API_BASE_URL_V1,
             sample_rate=sample_rate,
             latency=latency,
         )
 
     async def list_voices(self) -> List[Voice]:
         async with self._session.get(
-            f"{self._config.base_url}/voices",
-            headers={AUTHORIZATION_HEADER: self._config.api_key},
+            f"{self._opts.base_url}/voices",
+            headers={AUTHORIZATION_HEADER: self._opts.api_key},
         ) as resp:
             data = await resp.json()
             return dict_to_voices_list(data)
 
     def synthesize(
         self,
         text: str,
     ) -> AsyncIterable[tts.SynthesizedAudio]:
-        voice = self._config.voice
+        voice = self._opts.voice
+        url = f"{self._opts.base_url}/text-to-speech/{voice.id}?output_format=pcm_{self._opts.sample_rate}"
 
         async def generator():
-            async with self._session.post(
-                f"{self._config.base_url}/text-to-speech/{voice.id}?output_format=pcm_44100",
-                headers={AUTHORIZATION_HEADER: self._config.api_key},
-                json=dict(
-                    text=text,
-                    model_id=self._config.model_id,
-                    voice_settings=dataclasses.asdict(voice.settings)
-                    if voice.settings
-                    else None,
-                ),
-            ) as resp:
-                data = await resp.read()
-                yield tts.SynthesizedAudio(
-                    text=text,
-                    data=rtc.AudioFrame(
-                        data=data,
-                        sample_rate=44100,
-                        num_channels=1,
-                        samples_per_channel=len(data) // 2,  # 16-bit
+            try:
+                async with self._session.post(
+                    url,
+                    headers={AUTHORIZATION_HEADER: self._opts.api_key},
+                    json=dict(
+                        text=text,
+                        model_id=self._opts.model_id,
+                        voice_settings=dataclasses.asdict(voice.settings)
+                        if voice.settings
+                        else None,
                     ),
-                )
+                ) as resp:
+                    data = await resp.read()
+                    yield tts.SynthesizedAudio(
+                        text=text,
+                        data=rtc.AudioFrame(
+                            data=data,
+                            sample_rate=self._opts.sample_rate,
+                            num_channels=1,
+                            samples_per_channel=len(data) // 2,  # 16-bit
+                        ),
+                    )
+            except Exception as e:
+                logger.error(f"failed to synthesize: {e}")
 
         return generator()
 
     def stream(
         self,
     ) -> "SynthesizeStream":
-        return SynthesizeStream(self._session, self._config)
+        return SynthesizeStream(self._session, self._opts)
 
 
 class SynthesizeStream(tts.SynthesizeStream):
+    _STREAM_EOS = ""
+
     def __init__(
         self,
         session: aiohttp.ClientSession,
-        config: TTSOptions,
+        opts: TTSOptions,
+        max_retry: int = 32,
     ):
-        self._config = config
+        self._opts = opts
         self._session = session
 
-        self._queue = asyncio.Queue[str]()
-        self._event_queue = asyncio.Queue[tts.SynthesisEvent]()
+        self._queue = asyncio.Queue[str | None]()
+        self._event_queue = asyncio.Queue[tts.SynthesisEvent | None]()
         self._closed = False
-
-        self._main_task = asyncio.create_task(self._run(max_retry=32))
-
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logging.error(f"elevenlabs synthesis task failed: {task.exception()}")
-
-        self._main_task.add_done_callback(log_exception)
         self._text = ""
 
+        self._main_task = asyncio.create_task(self._run(max_retry))
+
     def _stream_url(self) -> str:
-        base_url = self._config.base_url
-        voice_id = self._config.voice.id
-        model_id = self._config.model_id
-        return f"{base_url}/text-to-speech/{voice_id}/stream-input?model_id={model_id}&output_format=pcm_{self._config.sample_rate}&optimize_streaming_latency={self._config.latency}"
+        base_url = self._opts.base_url
+        voice_id = self._opts.voice.id
+        model_id = self._opts.model_id
+        sample_rate = self._opts.sample_rate
+        latency = self._opts.latency
+        return f"{base_url}/text-to-speech/{voice_id}/stream-input?model_id={model_id}&output_format=pcm_{sample_rate}&optimize_streaming_latency={latency}"
 
     def push_text(self, token: str | None) -> None:
         if self._closed:
             raise ValueError("cannot push to a closed stream")
 
-        if not token or len(token) == 0:
+        if token is None:
+            self._flush_if_needed()
+            return
+
+        if len(token) == 0:
+            # 11labs marks the EOS with an empty string, avoid users from pushing empty strings
             return
 
-        # TODO: Native word boundary detection may not be good enough for all languages
+        # TODO: Naive word boundary detection may not be good enough for all languages
         # fmt: off
         splitters = (".", ",", "?", "!", ";", ":", "—", "-", "(", ")", "[", "]", "}", " ")
         # fmt: on
 
         self._text += token
-        if token[-1] in splitters:
-            self._queue.put_nowait(self._text)
-            self._text = ""
 
-    async def _run(self, max_retry: int) -> None:
-        retry_count = 0
-        listen_task: Optional[asyncio.Task] = None
-        ws: Optional[aiohttp.ClientWebSocketResponse] = None
-        retry_text_queue: asyncio.Queue[str] = asyncio.Queue()
         while True:
-            try:
-                ws = await self._try_connect()
-                retry_count = 0  # reset retry count
+            last_split = -1
+            for i, c in enumerate(self._text):
+                if c in splitters:
+                    last_split = i
+                    break
 
-                listen_task = asyncio.create_task(self._listen_task(ws))
+            if last_split == -1:
+                break
 
-                # forward queued text to 11labs
-                started = False
-                while not ws.closed:
-                    text = None
-                    if not retry_text_queue.empty():
-                        text = await retry_text_queue.get()
-                        retry_text_queue.task_done()
-                    else:
-                        text = await self._queue.get()
-
-                    if not started:
-                        self._event_queue.put_nowait(
-                            tts.SynthesisEvent(type=tts.SynthesisEventType.STARTED)
-                        )
-                        started = True
-                    text_packet = dict(
-                        text=text,
-                        try_trigger_generation=True,
-                    )
+            seg = self._text[: last_split + 1]
+            seg = seg.strip() + " "  # 11labs expects a space at the end
+            self._queue.put_nowait(seg)
+            self._text = self._text[last_split + 1 :]
+
+    async def aclose(self, *, wait: bool = True) -> None:
+        self._flush_if_needed()
+        self._queue.put_nowait(None)
+        self._closed = True
 
-                    # This case can happen in normal operation because 11labs will not
-                    # keep connections open indefinitely if we are not sending data.
-                    try:
-                        await ws.send_str(json.dumps(text_packet))
-                    except Exception:
-                        await retry_text_queue.put(text)
+        if not wait:
+            self._main_task.cancel()
+
+        with contextlib.suppress(asyncio.CancelledError):
+            await self._main_task
+
+    def _flush_if_needed(self) -> None:
+        seg = self._text.strip()
+        if len(seg) > 0:
+            self._queue.put_nowait(seg + " ")
+
+        self._text = ""
+        self._queue.put_nowait(SynthesizeStream._STREAM_EOS)
+
+    async def _run(self, max_retry: int) -> None:
+        retry_count = 0
+        ws: aiohttp.ClientWebSocketResponse | None = None
+        ws_task: asyncio.Task | None = None
+        data_tx: aio.ChanSender[str] | None = None
+
+        try:
+            while True:
+                ws_connected = ws is not None and not ws.closed
+                try:
+                    data = await self._queue.get()
+
+                    if data is None:
+                        if ws_task is not None:
+                            await ws_task
                         break
 
-                    # We call self._queue.task_done() even if we are retrying the text because
-                    # all text has gone through self._queue. An exception may have short-circuited
-                    # out of the loop so task_done() will not have already been called on text that
-                    # is being retried.
-                    self._queue.task_done()
-                    if text == STREAM_EOS:
-                        await listen_task
-                        # We know 11labs is closing the stream after each request/flush
-                        self._event_queue.put_nowait(
-                            tts.SynthesisEvent(type=tts.SynthesisEventType.FINISHED)
+                    if not ws_connected:
+                        if data == SynthesizeStream._STREAM_EOS:
+                            continue
+
+                        with contextlib.suppress(asyncio.CancelledError):
+                            if ws_task is not None:
+                                await ws_task
+
+                        ws = await self._session.ws_connect(
+                            self._stream_url(),
+                            headers={AUTHORIZATION_HEADER: self._opts.api_key},
+                        )
+                        data_tx, data_rx = aio.channel()
+                        ws_task = asyncio.create_task(self._run_ws(ws, data_rx))
+
+                    assert data_tx is not None
+                    assert ws_task is not None
+                    assert ws is not None
+
+                    data_tx.send_nowait(data)
+
+                except Exception:
+                    if retry_count >= max_retry:
+                        logger.exception(
+                            f"failed to connect to 11labs after {max_retry} retries"
                         )
                         break
 
-            except asyncio.CancelledError:
-                if ws:
-                    await ws.close()
-                    if listen_task:
-                        await asyncio.shield(listen_task)
-                break
-            except Exception as e:
-                if retry_count > max_retry and max_retry > 0:
-                    logging.error(f"failed to connect to ElevenLabs: {e}")
-                    break
+                    retry_delay = min(retry_count * 5, 5)  # max 5s
+                    retry_count += 1
 
-                retry_delay = min(retry_count * 5, 5)  # max 5s
-                retry_count += 1
-                logging.warning(
-                    f"failed to connect to ElevenLabs: {e} - retrying in {retry_delay}s"
-                )
-                await asyncio.sleep(retry_delay)
+                    logger.warning(
+                        f"failed to connect to 11labs, retrying in {retry_delay}s"
+                    )
+                    await asyncio.sleep(retry_delay)
 
-        self._closed = True
+        except Exception:
+            logger.exception("11labs task failed")
+        finally:
+            with contextlib.suppress(asyncio.CancelledError):
+                if ws_task is not None:
+                    ws_task.cancel()
+                    await ws_task
 
-    async def _try_connect(self) -> aiohttp.ClientWebSocketResponse:
-        ws = await self._session.ws_connect(
-            self._stream_url(),
-            headers={AUTHORIZATION_HEADER: self._config.api_key},
-        )
+            self._event_queue.put_nowait(None)
 
-        voice = self._config.voice
-        voice_settings = dataclasses.asdict(voice.settings) if voice.settings else None
+    async def _run_ws(
+        self, ws: aiohttp.ClientWebSocketResponse, data_rx: aio.ChanReceiver[str]
+    ) -> None:
+        closing_ws = False
 
-        init_packet = dict(
-            text=" ",
-            voice_settings=voice_settings,
+        self._event_queue.put_nowait(
+            tts.SynthesisEvent(type=tts.SynthesisEventType.STARTED)
         )
-        await ws.send_str(json.dumps(init_packet))
-        return ws
 
-    async def _listen_task(self, ws: aiohttp.ClientWebSocketResponse) -> None:
-        while True:
-            msg = await ws.receive()
+        async def send_task():
+            nonlocal closing_ws
 
-            if msg.type in (
-                aiohttp.WSMsgType.CLOSED,
-                aiohttp.WSMsgType.CLOSE,
-                aiohttp.WSMsgType.CLOSING,
-            ):
-                break
-
-            if msg.type != aiohttp.WSMsgType.TEXT:
-                continue
+            # 11labs stream must be initialized with a space
+            voice = self._opts.voice
+            voice_settings = (
+                dataclasses.asdict(voice.settings) if voice.settings else None
+            )
+            init_pkt = dict(
+                text=" ",
+                voice_settings=voice_settings,
+            )
+            await ws.send_str(json.dumps(init_pkt))
 
-            jsonMessage: Dict[str, Any] = json.loads(str(msg.data))
-            if jsonMessage.get("audio"):
-                data = base64.b64decode(jsonMessage["audio"])
-                audio_frame = rtc.AudioFrame(
-                    data=data,
-                    sample_rate=self._config.sample_rate,
-                    num_channels=1,
-                    samples_per_channel=len(data) // 2,
-                )
-                self._event_queue.put_nowait(
-                    tts.SynthesisEvent(
-                        type=tts.SynthesisEventType.AUDIO,
-                        audio=tts.SynthesizedAudio(text="", data=audio_frame),
-                    )
+            while True:
+                data = await data_rx.recv()
+                data_pkt = dict(
+                    text=data,
+                    try_trigger_generation=False,
                 )
-            elif jsonMessage.get("isFinal"):
-                break
-            else:
-                logging.error(f"Unhandled message from ElevenLabs: {msg}")
+                if data == SynthesizeStream._STREAM_EOS:
+                    closing_ws = True
 
-    async def flush(self) -> None:
-        self._queue.put_nowait(self._text + " ")
-        self._text = ""
-        self._queue.put_nowait(STREAM_EOS)
-        await self._queue.join()
+                await ws.send_str(json.dumps(data_pkt))
+
+                if closing_ws:
+                    return
 
-    async def aclose(self, wait=False) -> None:
-        if wait:
-            logging.warning(
-                "wait=True is not yet supported for ElevenLabs TTS. Closing immediately."
+        async def recv_task():
+            nonlocal closing_ws
+            while True:
+                msg = await ws.receive()
+                if msg.type in (
+                    aiohttp.WSMsgType.CLOSED,
+                    aiohttp.WSMsgType.CLOSE,
+                    aiohttp.WSMsgType.CLOSING,
+                ):
+                    if closing_ws:  # close is expected
+                        return
+
+                    raise Exception("11labs connection closed unexpectedly")
+
+                if msg.type != aiohttp.WSMsgType.TEXT:
+                    logger.warning("unexpected 11labs message type %s", msg.type)
+                    continue
+
+                data: dict = json.loads(msg.data)
+                if data.get("audio"):
+                    b64data = base64.b64decode(data["audio"])
+                    frame = rtc.AudioFrame(
+                        data=b64data,
+                        sample_rate=self._opts.sample_rate,
+                        num_channels=1,
+                        samples_per_channel=len(data) // 2,
+                    )
+                    self._event_queue.put_nowait(
+                        tts.SynthesisEvent(
+                            type=tts.SynthesisEventType.AUDIO,
+                            audio=tts.SynthesizedAudio(text="", data=frame),
+                        )
+                    )
+                elif data.get("isFinal"):
+                    return
+
+        try:
+            await asyncio.gather(send_task(), recv_task())
+        except Exception:
+            logger.exception("11labs connection failed")
+        finally:
+            self._event_queue.put_nowait(
+                tts.SynthesisEvent(type=tts.SynthesisEventType.FINISHED)
             )
-        self._main_task.cancel()
-        with contextlib.suppress(asyncio.CancelledError):
-            await self._main_task
 
     async def __anext__(self) -> tts.SynthesisEvent:
-        if self._closed and self._event_queue.empty():
+        evt = await self._event_queue.get()
+        if evt is None:
             raise StopAsyncIteration
 
-        return await self._event_queue.get()
+        return evt
 
 
 def dict_to_voices_list(data: dict) -> List[Voice]:
     voices = []
     for voice in data["voices"]:
         voices.append(
             Voice(
```

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py` & `livekit_plugins_elevenlabs-0.4.dev0/livekit/plugins/elevenlabs/version.py`

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

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit_plugins_elevenlabs-0.4.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
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
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit-plugins-elevenlabs-0.3.dev0/setup.py` & `livekit_plugins_elevenlabs-0.4.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "elevenlabs"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
-        "livekit ~= 0.9",
-        "livekit-agents~=0.5.dev0",
+        "livekit ~= 0.11",
+        "livekit-agents~=0.6.dev0",
         "aiohttp >= 3.8.5",
     ],
     package_data={
         "livekit.plugins.elevenlabs": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

