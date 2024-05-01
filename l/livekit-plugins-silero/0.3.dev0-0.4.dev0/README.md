# Comparing `tmp/livekit-plugins-silero-0.3.dev0.tar.gz` & `tmp/livekit_plugins_silero-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-silero-0.3.dev0.tar", last modified: Thu Apr 11 22:03:55 2024, max compression
+gzip compressed data, was "livekit_plugins_silero-0.4.dev0.tar", last modified: Wed May  1 00:22:47 2024, max compression
```

## Comparing `livekit-plugins-silero-0.3.dev0.tar` & `livekit_plugins_silero-0.4.dev0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:47.000000 livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:47.213093 livekit_plugins_silero-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-01 00:22:32.000000 livekit_plugins_silero-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-silero-0.3.dev0/PKG-INFO` & `livekit_plugins_silero-0.4.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 Requires-Dist: torch<3,>=2
 Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
 Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
```

### Comparing `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/__init__.py` & `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,11 +25,12 @@
     def __init__(self):
         super().__init__(__name__, __version__, __package__)
 
     def download_files(self):
         _ = torch.hub.load(
             repo_or_dir="snakers4/silero-vad",
             model="silero_vad",
+            use_onnx=True,
         )
 
 
 Plugin.register_plugin(SileroPlugin())
```

### Comparing `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/vad.py` & `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/vad.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,47 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
-import logging
+import time
 from collections import deque
-from typing import List, Optional
+from typing import List
 
 import numpy as np
 import torch
 from livekit import agents, rtc
 
+from .log import logger
+
 
 class VAD(agents.vad.VAD):
-    def __init__(
-        self, *, model_path: Optional[str] = None, use_onnx: bool = True
-    ) -> None:
+    def __init__(self, *, model_path: str | None = None, use_onnx: bool = True) -> None:
         if model_path:
             model = torch.jit.load(model_path)
             model.eval()
         else:
             model, _ = torch.hub.load(
                 repo_or_dir="snakers4/silero-vad",
                 model="silero_vad",
                 onnx=use_onnx,
             )
         self._model = model
 
     def stream(
         self,
         *,
-        min_speaking_duration: float = 0.5,
-        min_silence_duration: float = 0.5,
+        min_speaking_duration: float = 0.2,
+        min_silence_duration: float = 0.8,
         padding_duration: float = 0.1,
         sample_rate: int = 16000,
         max_buffered_speech: float = 45.0,
-        threshold: float = 0.5,
+        threshold: float = 0.2,
     ) -> "VADStream":
         return VADStream(
             self._model,
             min_speaking_duration=min_speaking_duration,
             min_silence_duration=min_silence_duration,
             padding_duration=padding_duration,
             sample_rate=sample_rate,
@@ -89,30 +89,25 @@
         self._model = model
 
         self._closed = False
         self._speaking = False
         self._waiting_start = False
         self._waiting_end = False
         self._current_sample = 0
+        self._filter = agents.utils.ExpFilter(0.8)
         self._min_speaking_samples = min_speaking_duration * sample_rate
         self._min_silence_samples = min_silence_duration * sample_rate
         self._padding_duration_samples = padding_duration * sample_rate
         self._max_buffered_samples = max_buffered_speech * sample_rate
 
         self._queued_frames: deque[rtc.AudioFrame] = deque()
         self._original_frames: deque[rtc.AudioFrame] = deque()
         self._buffered_frames: List[rtc.AudioFrame] = []
         self._main_task = asyncio.create_task(self._run())
 
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logging.error(f"silero vad task failed: {task.exception()}")
-
-        self._main_task.add_done_callback(log_exception)
-
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         if self._closed:
             raise ValueError("cannot push frame to closed stream")
 
         self._queue.put_nowait(frame)
 
     async def aclose(self, *, wait: bool = True) -> None:
@@ -147,14 +142,17 @@
                     )
 
                     samples_40ms = self._sample_rate // 1000 * 40
                     if available_length < samples_40ms:
                         break
 
                     await asyncio.shield(self._run_inference())
+
+        except Exception:
+            logger.exception("silero stream failed")
         finally:
             self._event_queue.put_nowait(None)
 
     async def _run_inference(self) -> None:
         # merge the first 4 frames (we know each is 10ms)
         if len(self._queued_frames) < 4:
             return
@@ -165,21 +163,41 @@
         )
 
         # convert data_40ms to tensor & f32
         tensor = torch.from_numpy(np.frombuffer(merged_frame.data, dtype=np.int16))
         tensor = tensor.to(torch.float32) / 32768.0
 
         # run inference
