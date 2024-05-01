# Comparing `tmp/isic-metadata-1.5.0.tar.gz` & `tmp/isic_metadata-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-metadata-1.5.0.tar", last modified: Fri Mar 29 20:07:33 2024, max compression
+gzip compressed data, was "isic_metadata-1.6.0.tar", last modified: Wed May  1 17:49:57 2024, max compression
```

## Comparing `isic-metadata-1.5.0.tar` & `isic_metadata-1.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.045367 isic-metadata-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.041366 isic-metadata-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.041366 isic-metadata-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-29 20:07:33.045367 isic-metadata-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.041366 isic-metadata-1.5.0/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/isic_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/isic_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.045367 isic-metadata-1.5.0/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-29 20:07:33.000000 isic-metadata-1.5.0/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-29 20:07:33.000000 isic-metadata-1.5.0/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:07:33.000000 isic-metadata-1.5.0/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 20:07:33.000000 isic-metadata-1.5.0/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 20:07:33.000000 isic-metadata-1.5.0/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:07:33.045367 isic-metadata-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:33.045367 isic-metadata-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tests/test_dependent_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-29 20:07:18.000000 isic-metadata-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.774659 isic_metadata-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.778658 isic_metadata-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.778658 isic_metadata-1.6.0/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/isic_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 17:49:57.000000 isic_metadata-1.6.0/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:57.782658 isic_metadata-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_dependent_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-01 17:49:39.000000 isic_metadata-1.6.0/tox.ini
```

### Comparing `isic-metadata-1.5.0/.github/workflows/ci.yml` & `isic_metadata-1.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/.github/workflows/release.yml` & `isic_metadata-1.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/.gitignore` & `isic_metadata-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/LICENSE` & `isic_metadata-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/PKG-INFO` & `isic_metadata-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.5.0
+Version: 1.6.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-1.5.0/isic_metadata/__init__.py` & `isic_metadata-1.6.0/isic_metadata/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
+import contextlib
 from dataclasses import dataclass
 from importlib.metadata import PackageNotFoundError, version
 from typing import Any, Literal
 
-try:
+with contextlib.suppress(PackageNotFoundError):
     __version__ = version("isic-metadata")
-except PackageNotFoundError:
-    # package is not installed
-    pass
 
 
 @dataclass()
 class SearchConfig:
     key: str
     es_property: dict[str, Any]
     es_facet: dict[str, Any]
@@ -129,15 +127,15 @@
                     }
                 },
             )
         ),
     }
 )
 
