# Comparing `tmp/langchain_google_vertexai-1.0.2.tar.gz` & `tmp/langchain_google_vertexai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_vertexai-1.0.2.tar", max compression
+gzip compressed data, was "langchain_google_vertexai-1.0.3.tar", max compression
```

## Comparing `langchain_google_vertexai-1.0.2.tar` & `langchain_google_vertexai-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/LICENSE
--rw-r--r--   0        0        0     2594 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/README.md
--rw-r--r--   0        0        0     1853 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/__init__.py
--rw-r--r--   0        0        0     3255 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_anthropic_utils.py
--rw-r--r--   0        0        0    11734 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_base.py
--rw-r--r--   0        0        0      151 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_enums.py
--rw-r--r--   0        0        0     8169 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_image_utils.py
--rw-r--r--   0        0        0     6623 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/_utils.py
--rw-r--r--   0        0        0     2511 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/callbacks.py
--rw-r--r--   0        0        0     6062 2024-04-26 16:55:02.533200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/chains.py
--rw-r--r--   0        0        0    41354 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/chat_models.py
--rw-r--r--   0        0        0    16394 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/embeddings.py
--rw-r--r--   0        0        0     9948 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/functions_utils.py
--rw-r--r--   0        0        0    12748 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/gemma.py
--rw-r--r--   0        0        0    11722 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/llms.py
--rw-r--r--   0        0        0     8224 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/model_garden.py
--rw-r--r--   0        0        0        0 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/py.typed
--rw-r--r--   0        0        0      471 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_sdk_manager.py
--rw-r--r--   0        0        0     6103 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_searcher.py
--rw-r--r--   0        0        0     5436 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_utils.py
--rw-r--r--   0        0        0     8050 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/document_storage.py
--rw-r--r--   0        0        0    15958 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/vectorstores.py
--rw-r--r--   0        0        0    18548 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/langchain_google_vertexai/vision_models.py
--rw-r--r--   0        0        0     3366 2024-04-26 16:55:02.537200 langchain_google_vertexai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2594 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/README.md
+-rw-r--r--   0        0        0     1853 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/__init__.py
+-rw-r--r--   0        0        0     3255 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_anthropic_utils.py
+-rw-r--r--   0        0        0    11995 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_base.py
+-rw-r--r--   0        0        0      151 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_enums.py
+-rw-r--r--   0        0        0     8169 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_image_utils.py
+-rw-r--r--   0        0        0     6623 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_utils.py
+-rw-r--r--   0        0        0     2511 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/callbacks.py
+-rw-r--r--   0        0        0     6062 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/chains.py
+-rw-r--r--   0        0        0    41816 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/chat_models.py
+-rw-r--r--   0        0        0    16445 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/embeddings.py
+-rw-r--r--   0        0        0     9948 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/functions_utils.py
+-rw-r--r--   0        0        0    13960 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/gemma.py
+-rw-r--r--   0        0        0    12145 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/llms.py
+-rw-r--r--   0        0        0     8536 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/model_garden.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/py.typed
+-rw-r--r--   0        0        0      471 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     4679 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_sdk_manager.py
+-rw-r--r--   0        0        0     6103 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_searcher.py
+-rw-r--r--   0        0        0     5436 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_utils.py
+-rw-r--r--   0        0        0     8050 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/document_storage.py
+-rw-r--r--   0        0        0    15958 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/vectorstores.py
+-rw-r--r--   0        0        0    18548 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vision_models.py
+-rw-r--r--   0        0        0     3343 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.3/PKG-INFO
```

### Comparing `langchain_google_vertexai-1.0.2/LICENSE` & `langchain_google_vertexai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/README.md` & `langchain_google_vertexai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/__init__.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_anthropic_utils.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_base.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,38 @@
     "The default location to use when making API calls."
     request_parallelism: int = 5
     "The amount of parallelism allowed for requests issued to VertexAI models. "
     "Default is 5."
     max_retries: int = 6
     """The maximum number of retries to make when generating."""
     task_executor: ClassVar[Optional[Executor]] = Field(default=None, exclude=True)
-    stop: Optional[List[str]] = None
+    stop: Optional[List[str]] = Field(default=None, alias="stop_sequences")
     "Optional list of stop words to use when generating."
-    model_name: Optional[str] = None
+    model_name: Optional[str] = Field(default=None, alias="model")
     "Underlying model name."
 
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+
     @root_validator(pre=True)
     def validate_params(cls, values: dict) -> dict:
         if "model" in values and "model_name" not in values:
             values["model_name"] = values.pop("model")
         return values
 
 
 class _VertexAICommon(_VertexAIBase):
     client_preview: Any = None  #: :meta private:
-    model_name: str
+    model_name: str = Field(default=None, alias="model")
     "Underlying model name."
     temperature: Optional[float] = None
     "Sampling temperature, it controls the degree of randomness in token selection."
