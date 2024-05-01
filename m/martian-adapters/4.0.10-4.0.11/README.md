# Comparing `tmp/martian_adapters-4.0.10.tar.gz` & `tmp/martian_adapters-4.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-4.0.10.tar", max compression
+gzip compressed data, was "martian_adapters-4.0.11.tar", max compression
```

## Comparing `martian_adapters-4.0.10.tar` & `martian_adapters-4.0.11.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-04-30 00:30:40.565520 martian_adapters-4.0.10/LICENSE
--rw-r--r--   0        0        0     4319 2024-04-29 21:51:08.295614 martian_adapters-4.0.10/README.md
--rw-r--r--   0        0        0      725 2024-04-24 23:08:19.279531 martian_adapters-4.0.10/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-03-12 21:13:48.732102 martian_adapters-4.0.10/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2117 2024-02-06 20:08:59.742583 martian_adapters-4.0.10/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     3347 2024-04-25 03:58:20.005866 martian_adapters-4.0.10/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-03-15 23:53:07.585309 martian_adapters-4.0.10/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-04-01 03:49:11.566774 martian_adapters-4.0.10/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2386 2024-04-24 23:08:19.280106 martian_adapters-4.0.10/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0     3419 2024-04-25 03:58:20.006328 martian_adapters-4.0.10/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5816 2024-04-25 03:58:20.007161 martian_adapters-4.0.10/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     5812 2024-04-25 03:58:20.007536 martian_adapters-4.0.10/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-03-12 21:13:48.733334 martian_adapters-4.0.10/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-24 23:08:19.282029 martian_adapters-4.0.10/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0      942 2024-04-25 21:01:54.033018 martian_adapters-4.0.10/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9225 2024-04-25 03:58:20.008865 martian_adapters-4.0.10/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3563 2024-04-25 21:01:54.033635 martian_adapters-4.0.10/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2053 2024-04-25 03:58:20.009535 martian_adapters-4.0.10/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1203 2024-04-26 19:57:14.024569 martian_adapters-4.0.10/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-04-29 21:51:04.769723 martian_adapters-4.0.10/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1663 2024-04-24 23:08:19.283717 martian_adapters-4.0.10/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-04-25 03:58:20.009986 martian_adapters-4.0.10/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-04-25 21:01:54.034177 martian_adapters-4.0.10/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3855 2024-04-30 20:00:14.257048 martian_adapters-4.0.10/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1425 2024-04-25 21:01:54.034673 martian_adapters-4.0.10/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2307 2024-03-15 23:53:07.590557 martian_adapters-4.0.10/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    10017 2024-04-25 21:01:54.035420 martian_adapters-4.0.10/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2023-11-30 19:57:07.662865 martian_adapters-4.0.10/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-02-06 20:08:59.751016 martian_adapters-4.0.10/adapters/rate_limiter.py
--rw-r--r--   0        0        0      334 2024-02-06 20:08:59.751444 martian_adapters-4.0.10/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-04-25 03:58:20.012283 martian_adapters-4.0.10/adapters/types.py
--rw-r--r--   0        0        0        0 2023-11-09 21:00:33.698900 martian_adapters-4.0.10/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-04-24 23:08:19.285444 martian_adapters-4.0.10/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-03-12 21:13:48.734260 martian_adapters-4.0.10/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-03-08 00:01:49.626651 martian_adapters-4.0.10/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-04-24 23:08:19.285987 martian_adapters-4.0.10/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1171 2024-04-30 21:07:11.936229 martian_adapters-4.0.10/pyproject.toml
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 martian_adapters-4.0.10/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 00:30:40.565520 martian_adapters-4.0.11/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-01 00:14:43.669585 martian_adapters-4.0.11/README.md
+-rw-r--r--   0        0        0      725 2024-04-24 23:08:19.279531 martian_adapters-4.0.11/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-03-12 21:13:48.732102 martian_adapters-4.0.11/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2117 2024-02-06 20:08:59.742583 martian_adapters-4.0.11/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     3347 2024-04-25 03:58:20.005866 martian_adapters-4.0.11/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-03-15 23:53:07.585309 martian_adapters-4.0.11/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-04-01 03:49:11.566774 martian_adapters-4.0.11/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2386 2024-04-24 23:08:19.280106 martian_adapters-4.0.11/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0     3419 2024-04-25 03:58:20.006328 martian_adapters-4.0.11/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5816 2024-04-25 03:58:20.007161 martian_adapters-4.0.11/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     5812 2024-04-25 03:58:20.007536 martian_adapters-4.0.11/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-03-12 21:13:48.733334 martian_adapters-4.0.11/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3429 2024-04-24 23:08:19.282029 martian_adapters-4.0.11/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0      942 2024-04-25 21:01:54.033018 martian_adapters-4.0.11/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9225 2024-04-25 03:58:20.008865 martian_adapters-4.0.11/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3563 2024-04-25 21:01:54.033635 martian_adapters-4.0.11/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2053 2024-04-25 03:58:20.009535 martian_adapters-4.0.11/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1203 2024-04-26 19:57:14.024569 martian_adapters-4.0.11/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-04-29 21:51:04.769723 martian_adapters-4.0.11/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1663 2024-04-24 23:08:19.283717 martian_adapters-4.0.11/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-04-25 03:58:20.009986 martian_adapters-4.0.11/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-04-25 21:01:54.034177 martian_adapters-4.0.11/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-01 00:14:43.670186 martian_adapters-4.0.11/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1425 2024-04-25 21:01:54.034673 martian_adapters-4.0.11/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2307 2024-03-15 23:53:07.590557 martian_adapters-4.0.11/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    10017 2024-04-25 21:01:54.035420 martian_adapters-4.0.11/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2023-11-30 19:57:07.662865 martian_adapters-4.0.11/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-02-06 20:08:59.751016 martian_adapters-4.0.11/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      334 2024-02-06 20:08:59.751444 martian_adapters-4.0.11/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-04-25 03:58:20.012283 martian_adapters-4.0.11/adapters/types.py
+-rw-r--r--   0        0        0        0 2023-11-09 21:00:33.698900 martian_adapters-4.0.11/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-24 23:08:19.285444 martian_adapters-4.0.11/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-03-12 21:13:48.734260 martian_adapters-4.0.11/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-03-08 00:01:49.626651 martian_adapters-4.0.11/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-04-24 23:08:19.285987 martian_adapters-4.0.11/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1171 2024-05-01 00:14:46.894831 martian_adapters-4.0.11/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 martian_adapters-4.0.11/PKG-INFO
```

### Comparing `martian_adapters-4.0.10/LICENSE` & `martian_adapters-4.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/__init__.py` & `martian_adapters-4.0.11/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-4.0.11/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/adapter_factory.py` & `martian_adapters-4.0.11/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-4.0.11/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/__init__.py` & `martian_adapters-4.0.11/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     vendor_name: str = PROVIDER_NAME
     provider_name: str = PROVIDER_NAME
 
 
 MODELS = [
     OpenAIModel(
         name="gpt-3.5-turbo-1106",
-        cost=Cost(prompt=0.5e-6, completion=1.5e-6),
+        cost=Cost(prompt=1.0e-6, completion=2.0e-6),
         context_length=16385,
         completion_length=16385,
     ),
     OpenAIModel(
         name="gpt-3.5-turbo",
         cost=Cost(prompt=0.5e-6, completion=1.5e-6),
-        context_length=4096,
+        context_length=16385,
         completion_length=16385,
     ),
     OpenAIModel(
         name="gpt-3.5-turbo-0125",
         cost=Cost(prompt=0.5e-6, completion=1.5e-6),
         context_length=16385,
         completion_length=16385,
@@ -47,14 +47,20 @@
         context_length=32768,
         completion_length=32768,
         supports_json_output=False,
         supports_functions=False,
         supports_tools=False,
     ),
     OpenAIModel(
+        name="gpt-4-0125-preview",
+        cost=Cost(prompt=10.0e-6, completion=30.0e-6),
+        context_length=128000,
+        completion_length=4096,
+    ),
+    OpenAIModel(
         name="gpt-4-32k-0613",
         cost=Cost(prompt=60.0e-6, completion=120.0e-6),
         context_length=32768,
         completion_length=32768,
         supports_json_output=False,
     ),
     OpenAIModel(
@@ -103,14 +109,28 @@
     ),
     OpenAIModel(
         name="gpt-4-0125-preview",
         cost=Cost(prompt=10.0e-6, completion=30.0e-6),
         context_length=128000,
         completion_length=4096,
     ),
+    OpenAIModel(
+        name="gpt-4-turbo-2024-04-09",
+        cost=Cost(prompt=10.0e-6, completion=30.0e-6),
+        context_length=128000,
+        completion_length=4096,
+        supports_vision=True,
+    ),
+    OpenAIModel(
+        name="gpt-4-turbo",
+        cost=Cost(prompt=10.0e-6, completion=30.0e-6),
+        context_length=128000,
+        completion_length=4096,
+        supports_vision=True,
+    ),
 ]
 
 
 class OpenAISDKChatProviderAdapter(ProviderAdapterMixin, OpenAISDKChatAdapter):
     @staticmethod
     def get_supported_models():
         return MODELS
```

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-4.0.11/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/rate_limiter.py` & `martian_adapters-4.0.11/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/types.py` & `martian_adapters-4.0.11/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/utils/general_utils.py` & `martian_adapters-4.0.11/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/utils/network_utils.py` & `martian_adapters-4.0.11/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/adapters/utils/openai_client_factory.py` & `martian_adapters-4.0.11/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.0.10/pyproject.toml` & `martian_adapters-4.0.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "4.0.10"
+version = "4.0.11"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