-for field in FIELD_REGISTRY.keys():
+for field in FIELD_REGISTRY:
     if field in [
         "blurry",
         "color_tint",
         "dermoscopic_type",
         "hairy",
         "image_type",
         "marker_pen",
```

### Comparing `isic-metadata-1.5.0/isic_metadata/fields.py` & `isic_metadata-1.6.0/isic_metadata/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return value
 
     @staticmethod
     def clamp_upper_bound(value: int) -> int:
         return min(value, 85)
 
 
-# todo indeterminable
+# TODO: indeterminable
 class BenignMalignantEnum(str, Enum):
     benign = "benign"
     malignant = "malignant"
     indeterminate = "indeterminate"
     indeterminate_benign = "indeterminate/benign"
     indeterminate_malignant = "indeterminate/malignant"
 
@@ -108,16 +108,16 @@
     plexiform_spindle_cell = "plexiform spindle cell"
     special_site = "special site"
     spitz = "spitz"
 
 
 class ImageTypeEnum(str, Enum):
     dermoscopic = "dermoscopic"
-    clinical_close_up = "clinical: close-up"
     clinical_overview = "clinical: overview"
+    clinical_close_up = "clinical: close-up"
     tbp_tile_close_up = "TBP tile: close-up"
     tbp_tile_overview = "TBP tile: overview"
 
 
 class DermoscopicTypeEnum(str, Enum):
     contact_polarized = "contact polarized"
     contact_non_polarized = "contact non-polarized"
```

### Comparing `isic-metadata-1.5.0/isic_metadata/metadata.py` & `isic_metadata-1.6.0/isic_metadata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Any, Literal
+from typing import Annotated, Any, Literal
 
-from annotated_types import Ge
+from annotated_types import Ge  # noqa: TCH002
 from pydantic import (
     AfterValidator,
     BaseModel,
     BeforeValidator,
     ConfigDict,
     ValidationError,
     field_validator,
     model_validator,
 )
 from pydantic_core import ErrorDetails, PydanticCustomError
-from typing_extensions import Annotated
 
 from isic_metadata.fields import (
     Age,
     AnatomSiteGeneralEnum,
     BenignMalignantEnum,
     ClinSizeLongDiamMm,
     ColorTintEnum,
@@ -111,15 +110,15 @@
 
     This is useful for performing checks that span across multiple rows.
     """
 
     items: list[MetadataRow]
 
     @model_validator(mode="after")
-    def check_patients_lesions(self) -> "MetadataBatch":
+    def check_patients_lesions(self) -> MetadataBatch:
         lesion_to_patients: dict[str, set[str]] = defaultdict(set)
 
         for item in self.items:
             if item.patient_id and item.lesion_id:
                 lesion_to_patients[item.lesion_id].add(item.patient_id)
 
         bad_lesions = [
@@ -223,15 +222,15 @@
     @classmethod
     def lower(cls, v: Any) -> Any:
         if isinstance(v, str):
             v = v.lower()
         return v
 
     @model_validator(mode="after")
-    def validate_no_benign_melanoma(self) -> "MetadataRow":
+    def validate_no_benign_melanoma(self) -> MetadataRow:
         if not self.benign_malignant:
             return self
 
         if (self.diagnosis == "melanoma" and self.benign_malignant == "benign") or (
             self.diagnosis == "nevus"
             and self.benign_malignant
             not in [
@@ -246,68 +245,70 @@
                 self.diagnosis.value,
                 self.benign_malignant.value,
             )
 
         return self
 
     @model_validator(mode="after")
-    def validate_non_nevus_diagnoses(self) -> "MetadataRow":
+    def validate_non_nevus_diagnoses(self) -> MetadataRow:
         if not self.nevus_type:
             return self
 
         if not self.diagnosis:
             raise error_missing_field("nevus_type", "diagnosis")
-        elif self.diagnosis not in [
+
+        if self.diagnosis not in [
             DiagnosisEnum.nevus,
             DiagnosisEnum.nevus_spilus,
         ]:
             raise error_incompatible_fields("nevus_type", "diagnosis", field2_value=self.diagnosis)
 
         return self
 
     @model_validator(mode="after")
-    def validate_melanoma_fields(self) -> "MetadataRow":
+    def validate_melanoma_fields(self) -> MetadataRow:
         melanoma_fields: list[str] = [
             "mel_class",
             "mel_mitotic_index",
             "mel_thick_mm",
             "mel_type",
             "mel_ulcer",
         ]
 
         for field in melanoma_fields:
             if not getattr(self, field):
                 continue
 
             if not self.diagnosis:
                 raise error_missing_field(field, "diagnosis", field2_value="melanoma")
-            elif self.diagnosis != "melanoma":
+
+            if self.diagnosis != "melanoma":
                 raise error_incompatible_fields(
                     field, "diagnosis", field2_value=self.diagnosis.value
                 )
 
         return self
 
     @model_validator(mode="after")
-    def validate_dermoscopic_fields(self) -> "MetadataRow":
+    def validate_dermoscopic_fields(self) -> MetadataRow:
         if not self.dermoscopic_type:
             return self
 
         if not self.image_type:
             raise error_missing_field("dermoscopic_type", "image_type")
 
         if self.image_type != ImageTypeEnum.dermoscopic:
             raise error_incompatible_fields(
                 "dermoscopic_type", "image_type", field2_value="dermoscopic"
             )
 
         return self
 
     @model_validator(mode="after")
-    def validate_tbp_tile_fields(self) -> "MetadataRow":
+    def validate_tbp_tile_fields(self) -> MetadataRow:
         if not self.tbp_tile_type:
             return self
 
         if not self.image_type:
             raise error_missing_field("tbp_tile_type", "image_type")
 
         if self.image_type not in [
@@ -317,15 +318,15 @@
             raise error_incompatible_fields(
                 "tbp_tile_type", "image_type", field2_value=self.image_type.value
             )
 
         return self
 
     @model_validator(mode="after")
-    def validate_concomitant_biopsy(self) -> "MetadataRow":
+    def validate_concomitant_biopsy(self) -> MetadataRow:
         if self.concomitant_biopsy and (
             not self.diagnosis_confirm_type or self.diagnosis_confirm_type != "histopathology"
         ):
             raise error_missing_field(
                 "concomitant_biopsy", "diagnosis_confirm_type", field2_value="histopathology"
             )
```

### Comparing `isic-metadata-1.5.0/isic_metadata.egg-info/PKG-INFO` & `isic_metadata-1.6.0/isic_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.5.0
+Version: 1.6.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic-metadata-1.5.0/isic_metadata.egg-info/SOURCES.txt` & `isic_metadata-1.6.0/isic_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/setup.py` & `isic_metadata-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/tests/test_batch.py` & `isic_metadata-1.6.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `isic-metadata-1.5.0/tests/test_dependent_fields.py` & `isic_metadata-1.6.0/tests/test_dependent_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,33 +18,33 @@
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"diagnosis": "nevus", "benign_malignant": benign_malignant})
     assert len(excinfo.value.errors()) == 1
     assert "nevus is incompatible with benign_malignant" in excinfo.value.errors()[0]["msg"]
 
 
 @pytest.mark.parametrize(
-    ["diagnosis", "error_message"],
-    [[None, "requires setting diagnosis"], ["melanoma", "is incompatible with diagnosis"]],
+    ("diagnosis", "error_message"),
+    [(None, "requires setting diagnosis"), ("melanoma", "is incompatible with diagnosis")],
 )
 def test_nevus_type_needs_nevus_diagnosis(diagnosis: str | None, error_message: str):
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"diagnosis": diagnosis, "nevus_type": "spitz"})
     assert len(excinfo.value.errors()) == 1
     assert f"nevus_type {error_message}" in excinfo.value.errors()[0]["msg"]
 
 
 @pytest.mark.parametrize("diagnosis", [None, "basal cell carcinoma"])
 @pytest.mark.parametrize(
-    "field_name, field_value",
+    ("field_name", "field_value"),
     [
-        ["mel_class", "melanoma in situ"],
-        ["mel_mitotic_index", "4/mm^2"],
-        ["mel_thick_mm", "4mm"],
-        ["mel_type", "nodular melanoma"],
-        ["mel_ulcer", True],
+        ("mel_class", "melanoma in situ"),
+        ("mel_mitotic_index", "4/mm^2"),
+        ("mel_thick_mm", "4mm"),
+        ("mel_type", "nodular melanoma"),
+        ("mel_ulcer", True),
     ],
 )
 def test_melanoma_fields_require_melanoma_diagnosis(
     diagnosis: str | None, field_name: str, field_value: Any
 ):
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({field_name: field_value, "diagnosis": diagnosis})
```

### Comparing `isic-metadata-1.5.0/tests/test_fields.py` & `isic_metadata-1.6.0/tests/test_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Any
 
-from hypothesis import given, strategies as st
+from hypothesis import given
+from hypothesis import strategies as st
 from pydantic import ValidationError
 import pytest
 
 from isic_metadata.metadata import MetadataRow, convert_errors
 
 
 @pytest.mark.parametrize(
-    "field, str_value, parsed_value, dependent_fields",
+    ("field", "str_value", "parsed_value", "dependent_fields"),
     # dependent_fields is a dict of field names to values are there just to satisfy
     # the field validators.
     [
-        ["age", "54", 54, {}],
-        ["melanocytic", "True", True, {}],
-        ["clin_size_long_diam_mm", "4mm", 4.0, {}],
-        ["mel_thick_mm", ".33mm", 0.33, {"diagnosis": "melanoma"}],
-        ["mel_ulcer", "false", False, {"diagnosis": "melanoma"}],
-        ["family_hx_mm", "False", False, {}],
-        ["personal_hx_mm", "0", False, {}],
-        ["acquisition_day", "142", 142, {}],
+        ("age", "54", 54, {}),
+        ("melanocytic", "True", True, {}),
+        ("clin_size_long_diam_mm", "4mm", 4.0, {}),
+        ("mel_thick_mm", ".33mm", 0.33, {"diagnosis": "melanoma"}),
+        ("mel_ulcer", "false", False, {"diagnosis": "melanoma"}),
+        ("family_hx_mm", "False", False, {}),
+        ("personal_hx_mm", "0", False, {}),
+        ("acquisition_day", "142", 142, {}),
     ],
 )
 def test_non_str_types(
     field: str, str_value: str, parsed_value: Any, dependent_fields: dict[str, Any]
 ):
     as_str = MetadataRow.model_validate({field: str_value, **dependent_fields})
     as_real = MetadataRow.model_validate({field: parsed_value, **dependent_fields})
@@ -54,15 +55,16 @@
     # mel_class can only be set if diagnosis is melanoma
     MetadataRow.model_validate({"diagnosis": "melanoma", "mel_class": "invasive melanoma"})
 
 
 @given(age=st.integers(min_value=0).map(str))
 def test_age_ceiling(age: str):
     metadata = MetadataRow.model_validate({"age": age})
-    assert metadata.age is not None and metadata.age <= 85
+    assert metadata.age is not None
+    assert metadata.age <= 85
 
 
 def test_age_special_case():
     assert MetadataRow.model_validate({"age": "85+"}).age == 85
 
 
 def test_fitzpatrick_skin_type():
@@ -74,21 +76,21 @@
 
 
 def test_nevus_diagnosis():
     MetadataRow.model_validate({"diagnosis": "nevus", "nevus_type": "blue"})
 
 
 @pytest.mark.parametrize(
-    ["raw", "parsed"],
+    ("raw", "parsed"),
     [
-        ["4.5 mm", 4.5],
-        ["14.2   mm", 14.2],
-        ["4.5mm", 4.5],
-        ["1mm", 1.0],
-        ["3.25", 3.25],
+        ("4.5 mm", 4.5),
+        ("14.2   mm", 14.2),
+        ("4.5mm", 4.5),
+        ("1mm", 1.0),
+        ("3.25", 3.25),
     ],
 )
 def test_mel_thick_mm(raw: str, parsed: float):
     metadata = MetadataRow.model_validate({"diagnosis": "melanoma", "mel_thick_mm": raw})
     assert metadata.mel_thick_mm == parsed
```

