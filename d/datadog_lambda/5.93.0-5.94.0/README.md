# Comparing `tmp/datadog_lambda-5.93.0.tar.gz` & `tmp/datadog_lambda-5.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-5.93.0.tar", max compression
+gzip compressed data, was "datadog_lambda-5.94.0.tar", max compression
```

## Comparing `datadog_lambda-5.93.0.tar` & `datadog_lambda-5.94.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11379 2024-04-25 17:56:08.424389 datadog_lambda-5.93.0/LICENSE
--rw-r--r--   0        0        0     1381 2024-04-25 17:56:08.876391 datadog_lambda-5.93.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      141 2024-04-25 17:56:08.424389 datadog_lambda-5.93.0/NOTICE
--rw-r--r--   0        0        0     5943 2024-04-25 17:56:08.876391 datadog_lambda-5.93.0/README.md
--rw-r--r--   0        0        0      637 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     8171 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0      621 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      992 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0      766 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/logger.py
--rw-r--r--   0        0        0     4595 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4710 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     2091 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     2487 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    47962 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12177 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0       23 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/version.py
--rw-r--r--   0        0        0    15272 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3749 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1435 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/pyproject.toml
--rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 datadog_lambda-5.93.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2024-05-01 17:24:13.401643 datadog_lambda-5.94.0/LICENSE
+-rw-r--r--   0        0        0     1381 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      141 2024-05-01 17:24:13.401643 datadog_lambda-5.94.0/NOTICE
+-rw-r--r--   0        0        0     5943 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/README.md
+-rw-r--r--   0        0        0      637 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     8171 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0      621 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0     1351 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0      766 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/logger.py
+-rw-r--r--   0        0        0     4601 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4710 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     2091 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     2532 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    48927 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12177 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0       23 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/version.py
+-rw-r--r--   0        0        0    15272 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3749 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1435 2024-05-01 17:24:13.821647 datadog_lambda-5.94.0/pyproject.toml
+-rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 datadog_lambda-5.94.0/PKG-INFO
```

### Comparing `datadog_lambda-5.93.0/LICENSE` & `datadog_lambda-5.94.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/LICENSE-3rdparty.csv` & `datadog_lambda-5.94.0/LICENSE-3rdparty.csv`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/README.md` & `datadog_lambda-5.94.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/__init__.py` & `datadog_lambda-5.94.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/api.py` & `datadog_lambda-5.94.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/cold_start.py` & `datadog_lambda-5.94.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/constants.py` & `datadog_lambda-5.94.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-5.94.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/extension.py` & `datadog_lambda-5.94.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/handler.py` & `datadog_lambda-5.94.0/datadog_lambda/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2020 Datadog, Inc.
 
 from __future__ import absolute_import
 from importlib import import_module
 
 import os
+from time import time_ns
+
+from datadog_lambda.tracing import emit_telemetry_on_exception_outside_of_handler
 from datadog_lambda.wrapper import datadog_lambda_wrapper
 from datadog_lambda.module_name import modify_module_name
 
 
 class HandlerError(Exception):
     pass
 
@@ -23,9 +26,21 @@
 parts = path.rsplit(".", 1)
 if len(parts) != 2:
     raise HandlerError(f"Value {path} for DD_LAMBDA_HANDLER has invalid format.")
 
 
 (mod_name, handler_name) = parts
 modified_mod_name = modify_module_name(mod_name)
-handler_module = import_module(modified_mod_name)
-handler = datadog_lambda_wrapper(getattr(handler_module, handler_name))
+
+try:
+    handler_load_start_time_ns = time_ns()
+    handler_module = import_module(modified_mod_name)
+    handler_func = getattr(handler_module, handler_name)
+except Exception as e:
+    emit_telemetry_on_exception_outside_of_handler(
+        e,
+        modified_mod_name,
+        handler_load_start_time_ns,
+    )
+    raise
+
+handler = datadog_lambda_wrapper(handler_func)
```

### Comparing `datadog_lambda-5.93.0/datadog_lambda/logger.py` & `datadog_lambda-5.94.0/datadog_lambda/logger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/metric.py` & `datadog_lambda-5.94.0/datadog_lambda/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def submit_enhanced_metric(metric_name, lambda_context):
     """Submits the enhanced metric with the given name
 
     Args:
         metric_name (str): metric name w/o enhanced prefix i.e. "invocations" or "errors"
-        lambda_context (dict): Lambda context dict passed to the function by AWS
+        lambda_context (object): Lambda context dict passed to the function by AWS
     """
     if not enhanced_metrics_enabled:
         logger.debug(
             "Not submitting enhanced metric %s because enhanced metrics are disabled",
             metric_name,
         )
         return
