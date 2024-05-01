# Comparing `tmp/livekit-plugins-deepgram-0.3.dev0.tar.gz` & `tmp/livekit_plugins_deepgram-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-deepgram-0.3.dev0.tar", last modified: Thu Apr 11 22:01:22 2024, max compression
+gzip compressed data, was "livekit_plugins_deepgram-0.4.dev0.tar", last modified: Wed May  1 00:22:14 2024, max compression
```

## Comparing `livekit-plugins-deepgram-0.3.dev0.tar` & `livekit_plugins_deepgram-0.4.dev0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:14.839242 livekit_plugins_deepgram-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 00:22:14.839242 livekit_plugins_deepgram-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:14.835242 livekit_plugins_deepgram-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:14.835242 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:14.839242 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:14.839242 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 00:22:14.000000 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-01 00:22:14.000000 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:14.000000 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:22:14.000000 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:14.000000 livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:14.839242 livekit_plugins_deepgram-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-01 00:22:10.000000 livekit_plugins_deepgram-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-deepgram-0.3.dev0/PKG-INFO` & `livekit_plugins_deepgram-0.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
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
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/models.py` & `livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/models.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/stt.py` & `livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/stt.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 from __future__ import annotations
 
 import asyncio
 import dataclasses
 import io
 import json
-import logging
 import os
 import wave
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import List
 from urllib.parse import urlencode
 
 import aiohttp
 from livekit import rtc
 from livekit.agents import stt
 from livekit.agents.utils import AudioBuffer, merge_frames
 
+from .log import logger
 from .models import DeepgramLanguages, DeepgramModels
 
 
 @dataclass
 class STTOptions:
     language: DeepgramLanguages | str | None
     detect_language: bool
@@ -52,23 +52,23 @@
         language: DeepgramLanguages = "en-US",
         detect_language: bool = False,
         interim_results: bool = True,
         punctuate: bool = True,
         smart_format: bool = True,
         model: DeepgramModels = "nova-2-general",
         api_key: str | None = None,
-        min_silence_duration: int = 100,  # 100ms for a RTC app seems like a strong default
+        min_silence_duration: int = 0,
     ) -> None:
         super().__init__(streaming_supported=True)
         api_key = api_key or os.environ.get("DEEPGRAM_API_KEY")
         if api_key is None:
             raise ValueError("Deepgram API key is required")
         self._api_key = api_key
 
