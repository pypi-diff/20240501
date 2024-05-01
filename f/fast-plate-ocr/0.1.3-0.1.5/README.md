# Comparing `tmp/fast_plate_ocr-0.1.3.tar.gz` & `tmp/fast_plate_ocr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_plate_ocr-0.1.3.tar", max compression
+gzip compressed data, was "fast_plate_ocr-0.1.5.tar", max compression
```

## Comparing `fast_plate_ocr-0.1.3.tar` & `fast_plate_ocr-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-05-01 19:35:41.833824 fast_plate_ocr-0.1.3/LICENSE
--rw-r--r--   0        0        0    12612 2024-05-01 19:35:41.833824 fast_plate_ocr-0.1.3/README.md
--rw-r--r--   0        0        0      140 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/__init__.py
--rw-r--r--   0        0        0      802 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/cli.py
--rw-r--r--   0        0        0     2696 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/onnx_converter.py
--rw-r--r--   0        0        0     6576 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/train.py
--rw-r--r--   0        0        0     1773 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/valid.py
--rw-r--r--   0        0        0     4344 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_augmentation.py
--rw-r--r--   0        0        0     2662 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_predictions.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/common/__init__.py
--rw-r--r--   0        0        0     1235 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/common/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/config.py
--rw-r--r--   0        0        0     3548 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/hub.py
--rw-r--r--   0        0        0     7684 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/onnx_inference.py
--rw-r--r--   0        0        0     2726 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/process.py
--rw-r--r--   0        0        0      752 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/__init__.py
--rw-r--r--   0        0        0      804 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/augmentation.py
--rw-r--r--   0        0        0     1681 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/dataset.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/__init__.py
--rw-r--r--   0        0        0     1452 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/config.py
--rw-r--r--   0        0        0     2601 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/custom.py
--rw-r--r--   0        0        0     2400 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/layer_blocks.py
--rw-r--r--   0        0        0     2709 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/models.py
--rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/__init__.py
--rw-r--r--   0        0        0      900 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/backend_utils.py
--rw-r--r--   0        0        0     5345 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/utils.py
--rw-r--r--   0        0        0     3858 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/LICENSE
+-rw-r--r--   0        0        0    12612 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/README.md
+-rw-r--r--   0        0        0      140 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/__init__.py
+-rw-r--r--   0        0        0      802 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/onnx_converter.py
+-rw-r--r--   0        0        0     6576 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/train.py
+-rw-r--r--   0        0        0     1773 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/valid.py
+-rw-r--r--   0        0        0     4344 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_augmentation.py
+-rw-r--r--   0        0        0     2662 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_predictions.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/common/__init__.py
+-rw-r--r--   0        0        0     1235 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/common/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/config.py
+-rw-r--r--   0        0        0     3548 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/hub.py
+-rw-r--r--   0        0        0     7684 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/onnx_inference.py
+-rw-r--r--   0        0        0     2726 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/process.py
+-rw-r--r--   0        0        0      752 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/augmentation.py
+-rw-r--r--   0        0        0     1681 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/__init__.py
+-rw-r--r--   0        0        0     1452 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/config.py
+-rw-r--r--   0        0        0     2601 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/custom.py
+-rw-r--r--   0        0        0     2400 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/layer_blocks.py
+-rw-r--r--   0        0        0     2709 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/backend_utils.py
+-rw-r--r--   0        0        0     5345 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/utils.py
+-rw-r--r--   0        0        0     3858 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.5/PKG-INFO
```

### Comparing `fast_plate_ocr-0.1.3/LICENSE` & `fast_plate_ocr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/README.md` & `fast_plate_ocr-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/cli.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/onnx_converter.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/onnx_converter.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/train.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/train.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/valid.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/valid.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_augmentation.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_predictions.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_predictions.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/common/utils.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/common/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/config.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/hub.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/hub.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/onnx_inference.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/process.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/process.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/utils.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/augmentation.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/dataset.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/config.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/custom.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/custom.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/layer_blocks.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/layer_blocks.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/models.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/models.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/backend_utils.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/backend_utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/utils.py` & `fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.3/pyproject.toml` & `fast_plate_ocr-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-plate-ocr"
-version = "0.1.3"
+version = "0.1.5"
 description = "Fast & Lightweight OCR for vehicle license plates."
 authors = ["ankandrew <61120139+ankandrew@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/ankandrew/fast-plate-ocr/"
 documentation = "https://ankandrew.github.io/fast-plate-ocr"
 keywords = ["plate-recognition", "license-plate-recognition", "license-plate-ocr"]
 license = "MIT"
```

### Comparing `fast_plate_ocr-0.1.3/PKG-INFO` & `fast_plate_ocr-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-plate-ocr
-Version: 0.1.3
+Version: 0.1.5
 Summary: Fast & Lightweight OCR for vehicle license plates.
 Home-page: https://github.com/ankandrew/fast-plate-ocr/
 License: MIT
 Keywords: plate-recognition,license-plate-recognition,license-plate-ocr
 Author: ankandrew
 Author-email: 61120139+ankandrew@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

