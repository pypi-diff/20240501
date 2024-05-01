# Comparing `tmp/great_expectations_cloud-20240429.0.dev4.tar.gz` & `tmp/great_expectations_cloud-20240430.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240429.0.dev4.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240430.0.tar", max compression
```

## Comparing `great_expectations_cloud-20240429.0.dev4.tar` & `great_expectations_cloud-20240430.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-30 19:48:45.385761 great_expectations_cloud-20240429.0.dev4/LICENSE
--rw-r--r--   0        0        0     9532 2024-04-30 19:48:45.385761 great_expectations_cloud-20240429.0.dev4/README.md
--rw-r--r--   0        0        0      150 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    17127 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5918 2024-04-30 19:48:45.413761 great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9462 2024-04-30 19:48:45.417761 great_expectations_cloud-20240429.0.dev4/pyproject.toml
--rw-r--r--   0        0        0    10866 1970-01-01 00:00:00.000000 great_expectations_cloud-20240429.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-05-01 17:50:22.679924 great_expectations_cloud-20240430.0/LICENSE
+-rw-r--r--   0        0        0     9532 2024-05-01 17:50:22.679924 great_expectations_cloud-20240430.0/README.md
+-rw-r--r--   0        0        0      150 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17221 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4663 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-05-01 17:50:22.707924 great_expectations_cloud-20240430.0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9377 2024-05-01 17:50:22.711924 great_expectations_cloud-20240430.0/pyproject.toml
+-rw-r--r--   0        0        0    10881 1970-01-01 00:00:00.000000 great_expectations_cloud-20240430.0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240429.0.dev4/LICENSE` & `great_expectations_cloud-20240430.0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/README.md` & `great_expectations_cloud-20240430.0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections import defaultdict
 from concurrent.futures import Future
 from concurrent.futures.thread import ThreadPoolExecutor
 from functools import partial
 from importlib.metadata import version as metadata_version
 from typing import TYPE_CHECKING, Any, Dict, Final
 
-from great_expectations import get_context
+from great_expectations import get_context  # type: ignore[attr-defined] # TODO: fix this
 from great_expectations.compatibility import pydantic
 from great_expectations.compatibility.pydantic import AmqpDsn, AnyUrl
 from great_expectations.core.http import create_session
 from great_expectations.data_context.cloud_constants import CLOUD_DEFAULT_BASE_URL
 from packaging.version import Version
 from pika.exceptions import AuthenticationError, ProbableAuthenticationError
 from tenacity import after_log, retry, retry_if_exception_type, stop_after_attempt, wait_exponential
@@ -358,15 +358,15 @@
         Set the the session headers for requests to GX Cloud.
         In particular, set the User-Agent header to identify the GX Agent and the correlation_id as
         Agent-Job-Id if provided.
 
         Note: the Agent-Job-Id header value will be set for all GX Cloud request until this method is
         called again.
         """
-        from great_expectations import __version__
+        from great_expectations import __version__  # type: ignore[attr-defined] # TODO: fix this
         from great_expectations.core import http
         from great_expectations.data_context.store.gx_cloud_store_backend import GXCloudStoreBackend
 
         if Version(__version__) > Version(
             "0.19"  # using 0.19 instead of 1.0 to account for pre-releases
         ):
             # TODO: public API should be available in v1
```

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/event_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,16 @@
     """Get major version as a string from version as a string. For example, "0.18.0" -> "0"."""
     parsed: Version | LegacyVersion = parse_version(version)
     if not isinstance(parsed, Version):
         raise InvalidVersionError(version)
     return str(parsed.major)
 
 
-_GX_MAJOR_VERSION = _get_major_version(str(gx.__version__))
+version = gx.__version__  # type: ignore[attr-defined] # TODO: fix this
+_GX_MAJOR_VERSION = _get_major_version(str(version))
 
 
 def _get_event_name(event: Event) -> str:
     try:
         return str(event.__name__)
     except AttributeError:
         return str(event.__class__.__name__)
```

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240430.0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240430.0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240429.0.dev4/pyproject.toml` & `great_expectations_cloud-20240430.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240429.0.dev4"
+version = "20240430.0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-great-expectations = "*" # Needs to be ^0.18.4 but keeping unbounded to deal with dependency resolver conflicts
+great-expectations = "^0.18.13"
 pydantic = "<3"
 pika = "^1.3.1"
 # needed for metrics serialization
 orjson = "^3.9.7, !=3.9.10" # TODO: remove inequality once dep resolution issue is resolved
 # relying on packaging in agent code so declaring it explicitly here
 packaging = "^21.3"
 tenacity = "^8.2.3"
```

### Comparing `great_expectations_cloud-20240429.0.dev4/PKG-INFO` & `great_expectations_cloud-20240430.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240429.0.dev4
+Version: 20240430.0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: postgres
 Provides-Extra: snowflake
-Requires-Dist: great-expectations
+Requires-Dist: great-expectations (>=0.18.13,<0.19.0)
 Requires-Dist: orjson (>=3.9.7,<4.0.0,!=3.9.10)
 Requires-Dist: packaging (>=21.3,<22.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pydantic (<3)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Project-URL: Repository, https://github.com/great-expectations/cloud
 Description-Content-Type: text/markdown
```