-        self._config = STTOptions(
+        self._opts = STTOptions(
             language=language,
             detect_language=detect_language,
             interim_results=interim_results,
             punctuate=punctuate,
             model=model,
             smart_format=smart_format,
             endpointing=min_silence_duration,
@@ -128,68 +128,62 @@
         return SpeechStream(config, api_key=self._api_key)
 
     def _sanitize_options(
         self,
         *,
         language: str | None = None,
     ) -> STTOptions:
-        config = dataclasses.replace(self._config)
+        config = dataclasses.replace(self._opts)
         config.language = language or config.language
 
         if config.detect_language:
             config.language = None
 
         return config
 
 
 class SpeechStream(stt.SpeechStream):
     _KEEPALIVE_MSG: str = json.dumps({"type": "KeepAlive"})
     _CLOSE_MSG: str = json.dumps({"type": "CloseStream"})
 
     def __init__(
         self,
-        config: STTOptions,
+        opts: STTOptions,
         api_key: str,
         sample_rate: int = 16000,
         num_channels: int = 1,
         max_retry: int = 32,
     ) -> None:
         super().__init__()
 
-        if config.language is None:
+        if opts.detect_language and opts.language is None:
             raise ValueError("language detection is not supported in streaming mode")
 
-        self._config = config
+        self._opts = opts
         self._sample_rate = sample_rate
         self._num_channels = num_channels
         self._api_key = api_key
         self._speaking = False
 
         self._session = aiohttp.ClientSession()
         self._queue = asyncio.Queue[rtc.AudioFrame | str]()
         self._event_queue = asyncio.Queue[stt.SpeechEvent | None]()
         self._closed = False
         self._main_task = asyncio.create_task(self._run(max_retry))
 
         # keep a list of final transcripts to combine them inside the END_OF_SPEECH event
         self._final_events: List[stt.SpeechEvent] = []
 
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logging.error(f"deepgram task failed: {task.exception()}")
-
-        self._main_task.add_done_callback(log_exception)
-
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         if self._closed:
             raise ValueError("cannot push frame to closed stream")
 
         self._queue.put_nowait(frame)
 
-    async def aclose(self, wait: bool = True) -> None:
+    async def aclose(self, *, wait: bool = True) -> None:
         self._closed = True
         self._queue.put_nowait(SpeechStream._CLOSE_MSG)
 
         if not wait:
             self._main_task.cancel()
 
         with suppress(asyncio.CancelledError):
@@ -204,52 +198,52 @@
         """
 
         try:
             retry_count = 0
             while not self._closed:
                 try:
                     live_config = {
-                        "model": self._config.model,
-                        "punctuate": self._config.punctuate,
-                        "smart_format": self._config.smart_format,
-                        "interim_results": self._config.interim_results,
+                        "model": self._opts.model,
+                        "punctuate": self._opts.punctuate,
+                        "smart_format": self._opts.smart_format,
+                        "interim_results": self._opts.interim_results,
                         "encoding": "linear16",
                         "sample_rate": self._sample_rate,
                         "vad_events": True,
                         "channels": self._num_channels,
-                        "endpointing": self._config.endpointing,
+                        "endpointing": self._opts.endpointing,
                     }
 
-                    if self._config.language:
-                        live_config["language"] = self._config.language
+                    if self._opts.language:
+                        live_config["language"] = self._opts.language
 
                     headers = {"Authorization": f"Token {self._api_key}"}
 
                     url = f"wss://api.deepgram.com/v1/listen?{urlencode(live_config).lower()}"
                     ws = await self._session.ws_connect(url, headers=headers)
                     retry_count = 0  # connected successfully, reset the retry_count
 
                     await self._run_ws(ws)
-                except Exception as e:
+                except Exception:
                     # Something went wrong, retry the connection
                     if retry_count >= max_retry:
-                        logging.error(
-                            f"failed to connect to deepgram after {max_retry} tries",
-                            exc_info=e,
+                        logger.exception(
+                            f"failed to connect to deepgram after {max_retry} tries"
                         )
                         break
 
                     retry_delay = min(retry_count * 2, 10)  # max 10s
                     retry_count += 1  # increment after calculating the delay, the first retry should happen directly
 
-                    logging.warning(
-                        f"deepgram connection failed, retrying in {retry_delay}s",
-                        exc_info=e,
+                    logger.warning(
+                        f"deepgram connection failed, retrying in {retry_delay}s"
                     )
                     await asyncio.sleep(retry_delay)
+        except Exception:
+            logger.exception("deepgram task failed")
         finally:
             self._event_queue.put_nowait(None)
 
     async def _run_ws(self, ws: aiohttp.ClientWebSocketResponse) -> None:
         """
         This method can throw ws errors, these are handled inside the _run method
         """
@@ -301,66 +295,66 @@
                         return
 
                     raise Exception(
                         "deepgram connection closed unexpectedly"
                     )  # this will trigger a reconnection, see the _run loop
 
                 if msg.type != aiohttp.WSMsgType.TEXT:
-                    logging.warning("unexpected deepgram message type %s", msg.type)
+                    logger.warning("unexpected deepgram message type %s", msg.type)
                     continue
 
                 try:
                     # received a message from deepgram
                     data = json.loads(msg.data)
                     self._process_stream_event(data)
-                except Exception as e:
-                    logging.error(f"failed to process deepgram message: {e}")
+                except Exception:
+                    logger.exception("failed to process deepgram message")
 
         await asyncio.gather(send_task(), recv_task(), keepalive_task())
 
     def _end_speech(self) -> None:
         if not self._speaking:
-            logging.warning(
+            logger.warning(
                 "trying to commit final events without being in the speaking state"
             )
             return
 
         if len(self._final_events) == 0:
-            logging.warning("received end of speech without any final transcription")
             return
 
         self._speaking = False
 
         # combine all final transcripts since the start of the speech
         sentence = ""
         confidence = 0.0
-        for alt in self._final_events:
-            sentence += f"{alt.alternatives[0].text.strip()} "
-            confidence += alt.alternatives[0].confidence
+        for f in self._final_events:
+            alt = f.alternatives[0]
+            sentence += f"{alt.text.strip()} "
+            confidence += alt.confidence
 
         sentence = sentence.rstrip()
         confidence /= len(self._final_events)  # avg. of confidence
 
         end_event = stt.SpeechEvent(
             type=stt.SpeechEventType.END_OF_SPEECH,
             alternatives=[
                 stt.SpeechData(
-                    language=str(self._config.language),
+                    language=str(self._opts.language),
                     start_time=self._final_events[0].alternatives[0].start_time,
                     end_time=self._final_events[-1].alternatives[0].end_time,
                     confidence=confidence,
                     text=sentence,
                 )
             ],
         )
         self._event_queue.put_nowait(end_event)
         self._final_events = []
 
     def _process_stream_event(self, data: dict) -> None:
-        assert self._config.language is not None
+        assert self._opts.language is not None
 
         if data["type"] == "SpeechStarted":
             # This is a normal case. Deepgram's SpeechStarted events
             # are not correlated with speech_final or utterance end.
             # It's poossible that we receive two in a row without an endpoint
             # It's also possible we receive a transcript without a SpeechStarted event.
             if self._speaking:
@@ -373,46 +367,49 @@
         # see this page:
         # https://developers.deepgram.com/docs/understand-endpointing-interim-results#using-endpointing-speech_final
         # for more information about the different types of events
         elif data["type"] == "Results":
             is_final_transcript = data["is_final"]
             is_endpoint = data["speech_final"]
 
-            alts = live_transcription_to_speech_data(self._config.language, data)
+            alts = live_transcription_to_speech_data(self._opts.language, data)
             # If, for some reason, we didn't get a SpeechStarted event but we got
             # a transcript with text, we should start speaking. It's rare but has
             # been observed.
-            if not self._speaking and len(alts) and alts[0].text.strip() != "":
-                self._speaking = True
-                start_event = stt.SpeechEvent(type=stt.SpeechEventType.START_OF_SPEECH)
-                self._event_queue.put_nowait(start_event)
-
-            if is_final_transcript:
-                final_event = stt.SpeechEvent(
-                    type=stt.SpeechEventType.FINAL_TRANSCRIPT,
-                    alternatives=alts,
-                )
-                self._final_events.append(final_event)
-                self._event_queue.put_nowait(final_event)
-            else:
-                interim_event = stt.SpeechEvent(
-                    type=stt.SpeechEventType.INTERIM_TRANSCRIPT,
-                    alternatives=alts,
-                )
-                self._event_queue.put_nowait(interim_event)
+            if len(alts) > 0 and alts[0].text:
+                if not self._speaking:
+                    self._speaking = True
+                    start_event = stt.SpeechEvent(
+                        type=stt.SpeechEventType.START_OF_SPEECH
+                    )
+                    self._event_queue.put_nowait(start_event)
+
+                if is_final_transcript:
+                    final_event = stt.SpeechEvent(
+                        type=stt.SpeechEventType.FINAL_TRANSCRIPT,
+                        alternatives=alts,
+                    )
+                    self._final_events.append(final_event)
+                    self._event_queue.put_nowait(final_event)
+                else:
+                    interim_event = stt.SpeechEvent(
+                        type=stt.SpeechEventType.INTERIM_TRANSCRIPT,
+                        alternatives=alts,
+                    )
+                    self._event_queue.put_nowait(interim_event)
 
             # if we receive an endpoint, only end the speech if
             # we either had a SpeechStarted event or we have a seen
             # a non-empty transcript
             if is_endpoint and self._speaking:
                 self._end_speech()
         elif data["type"] == "Metadata":
             pass
         else:
-            logging.warning("received unexpected message from deepgram %s", data)
+            logger.warning("received unexpected message from deepgram %s", data)
 
     async def __anext__(self) -> stt.SpeechEvent:
         evt = await self._event_queue.get()
         if evt is None:
             raise StopAsyncIteration
 
         return evt
```

### Comparing `livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/version.py` & `livekit_plugins_deepgram-0.4.dev0/livekit/plugins/deepgram/version.py`

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

### Comparing `livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO` & `livekit_plugins_deepgram-0.4.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
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
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit-plugins-deepgram-0.3.dev0/setup.py` & `livekit_plugins_deepgram-0.4.dev0/setup.py`

 * *Files 5% similar despite different names*

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
         "aiohttp >= 3.7.4",
     ],
     package_data={
         "livekit.plugins.deepgram": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