-    max_output_tokens: Optional[int] = None
+    max_output_tokens: Optional[int] = Field(default=None, alias="max_tokens")
     "Token limit determines the maximum amount of text output from one prompt."
     top_p: Optional[float] = None
     "Tokens are selected from most probable to least until the sum of their "
     "probabilities equals the top-p value. Top-p is ignored for Codey models."
     top_k: Optional[int] = None
     "How the model selects tokens for output, the next token is selected from "
     "among the top-k most probable tokens. Top-k is ignored for Codey models."
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_image_utils.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_image_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/_utils.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/callbacks.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/chains.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/chains.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/chat_models.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputToolsParser,
     PydanticToolsParser,
 )
 from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
-from langchain_core.pydantic_v1 import BaseModel, root_validator
+from langchain_core.pydantic_v1 import BaseModel, root_validator, Field
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from vertexai.generative_models import (  # type: ignore
     Candidate,
     Content,
     GenerativeModel,
     Part,
     Tool as VertexTool,
@@ -494,26 +494,38 @@
 
     return await _completion_with_retry_inner(generation_method, **kwargs)
 
 
 class ChatVertexAI(_VertexAICommon, BaseChatModel):
     """`Vertex AI` Chat large language models API."""
 
-    model_name: str = "chat-bison"
+    model_name: str = Field(default="chat-bison", alias="model")
     "Underlying model name."
     examples: Optional[List[BaseMessage]] = None
     tuned_model_name: Optional[str] = None
     """The name of a tuned model. If tuned_model_name is passed
     model_name will be used to determine the model family
     """
     convert_system_message_to_human: bool = False
     """[Deprecated] Since new Gemini models support setting a System Message,
     setting this parameter to True is discouraged.
     """
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Needed for mypy typing to recognize model_name as a valid arg."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+        arbitrary_types_allowed = True
+
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/embeddings.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,30 +74,31 @@
                 values["client"] = TextEmbeddingModel.from_pretrained(
                     values["model_name"]
                 )
         return values
 
     def __init__(
         self,
-        model_name: str,
+        model_name: Optional[str] = None,
         project: Optional[str] = None,
         location: str = "us-central1",
         request_parallelism: int = 5,
         max_retries: int = 6,
         credentials: Optional[Any] = None,
         **kwargs: Any,
     ):
         """Initialize the sentence_transformer."""
+        if model_name:
+            kwargs["model_name"] = model_name
         super().__init__(
             project=project,
             location=location,
             credentials=credentials,
             request_parallelism=request_parallelism,
             max_retries=max_retries,
-            model_name=model_name,
             **kwargs,
         )
         self.instance["max_batch_size"] = kwargs.get("max_batch_size", _MAX_BATCH_SIZE)
         self.instance["batch_size"] = self.instance["max_batch_size"]
         self.instance["min_batch_size"] = kwargs.get("min_batch_size", _MIN_BATCH_SIZE)
         self.instance["min_good_batch_size"] = self.instance["min_batch_size"]
         self.instance["lock"] = threading.Lock()
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/functions_utils.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/functions_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/gemma.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/gemma.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from langchain_core.outputs import (
     ChatGeneration,
     ChatResult,
     Generation,
     LLMResult,
 )
-from langchain_core.pydantic_v1 import BaseModel, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 
 from langchain_google_vertexai._base import _BaseVertexAIModelGarden
 from langchain_google_vertexai._utils import enforce_stop_tokens
 from langchain_google_vertexai.model_garden import VertexAIModelGarden
 
 USER_CHAT_TEMPLATE = "<start_of_turn>user\n{prompt}<end_of_turn>\n"
 MODEL_CHAT_TEMPLATE = "<start_of_turn>model\n{prompt}<end_of_turn>\n"
@@ -111,14 +111,25 @@
         "top_k",
         "max_tokens",
     ]
     parse_response: bool = False
     """Whether to post-process the chat response and clean repeations """
     """or multi-turn statements."""
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Needed for mypy typing to recognize model_name as a valid arg."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+
     @property
     def _llm_type(self) -> str:
         return "gemma_vertexai_model_garden"
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling gemma."""
@@ -174,17 +185,23 @@
 
 
 class _GemmaLocalKaggleBase(_GemmaBase):
     """Local gemma model loaded from Kaggle."""
 
     client: Any = None  #: :meta private:
     keras_backend: str = "jax"
-    model_name: str = "gemma_2b_en"
+    model_name: str = Field(default="gemma_2b_en", alias="model")
     """Gemma model name."""
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Needed for mypy typing to recognize model_name as a valid arg."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that llama-cpp-python library is installed."""
         try:
             os.environ["KERAS_BACKEND"] = values["keras_backend"]
             from keras_nlp.models import GemmaCausalLM  # type: ignore
         except ImportError:
@@ -208,14 +225,20 @@
         params = {mapping[k]: v for k, v in kwargs.items() if k in mapping}
         return {**self._default_params, **params}
 
 
 class GemmaLocalKaggle(_GemmaLocalKaggleBase, BaseLLM):
     """Local gemma chat model loaded from Kaggle."""
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Only needed for typing."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
     def _generate(
         self,
         prompts: List[str],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> LLMResult:
@@ -234,14 +257,20 @@
 
 
 class GemmaChatLocalKaggle(_GemmaLocalKaggleBase, BaseChatModel):
     parse_response: bool = False
     """Whether to post-process the chat response and clean repeations """
     """or multi-turn statements."""
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Needed for mypy typing to recognize model_name as a valid arg."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
@@ -264,15 +293,15 @@
 class _GemmaLocalHFBase(_GemmaBase):
     """Local gemma model loaded from HuggingFace."""
 
     tokenizer: Any = None  #: :meta private:
     client: Any = None  #: :meta private:
     hf_access_token: str
     cache_dir: Optional[str] = None
-    model_name: str = "gemma_2b_en"
+    model_name: str = Field(default="gemma_2b_en", alias="model")
     """Gemma model name."""
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that llama-cpp-python library is installed."""
         try:
             from transformers import AutoTokenizer, GemmaForCausalLM  # type: ignore
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/llms.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from google.cloud.aiplatform import telemetry
 from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.llms import BaseLLM
 from langchain_core.outputs import Generation, GenerationChunk, LLMResult
-from langchain_core.pydantic_v1 import root_validator
+from langchain_core.pydantic_v1 import Field, root_validator
 from vertexai.generative_models import (  # type: ignore[import-untyped]
     Candidate,
     GenerativeModel,
     Image,
 )
 from vertexai.language_models import (  # type: ignore[import-untyped]
     CodeGenerationModel,
@@ -106,21 +106,32 @@
             prompt, is_gemini, stream=stream, **kwargs
         )
 
 
 class VertexAI(_VertexAICommon, BaseLLM):
     """Google Vertex AI large language models."""
 
-    model_name: str = "text-bison"
+    model_name: str = Field(default="text-bison", alias="model")
     "The name of the Vertex AI large language model."
     tuned_model_name: Optional[str] = None
     """The name of a tuned model. If tuned_model_name is passed
     model_name will be used to determine the model family
     """
 
+    def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
+        """Needed for mypy typing to recognize model_name as a valid arg."""
+        if model_name:
+            kwargs["model_name"] = model_name
+        super().__init__(**kwargs)
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/model_garden.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/model_garden.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,28 @@
 from langchain_core.outputs import (
     ChatGeneration,
     ChatGenerationChunk,
     ChatResult,
     Generation,
     LLMResult,
 )
-from langchain_core.pydantic_v1 import root_validator
+from langchain_core.pydantic_v1 import Field, root_validator
 
 from langchain_google_vertexai._anthropic_utils import _format_messages_anthropic
 from langchain_google_vertexai._base import _BaseVertexAIModelGarden, _VertexAICommon
 
 
 class VertexAIModelGarden(_BaseVertexAIModelGarden, BaseLLM):
     """Large language models served from Vertex AI Model Garden."""
 
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+
     def _generate(
         self,
         prompts: List[str],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> LLMResult:
@@ -88,17 +93,22 @@
             endpoint=self.endpoint_path, instances=instances
         )
         return self._parse_response(response)
 
 
 class ChatAnthropicVertex(_VertexAICommon, BaseChatModel):
     async_client: Any = None  #: :meta private:
-    model_name: Optional[str] = None  # type: ignore[assignment]
+    model_name: Optional[str] = Field(default=None, alias="model")  # type: ignore[assignment]
     "Underlying model name."
-    max_output_tokens: int = 1024
+    max_output_tokens: int = Field(default=1024, alias="max_tokens")
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         from anthropic import (  # type: ignore[import-not-found]
             AnthropicVertex,
             AsyncAnthropicVertex,
         )
```

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_sdk_manager.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_sdk_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_searcher.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_searcher.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/_utils.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/document_storage.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/document_storage.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vectorstores/vectorstores.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/langchain_google_vertexai/vision_models.py` & `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vision_models.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.2/pyproject.toml` & `langchain_google_vertexai-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "langchain-google-vertexai"
 
-version = "1.0.2"
+version = "1.0.3"
 description = "An integration package connecting Google VertexAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -102,15 +102,15 @@
 #
 # https://docs.pytest.org/en/7.1.x/reference/reference.html
 # --strict-config       any warnings encountered while parsing the `pytest`
 #                       section of the configuration file raise errors.
 #
 # https://github.com/tophat/syrupy
 # --snapshot-warn-unused    Prints a warning on unused snapshots rather than fail the test suite.
-addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
+addopts = "--strict-markers --strict-config --durations=5"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
   "compile: mark placeholder test used to compile integration tests without running them",
 ]
```

### Comparing `langchain_google_vertexai-1.0.2/PKG-INFO` & `langchain_google_vertexai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-vertexai
-Version: 1.0.2
+Version: 1.0.3
 Summary: An integration package connecting Google VertexAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

