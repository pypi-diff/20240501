# Comparing `tmp/hmt-basemodels-0.2.9.tar.gz` & `tmp/hmt-basemodels-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmt-basemodels-0.2.9.tar", last modified: Wed Mar 20 20:18:54 2024, max compression
+gzip compressed data, was "hmt-basemodels-1.0.0.tar", last modified: Wed May  1 14:58:49 2024, max compression
```

## Comparing `hmt-basemodels-0.2.9.tar` & `hmt-basemodels-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.680201 hmt-basemodels-0.2.9/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1071 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/LICENSE
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       18 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/MANIFEST.in
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      469 2024-03-20 20:18:54.679968 hmt-basemodels-0.2.9/PKG-INFO
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     2149 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/README.md
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.675561 hmt-basemodels-0.2.9/basemodels/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      445 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/__init__.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      478 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/constants.py
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.676412 hmt-basemodels-0.2.9/basemodels/manifest/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      172 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/__init__.py
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.677665 hmt-basemodels-0.2.9/basemodels/manifest/data/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      327 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/__init__.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3770 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/groundtruth.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      740 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/helpers.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      481 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/preprocess.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1295 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/requester_question_example.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1739 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/requester_restricted_answer_set.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3375 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/basemodels/manifest/data/taskdata.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)    19411 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/basemodels/manifest/manifest.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     2777 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/manifest/restricted_audience.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1695 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/basemodels/via.py
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.679696 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      469 2024-03-20 20:18:54.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/PKG-INFO
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      846 2024-03-20 20:18:54.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/SOURCES.txt
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)        1 2024-03-20 20:18:54.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/dependency_links.txt
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       48 2024-03-20 20:18:54.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/requires.txt
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       11 2024-03-20 20:18:54.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/top_level.txt
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)        1 2024-01-29 15:04:24.000000 hmt-basemodels-0.2.9/hmt_basemodels.egg-info/zip-safe
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      462 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/pyproject.toml
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)       38 2024-03-20 20:18:54.680255 hmt-basemodels-0.2.9/setup.cfg
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)      606 2024-03-20 20:10:15.000000 hmt-basemodels-0.2.9/setup.py
-drwxr-xr-x   0 vladimir_shishkaryov   (501) staff       (20)        0 2024-03-20 20:18:54.679463 hmt-basemodels-0.2.9/tests/
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)    39333 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/tests/test_manifest_validation.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     1199 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/tests/test_preprocess.py
--rw-r--r--   0 vladimir_shishkaryov   (501) staff       (20)     3195 2024-01-29 14:58:22.000000 hmt-basemodels-0.2.9/tests/test_restricted_answer_set.py
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1071 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/LICENSE
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       18 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/MANIFEST.in
+-rw-r--r--   0 alidzm    (1000) alidzm    (1000)      467 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/PKG-INFO
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     2155 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/README.md
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      445 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/__init__.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1505 2024-04-17 08:57:12.000000 hmt-basemodels-1.0.0/basemodels/constants.py
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/manifest/
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      172 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/manifest/__init__.py
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.789386 hmt-basemodels-1.0.0/basemodels/manifest/data/
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      327 2023-10-31 09:29:49.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/__init__.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     4706 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/groundtruth.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      595 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/helpers.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      479 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/preprocess.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      982 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/requester_question_example.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1329 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/requester_restricted_answer_set.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3338 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/data/taskdata.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)    19300 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/manifest.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3031 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/basemodels/manifest/restricted_audience.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1695 2024-04-17 08:57:12.000000 hmt-basemodels-1.0.0/basemodels/via.py
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/
+-rw-r--r--   0 alidzm    (1000) alidzm    (1000)      467 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      846 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)        1 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       46 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/requires.txt
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       11 2024-05-01 14:58:49.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/top_level.txt
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)        1 2024-04-24 07:32:50.000000 hmt-basemodels-1.0.0/hmt_basemodels.egg-info/zip-safe
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      462 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/pyproject.toml
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)       38 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/setup.cfg
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)      604 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/setup.py
+drwxrwxr-x   0 alidzm    (1000) alidzm    (1000)        0 2024-05-01 14:58:49.793386 hmt-basemodels-1.0.0/tests/
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)    39004 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_manifest_validation.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     1181 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_preprocess.py
+-rw-rw-r--   0 alidzm    (1000) alidzm    (1000)     3188 2024-05-01 14:55:05.000000 hmt-basemodels-1.0.0/tests/test_restricted_answer_set.py
```

### Comparing `hmt-basemodels-0.2.9/LICENSE` & `hmt-basemodels-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.2.9/README.md` & `hmt-basemodels-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 }
 # Validate model on creation
 try:
    manifest = basemodels.Manifest(**model)
 except ValidationError as e:
    print(e.json())
 # Or creating model without validation
