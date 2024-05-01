# Comparing `tmp/fast_plate_ocr-0.1.2.tar.gz` & `tmp/fast_plate_ocr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_plate_ocr-0.1.2.tar", max compression
+gzip compressed data, was "fast_plate_ocr-0.1.3.tar", max compression
```

## Comparing `fast_plate_ocr-0.1.2.tar` & `fast_plate_ocr-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/LICENSE
--rw-r--r--   0        0        0    12182 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/README.md
--rw-r--r--   0        0        0      140 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/__init__.py
--rw-r--r--   0        0        0      802 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/cli.py
--rw-r--r--   0        0        0     2665 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/onnx_converter.py
--rw-r--r--   0        0        0     6300 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/train.py
--rw-r--r--   0        0        0     1773 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/valid.py
--rw-r--r--   0        0        0     4344 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_augmentation.py
--rw-r--r--   0        0        0     2662 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_predictions.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/common/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/common/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/config.py
--rw-r--r--   0        0        0     3548 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/hub.py
--rw-r--r--   0        0        0     7684 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/onnx_inference.py
--rw-r--r--   0        0        0     2726 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/process.py
--rw-r--r--   0        0        0      752 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/py.typed
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/__init__.py
--rw-r--r--   0        0        0      804 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/augmentation.py
--rw-r--r--   0        0        0     1615 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/__init__.py
--rw-r--r--   0        0        0     1452 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/config.py
--rw-r--r--   0        0        0     2601 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/custom.py
--rw-r--r--   0        0        0     2400 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/layer_blocks.py
--rw-r--r--   0        0        0     2709 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/models.py
--rw-r--r--   0        0        0        0 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/__init__.py
--rw-r--r--   0        0        0      900 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/backend_utils.py
--rw-r--r--   0        0        0     5345 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/utils.py
--rw-r--r--   0        0        0     3858 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14474 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-01 19:35:41.833824 fast_plate_ocr-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12612 2024-05-01 19:35:41.833824 fast_plate_ocr-0.1.3/README.md
+-rw-r--r--   0        0        0      140 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/__init__.py
+-rw-r--r--   0        0        0      802 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/onnx_converter.py
+-rw-r--r--   0        0        0     6576 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/train.py
+-rw-r--r--   0        0        0     1773 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/valid.py
+-rw-r--r--   0        0        0     4344 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_augmentation.py
+-rw-r--r--   0        0        0     2662 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_predictions.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/common/__init__.py
+-rw-r--r--   0        0        0     1235 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/common/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/config.py
+-rw-r--r--   0        0        0     3548 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/hub.py
+-rw-r--r--   0        0        0     7684 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/onnx_inference.py
+-rw-r--r--   0        0        0     2726 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/process.py
+-rw-r--r--   0        0        0      752 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/inference/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/augmentation.py
+-rw-r--r--   0        0        0     1681 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/__init__.py
+-rw-r--r--   0        0        0     1452 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/config.py
+-rw-r--r--   0        0        0     2601 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/custom.py
+-rw-r--r--   0        0        0     2400 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/layer_blocks.py
+-rw-r--r--   0        0        0     2709 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/backend_utils.py
+-rw-r--r--   0        0        0     5345 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/utils.py
+-rw-r--r--   0        0        0     3858 2024-05-01 19:35:41.837824 fast_plate_ocr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.3/PKG-INFO
```

### Comparing `fast_plate_ocr-0.1.2/LICENSE` & `fast_plate_ocr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/README.md` & `fast_plate_ocr-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 **Lightweight** and **fast** OCR models for license plate text recognition. You can train models from scratch or use
 the trained models for inference.
 
 The idea is to use this after a plate object detector, since the OCR expects the cropped plates.
 
 ### Features
 
