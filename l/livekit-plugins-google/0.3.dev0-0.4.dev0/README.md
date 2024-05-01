# Comparing `tmp/livekit-plugins-google-0.3.dev0.tar.gz` & `tmp/livekit_plugins_google-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-google-0.3.dev0.tar", last modified: Thu Apr 11 22:03:37 2024, max compression
+gzip compressed data, was "livekit_plugins_google-0.4.dev0.tar", last modified: Wed May  1 00:22:21 2024, max compression
```

## Comparing `livekit-plugins-google-0.3.dev0.tar` & `livekit_plugins_google-0.4.dev0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.729574 livekit-plugins-google-0.3.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.729574 livekit-plugins-google-0.3.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/livekit/plugins/google/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:21.451394 livekit_plugins_google-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/livekit/plugins/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/livekit/plugins/google/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-01 00:22:21.000000 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 00:22:21.000000 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:21.000000 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 00:22:21.000000 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:21.000000 livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:21.455394 livekit_plugins_google-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-01 00:22:17.000000 livekit_plugins_google-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-google-0.3.dev0/PKG-INFO` & `livekit_plugins_google-0.4.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -25,16 +25,16 @@
 Requires-Dist: google-api-core<3,>=2
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
-Requires-Dist: livekit>=0.9.2
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit-plugins-google-0.3.dev0/README.md` & `livekit_plugins_google-0.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `livekit-plugins-google-0.3.dev0/livekit/plugins/google/__init__.py` & `livekit_plugins_google-0.4.dev0/livekit/plugins/google/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-google-0.3.dev0/livekit/plugins/google/models.py` & `livekit_plugins_google-0.4.dev0/livekit/plugins/google/models.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-google-0.3.dev0/livekit/plugins/google/stt.py` & `livekit_plugins_google-0.4.dev0/livekit/plugins/google/stt.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import dataclasses
-import logging
 from dataclasses import dataclass
 from typing import Any, AsyncIterable, Dict, List
 
 from livekit import agents, rtc
 from livekit.agents import stt
 from livekit.agents.utils import AudioBuffer
 
 from google.auth import credentials  # type: ignore
 from google.cloud.speech_v2 import SpeechAsyncClient
 from google.cloud.speech_v2.types import cloud_speech
 
+from .log import logger
 from .models import SpeechLanguages, SpeechModels
 
 LgType = SpeechLanguages | str
 LanguageCode = LgType | List[LgType]
 
 
 # This class is only be used internally to encapsulate the options
@@ -101,15 +101,15 @@
         if language:
             config.languages = [language]
 
         if not isinstance(config.languages, list):
             config.languages = [config.languages]
         elif not config.detect_language:
             if len(config.languages) > 1:
-                logging.warning(
+                logger.warning(
                     "multiple languages provided, but language detection is disabled"
                 )
             config.languages = [config.languages[0]]
 
         return config
 
     async def recognize(
@@ -204,15 +204,15 @@
                 enable_voice_activity_events=True,
                 interim_results=self._config.interim_results,
             ),
         )
 
         def log_exception(task: asyncio.Task) -> None:
             if not task.cancelled() and task.exception():
-                logging.error(f"google stt task failed: {task.exception()}")
+                logger.error(f"google stt task failed: {task.exception()}")
 
         self._main_task.add_done_callback(log_exception)
 
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         if self._closed:
             raise ValueError("cannot push frame to closed stream")
 
@@ -252,36 +252,36 @@
                                 frame = frame.remix_and_resample(
                                     self._sample_rate, self._num_channels
                                 )
                                 yield cloud_speech.StreamingRecognizeRequest(
                                     audio=frame.data.tobytes(),
                                 )
                         except Exception as e:
-                            logging.error(
+                            logger.error(
                                 f"an error occurred while streaming inputs: {e}"
                             )
 
                     # try to connect
                     stream = await self._client.streaming_recognize(
                         requests=input_generator()
                     )
                     retry_count = 0  # connection successful, reset retry count
 
                     await self._run_stream(stream)
                 except Exception as e:
                     if retry_count >= max_retry:
-                        logging.error(
+                        logger.error(
                             f"failed to connect to google stt after {max_retry} tries",
                             exc_info=e,
                         )
                         break
 
                     retry_delay = min(retry_count * 2, 10)  # max 10s
                     retry_count += 1
-                    logging.warning(
+                    logger.warning(
                         f"google stt connection failed, retrying in {retry_delay}s",
                         exc_info=e,
                     )
                     await asyncio.sleep(retry_delay)
         finally:
             self._event_queue.put_nowait(None)
```

### Comparing `livekit-plugins-google-0.3.dev0/livekit/plugins/google/version.py` & `livekit_plugins_google-0.4.dev0/livekit/plugins/google/version.py`

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

### Comparing `livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/PKG-INFO` & `livekit_plugins_google-0.4.dev0/livekit_plugins_google.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.3.dev0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -25,16 +25,16 @@
 Requires-Dist: google-api-core<3,>=2
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
-Requires-Dist: livekit>=0.9.2
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit~=0.11
+Requires-Dist: livekit-agents~=0.6.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit-plugins-google-0.3.dev0/setup.py` & `livekit_plugins_google-0.4.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         "google-api-core >= 2, < 3",
         "google-auth >= 2, < 3",
         "google-cloud-core >= 2, < 3",
         "google-cloud-speech >= 2, < 3",
         "google-cloud-texttospeech >= 2, < 3",
         "google-cloud-translate >= 3, < 4",
         "googleapis-common-protos >= 1, < 2",
-        "livekit >= 0.9.2",
-        "livekit-agents~=0.5.dev0",
+        "livekit ~= 0.11",
+        "livekit-agents~=0.6.dev0",
     ],
     package_data={
         "livekit.plugins.google": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

