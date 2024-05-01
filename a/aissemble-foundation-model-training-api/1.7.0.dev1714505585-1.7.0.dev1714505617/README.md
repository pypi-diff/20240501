# Comparing `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714505585.tar.gz` & `tmp/aissemble_foundation_model_training_api-1.7.0.dev1714505617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714505585.tar", max compression
+gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1714505617.tar", max compression
```

## Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585.tar` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-04-30 19:32:49.836589 aissemble_foundation_model_training_api-1.7.0.dev1714505585/LICENSE
--rw-r--r--   0        0        0      318 2024-04-30 19:23:29.269274 aissemble_foundation_model_training_api-1.7.0.dev1714505585/LICENSE.txt
--rw-r--r--   0        0        0     1796 2024-04-30 19:23:29.270274 aissemble_foundation_model_training_api-1.7.0.dev1714505585/README.md
--rw-r--r--   0        0        0      859 2024-04-30 19:33:05.839606 aissemble_foundation_model_training_api-1.7.0.dev1714505585/pyproject.toml
--rw-r--r--   0        0        0     6779 2024-04-30 19:23:29.270274 aissemble_foundation_model_training_api-1.7.0.dev1714505585/src/model_training_api/model_training_api.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714505585/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-30 19:33:18.462365 aissemble_foundation_model_training_api-1.7.0.dev1714505617/LICENSE
+-rw-r--r--   0        0        0      318 2024-04-30 19:23:29.237569 aissemble_foundation_model_training_api-1.7.0.dev1714505617/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2024-04-30 19:23:29.237569 aissemble_foundation_model_training_api-1.7.0.dev1714505617/README.md
+-rw-r--r--   0        0        0      859 2024-04-30 19:33:37.531876 aissemble_foundation_model_training_api-1.7.0.dev1714505617/pyproject.toml
+-rw-r--r--   0        0        0     6779 2024-04-30 19:23:29.237569 aissemble_foundation_model_training_api-1.7.0.dev1714505617/src/model_training_api/model_training_api.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1714505617/PKG-INFO
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585/LICENSE` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585/README.md` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585/pyproject.toml` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-model-training-api"
-version = "1.7.0.dev1714505585"
+version = "1.7.0.dev1714505617"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api", from = "src"},
 ]
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585/src/model_training_api/model_training_api.py` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617/src/model_training_api/model_training_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1714505585/PKG-INFO` & `aissemble_foundation_model_training_api-1.7.0.dev1714505617/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-model-training-api
-Version: 1.7.0.dev1714505585
+Version: 1.7.0.dev1714505617
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
 Requires-Dist: fastapi (>=0.95.0)
```