-        speech_prob = await asyncio.to_thread(
+        start_time = time.time()
+        raw_prob = await asyncio.to_thread(
             lambda: self._model(tensor, self._sample_rate).item()
         )
-        self._dispatch_event(speech_prob, original_frames)
+        probability = self._filter.apply(1.0, raw_prob)
+        inference_duration = time.time() - start_time
+
+        # inference done
+        event = agents.vad.VADEvent(
+            type=agents.vad.VADEventType.INFERENCE_DONE,
+            samples_index=self._current_sample,
+            probability=probability,
+            raw_inference_prob=raw_prob,
+            inference_duration=inference_duration,
+        )
+        self._event_queue.put_nowait(event)
+
+        self._dispatch_event(original_frames, probability, raw_prob, inference_duration)
         self._current_sample += merged_frame.samples_per_channel
 
-    def _dispatch_event(self, speech_prob: int, original_frames: List[rtc.AudioFrame]):
+    def _dispatch_event(
+        self,
+        original_frames: List[rtc.AudioFrame],
+        probability: float,
+        raw_inference_prob: float,
+        inference_duration: float,
+    ):
         """
         Dispatches a VAD event based on the speech probability and the options
         Args:
             speech_prob: speech probability of the current frame
             original_frames: original frames of the current inference
         """
 
@@ -199,79 +217,73 @@
             ]
 
         max_buffer_len = padding_count + max(
             int(self._max_buffered_samples // samples_10ms),
             int(self._min_speaking_samples // samples_10ms),
         )
         if len(self._buffered_frames) > max_buffer_len:
-            # if unaware of this, may be hard to debug, so logging seems ok here
-            logging.warning(
-                f"VAD buffer overflow, dropping {len(self._buffered_frames) - max_buffer_len} frames"
-            )
             self._buffered_frames = self._buffered_frames[
                 len(self._buffered_frames) - max_buffer_len :
             ]
 
-        if speech_prob >= self._threshold:
+        if probability >= self._threshold:
             # speaking, wait for min_speaking_duration to trigger START_OF_SPEECH
             self._waiting_end = False
             if not self._waiting_start and not self._speaking:
                 self._waiting_start = True
                 self._start_speech = self._current_sample
 
             if self._waiting_start and (
                 self._current_sample - self._start_speech >= self._min_speaking_samples
             ):
                 self._waiting_start = False
                 self._speaking = True
-                event = agents.vad.VADEvent(
-                    type=agents.vad.VADEventType.START_OF_SPEECH,
-                    samples_index=self._start_speech,
-                )
-                self._event_queue.put_nowait(event)
 
                 # since we're waiting for the min_spaking_duration to trigger START_OF_SPEECH,
-                # the SPEAKING data is missing the first few frames, trigger it here
-                # TODO(theomonnom): Maybe it is better to put the data inside the START_OF_SPEECH event?
+                # put the speech that were used to trigger the start here
                 event = agents.vad.VADEvent(
-                    type=agents.vad.VADEventType.SPEAKING,
+                    type=agents.vad.VADEventType.START_OF_SPEECH,
                     samples_index=self._start_speech,
-                    speech=self._buffered_frames[padding_count:],
+                    frames=self._buffered_frames[padding_count:],
+                    speaking=True,
                 )
+                self._event_queue.put_nowait(event)
 
-                return
-
-        if self._speaking:
-            # we don't check the speech_prob here
-            event = agents.vad.VADEvent(
-                type=agents.vad.VADEventType.SPEAKING,
-                samples_index=self._current_sample,
-                speech=original_frames,
-            )
-            self._event_queue.put_nowait(event)
+        # we don't check the speech_prob here
+        event = agents.vad.VADEvent(
+            type=agents.vad.VADEventType.INFERENCE_DONE,
+            samples_index=self._current_sample,
+            frames=original_frames,
+            probability=probability,
+            raw_inference_prob=raw_inference_prob,
+            inference_duration=inference_duration,
+            speaking=self._speaking,
+        )
+        self._event_queue.put_nowait(event)
 
-        if speech_prob < self._threshold:
-            # stopped speaking, wait for min_silence_duration to trigger END_OF_SPEECH,
+        if probability < self._threshold:
+            # stopped speaking, s for min_silence_duration to trigger END_OF_SPEECH,
             self._waiting_start = False
             if not self._waiting_end and self._speaking:
                 self._waiting_end = True
                 self._end_speech = self._current_sample
 
             if self._waiting_end and (
                 self._current_sample - self._end_speech
                 >= max(self._min_silence_samples, self._padding_duration_samples)
             ):
                 self._waiting_end = False
                 self._speaking = False
                 event = agents.vad.VADEvent(
                     type=agents.vad.VADEventType.END_OF_SPEECH,
                     samples_index=self._end_speech,
-                    duration=(self._current_sample - self._start_speech)
+                    duration=(self._end_speech - self._start_speech)
                     / self._sample_rate,
-                    speech=self._buffered_frames,
+                    frames=self._buffered_frames,
+                    speaking=False,
                 )
                 self._event_queue.put_nowait(event)
 
     async def __anext__(self) -> agents.vad.VADEvent:
         evt = await self._event_queue.get()
         if evt is None:
             raise StopAsyncIteration
```

### Comparing `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/version.py` & `livekit_plugins_silero-0.4.dev0/livekit/plugins/silero/version.py`

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

### Comparing `livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/PKG-INFO` & `livekit_plugins_silero-0.4.dev0/livekit_plugins_silero.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 Requires-Dist: torch<3,>=2
 Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
 Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
```

### Comparing `livekit-plugins-silero-0.3.dev0/setup.py` & `livekit_plugins_silero-0.4.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.8.0",
     install_requires=[
-        "livekit ~= 0.9",
-        "livekit-agents~=0.5.dev0",
+        "livekit ~= 0.11",
+        "livekit-agents~=0.6.dev0",
         "torch >= 2, < 3",
         "torchaudio >= 2",
         "numpy >= 1, < 2",
         "onnxruntime~=1.17.0",
     ],
     package_data={"livekit.plugins.silero": ["files/silero_vad.jit"]},
     project_urls={
```