-manifest = basemodels.Manifest.construct(**model)
+manifest = basemodels.Manifest.model_construct(**model)
 # See https://pydantic-docs.helpmanual.io/usage/models/#creating-models-without-validation
 ```
 ## Note for maintainers: Deploying to PyPi
 
 A build will automatically be deployed to PyPi from master if tagged with a version number.  This version number should  match the version in the `setup.py` file.
 
 The tags will need to be pushed to master via a user that has the proper privileges (see the contributors of this repo).
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/data/groundtruth.py` & `hmt-basemodels-1.0.0/basemodels/manifest/data/groundtruth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import List, Optional, Union
+from uuid import UUID
 
 import requests
-from pydantic.v1 import BaseModel, HttpUrl, ValidationError, conlist, validator, root_validator, Field
+from pydantic import BaseModel, HttpUrl, ValidationError, ConfigDict
 from requests import RequestException
 from typing_extensions import Literal
 
-from basemodels.constants import SUPPORTED_CONTENT_TYPES
+from basemodels.constants import SUPPORTED_CONTENT_TYPES, BaseJobTypesEnum
 
 
 def create_wrapper_model(type):
     class WrapperModel(BaseModel):
-        data: Optional[type]
-
-        class Config:
-            arbitrary_types_allowed = True
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+        data: Optional[type] = None
 
     return WrapperModel
 
 
 def validate_wrapper_model(Model, data):
     Model.validate({"data": data})
 
@@ -51,15 +50,15 @@
 }
 """
 ilmc_groundtruth_entry_type = List[List[str]]
 ILMCGroundtruthEntryModel = create_wrapper_model(ilmc_groundtruth_entry_type)
 
 
 class ILASGroundtruthEntry(BaseModel):
-    entity_name: Optional[Union[int, float]]
+    entity_name: Optional[Union[int, float]] = None
     entity_type: str
     entity_coords: List[Union[int, float]]
 
 
 """
 Groundtruth file format for `image_label_area_select` job type
 
@@ -74,14 +73,41 @@
     ]
   ]
 }
 """
 ilas_groundtruth_entry_type = List[List[ILASGroundtruthEntry]]
 ILASGroundtruthEntryModel = create_wrapper_model(ilas_groundtruth_entry_type)
 
+
+class IDDGroundtruthEntry(BaseModel):
+    entity_name: UUID
+    entity_type: Optional[str]
+    entity_coords: List[int]
+
+
+"""
+Groundtruth file format for `image_drag_drop` job type
+
+{
+  "81fb76f3-3906-4fbd-8168-9dff208860a5": [
+    {
+      "entity_name": "04606112-4b9d-455f-8f43-9cc1a9bca185",
+      "entity_type": "default",
+      "entity_coords": [275, 184]
+    }
+  ]
+}
+"""
+idd_groundtruth_entry_type = List[IDDGroundtruthEntry]
+IDDGroundtruthEntryModel = create_wrapper_model(idd_groundtruth_entry_type)
+
+idd_groundtruth_entry_key_type = UUID
+IDDGroundtruthEntryKeyModel = create_wrapper_model(idd_groundtruth_entry_key_type)
+
+
 class TLMSSGroundTruthEntry(BaseModel):
     start: int
     end: int
     label: str
 
 
 """
@@ -102,42 +128,48 @@
 
 
 groundtruth_entry_models_map = {
     "image_label_binary": ILBGroundtruthEntryModel,
     "image_label_multiple_choice": ILMCGroundtruthEntryModel,
     "image_label_area_select": ILASGroundtruthEntryModel,
     "text_label_multiple_span_select": TLMSSGroundTruthEntryModel,
+    "image_drag_drop": IDDGroundtruthEntryModel,
 }
 
+
 def validate_content_type(uri: str) -> None:
     """Validate uri content type"""
     try:
         response = requests.head(uri, timeout=(3.5, 5))
         response.raise_for_status()
     except RequestException as e:
-        raise ValidationError(f"groundtruth content type ({uri}) validation failed", GroundtruthEntryKeyModel) from e
+        raise ValidationError(f"groundtruth content type ({uri}) validation failed", GroundtruthEntryKeyModel()) from e
 
     content_type = response.headers.get("Content-Type", "")
     if content_type not in SUPPORTED_CONTENT_TYPES:
         raise ValidationError(
             f"groundtruth entry has unsupported type {content_type}",
-            GroundtruthEntryKeyModel,
+            GroundtruthEntryKeyModel(),
         )
 
 
 def validate_groundtruth_entry(
     key: str,
     value: Union[dict, list],
     request_type: str,
     validate_image_content_type: bool,
 ):
     """Validate key & value of groundtruth entry based on request_type"""
-    GroundtruthEntryValueModel = groundtruth_entry_models_map.get(request_type)
+    groundtruth_entry_value_model_class = groundtruth_entry_models_map.get(request_type)
+    groundtruth_entry_key_model_class = GroundtruthEntryKeyModel
 
-    if GroundtruthEntryValueModel is None:
+    if groundtruth_entry_value_model_class is None:
         return
 
-    validate_wrapper_model(GroundtruthEntryKeyModel, key)
-    validate_wrapper_model(GroundtruthEntryValueModel, value)
+    if request_type == BaseJobTypesEnum.image_drag_drop:
+        groundtruth_entry_key_model_class = IDDGroundtruthEntryKeyModel
+
+    validate_wrapper_model(groundtruth_entry_key_model_class, key)
+    validate_wrapper_model(groundtruth_entry_value_model_class, value)
 
     if validate_image_content_type:
         validate_content_type(key)
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/data/requester_question_example.py` & `hmt-basemodels-1.0.0/basemodels/manifest/data/requester_question_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Union
 
-from pydantic.v1.error_wrappers import ErrorWrapper
 from requests import RequestException
 from pydantic.v1 import ValidationError
 from .helpers import validate_content_type, ExampleResourceModel
 
 
 def validate_requester_example_image(
     value: Union[str, list],
@@ -18,24 +17,12 @@
         elif isinstance(value, list):
             for uri in value:
                 uri_val = uri
                 validate_content_type(uri)
         else:
             raise ValueError(f"Not supported format for requester_question_example.")
     except RequestException as e:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"could not retrieve requester example ({uri_val})"), "answer_example_uri")
-            ],
-            ExampleResourceModel
-        ) from e
+        raise ValidationError(f"could not retrieve requester example ({uri_val})", ExampleResourceModel()) from e
     except ValidationError as e:
         raise ValidationError(
-            [
-                ErrorWrapper(
-                    ValueError(f"requester example image for {uri_val} has unsupported type"),
-                    "answer_example_uri"
-                )
-            ],
-            ExampleResourceModel
+            f"requester example image for {uri_val} has unsupported type", ExampleResourceModel()
         ) from e
-
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/data/requester_restricted_answer_set.py` & `hmt-basemodels-1.0.0/basemodels/manifest/data/requester_restricted_answer_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pydantic.v1.error_wrappers import ErrorWrapper
 from requests import RequestException
 from pydantic.v1 import ValidationError
 from .helpers import validate_content_type, ExampleResourceModel
 
 
 def extract_answer_uri(restricted_answer_set: dict) -> list:
     """Extract the answer_uri from the answer set"""
@@ -13,34 +12,22 @@
 
     return answer_uris
 
 
 def validate_requester_restricted_answer_set_uris(restricted_answer_set: dict) -> None:
     """Validate requester restricted entry"""
     if not isinstance(restricted_answer_set, dict):
-        raise ValidationError("Requester restricted set should be a dict")
+        raise ValueError("Requester restricted set should be a dict")
     uris = extract_answer_uri(restricted_answer_set)
     for uri in uris:
         try:
             validate_content_type(uri)
         except RequestException as e:
             raise ValidationError(
-                [
-                    ErrorWrapper(
-                        ValueError(f"could not retrieve requester restricted answer set example uri ({uri})"),
-                        "answer_example_uri"
-                    )
-                ],
-                ExampleResourceModel
+                f"could not retrieve requester restricted answer set example uri ({uri})",
+                ExampleResourceModel()
             ) from e
         except ValidationError as e:
-
             raise ValidationError(
-                [
-                    ErrorWrapper(
-                        ValueError(f"requester restricted answer set example uri "
-                                   f"({uri}) content type failed validation"),
-                        "answer_example_uri"
-                    )
-                ],
-                ExampleResourceModel
+                f"requester restricted answer set example uri({uri}) content type failed validation",
+                ExampleResourceModel()
             ) from e
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/data/taskdata.py` & `hmt-basemodels-1.0.0/basemodels/manifest/data/taskdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import Dict, Optional, Union, Any
+from typing import Dict, Optional, Union, Any, List, Tuple
 from uuid import UUID
 
 import requests
-from pydantic.v1 import BaseModel, HttpUrl, validate_model, ValidationError, validator, root_validator
-from pydantic.v1.error_wrappers import ErrorWrapper
+from pydantic import BaseModel, AnyHttpUrl, HttpUrl, ValidationError, field_validator, model_validator
+from pydantic_core.core_schema import ValidationInfo
 from requests import RequestException
 
 from basemodels.constants import SUPPORTED_CONTENT_TYPES
 
 
-# New type
-class AtLeastTenCharUrl(HttpUrl):
-    min_length = 10
+class Entity(BaseModel):
+    """Entity configuration"""
+
+    entity_id: UUID
+    entity_uri: AnyHttpUrl
+    coords: Tuple[int, int]
 
 
 class TaskDataEntry(BaseModel):
     """
     Taskdata file format:
 
     [
@@ -30,82 +33,70 @@
         "datapoint_uri": "https://domain.com/file2.jpg",
         "datapoint_text": {},
         "datapoint_hash": "f4acbe8562907183a484498ba901bfe5c5503aaa"
       }
     ]
     """
 
-    task_key: Optional[UUID]
-    datapoint_uri: Optional[HttpUrl]
-    datapoint_text: Optional[Dict[str, str]]
+    task_key: Optional[UUID] = None
+    datapoint_uri: Optional[HttpUrl] = None
+    entities: Optional[List[Entity]] = None
+    datapoint_text: Optional[Dict[str, str]] = None
+    datapoint_hash: Optional[str] = None
+    metadata: Optional[Dict[str, Optional[Union[str, int, float, Dict[str, Any]]]]] = None
 
-    @validator("datapoint_uri", always=True)
+    @field_validator("datapoint_uri")
     def validate_datapoint_uri(cls, value):
-        if value and len(value) < 10:
-            raise ValidationError("datapoint_uri need to be at least 10 char length.")
+        if value and len(str(value)) < 10:
+            raise ValueError("datapoint_uri need to be at least 10 char length.")
         return value
 
-    @validator("metadata")
+    @model_validator(mode="before")
+    def validate_task_data(cls, values):
+        """
+        Validate datapoint_uri.
+
+        Raise error if no datapoint_text and no value for URI.
+        """
+        if not values.get("datapoint_uri") and not values.get("datapoint_text"):
+            raise ValueError(f"datapoint_uri is missing. {list(values.keys())}")
+        return values
+
+    @field_validator("metadata")
     def validate_metadata(cls, value):
         if value is None:
             return value
 
         if len(value) > 10:
-            raise ValidationError("10 key max. in metadata")
+            raise ValueError("10 key max. in metadata")
 
         if len(str(value)) > 1024:
-            raise ValidationError("metadata should be < 1024")
+            raise ValueError("metadata should be < 1024")
 
         return value
 
-    datapoint_hash: Optional[str]
-    metadata: Optional[Dict[str, Optional[Union[str, int, float, Dict[str, Any]]]]]
-
-    @root_validator
-    def validate_datapoint_text(cls, values):
-        """
-        Validate datapoint_uri.
-
-        Raise error if no datapoint_text and no value for URI.
-        """
-        if not values.get("datapoint_uri") and not values.get("datapoint_text"):
-            raise ValueError("datapoint_uri is missing.")
-        return values
+    datapoint_hash: Optional[str] = None
+    metadata: Optional[Dict[str, Optional[Union[str, int, float, Dict[str, Any]]]]] = None
 
 
 def validate_content_type(uri: str) -> None:
     """Validate uri content type"""
     try:
         response = requests.head(uri, timeout=(3.5, 5))
         response.raise_for_status()
     except RequestException as e:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"taskdata content type ({uri}) validation failed"), "datapoint_uri")
-            ],
-            TaskDataEntry
-        ) from e
+        raise ValidationError(f"taskdata content type ({uri}) validation failed", TaskDataEntry()) from e
 
     content_type = response.headers.get("Content-Type", "")
     if content_type not in SUPPORTED_CONTENT_TYPES:
-        raise ValidationError(
-            [
-                ErrorWrapper(
-                    ValueError(f"taskdata entry datapoint_uri has unsupported type {content_type}"),
-                    "datapoint_uri"
-                )
-            ],
-            TaskDataEntry
-        )
+        raise ValidationError(f"taskdata entry datapoint_uri has unsupported type {content_type}", TaskDataEntry())
 
 
 def validate_taskdata_entry(value: dict, validate_image_content_type: bool) -> None:
     """Validate taskdata entry"""
     if not isinstance(value, dict):
         raise ValidationError("taskdata entry should be dict", TaskDataEntry())
 
-    *_, validation_error = validate_model(TaskDataEntry, value)
-    if validation_error:
-        raise validation_error
+    task_data = TaskDataEntry(**value)
 
     if validate_image_content_type:
-        validate_content_type(value["datapoint_uri"])
+        validate_content_type(task_data.datapoint_uri)
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/manifest.py` & `hmt-basemodels-1.0.0/basemodels/manifest/manifest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,191 +1,174 @@
 import json
 import uuid
 from datetime import datetime
 
 import requests
+from pydantic_core.core_schema import ValidationInfo
 from requests.exceptions import RequestException
 from typing_extensions import Literal
-from typing import Dict, Union, List, Optional, Any
+from typing import Any, Dict, List, Optional, Union
 from enum import Enum
 from uuid import UUID, uuid4
 from .data.groundtruth import validate_groundtruth_entry
 from .data.requester_question_example import validate_requester_example_image
 from .data.requester_restricted_answer_set import validate_requester_restricted_answer_set_uris
-from .data.taskdata import validate_taskdata_entry
-from pydantic.v1 import BaseModel, validator, ValidationError, validate_model, HttpUrl, AnyHttpUrl, root_validator
-from pydantic.v1.error_wrappers import ErrorWrapper
-from pydantic.v1.fields import Field
+from .data.taskdata import validate_taskdata_entry, Entity
+from pydantic import BaseModel, field_validator, ValidationError, HttpUrl, AnyHttpUrl, model_validator, ConfigDict
+from pydantic.fields import Field
 from decimal import Decimal
 from basemodels.manifest.restricted_audience import RestrictedAudience
-from basemodels.constants import JOB_TYPES_FOR_CONTENT_TYPE_VALIDATION
+from basemodels.constants import JOB_TYPES_FOR_CONTENT_TYPE_VALIDATION, BaseJobTypesEnum
 
 
 # A validator function for UUID fields
 def validate_uuid(cls, value):
     return value or uuid.uuid4()
 
 
-# Base job types
-class BaseJobTypesEnum(str, Enum):
-    image_label_binary = "image_label_binary"
-    image_label_multiple_choice = "image_label_multiple_choice"
-    text_free_entry = "text_free_entry"
-    text_label_multiple_span_select = "text_label_multiple_span_select"
-    text_multiple_choice_one_option = "text_multiple_choice_one_option"
-    text_multiple_choice_multiple_options = "text_multiple_choice_multiple_options"
-    image_label_area_adjust = "image_label_area_adjust"
-    image_label_area_select = "image_label_area_select"
-    image_label_single_polygon = "image_label_single_polygon"
-    image_label_multiple_polygons = "image_label_multiple_polygons"
-    image_label_semantic_segmentation_one_option = "image_label_semantic_segmentation_one_option"
-    image_label_semantic_segmentation_multiple_options = "image_label_semantic_segmentation_multiple_options"
-    image_label_text = "image_label_text"
-    multi_challenge = "multi_challenge"
-
-
 # Return a request type validator function
 class RequestTypeValidator(object):
     def __init__(self, multi_challenge: bool = True):
         self.multi_challenge = multi_challenge
 
-    def validate(self, cls, value, values):
+    def validate(cls, value, validation_info: ValidationInfo):
         """
         validate request types for all types of challenges
         multi_challenge should always have multi_challenge_manifests
         """
+        values = validation_info.data
         if value == BaseJobTypesEnum.multi_challenge:
-            if not self.multi_challenge:
-                raise ValidationError("multi_challenge request is not allowed here.")
+            if not cls.multi_challenge:
+                raise ValueError("multi_challenge request is not allowed here.")
             if "multi_challenge_manifests" not in values:
-                raise ValidationError("multi_challenge requires multi_challenge_manifests.")
+                raise ValueError("multi_challenge requires multi_challenge_manifests.")
         elif value in [BaseJobTypesEnum.image_label_multiple_choice, BaseJobTypesEnum.image_label_area_select]:
             if values.get("multiple_choice_min_choices", 1) > values.get("multiple_choice_max_choices", 1):
-                raise ValidationError("multiple_choice_min_choices cannot be greater than multiple_choice_max_choices")
+                raise ValueError("multiple_choice_min_choices cannot be greater than multiple_choice_max_choices")
         return value
 
 
 # Shape types enum
 class ShapeTypes(str, Enum):
     point = "point"
     bounding_box = "bounding_box"
     polygon = "polygon"
 
 
 class Model(BaseModel):
     def to_primitive(self):
-        return self.dict()
+        return self.model_dump()
 
-    # Helper function for using in the unittest
     def check(self, return_new=False):
-        self.__class__.validate(self.dict())
-        out_dict, _, validation_error = validate_model(self.__class__, self.__dict__)
-        if validation_error:
-            raise validation_error
-
+        validated_obj = self.__class__.model_validate(self.model_dump())
         # For compatibility with tests
         if return_new:
-            return self.__class__(**out_dict)
+            return validated_obj
 
 
 class Webhook(Model):
     """Model for webhook configuration"""
 
     webhook_id: UUID
-    chunk_completed: Optional[List[str]]
-    job_completed: Optional[List[str]]
+    chunk_completed: Optional[List[str]] = None
+    job_completed: Optional[List[str]] = None
 
     # States that might be interesting later
     # job_skipped: List[str] = None
     # job_inserted : List[str] = None
     # job_activated : List[str] = None
 
 
 class TaskData(BaseModel):
     """objects within taskdata list in Manifest"""
 
     task_key: UUID
-    datapoint_uri: Optional[AnyHttpUrl]
-    datapoint_text: Optional[Dict[str, str]]
-    datapoint_hash: str = Field(..., min_length=10, strip_whitespace=True)
+    datapoint_uri: Optional[AnyHttpUrl] = None
+    entities: Optional[List[Entity]] = None
+    polygon: Optional[List[int]] = None
+    datapoint_text: Optional[Dict[str, str]] = None
+    datapoint_hash: str = Field(..., min_length=10, json_schema_extra={"strip_whitespace": True})
 
-    @validator("datapoint_uri", always=True)
+    @field_validator("datapoint_uri")
     def validate_datapoint_uri(cls, value):
-        if value and len(value) < 10:
+        if value and len(str(value)) < 10:
             raise ValueError("datapoint_uri need to be at least 10 char length.")
         return value
 
-    @root_validator
-    def validate_datapoint_text(cls, values):
+    @model_validator(mode='before')
+    def validate_datapoint_text(cls, values: Dict[str, Any]):
         """
         Validate datapoint_uri.
 
         Raise error if no datapoint_text and no value for URI.
         """
         if not values.get("datapoint_uri") and not values.get("datapoint_text"):
             raise ValueError("datapoint_uri is missing.")
         return values
 
 
 class RequestConfig(Model):
     """definition of the request_config object in manifest"""
 
     version: int = 0
-    shape_type: Optional[ShapeTypes]
-    min_points: Optional[int]
-    max_points: Optional[int]
-    min_shapes_per_image: Optional[int]
-    max_shapes_per_image: Optional[int]
-    restrict_to_coords: Optional[bool]
-    minimum_selection_area_per_shape: Optional[int]
+    shape_type: Optional[ShapeTypes] = None
+    min_points: Optional[int] = None
+    max_points: Optional[int] = None
+    min_shapes_per_image: Optional[int] = None
+    max_shapes_per_image: Optional[int] = None
+    restrict_to_coords: Optional[bool] = None
+    minimum_selection_area_per_shape: Optional[int] =None
     multiple_choice_max_choices: Optional[int] = 1
     multiple_choice_min_choices: Optional[int] = 1
-    overlap_threshold: Optional[float]
+    overlap_threshold: Optional[float] = None
     answer_type: Optional[str] = "str"
-    max_value: Optional[float]
-    min_value: Optional[float]
-    max_length: Optional[int]
-    min_length: Optional[int]
-    sig_figs: Optional[int]
-    keep_answers_order: Optional[bool]
+    max_value: Optional[float] = None
+    min_value: Optional[float] = None
+    max_length: Optional[int] = None
+    min_length: Optional[int] = None
+    sig_figs: Optional[int] = None
+    keep_answers_order: Optional[bool] = None
     ignore_case: Optional[bool] = False
+    enable_hold_time: Optional[bool] = False
 
 
 class InternalConfig(Model):
     """discarded from incoming manifests"""
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    exchange: Optional[Dict[str, Union[str, int, float]]]
-    reco: Optional[Dict[str, Union[str, int, float]]]
-    repo: Optional[Dict[str, Union[str, int, float]]]
-    other: Optional[Dict[str, Union[str, int, float]]]
+    exchange: Optional[Dict[str, Union[str, int, float]]] = None
+    reco: Optional[Dict[str, Union[str, int, float]]] = None
+    repo: Optional[Dict[str, Union[str, int, float]]] = None
+    other: Optional[Dict[str, Union[str, int, float]]] = None
     # Accept one layer of nested
-    mitl: Optional[Dict[str, Union[str, int, float, Dict[str, Union[str, int, float]]]]]
-
-    class Config:
-        arbitrary_types_allowed = True
+    mitl: Optional[Dict[str, Union[str, int, float, Dict[str, Union[str, int, float]]]]] = None
 
 
 class NestedManifest(Model):
     """The nested manifest description for multi_challenge jobs"""
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     # We will set a default dynamic value for job_id
-    job_id: Optional[UUID]
-    validate_job_id = validator("job_id", always=True, allow_reuse=True)(validate_uuid)
+    job_id: Optional[UUID] = None
+    validate_job_id = field_validator("job_id")(validate_uuid)
 
     request_type: BaseJobTypesEnum
-    validate_request_type = validator("request_type", allow_reuse=True, always=True)(
-        RequestTypeValidator(multi_challenge=False).validate
-    )
-    requester_restricted_answer_set: Optional[Dict[str, Dict[str, str]]]
+    requester_restricted_answer_set: Optional[Dict[str, Dict[str, str]]] = None
+
+    @field_validator("request_type")
+    def validate_request_type(cls, value, validation_info: ValidationInfo):
+        request_validator = RequestTypeValidator(multi_challenge=False)
+        return request_validator.validate(value, validation_info)
 
-    @validator("requester_restricted_answer_set", always=True)
-    def validate_requester_restricted_answer_set(cls, value, values, **kwargs):
+    @field_validator("requester_restricted_answer_set")
+    def validate_requester_restricted_answer_set(cls, value, validation_info: ValidationInfo, **kwargs):
         """image_label_area_select should always have a single RAS set"""
 
         # validation runs before other params, so need to handle missing case
+        values = validation_info.data
         if "request_type" not in values:
             raise ValueError("request_type missing")
         if values["request_type"] == BaseJobTypesEnum.image_label_area_select:
             if not value or len(value.keys()) == 0:
                 value = {"label": {}}
                 values["requester_restricted_answer_set"] = value
         if values["request_type"] == BaseJobTypesEnum.image_label_multiple_choice:
@@ -195,136 +178,136 @@
                 )
             elif len(value.keys()) > 4:
                 raise ValueError(
                     "image_label_multiple_choice can not handle more than 4 options requester_restricted_answer_set"
                 )
         return value
 
-    requester_description: Optional[str]
+    requester_description: Optional[str] = None
     requester_max_repeats: int = 100
     requester_min_repeats: int = 1
-    requester_question: Optional[Dict[str, str]]
-    requester_question_example: Optional[Union[HttpUrl, List[HttpUrl]]]
+    requester_question: Optional[Dict[str, str]] = None
+    requester_question_example: Optional[Union[HttpUrl, List[HttpUrl]]] = None
 
-    @validator("requester_question_example")
-    def validate_requester_question_example(cls, value, values, **kwargs):
+    @field_validator("requester_question_example")
+    def validate_requester_question_example(cls, value, validation_info: ValidationInfo, **kwargs):
         # validation runs before other params, so need to handle missing case
+        values = validation_info.data
         if not ("request_type" in values):
             raise ValueError("request_type missing")
 
         # based on https://github.com/hCaptcha/hmt-basemodels/issues/27#issuecomment-590706643
         supports_lists = [BaseJobTypesEnum.image_label_area_select, BaseJobTypesEnum.image_label_binary]
 
         if isinstance(value, list) and not values["request_type"] in supports_lists:
             raise ValueError("Lists are not allowed in this challenge type")
         return value
 
     unsafe_content: bool = False
     requester_accuracy_target: float = 0.1
 
-    request_config: Optional[RequestConfig]
+    request_config: Optional[RequestConfig] = None
 
     # Groundtruth data is stored as a URL or optionally as an inlined json-serialized stringtype
-    groundtruth_uri: Optional[HttpUrl]
-    groundtruth: Optional[str]
+    groundtruth_uri: Optional[HttpUrl] = None
+    groundtruth: Optional[str] = None
 
-    @validator("groundtruth", always=True)
-    def validate_groundtruth(cls, v, values, **kwargs):
+    @field_validator("groundtruth")
+    def validate_groundtruth(cls, v, validation_info: ValidationInfo, **kwargs):
+        values = validation_info.data
         if "groundtruth_uri" in values and "groundtruth" in values:
             raise ValueError("Specify only groundtruth_uri or groundtruth, not both.")
         return v
 
     # Configuration id -- XXX LEGACY
-    confcalc_configuration_id: Optional[str]
-    webhook: Optional[Webhook]
-
-    class Config:
-        arbitrary_types_allowed = True
+    confcalc_configuration_id: Optional[str] = None
+    webhook: Optional[Webhook] = None
 
 
 class Manifest(Model):
     """The manifest description."""
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     job_mode: Literal["batch", "online", "instant_delivery"]
 
     # We will set a default dynamic value for job_api_key
-    job_api_key: Optional[UUID]
+    job_api_key: Optional[UUID] = None
 
     # We will set a default dynamic value for job_id
     job_id: UUID = Field(default_factory=uuid4)
 
     job_total_tasks: int
-    multi_challenge_manifests: Optional[List[NestedManifest]]
+    multi_challenge_manifests: Optional[List[NestedManifest]] = None
     request_type: BaseJobTypesEnum
-    network: Optional[str]
+    network: Optional[str] = None
     only_sign_results: bool = False
     public_results: bool = False
 
-    requester_restricted_answer_set: Optional[Dict[str, Dict[str, str]]]
+    requester_restricted_answer_set: Optional[Dict[str, Dict[str, str]]] = None
 
-    requester_description: Optional[str]
+    requester_description: Optional[str] = None
     requester_max_repeats: int = 100
     requester_min_repeats: int = 1
-    requester_question: Optional[Dict[str, str]]
+    requester_question: Dict[str, str]
 
-    requester_question_example: Optional[Union[HttpUrl, List[HttpUrl]]]
-    requester_example_extra_fields: Optional[Union[Dict[str, str], List[Union[Dict[str, str]]]]]
+    requester_question_example: Optional[Union[HttpUrl, List[HttpUrl]]] = None
+    requester_example_extra_fields: Optional[Union[Dict[str, str], List[Union[Dict[str, str]]]]] = None
 
     unsafe_content: bool = False
     task_bid_price: float
-    oracle_stake: Decimal
-    expiration_date: Optional[int]
-    start_date: Optional[int]
+    oracle_stake: float
+    expiration_date: Optional[int] = None
+    start_date: Optional[int] = None
     requester_accuracy_target: float = 0.1
-    manifest_smart_bounty_addr: Optional[str]
-    hmtoken_addr: Optional[str]
+    manifest_smart_bounty_addr: Optional[str] = None
+    hmtoken_addr: Optional[str] = None
     minimum_trust_server: float = 0.1
     minimum_trust_client: float = 0.1
-    recording_oracle_addr: Optional[str]
-    reputation_oracle_addr: Optional[str]
-    reputation_agent_addr: Optional[str]
-    requester_pgp_public_key: Optional[str]
-    ro_uri: Optional[str]
-    repo_uri: Optional[str]
-    batch_result_delivery_webhook: Optional[AnyHttpUrl]
-    online_result_delivery_webhook: Optional[AnyHttpUrl]
-    instant_result_delivery_webhook: Optional[AnyHttpUrl]
+    recording_oracle_addr: Optional[str] = None
+    reputation_oracle_addr: Optional[str] = None
+    reputation_agent_addr: Optional[str] = None
+    requester_pgp_public_key: Optional[str] = None
+    ro_uri: Optional[str] = None
+    repo_uri: Optional[str] = None
+    batch_result_delivery_webhook: Optional[AnyHttpUrl] = None
+    online_result_delivery_webhook: Optional[AnyHttpUrl] = None
+    instant_result_delivery_webhook: Optional[AnyHttpUrl] = None
 
-    request_config: Optional[RequestConfig]
+    request_config: Optional[RequestConfig] = None
 
     # If taskdata is directly provided
-    taskdata: Optional[List[TaskData]]
+    taskdata: Optional[List[TaskData]] = None
 
     # If taskdata is separately stored
-    taskdata_uri: Optional[AnyHttpUrl]
+    taskdata_uri: Optional[AnyHttpUrl] = None
 
     # Groundtruth data is stored as a URL or optionally as an inlined json-serialized stringtype
-    groundtruth_uri: Optional[AnyHttpUrl]
-    groundtruth: Optional[str]
+    groundtruth_uri: Optional[AnyHttpUrl] = None
+    groundtruth: Optional[str] = None
 
     # internal config options for param tests etc.
-    internal_config: Optional[InternalConfig]
+    internal_config: Optional[InternalConfig] = None
 
     # Configuration id
-    confcalc_configuration_id: Optional[str]
+    confcalc_configuration_id: Optional[str] = None
     restricted_audience: Optional[RestrictedAudience] = {}
 
-    webhook: Optional[Webhook]
+    webhook: Optional[Webhook] = None
 
-    rejected_uri: Optional[AnyHttpUrl]
-    rejected_count: Optional[int]
+    rejected_uri: Optional[AnyHttpUrl] = None
+    rejected_count: Optional[int] = None
 
     is_verification: bool = False
 
-    ##### Validators
+    # #### Validators
 
-    @root_validator
+    @model_validator(mode="before")
     def validate(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        start_date = values["start_date"]
-        expiration_date = values["expiration_date"]
+        start_date = values.get("start_date")
+        expiration_date = values.get("expiration_date")
         # validate at least taskdata or taskdata_uri is present
         taskdata = values.get("taskdata")
         taskdata_uri = values.get("taskdata_uri")
         if taskdata is not None and len(taskdata) > 0 and taskdata_uri is not None:
             raise ValueError("Specify only one of taskdata {} or taskdata_uri {}".format(taskdata, taskdata_uri))
         if taskdata is None and taskdata_uri is None:
             raise ValueError("No taskdata or taskdata_uri found in manifest")
@@ -341,31 +324,34 @@
 
         duration = datetime.utcfromtimestamp(expiration_date) - datetime.utcfromtimestamp(start_date)
         if 7 < duration.days:
             raise ValueError("Max job duration is 7 days.")
 
         return values
 
-    @validator("requester_min_repeats")
-    def validate_min_repeats(cls, v, values):
+    @field_validator("requester_min_repeats")
+    def validate_min_repeats(cls, v, validation_info: ValidationInfo):
         """min repeats are required to be at least 4 if ilmc"""
+        values = validation_info.data
         if values["request_type"] == "image_label_multiple_choice":
             return max(v, 4)
         return v
 
-    @validator("groundtruth", always=True)
-    def validate_groundtruth(cls, value, values):
+    @field_validator("groundtruth")
+    def validate_groundtruth(cls, value, validation_info: ValidationInfo):
+        values = validation_info.data
         if "groundtruth_uri" in values and "groundtruth" in values:
             raise ValueError("Specify only groundtruth_uri or groundtruth, not both.")
         return value
 
-    @validator("requester_restricted_answer_set", always=True)
-    def validate_requester_restricted_answer_set(cls, value, values, **kwargs):
+    @field_validator("requester_restricted_answer_set")
+    def validate_requester_restricted_answer_set(cls, value, validation_info: ValidationInfo, **kwargs):
         """image_label_area_select should always have a single RAS set"""
         # validation runs before other params, so need to handle missing case
+        values = validation_info.data
         if not ("request_type" in values):
             raise ValueError("request_type missing")
 
         if values["request_type"] == BaseJobTypesEnum.image_label_area_select:
             if not value or len(value.keys()) == 0:
                 value = {"label": {}}
                 values["requester_restricted_answer_set"] = value
@@ -377,41 +363,45 @@
                 )
             elif len(value.keys()) > 4:
                 raise ValueError(
                     "image_label_multiple_choice can not handle more than 4 options requester_restricted_answer_set"
                 )
         return value
 
-    @validator("requester_question_example")
-    def validate_requester_question_example(cls, value, values, **kwargs):
+    @field_validator("requester_question_example")
+    def validate_requester_question_example(cls, value, validation_info: ValidationInfo, **kwargs):
         # validation runs before other params, so need to handle missing case
+        values = validation_info.data
         if not ("request_type" in values):
             raise ValueError("request_type missing")
 
         # based on https://github.com/hCaptcha/hmt-basemodels/issues/27#issuecomment-590706643
         supports_lists = [
             BaseJobTypesEnum.image_label_area_select,
             BaseJobTypesEnum.image_label_binary,
         ]
 
         if isinstance(value, list) and not (values["request_type"] in supports_lists):
             raise ValueError("Lists are not allowed in this challenge type")
         return value
 
-    validate_request_type = validator("request_type", allow_reuse=True, always=True)(RequestTypeValidator().validate)
-    validate_job_api_key = validator("job_api_key", always=True, allow_reuse=True)(validate_uuid)
-    validate_job_id = validator("job_id", always=True, allow_reuse=True)(validate_uuid)
+    @field_validator("request_type")
+    def validate_request_type(cls, value, validation_info: ValidationInfo):
+        request_validator = RequestTypeValidator()
+        return request_validator.validate(value, validation_info)
 
-    class Config:
-        arbitrary_types_allowed = True
+    validate_job_api_key = field_validator("job_api_key")(validate_uuid)
+    validate_job_id = field_validator("job_id")(validate_uuid)
 
     def to_primitive(self):
         """Override primitive function to make it serializable."""
-        manifest_json = self.json()
-        return json.loads(manifest_json)
+        d = json.loads(self.model_dump_json())
+        if isinstance(self.restricted_audience, RestrictedAudience):
+            d["restricted_audience"] = self.restricted_audience.to_primitive()
+        return d
 
 
 def validate_groundtruth_uri(manifest: dict):
     """
     Validate groundtruth_uri
     Returns entries count if succeeded
     """
@@ -435,28 +425,18 @@
         else:
             for v in data:
                 entries_count += 1
                 validate_groundtruth_entry("", v, request_type, validate_image_content_type)
                 validate_image_content_type = False
 
     except (ValidationError, RequestException) as e:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"Validation failed for {uri}: {e}"), uri_key)
-            ],
-            Manifest
-        ) from e
+        raise ValidationError(f"Validation failed for {uri}: {e}", TaskData()) from e
 
     if entries_count == 0:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"fetched {uri} is empty"), uri_key)
-            ],
-            Manifest
-        )
+        raise ValidationError(f"fetched {uri} is empty", TaskData())
 
 
 def validate_taskdata_uri(manifest: dict):
     """
     Validate taskdata_uri
     Returns entries count if succeeded
     """
@@ -474,28 +454,18 @@
         data = response.json()
         for v in data:
             entries_count += 1
             validate_taskdata_entry(v, validate_image_content_type)
             validate_image_content_type = False  # We want to validate only first entry for content type
 
     except (ValidationError, RequestException) as e:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"Validation failed for {uri}: {e}"), uri_key)
-            ],
-            Manifest
-        ) from e
+        raise ValidationError(f"Validation failed for {uri}: {e}", TaskData())
 
     if entries_count == 0:
-        raise ValidationError(
-            [
-                ErrorWrapper(ValueError(f"fetched {uri} is empty"), uri_key)
-            ],
-            Manifest
-        )
+        raise ValidationError(f"fetched {uri} is empty"f"fetched {uri} is empty", TaskData())
 
 
 def validate_manifest_example_images(manifest: dict):
     """Fetch and validate the example resources."""
     question_example = manifest.get("requester_question_example")
     req_res_answer_set = manifest.get("requester_restricted_answer_set", {})
     if question_example:
```

