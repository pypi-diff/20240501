# Comparing `tmp/classification_models_3D-1.0.8.tar.gz` & `tmp/classification_models_3D-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\classification_models_3D-1.0.8.tar", last modified: Sat Nov 11 07:55:23 2023, max compression
+gzip compressed data, was "dist\classification_models_3D-1.1.0.tar", last modified: Wed May  1 11:36:27 2024, max compression
```

## Comparing `classification_models_3D-1.0.8.tar` & `classification_models_3D-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-11-11 07:55:23.202459 classification_models_3D-1.0.8/
--rw-rw-rw-   0        0        0      584 2023-11-11 07:55:23.202459 classification_models_3D-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6569 2022-12-16 20:43:50.000000 classification_models_3D-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-11 07:55:23.169458 classification_models_3D-1.0.8/classification_models_3D/
--rw-rw-rw-   0        0        0      361 2020-07-17 14:42:34.000000 classification_models_3D-1.0.8/classification_models_3D/__init__.py
--rw-rw-rw-   0        0        0       63 2022-05-10 15:00:35.000000 classification_models_3D-1.0.8/classification_models_3D/__version__.py
--rw-rw-rw-   0        0        0      347 2020-02-26 08:57:00.000000 classification_models_3D-1.0.8/classification_models_3D/keras.py
-drwxrwxrwx   0        0        0        0 2023-11-11 07:55:23.196458 classification_models_3D-1.0.8/classification_models_3D/models/
--rw-rw-rw-   0        0        0    20064 2020-07-31 22:42:02.000000 classification_models_3D-1.0.8/classification_models_3D/models/_DepthwiseConv3D.py
--rw-rw-rw-   0        0        0        0 2020-02-26 08:57:00.000000 classification_models_3D-1.0.8/classification_models_3D/models/__init__.py
--rw-rw-rw-   0        0        0     4510 2020-07-17 13:17:25.000000 classification_models_3D-1.0.8/classification_models_3D/models/_common_blocks.py
--rw-rw-rw-   0        0        0    24756 2022-09-20 20:23:26.000000 classification_models_3D-1.0.8/classification_models_3D/models/convnext.py
--rw-rw-rw-   0        0        0    11695 2022-04-29 22:08:42.000000 classification_models_3D-1.0.8/classification_models_3D/models/densenet.py
--rw-rw-rw-   0        0        0    25826 2023-11-10 13:16:37.000000 classification_models_3D-1.0.8/classification_models_3D/models/efficientnet.py
--rw-rw-rw-   0        0        0    40461 2022-06-07 09:53:55.000000 classification_models_3D-1.0.8/classification_models_3D/models/efficientnet_v2.py
--rw-rw-rw-   0        0        0    14929 2022-05-10 14:49:56.000000 classification_models_3D-1.0.8/classification_models_3D/models/inception_resnet_v2.py
--rw-rw-rw-   0        0        0    14911 2022-05-10 14:51:33.000000 classification_models_3D-1.0.8/classification_models_3D/models/inception_v3.py
--rw-rw-rw-   0        0        0    18470 2022-04-29 16:59:23.000000 classification_models_3D-1.0.8/classification_models_3D/models/mobilenet.py
--rw-rw-rw-   0        0        0    21115 2022-05-10 09:40:27.000000 classification_models_3D-1.0.8/classification_models_3D/models/mobilenet_v2.py
--rw-rw-rw-   0        0        0    17443 2022-09-21 11:19:53.000000 classification_models_3D-1.0.8/classification_models_3D/models/resnet.py
--rw-rw-rw-   0        0        0    11940 2022-04-29 18:17:40.000000 classification_models_3D-1.0.8/classification_models_3D/models/resnext.py
--rw-rw-rw-   0        0        0    18790 2022-04-29 19:38:32.000000 classification_models_3D-1.0.8/classification_models_3D/models/senet.py
--rw-rw-rw-   0        0        0     6307 2022-04-29 18:45:28.000000 classification_models_3D-1.0.8/classification_models_3D/models/vgg16.py
--rw-rw-rw-   0        0        0     6308 2022-04-29 18:46:53.000000 classification_models_3D-1.0.8/classification_models_3D/models/vgg19.py
--rw-rw-rw-   0        0        0     4617 2022-08-29 11:20:45.000000 classification_models_3D-1.0.8/classification_models_3D/models_factory.py
--rw-rw-rw-   0        0        0      381 2020-02-26 08:57:00.000000 classification_models_3D-1.0.8/classification_models_3D/tfkeras.py
--rw-rw-rw-   0        0        0    27109 2022-08-29 12:52:19.000000 classification_models_3D-1.0.8/classification_models_3D/weights.py
-drwxrwxrwx   0        0        0        0 2023-11-11 07:55:23.172460 classification_models_3D-1.0.8/classification_models_3D.egg-info/
--rw-rw-rw-   0        0        0      584 2023-11-11 07:55:23.000000 classification_models_3D-1.0.8/classification_models_3D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1910 2023-11-11 07:55:23.000000 classification_models_3D-1.0.8/classification_models_3D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-11 07:55:23.000000 classification_models_3D-1.0.8/classification_models_3D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-11-11 07:55:23.000000 classification_models_3D-1.0.8/classification_models_3D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-11 07:55:23.202459 classification_models_3D-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-11-11 07:55:21.000000 classification_models_3D-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:36:27.175751 classification_models_3D-1.1.0/
+-rw-rw-rw-   0        0        0      658 2024-05-01 11:36:27.175751 classification_models_3D-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7435 2024-05-01 11:32:36.000000 classification_models_3D-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 11:36:27.159751 classification_models_3D-1.1.0/classification_models_3D/
+-rw-rw-rw-   0        0        0      300 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-11-29 15:26:53.000000 classification_models_3D-1.1.0/classification_models_3D/__version__.py
+-rw-rw-rw-   0        0        0      364 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/kkeras.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:36:27.171751 classification_models_3D-1.1.0/classification_models_3D/models/
+-rw-rw-rw-   0        0        0    18446 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/_DepthwiseConv3D.py
+-rw-rw-rw-   0        0        0        0 2020-02-26 08:57:00.000000 classification_models_3D-1.1.0/classification_models_3D/models/__init__.py
+-rw-rw-rw-   0        0        0     4661 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/_common_blocks.py
+-rw-rw-rw-   0        0        0    24700 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/convnext.py
+-rw-rw-rw-   0        0        0    11953 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/densenet.py
+-rw-rw-rw-   0        0        0    26629 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/efficientnet.py
+-rw-rw-rw-   0        0        0    41715 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/efficientnet_v2.py
+-rw-rw-rw-   0        0        0    15327 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    15315 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/inception_v3.py
+-rw-rw-rw-   0        0        0    18903 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/mobilenet.py
+-rw-rw-rw-   0        0        0    21614 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/mobilenet_v2.py
+-rw-rw-rw-   0        0        0    17443 2022-09-21 11:19:53.000000 classification_models_3D-1.1.0/classification_models_3D/models/resnet.py
+-rw-rw-rw-   0        0        0    11940 2022-04-29 18:17:40.000000 classification_models_3D-1.1.0/classification_models_3D/models/resnext.py
+-rw-rw-rw-   0        0        0    19439 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/senet.py
+-rw-rw-rw-   0        0        0     6481 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/vgg16.py
+-rw-rw-rw-   0        0        0     6482 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models/vgg19.py
+-rw-rw-rw-   0        0        0     4724 2024-05-01 11:23:08.000000 classification_models_3D-1.1.0/classification_models_3D/models_factory.py
+-rw-rw-rw-   0        0        0    27109 2022-08-29 12:52:19.000000 classification_models_3D-1.1.0/classification_models_3D/weights.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:36:27.161751 classification_models_3D-1.1.0/classification_models_3D.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-01 11:36:27.000000 classification_models_3D-1.1.0/classification_models_3D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1875 2024-05-01 11:36:27.000000 classification_models_3D-1.1.0/classification_models_3D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:36:27.000000 classification_models_3D-1.1.0/classification_models_3D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-01 11:36:27.000000 classification_models_3D-1.1.0/classification_models_3D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:36:27.176751 classification_models_3D-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      880 2024-05-01 11:34:33.000000 classification_models_3D-1.1.0/setup.py
```

### Comparing `classification_models_3D-1.0.8/PKG-INFO` & `classification_models_3D-1.1.0/classification_models_3D.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: classification_models_3D
-Version: 1.0.8
+Name: classification-models-3D
+Version: 1.1.0
 Summary: Set of models for classification of 3D volumes.
 Home-page: https://github.com/ZFTurbo/classification_models_3D
 Author: Roman Sol (ZFTurbo)
 Author-email: UNKNOWN
 License: UNKNOWN
-Description: 3D variants of popular CNN models for classification like ResNets, DenseNets, VGG, etc. It also contains weights obtained by converting ImageNet weights from the same 2D models. Models work with keras and tensorflow.keras.More details: https://github.com/ZFTurbo/classification_models_3D
+Description: This repository contains 3D variants of popular classification CNN models like ResNets, DenseNets, VGG, etc for keras module. It also contains weights obtained by converting ImageNet weights from the same 2D models. Models work with keras 3 with different backends like Tensorflow, Torch and Jax.More details: https://github.com/ZFTurbo/classification_models_3D
 Platform: UNKNOWN
```

### Comparing `classification_models_3D-1.0.8/README.md` & `classification_models_3D-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Classification models 3D Zoo - Keras and TF.Keras
 
