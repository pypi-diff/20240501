# Comparing `tmp/cntrlai-0.0.33.tar.gz` & `tmp/cntrlai-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cntrlai-0.0.33.tar", max compression
+gzip compressed data, was "cntrlai-0.0.34.tar", max compression
```

## Comparing `cntrlai-0.0.33.tar` & `cntrlai-0.0.34.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        6 2024-04-27 00:39:09.943029 cntrlai-0.0.33/README.md
--rw-r--r--   0        0        0      284 2024-04-29 00:59:20.632041 cntrlai-0.0.33/cntrlai/__init__.py
--rw-r--r--   0        0        0     7579 2024-04-29 00:59:54.678362 cntrlai-0.0.33/cntrlai/batch_evaluation.py
--rw-r--r--   0        0        0     3401 2024-04-29 01:00:28.289059 cntrlai-0.0.33/cntrlai/guardrails.py
--rw-r--r--   0        0        0    11044 2024-04-29 01:04:56.414065 cntrlai-0.0.33/cntrlai/langchain.py
--rw-r--r--   0        0        0     8710 2024-04-29 05:35:40.848340 cntrlai-0.0.33/cntrlai/logger.py
--rw-r--r--   0        0        0    20766 2024-04-29 05:35:35.729115 cntrlai-0.0.33/cntrlai/openai.py
--rw-r--r--   0        0        0     3588 2024-04-29 01:05:54.216065 cntrlai-0.0.33/cntrlai/types.py
--rw-r--r--   0        0        0     2720 2024-04-29 01:06:09.308725 cntrlai-0.0.33/cntrlai/utils.py
--rw-r--r--   0        0        0     1477 2024-04-29 05:46:37.581213 cntrlai-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 cntrlai-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-04-27 00:39:09.943029 cntrlai-0.0.34/README.md
+-rw-r--r--   0        0        0      284 2024-04-29 00:59:20.632041 cntrlai-0.0.34/cntrlai/__init__.py
+-rw-r--r--   0        0        0     7579 2024-04-29 00:59:54.678362 cntrlai-0.0.34/cntrlai/batch_evaluation.py
+-rw-r--r--   0        0        0     3401 2024-04-29 01:00:28.289059 cntrlai-0.0.34/cntrlai/guardrails.py
+-rw-r--r--   0        0        0    11044 2024-04-29 01:04:56.414065 cntrlai-0.0.34/cntrlai/langchain.py
+-rw-r--r--   0        0        0     8710 2024-04-29 05:35:40.848340 cntrlai-0.0.34/cntrlai/logger.py
+-rw-r--r--   0        0        0    20786 2024-04-30 05:30:49.803422 cntrlai-0.0.34/cntrlai/openai.py
+-rw-r--r--   0        0        0     3588 2024-04-29 01:05:54.216065 cntrlai-0.0.34/cntrlai/types.py
+-rw-r--r--   0        0        0     2720 2024-04-29 01:06:09.308725 cntrlai-0.0.34/cntrlai/utils.py
+-rw-r--r--   0        0        0     1477 2024-05-01 04:07:37.875840 cntrlai-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 cntrlai-0.0.34/PKG-INFO
```

### Comparing `cntrlai-0.0.33/cntrlai/batch_evaluation.py` & `cntrlai-0.0.34/cntrlai/batch_evaluation.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/cntrlai/guardrails.py` & `cntrlai-0.0.34/cntrlai/guardrails.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/cntrlai/langchain.py` & `cntrlai-0.0.34/cntrlai/langchain.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/cntrlai/logger.py` & `cntrlai-0.0.34/cntrlai/logger.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/cntrlai/openai.py` & `cntrlai-0.0.34/cntrlai/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 )
 
 from openai.types import Completion
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
 logger = logging.getLogger("chainlit")
 
-class OpenAITracer(BaseContextTracer):
+class BasicLoggerOpenAI(BaseContextTracer):
     """
     Tracing for both Completion and ChatCompletion endpoints
     """
 
     def __init__(
         self,
         instance: Union[OpenAI, AsyncOpenAI],
@@ -63,24 +63,24 @@
             instance=instance, trace_id=trace_id, metadata=metadata
         )
 
     def __enter__(self):
         super().__enter__()
         self.completion_tracer.__enter__()
         self.chat_completion_tracer.__enter__()
-        logger.info("Entered OpenAITracer")
+        logger.info("Entered BasicLoggerOpenAI")
 
     def __exit__(self, _type, _value, _traceback):
         super().__exit__(_type, _value, _traceback)
         self.completion_tracer.__exit__(_type, _value, _traceback)
         self.chat_completion_tracer.__exit__(_type, _value, _traceback)
-        logger.info("Exited OpenAITracer")
+        logger.info("Exited BasicLoggerOpenAI")
 
 
-class AzureOpenAITracer(OpenAITracer):
+class AzureOpenAITracer(BasicLoggerOpenAI):
     """
     Tracing for both Completion and ChatCompletion endpoints
     """
 
     def __init__(
         self,
         instance: Union[AzureOpenAI, AsyncAzureOpenAI],
```

### Comparing `cntrlai-0.0.33/cntrlai/types.py` & `cntrlai-0.0.34/cntrlai/types.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/cntrlai/utils.py` & `cntrlai-0.0.34/cntrlai/utils.py`

 * *Files identical despite different names*

### Comparing `cntrlai-0.0.33/pyproject.toml` & `cntrlai-0.0.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cntrlai"
-version = "0.0.33"
+version = "0.0.34"
 description = "ControlAI's Client for Monitoring Your LLM performance"
 authors = ["Lukasz Bartoszcze <lbartoszcze@controlai.org>"]
 homepage = "https://controlai.org"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `cntrlai-0.0.33/PKG-INFO` & `cntrlai-0.0.34/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cntrlai
-Version: 0.0.33
+Version: 0.0.34
 Summary: ControlAI's Client for Monitoring Your LLM performance
 Home-page: https://controlai.org
 License: MIT
 Author: Lukasz Bartoszcze
 Author-email: lbartoszcze@controlai.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