### Comparing `hmt-basemodels-0.2.9/basemodels/manifest/restricted_audience.py` & `hmt-basemodels-1.0.0/basemodels/manifest/restricted_audience.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from enum import Enum
 from uuid import UUID
 from typing import Optional, List, Dict, Any
-from pydantic.v1 import BaseModel, root_validator, ValidationError, conint, confloat, validator
+from pydantic import (
+    BaseModel,
+    conint,
+    confloat,
+    field_validator,
+    model_validator,
+)
 
 
 class RestrictedAudienceBrowserEnum(str, Enum):
     mobile = "mobile"
     tablet = "tablet"
     desktop = "desktop"
     modern_browser = "modern_browser"
@@ -16,39 +22,43 @@
 
 
 class RestrictedAudienceScore(BaseModel):
     score: confloat(ge=0, le=1)
 
 
 class RestrictedAudience(BaseModel):
-    lang: Optional[List[Dict[str, RestrictedAudienceScore]]]
-    country: Optional[List[Dict[str, RestrictedAudienceScore]]]
-    sitekey: Optional[List[Dict[str, RestrictedAudienceScore]]]
-    serverdomain: Optional[List[Dict[str, RestrictedAudienceScore]]]
-    browser: Optional[List[Dict[RestrictedAudienceBrowserEnum, RestrictedAudienceScore]]]
-    confidence: Optional[List[Dict[RestrictedAudienceConfidenceEnum, RestrictedAudienceScore]]]
-    reason: Optional[List[Dict[str, RestrictedAudienceScore]]]
-    roles: Optional[List[Dict[str, RestrictedAudienceScore]]]
-
-    min_difficulty: Optional[conint(ge=0, le=4, strict=True)]
-    min_user_score: Optional[confloat(ge=0, le=1)]
-    max_user_score: Optional[confloat(ge=0, le=1)]
+    lang: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+    country: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+    sitekey: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+    serverdomain: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+    browser: Optional[List[Dict[RestrictedAudienceBrowserEnum, RestrictedAudienceScore]]] = None
+    confidence: Optional[List[Dict[RestrictedAudienceConfidenceEnum, RestrictedAudienceScore]]] = None
+    reason: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+    roles: Optional[List[Dict[str, RestrictedAudienceScore]]] = None
+
+    min_difficulty: Optional[conint(ge=0, le=4, strict=True)] = None
+    min_user_score: Optional[confloat(ge=0, le=1)] = None
+    max_user_score: Optional[confloat(ge=0, le=1)] = None
 
