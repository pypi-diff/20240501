# Comparing `tmp/athena_intelligence-0.1.54.tar.gz` & `tmp/athena_intelligence-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.54.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.55.tar", max compression
```

## Comparing `athena_intelligence-0.1.54.tar` & `athena_intelligence-0.1.55.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     4235 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/README.md
--rw-r--r--   0        0        0      603 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     1499 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/__init__.py
--rw-r--r--   0        0        0     6659 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/base_client.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/chain/__init__.py
--rw-r--r--   0        0        0    16177 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/chain/client.py
--rw-r--r--   0        0        0     3576 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/client.py
--rw-r--r--   0        0        0      853 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12498 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6338 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6623 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-25 21:59:46.605950 athena_intelligence-0.1.54/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    20094 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/tools/client.py
--rw-r--r--   0        0        0     1678 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/__init__.py
--rw-r--r--   0        0        0      994 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1061 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/document.py
--rw-r--r--   0        0        0      875 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1001 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1143 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      969 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      969 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      953 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      892 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0     4101 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/llm_model.py
--rw-r--r--   0        0        0      950 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/map_reduce_chain_out.py
--rw-r--r--   0        0        0      845 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1031 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2991 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/model.py
--rw-r--r--   0        0        0      926 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/report.py
--rw-r--r--   0        0        0     1106 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/snippet.py
--rw-r--r--   0        0        0      880 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      885 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1422 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/tools.py
--rw-r--r--   0        0        0      873 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/url_result.py
--rw-r--r--   0        0        0      972 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       87 2024-04-25 21:59:46.609950 athena_intelligence-0.1.54/src/athena/version.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/README.md
+-rw-r--r--   0        0        0      603 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     1539 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/__init__.py
+-rw-r--r--   0        0        0     6659 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0    16177 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0    11323 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    20094 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1742 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-04-30 23:45:50.146377 athena_intelligence-0.1.55/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1001 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      879 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/get_snippet_out.py
+-rw-r--r--   0        0        0      969 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      892 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4101 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      950 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/map_reduce_chain_out.py
+-rw-r--r--   0        0        0      845 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2991 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/model.py
+-rw-r--r--   0        0        0      926 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/report.py
+-rw-r--r--   0        0        0     1106 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1422 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/tools.py
+-rw-r--r--   0        0        0      873 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       87 2024-04-30 23:45:50.150377 athena_intelligence-0.1.55/src/athena/version.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.55/PKG-INFO
```

### Comparing `athena_intelligence-0.1.54/README.md` & `athena_intelligence-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/pyproject.toml` & `athena_intelligence-0.1.55/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-intelligence"
-version = "0.1.54"
+version = "0.1.55"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "athena", from = "src"}
 ]
```

### Comparing `athena_intelligence-0.1.54/src/athena/__init__.py` & `athena_intelligence-0.1.55/src/athena/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .types import (
     Dataset,
     Document,
     ExcecuteToolFirstWorkflowOut,
     FirecrawlScrapeUrlDataReponseDto,
     FirecrawlScrapeUrlMetadata,
     GetDatasetsResponse,
+    GetSnippetOut,
     GetSnippetsResponse,
     HttpValidationError,
     LangchainDocumentsRequestOut,
     LlmModel,
     MapReduceChainOut,
     MessageOut,
     MessageOutDto,
@@ -34,14 +35,15 @@
     "AthenaEnvironment",
     "Dataset",
     "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
+    "GetSnippetOut",
     "GetSnippetsResponse",
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
     "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
```

### Comparing `athena_intelligence-0.1.54/src/athena/base_client.py` & `athena_intelligence-0.1.55/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/chain/client.py` & `athena_intelligence-0.1.55/src/athena/chain/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/client.py` & `athena_intelligence-0.1.55/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/__init__.py` & `athena_intelligence-0.1.55/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.55/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.54",
+            "X-Fern-SDK-Version": "0.1.55",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.54/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.55/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/file.py` & `athena_intelligence-0.1.55/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/http_client.py` & `athena_intelligence-0.1.55/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.55/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/core/request_options.py` & `athena_intelligence-0.1.55/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/dataset/client.py` & `athena_intelligence-0.1.55/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/message/client.py` & `athena_intelligence-0.1.55/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/polling_message_client.py` & `athena_intelligence-0.1.55/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/query/client.py` & `athena_intelligence-0.1.55/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/report/client.py` & `athena_intelligence-0.1.55/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/search/client.py` & `athena_intelligence-0.1.55/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/snippet/client.py` & `athena_intelligence-0.1.55/src/athena/snippet/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.get_snippet_out import GetSnippetOut
 from ..types.get_snippets_response import GetSnippetsResponse
 from ..types.http_validation_error import HttpValidationError
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
+
 
 class SnippetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(
         self,
@@ -79,14 +83,68 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_by_id(self, *, id: str, request_options: typing.Optional[RequestOptions] = None) -> GetSnippetOut:
+        """
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from athena.client import Athena
+
+        client = Athena(
+            api_key="YOUR_API_KEY",
+        )
+        client.snippet.get_by_id(
+            id="snippet_02329f1b-f6ad-4e93-be84-355c33202024b",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippet"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder({"id": id})
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder({"id": id}),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(GetSnippetOut, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncSnippetClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(
         self,
@@ -145,9 +203,63 @@
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_by_id(self, *, id: str, request_options: typing.Optional[RequestOptions] = None) -> GetSnippetOut:
+        """
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from athena.client import AsyncAthena
+
+        client = AsyncAthena(
+            api_key="YOUR_API_KEY",
+        )
+        await client.snippet.get_by_id(
+            id="snippet_02329f1b-f6ad-4e93-be84-355c33202024b",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippet"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder({"id": id})
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder({"id": id}),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(GetSnippetOut, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.54/src/athena/tools/client.py` & `athena_intelligence-0.1.55/src/athena/tools/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/__init__.py` & `athena_intelligence-0.1.55/src/athena/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .dataset import Dataset
 from .document import Document
 from .excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from .firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
 from .get_datasets_response import GetDatasetsResponse
+from .get_snippet_out import GetSnippetOut
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
 from .langchain_documents_request_out import LangchainDocumentsRequestOut
 from .llm_model import LlmModel
 from .map_reduce_chain_out import MapReduceChainOut
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
@@ -27,14 +28,15 @@
 __all__ = [
     "Dataset",
     "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
+    "GetSnippetOut",
     "GetSnippetsResponse",
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
     "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
```

### Comparing `athena_intelligence-0.1.54/src/athena/types/dataset.py` & `athena_intelligence-0.1.55/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/document.py` & `athena_intelligence-0.1.55/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.55/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.55/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.55/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.55/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.55/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.55/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.55/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/llm_model.py` & `athena_intelligence-0.1.55/src/athena/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/map_reduce_chain_out.py` & `athena_intelligence-0.1.55/src/athena/types/map_reduce_chain_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/message_out.py` & `athena_intelligence-0.1.55/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.55/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/model.py` & `athena_intelligence-0.1.55/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/report.py` & `athena_intelligence-0.1.55/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/snippet.py` & `athena_intelligence-0.1.55/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/sql_results.py` & `athena_intelligence-0.1.55/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/status_enum.py` & `athena_intelligence-0.1.55/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.55/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/tools.py` & `athena_intelligence-0.1.55/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/url_result.py` & `athena_intelligence-0.1.55/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/src/athena/types/validation_error.py` & `athena_intelligence-0.1.55/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.54/PKG-INFO` & `athena_intelligence-0.1.55/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.54
+Version: 0.1.55
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

