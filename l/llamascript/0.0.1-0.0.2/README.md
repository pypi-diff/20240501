# Comparing `tmp/llamascript-0.0.1.tar.gz` & `tmp/llamascript-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.0.1.tar", last modified: Tue Apr 30 20:38:09 2024, max compression
+gzip compressed data, was "llamascript-0.0.2.tar", last modified: Tue Apr 30 23:16:31 2024, max compression
```

## Comparing `llamascript-0.0.1.tar` & `llamascript-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-30 20:38:09.609562 llamascript-0.0.1/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1162 2024-04-30 20:38:09.608875 llamascript-0.0.1/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      719 2024-04-30 20:26:55.000000 llamascript-0.0.1/README.md
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-30 20:38:09.604227 llamascript-0.0.1/llamascript/
--rw-r--r--   0 lewis-family   (501) staff       (20)     3254 2024-04-30 20:35:20.000000 llamascript-0.0.1/llamascript/__init__.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-30 20:38:09.607788 llamascript-0.0.1/llamascript.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1162 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      254 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       48 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/requires.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       12 2024-04-30 20:38:09.000000 llamascript-0.0.1/llamascript.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-30 20:38:09.609745 llamascript-0.0.1/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      739 2024-04-30 20:35:27.000000 llamascript-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:16:31.953312 llamascript-0.0.2/
+-rw-rw-rw-   0        0        0    11525 2024-04-30 21:46:58.000000 llamascript-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1208 2024-04-30 23:16:31.952311 llamascript-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2024-04-30 23:13:49.000000 llamascript-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 23:16:31.921310 llamascript-0.0.2/llamascript/
+-rw-rw-rw-   0        0        0     2621 2024-04-30 21:54:01.000000 llamascript-0.0.2/llamascript/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:16:31.949313 llamascript-0.0.2/llamascript.egg-info/
+-rw-rw-rw-   0        0        0     1208 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 23:16:31.000000 llamascript-0.0.2/llamascript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 23:16:31.953312 llamascript-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-04-30 23:14:02.000000 llamascript-0.0.2/setup.py
```

### Comparing `llamascript-0.0.1/PKG-INFO` & `llamascript-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-Metadata-Version: 2.1
-Name: llamascript
-Version: 0.0.1
-Summary: No-code AI chatbot using Ollama.
-Home-page: https://github.com/WolfTheDeveloper/llamascript
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: ollama
-
-# LlamaScript
-
-LlamaScript is a no-code AI chatbot using Ollama.
-
-## Installation
-
-You can install LlamaScript using pip:
-
-```bash
-pip install llamascript
-```
-
-## Usage
-To use LlamaScript, create a llama file (no file extension) with the following commands:
-
-```llamascript
-USE <model>: This command loads the specified model.
-PROMPT <message>: This command sets the message to be sent to the chatbot.
-CHAT: This command sends the message to the chatbot and prints the response.
-```
-
-Here's an example:
-
-```llamascript
-USE llama3
-PROMPT Hello, how are you?
-CHAT
-```
-
-You can then run LlamaScript with the following command:
-
-```bash
-llamascript
-```
-
-## License
-LlamaScript is licensed under the Apache 2.0 License.
-
-```
+Metadata-Version: 2.1
+Name: llamascript
+Version: 0.0.2
+Summary: No-code AI chatbot using Ollama.
+Home-page: https://github.com/WolfTheDeveloper/llamascript
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LlamaScript
+
+LlamaScript is a no-code AI chatbot using Ollama.
+
+## Installation
+
+You can install LlamaScript using pip:
+
+```bash
+pip install llamascript
+```
+
+## Usage
+To use LlamaScript, create a llama file (no file extension) with the following commands:
+
+```llamascript
+USE <model>: This command loads the specified model.
+PROMPT <message>: This command sets the message to be sent to the chatbot.
+CHAT: This command sends the message to the chatbot and prints the response.
+```
+
+Here's an example:
+
+```llamascript
+USE llama3
+PROMPT Hello, how are you?
+CHAT
+```
+
+You can then run LlamaScript with the following command:
+
+```bash
+llamascript
+```
+
+## License
+LlamaScript is licensed under the Apache 2.0 License.
```