-This repository contains 3D variants of popular CNN models for classification like ResNets, DenseNets, VGG, etc. It also contains weights 
+This repository contains 3D variants of popular classification CNN models like ResNets, DenseNets, VGG, etc for keras module. It also contains weights 
 obtained by converting ImageNet weights from the same 2D models. 
 
 This repository is based on great [classification_models](https://github.com/qubvel/classification_models) repo by [@qubvel](https://github.com/qubvel/)
 
 ### Architectures: 
 - [VGG](https://arxiv.org/abs/1409.1556) [16, 19]
 - [ResNet](https://arxiv.org/abs/1512.03385) [18, 34, 50, 101, 152]
@@ -27,26 +27,33 @@
 
 ### Examples 
 
 #### Loading model with `imagenet` weights:
 
 ```python
 
-from classification_models_3D.tfkeras import Classifiers
+from classification_models_3D.kkeras import Classifiers
 
 ResNet18, preprocess_input = Classifiers.get('resnet18')
 model = ResNet18(input_shape=(128, 128, 128, 3), weights='imagenet')
 ```
 
 #### Create model examples:
-- [tst_tfkeras.py](tst_tfkeras.py)
-- [tst_tfkeras_special_cases.py](tst_tfkeras_special_cases.py)
-
-#### Training example:
-- [training_example.py](training_example.py)
+Keras 3 support different backends like: Tensorflow, Torch and Jax. Below you can find examples for different backends:
+- Tensorflow: [tst_keras_tensorflow.py](tst_keras_tensorflow.py)
+- Tensorflow: [tst_special_cases_keras_tensorflow.py](tst_special_cases_keras_tensorflow.py)
+- Torch: [tst_keras_torch.py](tst_keras_torch.py)
+- Torch: [tst_special_cases_keras_torch.py](tst_special_cases_keras_torch.py)
+- Jax: [tst_keras_jax.py](tst_keras_jax.py)
+- Jax: [tst_special_cases_keras_jax.py](tst_special_cases_keras_jax.py)
+
+#### Training examples:
+- Tensorflow: [training_example_keras_tensorflow.py](training_example_keras_tensorflow.py)
+- Torch: [training_example_keras_torch.py](training_example_keras_torch.py)
+- Jax: [training_example_keras_jax.py](training_example_keras_jax.py)
 
 #### All possible nets for `Classifiers.get()` method: 
 `'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152', 'seresnet18', 'seresnet34', 'seresnet50',
         'seresnet101', 'seresnet152', 'seresnext50', 'seresnext101', 'senet154', 'resnext50', 'resnext101',
         'vgg16', 'vgg19', 'densenet121', 'densenet169', 'densenet201', 'mobilenet', 'mobilenetv2',
         'inceptionresnetv2', 'inceptionv3',  'efficientnetb0', 'efficientnetb1', 'efficientnetb2', 'efficientnetb3',
         'efficientnetb4', 'efficientnetb5', 'efficientnetb6', 'efficientnetb7', 'efficientnetv2-b0',
@@ -70,15 +77,15 @@
 ### Additional features
 
 #### Pooling
 Default pooling/stride size for 3D models is set equal to 2. You can change it for your needs using parameter 
  `stride_size`. Example:
  
  ```python
-from classification_models_3D.tfkeras import Classifiers
+from classification_models_3D.kkeras import Classifiers
 
 ResNet18, preprocess_input = Classifiers.get('resnet18')
 model = ResNet18(
     input_shape=(224, 224, 224, 3),
     stride_size=4,
     kernel_size=3, 
     weights=None
@@ -94,15 +101,15 @@
 
 #### More blocks
 
 * For some models like (resnet, resnext, senet, vgg16, vgg19, densenet) it's possible to change number of blocks/poolings. 
 For example if you want to make more poolings overall. You can do it like that:
 
  ```python
-from classification_models_3D.tfkeras import Classifiers
+from classification_models_3D.kkeras import Classifiers
 
 ResNet18, preprocess_input = Classifiers.get('resnet18')
 model = ResNet18(
     input_shape=(128, 128, 128, 3),
     include_top=False,
     weights=None,
     stride_size=(1, 1, 2, 2, 2, 2, 2, 2),
@@ -112,19 +119,26 @@
 ```
 
 - **Note 1**: Since number of filters grows 2 times, you can set initial number of filters with `init_filters` parameter.
 - **Note 2**: There is no `imagenet` weights for models which were modified this way. 
 
 ### Related repositories
 
- * [https://github.com/qubvel/classification_models](https://github.com/qubvel/classification_models) - original 2D repo
- * [volumentations](https://github.com/ZFTurbo/volumentations) - 3D augmentations
- * [segmentation models 3D](https://github.com/ZFTurbo/segmentation_models_3D) - models for segmentation in 3D
- * [driven_data_repo](https://github.com/ZFTurbo/DrivenData-Alzheimer-Research-1st-place-solution) - code for training and inference on real dataset
+* [https://github.com/qubvel/classification_models](https://github.com/qubvel/classification_models) - original 2D repo
+* [timm_3d](https://github.com/ZFTurbo/timm_3d) - models for classification in 3D for PyTorch
+* [segmentation models 3D](https://github.com/ZFTurbo/segmentation_models_3D) - models for segmentation in 3D for Keras/Tensorflow
+* [volumentations](https://github.com/ZFTurbo/volumentations) - 3D augmentations
+* [driven_data_repo](https://github.com/ZFTurbo/DrivenData-Alzheimer-Research-1st-place-solution) - code for training and inference on real dataset
  
+### Older versions
+
+Last version which supports Keras2 is 1.0.10
+
+`pip install classification-models-3D==1.0.10`
+
 ### Unresolved problems
 
 * There is no DepthwiseConv3D layer in keras, so repo used custom layer from [this repo](https://github.com/alexandrosstergiou/keras-DepthwiseConv3D) by [@alexandrosstergiou]( https://github.com/alexandrosstergiou/keras-DepthwiseConv3D) which can be slower than native implementation. 
 * There is no imagenet weights for 'inceptionresnetv2' and 'inceptionv3'.
  
 ### Description
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/_DepthwiseConv3D.py` & `classification_models_3D-1.1.0/classification_models_3D/models/_DepthwiseConv3D.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,179 +1,114 @@
 # Implementation: https://github.com/alexandrosstergiou/keras-DepthwiseConv3D
 
-import tensorflow as tf
-try:
-    from keras_applications import imagenet_utils
-    from keras import backend as K
-    from keras import initializers
-    from keras import regularizers
-    from keras import constraints
-    from keras import layers
-    from keras.engine import InputSpec
-    from keras.legacy.interfaces import conv3d_args_preprocessor, generate_legacy_interface
-    from keras.layers import Conv3D
-    from keras.backend.tensorflow_backend import _preprocess_padding, _preprocess_conv3d_input
-    from keras.utils import conv_utils
-except:
-    from tensorflow.keras import backend as K
-    from tensorflow.keras import initializers
-    from tensorflow.keras import regularizers
-    from tensorflow.keras import constraints
-    from tensorflow.keras import layers
-    from tensorflow.keras.layers import Conv3D
-    from tensorflow.keras.layers import InputSpec
-    # from tensorflow.keras.utils import conv_utils
-    import tensorflow.keras.utils as conv_utils
-    import six
-    import warnings
-    from distutils.version import StrictVersion
-
-
-    def generate_legacy_interface(allowed_positional_args=None,
-                                  conversions=None,
-                                  preprocessor=None,
-                                  value_conversions=None):
-        allowed_positional_args = allowed_positional_args or []
-        conversions = conversions or []
-        value_conversions = value_conversions or []
-
-        def legacy_support(func):
-            @six.wraps(func)
-            def wrapper(*args, **kwargs):
-                layer_name = args[0].__class__.__name__
-                if preprocessor:
-                    args, kwargs, converted = preprocessor(args, kwargs)
-                else:
-                    converted = []
-                if len(args) > len(allowed_positional_args) + 1:
-                    raise TypeError('Layer `' + layer_name +
-                                    '` can accept only ' +
-                                    str(len(allowed_positional_args)) +
-                                    ' positional arguments (' +
-                                    str(allowed_positional_args) + '), but '
-                                                                   'you passed the following '
-                                                                   'positional arguments: ' +
-                                    str(args[1:]))
-                for key in value_conversions:
-                    if key in kwargs:
-                        old_value = kwargs[key]
-                        if old_value in value_conversions[key]:
-                            kwargs[key] = value_conversions[key][old_value]
-                for old_name, new_name in conversions:
-                    if old_name in kwargs:
-                        value = kwargs.pop(old_name)
-                        kwargs[new_name] = value
-                        converted.append((new_name, old_name))
-                if converted:
-                    signature = '`' + layer_name + '('
-                    for value in args[1:]:
-                        if isinstance(value, six.string_types):
-                            signature += '"' + value + '"'
-                        else:
-                            signature += str(value)
+import keras.ops as kops
+from keras import backend as K
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import layers
+from keras import InputSpec
+from keras.src.legacy.backend import _preprocess_padding, _preprocess_conv3d_input
+
+
+def generate_legacy_interface(allowed_positional_args=None,
+                                conversions=None,
+                                preprocessor=None,
+                                value_conversions=None):
+    allowed_positional_args = allowed_positional_args or []
+    conversions = conversions or []
+    value_conversions = value_conversions or []
+
+    def legacy_support(func):
+        @six.wraps(func)
+        def wrapper(*args, **kwargs):
+            layer_name = args[0].__class__.__name__
+            if preprocessor:
+                args, kwargs, converted = preprocessor(args, kwargs)
+            else:
+                converted = []
+            if len(args) > len(allowed_positional_args) + 1:
+                raise TypeError('Layer `' + layer_name +
+                                '` can accept only ' +
+                                str(len(allowed_positional_args)) +
+                                ' positional arguments (' +
+                                str(allowed_positional_args) + '), but '
+                                                                'you passed the following '
+                                                                'positional arguments: ' +
+                                str(args[1:]))
+            for key in value_conversions:
+                if key in kwargs:
+                    old_value = kwargs[key]
+                    if old_value in value_conversions[key]:
+                        kwargs[key] = value_conversions[key][old_value]
+            for old_name, new_name in conversions:
+                if old_name in kwargs:
+                    value = kwargs.pop(old_name)
+                    kwargs[new_name] = value
+                    converted.append((new_name, old_name))
+            if converted:
+                signature = '`' + layer_name + '('
+                for value in args[1:]:
+                    if isinstance(value, six.string_types):
+                        signature += '"' + value + '"'
+                    else:
+                        signature += str(value)
+                    signature += ', '
+                for i, (name, value) in enumerate(kwargs.items()):
+                    signature += name + '='
+                    if isinstance(value, six.string_types):
+                        signature += '"' + value + '"'
+                    else:
+                        signature += str(value)
+                    if i < len(kwargs) - 1:
                         signature += ', '
-                    for i, (name, value) in enumerate(kwargs.items()):
-                        signature += name + '='
-                        if isinstance(value, six.string_types):
-                            signature += '"' + value + '"'
-                        else:
-                            signature += str(value)
-                        if i < len(kwargs) - 1:
-                            signature += ', '
-                    signature += ')`'
-                    warnings.warn('Update your `' + layer_name +
-                                  '` layer call to the Keras 2 API: ' + signature)
-                return func(*args, **kwargs)
-
-            return wrapper
-
-        return legacy_support
-
-
-    def conv3d_args_preprocessor(args, kwargs):
-        if len(args) > 5:
-            raise TypeError('Layer can receive at most 4 positional arguments.')
-        if len(args) == 5:
-            if isinstance(args[2], int) and isinstance(args[3], int) and isinstance(args[4], int):
-                kernel_size = (args[2], args[3], args[4])
-                args = [args[0], args[1], kernel_size]
-        elif len(args) == 4 and isinstance(args[3], int):
-            if isinstance(args[2], int) and isinstance(args[3], int):
-                new_keywords = ['padding', 'strides', 'data_format']
-                for kwd in new_keywords:
-                    if kwd in kwargs:
-                        raise ValueError(
-                            'It seems that you are using the Keras 2 '
-                            'and you are passing both `kernel_size` and `strides` '
-                            'as integer positional arguments. For safety reasons, '
-                            'this is disallowed. Pass `strides` '
-                            'as a keyword argument instead.')
-            if 'kernel_dim3' in kwargs:
-                kernel_size = (args[2], args[3], kwargs.pop('kernel_dim3'))
-                args = [args[0], args[1], kernel_size]
-        elif len(args) == 3:
-            if 'kernel_dim2' in kwargs and 'kernel_dim3' in kwargs:
-                kernel_size = (args[2],
-                               kwargs.pop('kernel_dim2'),
-                               kwargs.pop('kernel_dim3'))
-                args = [args[0], args[1], kernel_size]
-        elif len(args) == 2:
-            if 'kernel_dim1' in kwargs and 'kernel_dim2' in kwargs and 'kernel_dim3' in kwargs:
-                kernel_size = (kwargs.pop('kernel_dim1'),
-                               kwargs.pop('kernel_dim2'),
-                               kwargs.pop('kernel_dim3'))
-                args = [args[0], args[1], kernel_size]
-        return args, kwargs, [('kernel_size', 'kernel_dim*')]
-
-
-    def _preprocess_padding(padding):
-        """Convert keras' padding to tensorflow's padding.
-
-        # Arguments
-            padding: string, `"same"` or `"valid"`.
-
-        # Returns
-            a string, `"SAME"` or `"VALID"`.
-
-        # Raises
-            ValueError: if `padding` is invalid.
-        """
-        if padding == 'same':
-            padding = 'SAME'
-        elif padding == 'valid':
-            padding = 'VALID'
-        else:
-            raise ValueError('Invalid padding: ' + str(padding))
-        return padding
-
-
-    def dtype(x):
-        return x.dtype.base_dtype.name
-
-
-    def _has_nchw_support():
-        return True
-
-
-    def _preprocess_conv3d_input(x, data_format):
-        """Transpose and cast the input before the conv3d.
-
-        # Arguments
-            x: input tensor.
-            data_format: string, `"channels_last"` or `"channels_first"`.
-
-        # Returns
-            A tensor.
-        """
-        # tensorflow doesn't support float64 for conv layer before 1.8.0
-        if (dtype(x) == 'float64' and
-                StrictVersion(tf.__version__.split('-')[0]) < StrictVersion('1.8.0')):
-            x = tf.cast(x, 'float32')
-        tf_data_format = 'NDHWC'
-        return x, tf_data_format
+                signature += ')`'
+                warnings.warn('Update your `' + layer_name +
+                                '` layer call to the Keras 2 API: ' + signature)
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return legacy_support
+
+
+def conv3d_args_preprocessor(args, kwargs):
+    if len(args) > 5:
+        raise TypeError('Layer can receive at most 4 positional arguments.')
+    if len(args) == 5:
+        if isinstance(args[2], int) and isinstance(args[3], int) and isinstance(args[4], int):
+            kernel_size = (args[2], args[3], args[4])
+            args = [args[0], args[1], kernel_size]
+    elif len(args) == 4 and isinstance(args[3], int):
+        if isinstance(args[2], int) and isinstance(args[3], int):
+            new_keywords = ['padding', 'strides', 'data_format']
+            for kwd in new_keywords:
+                if kwd in kwargs:
+                    raise ValueError(
+                        'It seems that you are using the Keras 2 '
+                        'and you are passing both `kernel_size` and `strides` '
+                        'as integer positional arguments. For safety reasons, '
+                        'this is disallowed. Pass `strides` '
+                        'as a keyword argument instead.')
+        if 'kernel_dim3' in kwargs:
+            kernel_size = (args[2], args[3], kwargs.pop('kernel_dim3'))
+            args = [args[0], args[1], kernel_size]
+    elif len(args) == 3:
+        if 'kernel_dim2' in kwargs and 'kernel_dim3' in kwargs:
+            kernel_size = (args[2],
+                            kwargs.pop('kernel_dim2'),
+                            kwargs.pop('kernel_dim3'))
+            args = [args[0], args[1], kernel_size]
+    elif len(args) == 2:
+        if 'kernel_dim1' in kwargs and 'kernel_dim2' in kwargs and 'kernel_dim3' in kwargs:
+            kernel_size = (kwargs.pop('kernel_dim1'),
+                            kwargs.pop('kernel_dim2'),
+                            kwargs.pop('kernel_dim3'))
+            args = [args[0], args[1], kernel_size]
+    return args, kwargs, [('kernel_size', 'kernel_dim*')]
 
 
 def depthwise_conv3d_args_preprocessor(args, kwargs):
     converted = []
 
     if 'init' in kwargs:
         init = kwargs.pop('init')
@@ -305,16 +240,14 @@
         self.groups = groups
         self.depthwise_initializer = initializers.get(depthwise_initializer)
         self.depthwise_regularizer = regularizers.get(depthwise_regularizer)
         self.depthwise_constraint = constraints.get(depthwise_constraint)
         self.bias_initializer = initializers.get(bias_initializer)
         self.dilation_rate = dilation_rate
         self._padding = _preprocess_padding(self.padding)
-        self._strides = (1,) + self.strides + (1,)
-        self._data_format = "NDHWC"
         self.input_dim = None
 
     def build(self, input_shape):
         if len(input_shape) < 5:
             raise ValueError('Inputs to `DepthwiseConv3D` should have rank 5. '
                              'Received input shape:', str(input_shape))
         if self.data_format == 'channels_first':
@@ -338,15 +271,15 @@
 
         depthwise_kernel_shape = (self.kernel_size[0],
                                   self.kernel_size[1],
                                   self.kernel_size[2],
                                   self.input_dim,
                                   self.depth_multiplier)
 
-        self.depthwise_kernel = self.add_weight(
+        self._kernel = self.add_weight(
             shape=depthwise_kernel_shape,
             initializer=self.depthwise_initializer,
             name='depthwise_kernel',
             regularizer=self.depthwise_regularizer,
             constraint=self.depthwise_constraint)
 
         if self.use_bias:
@@ -360,67 +293,87 @@
         # Set input spec.
         self.input_spec = InputSpec(ndim=5, axes={channel_axis: self.input_dim})
         self.built = True
 
     def call(self, inputs, training=None):
         inputs = _preprocess_conv3d_input(inputs, self.data_format)
 
-        if self.data_format == 'channels_last':
-            dilation = (1,) + self.dilation_rate + (1,)
-        else:
-            dilation = self.dilation_rate + (1,) + (1,)
-
-        if self._data_format == 'NCDHW':
-            outputs = tf.concat(
-                [tf.nn.conv3d(inputs[0][:, i:i+self.input_dim//self.groups, :, :, :], self.depthwise_kernel[:, :, :, i:i+self.input_dim//self.groups, :],
-                    strides=self._strides,
+        if self.data_format == 'channel_first':
+            outputs = kops.concatenate(
+                [kops.conv(inputs[0][:, i:i+self.input_dim//self.groups, :, :, :], self._kernel[:, :, :, i:i+self.input_dim//self.groups, :],
+                    strides=self.strides,
                     padding=self._padding,
-                    dilations=dilation,
-                    data_format=self._data_format) for i in range(0, self.input_dim, self.input_dim//self.groups)], axis=1)
+                    dilation_rate=self.dilation_rate,
+                    data_format=self.data_format) for i in range(0, self.input_dim, self.input_dim//self.groups)], axis=1)
 
         else:
-            outputs = tf.concat(
-                [tf.nn.conv3d(inputs[0][:, :, :, :, i:i+self.input_dim//self.groups], self.depthwise_kernel[:, :, :, i:i+self.input_dim//self.groups, :],
-                    strides=self._strides,
+            outputs = kops.concatenate(
+                [kops.conv(inputs[0][:, :, :, :, i:i+self.input_dim//self.groups], self._kernel[:, :, :, i:i+self.input_dim//self.groups, :],
+                    strides=self.strides,
                     padding=self._padding,
-                    dilations=dilation,
-                    data_format=self._data_format) for i in range(0, self.input_dim, self.input_dim//self.groups)], axis=-1)
+                    dilation_rate=self.dilation_rate,
+                    data_format=self.data_format) for i in range(0, self.input_dim, self.input_dim//self.groups)], axis=-1)
 
         if self.bias is not None:
             outputs = K.bias_add(
                 outputs,
                 self.bias,
                 data_format=self.data_format)
 
         if self.activation is not None:
             return self.activation(outputs)
 
         return outputs
 
     def compute_output_shape(self, input_shape):
+        def conv_output_length(input_length, filter_size, padding, stride, dilation=1):
+            """Determines output length of a convolution given input length.
+
+            Args:
+                input_length: integer.
+                filter_size: integer.
+                padding: one of "same", "valid", "full", "causal"
+                stride: integer.
+                dilation: dilation rate, integer.
+
+            Returns:
+                The output length (integer).
+            """
+            if input_length is None:
+                return None
+            assert padding in {"same", "valid", "full", "causal"}
+            dilated_filter_size = filter_size + (filter_size - 1) * (dilation - 1)
+            if padding in ["same", "causal"]:
+                output_length = input_length
+            elif padding == "valid":
+                output_length = input_length - dilated_filter_size + 1
+            elif padding == "full":
+                output_length = input_length + dilated_filter_size - 1
+            return (output_length + stride - 1) // stride
+
         if self.data_format == 'channels_first':
             depth = input_shape[2]
             rows = input_shape[3]
             cols = input_shape[4]
             out_filters = self.groups * self.depth_multiplier
         elif self.data_format == 'channels_last':
             depth = input_shape[1]
             rows = input_shape[2]
             cols = input_shape[3]
             out_filters = self.groups * self.depth_multiplier
 
-        depth = conv_utils.conv_output_length(depth, self.kernel_size[0],
+        depth = conv_output_length(depth, self.kernel_size[0],
                                              self.padding,
                                              self.strides[0])
 
-        rows = conv_utils.conv_output_length(rows, self.kernel_size[1],
+        rows = conv_output_length(rows, self.kernel_size[1],
                                              self.padding,
                                              self.strides[1])
 
-        cols = conv_utils.conv_output_length(cols, self.kernel_size[2],
+        cols = conv_output_length(cols, self.kernel_size[2],
                                              self.padding,
                                              self.strides[2])
 
         if self.data_format == 'channels_first':
             return (input_shape[0], out_filters, depth, rows, cols)
 
         elif self.data_format == 'channels_last':
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/convnext.py` & `classification_models_3D-1.1.0/classification_models_3D/models/convnext.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 
 - [A ConvNet for the 2020s](https://arxiv.org/abs/2201.03545)
   (CVPR 2022)
 """
 
 import os
 import numpy as np
-import tensorflow.compat.v2 as tf
+import keras.ops as kops
+import keras.random as krandom
+from keras import Variable
+from keras.src.utils import file_utils
 
 from .. import get_submodules_from_kwargs
 from ..weights import load_model_weights
 from keras import backend
 from keras import layers
 from keras import utils
 from keras.applications import imagenet_utils
-from keras.engine import sequential
-from keras.engine import training as training_lib
+from keras import models
 
-# isort: off
-from tensorflow.python.util.tf_export import keras_export
 
 
 MODEL_CONFIGS = {
     "tiny": {
         "depths": [3, 3, 9, 3],
         "projection_dims": [96, 192, 384, 768],
         "default_size": 224,
@@ -156,17 +156,17 @@
     def __init__(self, drop_path_rate, **kwargs):
         super().__init__(**kwargs)
         self.drop_path_rate = drop_path_rate
 
     def call(self, x, training=None):
         if training:
             keep_prob = 1 - self.drop_path_rate
-            shape = (tf.shape(x)[0],) + (1,) * (len(tf.shape(x)) - 1)
-            random_tensor = keep_prob + tf.random.uniform(shape, 0, 1)
-            random_tensor = tf.floor(random_tensor)
+            shape = (kops.shape(x)[0],) + (1,) * (len(kops.shape(x)) - 1)
+            random_tensor = keep_prob + krandom.uniform(shape, 0, 1)
+            random_tensor = kops.floor(random_tensor)
             return (x / keep_prob) * random_tensor
         return x
 
     def get_config(self):
         config = super().get_config()
         config.update({"drop_path_rate": self.drop_path_rate})
         return config
@@ -189,16 +189,16 @@
 
     def __init__(self, init_values, projection_dim, **kwargs):
         super().__init__(**kwargs)
         self.init_values = init_values
         self.projection_dim = projection_dim
 
     def build(self, input_shape):
-        self.gamma = tf.Variable(
-            self.init_values * tf.ones((self.projection_dim,))
+        self.gamma = Variable(
+            self.init_values * kops.ones((self.projection_dim,))
         )
 
     def call(self, x):
         return x * self.gamma
 
     def get_config(self):
         config = super().get_config()
@@ -392,15 +392,15 @@
         ValueError: if `include_top` is True but `num_classes` is not 1000
           when using ImageNet.
     """
 
     global backend, layers, models, keras_utils
     backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
 
-    if not (weights in {"imagenet", None} or tf.io.gfile.exists(weights)):
+    if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
         )
 
@@ -449,15 +449,15 @@
             4 if backend.image_data_format() == "channels_last" else 1
         )
         num_channels = input_shape[channel_axis - 1]
         if num_channels == 3:
             x = PreStem(name=model_name)(x)
 
     # Stem block.
-    stem = sequential.Sequential(
+    stem = models.Sequential(
         [
             layers.Conv3D(
                 projection_dims[0],
                 kernel_size=4,
                 strides=stride_size[0],
                 name=model_name + "_stem_conv",
             ),
@@ -470,15 +470,15 @@
 
     # Downsampling blocks.
     downsample_layers = []
     downsample_layers.append(stem)
 
     num_downsample_layers = 3
     for i in range(num_downsample_layers):
-        downsample_layer = sequential.Sequential(
+        downsample_layer = models.Sequential(
             [
                 layers.LayerNormalization(
                     epsilon=1e-6,
                     name=model_name + "_downsampling_layernorm_" + str(i),
                 ),
                 layers.Conv3D(
                     projection_dims[i + 1],
@@ -520,15 +520,15 @@
     else:
         if pooling == "avg":
             x = layers.GlobalAveragePooling3D()(x)
         elif pooling == "max":
             x = layers.GlobalMaxPooling3D()(x)
         x = layers.LayerNormalization(epsilon=1e-6)(x)
 
-    model = training_lib.Model(inputs=inputs, outputs=x, name=model_name)
+    model = models.Model(inputs=inputs, outputs=x, name=model_name)
 
     # Load weights.
     if weights:
         if type(weights) == str and os.path.exists(weights):
             model.load_weights(weights)
         else:
             load_model_weights(model, model_name, weights, classes, include_top, **kwargs)
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/densenet.py` & `classification_models_3D-1.1.0/classification_models_3D/models/densenet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,351 +1,350 @@
-"""DenseNet models for Keras.
-
-# Reference paper
-
-- [Densely Connected Convolutional Networks]
-  (https://arxiv.org/abs/1608.06993) (CVPR 2017 Best Paper Award)
-
-# Reference implementation
-
-- [Torch DenseNets]
-  (https://github.com/liuzhuang13/DenseNet/blob/master/models/densenet.lua)
-- [TensorNets]
-  (https://github.com/taehoonlee/tensornets/blob/master/tensornets/densenets.py)
-"""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from .. import get_submodules_from_kwargs
-from keras_applications import imagenet_utils
-from keras_applications.imagenet_utils import decode_predictions
-from keras_applications.imagenet_utils import _obtain_input_shape
-from ..weights import load_model_weights
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-def dense_block(x, blocks, name):
-    """A dense block.
-
-    # Arguments
-        x: input tensor.
-        blocks: integer, the number of building blocks.
-        name: string, block label.
-
-    # Returns
-        output tensor for the block.
-    """
-    for i in range(blocks):
-        x = conv_block(x, 32, name=name + '_block' + str(i + 1))
-    return x
-
-
-def transition_block(x, reduction, name, stride_size):
-    """A transition block.
-
-    # Arguments
-        x: input tensor.
-        reduction: float, compression rate at transition layers.
-        name: string, block label.
-
-    # Returns
-        output tensor for the block.
-    """
-    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
-    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5,
-                                  name=name + '_bn')(x)
-    x = layers.Activation('relu', name=name + '_relu')(x)
-    x = layers.Conv3D(
-        int(backend.int_shape(x)[bn_axis] * reduction),
-        1,
-        use_bias=False,
-        name=name + '_conv'
-    )(x)
-    x = layers.AveragePooling3D(stride_size, strides=stride_size, name=name + '_pool')(x)
-    return x
-
-
-def conv_block(x, growth_rate, name):
-    """A building block for a dense block.
-
-    # Arguments
-        x: input tensor.
-        growth_rate: float, growth rate at dense layers.
-        name: string, block label.
-
-    # Returns
-        Output tensor for the block.
-    """
-    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
-    x1 = layers.BatchNormalization(axis=bn_axis,
-                                   epsilon=1.001e-5,
-                                   name=name + '_0_bn')(x)
-    x1 = layers.Activation('relu', name=name + '_0_relu')(x1)
-    x1 = layers.Conv3D(4 * growth_rate, 1,
-                       use_bias=False,
-                       name=name + '_1_conv')(x1)
-    x1 = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5,
-                                   name=name + '_1_bn')(x1)
-    x1 = layers.Activation('relu', name=name + '_1_relu')(x1)
-    x1 = layers.Conv3D(growth_rate, 3,
-                       padding='same',
-                       use_bias=False,
-                       name=name + '_2_conv')(x1)
-    x = layers.Concatenate(axis=bn_axis, name=name + '_concat')([x, x1])
-    return x
-
-
-def DenseNet(
-        blocks,
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        **kwargs
-):
-    """Instantiates the DenseNet architecture.
-
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    # Arguments
-        blocks: numbers of building blocks for the four dense layers.
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor
-            (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(224, 224, 3)` (with `'channels_last'` data format)
-            or `(3, 224, 224)` (with `'channels_first'` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 32.
-            E.g. `(200, 200, 3)` would be one valid value.
-        pooling: optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a 2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) < 3:
-        print('Error: stride_size length must be 3 or more')
-        return None
-
-    if len(stride_size) - 1 != len(blocks):
-        print('Error: stride_size length must be equal to repetitions length - 1')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    x = layers.ZeroPadding3D(padding=((3, 3), (3, 3), (3, 3)))(img_input)
-    x = layers.Conv3D(64, 7, strides=stride_size[0], use_bias=False, name='conv1/conv')(x)
-    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5, name='conv1/bn')(x)
-    x = layers.Activation('relu', name='conv1/relu')(x)
-    x = layers.ZeroPadding3D(padding=((1, 1), (1, 1), (1, 1)))(x)
-    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
-    x = layers.MaxPooling3D(pool, strides=stride_size[1], name='pool1')(x)
-
-    for i in range(2, len(blocks) + 1):
-        x = dense_block(x, blocks[i-2], name='conv{}'.format(i))
-        x = transition_block(x, 0.5, name='pool{}'.format(i), stride_size=stride_size[i])
-    x = dense_block(x, blocks[-1], name='conv{}'.format(len(blocks) + 1))
-
-    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5, name='bn')(x)
-    x = layers.Activation('relu', name='relu')(x)
-
-    if include_top:
-        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        x = layers.Dense(classes, activation='softmax', name='fc1000')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D(name='max_pool')(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model_name = ''
-    if blocks == (6, 12, 24, 16):
-        model_name = 'densenet121'
-        model = models.Model(inputs, x, name='densenet121')
-    elif blocks == (6, 12, 32, 32):
-        model_name = 'densenet169'
-        model = models.Model(inputs, x, name='densenet169')
-    elif blocks == (6, 12, 48, 32):
-        model_name = 'densenet201'
-        model = models.Model(inputs, x, name='densenet201')
-    else:
-        model_name = 'densenet'
-        model = models.Model(inputs, x, name='densenet')
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, model_name, weights, classes, include_top, **kwargs)
-
-    return model
-
-
-def DenseNet121(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        repetitions=(6, 12, 24, 16),
-        **kwargs
-):
-    return DenseNet(
-        repetitions,
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
-        stride_size=stride_size,
-        **kwargs
-    )
-
-
-def DenseNet169(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        repetitions=(6, 12, 32, 32),
-        **kwargs
-):
-    return DenseNet(
-        repetitions,
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
-        stride_size=stride_size,
-        **kwargs
-    )
-
-
-def DenseNet201(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        repetitions=(6, 12, 48, 32),
-        **kwargs
-):
-    return DenseNet(
-        repetitions,
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
-        stride_size=stride_size,
-        **kwargs
-    )
-
-
-def preprocess_input(x, data_format=None, **kwargs):
-    """Preprocesses a numpy array encoding a batch of images.
-
-    # Arguments
-        x: a 3D or 4D numpy array consists of RGB values within [0, 255].
-        data_format: data format of the image tensor.
-
-    # Returns
-        Preprocessed array.
-    """
-    return imagenet_utils.preprocess_input(x, data_format, mode='torch', **kwargs)
-
-
-setattr(DenseNet121, '__doc__', DenseNet.__doc__)
-setattr(DenseNet169, '__doc__', DenseNet.__doc__)
-setattr(DenseNet201, '__doc__', DenseNet.__doc__)
+"""DenseNet models for Keras.
+
+# Reference paper
+
+- [Densely Connected Convolutional Networks]
+  (https://arxiv.org/abs/1608.06993) (CVPR 2017 Best Paper Award)
+
+# Reference implementation
+
+- [Torch DenseNets]
+  (https://github.com/liuzhuang13/DenseNet/blob/master/models/densenet.lua)
+- [TensorNets]
+  (https://github.com/taehoonlee/tensornets/blob/master/tensornets/densenets.py)
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import os
+from .. import get_submodules_from_kwargs
+from keras.applications import imagenet_utils
+from keras.src.legacy.backend import int_shape
+from ..weights import load_model_weights
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+def dense_block(x, blocks, name):
+    """A dense block.
+
+    # Arguments
+        x: input tensor.
+        blocks: integer, the number of building blocks.
+        name: string, block label.
+
+    # Returns
+        output tensor for the block.
+    """
+    for i in range(blocks):
+        x = conv_block(x, 32, name=name + '_block' + str(i + 1))
+    return x
+
+
+def transition_block(x, reduction, name, stride_size):
+    """A transition block.
+
+    # Arguments
+        x: input tensor.
+        reduction: float, compression rate at transition layers.
+        name: string, block label.
+
+    # Returns
+        output tensor for the block.
+    """
+    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
+    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5,
+                                  name=name + '_bn')(x)
+    x = layers.Activation('relu', name=name + '_relu')(x)
+    x = layers.Conv3D(
+        int(int_shape(x)[bn_axis] * reduction),
+        1,
+        use_bias=False,
+        name=name + '_conv'
+    )(x)
+    x = layers.AveragePooling3D(stride_size, strides=stride_size, name=name + '_pool')(x)
+    return x
+
+
+def conv_block(x, growth_rate, name):
+    """A building block for a dense block.
+
+    # Arguments
+        x: input tensor.
+        growth_rate: float, growth rate at dense layers.
+        name: string, block label.
+
+    # Returns
+        Output tensor for the block.
+    """
+    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
+    x1 = layers.BatchNormalization(axis=bn_axis,
+                                   epsilon=1.001e-5,
+                                   name=name + '_0_bn')(x)
+    x1 = layers.Activation('relu', name=name + '_0_relu')(x1)
+    x1 = layers.Conv3D(4 * growth_rate, 1,
+                       use_bias=False,
+                       name=name + '_1_conv')(x1)
+    x1 = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5,
+                                   name=name + '_1_bn')(x1)
+    x1 = layers.Activation('relu', name=name + '_1_relu')(x1)
+    x1 = layers.Conv3D(growth_rate, 3,
+                       padding='same',
+                       use_bias=False,
+                       name=name + '_2_conv')(x1)
+    x = layers.Concatenate(axis=bn_axis, name=name + '_concat')([x, x1])
+    return x
+
+
+def DenseNet(
+        blocks,
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        **kwargs
+):
+    """Instantiates the DenseNet architecture.
+
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    # Arguments
+        blocks: numbers of building blocks for the four dense layers.
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+            (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(224, 224, 3)` (with `'channels_last'` data format)
+            or `(3, 224, 224)` (with `'channels_first'` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 32.
+            E.g. `(200, 200, 3)` would be one valid value.
+        pooling: optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a 2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) < 3:
+        print('Error: stride_size length must be 3 or more')
+        return None
+
+    if len(stride_size) - 1 != len(blocks):
+        print('Error: stride_size length must be equal to repetitions length - 1')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    x = layers.ZeroPadding3D(padding=((3, 3), (3, 3), (3, 3)))(img_input)
+    x = layers.Conv3D(64, 7, strides=stride_size[0], use_bias=False, name='conv1_conv')(x)
+    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5, name='conv1_bn')(x)
+    x = layers.Activation('relu', name='conv1_relu')(x)
+    x = layers.ZeroPadding3D(padding=((1, 1), (1, 1), (1, 1)))(x)
+    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
+    x = layers.MaxPooling3D(pool, strides=stride_size[1], name='pool1')(x)
+
+    for i in range(2, len(blocks) + 1):
+        x = dense_block(x, blocks[i-2], name='conv{}'.format(i))
+        x = transition_block(x, 0.5, name='pool{}'.format(i), stride_size=stride_size[i])
+    x = dense_block(x, blocks[-1], name='conv{}'.format(len(blocks) + 1))
+
+    x = layers.BatchNormalization(axis=bn_axis, epsilon=1.001e-5, name='bn')(x)
+    x = layers.Activation('relu', name='relu')(x)
+
+    if include_top:
+        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        x = layers.Dense(classes, activation='softmax', name='fc1000')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D(name='max_pool')(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model_name = ''
+    if blocks == (6, 12, 24, 16):
+        model_name = 'densenet121'
+        model = models.Model(inputs, x, name='densenet121')
+    elif blocks == (6, 12, 32, 32):
+        model_name = 'densenet169'
+        model = models.Model(inputs, x, name='densenet169')
+    elif blocks == (6, 12, 48, 32):
+        model_name = 'densenet201'
+        model = models.Model(inputs, x, name='densenet201')
+    else:
+        model_name = 'densenet'
+        model = models.Model(inputs, x, name='densenet')
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, model_name, weights, classes, include_top, **kwargs)
+
+    return model
+
+
+def DenseNet121(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        repetitions=(6, 12, 24, 16),
+        **kwargs
+):
+    return DenseNet(
+        repetitions,
+        include_top,
+        weights,
+        input_tensor,
+        input_shape,
+        pooling,
+        classes,
+        stride_size=stride_size,
+        **kwargs
+    )
+
+
+def DenseNet169(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        repetitions=(6, 12, 32, 32),
+        **kwargs
+):
+    return DenseNet(
+        repetitions,
+        include_top,
+        weights,
+        input_tensor,
+        input_shape,
+        pooling,
+        classes,
+        stride_size=stride_size,
+        **kwargs
+    )
+
+
+def DenseNet201(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        repetitions=(6, 12, 48, 32),
+        **kwargs
+):
+    return DenseNet(
+        repetitions,
+        include_top,
+        weights,
+        input_tensor,
+        input_shape,
+        pooling,
+        classes,
+        stride_size=stride_size,
+        **kwargs
+    )
+
+
+def preprocess_input(x, data_format=None, **kwargs):
+    """Preprocesses a numpy array encoding a batch of images.
+
+    # Arguments
+        x: a 3D or 4D numpy array consists of RGB values within [0, 255].
+        data_format: data format of the image tensor.
+
+    # Returns
+        Preprocessed array.
+    """
+    return imagenet_utils.preprocess_input(x, data_format, mode='torch', **kwargs)
+
+
+setattr(DenseNet121, '__doc__', DenseNet.__doc__)
+setattr(DenseNet169, '__doc__', DenseNet.__doc__)
+setattr(DenseNet201, '__doc__', DenseNet.__doc__)
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/efficientnet.py` & `classification_models_3D-1.1.0/classification_models_3D/models/efficientnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,817 +1,817 @@
-# Copyright 2019 The TensorFlow Authors. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-# pylint: disable=invalid-name
-# pylint: disable=missing-docstring
-"""EfficientNet models for Keras.
-
-Reference:
-  - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](
-      https://arxiv.org/abs/1905.11946) (ICML 2019)
-"""
-
-from .. import get_submodules_from_kwargs
-from ..weights import load_model_weights
-import tensorflow.compat.v2 as tf
-
-import os
-import copy
-import math
-
-from keras.applications import imagenet_utils
-from keras.engine import training
-from keras.layers import VersionAwareLayers
-from keras.utils import data_utils
-from keras.utils import layer_utils
-from ..models._DepthwiseConv3D import DepthwiseConv3D
-
-
-DEFAULT_BLOCKS_ARGS = [{
-    'kernel_size': 3,
-    'repeats': 1,
-    'filters_in': 32,
-    'filters_out': 16,
-    'expand_ratio': 1,
-    'id_skip': True,
-    'strides': 1,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 3,
-    'repeats': 2,
-    'filters_in': 16,
-    'filters_out': 24,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 2,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 5,
-    'repeats': 2,
-    'filters_in': 24,
-    'filters_out': 40,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 2,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 3,
-    'repeats': 3,
-    'filters_in': 40,
-    'filters_out': 80,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 2,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 5,
-    'repeats': 3,
-    'filters_in': 80,
-    'filters_out': 112,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 1,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 5,
-    'repeats': 4,
-    'filters_in': 112,
-    'filters_out': 192,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 2,
-    'se_ratio': 0.25
-}, {
-    'kernel_size': 3,
-    'repeats': 1,
-    'filters_in': 192,
-    'filters_out': 320,
-    'expand_ratio': 6,
-    'id_skip': True,
-    'strides': 1,
-    'se_ratio': 0.25
-}]
-
-CONV_KERNEL_INITIALIZER = {
-    'class_name': 'VarianceScaling',
-    'config': {
-        'scale': 2.0,
-        'mode': 'fan_out',
-        'distribution': 'truncated_normal'
-    }
-}
-
-DENSE_KERNEL_INITIALIZER = {
-    'class_name': 'VarianceScaling',
-    'config': {
-        'scale': 1. / 3.,
-        'mode': 'fan_out',
-        'distribution': 'uniform'
-    }
-}
-
-layers = VersionAwareLayers()
-
-BASE_DOCSTRING = """Instantiates the {name} architecture.
-
-  Reference:
-  - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](
-      https://arxiv.org/abs/1905.11946) (ICML 2019)
-
-  This function returns a Keras image classification model,
-  optionally loaded with weights pre-trained on ImageNet.
-
-  For image classification use cases, see
-  [this page for detailed examples](
-    https://keras.io/api/applications/#usage-examples-for-image-classification-models).
-
-  For transfer learning use cases, make sure to read the
-  [guide to transfer learning & fine-tuning](
-    https://keras.io/guides/transfer_learning/).
-
-  Note: each Keras Application expects a specific kind of input preprocessing.
-  For EfficientNet, input preprocessing is included as part of the model
-  (as a `Rescaling` layer), and thus
-  `tf.keras.applications.efficientnet.preprocess_input` is actually a
-  pass-through function. EfficientNet models expect their inputs to be float
-  tensors of pixels with values in the [0-255] range.
-
-  Args:
-    include_top: Whether to include the fully-connected
-        layer at the top of the network. Defaults to True.
-    weights: One of `None` (random initialization),
-          'imagenet' (pre-training on ImageNet),
-          or the path to the weights file to be loaded. Defaults to 'imagenet'.
-    input_tensor: Optional Keras tensor
-        (i.e. output of `layers.Input()`)
-        to use as image input for the model.
-    input_shape: Optional shape tuple, only to be specified
-        if `include_top` is False.
-        It should have exactly 3 inputs channels.
-    pooling: Optional pooling mode for feature extraction
-        when `include_top` is `False`. Defaults to None.
-        - `None` means that the output of the model will be
-            the 4D tensor output of the
-            last convolutional layer.
-        - `avg` means that global average pooling
-            will be applied to the output of the
-            last convolutional layer, and thus
-            the output of the model will be a 2D tensor.
-        - `max` means that global max pooling will
-            be applied.
-    classes: Optional number of classes to classify images
-        into, only to be specified if `include_top` is True, and
-        if no `weights` argument is specified. Defaults to 1000 (number of
-        ImageNet classes).
-    classifier_activation: A `str` or callable. The activation function to use
-        on the "top" layer. Ignored unless `include_top=True`. Set
-        `classifier_activation=None` to return the logits of the "top" layer.
-        Defaults to 'softmax'.
-        When loading pretrained weights, `classifier_activation` can only
-        be `None` or `"softmax"`.
-
-  Returns:
-    A `keras.Model` instance.
-"""
-
-def correct_pad_3d(inputs, kernel_size):
-    """Returns a tuple for zero-padding for 3D convolution with downsampling.
-
-      Args:
-        inputs: Input tensor.
-        kernel_size: An integer or tuple/list of 2 integers.
-
-      Returns:
-        A tuple.
-      """
-    img_dim = 2 if backend.image_data_format() == 'channels_first' else 1
-    input_size = backend.int_shape(inputs)[img_dim:(img_dim + 3)]
-    if isinstance(kernel_size, int):
-        kernel_size = (kernel_size, kernel_size, kernel_size)
-    if input_size[0] is None:
-        adjust = (1, 1, 1)
-    else:
-        adjust = (1 - input_size[0] % 2, 1 - input_size[1] % 2, 1 - input_size[2] % 2)
-    correct = (kernel_size[0] // 2, kernel_size[1] // 2, kernel_size[2] // 2)
-    return (
-        (correct[0] - adjust[0], correct[0]),
-        (correct[1] - adjust[1], correct[1]),
-        (correct[2] - adjust[2], correct[2]),
-    )
-
-
-def EfficientNet(
-        width_coefficient,
-        depth_coefficient,
-        default_size,
-        dropout_rate=0.2,
-        drop_connect_rate=0.2,
-        depth_divisor=8,
-        activation='swish',
-        blocks_args='default',
-        model_name='efficientnet',
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    """Instantiates the EfficientNet architecture using given scaling coefficients.
-
-      Args:
-        width_coefficient: float, scaling coefficient for network width.
-        depth_coefficient: float, scaling coefficient for network depth.
-        default_size: integer, default input image size.
-        dropout_rate: float, dropout rate before final classifier layer.
-        drop_connect_rate: float, dropout rate at skip connections.
-        depth_divisor: integer, a unit of network width.
-        activation: activation function.
-        blocks_args: list of dicts, parameters to construct block modules.
-        model_name: string, model name.
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor
-            (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False.
-            It should have exactly 3 inputs channels.
-        pooling: optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the
-                last convolutional layer.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional layer, and thus
-                the output of the model will be a 2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-        classifier_activation: A `str` or callable. The activation function to use
-            on the "top" layer. Ignored unless `include_top=True`. Set
-            `classifier_activation=None` to return the logits of the "top" layer.
-
-      Returns:
-        A `keras.Model` instance.
-
-      Raises:
-        ValueError: in case of invalid argument for `weights`,
-          or invalid input shape.
-        ValueError: if `classifier_activation` is not `softmax` or `None` when
-          using a pretrained top layer.
-      """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if blocks_args == 'default':
-        blocks_args = DEFAULT_BLOCKS_ARGS
-
-    if not (weights in {'imagenet', None} or tf.io.gfile.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) != 5:
-        print('Error: stride_size length must be exactly 5')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
-
-    def round_filters(filters, divisor=depth_divisor):
-        """Round number of filters based on depth multiplier."""
-        filters *= width_coefficient
-        new_filters = max(divisor, int(filters + divisor / 2) // divisor * divisor)
-        # Make sure that round down does not go down by more than 10%.
-        if new_filters < 0.9 * filters:
-            new_filters += divisor
-        return int(new_filters)
-
-    def round_repeats(repeats):
-        """Round number of repeats based on depth multiplier."""
-        return int(math.ceil(depth_coefficient * repeats))
-
-    # Build stem
-    x = img_input
-    x = layers.Rescaling(1. / 255.)(x)
-    x = layers.Normalization(axis=bn_axis)(x)
-
-    x = layers.ZeroPadding3D(
-        padding=correct_pad_3d(x, 3),
-        name='stem_conv_pad')(x)
-    x = layers.Conv3D(
-        round_filters(32),
-        3,
-        strides=stride_size[0],
-        padding='valid',
-        use_bias=False,
-        kernel_initializer=CONV_KERNEL_INITIALIZER,
-        name='stem_conv')(x)
-    x = layers.BatchNormalization(axis=bn_axis, name='stem_bn')(x)
-    x = layers.Activation(activation, name='stem_activation')(x)
-
-    # Build blocks
-    blocks_args = copy.deepcopy(blocks_args)
-
-    b = 0
-    blocks = float(sum(round_repeats(args['repeats']) for args in blocks_args))
-
-    strides_count = 1
-    for (i, args) in enumerate(blocks_args):
-        assert args['repeats'] > 0
-        # Update block input and output filters based on depth multiplier.
-        args['filters_in'] = round_filters(args['filters_in'])
-        args['filters_out'] = round_filters(args['filters_out'])
-
-        for j in range(round_repeats(args.pop('repeats'))):
-            # The first block needs to take care of stride and filter size increase.
-            if j > 0:
-                args['strides'] = 1
-                args['filters_in'] = args['filters_out']
-            elif args['strides'] > 1:
-                args['strides'] = stride_size[strides_count]
-                strides_count += 1
-            x = block(
-                x,
-                activation,
-                drop_connect_rate * b / blocks,
-                name='block{}{}_'.format(i + 1, chr(j + 97)),
-                **args)
-            b += 1
-
-    # Build top
-    x = layers.Conv3D(
-        round_filters(1280),
-        1,
-        padding='same',
-        use_bias=False,
-        kernel_initializer=CONV_KERNEL_INITIALIZER,
-        name='top_conv'
-    )(x)
-    x = layers.BatchNormalization(axis=bn_axis, name='top_bn')(x)
-    x = layers.Activation(activation, name='top_activation')(x)
-    if include_top:
-        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        if dropout_rate > 0:
-            x = layers.Dropout(dropout_rate, name='top_dropout')(x)
-        imagenet_utils.validate_activation(classifier_activation, weights)
-        x = layers.Dense(
-            classes,
-            activation=classifier_activation,
-            kernel_initializer=DENSE_KERNEL_INITIALIZER,
-            name='predictions'
-        )(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D(name='max_pool')(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = layer_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model = training.Model(inputs, x, name=model_name)
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, model_name, weights, classes, include_top, **kwargs)
-
-    return model
-
-
-def block(
-        inputs,
-        activation='swish',
-        drop_rate=0.,
-        name='',
-        filters_in=32,
-        filters_out=16,
-        kernel_size=3,
-        strides=1,
-        expand_ratio=1,
-        se_ratio=0.,
-        id_skip=True,
-):
-    """An inverted residual block.
-
-      Args:
-          inputs: input tensor.
-          activation: activation function.
-          drop_rate: float between 0 and 1, fraction of the input units to drop.
-          name: string, block label.
-          filters_in: integer, the number of input filters.
-          filters_out: integer, the number of output filters.
-          kernel_size: integer, the dimension of the convolution window.
-          strides: integer, the stride of the convolution.
-          expand_ratio: integer, scaling coefficient for the input filters.
-          se_ratio: float between 0 and 1, fraction to squeeze the input filters.
-          id_skip: boolean.
-
-      Returns:
-          output tensor for the block.
-      """
-    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
-
-    # Expansion phase
-    filters = filters_in * expand_ratio
-    if expand_ratio != 1:
-        x = layers.Conv3D(
-            filters,
-            1,
-            padding='same',
-            use_bias=False,
-            kernel_initializer=CONV_KERNEL_INITIALIZER,
-            name=name + 'expand_conv')(
-            inputs)
-        x = layers.BatchNormalization(axis=bn_axis, name=name + 'expand_bn')(x)
-        x = layers.Activation(activation, name=name + 'expand_activation')(x)
-    else:
-        x = inputs
-
-    # Depthwise Convolution
-    if strides == 2:
-        x = layers.ZeroPadding3D(
-            padding=correct_pad_3d(x, kernel_size),
-            name=name + 'dwconv_pad')(x)
-        conv_pad = 'valid'
-    else:
-        conv_pad = 'same'
-    x = DepthwiseConv3D(
-        kernel_size,
-        strides=strides,
-        padding=conv_pad,
-        use_bias=False,
-        depthwise_initializer=CONV_KERNEL_INITIALIZER,
-        name=name + 'dwconv'
-    )(x)
-    x = layers.BatchNormalization(axis=bn_axis, name=name + 'bn')(x)
-    x = layers.Activation(activation, name=name + 'activation')(x)
-
-    # Squeeze and Excitation phase
-    if 0 < se_ratio <= 1:
-        filters_se = max(1, int(filters_in * se_ratio))
-        se = layers.GlobalAveragePooling3D(name=name + 'se_squeeze')(x)
-        if bn_axis == 1:
-            se_shape = (filters, 1, 1, 1)
-        else:
-            se_shape = (1, 1, 1, filters)
-        se = layers.Reshape(se_shape, name=name + 'se_reshape')(se)
-        se = layers.Conv3D(
-            filters_se,
-            1,
-            padding='same',
-            activation=activation,
-            kernel_initializer=CONV_KERNEL_INITIALIZER,
-            name=name + 'se_reduce'
-        )(se)
-        se = layers.Conv3D(
-            filters,
-            1,
-            padding='same',
-            activation='sigmoid',
-            kernel_initializer=CONV_KERNEL_INITIALIZER,
-            name=name + 'se_expand')(se)
-        x = layers.multiply([x, se], name=name + 'se_excite')
-
-    # Output phase
-    x = layers.Conv3D(
-        filters_out,
-        1,
-        padding='same',
-        use_bias=False,
-        kernel_initializer=CONV_KERNEL_INITIALIZER,
-        name=name + 'project_conv'
-    )(x)
-    x = layers.BatchNormalization(axis=bn_axis, name=name + 'project_bn')(x)
-    if id_skip and strides == 1 and filters_in == filters_out:
-        if drop_rate > 0:
-            x = layers.Dropout(drop_rate, noise_shape=(None, 1, 1, 1, 1), name=name + 'drop')(x)
-        x = layers.add([x, inputs], name=name + 'add')
-    return x
-
-
-def EfficientNetB0(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.0,
-        1.0,
-        224,
-        0.2,
-        model_name='efficientnetb0',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB1(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.0,
-        1.1,
-        240,
-        0.2,
-        model_name='efficientnetb1',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB2(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.1,
-        1.2,
-        260,
-        0.3,
-        model_name='efficientnetb2',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB3(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.2,
-        1.4,
-        300,
-        0.3,
-        model_name='efficientnetb3',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB4(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.4,
-        1.8,
-        380,
-        0.4,
-        model_name='efficientnetb4',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB5(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.6,
-        2.2,
-        456,
-        0.4,
-        model_name='efficientnetb5',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB6(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        1.8,
-        2.6,
-        528,
-        0.5,
-        model_name='efficientnetb6',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-def EfficientNetB7(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        classifier_activation='softmax',
-        **kwargs
-):
-    return EfficientNet(
-        2.0,
-        3.1,
-        600,
-        0.5,
-        model_name='efficientnetb7',
-        include_top=include_top,
-        weights=weights,
-        input_tensor=input_tensor,
-        input_shape=input_shape,
-        pooling=pooling,
-        classes=classes,
-        stride_size=stride_size,
-        classifier_activation=classifier_activation,
-        **kwargs
-    )
-
-
-EfficientNetB0.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB0')
-EfficientNetB1.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB1')
-EfficientNetB2.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB2')
-EfficientNetB3.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB3')
-EfficientNetB4.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB4')
-EfficientNetB5.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB5')
-EfficientNetB6.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB6')
-EfficientNetB7.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB7')
-
-
-def preprocess_input(x, data_format=None, **kwargs):  # pylint: disable=unused-argument
-    """A placeholder method for backward compatibility.
-
-    The preprocessing logic has been included in the efficientnet model
-    implementation. Users are no longer required to call this method to normalize
-    the input data. This method does nothing and only kept as a placeholder to
-    align the API surface between old and new version of model.
-
-    Args:
-    x: A floating point `numpy.array` or a `tf.Tensor`.
-    data_format: Optional data format of the image tensor/array. Defaults to
-      None, in which case the global setting
-      `tf.keras.backend.image_data_format()` is used (unless you changed it,
-      it defaults to "channels_last").{mode}
-
-    Returns:
-    Unchanged `numpy.array` or `tf.Tensor`.
-    """
-    return x
-
-
-def decode_predictions(preds, top=5):
-    return imagenet_utils.decode_predictions(preds, top=top)
-
-
-decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
+# Copyright 2019 The TensorFlow Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+# pylint: disable=invalid-name
+# pylint: disable=missing-docstring
+"""EfficientNet models for Keras.
+
+Reference:
+  - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](
+      https://arxiv.org/abs/1905.11946) (ICML 2019)
+"""
+
+from .. import get_submodules_from_kwargs
+from ..weights import load_model_weights
+from keras.src.utils import file_utils
+
+import os
+import copy
+import math
+
+from keras.applications import imagenet_utils
+from keras import models
+from keras import layers as klayers
+from keras.src.ops import operation_utils
+from ..models._DepthwiseConv3D import DepthwiseConv3D
+from keras.src.legacy.backend import int_shape
+
+
+DEFAULT_BLOCKS_ARGS = [{
+    'kernel_size': 3,
+    'repeats': 1,
+    'filters_in': 32,
+    'filters_out': 16,
+    'expand_ratio': 1,
+    'id_skip': True,
+    'strides': 1,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 3,
+    'repeats': 2,
+    'filters_in': 16,
+    'filters_out': 24,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 2,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 5,
+    'repeats': 2,
+    'filters_in': 24,
+    'filters_out': 40,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 2,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 3,
+    'repeats': 3,
+    'filters_in': 40,
+    'filters_out': 80,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 2,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 5,
+    'repeats': 3,
+    'filters_in': 80,
+    'filters_out': 112,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 1,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 5,
+    'repeats': 4,
+    'filters_in': 112,
+    'filters_out': 192,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 2,
+    'se_ratio': 0.25
+}, {
+    'kernel_size': 3,
+    'repeats': 1,
+    'filters_in': 192,
+    'filters_out': 320,
+    'expand_ratio': 6,
+    'id_skip': True,
+    'strides': 1,
+    'se_ratio': 0.25
+}]
+
+CONV_KERNEL_INITIALIZER = {
+    'class_name': 'VarianceScaling',
+    'config': {
+        'scale': 2.0,
+        'mode': 'fan_out',
+        'distribution': 'truncated_normal'
+    }
+}
+
+DENSE_KERNEL_INITIALIZER = {
+    'class_name': 'VarianceScaling',
+    'config': {
+        'scale': 1. / 3.,
+        'mode': 'fan_out',
+        'distribution': 'uniform'
+    }
+}
+
+layers = klayers
+
+BASE_DOCSTRING = """Instantiates the {name} architecture.
+
+  Reference:
+  - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](
+      https://arxiv.org/abs/1905.11946) (ICML 2019)
+
+  This function returns a Keras image classification model,
+  optionally loaded with weights pre-trained on ImageNet.
+
+  For image classification use cases, see
+  [this page for detailed examples](
+    https://keras.io/api/applications/#usage-examples-for-image-classification-models).
+
+  For transfer learning use cases, make sure to read the
+  [guide to transfer learning & fine-tuning](
+    https://keras.io/guides/transfer_learning/).
+
+  Note: each Keras Application expects a specific kind of input preprocessing.
+  For EfficientNet, input preprocessing is included as part of the model
+  (as a `Rescaling` layer), and thus
+  `tf.keras.applications.efficientnet.preprocess_input` is actually a
+  pass-through function. EfficientNet models expect their inputs to be float
+  tensors of pixels with values in the [0-255] range.
+
+  Args:
+    include_top: Whether to include the fully-connected
+        layer at the top of the network. Defaults to True.
+    weights: One of `None` (random initialization),
+          'imagenet' (pre-training on ImageNet),
+          or the path to the weights file to be loaded. Defaults to 'imagenet'.
+    input_tensor: Optional Keras tensor
+        (i.e. output of `layers.Input()`)
+        to use as image input for the model.
+    input_shape: Optional shape tuple, only to be specified
+        if `include_top` is False.
+        It should have exactly 3 inputs channels.
+    pooling: Optional pooling mode for feature extraction
+        when `include_top` is `False`. Defaults to None.
+        - `None` means that the output of the model will be
+            the 4D tensor output of the
+            last convolutional layer.
+        - `avg` means that global average pooling
+            will be applied to the output of the
+            last convolutional layer, and thus
+            the output of the model will be a 2D tensor.
+        - `max` means that global max pooling will
+            be applied.
+    classes: Optional number of classes to classify images
+        into, only to be specified if `include_top` is True, and
+        if no `weights` argument is specified. Defaults to 1000 (number of
+        ImageNet classes).
+    classifier_activation: A `str` or callable. The activation function to use
+        on the "top" layer. Ignored unless `include_top=True`. Set
+        `classifier_activation=None` to return the logits of the "top" layer.
+        Defaults to 'softmax'.
+        When loading pretrained weights, `classifier_activation` can only
+        be `None` or `"softmax"`.
+
+  Returns:
+    A `keras.Model` instance.
+"""
+
+def correct_pad_3d(inputs, kernel_size):
+    """Returns a tuple for zero-padding for 3D convolution with downsampling.
+
+      Args:
+        inputs: Input tensor.
+        kernel_size: An integer or tuple/list of 2 integers.
+
+      Returns:
+        A tuple.
+      """
+    img_dim = 2 if backend.image_data_format() == 'channels_first' else 1
+    input_size = int_shape(inputs)[img_dim:(img_dim + 3)]
+    if isinstance(kernel_size, int):
+        kernel_size = (kernel_size, kernel_size, kernel_size)
+    if input_size[0] is None:
+        adjust = (1, 1, 1)
+    else:
+        adjust = (1 - input_size[0] % 2, 1 - input_size[1] % 2, 1 - input_size[2] % 2)
+    correct = (kernel_size[0] // 2, kernel_size[1] // 2, kernel_size[2] // 2)
+    return (
+        (correct[0] - adjust[0], correct[0]),
+        (correct[1] - adjust[1], correct[1]),
+        (correct[2] - adjust[2], correct[2]),
+    )
+
+
+def EfficientNet(
+        width_coefficient,
+        depth_coefficient,
+        default_size,
+        dropout_rate=0.2,
+        drop_connect_rate=0.2,
+        depth_divisor=8,
+        activation='swish',
+        blocks_args='default',
+        model_name='efficientnet',
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    """Instantiates the EfficientNet architecture using given scaling coefficients.
+
+      Args:
+        width_coefficient: float, scaling coefficient for network width.
+        depth_coefficient: float, scaling coefficient for network depth.
+        default_size: integer, default input image size.
+        dropout_rate: float, dropout rate before final classifier layer.
+        drop_connect_rate: float, dropout rate at skip connections.
+        depth_divisor: integer, a unit of network width.
+        activation: activation function.
+        blocks_args: list of dicts, parameters to construct block modules.
+        model_name: string, model name.
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+            (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False.
+            It should have exactly 3 inputs channels.
+        pooling: optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the
+                last convolutional layer.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional layer, and thus
+                the output of the model will be a 2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+        classifier_activation: A `str` or callable. The activation function to use
+            on the "top" layer. Ignored unless `include_top=True`. Set
+            `classifier_activation=None` to return the logits of the "top" layer.
+
+      Returns:
+        A `keras.Model` instance.
+
+      Raises:
+        ValueError: in case of invalid argument for `weights`,
+          or invalid input shape.
+        ValueError: if `classifier_activation` is not `softmax` or `None` when
+          using a pretrained top layer.
+      """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if blocks_args == 'default':
+        blocks_args = DEFAULT_BLOCKS_ARGS
+
+    if not (weights in {'imagenet', None} or file_utils.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) != 5:
+        print('Error: stride_size length must be exactly 5')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
+
+    def round_filters(filters, divisor=depth_divisor):
+        """Round number of filters based on depth multiplier."""
+        filters *= width_coefficient
+        new_filters = max(divisor, int(filters + divisor / 2) // divisor * divisor)
+        # Make sure that round down does not go down by more than 10%.
+        if new_filters < 0.9 * filters:
+            new_filters += divisor
+        return int(new_filters)
+
+    def round_repeats(repeats):
+        """Round number of repeats based on depth multiplier."""
+        return int(math.ceil(depth_coefficient * repeats))
+
+    # Build stem
+    x = img_input
+    x = layers.Rescaling(1. / 255.)(x)
+    x = layers.Normalization(axis=bn_axis)(x)
+
+    x = layers.ZeroPadding3D(
+        padding=correct_pad_3d(x, 3),
+        name='stem_conv_pad')(x)
+    x = layers.Conv3D(
+        round_filters(32),
+        3,
+        strides=stride_size[0],
+        padding='valid',
+        use_bias=False,
+        kernel_initializer=CONV_KERNEL_INITIALIZER,
+        name='stem_conv')(x)
+    x = layers.BatchNormalization(axis=bn_axis, name='stem_bn')(x)
+    x = layers.Activation(activation, name='stem_activation')(x)
+
+    # Build blocks
+    blocks_args = copy.deepcopy(blocks_args)
+
+    b = 0
+    blocks = float(sum(round_repeats(args['repeats']) for args in blocks_args))
+
+    strides_count = 1
+    for (i, args) in enumerate(blocks_args):
+        assert args['repeats'] > 0
+        # Update block input and output filters based on depth multiplier.
+        args['filters_in'] = round_filters(args['filters_in'])
+        args['filters_out'] = round_filters(args['filters_out'])
+
+        for j in range(round_repeats(args.pop('repeats'))):
+            # The first block needs to take care of stride and filter size increase.
+            if j > 0:
+                args['strides'] = 1
+                args['filters_in'] = args['filters_out']
+            elif args['strides'] > 1:
+                args['strides'] = stride_size[strides_count]
+                strides_count += 1
+            x = block(
+                x,
+                activation,
+                drop_connect_rate * b / blocks,
+                name='block{}{}_'.format(i + 1, chr(j + 97)),
+                **args)
+            b += 1
+
+    # Build top
+    x = layers.Conv3D(
+        round_filters(1280),
+        1,
+        padding='same',
+        use_bias=False,
+        kernel_initializer=CONV_KERNEL_INITIALIZER,
+        name='top_conv'
+    )(x)
+    x = layers.BatchNormalization(axis=bn_axis, name='top_bn')(x)
+    x = layers.Activation(activation, name='top_activation')(x)
+    if include_top:
+        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        if dropout_rate > 0:
+            x = layers.Dropout(dropout_rate, name='top_dropout')(x)
+        imagenet_utils.validate_activation(classifier_activation, weights)
+        x = layers.Dense(
+            classes,
+            activation=classifier_activation,
+            kernel_initializer=DENSE_KERNEL_INITIALIZER,
+            name='predictions'
+        )(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D(name='max_pool')(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = operation_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model = models.Model(inputs, x, name=model_name)
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, model_name, weights, classes, include_top, **kwargs)
+
+    return model
+
+
+def block(
+        inputs,
+        activation='swish',
+        drop_rate=0.,
+        name='',
+        filters_in=32,
+        filters_out=16,
+        kernel_size=3,
+        strides=1,
+        expand_ratio=1,
+        se_ratio=0.,
+        id_skip=True,
+):
+    """An inverted residual block.
+
+      Args:
+          inputs: input tensor.
+          activation: activation function.
+          drop_rate: float between 0 and 1, fraction of the input units to drop.
+          name: string, block label.
+          filters_in: integer, the number of input filters.
+          filters_out: integer, the number of output filters.
+          kernel_size: integer, the dimension of the convolution window.
+          strides: integer, the stride of the convolution.
+          expand_ratio: integer, scaling coefficient for the input filters.
+          se_ratio: float between 0 and 1, fraction to squeeze the input filters.
+          id_skip: boolean.
+
+      Returns:
+          output tensor for the block.
+      """
+    bn_axis = -1 if backend.image_data_format() == 'channels_last' else 1
+
+    # Expansion phase
+    filters = filters_in * expand_ratio
+    if expand_ratio != 1:
+        x = layers.Conv3D(
+            filters,
+            1,
+            padding='same',
+            use_bias=False,
+            kernel_initializer=CONV_KERNEL_INITIALIZER,
+            name=name + 'expand_conv')(
+            inputs)
+        x = layers.BatchNormalization(axis=bn_axis, name=name + 'expand_bn')(x)
+        x = layers.Activation(activation, name=name + 'expand_activation')(x)
+    else:
+        x = inputs
+
+    # Depthwise Convolution
+    if strides == 2:
+        x = layers.ZeroPadding3D(
+            padding=correct_pad_3d(x, kernel_size),
+            name=name + 'dwconv_pad')(x)
+        conv_pad = 'valid'
+    else:
+        conv_pad = 'same'
+    x = DepthwiseConv3D(
+        kernel_size,
+        strides=strides,
+        padding=conv_pad,
+        use_bias=False,
+        depthwise_initializer=CONV_KERNEL_INITIALIZER,
+        name=name + 'dwconv'
+    )(x)
+    x = layers.BatchNormalization(axis=bn_axis, name=name + 'bn')(x)
+    x = layers.Activation(activation, name=name + 'activation')(x)
+
+    # Squeeze and Excitation phase
+    if 0 < se_ratio <= 1:
+        filters_se = max(1, int(filters_in * se_ratio))
+        se = layers.GlobalAveragePooling3D(name=name + 'se_squeeze')(x)
+        if bn_axis == 1:
+            se_shape = (filters, 1, 1, 1)
+        else:
+            se_shape = (1, 1, 1, filters)
+        se = layers.Reshape(se_shape, name=name + 'se_reshape')(se)
+        se = layers.Conv3D(
+            filters_se,
+            1,
+            padding='same',
+            activation=activation,
+            kernel_initializer=CONV_KERNEL_INITIALIZER,
+            name=name + 'se_reduce'
+        )(se)
+        se = layers.Conv3D(
+            filters,
+            1,
+            padding='same',
+            activation='sigmoid',
+            kernel_initializer=CONV_KERNEL_INITIALIZER,
+            name=name + 'se_expand')(se)
+        x = layers.multiply([x, se], name=name + 'se_excite')
+
+    # Output phase
+    x = layers.Conv3D(
+        filters_out,
+        1,
+        padding='same',
+        use_bias=False,
+        kernel_initializer=CONV_KERNEL_INITIALIZER,
+        name=name + 'project_conv'
+    )(x)
+    x = layers.BatchNormalization(axis=bn_axis, name=name + 'project_bn')(x)
+    if id_skip and strides == 1 and filters_in == filters_out:
+        if drop_rate > 0:
+            x = layers.Dropout(drop_rate, noise_shape=(None, 1, 1, 1, 1), name=name + 'drop')(x)
+        x = layers.add([x, inputs], name=name + 'add')
+    return x
+
+
+def EfficientNetB0(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.0,
+        1.0,
+        224,
+        0.2,
+        model_name='efficientnetb0',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB1(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.0,
+        1.1,
+        240,
+        0.2,
+        model_name='efficientnetb1',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB2(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.1,
+        1.2,
+        260,
+        0.3,
+        model_name='efficientnetb2',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB3(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.2,
+        1.4,
+        300,
+        0.3,
+        model_name='efficientnetb3',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB4(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.4,
+        1.8,
+        380,
+        0.4,
+        model_name='efficientnetb4',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB5(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.6,
+        2.2,
+        456,
+        0.4,
+        model_name='efficientnetb5',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB6(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        1.8,
+        2.6,
+        528,
+        0.5,
+        model_name='efficientnetb6',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+def EfficientNetB7(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        classifier_activation='softmax',
+        **kwargs
+):
+    return EfficientNet(
+        2.0,
+        3.1,
+        600,
+        0.5,
+        model_name='efficientnetb7',
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
+        stride_size=stride_size,
+        classifier_activation=classifier_activation,
+        **kwargs
+    )
+
+
+EfficientNetB0.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB0')
+EfficientNetB1.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB1')
+EfficientNetB2.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB2')
+EfficientNetB3.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB3')
+EfficientNetB4.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB4')
+EfficientNetB5.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB5')
+EfficientNetB6.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB6')
+EfficientNetB7.__doc__ = BASE_DOCSTRING.format(name='EfficientNetB7')
+
+
+def preprocess_input(x, data_format=None, **kwargs):  # pylint: disable=unused-argument
+    """A placeholder method for backward compatibility.
+
+    The preprocessing logic has been included in the efficientnet model
+    implementation. Users are no longer required to call this method to normalize
+    the input data. This method does nothing and only kept as a placeholder to
+    align the API surface between old and new version of model.
+
+    Args:
+    x: A floating point `numpy.array` or a `tf.Tensor`.
+    data_format: Optional data format of the image tensor/array. Defaults to
+      None, in which case the global setting
+      `tf.keras.backend.image_data_format()` is used (unless you changed it,
+      it defaults to "channels_last").{mode}
+
+    Returns:
+    Unchanged `numpy.array` or `tf.Tensor`.
+    """
+    return x
+
+
+def decode_predictions(preds, top=5):
+    return imagenet_utils.decode_predictions(preds, top=top)
+
+
+decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/inception_resnet_v2.py` & `classification_models_3D-1.1.0/classification_models_3D/models/inception_resnet_v2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,366 +1,367 @@
-"""Inception-ResNet V2 model for Keras.
-
-Model naming and structure follows TF-slim implementation
-(which has some additional layers and different number of
-filters from the original arXiv paper):
-https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_resnet_v2.py
-
-Pre-trained ImageNet weights are also converted from TF-slim,
-which can be found in:
-https://github.com/tensorflow/models/tree/master/research/slim#pre-trained-models
-
-# Reference
-- [Inception-v4, Inception-ResNet and the Impact of
-   Residual Connections on Learning](https://arxiv.org/abs/1602.07261) (AAAI 2017)
-
-"""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from .. import get_submodules_from_kwargs
-from keras_applications import imagenet_utils
-
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-def preprocess_input(x, **kwargs):
-    """Preprocesses a numpy array encoding a batch of images.
-
-    # Arguments
-        x: a 4D numpy array consists of RGB values within [0, 255].
-
-    # Returns
-        Preprocessed array.
-    """
-    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
-
-
-def conv3d_bn(x,
-              filters,
-              kernel_size,
-              strides=1,
-              padding='same',
-              activation='relu',
-              use_bias=False,
-              name=None):
-    """Utility function to apply conv + BN.
-
-    # Arguments
-        x: input tensor.
-        filters: filters in `Conv2D`.
-        kernel_size: kernel size as in `Conv2D`.
-        strides: strides in `Conv2D`.
-        padding: padding mode in `Conv2D`.
-        activation: activation in `Conv2D`.
-        use_bias: whether to use a bias in `Conv2D`.
-        name: name of the ops; will become `name + '_ac'` for the activation
-            and `name + '_bn'` for the batch norm layer.
-
-    # Returns
-        Output tensor after applying `Conv2D` and `BatchNormalization`.
-    """
-    x = layers.Conv3D(filters,
-                      kernel_size,
-                      strides=strides,
-                      padding=padding,
-                      use_bias=use_bias,
-                      name=name)(x)
-    if not use_bias:
-        bn_axis = 1 if backend.image_data_format() == 'channels_first' else 4
-        bn_name = None if name is None else name + '_bn'
-        x = layers.BatchNormalization(axis=bn_axis,
-                                      scale=False,
-                                      name=bn_name)(x)
-    if activation is not None:
-        ac_name = None if name is None else name + '_ac'
-        x = layers.Activation(activation, name=ac_name)(x)
-    return x
-
-
-def inception_resnet_block(x, scale, block_type, block_idx, activation='relu'):
-    """Adds a Inception-ResNet block.
-
-    This function builds 3 types of Inception-ResNet blocks mentioned
-    in the paper, controlled by the `block_type` argument (which is the
-    block name used in the official TF-slim implementation):
-        - Inception-ResNet-A: `block_type='block35'`
-        - Inception-ResNet-B: `block_type='block17'`
-        - Inception-ResNet-C: `block_type='block8'`
-
-    # Arguments
-        x: input tensor.
-        scale: scaling factor to scale the residuals (i.e., the output of
-            passing `x` through an inception module) before adding them
-            to the shortcut branch.
-            Let `r` be the output from the residual branch,
-            the output of this block will be `x + scale * r`.
-        block_type: `'block35'`, `'block17'` or `'block8'`, determines
-            the network structure in the residual branch.
-        block_idx: an `int` used for generating layer names.
-            The Inception-ResNet blocks
-            are repeated many times in this network.
-            We use `block_idx` to identify
-            each of the repetitions. For example,
-            the first Inception-ResNet-A block
-            will have `block_type='block35', block_idx=0`,
-            and the layer names will have
-            a common prefix `'block35_0'`.
-        activation: activation function to use at the end of the block
-            (see [activations](../activations.md)).
-            When `activation=None`, no activation is applied
-            (i.e., "linear" activation: `a(x) = x`).
-
-    # Returns
-        Output tensor for the block.
-
-    # Raises
-        ValueError: if `block_type` is not one of `'block35'`,
-            `'block17'` or `'block8'`.
-    """
-    if block_type == 'block35':
-        branch_0 = conv3d_bn(x, 32, 1)
-        branch_1 = conv3d_bn(x, 32, 1)
-        branch_1 = conv3d_bn(branch_1, 32, 3)
-        branch_2 = conv3d_bn(x, 32, 1)
-        branch_2 = conv3d_bn(branch_2, 48, 3)
-        branch_2 = conv3d_bn(branch_2, 64, 3)
-        branches = [branch_0, branch_1, branch_2]
-    elif block_type == 'block17':
-        branch_0 = conv3d_bn(x, 192, 1)
-        branch_1 = conv3d_bn(x, 128, 1)
-        branch_1 = conv3d_bn(branch_1, 160, [1, 7, 1])
-        branch_1 = conv3d_bn(branch_1, 192, [7, 1, 1])
-        branches = [branch_0, branch_1]
-    elif block_type == 'block8':
-        branch_0 = conv3d_bn(x, 192, 1)
-        branch_1 = conv3d_bn(x, 192, 1)
-        branch_1 = conv3d_bn(branch_1, 224, [1, 3, 1])
-        branch_1 = conv3d_bn(branch_1, 256, [3, 1, 1])
-        branches = [branch_0, branch_1]
-    else:
-        raise ValueError('Unknown Inception-ResNet block type. '
-                         'Expects "block35", "block17" or "block8", '
-                         'but got: ' + str(block_type))
-
-    block_name = block_type + '_' + str(block_idx)
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else 4
-    mixed = layers.Concatenate(
-        axis=channel_axis, name=block_name + '_mixed')(branches)
-    up = conv3d_bn(mixed,
-                   backend.int_shape(x)[channel_axis],
-                   1,
-                   activation=None,
-                   use_bias=True,
-                   name=block_name + '_conv')
-
-    x = layers.Lambda(lambda inputs, scale: inputs[0] + inputs[1] * scale,
-                      output_shape=backend.int_shape(x)[1:],
-                      arguments={'scale': scale},
-                      name=block_name)([x, up])
-    if activation is not None:
-        x = layers.Activation(activation, name=block_name + '_ac')(x)
-    return x
-
-
-def InceptionResNetV2(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        **kwargs
-):
-    """Instantiates the Inception-ResNet v2 architecture.
-
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    # Arguments
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is `False` (otherwise the input shape
-            has to be `(299, 299, 3)` (with `'channels_last'` data format)
-            or `(3, 299, 299)` (with `'channels_first'` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 75.
-            E.g. `(150, 150, 3)` would be one valid value.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the last convolutional block.
-            - `'avg'` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a 2D tensor.
-            - `'max'` means that global max pooling will be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is `True`, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras `Model` instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) != 5:
-        print('Error: stride_size length must be exactly 5')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    # Stem block: 35 x 35 x 192
-    x = conv3d_bn(img_input, 32, 3, strides=stride_size[0], padding='same')
-    x = conv3d_bn(x, 32, 3, padding='same')
-    x = conv3d_bn(x, 64, 3)
-    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
-    x = layers.MaxPooling3D(pool, strides=stride_size[1], padding='same')(x)
-    x = conv3d_bn(x, 80, 1, padding='same')
-    x = conv3d_bn(x, 192, 3, padding='same')
-    pool = (stride_size[2][0] + 1, stride_size[2][1] + 1, stride_size[2][2] + 1)
-    x = layers.MaxPooling3D(pool, strides=stride_size[2], padding='same')(x)
-
-    # Mixed 5b (Inception-A block): 35 x 35 x 320
-    branch_0 = conv3d_bn(x, 96, 1)
-    branch_1 = conv3d_bn(x, 48, 1)
-    branch_1 = conv3d_bn(branch_1, 64, 5)
-    branch_2 = conv3d_bn(x, 64, 1)
-    branch_2 = conv3d_bn(branch_2, 96, 3)
-    branch_2 = conv3d_bn(branch_2, 96, 3)
-    branch_pool = layers.AveragePooling3D(3, strides=1, padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 64, 1)
-    branches = [branch_0, branch_1, branch_2, branch_pool]
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else 4
-    x = layers.Concatenate(axis=channel_axis, name='mixed_5b')(branches)
-
-    # 10x block35 (Inception-ResNet-A block): 35 x 35 x 320
-    for block_idx in range(1, 11):
-        x = inception_resnet_block(x,
-                                   scale=0.17,
-                                   block_type='block35',
-                                   block_idx=block_idx)
-
-    # Mixed 6a (Reduction-A block): 17 x 17 x 1088
-    branch_0 = conv3d_bn(x, 384, 3, strides=stride_size[3], padding='same')
-    branch_1 = conv3d_bn(x, 256, 1)
-    branch_1 = conv3d_bn(branch_1, 256, 3)
-    branch_1 = conv3d_bn(branch_1, 384, 3, strides=stride_size[3], padding='same')
-    pool = (stride_size[3][0] + 1, stride_size[3][1] + 1, stride_size[3][2] + 1)
-    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[3], padding='same')(x)
-    branches = [branch_0, branch_1, branch_pool]
-    x = layers.Concatenate(axis=channel_axis, name='mixed_6a')(branches)
-
-    # 20x block17 (Inception-ResNet-B block): 17 x 17 x 1088
-    for block_idx in range(1, 21):
-        x = inception_resnet_block(x,
-                                   scale=0.1,
-                                   block_type='block17',
-                                   block_idx=block_idx)
-
-    # Mixed 7a (Reduction-B block): 8 x 8 x 2080
-    branch_0 = conv3d_bn(x, 256, 1)
-    branch_0 = conv3d_bn(branch_0, 384, 3, strides=stride_size[4], padding='same')
-    branch_1 = conv3d_bn(x, 256, 1)
-    branch_1 = conv3d_bn(branch_1, 288, 3, strides=stride_size[4], padding='same')
-    branch_2 = conv3d_bn(x, 256, 1)
-    branch_2 = conv3d_bn(branch_2, 288, 3)
-    branch_2 = conv3d_bn(branch_2, 320, 3, strides=stride_size[4], padding='same')
-    pool = (stride_size[4][0] + 1, stride_size[4][1] + 1, stride_size[4][2] + 1)
-    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[4], padding='same')(x)
-    branches = [branch_0, branch_1, branch_2, branch_pool]
-    x = layers.Concatenate(axis=channel_axis, name='mixed_7a')(branches)
-
-    # 10x block8 (Inception-ResNet-C block): 8 x 8 x 2080
-    for block_idx in range(1, 10):
-        x = inception_resnet_block(x,
-                                   scale=0.2,
-                                   block_type='block8',
-                                   block_idx=block_idx)
-    x = inception_resnet_block(x,
-                               scale=1.,
-                               activation=None,
-                               block_type='block8',
-                               block_idx=10)
-
-    # Final convolution block: 8 x 8 x 1536
-    x = conv3d_bn(x, 1536, 1, name='conv_7b')
-
-    if include_top:
-        # Classification block
-        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model = models.Model(inputs, x, name='inception_resnet_v2')
-
-    # Load weights.
-    if weights == 'imagenet':
-        print('Warning: no imagenet weights available!!!')
-    elif weights is not None:
-        model.load_weights(weights)
-
-    return model
+"""Inception-ResNet V2 model for Keras.
+
+Model naming and structure follows TF-slim implementation
+(which has some additional layers and different number of
+filters from the original arXiv paper):
+https://github.com/tensorflow/models/blob/master/research/slim/nets/inception_resnet_v2.py
+
+Pre-trained ImageNet weights are also converted from TF-slim,
+which can be found in:
+https://github.com/tensorflow/models/tree/master/research/slim#pre-trained-models
+
+# Reference
+- [Inception-v4, Inception-ResNet and the Impact of
+   Residual Connections on Learning](https://arxiv.org/abs/1602.07261) (AAAI 2017)
+
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import os
+from .. import get_submodules_from_kwargs
+from keras.applications import imagenet_utils
+from keras.src.legacy.backend import int_shape
+
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+def preprocess_input(x, **kwargs):
+    """Preprocesses a numpy array encoding a batch of images.
+
+    # Arguments
+        x: a 4D numpy array consists of RGB values within [0, 255].
+
+    # Returns
+        Preprocessed array.
+    """
+    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
+
+
+def conv3d_bn(x,
+              filters,
+              kernel_size,
+              strides=1,
+              padding='same',
+              activation='relu',
+              use_bias=False,
+              name=None):
+    """Utility function to apply conv + BN.
+
+    # Arguments
+        x: input tensor.
+        filters: filters in `Conv2D`.
+        kernel_size: kernel size as in `Conv2D`.
+        strides: strides in `Conv2D`.
+        padding: padding mode in `Conv2D`.
+        activation: activation in `Conv2D`.
+        use_bias: whether to use a bias in `Conv2D`.
+        name: name of the ops; will become `name + '_ac'` for the activation
+            and `name + '_bn'` for the batch norm layer.
+
+    # Returns
+        Output tensor after applying `Conv2D` and `BatchNormalization`.
+    """
+    x = layers.Conv3D(filters,
+                      kernel_size,
+                      strides=strides,
+                      padding=padding,
+                      use_bias=use_bias,
+                      name=name)(x)
+    if not use_bias:
+        bn_axis = 1 if backend.image_data_format() == 'channels_first' else 4
+        bn_name = None if name is None else name + '_bn'
+        x = layers.BatchNormalization(axis=bn_axis,
+                                      scale=False,
+                                      name=bn_name)(x)
+    if activation is not None:
+        ac_name = None if name is None else name + '_ac'
+        x = layers.Activation(activation, name=ac_name)(x)
+    return x
+
+
+def inception_resnet_block(x, scale, block_type, block_idx, activation='relu'):
+    """Adds a Inception-ResNet block.
+
+    This function builds 3 types of Inception-ResNet blocks mentioned
+    in the paper, controlled by the `block_type` argument (which is the
+    block name used in the official TF-slim implementation):
+        - Inception-ResNet-A: `block_type='block35'`
+        - Inception-ResNet-B: `block_type='block17'`
+        - Inception-ResNet-C: `block_type='block8'`
+
+    # Arguments
+        x: input tensor.
+        scale: scaling factor to scale the residuals (i.e., the output of
+            passing `x` through an inception module) before adding them
+            to the shortcut branch.
+            Let `r` be the output from the residual branch,
+            the output of this block will be `x + scale * r`.
+        block_type: `'block35'`, `'block17'` or `'block8'`, determines
+            the network structure in the residual branch.
+        block_idx: an `int` used for generating layer names.
+            The Inception-ResNet blocks
+            are repeated many times in this network.
+            We use `block_idx` to identify
+            each of the repetitions. For example,
+            the first Inception-ResNet-A block
+            will have `block_type='block35', block_idx=0`,
+            and the layer names will have
+            a common prefix `'block35_0'`.
+        activation: activation function to use at the end of the block
+            (see [activations](../activations.md)).
+            When `activation=None`, no activation is applied
+            (i.e., "linear" activation: `a(x) = x`).
+
+    # Returns
+        Output tensor for the block.
+
+    # Raises
+        ValueError: if `block_type` is not one of `'block35'`,
+            `'block17'` or `'block8'`.
+    """
+    if block_type == 'block35':
+        branch_0 = conv3d_bn(x, 32, 1)
+        branch_1 = conv3d_bn(x, 32, 1)
+        branch_1 = conv3d_bn(branch_1, 32, 3)
+        branch_2 = conv3d_bn(x, 32, 1)
+        branch_2 = conv3d_bn(branch_2, 48, 3)
+        branch_2 = conv3d_bn(branch_2, 64, 3)
+        branches = [branch_0, branch_1, branch_2]
+    elif block_type == 'block17':
+        branch_0 = conv3d_bn(x, 192, 1)
+        branch_1 = conv3d_bn(x, 128, 1)
+        branch_1 = conv3d_bn(branch_1, 160, [1, 7, 1])
+        branch_1 = conv3d_bn(branch_1, 192, [7, 1, 1])
+        branches = [branch_0, branch_1]
+    elif block_type == 'block8':
+        branch_0 = conv3d_bn(x, 192, 1)
+        branch_1 = conv3d_bn(x, 192, 1)
+        branch_1 = conv3d_bn(branch_1, 224, [1, 3, 1])
+        branch_1 = conv3d_bn(branch_1, 256, [3, 1, 1])
+        branches = [branch_0, branch_1]
+    else:
+        raise ValueError('Unknown Inception-ResNet block type. '
+                         'Expects "block35", "block17" or "block8", '
+                         'but got: ' + str(block_type))
+
+    block_name = block_type + '_' + str(block_idx)
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else 4
+    mixed = layers.Concatenate(
+        axis=channel_axis, name=block_name + '_mixed')(branches)
+    up = conv3d_bn(mixed,
+                   int_shape(x)[channel_axis],
+                   1,
+                   activation=None,
+                   use_bias=True,
+                   name=block_name + '_conv')
+
+    x = layers.Lambda(lambda inputs, scale: inputs[0] + inputs[1] * scale,
+                      output_shape=int_shape(x)[1:],
+                      arguments={'scale': scale},
+                      name=block_name)([x, up])
+    if activation is not None:
+        x = layers.Activation(activation, name=block_name + '_ac')(x)
+    return x
+
+
+def InceptionResNetV2(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        **kwargs
+):
+    """Instantiates the Inception-ResNet v2 architecture.
+
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    # Arguments
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is `False` (otherwise the input shape
+            has to be `(299, 299, 3)` (with `'channels_last'` data format)
+            or `(3, 299, 299)` (with `'channels_first'` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 75.
+            E.g. `(150, 150, 3)` would be one valid value.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the last convolutional block.
+            - `'avg'` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a 2D tensor.
+            - `'max'` means that global max pooling will be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is `True`, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras `Model` instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) != 5:
+        print('Error: stride_size length must be exactly 5')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    # Stem block: 35 x 35 x 192
+    x = conv3d_bn(img_input, 32, 3, strides=stride_size[0], padding='same')
+    x = conv3d_bn(x, 32, 3, padding='same')
+    x = conv3d_bn(x, 64, 3)
+    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
+    x = layers.MaxPooling3D(pool, strides=stride_size[1], padding='same')(x)
+    x = conv3d_bn(x, 80, 1, padding='same')
+    x = conv3d_bn(x, 192, 3, padding='same')
+    pool = (stride_size[2][0] + 1, stride_size[2][1] + 1, stride_size[2][2] + 1)
+    x = layers.MaxPooling3D(pool, strides=stride_size[2], padding='same')(x)
+
+    # Mixed 5b (Inception-A block): 35 x 35 x 320
+    branch_0 = conv3d_bn(x, 96, 1)
+    branch_1 = conv3d_bn(x, 48, 1)
+    branch_1 = conv3d_bn(branch_1, 64, 5)
+    branch_2 = conv3d_bn(x, 64, 1)
+    branch_2 = conv3d_bn(branch_2, 96, 3)
+    branch_2 = conv3d_bn(branch_2, 96, 3)
+    branch_pool = layers.AveragePooling3D(3, strides=1, padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 64, 1)
+    branches = [branch_0, branch_1, branch_2, branch_pool]
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else 4
+    x = layers.Concatenate(axis=channel_axis, name='mixed_5b')(branches)
+
+    # 10x block35 (Inception-ResNet-A block): 35 x 35 x 320
+    for block_idx in range(1, 11):
+        x = inception_resnet_block(x,
+                                   scale=0.17,
+                                   block_type='block35',
+                                   block_idx=block_idx)
+
+    # Mixed 6a (Reduction-A block): 17 x 17 x 1088
+    branch_0 = conv3d_bn(x, 384, 3, strides=stride_size[3], padding='same')
+    branch_1 = conv3d_bn(x, 256, 1)
+    branch_1 = conv3d_bn(branch_1, 256, 3)
+    branch_1 = conv3d_bn(branch_1, 384, 3, strides=stride_size[3], padding='same')
+    pool = (stride_size[3][0] + 1, stride_size[3][1] + 1, stride_size[3][2] + 1)
+    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[3], padding='same')(x)
+    branches = [branch_0, branch_1, branch_pool]
+    x = layers.Concatenate(axis=channel_axis, name='mixed_6a')(branches)
+
+    # 20x block17 (Inception-ResNet-B block): 17 x 17 x 1088
+    for block_idx in range(1, 21):
+        x = inception_resnet_block(x,
+                                   scale=0.1,
+                                   block_type='block17',
+                                   block_idx=block_idx)
+
+    # Mixed 7a (Reduction-B block): 8 x 8 x 2080
+    branch_0 = conv3d_bn(x, 256, 1)
+    branch_0 = conv3d_bn(branch_0, 384, 3, strides=stride_size[4], padding='same')
+    branch_1 = conv3d_bn(x, 256, 1)
+    branch_1 = conv3d_bn(branch_1, 288, 3, strides=stride_size[4], padding='same')
+    branch_2 = conv3d_bn(x, 256, 1)
+    branch_2 = conv3d_bn(branch_2, 288, 3)
+    branch_2 = conv3d_bn(branch_2, 320, 3, strides=stride_size[4], padding='same')
+    pool = (stride_size[4][0] + 1, stride_size[4][1] + 1, stride_size[4][2] + 1)
+    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[4], padding='same')(x)
+    branches = [branch_0, branch_1, branch_2, branch_pool]
+    x = layers.Concatenate(axis=channel_axis, name='mixed_7a')(branches)
+
+    # 10x block8 (Inception-ResNet-C block): 8 x 8 x 2080
+    for block_idx in range(1, 10):
+        x = inception_resnet_block(x,
+                                   scale=0.2,
+                                   block_type='block8',
+                                   block_idx=block_idx)
+    x = inception_resnet_block(x,
+                               scale=1.,
+                               activation=None,
+                               block_type='block8',
+                               block_idx=10)
+
+    # Final convolution block: 8 x 8 x 1536
+    x = conv3d_bn(x, 1536, 1, name='conv_7b')
+
+    if include_top:
+        # Classification block
+        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model = models.Model(inputs, x, name='inception_resnet_v2')
+
+    # Load weights.
+    if weights == 'imagenet':
+        print('Warning: no imagenet weights available!!!')
+    elif weights is not None:
+        model.load_weights(weights)
+
+    return model
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/inception_v3.py` & `classification_models_3D-1.1.0/classification_models_3D/models/inception_v3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,404 +1,404 @@
-"""Inception V3 model for Keras.
-
-Note that the input image format for this model is different than for
-the VGG16 and ResNet models (299x299 instead of 224x224),
-and that the input preprocessing function is also different (same as Xception).
-
-# Reference
-
-- [Rethinking the Inception Architecture for Computer Vision](
-    http://arxiv.org/abs/1512.00567) (CVPR 2016)
-
-"""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from .. import get_submodules_from_kwargs
-from keras_applications import imagenet_utils
-
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-def conv3d_bn(
-        x,
-        filters,
-        num_row,
-        num_col,
-        num_z,
-        padding='same',
-        strides=(1, 1, 1),
-        name=None
-):
-    """Utility function to apply conv + BN.
-
-    # Arguments
-        x: input tensor.
-        filters: filters in `Conv2D`.
-        num_row: height of the convolution kernel.
-        num_col: width of the convolution kernel.
-        padding: padding mode in `Conv2D`.
-        strides: strides in `Conv2D`.
-        name: name of the ops; will become `name + '_conv'`
-            for the convolution and `name + '_bn'` for the
-            batch norm layer.
-
-    # Returns
-        Output tensor after applying `Conv2D` and `BatchNormalization`.
-    """
-    if name is not None:
-        bn_name = name + '_bn'
-        conv_name = name + '_conv'
-    else:
-        bn_name = None
-        conv_name = None
-    if backend.image_data_format() == 'channels_first':
-        bn_axis = 1
-    else:
-        bn_axis = 4
-    x = layers.Conv3D(
-        filters, (num_row, num_col, num_z),
-        strides=strides,
-        padding=padding,
-        use_bias=False,
-        name=conv_name)(x)
-    x = layers.BatchNormalization(axis=bn_axis, scale=False, name=bn_name)(x)
-    x = layers.Activation('relu', name=name)(x)
-    return x
-
-
-def InceptionV3(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        **kwargs
-):
-    """Instantiates the Inception v3 architecture.
-
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    # Arguments
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(299, 299, 3)` (with `channels_last` data format)
-            or `(3, 299, 299)` (with `channels_first` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 75.
-            E.g. `(150, 150, 3)` would be one valid value.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a 2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) != 5:
-        print('Error: stride_size length must be exactly 5')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    if backend.image_data_format() == 'channels_first':
-        channel_axis = 1
-    else:
-        channel_axis = 4
-
-    x = conv3d_bn(img_input, 32, 3, 3, 3, strides=stride_size[0], padding='same')
-    x = conv3d_bn(x, 32, 3, 3, 3, padding='same')
-    x = conv3d_bn(x, 64, 3, 3, 3)
-    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
-    x = layers.MaxPooling3D(pool, strides=stride_size[1], padding='same')(x)
-
-    x = conv3d_bn(x, 80, 1, 1, 1, padding='same')
-    x = conv3d_bn(x, 192, 3, 3, 3, padding='same')
-    pool = (stride_size[2][0] + 1, stride_size[2][1] + 1, stride_size[2][2] + 1)
-    x = layers.MaxPooling3D(pool, strides=stride_size[2], padding='same')(x)
-
-    # mixed 0: 35 x 35 x 256
-    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
-
-    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
-    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
-
-    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-
-    branch_pool = layers.AveragePooling3D((3, 3, 3),
-                                          strides=(1, 1, 1),
-                                          padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 32, 1, 1, 1)
-    x = layers.concatenate(
-        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed0')
-
-    # mixed 1: 35 x 35 x 288
-    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
-
-    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
-    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
-
-    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-
-    branch_pool = layers.AveragePooling3D((3, 3, 3),
-                                          strides=(1, 1, 1),
-                                          padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 64, 1, 1, 1)
-    x = layers.concatenate(
-        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed1')
-
-    # mixed 2: 35 x 35 x 288
-    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
-
-    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
-    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
-
-    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-
-    branch_pool = layers.AveragePooling3D((3, 3, 3),
-                                          strides=(1, 1, 1),
-                                          padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 64, 1, 1, 1)
-    x = layers.concatenate(
-        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed2')
-
-    # mixed 3: 17 x 17 x 768
-    branch3x3 = conv3d_bn(x, 384, 3, 3, 3, strides=stride_size[3], padding='same')
-
-    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
-    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3, strides=stride_size[3], padding='same')
-
-    pool = (stride_size[3][0] + 1, stride_size[3][1] + 1, stride_size[3][2] + 1)
-    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[3], padding='same')(x)
-    x = layers.concatenate(
-        [branch3x3, branch3x3dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed3')
-
-    # mixed 4: 17 x 17 x 768
-    branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
-
-    branch7x7 = conv3d_bn(x, 128, 1, 1, 1)
-    branch7x7 = conv3d_bn(branch7x7, 128, 1, 7, 1)
-    branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
-
-    branch7x7dbl = conv3d_bn(x, 128, 1, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 7, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 1, 7, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 7, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
-
-    branch_pool = layers.AveragePooling3D((3, 3, 3),
-                                          strides=(1, 1, 1),
-                                          padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
-    x = layers.concatenate(
-        [branch1x1, branch7x7, branch7x7dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed4')
-
-    # mixed 5, 6: 17 x 17 x 768
-    for i in range(2):
-        branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
-
-        branch7x7 = conv3d_bn(x, 160, 1, 1, 1)
-        branch7x7 = conv3d_bn(branch7x7, 160, 1, 7, 1)
-        branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
-
-        branch7x7dbl = conv3d_bn(x, 160, 1, 1, 1)
-        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 7, 1, 1)
-        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 1, 7, 1)
-        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 7, 1, 1)
-        branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
-
-        branch_pool = layers.AveragePooling3D(
-            (3, 3, 3), strides=(1, 1, 1), padding='same')(x)
-        branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
-        x = layers.concatenate(
-            [branch1x1, branch7x7, branch7x7dbl, branch_pool],
-            axis=channel_axis,
-            name='mixed' + str(5 + i))
-
-    # mixed 7: 17 x 17 x 768
-    branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
-
-    branch7x7 = conv3d_bn(x, 192, 1, 1, 1)
-    branch7x7 = conv3d_bn(branch7x7, 192, 1, 7, 1)
-    branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
-
-    branch7x7dbl = conv3d_bn(x, 192, 1, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 7, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 7, 1, 1)
-    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
-
-    branch_pool = layers.AveragePooling3D((3, 3, 3),
-                                          strides=(1, 1, 1),
-                                          padding='same')(x)
-    branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
-    x = layers.concatenate(
-        [branch1x1, branch7x7, branch7x7dbl, branch_pool],
-        axis=channel_axis,
-        name='mixed7')
-
-    # mixed 8: 8 x 8 x 1280
-    branch3x3 = conv3d_bn(x, 192, 1, 1, 1)
-    branch3x3 = conv3d_bn(branch3x3, 320, 3, 3, 3,
-                          strides=stride_size[4], padding='same')
-
-    branch7x7x3 = conv3d_bn(x, 192, 1, 1, 1)
-    branch7x7x3 = conv3d_bn(branch7x7x3, 192, 1, 7, 1)
-    branch7x7x3 = conv3d_bn(branch7x7x3, 192, 7, 1, 1)
-    branch7x7x3 = conv3d_bn(
-        branch7x7x3, 192, 3, 3, 3, strides=stride_size[4], padding='same')
-
-    pool = (stride_size[4][0] + 1, stride_size[4][1] + 1, stride_size[4][2] + 1)
-    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[4], padding='same')(x)
-    x = layers.concatenate(
-        [branch3x3, branch7x7x3, branch_pool],
-        axis=channel_axis,
-        name='mixed8')
-
-    # mixed 9: 8 x 8 x 2048
-    for i in range(2):
-        branch1x1 = conv3d_bn(x, 320, 1, 1, 1)
-
-        branch3x3 = conv3d_bn(x, 384, 1, 1, 1)
-        branch3x3_1 = conv3d_bn(branch3x3, 384, 1, 3, 1)
-        branch3x3_2 = conv3d_bn(branch3x3, 384, 3, 1, 1)
-        branch3x3 = layers.concatenate(
-            [branch3x3_1, branch3x3_2],
-            axis=channel_axis,
-            name='mixed9_' + str(i))
-
-        branch3x3dbl = conv3d_bn(x, 448, 1, 1, 1)
-        branch3x3dbl = conv3d_bn(branch3x3dbl, 384, 3, 3, 3)
-        branch3x3dbl_1 = conv3d_bn(branch3x3dbl, 384, 1, 3, 1)
-        branch3x3dbl_2 = conv3d_bn(branch3x3dbl, 384, 3, 1, 1)
-        branch3x3dbl = layers.concatenate(
-            [branch3x3dbl_1, branch3x3dbl_2], axis=channel_axis)
-
-        branch_pool = layers.AveragePooling3D(
-            (3, 3, 3), strides=(1, 1, 1), padding='same')(x)
-        branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
-        x = layers.concatenate(
-            [branch1x1, branch3x3, branch3x3dbl, branch_pool],
-            axis=channel_axis,
-            name='mixed' + str(9 + i))
-    if include_top:
-        # Classification block
-        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
-        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-    # Create model.
-    model = models.Model(inputs, x, name='inception_v3')
-
-    # Load weights.
-    if weights == 'imagenet':
-        print('Warning: no imagenet weights available!!!')
-    elif weights is not None:
-        model.load_weights(weights)
-
-    return model
-
-
-def preprocess_input(x, **kwargs):
-    """Preprocesses a numpy array encoding a batch of images.
-
-    # Arguments
-        x: a 4D numpy array consists of RGB values within [0, 255].
-
-    # Returns
-        Preprocessed array.
-    """
-    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
+"""Inception V3 model for Keras.
+
+Note that the input image format for this model is different than for
+the VGG16 and ResNet models (299x299 instead of 224x224),
+and that the input preprocessing function is also different (same as Xception).
+
+# Reference
+
+- [Rethinking the Inception Architecture for Computer Vision](
+    http://arxiv.org/abs/1512.00567) (CVPR 2016)
+
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import os
+from .. import get_submodules_from_kwargs
+from keras.applications import imagenet_utils
+
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+def conv3d_bn(
+        x,
+        filters,
+        num_row,
+        num_col,
+        num_z,
+        padding='same',
+        strides=(1, 1, 1),
+        name=None
+):
+    """Utility function to apply conv + BN.
+
+    # Arguments
+        x: input tensor.
+        filters: filters in `Conv2D`.
+        num_row: height of the convolution kernel.
+        num_col: width of the convolution kernel.
+        padding: padding mode in `Conv2D`.
+        strides: strides in `Conv2D`.
+        name: name of the ops; will become `name + '_conv'`
+            for the convolution and `name + '_bn'` for the
+            batch norm layer.
+
+    # Returns
+        Output tensor after applying `Conv2D` and `BatchNormalization`.
+    """
+    if name is not None:
+        bn_name = name + '_bn'
+        conv_name = name + '_conv'
+    else:
+        bn_name = None
+        conv_name = None
+    if backend.image_data_format() == 'channels_first':
+        bn_axis = 1
+    else:
+        bn_axis = 4
+    x = layers.Conv3D(
+        filters, (num_row, num_col, num_z),
+        strides=strides,
+        padding=padding,
+        use_bias=False,
+        name=conv_name)(x)
+    x = layers.BatchNormalization(axis=bn_axis, scale=False, name=bn_name)(x)
+    x = layers.Activation('relu', name=name)(x)
+    return x
+
+
+def InceptionV3(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        **kwargs
+):
+    """Instantiates the Inception v3 architecture.
+
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    # Arguments
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(299, 299, 3)` (with `channels_last` data format)
+            or `(3, 299, 299)` (with `channels_first` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 75.
+            E.g. `(150, 150, 3)` would be one valid value.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a 2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) != 5:
+        print('Error: stride_size length must be exactly 5')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    if backend.image_data_format() == 'channels_first':
+        channel_axis = 1
+    else:
+        channel_axis = 4
+
+    x = conv3d_bn(img_input, 32, 3, 3, 3, strides=stride_size[0], padding='same')
+    x = conv3d_bn(x, 32, 3, 3, 3, padding='same')
+    x = conv3d_bn(x, 64, 3, 3, 3)
+    pool = (stride_size[1][0] + 1, stride_size[1][1] + 1, stride_size[1][2] + 1)
+    x = layers.MaxPooling3D(pool, strides=stride_size[1], padding='same')(x)
+
+    x = conv3d_bn(x, 80, 1, 1, 1, padding='same')
+    x = conv3d_bn(x, 192, 3, 3, 3, padding='same')
+    pool = (stride_size[2][0] + 1, stride_size[2][1] + 1, stride_size[2][2] + 1)
+    x = layers.MaxPooling3D(pool, strides=stride_size[2], padding='same')(x)
+
+    # mixed 0: 35 x 35 x 256
+    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
+
+    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
+    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
+
+    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+
+    branch_pool = layers.AveragePooling3D((3, 3, 3),
+                                          strides=(1, 1, 1),
+                                          padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 32, 1, 1, 1)
+    x = layers.concatenate(
+        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed0')
+
+    # mixed 1: 35 x 35 x 288
+    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
+
+    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
+    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
+
+    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+
+    branch_pool = layers.AveragePooling3D((3, 3, 3),
+                                          strides=(1, 1, 1),
+                                          padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 64, 1, 1, 1)
+    x = layers.concatenate(
+        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed1')
+
+    # mixed 2: 35 x 35 x 288
+    branch1x1 = conv3d_bn(x, 64, 1, 1, 1)
+
+    branch5x5 = conv3d_bn(x, 48, 1, 1, 1)
+    branch5x5 = conv3d_bn(branch5x5, 64, 5, 5, 5)
+
+    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+
+    branch_pool = layers.AveragePooling3D((3, 3, 3),
+                                          strides=(1, 1, 1),
+                                          padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 64, 1, 1, 1)
+    x = layers.concatenate(
+        [branch1x1, branch5x5, branch3x3dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed2')
+
+    # mixed 3: 17 x 17 x 768
+    branch3x3 = conv3d_bn(x, 384, 3, 3, 3, strides=stride_size[3], padding='same')
+
+    branch3x3dbl = conv3d_bn(x, 64, 1, 1, 1)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3)
+    branch3x3dbl = conv3d_bn(branch3x3dbl, 96, 3, 3, 3, strides=stride_size[3], padding='same')
+
+    pool = (stride_size[3][0] + 1, stride_size[3][1] + 1, stride_size[3][2] + 1)
+    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[3], padding='same')(x)
+    x = layers.concatenate(
+        [branch3x3, branch3x3dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed3')
+
+    # mixed 4: 17 x 17 x 768
+    branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
+
+    branch7x7 = conv3d_bn(x, 128, 1, 1, 1)
+    branch7x7 = conv3d_bn(branch7x7, 128, 1, 7, 1)
+    branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
+
+    branch7x7dbl = conv3d_bn(x, 128, 1, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 7, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 1, 7, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 128, 7, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
+
+    branch_pool = layers.AveragePooling3D((3, 3, 3),
+                                          strides=(1, 1, 1),
+                                          padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
+    x = layers.concatenate(
+        [branch1x1, branch7x7, branch7x7dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed4')
+
+    # mixed 5, 6: 17 x 17 x 768
+    for i in range(2):
+        branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
+
+        branch7x7 = conv3d_bn(x, 160, 1, 1, 1)
+        branch7x7 = conv3d_bn(branch7x7, 160, 1, 7, 1)
+        branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
+
+        branch7x7dbl = conv3d_bn(x, 160, 1, 1, 1)
+        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 7, 1, 1)
+        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 1, 7, 1)
+        branch7x7dbl = conv3d_bn(branch7x7dbl, 160, 7, 1, 1)
+        branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
+
+        branch_pool = layers.AveragePooling3D(
+            (3, 3, 3), strides=(1, 1, 1), padding='same')(x)
+        branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
+        x = layers.concatenate(
+            [branch1x1, branch7x7, branch7x7dbl, branch_pool],
+            axis=channel_axis,
+            name='mixed' + str(5 + i))
+
+    # mixed 7: 17 x 17 x 768
+    branch1x1 = conv3d_bn(x, 192, 1, 1, 1)
+
+    branch7x7 = conv3d_bn(x, 192, 1, 1, 1)
+    branch7x7 = conv3d_bn(branch7x7, 192, 1, 7, 1)
+    branch7x7 = conv3d_bn(branch7x7, 192, 7, 1, 1)
+
+    branch7x7dbl = conv3d_bn(x, 192, 1, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 7, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 7, 1, 1)
+    branch7x7dbl = conv3d_bn(branch7x7dbl, 192, 1, 7, 1)
+
+    branch_pool = layers.AveragePooling3D((3, 3, 3),
+                                          strides=(1, 1, 1),
+                                          padding='same')(x)
+    branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
+    x = layers.concatenate(
+        [branch1x1, branch7x7, branch7x7dbl, branch_pool],
+        axis=channel_axis,
+        name='mixed7')
+
+    # mixed 8: 8 x 8 x 1280
+    branch3x3 = conv3d_bn(x, 192, 1, 1, 1)
+    branch3x3 = conv3d_bn(branch3x3, 320, 3, 3, 3,
+                          strides=stride_size[4], padding='same')
+
+    branch7x7x3 = conv3d_bn(x, 192, 1, 1, 1)
+    branch7x7x3 = conv3d_bn(branch7x7x3, 192, 1, 7, 1)
+    branch7x7x3 = conv3d_bn(branch7x7x3, 192, 7, 1, 1)
+    branch7x7x3 = conv3d_bn(
+        branch7x7x3, 192, 3, 3, 3, strides=stride_size[4], padding='same')
+
+    pool = (stride_size[4][0] + 1, stride_size[4][1] + 1, stride_size[4][2] + 1)
+    branch_pool = layers.MaxPooling3D(pool, strides=stride_size[4], padding='same')(x)
+    x = layers.concatenate(
+        [branch3x3, branch7x7x3, branch_pool],
+        axis=channel_axis,
+        name='mixed8')
+
+    # mixed 9: 8 x 8 x 2048
+    for i in range(2):
+        branch1x1 = conv3d_bn(x, 320, 1, 1, 1)
+
+        branch3x3 = conv3d_bn(x, 384, 1, 1, 1)
+        branch3x3_1 = conv3d_bn(branch3x3, 384, 1, 3, 1)
+        branch3x3_2 = conv3d_bn(branch3x3, 384, 3, 1, 1)
+        branch3x3 = layers.concatenate(
+            [branch3x3_1, branch3x3_2],
+            axis=channel_axis,
+            name='mixed9_' + str(i))
+
+        branch3x3dbl = conv3d_bn(x, 448, 1, 1, 1)
+        branch3x3dbl = conv3d_bn(branch3x3dbl, 384, 3, 3, 3)
+        branch3x3dbl_1 = conv3d_bn(branch3x3dbl, 384, 1, 3, 1)
+        branch3x3dbl_2 = conv3d_bn(branch3x3dbl, 384, 3, 1, 1)
+        branch3x3dbl = layers.concatenate(
+            [branch3x3dbl_1, branch3x3dbl_2], axis=channel_axis)
+
+        branch_pool = layers.AveragePooling3D(
+            (3, 3, 3), strides=(1, 1, 1), padding='same')(x)
+        branch_pool = conv3d_bn(branch_pool, 192, 1, 1, 1)
+        x = layers.concatenate(
+            [branch1x1, branch3x3, branch3x3dbl, branch_pool],
+            axis=channel_axis,
+            name='mixed' + str(9 + i))
+    if include_top:
+        # Classification block
+        x = layers.GlobalAveragePooling3D(name='avg_pool')(x)
+        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+    # Create model.
+    model = models.Model(inputs, x, name='inception_v3')
+
+    # Load weights.
+    if weights == 'imagenet':
+        print('Warning: no imagenet weights available!!!')
+    elif weights is not None:
+        model.load_weights(weights)
+
+    return model
+
+
+def preprocess_input(x, **kwargs):
+    """Preprocesses a numpy array encoding a batch of images.
+
+    # Arguments
+        x: a 4D numpy array consists of RGB values within [0, 255].
+
+    # Returns
+        Preprocessed array.
+    """
+    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/mobilenet.py` & `classification_models_3D-1.1.0/classification_models_3D/models/mobilenet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,433 +1,433 @@
-"""MobileNet v1 models for Keras.
-
-MobileNet is a general architecture and can be used for multiple use cases.
-Depending on the use case, it can use different input layer size and
-different width factors. This allows different width models to reduce
-the number of multiply-adds and thereby
-reduce inference cost on mobile devices.
-
-MobileNets support any input size greater than 32 x 32, with larger image sizes
-offering better performance.
-The number of parameters and number of multiply-adds
-can be modified by using the `alpha` parameter,
-which increases/decreases the number of filters in each layer.
-By altering the image size and `alpha` parameter,
-all 16 models from the paper can be built, with ImageNet weights provided.
-
-The paper demonstrates the performance of MobileNets using `alpha` values of
-1.0 (also called 100 % MobileNet), 0.75, 0.5 and 0.25.
-For each of these `alpha` values, weights for 4 different input image sizes
-are provided (224, 192, 160, 128).
-
-The following table describes the size and accuracy of the 100% MobileNet
-on size 224 x 224:
-----------------------------------------------------------------------------
-Width Multiplier (alpha) | ImageNet Acc |  Multiply-Adds (M) |  Params (M)
-----------------------------------------------------------------------------
-|   1.0 MobileNet-224    |    70.6 %     |        529        |     4.2     |
-|   0.75 MobileNet-224   |    68.4 %     |        325        |     2.6     |
-|   0.50 MobileNet-224   |    63.7 %     |        149        |     1.3     |
-|   0.25 MobileNet-224   |    50.6 %     |        41         |     0.5     |
-----------------------------------------------------------------------------
-
-The following table describes the performance of
-the 100 % MobileNet on various input sizes:
-------------------------------------------------------------------------
-      Resolution      | ImageNet Acc | Multiply-Adds (M) | Params (M)
-------------------------------------------------------------------------
-|  1.0 MobileNet-224  |    70.6 %    |        529        |     4.2     |
-|  1.0 MobileNet-192  |    69.1 %    |        529        |     4.2     |
-|  1.0 MobileNet-160  |    67.2 %    |        529        |     4.2     |
-|  1.0 MobileNet-128  |    64.4 %    |        529        |     4.2     |
-------------------------------------------------------------------------
-
-The weights for all 16 models are obtained and translated
-from TensorFlow checkpoints found at
-https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet_v1.md
-
-# Reference
-
-- [MobileNets: Efficient Convolutional Neural Networks for
-   Mobile Vision Applications](https://arxiv.org/abs/1704.04861)
-"""
-from __future__ import print_function
-from __future__ import absolute_import
-from __future__ import division
-
-import os
-import warnings
-from .. import get_submodules_from_kwargs
-from ..weights import load_model_weights
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-from keras_applications import imagenet_utils
-
-
-
-def preprocess_input(x, **kwargs):
-    """Preprocesses a numpy array encoding a batch of images.
-
-    # Arguments
-        x: a 4D numpy array consists of RGB values within [0, 255].
-
-    # Returns
-        Preprocessed array.
-    """
-    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
-
-
-def MobileNet(
-        input_shape=None,
-        alpha=1.0,
-        depth_multiplier=1,
-        dropout=1e-3,
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        **kwargs
-):
-    """Instantiates the MobileNet architecture.
-
-    # Arguments
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(224, 224, 3)`
-            (with `channels_last` data format)
-            or (3, 224, 224) (with `channels_first` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 32.
-            E.g. `(200, 200, 3)` would be one valid value.
-        alpha: controls the width of the network. This is known as the
-            width multiplier in the MobileNet paper.
-            - If `alpha` < 1.0, proportionally decreases the number
-                of filters in each layer.
-            - If `alpha` > 1.0, proportionally increases the number
-                of filters in each layer.
-            - If `alpha` = 1, default number of filters from the paper
-                 are used at each layer.
-        depth_multiplier: depth multiplier for depthwise convolution. This
-            is called the resolution multiplier in the MobileNet paper.
-        dropout: dropout rate
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor (i.e. output of
-            `layers.Input()`)
-            to use as image input for the model.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model
-                will be the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a
-                2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-        RuntimeError: If attempting to run this model with a
-            backend that does not support separable convolutions.
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top` '
-                         'as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) != 5:
-        print('Error: stride_size length must be exactly 5')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    # Determine proper input shape and default size.
-    if input_shape is None:
-        default_size = 224
-    else:
-        if backend.image_data_format() == 'channels_first':
-            rows = input_shape[1]
-            cols = input_shape[2]
-        else:
-            rows = input_shape[0]
-            cols = input_shape[1]
-
-        if rows == cols and rows in [128, 160, 192, 224]:
-            default_size = rows
-        else:
-            default_size = 224
-
-
-    if backend.image_data_format() == 'channels_last':
-        row_axis, col_axis = (0, 1)
-    else:
-        row_axis, col_axis = (1, 2)
-    rows = input_shape[row_axis]
-    cols = input_shape[col_axis]
-
-    if weights == 'imagenet':
-        if depth_multiplier != 1:
-            raise ValueError('If imagenet weights are being loaded, '
-                             'depth multiplier must be 1')
-
-        if alpha not in [0.25, 0.50, 0.75, 1.0]:
-            raise ValueError('If imagenet weights are being loaded, '
-                             'alpha can be one of'
-                             '`0.25`, `0.50`, `0.75` or `1.0` only.')
-
-        if rows != cols or rows not in [128, 160, 192, 224]:
-            rows = 224
-            warnings.warn('`input_shape` is undefined or non-square, '
-                          'or `rows` is not in [128, 160, 192, 224]. '
-                          'Weights for input shape (224, 224) will be'
-                          ' loaded as the default.')
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    x = _conv_block(img_input, 32, alpha, strides=stride_size[0])
-    x = _depthwise_conv_block(x, 64, alpha, depth_multiplier, block_id=1)
-
-    x = _depthwise_conv_block(x, 128, alpha, depth_multiplier, strides=stride_size[1], block_id=2)
-    x = _depthwise_conv_block(x, 128, alpha, depth_multiplier, block_id=3)
-
-    x = _depthwise_conv_block(x, 256, alpha, depth_multiplier, strides=stride_size[2], block_id=4)
-    x = _depthwise_conv_block(x, 256, alpha, depth_multiplier, block_id=5)
-
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, strides=stride_size[3], block_id=6)
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=7)
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=8)
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=9)
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=10)
-    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=11)
-
-    x = _depthwise_conv_block(x, 1024, alpha, depth_multiplier, strides=stride_size[4], block_id=12)
-    x = _depthwise_conv_block(x, 1024, alpha, depth_multiplier, block_id=13)
-
-    if include_top:
-        if backend.image_data_format() == 'channels_first':
-            shape = (int(1024 * alpha), 1, 1, 1)
-        else:
-            shape = (1, 1, 1, int(1024 * alpha))
-
-        x = layers.GlobalAveragePooling3D()(x)
-        x = layers.Reshape(shape, name='reshape_1')(x)
-        x = layers.Dropout(dropout, name='dropout')(x)
-        x = layers.Conv3D(classes, (1, 1, 1),
-                          padding='same',
-                          name='conv_preds')(x)
-        x = layers.Reshape((classes,), name='reshape_2')(x)
-        x = layers.Activation('softmax', name='act_softmax')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model = models.Model(inputs, x, name='mobilenet_%0.2f_%s' % (alpha, rows))
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, 'mobilenet', weights, classes, include_top, **kwargs)
-
-    return model
-
-
-def _conv_block(inputs, filters, alpha, kernel=(3, 3, 3), strides=(1, 1, 1)):
-    """Adds an initial convolution layer (with batch normalization and relu6).
-
-    # Arguments
-        inputs: Input tensor of shape `(rows, cols, 3)`
-            (with `channels_last` data format) or
-            (3, rows, cols) (with `channels_first` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 32.
-            E.g. `(224, 224, 3)` would be one valid value.
-        filters: Integer, the dimensionality of the output space
-            (i.e. the number of output filters in the convolution).
-        alpha: controls the width of the network.
-            - If `alpha` < 1.0, proportionally decreases the number
-                of filters in each layer.
-            - If `alpha` > 1.0, proportionally increases the number
-                of filters in each layer.
-            - If `alpha` = 1, default number of filters from the paper
-                 are used at each layer.
-        kernel: An integer or tuple/list of 2 integers, specifying the
-            width and height of the 2D convolution window.
-            Can be a single integer to specify the same value for
-            all spatial dimensions.
-        strides: An integer or tuple/list of 2 integers,
-            specifying the strides of the convolution
-            along the width and height.
-            Can be a single integer to specify the same value for
-            all spatial dimensions.
-            Specifying any stride value != 1 is incompatible with specifying
-            any `dilation_rate` value != 1.
-
-    # Input shape
-        4D tensor with shape:
-        `(samples, channels, rows, cols)` if data_format='channels_first'
-        or 4D tensor with shape:
-        `(samples, rows, cols, channels)` if data_format='channels_last'.
-
-    # Output shape
-        4D tensor with shape:
-        `(samples, filters, new_rows, new_cols)`
-        if data_format='channels_first'
-        or 4D tensor with shape:
-        `(samples, new_rows, new_cols, filters)`
-        if data_format='channels_last'.
-        `rows` and `cols` values might have changed due to stride.
-
-    # Returns
-        Output tensor of block.
-    """
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
-    filters = int(filters * alpha)
-    x = layers.ZeroPadding3D(padding=((0, 1), (0, 1), (0, 1)), name='conv1_pad')(inputs)
-    x = layers.Conv3D(filters, kernel,
-                      padding='valid',
-                      use_bias=False,
-                      strides=strides,
-                      name='conv1')(x)
-    x = layers.BatchNormalization(axis=channel_axis, name='conv1_bn')(x)
-    return layers.ReLU(6., name='conv1_relu')(x)
-
-
-def _depthwise_conv_block(inputs, pointwise_conv_filters, alpha,
-                          depth_multiplier=1, strides=(1, 1, 1), block_id=1):
-    """Adds a depthwise convolution block.
-
-    A depthwise convolution block consists of a depthwise conv,
-    batch normalization, relu6, pointwise convolution,
-    batch normalization and relu6 activation.
-
-    # Arguments
-        inputs: Input tensor of shape `(rows, cols, channels)`
-            (with `channels_last` data format) or
-            (channels, rows, cols) (with `channels_first` data format).
-        pointwise_conv_filters: Integer, the dimensionality of the output space
-            (i.e. the number of output filters in the pointwise convolution).
-        alpha: controls the width of the network.
-            - If `alpha` < 1.0, proportionally decreases the number
-                of filters in each layer.
-            - If `alpha` > 1.0, proportionally increases the number
-                of filters in each layer.
-            - If `alpha` = 1, default number of filters from the paper
-                 are used at each layer.
-        depth_multiplier: The number of depthwise convolution output channels
-            for each input channel.
-            The total number of depthwise convolution output
-            channels will be equal to `filters_in * depth_multiplier`.
-        strides: An integer or tuple/list of 2 integers,
-            specifying the strides of the convolution
-            along the width and height.
-            Can be a single integer to specify the same value for
-            all spatial dimensions.
-            Specifying any stride value != 1 is incompatible with specifying
-            any `dilation_rate` value != 1.
-        block_id: Integer, a unique identification designating
-            the block number.
-
-    # Input shape
-        4D tensor with shape:
-        `(batch, channels, rows, cols)` if data_format='channels_first'
-        or 4D tensor with shape:
-        `(batch, rows, cols, channels)` if data_format='channels_last'.
-
-    # Output shape
-        4D tensor with shape:
-        `(batch, filters, new_rows, new_cols)`
-        if data_format='channels_first'
-        or 4D tensor with shape:
-        `(batch, new_rows, new_cols, filters)`
-        if data_format='channels_last'.
-        `rows` and `cols` values might have changed due to stride.
-
-    # Returns
-        Output tensor of block.
-    """
-    from ..models._DepthwiseConv3D import DepthwiseConv3D
-
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
-    pointwise_conv_filters = int(pointwise_conv_filters * alpha)
-
-    if strides == (1, 1, 1):
-        x = inputs
-    else:
-        x = layers.ZeroPadding3D(((0, 1), (0, 1), (0, 1)),
-                                 name='conv_pad_%d' % block_id)(inputs)
-    x = DepthwiseConv3D((3, 3, 3),
-                               padding='same' if strides == (1, 1, 1) else 'valid',
-                               depth_multiplier=depth_multiplier,
-                               strides=strides,
-                               use_bias=False,
-                               name='conv_dw_%d' % block_id)(x)
-    x = layers.BatchNormalization(
-        axis=channel_axis, name='conv_dw_%d_bn' % block_id)(x)
-    x = layers.ReLU(6., name='conv_dw_%d_relu' % block_id)(x)
-
-    x = layers.Conv3D(pointwise_conv_filters, (1, 1, 1),
-                      padding='same',
-                      use_bias=False,
-                      strides=(1, 1, 1),
-                      name='conv_pw_%d' % block_id)(x)
-    x = layers.BatchNormalization(axis=channel_axis,
-                                  name='conv_pw_%d_bn' % block_id)(x)
-    return layers.ReLU(6., name='conv_pw_%d_relu' % block_id)(x)
+"""MobileNet v1 models for Keras.
+
+MobileNet is a general architecture and can be used for multiple use cases.
+Depending on the use case, it can use different input layer size and
+different width factors. This allows different width models to reduce
+the number of multiply-adds and thereby
+reduce inference cost on mobile devices.
+
+MobileNets support any input size greater than 32 x 32, with larger image sizes
+offering better performance.
+The number of parameters and number of multiply-adds
+can be modified by using the `alpha` parameter,
+which increases/decreases the number of filters in each layer.
+By altering the image size and `alpha` parameter,
+all 16 models from the paper can be built, with ImageNet weights provided.
+
+The paper demonstrates the performance of MobileNets using `alpha` values of
+1.0 (also called 100 % MobileNet), 0.75, 0.5 and 0.25.
+For each of these `alpha` values, weights for 4 different input image sizes
+are provided (224, 192, 160, 128).
+
+The following table describes the size and accuracy of the 100% MobileNet
+on size 224 x 224:
+----------------------------------------------------------------------------
+Width Multiplier (alpha) | ImageNet Acc |  Multiply-Adds (M) |  Params (M)
+----------------------------------------------------------------------------
+|   1.0 MobileNet-224    |    70.6 %     |        529        |     4.2     |
+|   0.75 MobileNet-224   |    68.4 %     |        325        |     2.6     |
+|   0.50 MobileNet-224   |    63.7 %     |        149        |     1.3     |
+|   0.25 MobileNet-224   |    50.6 %     |        41         |     0.5     |
+----------------------------------------------------------------------------
+
+The following table describes the performance of
+the 100 % MobileNet on various input sizes:
+------------------------------------------------------------------------
+      Resolution      | ImageNet Acc | Multiply-Adds (M) | Params (M)
+------------------------------------------------------------------------
+|  1.0 MobileNet-224  |    70.6 %    |        529        |     4.2     |
+|  1.0 MobileNet-192  |    69.1 %    |        529        |     4.2     |
+|  1.0 MobileNet-160  |    67.2 %    |        529        |     4.2     |
+|  1.0 MobileNet-128  |    64.4 %    |        529        |     4.2     |
+------------------------------------------------------------------------
+
+The weights for all 16 models are obtained and translated
+from TensorFlow checkpoints found at
+https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet_v1.md
+
+# Reference
+
+- [MobileNets: Efficient Convolutional Neural Networks for
+   Mobile Vision Applications](https://arxiv.org/abs/1704.04861)
+"""
+from __future__ import print_function
+from __future__ import absolute_import
+from __future__ import division
+
+import os
+import warnings
+from .. import get_submodules_from_kwargs
+from ..weights import load_model_weights
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+from keras.applications import imagenet_utils
+
+
+
+def preprocess_input(x, **kwargs):
+    """Preprocesses a numpy array encoding a batch of images.
+
+    # Arguments
+        x: a 4D numpy array consists of RGB values within [0, 255].
+
+    # Returns
+        Preprocessed array.
+    """
+    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
+
+
+def MobileNet(
+        input_shape=None,
+        alpha=1.0,
+        depth_multiplier=1,
+        dropout=1e-3,
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        **kwargs
+):
+    """Instantiates the MobileNet architecture.
+
+    # Arguments
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(224, 224, 3)`
+            (with `channels_last` data format)
+            or (3, 224, 224) (with `channels_first` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 32.
+            E.g. `(200, 200, 3)` would be one valid value.
+        alpha: controls the width of the network. This is known as the
+            width multiplier in the MobileNet paper.
+            - If `alpha` < 1.0, proportionally decreases the number
+                of filters in each layer.
+            - If `alpha` > 1.0, proportionally increases the number
+                of filters in each layer.
+            - If `alpha` = 1, default number of filters from the paper
+                 are used at each layer.
+        depth_multiplier: depth multiplier for depthwise convolution. This
+            is called the resolution multiplier in the MobileNet paper.
+        dropout: dropout rate
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor (i.e. output of
+            `layers.Input()`)
+            to use as image input for the model.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model
+                will be the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a
+                2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+        RuntimeError: If attempting to run this model with a
+            backend that does not support separable convolutions.
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top` '
+                         'as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) != 5:
+        print('Error: stride_size length must be exactly 5')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    # Determine proper input shape and default size.
+    if input_shape is None:
+        default_size = 224
+    else:
+        if backend.image_data_format() == 'channels_first':
+            rows = input_shape[1]
+            cols = input_shape[2]
+        else:
+            rows = input_shape[0]
+            cols = input_shape[1]
+
+        if rows == cols and rows in [128, 160, 192, 224]:
+            default_size = rows
+        else:
+            default_size = 224
+
+
+    if backend.image_data_format() == 'channels_last':
+        row_axis, col_axis = (0, 1)
+    else:
+        row_axis, col_axis = (1, 2)
+    rows = input_shape[row_axis]
+    cols = input_shape[col_axis]
+
+    if weights == 'imagenet':
+        if depth_multiplier != 1:
+            raise ValueError('If imagenet weights are being loaded, '
+                             'depth multiplier must be 1')
+
+        if alpha not in [0.25, 0.50, 0.75, 1.0]:
+            raise ValueError('If imagenet weights are being loaded, '
+                             'alpha can be one of'
+                             '`0.25`, `0.50`, `0.75` or `1.0` only.')
+
+        if rows != cols or rows not in [128, 160, 192, 224]:
+            rows = 224
+            warnings.warn('`input_shape` is undefined or non-square, '
+                          'or `rows` is not in [128, 160, 192, 224]. '
+                          'Weights for input shape (224, 224) will be'
+                          ' loaded as the default.')
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    x = _conv_block(img_input, 32, alpha, strides=stride_size[0])
+    x = _depthwise_conv_block(x, 64, alpha, depth_multiplier, block_id=1)
+
+    x = _depthwise_conv_block(x, 128, alpha, depth_multiplier, strides=stride_size[1], block_id=2)
+    x = _depthwise_conv_block(x, 128, alpha, depth_multiplier, block_id=3)
+
+    x = _depthwise_conv_block(x, 256, alpha, depth_multiplier, strides=stride_size[2], block_id=4)
+    x = _depthwise_conv_block(x, 256, alpha, depth_multiplier, block_id=5)
+
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, strides=stride_size[3], block_id=6)
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=7)
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=8)
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=9)
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=10)
+    x = _depthwise_conv_block(x, 512, alpha, depth_multiplier, block_id=11)
+
+    x = _depthwise_conv_block(x, 1024, alpha, depth_multiplier, strides=stride_size[4], block_id=12)
+    x = _depthwise_conv_block(x, 1024, alpha, depth_multiplier, block_id=13)
+
+    if include_top:
+        if backend.image_data_format() == 'channels_first':
+            shape = (int(1024 * alpha), 1, 1, 1)
+        else:
+            shape = (1, 1, 1, int(1024 * alpha))
+
+        x = layers.GlobalAveragePooling3D()(x)
+        x = layers.Reshape(shape, name='reshape_1')(x)
+        x = layers.Dropout(dropout, name='dropout')(x)
+        x = layers.Conv3D(classes, (1, 1, 1),
+                          padding='same',
+                          name='conv_preds')(x)
+        x = layers.Reshape((classes,), name='reshape_2')(x)
+        x = layers.Activation('softmax', name='act_softmax')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model = models.Model(inputs, x, name='mobilenet_%0.2f_%s' % (alpha, rows))
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, 'mobilenet', weights, classes, include_top, **kwargs)
+
+    return model
+
+
+def _conv_block(inputs, filters, alpha, kernel=(3, 3, 3), strides=(1, 1, 1)):
+    """Adds an initial convolution layer (with batch normalization and relu6).
+
+    # Arguments
+        inputs: Input tensor of shape `(rows, cols, 3)`
+            (with `channels_last` data format) or
+            (3, rows, cols) (with `channels_first` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 32.
+            E.g. `(224, 224, 3)` would be one valid value.
+        filters: Integer, the dimensionality of the output space
+            (i.e. the number of output filters in the convolution).
+        alpha: controls the width of the network.
+            - If `alpha` < 1.0, proportionally decreases the number
+                of filters in each layer.
+            - If `alpha` > 1.0, proportionally increases the number
+                of filters in each layer.
+            - If `alpha` = 1, default number of filters from the paper
+                 are used at each layer.
+        kernel: An integer or tuple/list of 2 integers, specifying the
+            width and height of the 2D convolution window.
+            Can be a single integer to specify the same value for
+            all spatial dimensions.
+        strides: An integer or tuple/list of 2 integers,
+            specifying the strides of the convolution
+            along the width and height.
+            Can be a single integer to specify the same value for
+            all spatial dimensions.
+            Specifying any stride value != 1 is incompatible with specifying
+            any `dilation_rate` value != 1.
+
+    # Input shape
+        4D tensor with shape:
+        `(samples, channels, rows, cols)` if data_format='channels_first'
+        or 4D tensor with shape:
+        `(samples, rows, cols, channels)` if data_format='channels_last'.
+
+    # Output shape
+        4D tensor with shape:
+        `(samples, filters, new_rows, new_cols)`
+        if data_format='channels_first'
+        or 4D tensor with shape:
+        `(samples, new_rows, new_cols, filters)`
+        if data_format='channels_last'.
+        `rows` and `cols` values might have changed due to stride.
+
+    # Returns
+        Output tensor of block.
+    """
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
+    filters = int(filters * alpha)
+    x = layers.ZeroPadding3D(padding=((0, 1), (0, 1), (0, 1)), name='conv1_pad')(inputs)
+    x = layers.Conv3D(filters, kernel,
+                      padding='valid',
+                      use_bias=False,
+                      strides=strides,
+                      name='conv1')(x)
+    x = layers.BatchNormalization(axis=channel_axis, name='conv1_bn')(x)
+    return layers.ReLU(6., name='conv1_relu')(x)
+
+
+def _depthwise_conv_block(inputs, pointwise_conv_filters, alpha,
+                          depth_multiplier=1, strides=(1, 1, 1), block_id=1):
+    """Adds a depthwise convolution block.
+
+    A depthwise convolution block consists of a depthwise conv,
+    batch normalization, relu6, pointwise convolution,
+    batch normalization and relu6 activation.
+
+    # Arguments
+        inputs: Input tensor of shape `(rows, cols, channels)`
+            (with `channels_last` data format) or
+            (channels, rows, cols) (with `channels_first` data format).
+        pointwise_conv_filters: Integer, the dimensionality of the output space
+            (i.e. the number of output filters in the pointwise convolution).
+        alpha: controls the width of the network.
+            - If `alpha` < 1.0, proportionally decreases the number
+                of filters in each layer.
+            - If `alpha` > 1.0, proportionally increases the number
+                of filters in each layer.
+            - If `alpha` = 1, default number of filters from the paper
+                 are used at each layer.
+        depth_multiplier: The number of depthwise convolution output channels
+            for each input channel.
+            The total number of depthwise convolution output
+            channels will be equal to `filters_in * depth_multiplier`.
+        strides: An integer or tuple/list of 2 integers,
+            specifying the strides of the convolution
+            along the width and height.
+            Can be a single integer to specify the same value for
+            all spatial dimensions.
+            Specifying any stride value != 1 is incompatible with specifying
+            any `dilation_rate` value != 1.
+        block_id: Integer, a unique identification designating
+            the block number.
+
+    # Input shape
+        4D tensor with shape:
+        `(batch, channels, rows, cols)` if data_format='channels_first'
+        or 4D tensor with shape:
+        `(batch, rows, cols, channels)` if data_format='channels_last'.
+
+    # Output shape
+        4D tensor with shape:
+        `(batch, filters, new_rows, new_cols)`
+        if data_format='channels_first'
+        or 4D tensor with shape:
+        `(batch, new_rows, new_cols, filters)`
+        if data_format='channels_last'.
+        `rows` and `cols` values might have changed due to stride.
+
+    # Returns
+        Output tensor of block.
+    """
+    from ..models._DepthwiseConv3D import DepthwiseConv3D
+
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
+    pointwise_conv_filters = int(pointwise_conv_filters * alpha)
+
+    if strides == (1, 1, 1):
+        x = inputs
+    else:
+        x = layers.ZeroPadding3D(((0, 1), (0, 1), (0, 1)),
+                                 name='conv_pad_%d' % block_id)(inputs)
+    x = DepthwiseConv3D((3, 3, 3),
+                               padding='same' if strides == (1, 1, 1) else 'valid',
+                               depth_multiplier=depth_multiplier,
+                               strides=strides,
+                               use_bias=False,
+                               name='conv_dw_%d' % block_id)(x)
+    x = layers.BatchNormalization(
+        axis=channel_axis, name='conv_dw_%d_bn' % block_id)(x)
+    x = layers.ReLU(6., name='conv_dw_%d_relu' % block_id)(x)
+
+    x = layers.Conv3D(pointwise_conv_filters, (1, 1, 1),
+                      padding='same',
+                      use_bias=False,
+                      strides=(1, 1, 1),
+                      name='conv_pw_%d' % block_id)(x)
+    x = layers.BatchNormalization(axis=channel_axis,
+                                  name='conv_pw_%d_bn' % block_id)(x)
+    return layers.ReLU(6., name='conv_pw_%d_relu' % block_id)(x)
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/mobilenet_v2.py` & `classification_models_3D-1.1.0/classification_models_3D/models/mobilenet_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,515 +1,516 @@
-"""MobileNet v2 models for Keras.
-
-MobileNetV2 is a general architecture and can be used for multiple use cases.
-Depending on the use case, it can use different input layer size and
-different width factors. This allows different width models to reduce
-the number of multiply-adds and thereby
-reduce inference cost on mobile devices.
-
-MobileNetV2 is very similar to the original MobileNet,
-except that it uses inverted residual blocks with
-bottlenecking features. It has a drastically lower
-parameter count than the original MobileNet.
-MobileNets support any input size greater
-than 32 x 32, with larger image sizes
-offering better performance.
-
-The number of parameters and number of multiply-adds
-can be modified by using the `alpha` parameter,
-which increases/decreases the number of filters in each layer.
-By altering the image size and `alpha` parameter,
-all 22 models from the paper can be built, with ImageNet weights provided.
-
-The paper demonstrates the performance of MobileNets using `alpha` values of
-1.0 (also called 100 % MobileNet), 0.35, 0.5, 0.75, 1.0, 1.3, and 1.4
-
-For each of these `alpha` values, weights for 5 different input image sizes
-are provided (224, 192, 160, 128, and 96).
-
-
-The following table describes the performance of
-MobileNet on various input sizes:
-------------------------------------------------------------------------
-MACs stands for Multiply Adds
-
- Classification Checkpoint| MACs (M) | Parameters (M)| Top 1 Accuracy| Top 5 Accuracy
---------------------------|------------|---------------|---------|----|-------------
-| [mobilenet_v2_1.4_224]  | 582 | 6.06 |          75.0 | 92.5 |
-| [mobilenet_v2_1.3_224]  | 509 | 5.34 |          74.4 | 92.1 |
-| [mobilenet_v2_1.0_224]  | 300 | 3.47 |          71.8 | 91.0 |
-| [mobilenet_v2_1.0_192]  | 221 | 3.47 |          70.7 | 90.1 |
-| [mobilenet_v2_1.0_160]  | 154 | 3.47 |          68.8 | 89.0 |
-| [mobilenet_v2_1.0_128]  | 99  | 3.47 |          65.3 | 86.9 |
-| [mobilenet_v2_1.0_96]   | 56  | 3.47 |          60.3 | 83.2 |
-| [mobilenet_v2_0.75_224] | 209 | 2.61 |          69.8 | 89.6 |
-| [mobilenet_v2_0.75_192] | 153 | 2.61 |          68.7 | 88.9 |
-| [mobilenet_v2_0.75_160] | 107 | 2.61 |          66.4 | 87.3 |
-| [mobilenet_v2_0.75_128] | 69  | 2.61 |          63.2 | 85.3 |
-| [mobilenet_v2_0.75_96]  | 39  | 2.61 |          58.8 | 81.6 |
-| [mobilenet_v2_0.5_224]  | 97  | 1.95 |          65.4 | 86.4 |
-| [mobilenet_v2_0.5_192]  | 71  | 1.95 |          63.9 | 85.4 |
-| [mobilenet_v2_0.5_160]  | 50  | 1.95 |          61.0 | 83.2 |
-| [mobilenet_v2_0.5_128]  | 32  | 1.95 |          57.7 | 80.8 |
-| [mobilenet_v2_0.5_96]   | 18  | 1.95 |          51.2 | 75.8 |
-| [mobilenet_v2_0.35_224] | 59  | 1.66 |          60.3 | 82.9 |
-| [mobilenet_v2_0.35_192] | 43  | 1.66 |          58.2 | 81.2 |
-| [mobilenet_v2_0.35_160] | 30  | 1.66 |          55.7 | 79.1 |
-| [mobilenet_v2_0.35_128] | 20  | 1.66 |          50.8 | 75.0 |
-| [mobilenet_v2_0.35_96]  | 11  | 1.66 |          45.5 | 70.4 |
-
-The weights for all 16 models are obtained and
-translated from the Tensorflow checkpoints
-from TensorFlow checkpoints found [here]
-(https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet/README.md).
-
-# Reference
-
-This file contains building code for MobileNetV2, based on
-[MobileNetV2: Inverted Residuals and Linear Bottlenecks]
-(https://arxiv.org/abs/1801.04381) (CVPR 2018)
-
-Tests comparing this model to the existing Tensorflow model can be
-found at [mobilenet_v2_keras]
-(https://github.com/JonathanCMitchell/mobilenet_v2_keras)
-"""
-from __future__ import print_function
-from __future__ import absolute_import
-from __future__ import division
-
-import os
-import warnings
-from .. import get_submodules_from_kwargs
-from ..weights import load_model_weights
-from keras_applications import imagenet_utils
-
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-def preprocess_input(x, **kwargs):
-    """Preprocesses a numpy array encoding a batch of images.
-
-    # Arguments
-        x: a 4D numpy array consists of RGB values within [0, 255].
-
-    # Returns
-        Preprocessed array.
-    """
-    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
-
-
-# This function is taken from the original tf repo.
-# It ensures that all layers have a channel number that is divisible by 8
-# It can be seen here:
-# https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet/mobilenet.py
-
-
-def _make_divisible(v, divisor, min_value=None):
-    if min_value is None:
-        min_value = divisor
-    new_v = max(min_value, int(v + divisor / 2) // divisor * divisor)
-    # Make sure that round down does not go down by more than 10%.
-    if new_v < 0.9 * v:
-        new_v += divisor
-    return new_v
-
-
-def correct_pad(backend, inputs, kernel_size):
-    """Returns a tuple for zero-padding for 3D convolution with downsampling.
-
-    # Arguments
-        input_size: An integer or tuple/list of 3 integers.
-        kernel_size: An integer or tuple/list of 3 integers.
-
-    # Returns
-        A tuple.
-    """
-
-    img_dim = 2 if backend.image_data_format() == 'channels_first' else 1
-    input_size = backend.int_shape(inputs)[img_dim:(img_dim + 3)]
-
-    if isinstance(kernel_size, int):
-        kernel_size = (kernel_size, kernel_size, kernel_size)
-
-    if input_size[0] is None:
-        adjust = (1, 1, 1)
-    else:
-        adjust = (1 - input_size[0] % 2, 1 - input_size[1] % 2, 1 - input_size[2] % 2)
-
-    correct = (kernel_size[0] // 2, kernel_size[1] // 2, kernel_size[2] // 2)
-
-    ret = (
-        (correct[0] - adjust[0], correct[0]),
-        (correct[1] - adjust[1], correct[1]),
-        (correct[2] - adjust[2], correct[2])
-    )
-
-    return ret
-
-
-def MobileNetV2(
-        input_shape=None,
-        alpha=1.0,
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        **kwargs
-):
-    """Instantiates the MobileNetV2 architecture.
-
-    # Arguments
-        input_shape: optional shape tuple, to be specified if you would
-            like to use a model with an input img resolution that is not
-            (224, 224, 3).
-            It should have exactly 3 inputs channels (224, 224, 3).
-            You can also omit this option if you would like
-            to infer input_shape from an input_tensor.
-            If you choose to include both input_tensor and input_shape then
-            input_shape will be used if they match, if the shapes
-            do not match then we will throw an error.
-            E.g. `(160, 160, 3)` would be one valid value.
-        alpha: controls the width of the network. This is known as the
-        width multiplier in the MobileNetV2 paper, but the name is kept for
-        consistency with MobileNetV1 in Keras.
-            - If `alpha` < 1.0, proportionally decreases the number
-                of filters in each layer.
-            - If `alpha` > 1.0, proportionally increases the number
-                of filters in each layer.
-            - If `alpha` = 1, default number of filters from the paper
-                 are used at each layer.
-        include_top: whether to include the fully-connected
-            layer at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor (i.e. output of
-            `layers.Input()`)
-            to use as image input for the model.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model
-                will be the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a
-                2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape or invalid alpha, rows when
-            weights='imagenet'
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top` '
-                         'as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) != 5:
-        print('Error: stride_size length must be exactly 5')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    # Determine proper input shape and default size.
-    # If both input_shape and input_tensor are used, they should match
-    if input_shape is not None and input_tensor is not None:
-        try:
-            is_input_t_tensor = backend.is_keras_tensor(input_tensor)
-        except ValueError:
-            try:
-                is_input_t_tensor = backend.is_keras_tensor(
-                    keras_utils.get_source_inputs(input_tensor))
-            except ValueError:
-                raise ValueError('input_tensor: ', input_tensor,
-                                 'is not type input_tensor')
-        if is_input_t_tensor:
-            if backend.image_data_format == 'channels_first':
-                if backend.int_shape(input_tensor)[1] != input_shape[1]:
-                    raise ValueError('input_shape: ', input_shape,
-                                     'and input_tensor: ', input_tensor,
-                                     'do not meet the same shape requirements')
-            else:
-                if backend.int_shape(input_tensor)[2] != input_shape[1]:
-                    raise ValueError('input_shape: ', input_shape,
-                                     'and input_tensor: ', input_tensor,
-                                     'do not meet the same shape requirements')
-        else:
-            raise ValueError('input_tensor specified: ', input_tensor,
-                             'is not a keras tensor')
-
-    # If input_shape is None, infer shape from input_tensor
-    if input_shape is None and input_tensor is not None:
-
-        try:
-            backend.is_keras_tensor(input_tensor)
-        except ValueError:
-            raise ValueError('input_tensor: ', input_tensor,
-                             'is type: ', type(input_tensor),
-                             'which is not a valid type')
-
-        if input_shape is None and not backend.is_keras_tensor(input_tensor):
-            default_size = 224
-        elif input_shape is None and backend.is_keras_tensor(input_tensor):
-            if backend.image_data_format() == 'channels_first':
-                rows = backend.int_shape(input_tensor)[2]
-                cols = backend.int_shape(input_tensor)[3]
-            else:
-                rows = backend.int_shape(input_tensor)[1]
-                cols = backend.int_shape(input_tensor)[2]
-
-            if rows == cols and rows in [96, 128, 160, 192, 224]:
-                default_size = rows
-            else:
-                default_size = 224
-
-    # If input_shape is None and no input_tensor
-    elif input_shape is None:
-        default_size = 224
-
-    # If input_shape is not None, assume default size
-    else:
-        if backend.image_data_format() == 'channels_first':
-            rows = input_shape[1]
-            cols = input_shape[2]
-        else:
-            rows = input_shape[0]
-            cols = input_shape[1]
-
-        if rows == cols and rows in [96, 128, 160, 192, 224]:
-            default_size = rows
-        else:
-            default_size = 224
-
-    if backend.image_data_format() == 'channels_last':
-        row_axis, col_axis = (0, 1)
-    else:
-        row_axis, col_axis = (1, 2)
-    rows = input_shape[row_axis]
-    cols = input_shape[col_axis]
-
-    if weights == 'imagenet':
-        if alpha not in [0.35, 0.50, 0.75, 1.0, 1.3, 1.4]:
-            raise ValueError('If imagenet weights are being loaded, '
-                             'alpha can be one of `0.35`, `0.50`, `0.75`, '
-                             '`1.0`, `1.3` or `1.4` only.')
-
-        if rows != cols or rows not in [96, 128, 160, 192, 224]:
-            rows = 224
-            warnings.warn('`input_shape` is undefined or non-square, '
-                          'or `rows` is not in [96, 128, 160, 192, 224].'
-                          ' Weights for input shape (224, 224) will be'
-                          ' loaded as the default.')
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
-
-    first_block_filters = _make_divisible(32 * alpha, 8)
-    x = layers.ZeroPadding3D(padding=correct_pad(backend, img_input, 3),
-                             name='Conv1_pad')(img_input)
-    x = layers.Conv3D(first_block_filters,
-                      kernel_size=3,
-                      strides=stride_size[0],
-                      padding='valid',
-                      use_bias=False,
-                      name='Conv1')(x)
-    x = layers.BatchNormalization(axis=channel_axis,
-                                  epsilon=1e-3,
-                                  momentum=0.999,
-                                  name='bn_Conv1')(x)
-    x = layers.ReLU(6., name='Conv1_relu')(x)
-
-    x = _inverted_res_block(x, filters=16, alpha=alpha, stride=1,
-                            expansion=1, block_id=0)
-
-    x = _inverted_res_block(x, filters=24, alpha=alpha, stride=stride_size[1],
-                            expansion=6, block_id=1)
-    x = _inverted_res_block(x, filters=24, alpha=alpha, stride=1,
-                            expansion=6, block_id=2)
-
-    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=stride_size[2],
-                            expansion=6, block_id=3)
-    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=1,
-                            expansion=6, block_id=4)
-    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=1,
-                            expansion=6, block_id=5)
-
-    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=stride_size[3],
-                            expansion=6, block_id=6)
-    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
-                            expansion=6, block_id=7)
-    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
-                            expansion=6, block_id=8)
-    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
-                            expansion=6, block_id=9)
-
-    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
-                            expansion=6, block_id=10)
-    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
-                            expansion=6, block_id=11)
-    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
-                            expansion=6, block_id=12)
-
-    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=stride_size[4],
-                            expansion=6, block_id=13)
-    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=1,
-                            expansion=6, block_id=14)
-    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=1,
-                            expansion=6, block_id=15)
-
-    x = _inverted_res_block(x, filters=320, alpha=alpha, stride=1,
-                            expansion=6, block_id=16)
-
-    # no alpha applied to last conv as stated in the paper:
-    # if the width multiplier is greater than 1 we
-    # increase the number of output channels
-    if alpha > 1.0:
-        last_block_filters = _make_divisible(1280 * alpha, 8)
-    else:
-        last_block_filters = 1280
-
-    x = layers.Conv3D(last_block_filters,
-                      kernel_size=1,
-                      use_bias=False,
-                      name='Conv_1')(x)
-    x = layers.BatchNormalization(axis=channel_axis,
-                                  epsilon=1e-3,
-                                  momentum=0.999,
-                                  name='Conv_1_bn')(x)
-    x = layers.ReLU(6., name='out_relu')(x)
-
-    if include_top:
-        x = layers.GlobalAveragePooling3D()(x)
-        x = layers.Dense(classes, activation='softmax',
-                         use_bias=True, name='Logits')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-
-    # Create model.
-    model = models.Model(inputs, x,
-                         name='mobilenetv2_%0.2f_%s' % (alpha, rows))
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, 'mobilenetv2', weights, classes, include_top, **kwargs)
-
-    return model
-
-
-def _inverted_res_block(inputs, expansion, stride, alpha, filters, block_id):
-    from ..models._DepthwiseConv3D import DepthwiseConv3D
-
-    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
-
-    in_channels = backend.int_shape(inputs)[channel_axis]
-    pointwise_conv_filters = int(filters * alpha)
-    pointwise_filters = _make_divisible(pointwise_conv_filters, 8)
-    x = inputs
-    prefix = 'block_{}_'.format(block_id)
-
-    if block_id:
-        # Expand
-        x = layers.Conv3D(expansion * in_channels,
-                          kernel_size=1,
-                          padding='same',
-                          use_bias=False,
-                          activation=None,
-                          name=prefix + 'expand')(x)
-        x = layers.BatchNormalization(axis=channel_axis,
-                                      epsilon=1e-3,
-                                      momentum=0.999,
-                                      name=prefix + 'expand_BN')(x)
-        x = layers.ReLU(6., name=prefix + 'expand_relu')(x)
-    else:
-        prefix = 'expanded_conv_'
-
-    # Depthwise
-    if stride == 2 or stride == (2, 2, 2):
-        pd = correct_pad(backend, x, 3)
-        x = layers.ZeroPadding3D(padding=pd, name=prefix + 'pad')(x)
-    x = DepthwiseConv3D(kernel_size=3,
-                               strides=stride,
-                               activation=None,
-                               use_bias=False,
-                               padding='same' if stride == 1 else 'valid',
-                               name=prefix + 'depthwise')(x)
-    x = layers.BatchNormalization(axis=channel_axis,
-                                  epsilon=1e-3,
-                                  momentum=0.999,
-                                  name=prefix + 'depthwise_BN')(x)
-
-    x = layers.ReLU(6., name=prefix + 'depthwise_relu')(x)
-
-    # Project
-    x = layers.Conv3D(pointwise_filters,
-                      kernel_size=1,
-                      padding='same',
-                      use_bias=False,
-                      activation=None,
-                      name=prefix + 'project')(x)
-    x = layers.BatchNormalization(axis=channel_axis,
-                                  epsilon=1e-3,
-                                  momentum=0.999,
-                                  name=prefix + 'project_BN')(x)
-
-    if in_channels == pointwise_filters and stride == 1:
-        return layers.Add(name=prefix + 'add')([inputs, x])
-    return x
+"""MobileNet v2 models for Keras.
+
+MobileNetV2 is a general architecture and can be used for multiple use cases.
+Depending on the use case, it can use different input layer size and
+different width factors. This allows different width models to reduce
+the number of multiply-adds and thereby
+reduce inference cost on mobile devices.
+
+MobileNetV2 is very similar to the original MobileNet,
+except that it uses inverted residual blocks with
+bottlenecking features. It has a drastically lower
+parameter count than the original MobileNet.
+MobileNets support any input size greater
+than 32 x 32, with larger image sizes
+offering better performance.
+
+The number of parameters and number of multiply-adds
+can be modified by using the `alpha` parameter,
+which increases/decreases the number of filters in each layer.
+By altering the image size and `alpha` parameter,
+all 22 models from the paper can be built, with ImageNet weights provided.
+
+The paper demonstrates the performance of MobileNets using `alpha` values of
+1.0 (also called 100 % MobileNet), 0.35, 0.5, 0.75, 1.0, 1.3, and 1.4
+
+For each of these `alpha` values, weights for 5 different input image sizes
+are provided (224, 192, 160, 128, and 96).
+
+
+The following table describes the performance of
+MobileNet on various input sizes:
+------------------------------------------------------------------------
+MACs stands for Multiply Adds
+
+ Classification Checkpoint| MACs (M) | Parameters (M)| Top 1 Accuracy| Top 5 Accuracy
+--------------------------|------------|---------------|---------|----|-------------
+| [mobilenet_v2_1.4_224]  | 582 | 6.06 |          75.0 | 92.5 |
+| [mobilenet_v2_1.3_224]  | 509 | 5.34 |          74.4 | 92.1 |
+| [mobilenet_v2_1.0_224]  | 300 | 3.47 |          71.8 | 91.0 |
+| [mobilenet_v2_1.0_192]  | 221 | 3.47 |          70.7 | 90.1 |
+| [mobilenet_v2_1.0_160]  | 154 | 3.47 |          68.8 | 89.0 |
+| [mobilenet_v2_1.0_128]  | 99  | 3.47 |          65.3 | 86.9 |
+| [mobilenet_v2_1.0_96]   | 56  | 3.47 |          60.3 | 83.2 |
+| [mobilenet_v2_0.75_224] | 209 | 2.61 |          69.8 | 89.6 |
+| [mobilenet_v2_0.75_192] | 153 | 2.61 |          68.7 | 88.9 |
+| [mobilenet_v2_0.75_160] | 107 | 2.61 |          66.4 | 87.3 |
+| [mobilenet_v2_0.75_128] | 69  | 2.61 |          63.2 | 85.3 |
+| [mobilenet_v2_0.75_96]  | 39  | 2.61 |          58.8 | 81.6 |
+| [mobilenet_v2_0.5_224]  | 97  | 1.95 |          65.4 | 86.4 |
+| [mobilenet_v2_0.5_192]  | 71  | 1.95 |          63.9 | 85.4 |
+| [mobilenet_v2_0.5_160]  | 50  | 1.95 |          61.0 | 83.2 |
+| [mobilenet_v2_0.5_128]  | 32  | 1.95 |          57.7 | 80.8 |
+| [mobilenet_v2_0.5_96]   | 18  | 1.95 |          51.2 | 75.8 |
+| [mobilenet_v2_0.35_224] | 59  | 1.66 |          60.3 | 82.9 |
+| [mobilenet_v2_0.35_192] | 43  | 1.66 |          58.2 | 81.2 |
+| [mobilenet_v2_0.35_160] | 30  | 1.66 |          55.7 | 79.1 |
+| [mobilenet_v2_0.35_128] | 20  | 1.66 |          50.8 | 75.0 |
+| [mobilenet_v2_0.35_96]  | 11  | 1.66 |          45.5 | 70.4 |
+
+The weights for all 16 models are obtained and
+translated from the Tensorflow checkpoints
+from TensorFlow checkpoints found [here]
+(https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet/README.md).
+
+# Reference
+
+This file contains building code for MobileNetV2, based on
+[MobileNetV2: Inverted Residuals and Linear Bottlenecks]
+(https://arxiv.org/abs/1801.04381) (CVPR 2018)
+
+Tests comparing this model to the existing Tensorflow model can be
+found at [mobilenet_v2_keras]
+(https://github.com/JonathanCMitchell/mobilenet_v2_keras)
+"""
+from __future__ import print_function
+from __future__ import absolute_import
+from __future__ import division
+
+import os
+import warnings
+from .. import get_submodules_from_kwargs
+from ..weights import load_model_weights
+from keras.applications import imagenet_utils
+from keras.src.legacy.backend import int_shape
+
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+def preprocess_input(x, **kwargs):
+    """Preprocesses a numpy array encoding a batch of images.
+
+    # Arguments
+        x: a 4D numpy array consists of RGB values within [0, 255].
+
+    # Returns
+        Preprocessed array.
+    """
+    return imagenet_utils.preprocess_input(x, mode='tf', **kwargs)
+
+
+# This function is taken from the original tf repo.
+# It ensures that all layers have a channel number that is divisible by 8
+# It can be seen here:
+# https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet/mobilenet.py
+
+
+def _make_divisible(v, divisor, min_value=None):
+    if min_value is None:
+        min_value = divisor
+    new_v = max(min_value, int(v + divisor / 2) // divisor * divisor)
+    # Make sure that round down does not go down by more than 10%.
+    if new_v < 0.9 * v:
+        new_v += divisor
+    return new_v
+
+
+def correct_pad(backend, inputs, kernel_size):
+    """Returns a tuple for zero-padding for 3D convolution with downsampling.
+
+    # Arguments
+        input_size: An integer or tuple/list of 3 integers.
+        kernel_size: An integer or tuple/list of 3 integers.
+
+    # Returns
+        A tuple.
+    """
+
+    img_dim = 2 if backend.image_data_format() == 'channels_first' else 1
+    input_size = int_shape(inputs)[img_dim:(img_dim + 3)]
+
+    if isinstance(kernel_size, int):
+        kernel_size = (kernel_size, kernel_size, kernel_size)
+
+    if input_size[0] is None:
+        adjust = (1, 1, 1)
+    else:
+        adjust = (1 - input_size[0] % 2, 1 - input_size[1] % 2, 1 - input_size[2] % 2)
+
+    correct = (kernel_size[0] // 2, kernel_size[1] // 2, kernel_size[2] // 2)
+
+    ret = (
+        (correct[0] - adjust[0], correct[0]),
+        (correct[1] - adjust[1], correct[1]),
+        (correct[2] - adjust[2], correct[2])
+    )
+
+    return ret
+
+
+def MobileNetV2(
+        input_shape=None,
+        alpha=1.0,
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        **kwargs
+):
+    """Instantiates the MobileNetV2 architecture.
+
+    # Arguments
+        input_shape: optional shape tuple, to be specified if you would
+            like to use a model with an input img resolution that is not
+            (224, 224, 3).
+            It should have exactly 3 inputs channels (224, 224, 3).
+            You can also omit this option if you would like
+            to infer input_shape from an input_tensor.
+            If you choose to include both input_tensor and input_shape then
+            input_shape will be used if they match, if the shapes
+            do not match then we will throw an error.
+            E.g. `(160, 160, 3)` would be one valid value.
+        alpha: controls the width of the network. This is known as the
+        width multiplier in the MobileNetV2 paper, but the name is kept for
+        consistency with MobileNetV1 in Keras.
+            - If `alpha` < 1.0, proportionally decreases the number
+                of filters in each layer.
+            - If `alpha` > 1.0, proportionally increases the number
+                of filters in each layer.
+            - If `alpha` = 1, default number of filters from the paper
+                 are used at each layer.
+        include_top: whether to include the fully-connected
+            layer at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor (i.e. output of
+            `layers.Input()`)
+            to use as image input for the model.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model
+                will be the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a
+                2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape or invalid alpha, rows when
+            weights='imagenet'
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top` '
+                         'as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) != 5:
+        print('Error: stride_size length must be exactly 5')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    # Determine proper input shape and default size.
+    # If both input_shape and input_tensor are used, they should match
+    if input_shape is not None and input_tensor is not None:
+        try:
+            is_input_t_tensor = backend.is_keras_tensor(input_tensor)
+        except ValueError:
+            try:
+                is_input_t_tensor = backend.is_keras_tensor(
+                    keras_utils.get_source_inputs(input_tensor))
+            except ValueError:
+                raise ValueError('input_tensor: ', input_tensor,
+                                 'is not type input_tensor')
+        if is_input_t_tensor:
+            if backend.image_data_format == 'channels_first':
+                if int_shape(input_tensor)[1] != input_shape[1]:
+                    raise ValueError('input_shape: ', input_shape,
+                                     'and input_tensor: ', input_tensor,
+                                     'do not meet the same shape requirements')
+            else:
+                if int_shape(input_tensor)[2] != input_shape[1]:
+                    raise ValueError('input_shape: ', input_shape,
+                                     'and input_tensor: ', input_tensor,
+                                     'do not meet the same shape requirements')
+        else:
+            raise ValueError('input_tensor specified: ', input_tensor,
+                             'is not a keras tensor')
+
+    # If input_shape is None, infer shape from input_tensor
+    if input_shape is None and input_tensor is not None:
+
+        try:
+            backend.is_keras_tensor(input_tensor)
+        except ValueError:
+            raise ValueError('input_tensor: ', input_tensor,
+                             'is type: ', type(input_tensor),
+                             'which is not a valid type')
+
+        if input_shape is None and not backend.is_keras_tensor(input_tensor):
+            default_size = 224
+        elif input_shape is None and backend.is_keras_tensor(input_tensor):
+            if backend.image_data_format() == 'channels_first':
+                rows = int_shape(input_tensor)[2]
+                cols = int_shape(input_tensor)[3]
+            else:
+                rows = int_shape(input_tensor)[1]
+                cols = int_shape(input_tensor)[2]
+
+            if rows == cols and rows in [96, 128, 160, 192, 224]:
+                default_size = rows
+            else:
+                default_size = 224
+
+    # If input_shape is None and no input_tensor
+    elif input_shape is None:
+        default_size = 224
+
+    # If input_shape is not None, assume default size
+    else:
+        if backend.image_data_format() == 'channels_first':
+            rows = input_shape[1]
+            cols = input_shape[2]
+        else:
+            rows = input_shape[0]
+            cols = input_shape[1]
+
+        if rows == cols and rows in [96, 128, 160, 192, 224]:
+            default_size = rows
+        else:
+            default_size = 224
+
+    if backend.image_data_format() == 'channels_last':
+        row_axis, col_axis = (0, 1)
+    else:
+        row_axis, col_axis = (1, 2)
+    rows = input_shape[row_axis]
+    cols = input_shape[col_axis]
+
+    if weights == 'imagenet':
+        if alpha not in [0.35, 0.50, 0.75, 1.0, 1.3, 1.4]:
+            raise ValueError('If imagenet weights are being loaded, '
+                             'alpha can be one of `0.35`, `0.50`, `0.75`, '
+                             '`1.0`, `1.3` or `1.4` only.')
+
+        if rows != cols or rows not in [96, 128, 160, 192, 224]:
+            rows = 224
+            warnings.warn('`input_shape` is undefined or non-square, '
+                          'or `rows` is not in [96, 128, 160, 192, 224].'
+                          ' Weights for input shape (224, 224) will be'
+                          ' loaded as the default.')
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
+
+    first_block_filters = _make_divisible(32 * alpha, 8)
+    x = layers.ZeroPadding3D(padding=correct_pad(backend, img_input, 3),
+                             name='Conv1_pad')(img_input)
+    x = layers.Conv3D(first_block_filters,
+                      kernel_size=3,
+                      strides=stride_size[0],
+                      padding='valid',
+                      use_bias=False,
+                      name='Conv1')(x)
+    x = layers.BatchNormalization(axis=channel_axis,
+                                  epsilon=1e-3,
+                                  momentum=0.999,
+                                  name='bn_Conv1')(x)
+    x = layers.ReLU(6., name='Conv1_relu')(x)
+
+    x = _inverted_res_block(x, filters=16, alpha=alpha, stride=1,
+                            expansion=1, block_id=0)
+
+    x = _inverted_res_block(x, filters=24, alpha=alpha, stride=stride_size[1],
+                            expansion=6, block_id=1)
+    x = _inverted_res_block(x, filters=24, alpha=alpha, stride=1,
+                            expansion=6, block_id=2)
+
+    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=stride_size[2],
+                            expansion=6, block_id=3)
+    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=1,
+                            expansion=6, block_id=4)
+    x = _inverted_res_block(x, filters=32, alpha=alpha, stride=1,
+                            expansion=6, block_id=5)
+
+    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=stride_size[3],
+                            expansion=6, block_id=6)
+    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
+                            expansion=6, block_id=7)
+    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
+                            expansion=6, block_id=8)
+    x = _inverted_res_block(x, filters=64, alpha=alpha, stride=1,
+                            expansion=6, block_id=9)
+
+    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
+                            expansion=6, block_id=10)
+    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
+                            expansion=6, block_id=11)
+    x = _inverted_res_block(x, filters=96, alpha=alpha, stride=1,
+                            expansion=6, block_id=12)
+
+    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=stride_size[4],
+                            expansion=6, block_id=13)
+    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=1,
+                            expansion=6, block_id=14)
+    x = _inverted_res_block(x, filters=160, alpha=alpha, stride=1,
+                            expansion=6, block_id=15)
+
+    x = _inverted_res_block(x, filters=320, alpha=alpha, stride=1,
+                            expansion=6, block_id=16)
+
+    # no alpha applied to last conv as stated in the paper:
+    # if the width multiplier is greater than 1 we
+    # increase the number of output channels
+    if alpha > 1.0:
+        last_block_filters = _make_divisible(1280 * alpha, 8)
+    else:
+        last_block_filters = 1280
+
+    x = layers.Conv3D(last_block_filters,
+                      kernel_size=1,
+                      use_bias=False,
+                      name='Conv_1')(x)
+    x = layers.BatchNormalization(axis=channel_axis,
+                                  epsilon=1e-3,
+                                  momentum=0.999,
+                                  name='Conv_1_bn')(x)
+    x = layers.ReLU(6., name='out_relu')(x)
+
+    if include_top:
+        x = layers.GlobalAveragePooling3D()(x)
+        x = layers.Dense(classes, activation='softmax',
+                         use_bias=True, name='Logits')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+
+    # Create model.
+    model = models.Model(inputs, x,
+                         name='mobilenetv2_%0.2f_%s' % (alpha, rows))
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, 'mobilenetv2', weights, classes, include_top, **kwargs)
+
+    return model
+
+
+def _inverted_res_block(inputs, expansion, stride, alpha, filters, block_id):
+    from ..models._DepthwiseConv3D import DepthwiseConv3D
+
+    channel_axis = 1 if backend.image_data_format() == 'channels_first' else -1
+
+    in_channels = int_shape(inputs)[channel_axis]
+    pointwise_conv_filters = int(filters * alpha)
+    pointwise_filters = _make_divisible(pointwise_conv_filters, 8)
+    x = inputs
+    prefix = 'block_{}_'.format(block_id)
+
+    if block_id:
+        # Expand
+        x = layers.Conv3D(expansion * in_channels,
+                          kernel_size=1,
+                          padding='same',
+                          use_bias=False,
+                          activation=None,
+                          name=prefix + 'expand')(x)
+        x = layers.BatchNormalization(axis=channel_axis,
+                                      epsilon=1e-3,
+                                      momentum=0.999,
+                                      name=prefix + 'expand_BN')(x)
+        x = layers.ReLU(6., name=prefix + 'expand_relu')(x)
+    else:
+        prefix = 'expanded_conv_'
+
+    # Depthwise
+    if stride == 2 or stride == (2, 2, 2):
+        pd = correct_pad(backend, x, 3)
+        x = layers.ZeroPadding3D(padding=pd, name=prefix + 'pad')(x)
+    x = DepthwiseConv3D(kernel_size=3,
+                               strides=stride,
+                               activation=None,
+                               use_bias=False,
+                               padding='same' if stride == 1 else 'valid',
+                               name=prefix + 'depthwise')(x)
+    x = layers.BatchNormalization(axis=channel_axis,
+                                  epsilon=1e-3,
+                                  momentum=0.999,
+                                  name=prefix + 'depthwise_BN')(x)
+
+    x = layers.ReLU(6., name=prefix + 'depthwise_relu')(x)
+
+    # Project
+    x = layers.Conv3D(pointwise_filters,
+                      kernel_size=1,
+                      padding='same',
+                      use_bias=False,
+                      activation=None,
+                      name=prefix + 'project')(x)
+    x = layers.BatchNormalization(axis=channel_axis,
+                                  epsilon=1e-3,
+                                  momentum=0.999,
+                                  name=prefix + 'project_BN')(x)
+
+    if in_channels == pointwise_filters and stride == 1:
+        return layers.Add(name=prefix + 'add')([inputs, x])
+    return x
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/resnet.py` & `classification_models_3D-1.1.0/classification_models_3D/models/resnet.py`

 * *Files identical despite different names*

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/resnext.py` & `classification_models_3D-1.1.0/classification_models_3D/models/resnext.py`

 * *Files identical despite different names*

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/vgg16.py` & `classification_models_3D-1.1.0/classification_models_3D/models/vgg19.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-"""VGG16 model for Keras.
-
-# Reference
-
-- [Very Deep Convolutional Networks for Large-Scale Image Recognition](
-    https://arxiv.org/abs/1409.1556) (ICLR 2015)
-
-"""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from .. import get_submodules_from_kwargs
-from keras_applications import imagenet_utils
-from ..weights import load_model_weights
-
-
-preprocess_input = imagenet_utils.preprocess_input
-
-
-def VGG16(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        init_filters=64,
-        max_filters=512,
-        repetitions=(2, 2, 3, 3, 3),
-        **kwargs
-):
-    """Instantiates the VGG16 architecture.
-
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    # Arguments
-        include_top: whether to include the 3 fully-connected
-            layers at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor
-            (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(224, 224, 3)`
-            (with `channels_last` data format)
-            or `(3, 224, 224)` (with `channels_first` data format).
-            It should have exactly 3 input channels,
-            and width and height should be no smaller than 32.
-            E.g. `(200, 200, 3)` would be one valid value.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a 2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) < 3:
-        print('Error: stride_size length must be 3 or more')
-        return None
-
-    if len(stride_size) != len(repetitions):
-        print('Error: stride_size length must be equal to repetitions length - 1')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    x = img_input
-    for stage, rep in enumerate(repetitions):
-        for i in range(rep):
-            x = layers.Conv3D(
-                init_filters,
-                (3, 3, 3),
-                activation='relu',
-                padding='same',
-                name='block{}_conv{}'.format(stage + 1, i + 1)
-            )(x)
-
-        x = layers.MaxPooling3D(
-            stride_size[stage],
-            strides=stride_size[stage],
-            name='block{}_pool'.format(stage + 1)
-        )(x)
-
-        init_filters *= 2
-        if init_filters > max_filters:
-            init_filters = max_filters
-
-    if include_top:
-        # Classification block
-        x = layers.Flatten(name='flatten')(x)
-        x = layers.Dense(4096, activation='relu', name='fc1')(x)
-        x = layers.Dense(4096, activation='relu', name='fc2')(x)
-        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-    # Create model.
-    model = models.Model(inputs, x, name='vgg16')
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, 'vgg16', weights, classes, include_top, **kwargs)
-
-    return model
+"""VGG19 model for Keras.
+
+# Reference
+
+- [Very Deep Convolutional Networks for Large-Scale Image Recognition](
+    https://arxiv.org/abs/1409.1556) (ICLR 2015)
+
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import os
+from .. import get_submodules_from_kwargs
+from keras.applications import imagenet_utils
+from ..weights import load_model_weights
+
+
+preprocess_input = imagenet_utils.preprocess_input
+
+
+def VGG19(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        init_filters=64,
+        max_filters=512,
+        repetitions=(2, 2, 4, 4, 4),
+        **kwargs
+):
+    """Instantiates the VGG19 architecture.
+
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    # Arguments
+        include_top: whether to include the 3 fully-connected
+            layers at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+            (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(224, 224, 3)`
+            (with `channels_last` data format)
+            or `(3, 224, 224)` (with `channels_first` data format).
+            It should have exactly 3 inputs channels,
+            and width and height should be no smaller than 32.
+            E.g. `(200, 200, 3)` would be one valid value.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a 2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) < 3:
+        print('Error: stride_size length must be 3 or more')
+        return None
+
+    if len(stride_size) != len(repetitions):
+        print('Error: stride_size length must be equal to repetitions length - 1')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    x = img_input
+    for stage, rep in enumerate(repetitions):
+        for i in range(rep):
+            x = layers.Conv3D(
+                init_filters,
+                (3, 3, 3),
+                activation='relu',
+                padding='same',
+                name='block{}_conv{}'.format(stage + 1, i + 1)
+            )(x)
+
+        x = layers.MaxPooling3D(
+            stride_size[stage],
+            strides=stride_size[stage],
+            name='block{}_pool'.format(stage + 1)
+        )(x)
+
+        init_filters *= 2
+        if init_filters > max_filters:
+            init_filters = max_filters
+
+    if include_top:
+        # Classification block
+        x = layers.Flatten(name='flatten')(x)
+        x = layers.Dense(4096, activation='relu', name='fc1')(x)
+        x = layers.Dense(4096, activation='relu', name='fc2')(x)
+        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+    # Create model.
+    model = models.Model(inputs, x, name='vgg19')
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, 'vgg19', weights, classes, include_top, **kwargs)
+
+    return model
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models/vgg19.py` & `classification_models_3D-1.1.0/classification_models_3D/models/vgg16.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-"""VGG19 model for Keras.
-
-# Reference
-
-- [Very Deep Convolutional Networks for Large-Scale Image Recognition](
-    https://arxiv.org/abs/1409.1556) (ICLR 2015)
-
-"""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from .. import get_submodules_from_kwargs
-from keras_applications import imagenet_utils
-from ..weights import load_model_weights
-
-
-preprocess_input = imagenet_utils.preprocess_input
-
-
-def VGG19(
-        include_top=False,
-        weights='imagenet',
-        input_tensor=None,
-        input_shape=None,
-        pooling=None,
-        classes=1000,
-        stride_size=2,
-        init_filters=64,
-        max_filters=512,
-        repetitions=(2, 2, 4, 4, 4),
-        **kwargs
-):
-    """Instantiates the VGG19 architecture.
-
-    Optionally loads weights pre-trained on ImageNet.
-    Note that the data format convention used by the model is
-    the one specified in your Keras config at `~/.keras/keras.json`.
-
-    # Arguments
-        include_top: whether to include the 3 fully-connected
-            layers at the top of the network.
-        weights: one of `None` (random initialization),
-              'imagenet' (pre-training on ImageNet),
-              or the path to the weights file to be loaded.
-        input_tensor: optional Keras tensor
-            (i.e. output of `layers.Input()`)
-            to use as image input for the model.
-        input_shape: optional shape tuple, only to be specified
-            if `include_top` is False (otherwise the input shape
-            has to be `(224, 224, 3)`
-            (with `channels_last` data format)
-            or `(3, 224, 224)` (with `channels_first` data format).
-            It should have exactly 3 inputs channels,
-            and width and height should be no smaller than 32.
-            E.g. `(200, 200, 3)` would be one valid value.
-        pooling: Optional pooling mode for feature extraction
-            when `include_top` is `False`.
-            - `None` means that the output of the model will be
-                the 4D tensor output of the
-                last convolutional block.
-            - `avg` means that global average pooling
-                will be applied to the output of the
-                last convolutional block, and thus
-                the output of the model will be a 2D tensor.
-            - `max` means that global max pooling will
-                be applied.
-        classes: optional number of classes to classify images
-            into, only to be specified if `include_top` is True, and
-            if no `weights` argument is specified.
-
-    # Returns
-        A Keras model instance.
-
-    # Raises
-        ValueError: in case of invalid argument for `weights`,
-            or invalid input shape.
-    """
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if not (weights in {'imagenet', None} or os.path.exists(weights)):
-        raise ValueError('The `weights` argument should be either '
-                         '`None` (random initialization), `imagenet` '
-                         '(pre-training on ImageNet), '
-                         'or the path to the weights file to be loaded.')
-
-    if weights == 'imagenet' and include_top and classes != 1000:
-        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
-                         ' as true, `classes` should be 1000')
-
-    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
-    # (stride for each dimension for more flexibility)
-    if type(stride_size) not in (tuple, list):
-        stride_size = [
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-            (stride_size, stride_size, stride_size,),
-        ]
-    else:
-        stride_size = list(stride_size)
-
-    if len(stride_size) < 3:
-        print('Error: stride_size length must be 3 or more')
-        return None
-
-    if len(stride_size) != len(repetitions):
-        print('Error: stride_size length must be equal to repetitions length - 1')
-        return None
-
-    for i in range(len(stride_size)):
-        if type(stride_size[i]) not in (tuple, list):
-            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
-
-    if input_tensor is None:
-        img_input = layers.Input(shape=input_shape)
-    else:
-        if not backend.is_keras_tensor(input_tensor):
-            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
-        else:
-            img_input = input_tensor
-
-    x = img_input
-    for stage, rep in enumerate(repetitions):
-        for i in range(rep):
-            x = layers.Conv3D(
-                init_filters,
-                (3, 3, 3),
-                activation='relu',
-                padding='same',
-                name='block{}_conv{}'.format(stage + 1, i + 1)
-            )(x)
-
-        x = layers.MaxPooling3D(
-            stride_size[stage],
-            strides=stride_size[stage],
-            name='block{}_pool'.format(stage + 1)
-        )(x)
-
-        init_filters *= 2
-        if init_filters > max_filters:
-            init_filters = max_filters
-
-    if include_top:
-        # Classification block
-        x = layers.Flatten(name='flatten')(x)
-        x = layers.Dense(4096, activation='relu', name='fc1')(x)
-        x = layers.Dense(4096, activation='relu', name='fc2')(x)
-        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
-    else:
-        if pooling == 'avg':
-            x = layers.GlobalAveragePooling3D()(x)
-        elif pooling == 'max':
-            x = layers.GlobalMaxPooling3D()(x)
-
-    # Ensure that the model takes into account
-    # any potential predecessors of `input_tensor`.
-    if input_tensor is not None:
-        inputs = keras_utils.get_source_inputs(input_tensor)
-    else:
-        inputs = img_input
-    # Create model.
-    model = models.Model(inputs, x, name='vgg19')
-
-    # Load weights.
-    if weights:
-        if type(weights) == str and os.path.exists(weights):
-            model.load_weights(weights)
-        else:
-            load_model_weights(model, 'vgg19', weights, classes, include_top, **kwargs)
-
-    return model
+"""VGG16 model for Keras.
+
+# Reference
+
+- [Very Deep Convolutional Networks for Large-Scale Image Recognition](
+    https://arxiv.org/abs/1409.1556) (ICLR 2015)
+
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import os
+from .. import get_submodules_from_kwargs
+from keras.applications import imagenet_utils
+from ..weights import load_model_weights
+
+
+preprocess_input = imagenet_utils.preprocess_input
+
+
+def VGG16(
+        include_top=False,
+        weights='imagenet',
+        input_tensor=None,
+        input_shape=None,
+        pooling=None,
+        classes=1000,
+        stride_size=2,
+        init_filters=64,
+        max_filters=512,
+        repetitions=(2, 2, 3, 3, 3),
+        **kwargs
+):
+    """Instantiates the VGG16 architecture.
+
+    Optionally loads weights pre-trained on ImageNet.
+    Note that the data format convention used by the model is
+    the one specified in your Keras config at `~/.keras/keras.json`.
+
+    # Arguments
+        include_top: whether to include the 3 fully-connected
+            layers at the top of the network.
+        weights: one of `None` (random initialization),
+              'imagenet' (pre-training on ImageNet),
+              or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+            (i.e. output of `layers.Input()`)
+            to use as image input for the model.
+        input_shape: optional shape tuple, only to be specified
+            if `include_top` is False (otherwise the input shape
+            has to be `(224, 224, 3)`
+            (with `channels_last` data format)
+            or `(3, 224, 224)` (with `channels_first` data format).
+            It should have exactly 3 input channels,
+            and width and height should be no smaller than 32.
+            E.g. `(200, 200, 3)` would be one valid value.
+        pooling: Optional pooling mode for feature extraction
+            when `include_top` is `False`.
+            - `None` means that the output of the model will be
+                the 4D tensor output of the
+                last convolutional block.
+            - `avg` means that global average pooling
+                will be applied to the output of the
+                last convolutional block, and thus
+                the output of the model will be a 2D tensor.
+            - `max` means that global max pooling will
+                be applied.
+        classes: optional number of classes to classify images
+            into, only to be specified if `include_top` is True, and
+            if no `weights` argument is specified.
+
+    # Returns
+        A Keras model instance.
+
+    # Raises
+        ValueError: in case of invalid argument for `weights`,
+            or invalid input shape.
+    """
+    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
+
+    if not (weights in {'imagenet', None} or os.path.exists(weights)):
+        raise ValueError('The `weights` argument should be either '
+                         '`None` (random initialization), `imagenet` '
+                         '(pre-training on ImageNet), '
+                         'or the path to the weights file to be loaded.')
+
+    if weights == 'imagenet' and include_top and classes != 1000:
+        raise ValueError('If using `weights` as `"imagenet"` with `include_top`'
+                         ' as true, `classes` should be 1000')
+
+    # if stride_size is scalar make it tuple of length 5 with elements tuple of size 3
+    # (stride for each dimension for more flexibility)
+    if type(stride_size) not in (tuple, list):
+        stride_size = [
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+            (stride_size, stride_size, stride_size,),
+        ]
+    else:
+        stride_size = list(stride_size)
+
+    if len(stride_size) < 3:
+        print('Error: stride_size length must be 3 or more')
+        return None
+
+    if len(stride_size) != len(repetitions):
+        print('Error: stride_size length must be equal to repetitions length - 1')
+        return None
+
+    for i in range(len(stride_size)):
+        if type(stride_size[i]) not in (tuple, list):
+            stride_size[i] = (stride_size[i], stride_size[i], stride_size[i])
+
+    if input_tensor is None:
+        img_input = layers.Input(shape=input_shape)
+    else:
+        if not backend.is_keras_tensor(input_tensor):
+            img_input = layers.Input(tensor=input_tensor, shape=input_shape)
+        else:
+            img_input = input_tensor
+
+    x = img_input
+    for stage, rep in enumerate(repetitions):
+        for i in range(rep):
+            x = layers.Conv3D(
+                init_filters,
+                (3, 3, 3),
+                activation='relu',
+                padding='same',
+                name='block{}_conv{}'.format(stage + 1, i + 1)
+            )(x)
+
+        x = layers.MaxPooling3D(
+            stride_size[stage],
+            strides=stride_size[stage],
+            name='block{}_pool'.format(stage + 1)
+        )(x)
+
+        init_filters *= 2
+        if init_filters > max_filters:
+            init_filters = max_filters
+
+    if include_top:
+        # Classification block
+        x = layers.Flatten(name='flatten')(x)
+        x = layers.Dense(4096, activation='relu', name='fc1')(x)
+        x = layers.Dense(4096, activation='relu', name='fc2')(x)
+        x = layers.Dense(classes, activation='softmax', name='predictions')(x)
+    else:
+        if pooling == 'avg':
+            x = layers.GlobalAveragePooling3D()(x)
+        elif pooling == 'max':
+            x = layers.GlobalMaxPooling3D()(x)
+
+    # Ensure that the model takes into account
+    # any potential predecessors of `input_tensor`.
+    if input_tensor is not None:
+        inputs = keras_utils.get_source_inputs(input_tensor)
+    else:
+        inputs = img_input
+    # Create model.
+    model = models.Model(inputs, x, name='vgg16')
+
+    # Load weights.
+    if weights:
+        if type(weights) == str and os.path.exists(weights):
+            model.load_weights(weights)
+        else:
+            load_model_weights(model, 'vgg16', weights, classes, include_top, **kwargs)
+
+    return model
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/models_factory.py` & `classification_models_3D-1.1.0/classification_models_3D/models_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import functools
-import keras_applications as ka
-
-from .models import resnet as rn
-from .models import resnext as rx
-from .models import senet as sn
-from .models import densenet as dn
-from .models import vgg16 as vgg16
-from .models import vgg19 as vgg19
-from .models import inception_resnet_v2 as irv2
-from .models import inception_v3 as iv3
-from .models import mobilenet as mb1
-from .models import mobilenet_v2 as mb2
-from .models import efficientnet as eff
-from .models import efficientnet_v2 as eff2
-from .models import convnext as cnext
-
-
-class ModelsFactory:
-    _models = {
-
-        # ResNets
-        'resnet18': [rn.ResNet18, rn.preprocess_input],
-        'resnet34': [rn.ResNet34, rn.preprocess_input],
-        'resnet50': [rn.ResNet50, rn.preprocess_input],
-        'resnet101': [rn.ResNet101, rn.preprocess_input],
-        'resnet152': [rn.ResNet152, rn.preprocess_input],
-
-        # SE-Nets
-        'seresnet18': [rn.SEResNet18, rn.preprocess_input],
-        'seresnet34': [rn.SEResNet34, rn.preprocess_input],
-        'seresnet50': [sn.SEResNet50, sn.preprocess_input],
-        'seresnet101': [sn.SEResNet101, sn.preprocess_input],
-        'seresnet152': [sn.SEResNet152, sn.preprocess_input],
-        'seresnext50': [sn.SEResNeXt50, sn.preprocess_input],
-        'seresnext101': [sn.SEResNeXt101, sn.preprocess_input],
-        'senet154': [sn.SENet154, sn.preprocess_input],
-
-        # ResNext
-        'resnext50': [rx.ResNeXt50, rx.preprocess_input],
-        'resnext101': [rx.ResNeXt101, rx.preprocess_input],
-
-        # VGG
-        'vgg16': [vgg16.VGG16, vgg16.preprocess_input],
-        'vgg19': [vgg19.VGG19, vgg19.preprocess_input],
-
-        # Densnet
-        'densenet121': [dn.DenseNet121, dn.preprocess_input],
-        'densenet169': [dn.DenseNet169, dn.preprocess_input],
-        'densenet201': [dn.DenseNet201, dn.preprocess_input],
-
-        # Inception
-        'inceptionresnetv2': [irv2.InceptionResNetV2, irv2.preprocess_input],
-        'inceptionv3': [iv3.InceptionV3, iv3.preprocess_input],
-
-        # MobileNet
-        'mobilenet': [mb1.MobileNet, mb1.preprocess_input],
-        'mobilenetv2': [mb2.MobileNetV2, mb2.preprocess_input],
-
-        # EfficientNet
-        'efficientnetb0': [eff.EfficientNetB0, eff.preprocess_input],
-        'efficientnetb1': [eff.EfficientNetB1, eff.preprocess_input],
-        'efficientnetb2': [eff.EfficientNetB2, eff.preprocess_input],
-        'efficientnetb3': [eff.EfficientNetB3, eff.preprocess_input],
-        'efficientnetb4': [eff.EfficientNetB4, eff.preprocess_input],
-        'efficientnetb5': [eff.EfficientNetB5, eff.preprocess_input],
-        'efficientnetb6': [eff.EfficientNetB6, eff.preprocess_input],
-        'efficientnetb7': [eff.EfficientNetB7, eff.preprocess_input],
-
-        # EfficientNet v2
-        'efficientnetv2-b0': [eff2.EfficientNetV2B0, eff2.preprocess_input],
-        'efficientnetv2-b1': [eff2.EfficientNetV2B1, eff2.preprocess_input],
-        'efficientnetv2-b2': [eff2.EfficientNetV2B2, eff2.preprocess_input],
-        'efficientnetv2-b3': [eff2.EfficientNetV2B3, eff2.preprocess_input],
-        'efficientnetv2-s': [eff2.EfficientNetV2S, eff2.preprocess_input],
-        'efficientnetv2-m': [eff2.EfficientNetV2M, eff2.preprocess_input],
-        'efficientnetv2-l': [eff2.EfficientNetV2L, eff2.preprocess_input],
-
-        # ConvNext
-        'convnext_tiny': [cnext.ConvNeXtTiny, cnext.preprocess_input],
-        'convnext_small': [cnext.ConvNeXtSmall, cnext.preprocess_input],
-        'convnext_base': [cnext.ConvNeXtBase, cnext.preprocess_input],
-        'convnext_large': [cnext.ConvNeXtLarge, cnext.preprocess_input],
-        'convnext_xlarge': [cnext.ConvNeXtXLarge, cnext.preprocess_input],
-    }
-
-    @property
-    def models(self):
-        return self._models
-
-    def models_names(self):
-        return list(self.models.keys())
-
-    @staticmethod
-    def get_kwargs():
-        return {}
-
-    def inject_submodules(self, func):
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            modules_kwargs = self.get_kwargs()
-            new_kwargs = dict(list(kwargs.items()) + list(modules_kwargs.items()))
-            return func(*args, **new_kwargs)
-
-        return wrapper
-
-    def get(self, name):
-        if name not in self.models_names():
-            raise ValueError('No such model `{}`, available models: {}'.format(
-                name, list(self.models_names())))
-
-        model_fn, preprocess_input = self.models[name]
-        model_fn = self.inject_submodules(model_fn)
-        preprocess_input = self.inject_submodules(preprocess_input)
-        return model_fn, preprocess_input
+import functools
+
+from .models import resnet as rn
+from .models import resnext as rx
+from .models import senet as sn
+from .models import densenet as dn
+from .models import vgg16 as vgg16
+from .models import vgg19 as vgg19
+from .models import inception_resnet_v2 as irv2
+from .models import inception_v3 as iv3
+from .models import mobilenet as mb1
+from .models import mobilenet_v2 as mb2
+from .models import efficientnet as eff
+from .models import efficientnet_v2 as eff2
+from .models import convnext as cnext
+
+
+class ModelsFactory:
+    _models = {
+
+        # ResNets
+        'resnet18': [rn.ResNet18, rn.preprocess_input],
+        'resnet34': [rn.ResNet34, rn.preprocess_input],
+        'resnet50': [rn.ResNet50, rn.preprocess_input],
+        'resnet101': [rn.ResNet101, rn.preprocess_input],
+        'resnet152': [rn.ResNet152, rn.preprocess_input],
+
+        # SE-Nets
+        'seresnet18': [rn.SEResNet18, rn.preprocess_input],
+        'seresnet34': [rn.SEResNet34, rn.preprocess_input],
+        'seresnet50': [sn.SEResNet50, sn.preprocess_input],
+        'seresnet101': [sn.SEResNet101, sn.preprocess_input],
+        'seresnet152': [sn.SEResNet152, sn.preprocess_input],
+        'seresnext50': [sn.SEResNeXt50, sn.preprocess_input],
+        'seresnext101': [sn.SEResNeXt101, sn.preprocess_input],
+        'senet154': [sn.SENet154, sn.preprocess_input],
+
+        # ResNext
+        'resnext50': [rx.ResNeXt50, rx.preprocess_input],
+        'resnext101': [rx.ResNeXt101, rx.preprocess_input],
+
+        # VGG
+        'vgg16': [vgg16.VGG16, vgg16.preprocess_input],
+        'vgg19': [vgg19.VGG19, vgg19.preprocess_input],
+
+        # Densnet
+        'densenet121': [dn.DenseNet121, dn.preprocess_input],
+        'densenet169': [dn.DenseNet169, dn.preprocess_input],
+        'densenet201': [dn.DenseNet201, dn.preprocess_input],
+
+        # Inception
+        'inceptionresnetv2': [irv2.InceptionResNetV2, irv2.preprocess_input],
+        'inceptionv3': [iv3.InceptionV3, iv3.preprocess_input],
+
+        # MobileNet
+        'mobilenet': [mb1.MobileNet, mb1.preprocess_input],
+        'mobilenetv2': [mb2.MobileNetV2, mb2.preprocess_input],
+
+        # EfficientNet
+        'efficientnetb0': [eff.EfficientNetB0, eff.preprocess_input],
+        'efficientnetb1': [eff.EfficientNetB1, eff.preprocess_input],
+        'efficientnetb2': [eff.EfficientNetB2, eff.preprocess_input],
+        'efficientnetb3': [eff.EfficientNetB3, eff.preprocess_input],
+        'efficientnetb4': [eff.EfficientNetB4, eff.preprocess_input],
+        'efficientnetb5': [eff.EfficientNetB5, eff.preprocess_input],
+        'efficientnetb6': [eff.EfficientNetB6, eff.preprocess_input],
+        'efficientnetb7': [eff.EfficientNetB7, eff.preprocess_input],
+
+        # EfficientNet v2
+        'efficientnetv2-b0': [eff2.EfficientNetV2B0, eff2.preprocess_input],
+        'efficientnetv2-b1': [eff2.EfficientNetV2B1, eff2.preprocess_input],
+        'efficientnetv2-b2': [eff2.EfficientNetV2B2, eff2.preprocess_input],
+        'efficientnetv2-b3': [eff2.EfficientNetV2B3, eff2.preprocess_input],
+        'efficientnetv2-s': [eff2.EfficientNetV2S, eff2.preprocess_input],
+        'efficientnetv2-m': [eff2.EfficientNetV2M, eff2.preprocess_input],
+        'efficientnetv2-l': [eff2.EfficientNetV2L, eff2.preprocess_input],
+
+        # ConvNext
+        'convnext_tiny': [cnext.ConvNeXtTiny, cnext.preprocess_input],
+        'convnext_small': [cnext.ConvNeXtSmall, cnext.preprocess_input],
+        'convnext_base': [cnext.ConvNeXtBase, cnext.preprocess_input],
+        'convnext_large': [cnext.ConvNeXtLarge, cnext.preprocess_input],
+        'convnext_xlarge': [cnext.ConvNeXtXLarge, cnext.preprocess_input],
+    }
+
+    @property
+    def models(self):
+        return self._models
+
+    @staticmethod
+    def models_names():
+        return list(ModelsFactory._models.keys())
+
+    @staticmethod
+    def get_kwargs():
+        return {}
+
+    def inject_submodules(self, func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            modules_kwargs = self.get_kwargs()
+            new_kwargs = dict(list(kwargs.items()) + list(modules_kwargs.items()))
+            return func(*args, **new_kwargs)
+
+        return wrapper
+
+    def get(self, name):
+        if name not in self.models_names():
+            raise ValueError('No such model `{}`, available models: {}'.format(
+                name, list(self.models_names())))
+
+        model_fn, preprocess_input = self.models[name]
+        model_fn = self.inject_submodules(model_fn)
+        preprocess_input = self.inject_submodules(preprocess_input)
+        return model_fn, preprocess_input
```

### Comparing `classification_models_3D-1.0.8/classification_models_3D/weights.py` & `classification_models_3D-1.1.0/classification_models_3D/weights.py`

 * *Files identical despite different names*

### Comparing `classification_models_3D-1.0.8/classification_models_3D.egg-info/SOURCES.txt` & `classification_models_3D-1.1.0/classification_models_3D.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 setup.py
 classification_models_3D/__init__.py
 classification_models_3D/__version__.py
-classification_models_3D/keras.py
+classification_models_3D/kkeras.py
 classification_models_3D/models_factory.py
-classification_models_3D/tfkeras.py
 classification_models_3D/weights.py
 classification_models_3D.egg-info/PKG-INFO
 classification_models_3D.egg-info/SOURCES.txt
 classification_models_3D.egg-info/dependency_links.txt
 classification_models_3D.egg-info/top_level.txt
 classification_models_3D/models/_DepthwiseConv3D.py
 classification_models_3D/models/__init__.py
```

### Comparing `classification_models_3D-1.0.8/setup.py` & `classification_models_3D-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='classification_models_3D',
-    version='1.0.8',
+    version='1.1.0',
     author='Roman Sol (ZFTurbo)',
     packages=['classification_models_3D', 'classification_models_3D/models'],
     url='https://github.com/ZFTurbo/classification_models_3D',
     description='Set of models for classification of 3D volumes.',
-    long_description='3D variants of popular CNN models for classification like ResNets, DenseNets, VGG, etc. '
+    long_description='This repository contains 3D variants of popular classification CNN models like ResNets, DenseNets, VGG, etc for keras module. '
                      'It also contains weights obtained by converting ImageNet weights from the same 2D models. '
-                     'Models work with keras and tensorflow.keras.'
+                     'Models work with keras 3 with different backends like Tensorflow, Torch and Jax.'
                      'More details: https://github.com/ZFTurbo/classification_models_3D',
 )
```

