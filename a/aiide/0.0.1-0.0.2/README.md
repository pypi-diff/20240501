# Comparing `tmp/aiide-0.0.1.tar.gz` & `tmp/aiide-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiide-0.0.1.tar", max compression
+gzip compressed data, was "aiide-0.0.2.tar", max compression
```

## Comparing `aiide-0.0.1.tar` & `aiide-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-30 21:07:58.276939 aiide-0.0.1/LICENSE
--rw-r--r--   0        0        0     6496 2024-04-30 21:02:41.580603 aiide-0.0.1/README.md
--rw-r--r--   0        0        0       69 2024-04-30 18:06:00.619503 aiide-0.0.1/aiide/__init__.py
--rw-r--r--   0        0        0     8655 2024-04-30 20:47:27.743547 aiide-0.0.1/aiide/_aiide.py
--rw-r--r--   0        0        0      716 2024-04-30 17:44:07.018305 aiide-0.0.1/aiide/_utils.py
--rw-r--r--   0        0        0       27 2024-04-30 17:41:28.404617 aiide-0.0.1/aiide/tools/__init__.py
--rw-r--r--   0        0        0     6557 2024-04-30 18:01:53.387520 aiide-0.0.1/aiide/tools/_definitions.py
--rw-r--r--   0        0        0      288 2024-04-30 21:03:26.707972 aiide-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6914 1970-01-01 00:00:00.000000 aiide-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 21:07:58.276939 aiide-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6748 2024-04-30 21:27:22.430997 aiide-0.0.2/README.md
+-rw-r--r--   0        0        0       69 2024-04-30 21:28:40.182777 aiide-0.0.2/aiide/__init__.py
+-rw-r--r--   0        0        0     8655 2024-04-30 20:47:27.743547 aiide-0.0.2/aiide/_aiide.py
+-rw-r--r--   0        0        0      716 2024-04-30 17:44:07.018305 aiide-0.0.2/aiide/_utils.py
+-rw-r--r--   0        0        0       27 2024-04-30 17:41:28.404617 aiide-0.0.2/aiide/tools/__init__.py
+-rw-r--r--   0        0        0     6557 2024-04-30 18:01:53.387520 aiide-0.0.2/aiide/tools/_definitions.py
+-rw-r--r--   0        0        0      288 2024-04-30 21:28:26.891147 aiide-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7166 1970-01-01 00:00:00.000000 aiide-0.0.2/PKG-INFO
```

### Comparing `aiide-0.0.1/LICENSE` & `aiide-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiide-0.0.1/README.md` & `aiide-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 <div align="center"><picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/figures/logo_dark.svg">
-  <img alt="aiide" src="docs/figures/logo.svg" width=300">
+  <img alt="aiide" src="docs/figures/logo.svg" width=200">
 </picture></div>
 <br/>
 
 
-
-**`aiide`** is a LLM datastructure management library for providing a RL-type environment to the LLM. It allows you to declare live components(ENV), enable the LLM through tools to modify the ENV and provide the LLM with reward(as function response) and latest snapshot of the ENV.
+**`aiide`** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
 
 <div align="center"><picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_overview.png">
-  <img alt="guidance" src="docs/figures/aiide_overview.png" width=300">
+  <img alt="guidance" src="docs/figures/aiide_overview.png" width=700">
 </picture></div>
 <br/>
 
 ### Tutorial
 Let's build a simple form filling agent. We have a pandas dataframe with field names and we want the LLM to ask the user for answers to a couple of questions at a time and populate the said dataframe.
 
 Here
 * The environment is the dataframe
 * We need a single tool that enables the LLM to add or edit values for any of the fields
 * _The library will automatically provide the latest snapshot of the dataframe to the LLM.(aiide will automatically remove older snapshots of the dataframe from the LLM memory to avoid confusing it and saving tokens)_
 
+0. Install the package<br/>
+`pip install aiide`
+
 1. Let's start with defining a simple chat agent
 
 ```python
 # Import the AIIDE class
 from aiide import AIIDE
 # Import helper classes for defining functions for the LLM
 from aiide.tools import TOOL_DEF, INT, FLOAT, STR, BOOL, LIST, DICT
```

### Comparing `aiide-0.0.1/aiide/_aiide.py` & `aiide-0.0.2/aiide/_aiide.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.1/aiide/_utils.py` & `aiide-0.0.2/aiide/_utils.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.1/aiide/tools/_definitions.py` & `aiide-0.0.2/aiide/tools/_definitions.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.1/PKG-INFO` & `aiide-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: aiide
-Version: 0.0.1
+Version: 0.0.2
 Summary: Live components for your LLM
 Author: Anilturaga
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.24.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center"><picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/figures/logo_dark.svg">
-  <img alt="aiide" src="docs/figures/logo.svg" width=300">
+  <img alt="aiide" src="docs/figures/logo.svg" width=200">
 </picture></div>
 <br/>
 
 
-
-**`aiide`** is a LLM datastructure management library for providing a RL-type environment to the LLM. It allows you to declare live components(ENV), enable the LLM through tools to modify the ENV and provide the LLM with reward(as function response) and latest snapshot of the ENV.
+**`aiide`** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
 
 <div align="center"><picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_overview.png">
-  <img alt="guidance" src="docs/figures/aiide_overview.png" width=300">
+  <img alt="guidance" src="docs/figures/aiide_overview.png" width=700">
 </picture></div>
 <br/>
 
 ### Tutorial
 Let's build a simple form filling agent. We have a pandas dataframe with field names and we want the LLM to ask the user for answers to a couple of questions at a time and populate the said dataframe.
 
 Here
 * The environment is the dataframe
 * We need a single tool that enables the LLM to add or edit values for any of the fields
 * _The library will automatically provide the latest snapshot of the dataframe to the LLM.(aiide will automatically remove older snapshots of the dataframe from the LLM memory to avoid confusing it and saving tokens)_
 
+0. Install the package<br/>
+`pip install aiide`
+
 1. Let's start with defining a simple chat agent
 
 ```python
 # Import the AIIDE class
 from aiide import AIIDE
 # Import helper classes for defining functions for the LLM
 from aiide.tools import TOOL_DEF, INT, FLOAT, STR, BOOL, LIST, DICT
```