### Comparing `llamascript-0.0.1/README.md` & `llamascript-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-# LlamaScript
-
-LlamaScript is a no-code AI chatbot using Ollama.
-
-## Installation
-
-You can install LlamaScript using pip:
-
-```bash
-pip install llamascript
-```
-
-## Usage
-To use LlamaScript, create a llama file (no file extension) with the following commands:
-
-```llamascript
-USE <model>: This command loads the specified model.
-PROMPT <message>: This command sets the message to be sent to the chatbot.
-CHAT: This command sends the message to the chatbot and prints the response.
-```
-
-Here's an example:
-
-```llamascript
-USE llama3
-PROMPT Hello, how are you?
-CHAT
-```
-
-You can then run LlamaScript with the following command:
-
-```bash
-llamascript
-```
-
-## License
-LlamaScript is licensed under the Apache 2.0 License.
-
-```
+# LlamaScript
+
+LlamaScript is a no-code AI chatbot using Ollama.
+
+## Installation
+
+You can install LlamaScript using pip:
+
+```bash
+pip install llamascript
+```
+
+## Usage
+To use LlamaScript, create a llama file (no file extension) with the following commands:
+
+```llamascript
+USE <model>: This command loads the specified model.
+PROMPT <message>: This command sets the message to be sent to the chatbot.
+CHAT: This command sends the message to the chatbot and prints the response.
+```
+
+Here's an example:
+
+```llamascript
+USE llama3
+PROMPT Hello, how are you?
+CHAT
+```
+
+You can then run LlamaScript with the following command:
+
+```bash
+llamascript
+```
+
+## License
+LlamaScript is licensed under the Apache 2.0 License.
```

### Comparing `llamascript-0.0.1/llamascript.egg-info/PKG-INFO` & `llamascript-0.0.2/llamascript.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-Metadata-Version: 2.1
-Name: llamascript
-Version: 0.0.1
-Summary: No-code AI chatbot using Ollama.
-Home-page: https://github.com/WolfTheDeveloper/llamascript
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: ollama
-
-# LlamaScript
-
-LlamaScript is a no-code AI chatbot using Ollama.
-
-## Installation
-
-You can install LlamaScript using pip:
-
-```bash
-pip install llamascript
-```
-
-## Usage
-To use LlamaScript, create a llama file (no file extension) with the following commands:
-
-```llamascript
-USE <model>: This command loads the specified model.
-PROMPT <message>: This command sets the message to be sent to the chatbot.
-CHAT: This command sends the message to the chatbot and prints the response.
-```
-
-Here's an example:
-
-```llamascript
-USE llama3
-PROMPT Hello, how are you?
-CHAT
-```
-
-You can then run LlamaScript with the following command:
-
-```bash
-llamascript
-```
-
-## License
-LlamaScript is licensed under the Apache 2.0 License.
-
-```
+Metadata-Version: 2.1
+Name: llamascript
+Version: 0.0.2
+Summary: No-code AI chatbot using Ollama.
+Home-page: https://github.com/WolfTheDeveloper/llamascript
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LlamaScript
+
+LlamaScript is a no-code AI chatbot using Ollama.
+
+## Installation
+
+You can install LlamaScript using pip:
+
+```bash
+pip install llamascript
+```
+
+## Usage
+To use LlamaScript, create a llama file (no file extension) with the following commands:
+
+```llamascript
+USE <model>: This command loads the specified model.
+PROMPT <message>: This command sets the message to be sent to the chatbot.
+CHAT: This command sends the message to the chatbot and prints the response.
+```
+
+Here's an example:
+
+```llamascript
+USE llama3
+PROMPT Hello, how are you?
+CHAT
+```
+
+You can then run LlamaScript with the following command:
+
+```bash
+llamascript
+```
+
+## License
+LlamaScript is licensed under the Apache 2.0 License.
```