@@ -114,19 +114,19 @@
     lambda_metric(metric_name, 1, timestamp=None, tags=tags, force_async=True)
 
 
 def submit_invocations_metric(lambda_context):
     """Increment aws.lambda.enhanced.invocations by 1, applying runtime, layer, and cold_start tags
 
     Args:
-        lambda_context (dict): Lambda context dict passed to the function by AWS
+        lambda_context (object): Lambda context dict passed to the function by AWS
     """
     submit_enhanced_metric("invocations", lambda_context)
 
 
 def submit_errors_metric(lambda_context):
     """Increment aws.lambda.enhanced.errors by 1, applying runtime, layer, and cold_start tags
 
     Args:
-        lambda_context (dict): Lambda context dict passed to the function by AWS
+        lambda_context (object): Lambda context dict passed to the function by AWS
     """
     submit_enhanced_metric("errors", lambda_context)
```

### Comparing `datadog_lambda-5.93.0/datadog_lambda/patch.py` & `datadog_lambda-5.94.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/tag_object.py` & `datadog_lambda-5.94.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/tags.py` & `datadog_lambda-5.94.0/datadog_lambda/tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,19 @@
     tags.append(resource)
 
     return tags
 
 
 def get_enhanced_metrics_tags(lambda_context):
     """Get the list of tags to apply to enhanced metrics"""
-    tags = parse_lambda_tags_from_arn(lambda_context)
+    tags = []
+    if lambda_context:
+        tags = parse_lambda_tags_from_arn(lambda_context)
+        tags.append(f"memorysize:{lambda_context.memory_limit_in_mb}")
     tags.append(get_cold_start_tag())
-    tags.append(f"memorysize:{lambda_context.memory_limit_in_mb}")
     tags.append(runtime_tag)
     tags.append(library_version_tag)
     return tags
 
 
 def check_if_number(alias):
     """
```

### Comparing `datadog_lambda-5.93.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-5.94.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/tracing.py` & `datadog_lambda-5.94.0/datadog_lambda/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 import hashlib
 import logging
 import os
 import base64
+import traceback
 import ujson as json
 from datetime import datetime, timezone
 from typing import Optional, Dict
 
 from datadog_lambda.metric import submit_errors_metric
 
 try:
@@ -1316,7 +1317,38 @@
             logger.debug(
                 "Unabled to read the %s tag, returning False. \
                 Reason: %s.",
                 InferredSpanInfo.SYNCHRONICITY,
                 e,
             )
             return False
+
+
+def emit_telemetry_on_exception_outside_of_handler(
+    exception, resource_name, handler_load_start_time_ns
+):
+    """
+    Emit an enhanced error metric and create a span for exceptions occurring outside the handler
+    """
+    submit_errors_metric(None)
+    if dd_tracing_enabled:
+        span = tracer.trace(
+            "aws.lambda",
+            service="aws.lambda",
+            resource=resource_name,
+            span_type="serverless",
+        )
+        span.start_ns = handler_load_start_time_ns
+
+        tags = {
+            "error.status": 500,
+            "error.type": type(exception).__name__,
+            "error.message": exception,
+            "error.stack": traceback.format_exc(),
+            "resource_names": resource_name,
+            "resource.name": resource_name,
+            "operation_name": "aws.lambda",
+            "status": "error",
+        }
+        span.set_tags(tags)
+        span.error = 1
+        span.finish()
```

### Comparing `datadog_lambda-5.93.0/datadog_lambda/trigger.py` & `datadog_lambda-5.94.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/wrapper.py` & `datadog_lambda-5.94.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/datadog_lambda/xray.py` & `datadog_lambda-5.94.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.93.0/pyproject.toml` & `datadog_lambda-5.94.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "5.93.0"
+version = "5.94.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
```

### Comparing `datadog_lambda-5.93.0/PKG-INFO` & `datadog_lambda-5.94.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog_lambda
-Version: 5.93.0
+Version: 5.94.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.8.0,<4
```