-- **Keras 3 Backend Support**: Compatible with **TensorFlow**, **JAX**, and **PyTorch** backends 🧠
-- **Augmentation Variety**: Diverse augmentations via **Albumentations** library 🖼️
+- **Keras 3 Backend Support**: Compatible with **[TensorFlow](https://www.tensorflow.org/)**, **[JAX](https://github.com/google/jax)**, and **[PyTorch](https://pytorch.org/)** backends 🧠
+- **Augmentation Variety**: Diverse **augmentations** via **[Albumentations](https://albumentations.ai/)** library 🖼️
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
-- **ONNX Runtime Inference**: **Fast** and **optimized** inference with ONNX runtime ⚡
+- **ONNX Runtime Inference**: **Fast** and **optimized** inference with **[ONNX runtime](https://onnxruntime.ai/)** ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
-- **Model HUB**: Access to a collection of pre-trained models ready for inference 🌟
+- **Model HUB**: Access to a collection of **pre-trained models** ready for inference 🌟
 
 ### Available Models
 
 |          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
 |:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
 | argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
 
 _<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
-_<sup>[2]</sup> Accuracy is what we refer as plate_acc. See metrics section._
+_<sup>[2]</sup> Accuracy is what we refer as plate_acc. See [metrics section](#model-metrics)._
 
 
 <details>
   <summary>Reproduce results.</summary>
 
 * Calculate Inference Time:
 
@@ -159,27 +159,28 @@
 2. A labeled dataset,
    see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)
    for the expected data format.
 3. Run train script:
     ```shell
     # You can set the backend to either TensorFlow, JAX or PyTorch
     # (just make sure it is installed)
-    !KERAS_BACKEND=tensorflow fast_plate_ocr train \
+    KERAS_BACKEND=tensorflow fast_plate_ocr train \
         --annotations path_to_the_train.csv \
         --val-annotations path_to_the_val.csv \
+        --config-file config.yaml \
         --batch-size 128 \
         --epochs 750 \
         --dense \
         --early-stopping-patience 100 \
         --reduce-lr-patience 50
     ```
 
-You will probably want to change the augmentation pipeline to apply to your dataset. In order to do this
+You will probably want to change the augmentation pipeline to apply to your dataset.
 
-Define Albumentations pipeline:
+In order to do this define an Albumentations pipeline:
 
 ```python
 import albumentations as A
 
 transform_pipeline = A.Compose(
     [
         # ...
@@ -286,22 +287,25 @@
 Each head will output a probability distribution over the `vocabulary` specified during training. So the output
 prediction for a single plate will be of shape `(max_plate_slots, vocabulary_size)`.
 
 ### Model Metrics
 
 During training, you will see the following metrics
 
-* **plate_acc**: Compute how many plates were correctly classified. For a single plate, if ground truth is `ABC123`, and
-  the prediction is 'ABC 123', then this would give a score of 1. If the prediction was ABD 123, it would
-  score 0.
-* **cat_acc**: Calculates how many characters of the plate were correctly classified. Example if the correct label is
-  `ABC123` and `ABC133` is predicted, it will not give a precision of 0% like plate_acc (not completely
-  classified correctly), but 83.3% (5/6).
-* **top_3_k**: Calculates how often the true character is found in the top-3 predictions (the 3 with the highest
-  probability).
+* **plate_acc**: Compute the number of **license plates** that were **fully classified**. For a single plate, if the
+  ground truth is `ABC123` and the prediction is also `ABC123`, it would score 1. However, if the prediction was
+  `ABD123`, it would score 0, as **not all characters** were correctly classified.
+
+* **cat_acc**: Calculate the accuracy of **individual characters** within the license plates that were
+  **correctly classified**. For example, if the correct label is `ABC123` and the prediction is `ABC133`, it would yield
+  a precision of 83.3% (5 out of 6 characters correctly classified), rather than 0% as in plate_acc, because it's not
+  completely classified correctly.
+
+* **top_3_k**: Calculate how frequently the true character is included in the **top-3 predictions**
+  (the three predictions with the highest probability).
 
 ### Contributing
 
 Contributions to the repo are greatly appreciated. Whether it's bug fixes, feature enhancements, or new models,
 your contributions are warmly welcomed.
 
 To start contributing or to begin development, you can follow these steps:
```

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/cli.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/onnx_converter.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/onnx_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,19 +70,19 @@
         model,
         input_signature=spec,
         opset=opset,
         output_path=output_path,
     )
     output_names = [n.name for n in model_proto.graph.output]
     x = np.random.randint(0, 256, size=(1, config.img_height, config.img_width, 1), dtype=np.uint8)
-    providers = ["CPUExecutionProvider"]
     # Run dummy inference and log time taken
-    m = rt.InferenceSession(output_path, providers=providers)
+    m = rt.InferenceSession(output_path)
     with log_time_taken("ONNX inference took:"):
         onnx_pred = m.run(output_names, {"input": x})
-    # Check ONNX and keras have the same results
-    np.testing.assert_allclose(model.predict(x, verbose=0), onnx_pred[0], rtol=1e-5)
-    logging.info("Model converted successfully to ONNX! Saved at %s", output_path)
+    # Check if ONNX and keras have the same results
+    if not np.allclose(model.predict(x, verbose=0), onnx_pred[0], rtol=1e-5, atol=1e-5):
+        logging.warning("ONNX model output was not close to Keras model for the given tolerance!")
+    logging.info("Model converted to ONNX! Saved at %s", output_path)
 
 
 if __name__ == "__main__":
     export_onnx()
```

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/train.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,21 @@
     "--batch-size",
     default=128,
     show_default=True,
     type=int,
     help="Batch size for training.",
 )
 @click.option(
+    "--num-workers",
+    default=0,
+    show_default=True,
+    type=int,
+    help="How many subprocesses to load data, used in the torch DataLoader.",
+)
+@click.option(
     "--output-dir",
     default="./trained-models",
     type=click.Path(dir_okay=True, path_type=pathlib.Path),
     help="Output directory where model will be saved.",
 )
 @click.option(
     "--epochs",
@@ -116,14 +123,15 @@
     dense: bool,
     config_file: pathlib.Path,
     annotations: pathlib.Path,
     val_annotations: pathlib.Path,
     augmentation_path: pathlib.Path | None,
     lr: float,
     batch_size: int,
+    num_workers: int,
     output_dir: pathlib.Path,
     epochs: int,
     tensorboard: bool,
     tensorboard_dir: str,
     early_stopping_patience: int,
     reduce_lr_patience: int,
 ) -> None:
@@ -135,22 +143,26 @@
     )
     config = load_config_from_yaml(config_file)
     train_torch_dataset = LicensePlateDataset(
         annotations_file=annotations,
         transform=train_augmentation,
         config=config,
     )
-    train_dataloader = DataLoader(train_torch_dataset, batch_size=batch_size, shuffle=True)
+    train_dataloader = DataLoader(
+        train_torch_dataset, batch_size=batch_size, num_workers=num_workers, shuffle=True
+    )
 
     if val_annotations:
         val_torch_dataset = LicensePlateDataset(
             annotations_file=val_annotations,
             config=config,
         )
-        val_dataloader = DataLoader(val_torch_dataset, batch_size=batch_size, shuffle=False)
+        val_dataloader = DataLoader(
+            val_torch_dataset, batch_size=batch_size, num_workers=num_workers, shuffle=False
+        )
     else:
         val_dataloader = None
 
     # Train
     model = cnn_ocr_model(
         h=config.img_height,
         w=config.img_width,
```

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/valid.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/valid.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_augmentation.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_predictions.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/cli/visualize_predictions.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/common/utils.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/common/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/config.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/hub.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/hub.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/onnx_inference.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/process.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/process.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/utils.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/inference/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/augmentation.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/dataset.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/data/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,52 +2,52 @@
 Dataset module.
 """
 
 import os
 from os import PathLike
 
 import albumentations as A
+import numpy.typing as npt
 import pandas as pd
 from torch.utils.data import Dataset
 
 from fast_plate_ocr.train.model.config import PlateOCRConfig
 from fast_plate_ocr.train.utilities import utils
 
 
 class LicensePlateDataset(Dataset):
     def __init__(
         self,
         annotations_file: str | PathLike[str],
         config: PlateOCRConfig,
         transform: A.Compose | None = None,
-    ):
-        self.annotations = pd.read_csv(annotations_file)
-        self.annotations["image_path"] = (
-            os.path.dirname(os.path.realpath(annotations_file))
-            + os.sep
-            + self.annotations["image_path"]
+    ) -> None:
+        annotations = pd.read_csv(annotations_file)
+        annotations["image_path"] = (
+            os.path.dirname(os.path.realpath(annotations_file)) + os.sep + annotations["image_path"]
         )
         assert (
-            self.annotations["plate_text"].str.len() <= config.max_plate_slots
+            annotations["plate_text"].str.len() <= config.max_plate_slots
         ).all(), "Plates are longer than max_plate_slots specified param. Change the parameter."
+        self.annotations = annotations.to_numpy()
         self.config = config
         self.transform = transform
 
-    def __len__(self):
-        return len(self.annotations.index)
+    def __len__(self) -> int:
+        return self.annotations.shape[0]
 
-    def __getitem__(self, idx):
-        annotation = self.annotations.iloc[idx]
+    def __getitem__(self, idx) -> tuple[npt.NDArray, npt.NDArray]:
+        image_path, plate_text = self.annotations[idx]
         x = utils.read_plate_image(
-            image_path=annotation.image_path,
+            image_path=image_path,
             img_height=self.config.img_height,
             img_width=self.config.img_width,
         )
         y = utils.target_transform(
-            plate_text=annotation.plate_text,
+            plate_text=plate_text,
             max_plate_slots=self.config.max_plate_slots,
             alphabet=self.config.alphabet,
             pad_char=self.config.pad_char,
         )
         if self.transform:
             x = self.transform(image=x)["image"]
         return x, y
```

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/config.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/custom.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/custom.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/layer_blocks.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/layer_blocks.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/models.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/model/models.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/backend_utils.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/backend_utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/utils.py` & `fast_plate_ocr-0.1.3/fast_plate_ocr/train/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.2/pyproject.toml` & `fast_plate_ocr-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-plate-ocr"
-version = "0.1.2"
+version = "0.1.3"
 description = "Fast & Lightweight OCR for vehicle license plates."
 authors = ["ankandrew <61120139+ankandrew@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/ankandrew/fast-plate-ocr/"
 documentation = "https://ankandrew.github.io/fast-plate-ocr"
 keywords = ["plate-recognition", "license-plate-recognition", "license-plate-ocr"]
 license = "MIT"
@@ -21,15 +21,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 # Packages required for doing inference
-numpy = ">=1.17"
+numpy = ">=1.20"
 onnxruntime = ">=1.4.0"
 opencv-python = "*"
 pyyaml = ">=5.1"
 tqdm = "*"
 rich = "*"
 
 # By default, we install onnx CPU runtime
```

### Comparing `fast_plate_ocr-0.1.2/PKG-INFO` & `fast_plate_ocr-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-plate-ocr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fast & Lightweight OCR for vehicle license plates.
 Home-page: https://github.com/ankandrew/fast-plate-ocr/
 License: MIT
 Keywords: plate-recognition,license-plate-recognition,license-plate-ocr
 Author: ankandrew
 Author-email: 61120139+ankandrew@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -30,15 +30,15 @@
 Requires-Dist: albumentations ; extra == "train"
 Requires-Dist: click ; extra == "train"
 Requires-Dist: keras (>=3.1.1) ; extra == "train"
 Requires-Dist: matplotlib ; extra == "train"
 Requires-Dist: mike ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: mkdocstrings[python] ; extra == "docs"
-Requires-Dist: numpy (>=1.17)
+Requires-Dist: numpy (>=1.20)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: onnxruntime-gpu (>=1.4.0) ; (sys_platform != "darwin") and (extra == "inference-gpu")
 Requires-Dist: opencv-python
 Requires-Dist: pandas ; extra == "train"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0) ; extra == "train"
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: rich
@@ -71,31 +71,31 @@
 **Lightweight** and **fast** OCR models for license plate text recognition. You can train models from scratch or use
 the trained models for inference.
 
 The idea is to use this after a plate object detector, since the OCR expects the cropped plates.
 
 ### Features
 
-- **Keras 3 Backend Support**: Compatible with **TensorFlow**, **JAX**, and **PyTorch** backends 🧠
-- **Augmentation Variety**: Diverse augmentations via **Albumentations** library 🖼️
+- **Keras 3 Backend Support**: Compatible with **[TensorFlow](https://www.tensorflow.org/)**, **[JAX](https://github.com/google/jax)**, and **[PyTorch](https://pytorch.org/)** backends 🧠
+- **Augmentation Variety**: Diverse **augmentations** via **[Albumentations](https://albumentations.ai/)** library 🖼️
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
-- **ONNX Runtime Inference**: **Fast** and **optimized** inference with ONNX runtime ⚡
+- **ONNX Runtime Inference**: **Fast** and **optimized** inference with **[ONNX runtime](https://onnxruntime.ai/)** ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
-- **Model HUB**: Access to a collection of pre-trained models ready for inference 🌟
+- **Model HUB**: Access to a collection of **pre-trained models** ready for inference 🌟
 
 ### Available Models
 
 |          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
 |:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
 | argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
 
 _<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
-_<sup>[2]</sup> Accuracy is what we refer as plate_acc. See metrics section._
+_<sup>[2]</sup> Accuracy is what we refer as plate_acc. See [metrics section](#model-metrics)._
 
 
 <details>
   <summary>Reproduce results.</summary>
 
 * Calculate Inference Time:
 
@@ -212,27 +212,28 @@
 2. A labeled dataset,
    see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)
    for the expected data format.
 3. Run train script:
     ```shell
     # You can set the backend to either TensorFlow, JAX or PyTorch
     # (just make sure it is installed)
-    !KERAS_BACKEND=tensorflow fast_plate_ocr train \
+    KERAS_BACKEND=tensorflow fast_plate_ocr train \
         --annotations path_to_the_train.csv \
         --val-annotations path_to_the_val.csv \
+        --config-file config.yaml \
         --batch-size 128 \
         --epochs 750 \
         --dense \
         --early-stopping-patience 100 \
         --reduce-lr-patience 50
     ```
 
-You will probably want to change the augmentation pipeline to apply to your dataset. In order to do this
+You will probably want to change the augmentation pipeline to apply to your dataset.
 
-Define Albumentations pipeline:
+In order to do this define an Albumentations pipeline:
 
 ```python
 import albumentations as A
 
 transform_pipeline = A.Compose(
     [
         # ...
@@ -339,22 +340,25 @@
 Each head will output a probability distribution over the `vocabulary` specified during training. So the output
 prediction for a single plate will be of shape `(max_plate_slots, vocabulary_size)`.
 
 ### Model Metrics
 
 During training, you will see the following metrics
 
-* **plate_acc**: Compute how many plates were correctly classified. For a single plate, if ground truth is `ABC123`, and
-  the prediction is 'ABC 123', then this would give a score of 1. If the prediction was ABD 123, it would
-  score 0.
-* **cat_acc**: Calculates how many characters of the plate were correctly classified. Example if the correct label is
-  `ABC123` and `ABC133` is predicted, it will not give a precision of 0% like plate_acc (not completely
-  classified correctly), but 83.3% (5/6).
-* **top_3_k**: Calculates how often the true character is found in the top-3 predictions (the 3 with the highest
-  probability).
+* **plate_acc**: Compute the number of **license plates** that were **fully classified**. For a single plate, if the
+  ground truth is `ABC123` and the prediction is also `ABC123`, it would score 1. However, if the prediction was
+  `ABD123`, it would score 0, as **not all characters** were correctly classified.
+
+* **cat_acc**: Calculate the accuracy of **individual characters** within the license plates that were
+  **correctly classified**. For example, if the correct label is `ABC123` and the prediction is `ABC133`, it would yield
+  a precision of 83.3% (5 out of 6 characters correctly classified), rather than 0% as in plate_acc, because it's not
+  completely classified correctly.
+
+* **top_3_k**: Calculate how frequently the true character is included in the **top-3 predictions**
+  (the three predictions with the highest probability).
 
 ### Contributing
 
 Contributions to the repo are greatly appreciated. Whether it's bug fixes, feature enhancements, or new models,
 your contributions are warmly welcomed.
 
 To start contributing or to begin development, you can follow these steps:
```