-    launch_group_id: Optional[conint(ge=0, strict=True)]
-    interests: Optional[List[conint(strict=True)]]
+    launch_group_id: Optional[conint(ge=0, strict=True)] = None
+    interests: Optional[List[conint(strict=True)]] = None
 
     def dict(self, **kwargs):
         kwargs["exclude_unset"] = True
-        return super().dict(**kwargs)
+        return super().model_dump(**kwargs)
 
     def json(self, **kwargs):
         kwargs["exclude_unset"] = True
-        return super().json(**kwargs)
+        return super().model_dump_json(**kwargs)
 
-    @root_validator()
+    def to_primitive(self, **kwargs):
+        kwargs["exclude_unset"] = True
+        return self.model_dump(**kwargs)
+
+    @model_validator(mode="before")
     def validate_score_fields(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         for entry, value in values.items():
             if value is None:
                 continue
             if entry in ["lang", "country", "browser", "sitekey", "serverdomain", "confidence"]:
                 if isinstance(value, list):
                     for restriction in value:
@@ -56,17 +66,17 @@
                             raise ValueError("only 1 element per list item is allowed")
                         key = next(iter(restriction))
                         if entry in ["lang", "country", "sitekey"]:
                             if str(key) != str(key).lower():
                                 raise ValueError("use lowercase")
         return values
 
-    @validator("sitekey")
+    @field_validator("sitekey")
     def validate_sitekey(cls, value):
         if value is not None:
             for restriction in value:
                 for sitekey in restriction:
                     try:
                         UUID(sitekey)
                     except:
-                        raise ValidationError("invalid sitekey")
+                        raise ValueError("invalid sitekey")
         return value
```

### Comparing `hmt-basemodels-0.2.9/basemodels/via.py` & `hmt-basemodels-1.0.0/basemodels/via.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.2.9/hmt_basemodels.egg-info/SOURCES.txt` & `hmt-basemodels-1.0.0/hmt_basemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.2.9/setup.py` & `hmt-basemodels-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 setuptools.setup(
     name="hmt-basemodels",
-    version="0.2.9",
+    version="1.0.0",
     author="HUMAN Protocol",
     description="Common data models shared by various components of the Human Protocol stack",
     url="https://github.com/hCaptcha/hmt-basemodels",
     include_package_data=True,
     zip_safe=True,
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
     packages=setuptools.find_packages(),
     install_requires=[
-        "requests>=2", "typing-extensions", "pydantic>=1.10.12"
+        "requests>=2", "typing-extensions", "pydantic>=2.5.3"
     ],
 )
```

### Comparing `hmt-basemodels-0.2.9/tests/test_manifest_validation.py` & `hmt-basemodels-1.0.0/tests/test_manifest_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import unittest
 from copy import deepcopy
 from datetime import datetime
 from typing import Any
 from uuid import uuid4
 
 import httpretty
-from pydantic.v1 import ValidationError
+from pydantic import ValidationError
 
 import basemodels
 from basemodels.manifest.data.taskdata import TaskDataEntry
 from basemodels.manifest.restricted_audience import RestrictedAudience
 
 CALLBACK_URL = "http://google.com/webback"
 FAKE_URL = "http://google.com/fake"
@@ -22,54 +22,54 @@
 REP_ORACLE = "0x61F9F0B31eacB420553da8BCC59DC617279731Ac"
 REC_ORACLE = "0xD979105297fB0eee83F7433fC09279cb5B94fFC6"
 FAKE_ORACLE = "0x1413862c2b7054cdbfdc181b83962cb0fc11fd92"
 
 
 # A helper function for create manifest models based on model library
 def create_manifest(data: dict):
-    return basemodels.Manifest.construct(**data)
+    return basemodels.Manifest.model_construct(**data)
 
 
 # A helper function for create nested manifest models based on model library
 def create_nested_manifest(data: dict):
-    return basemodels.NestedManifest.construct(**data)
+    return basemodels.NestedManifest.model_construct(**data)
 
 
 # A helper function for create nested manifest models based on model library
 def create_webhook(data: dict):
-    return basemodels.Webhook.construct(**data)
+    return basemodels.Webhook.model_construct(**data)
 
 
 # Json serializer for models based on libraries
 def to_json(model):
 
     # Pydantic json serializer
-    return model.json()
+    return model.model_dump_json()
 
 
 # A helper function for providing validatation function based on libraries
 def validate_func(model):
     return model.check
 
 
 # To be changed in runtime
 test_models = basemodels
 
 
 def get_data(
-        number_of_tasks=100,
-        bid_amount=1.0,
-        oracle_stake=0.05,
-        expiration_date=0,
-        minimum_trust=0.1,
-        request_type=IMAGE_LABEL_BINARY,
-        request_config=None,
-        job_mode="batch",
-        multi_challenge_manifests=None,
-        is_verification=None,
+    number_of_tasks=100,
+    bid_amount=1.0,
+    oracle_stake=0.05,
+    expiration_date=0,
+    minimum_trust=0.1,
+    request_type=IMAGE_LABEL_BINARY,
+    request_config=None,
+    job_mode="batch",
+    multi_challenge_manifests=None,
+    is_verification=None,
 ) -> dict:
     internal_config = {"exchange": {"a": 1, "b": "c"}}
     model = {
         "requester_restricted_answer_set": {
             "0": {"en": "English Answer 1"},
             "1": {
                 "en": "English Answer 2",
@@ -165,15 +165,15 @@
     "datapoint_text": {},
     "datapoint_hash": "f4acbe8562907183a484498ba901bfe5c5503aaa",
     "metadata": {
         "key_1": "value_1",
         "key_2": "value_2",
         "key_3": {
             "inner_key_1": "inner_value_1",
-        }
+        },
     },
 }
 
 
 class ManifestTest(unittest.TestCase):
     """Manifest specific tests, validating that models work the way we want"""
 
@@ -201,41 +201,41 @@
         manifest = get_data()
         manifest["taskdata_uri"] = None
         with self.assertRaises(ValidationError):
             basemodels.manifest.Manifest(**manifest)
 
     def test_can_make_request_config_job(self):
         """Test that jobs with valid request_config parameter work"""
-        manifest = a_manifest(
+        a_manifest(
             request_type="image_label_area_select",
             request_config={"shape_type": "point", "overlap_threshold": 0.8},
         )
 
     def test_can_make_nested_request_config_job_single_nest(self):
         """Test that jobs with valid nested request_config parameter work"""
         nested_manifest = a_nested_manifest(
             request_type="image_label_area_select",
             request_config={"shape_type": "point"},
         )
 
-        manifest = a_manifest(request_type="multi_challenge", multi_challenge_manifests=[nested_manifest])
+        a_manifest(request_type="multi_challenge", multi_challenge_manifests=[nested_manifest])
 
     def test_can_make_nested_request_config_job_multiple_nest(self):
         """Test that jobs with multiple valid nested request_config parameters work"""
         nested_manifest = a_nested_manifest(
             request_type="image_label_area_select",
             request_config={"shape_type": "point"},
         )
 
         nested_manifest_2 = a_nested_manifest(
             request_type="image_label_area_select",
             request_config={"shape_type": "point"},
         )
 
-        manifest = a_manifest(
+        a_manifest(
             request_type="multi_challenge",
             multi_challenge_manifests=[nested_manifest, nested_manifest_2],
         )
 
     def test_can_bad_request_config(self):
         """Test that an invalid shape_type in request_config will fail"""
         manifest = a_manifest()
@@ -327,16 +327,16 @@
         )
         self.assertEqual(2, manifest.to_primitive()["restricted_audience"]["min_difficulty"])
 
     def test_parse_restricted_audience(self):
         """Test None fields are skipped in restricted audience"""
         restricted_audience = {"min_difficulty": 2}
 
-        self.assertEqual(RestrictedAudience(**restricted_audience).dict(), {"min_difficulty": 2})
-        self.assertEqual(RestrictedAudience(**restricted_audience).json(), '{"min_difficulty": 2}')
+        self.assertEqual(RestrictedAudience(**restricted_audience).dict(), {"min_difficulty":2})
+        self.assertEqual(RestrictedAudience(**restricted_audience).json(), '{"min_difficulty":2}')
 
     def test_restricted_audience_only(self):
         def assert_raises(data):
             with self.assertRaises(ValidationError):
                 RestrictedAudience(**data)
 
         for data in [
@@ -420,19 +420,15 @@
         for data in [
             {"launch_group_id": "launch_group_id"},
             {"launch_group_id": -3},
             {"launch_group_id": 1.1},
         ]:
             assert_raises(data)
 
-        for data in [
-                {"interests": 1},
-                {"interests": {"mapped": 1}},
-                {"interests": ["as", "string"]}
-        ]:
+        for data in [{"interests": 1}, {"interests": {"mapped": 1}}, {"interests": ["as", "string"]}]:
             assert_raises(data)
 
         data = {
             "lang": [{"us": {"score": 0}}, {"es": {"score": 0.5}}, {"en-us": {"score": 1}}],
             "country": [{"us": {"score": 0}}, {"es": {"score": 0.5}}, {"it": {"score": 1}}],
             "browser": [
                 {"tablet": {"score": 0.5}},
@@ -447,15 +443,15 @@
                 {"3hcaptcha.com": {"score": 1}},
             ],
             "confidence": [{"minimum_client_confidence": {"score": 0.5}}],
             "min_difficulty": 2,
             "min_user_score": 0,
             "max_user_score": 0.3,
             "launch_group_id": 101,
-            "interests": [1,2,3,4],
+            "interests": [1, 2, 3, 4],
         }
 
         RestrictedAudience(**data)
 
     def test_realistic_multi_challenge_example(self):
         """validates a realistic multi_challenge manifest"""
         obj = {
@@ -524,15 +520,14 @@
                     "datapoint_uri": "http://test.com/task.jpg",
                     "task_key": "2279daef-d10a-4b0f-85d1-0ccbf7c8906b",
                 }
             ],
         }
 
         model = create_manifest(obj)
-        # print(model.to_primitive())
         self.assertTrue(validate_func(model)() is None)
 
     def test_both_timestamps_are_required(self):
         """validates both start_date & expiration_date must be passed at the same time."""
         # Given
         data = get_data()
         del data["expiration_date"]
@@ -609,15 +604,18 @@
 
         with self.assertRaises(ValidationError):
             validate_func(create_manifest(manifest))()
 
         del manifest["requester_question_example"]
         validate_func(create_manifest(manifest))()
 
-        manifest["requester_example_extra_fields"] = {"answer_example_uri": FAKE_URL, "answer_example_coords": "coords"}
+        manifest["requester_example_extra_fields"] = {
+            "answer_example_uri": FAKE_URL,
+            "answer_example_coords": "coords",
+        }
         manifest["request_type"] = "image_label_area_select"
         validate_func(create_manifest(manifest))()
 
         manifest["requester_example_extra_fields"] = [
             {"answer_example_uri": FAKE_URL, "answer_example_coords": "coords"}
         ]
         validate_func(create_manifest(manifest))()
@@ -808,47 +806,43 @@
         with self.assertRaises(ValidationError):
             self.validate_groundtruth_response("image_label_area_select", body)
 
     def test_groundtruth_uri_tlmss_valid(self):
         groundtruth_uri = "https://domain.com/file1.txt"
         body = {
             groundtruth_uri: [
-              {"start": 0, "end": 4, "label": "0"},
-              {"start": 17, "end": 89, "label": "1"},
+                {"start": 0, "end": 4, "label": "0"},
+                {"start": 17, "end": 89, "label": "1"},
             ]
         }
         self.register_http_response(groundtruth_uri, method=httpretty.HEAD, headers={"Content-Type": "text/plain"})
         self.validate_groundtruth_response("text_label_multiple_span_select", body)
 
-
     def test_groundtruth_uri_tlmss_invalid_key(self):
         body = {
             "not_uri": [
-              {"start": 0, "end": 4, "label": "0"},
-              {"start": 17, "end": 89, "label": "1"},
+                {"start": 0, "end": 4, "label": "0"},
+                {"start": 17, "end": 89, "label": "1"},
             ]
         }
 
         with self.assertRaises(ValidationError):
             self.validate_groundtruth_response("text_label_multiple_span_select", body)
 
-
     def test_groundtruth_uri_tlmss_invalid_value(self):
         body = {
             "https://www.domain.com/file1.txt": [
-              {"span": [0, 4]},
-              {"span": [17, 89], "label": "1"},
+                {"span": [0, 4]},
+                {"span": [17, 89], "label": "1"},
             ]
         }
 
         with self.assertRaises(ValidationError):
             self.validate_groundtruth_response("text_label_multiple_span_select", body)
 
-
-
     def test_groundtruth_uri_ilas_invalid_value(self):
         body = {"https://domain.com/file1.jpeg": [[True]]}
 
         with self.assertRaises(ValidationError):
             self.validate_groundtruth_response("image_label_area_select", body)
 
     def test_taskdata_empty(self):
@@ -968,23 +962,17 @@
         first_uri = "http://test.com/example-image1.jpg"
         second_uri = "http://test.com/example-image2.jpg"
         third_uri = "http://test.com/example-image3.jpg"
 
         manifest = {
             "requester_question_example": first_uri,
             "requester_restricted_answer_set": {
-                "0": {
-                    "answer_example_uri": second_uri,
-                    "en": "Test en2"
-                },
-                "1": {
-                    "answer_example_uri": third_uri,
-                    "en": "Test en3"
-                },
-            }
+                "0": {"answer_example_uri": second_uri, "en": "Test en2"},
+                "1": {"answer_example_uri": third_uri, "en": "Test en3"},
+            },
         }
         self.register_http_response(first_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
         self.register_http_response(second_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
         self.register_http_response(third_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
 
         test_models.validate_manifest_example_images(manifest)
 
@@ -993,23 +981,17 @@
         first_uri = "http://test.com/example-image1.jpg"
         second_uri = "http://test.com/example-image2.jpg"
         third_uri = "http://test.com/example-image3.jpg"
 
         manifest = {
             "requester_question_example": first_uri,
             "requester_restricted_answer_set": {
-                "0": {
-                    "answer_example_uri": second_uri,
-                    "en": "Test en2"
-                },
-                "1": {
-                    "answer_example_uri": third_uri,
-                    "en": "Test en3"
-                },
-            }
+                "0": {"answer_example_uri": second_uri, "en": "Test en2"},
+                "1": {"answer_example_uri": third_uri, "en": "Test en3"},
+            },
         }
         self.register_http_response(first_uri, method=httpretty.HEAD, headers={"Content-Type": "image/html"})
         self.register_http_response(second_uri, method=httpretty.HEAD, headers={"Content-Type": "image/html"})
         self.register_http_response(third_uri, method=httpretty.HEAD, headers={"Content-Type": "image/jpeg"})
         with self.assertRaises(ValidationError):
             test_models.validate_manifest_example_images(manifest)
 
@@ -1042,15 +1024,15 @@
 
         with self.assertRaises(ValidationError):
             taskdata["datapoint_text"] = {}
             taskdata["datapoint_uri"] = ""
             TaskDataEntry(**taskdata)
 
         with self.assertRaises(ValidationError):
-            taskdata["datapoint_uri"] = "http://com"
+            taskdata["datapoint_uri"] = "http//com"
             TaskDataEntry(**taskdata)
 
         taskdata["datapoint_uri"] = "https://domain.com/file1.jpg"
         TaskDataEntry(**taskdata)
 
 
 if __name__ == "__main__":
```

### Comparing `hmt-basemodels-0.2.9/tests/test_preprocess.py` & `hmt-basemodels-1.0.0/tests/test_preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from pydantic.v1.error_wrappers import ValidationError
+from pydantic import ValidationError
 from basemodels import Preprocess, Pipeline
 
 
 class PipelineTest(unittest.TestCase):
     def test_preprocess(self):
         config = {}
         p = Preprocess(pipeline=Pipeline.FaceBlurPipeline, config=config)
```

### Comparing `hmt-basemodels-0.2.9/tests/test_restricted_answer_set.py` & `hmt-basemodels-1.0.0/tests/test_restricted_answer_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import basemodels
 
-from pydantic.v1 import ValidationError
+from pydantic import ValidationError
 
 MANIFEST_VALUES = {
     "job_mode": "batch",
     "request_type": "image_label_multiple_choice",
     "job_total_tasks": 0,
     "task_bid_price": -1,
     "oracle_stake": 0.05,
@@ -24,17 +24,17 @@
 
 def create_manifest_from_test_method(nested_manifest: bool, data: dict):
     if nested_manifest:
         data.update(NESTED_MANIFEST_VALUES)
     else:
         data.update(MANIFEST_VALUES)
     if nested_manifest:
-        return basemodels.NestedManifest.construct(**data)
+        return basemodels.NestedManifest.model_construct(**data)
     else:
-        return basemodels.Manifest.construct(**data)
+        return basemodels.Manifest.model_construct(**data)
 
 
 def validate_manifest_from_test_method(manifest):
     manifest.check()
 
 
 def get_exception_type_from_test_method():
@@ -43,65 +43,58 @@
 
 class TestILMCRequesterRestrictedAnswerSet(unittest.TestCase):
     """
     Tests that the restricted answer set is properly validated for ILMC challenges
     """
 
     def check_rsa_validation(self, rsa: dict, should_pass: bool, nested_manifest: bool = False):
-        data = {"requester_restricted_answer_set": rsa}
+        data = {
+            "requester_question": {
+                "en": "Requester question",
+            },
+            "requester_restricted_answer_set": rsa,
+        }
         m = create_manifest_from_test_method(nested_manifest, data)
         if should_pass:
             validate_manifest_from_test_method(m)
         else:
             with self.assertRaises(get_exception_type_from_test_method()):
                 validate_manifest_from_test_method(m)
 
     def test_one_option(self):
-        self.check_rsa_validation(
-            rsa={"one": {"en": "one"}},
-            should_pass=False
-        )
+        self.check_rsa_validation(rsa={"one": {"en": "one"}}, should_pass=False)
 
     def test_one_option_nested(self):
-        self.check_rsa_validation(
-            rsa={"one": {"en": "one"}},
-            should_pass=False,
-            nested_manifest=True
-        )
+        self.check_rsa_validation(rsa={"one": {"en": "one"}}, should_pass=False, nested_manifest=True)
 
     def test_two_options(self):
-        self.check_rsa_validation(
-            rsa={"one": {"en": "one"}, "two": {"en": "two"}},
-            should_pass=True
-        )
+        self.check_rsa_validation(rsa={"one": {"en": "one"}, "two": {"en": "two"}}, should_pass=True)
 
     def test_two_options_nested(self):
         self.check_rsa_validation(
-            rsa={"one": {"en": "one"}, "two": {"en": "two"}},
-            should_pass=True,
-            nested_manifest=True
+            rsa={"one": {"en": "one"}, "two": {"en": "two"}}, should_pass=True, nested_manifest=True
         )
 
     def test_five_options(self):
         self.check_rsa_validation(
             rsa={
                 "one": {"en": "one"},
                 "two": {"en": "two"},
                 "three": {"en": "three"},
                 "four": {"en": "four"},
-                "five": {"en": "five"}
+                "five": {"en": "five"},
             },
-            should_pass=False
+            should_pass=False,
         )
 
     def test_five_options_nested(self):
         self.check_rsa_validation(
             rsa={
                 "one": {"en": "one"},
                 "two": {"en": "two"},
                 "three": {"en": "three"},
                 "four": {"en": "four"},
-                "five": {"en": "five"}
+                "five": {"en": "five"},
             },
             should_pass=False,
-            nested_manifest=True
+            nested_manifest=True,
         )
```

