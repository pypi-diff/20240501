# Comparing `tmp/agentkit-llm-0.1.6.post1.tar.gz` & `tmp/agentkit-llm-0.1.6.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.6.post1.tar", last modified: Fri Apr 26 20:04:13 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.6.post2.tar", last modified: Wed May  1 19:52:12 2024, max compression
```

## Comparing `agentkit-llm-0.1.6.post1.tar` & `agentkit-llm-0.1.6.post2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6.post1/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8525 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8035 2024-04-26 20:02:45.000000 agentkit-llm-0.1.6.post1/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1001 2024-04-26 20:03:26.000000 agentkit-llm-0.1.6.post1/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.390998 agentkit-llm-0.1.6.post1/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6.post1/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.6.post1/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6.post1/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6.post1/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6.post1/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6.post1/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5142 2024-04-24 17:42:15.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6.post1/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6.post1/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6.post1/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6.post1/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-26 20:04:13.394998 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     8525 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-26 20:04:13.000000 agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6.post2/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8525 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8035 2024-04-26 20:02:45.000000 agentkit-llm-0.1.6.post2/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1001 2024-05-01 19:52:07.000000 agentkit-llm-0.1.6.post2/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.248815 agentkit-llm-0.1.6.post2/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6.post2/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.6.post2/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6.post2/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6.post2/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6.post2/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6.post2/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-01 19:51:25.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6.post2/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6.post2/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6.post2/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     8525 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.6.post1/LICENSE` & `agentkit-llm-0.1.6.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/PKG-INFO` & `agentkit-llm-0.1.6.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6.post1
+Version: 0.1.6.post2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.6.post1/README.md` & `agentkit-llm-0.1.6.post2/README.md`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/setup.py` & `agentkit-llm-0.1.6.post2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.6.post1"
+VERSION = "0.1.6.post2"
 EXTRAS = {
     "logging": ["wandb"],
     "all": ["wandb", "openai", "anthropic", "tiktoken"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
```

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/after_query.py` & `agentkit-llm-0.1.6.post2/src/agentkit/after_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 class BaseAfterQuery:
     """Base class for after query postprocessing.
 
     Each after query instance performs postprocessing after the LLM query.
 
     Attributes:
-        node (BaseNode): Node object.
+        node (SimpleDBNode): The Node object that this after-query instance is associated with.
     """
 
     def __init__(self):
         self.node = None
     
     def set_node(self, node):
         """Set the node for the after query.
 
+        This function will be called automatically upon initialization of a SimpleDBNode
+
         Args:
-            node (BaseNode): Node object.
+            node (SimpleDBNode): Node object.
         """
         self.node = node
         return self
     
     def post_process(self):
         """Post process the result of the LLM query.
```

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/base_node.py` & `agentkit-llm-0.1.6.post2/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.6.post2/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/exceptions.py` & `agentkit-llm-0.1.6.post2/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/graph.py` & `agentkit-llm-0.1.6.post2/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/GPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,28 +77,20 @@
         return self.enc_fn.decode(txt)
 
     def query_chat(self, messages, shrink_idx, max_gen=512, temp=0.):
         model_max = self.model_max
         messages = self.shrink_msg(messages, shrink_idx, model_max-max_gen)
         while(True):
             try:
-                if isinstance(client, OpenAI):
-                    completion = client.chat.completions.create(
-                        model=self.name,
-                        messages=messages,
-                        temperature=temp,
-                        max_tokens=max_gen,
-                    )
-                elif isinstance(client, AzureOpenAI):
-                    completion = client.completions.create(
-                        model=deployment_name,
-                        messages=messages,
-                        temperature=temp,
-                        max_tokens=max_gen,
-                    )
+                completion = client.chat.completions.create(
+                    model=deployment_name if deployment_name else self.name,
+                    messages=messages,
+                    temperature=temp,
+                    max_tokens=max_gen,
+                )
                 return completion.choices[0].message.content, {"prompt":completion.usage.prompt_tokens, "completion":completion.usage.completion_tokens, "total":completion.usage.total_tokens}
             except Exception as e:
                 if self.debug:
                     raise e
                 elif isinstance(e, openai.RateLimitError) or isinstance(e, openai.APIStatusError) or isinstance(e, openai.APITimeoutError) or isinstance(e, openai.APIConnectionError) or isinstance(e, openai.InternalServerError):
                     time.sleep(30)
                     print(e)
```

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/node.py` & `agentkit-llm-0.1.6.post2/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit/utils.py` & `agentkit-llm-0.1.6.post2/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6.post1
+Version: 0.1.6.post2
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.6.post1/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

