# Comparing `tmp/livekit-plugins-nltk-0.4.dev0.tar.gz` & `tmp/livekit_plugins_nltk-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-nltk-0.4.dev0.tar", last modified: Thu Apr 11 22:03:41 2024, max compression
+gzip compressed data, was "livekit_plugins_nltk-0.5.dev0.tar", last modified: Wed May  1 00:22:26 2024, max compression
```

## Comparing `livekit-plugins-nltk-0.4.dev0.tar` & `livekit_plugins_nltk-0.5.dev0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/sentence_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 00:22:26.000000 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-01 00:22:26.000000 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:26.000000 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 00:22:26.000000 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:26.000000 livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:26.882033 livekit_plugins_nltk-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-01 00:22:22.000000 livekit_plugins_nltk-0.5.dev0/setup.py
```

### Comparing `livekit-plugins-nltk-0.4.dev0/PKG-INFO` & `livekit_plugins_nltk-0.5.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.4.dev0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -14,17 +14,17 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
+Requires-Dist: livekit~=0.11
 Requires-Dist: nltk<4,>=3
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit-agents~=0.6.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py` & `livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py` & `livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/sentence_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 import dataclasses
-import logging
 from dataclasses import dataclass
 from typing import List, Optional
 
 from livekit import agents
 
 import nltk  # type: ignore
 
+from .log import logger
+
 # nltk is using the punkt tokenizer
 # https://www.nltk.org/_modules/nltk/tokenize/punkt.html
 # this code is using a whitespace to concatenate small sentences together
 # (languages such as Chinese and Japanese are not yet supported)
 
 
 @dataclass
@@ -85,15 +86,15 @@
         self._closed = False
 
         self._incomplete_sentences: List[str] = []  # <= min_sentence_len
         self._buffer = ""
 
     def push_text(self, text: str) -> None:
         if self._closed:
-            logging.error("Cannot push text to closed stream")
+            logger.error("Cannot push text to closed stream")
             return
 
         for char in text:
             self._buffer += char
 
             if len(self._buffer) < self._context_len:
                 continue
```

### Comparing `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py` & `livekit_plugins_nltk-0.5.dev0/livekit/plugins/nltk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.dev0"
+__version__ = "0.5.dev0"
```

### Comparing `livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO` & `livekit_plugins_nltk-0.5.dev0/livekit_plugins_nltk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.4.dev0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -14,17 +14,17 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit~=0.9
+Requires-Dist: livekit~=0.11
 Requires-Dist: nltk<4,>=3
-Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: livekit-agents~=0.6.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit-plugins-nltk-0.4.dev0/setup.py` & `livekit_plugins_nltk-0.5.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
-        "livekit~=0.9",
+        "livekit~=0.11",
         "nltk >= 3, < 4",
-        "livekit-agents~=0.5.dev0",
+        "livekit-agents~=0.6.dev0",
     ],
     package_data={
         "livekit.plugins.nltk": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

