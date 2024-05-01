# Comparing `tmp/segmentation_models_3D-1.0.7.tar.gz` & `tmp/segmentation_models_3D-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\segmentation_models_3D-1.0.7.tar", last modified: Sat Jan  6 23:44:40 2024, max compression
+gzip compressed data, was "dist\segmentation_models_3D-1.1.0.tar", last modified: Wed May  1 12:16:10 2024, max compression
```

## Comparing `segmentation_models_3D-1.0.7.tar` & `segmentation_models_3D-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.216954 segmentation_models_3D-1.0.7/
--rw-rw-rw-   0        0        0      487 2024-01-06 23:44:40.216954 segmentation_models_3D-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2024-01-03 08:31:38.000000 segmentation_models_3D-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.200955 segmentation_models_3D-1.0.7/segmentation_models_3D/
--rw-rw-rw-   0        0        0     3928 2022-05-10 07:59:23.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/__init__.py
--rw-rw-rw-   0        0        0       63 2023-11-29 15:28:46.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/__version__.py
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.204955 segmentation_models_3D-1.0.7/segmentation_models_3D/backbones/
--rw-rw-rw-   0        0        0        0 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/backbones/__init__.py
--rw-rw-rw-   0        0        0     5527 2022-05-10 08:28:01.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/backbones/backbones_factory.py
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.207956 segmentation_models_3D-1.0.7/segmentation_models_3D/base/
--rw-rw-rw-   0        0        0       71 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/base/__init__.py
--rw-rw-rw-   0        0        0    11687 2020-03-26 14:00:48.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/base/functional.py
--rw-rw-rw-   0        0        0     2687 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/base/objects.py
--rw-rw-rw-   0        0        0     8428 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/losses.py
--rw-rw-rw-   0        0        0     8812 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/metrics.py
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.213954 segmentation_models_3D-1.0.7/segmentation_models_3D/models/
--rw-rw-rw-   0        0        0        0 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/__init__.py
--rw-rw-rw-   0        0        0     2139 2020-03-13 15:33:33.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/_common_blocks.py
--rw-rw-rw-   0        0        0      367 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/_utils.py
--rw-rw-rw-   0        0        0     9139 2020-03-26 14:12:02.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/fpn.py
--rw-rw-rw-   0        0        0     9846 2020-03-26 14:19:26.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/linknet.py
--rw-rw-rw-   0        0        0     8688 2020-03-26 14:24:10.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/pspnet.py
--rw-rw-rw-   0        0        0     8495 2020-03-26 14:16:57.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/models/unet.py
--rw-rw-rw-   0        0        0     3002 2020-01-10 11:25:34.000000 segmentation_models_3D-1.0.7/segmentation_models_3D/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-06 23:44:40.204955 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/
--rw-rw-rw-   0        0        0      487 2024-01-06 23:44:40.000000 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2024-01-06 23:44:40.000000 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-06 23:44:40.000000 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-01-06 23:44:40.000000 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/requires.txt
--rw-rw-rw-   0        0        0      114 2024-01-06 23:44:40.000000 segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-06 23:44:40.216954 segmentation_models_3D-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      928 2024-01-06 23:43:56.000000 segmentation_models_3D-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.824137 segmentation_models_3D-1.1.0/
+-rw-rw-rw-   0        0        0      478 2024-05-01 12:16:10.824137 segmentation_models_3D-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4225 2024-05-01 12:09:54.000000 segmentation_models_3D-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.812137 segmentation_models_3D-1.1.0/segmentation_models_3D/
+-rw-rw-rw-   0        0        0     4930 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-11-29 15:28:46.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.816137 segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/
+-rw-rw-rw-   0        0        0        0 2020-01-10 11:25:34.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/__init__.py
+-rw-rw-rw-   0        0        0     5527 2022-05-10 08:28:01.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/backbones_factory.py
+-rw-rw-rw-   0        0        0    15307 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    15052 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/inception_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.818137 segmentation_models_3D-1.1.0/segmentation_models_3D/base/
+-rw-rw-rw-   0        0        0       71 2020-01-10 11:25:34.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/base/__init__.py
+-rw-rw-rw-   0        0        0    11945 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/base/functional.py
+-rw-rw-rw-   0        0        0     3188 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/base/objects.py
+-rw-rw-rw-   0        0        0     8428 2020-01-10 11:25:34.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/losses.py
+-rw-rw-rw-   0        0        0     8812 2020-01-10 11:25:34.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.822137 segmentation_models_3D-1.1.0/segmentation_models_3D/models/
+-rw-rw-rw-   0        0        0        0 2020-01-10 11:25:34.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/__init__.py
+-rw-rw-rw-   0        0        0     2198 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/_common_blocks.py
+-rw-rw-rw-   0        0        0      367 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/_utils.py
+-rw-rw-rw-   0        0        0     9425 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/fpn.py
+-rw-rw-rw-   0        0        0    10134 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/linknet.py
+-rw-rw-rw-   0        0        0     8966 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/pspnet.py
+-rw-rw-rw-   0        0        0     8742 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/models/unet.py
+-rw-rw-rw-   0        0        0     3066 2024-05-01 11:53:27.000000 segmentation_models_3D-1.1.0/segmentation_models_3D/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:16:10.814137 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/
+-rw-rw-rw-   0        0        0      478 2024-05-01 12:16:10.000000 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1536 2024-05-01 12:16:10.000000 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 12:16:10.000000 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-01 12:16:10.000000 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      114 2024-05-01 12:16:10.000000 segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 12:16:10.824137 segmentation_models_3D-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      839 2024-05-01 12:10:48.000000 segmentation_models_3D-1.1.0/setup.py
```

### Comparing `segmentation_models_3D-1.0.7/README.md` & `segmentation_models_3D-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Segmentation models 3D Zoo - Keras and TF.Keras
+# Segmentation models 3D Zoo for Keras 3
 
 The repository contains 3D variants of popular models for segmentation like FPN, Unet, Linknet and PSPNet. 
 
 This repository is based on great [segmentation_models](https://github.com/qubvel/segmentation_models) repo by [@qubvel](https://github.com/qubvel/)
 
 ### Available architectures: 
 -  [Unet](https://arxiv.org/abs/1505.04597)
@@ -22,15 +22,15 @@
 import segmentation_models_3D as sm
 
 model1 = sm.Unet(
     'resnet34', 
     encoder_weights='imagenet'
 )
 
-# binary segmentation (this parameters are default when you call Unet('resnet34')
+# binary segmentation (these parameters are default when you call Unet('resnet34')
 model2 = sm.FPN(
     'densenet121', 
     classes=1, 
     activation='sigmoid'
 )
 
 # multiclass segmentation with non overlapping class masks (your classes + background)
@@ -63,38 +63,49 @@
 'inceptionv3', 'mobilenet', 'mobilenetv2', 'efficientnetb0', 
 'efficientnetb1', 'efficientnetb2', 'efficientnetb3', 'efficientnetb4', 
 'efficientnetb5', 'efficientnetb6', 'efficientnetb7', 'efficientnetv2-b1', 
 'efficientnetv2-b2', 'efficientnetv2-b3', 'efficientnetv2-s', 
 'efficientnetv2-m', 'efficientnetv2-l'
 `
 
-More examples can be found in [tst_keras.py](tst_keras.py)
+More examples can be found in: 
+- Tensorflow: [tst_keras_tensorflow.py](tst_keras_tensorflow.py)
+- Torch: [tst_keras_torch.py](tst_keras_torch.py)
+- Jax: [tst_keras_jax.py](tst_keras_jax.py)
+
 
 ##### Training model:
 
-There is training example in [training_example.py](training_example.py)
+There is training example in [training_example_tensorflow.py](training_example_tensorflow.py)
 * I tried to keep code as simple as possible
 * I couldn't find good dataset for 3D segmentation task. So I randomly generate 3D volumes with dark background with light 
 figures (spheres and cuboids) and model tries to segment these figures independetly. 1st mask for circles and 2nd mask for cuboids.
 
 ### To Do List
 
 * Add `stride_size` parameter for better control of models
 
 ### Related repositories
 
  * [https://github.com/qubvel/classification_models](https://github.com/qubvel/classification_models) - original classification 2D repo
  * [https://github.com/qubvel/segmentation_models](https://github.com/qubvel/segmentation_models) - original segmentation 2D repo
  * [classification_models_3D](https://github.com/ZFTurbo/classification_models_3D) - models for classification in 3D
+ * [segmentation_models_pytorch_3d](https://github.com/ZFTurbo/segmentation_models_pytorch_3d) - models for segmentation in 3D for Pytorch
  * [volumentations](https://github.com/ZFTurbo/volumentations) - 3D augmentations
  
 ### Unresolved problems
 
 * There is no 'bilinear' interpolation for UpSample3D layer, so it uses Nearest Neighbour upsampling.
- 
+
+### Older versions
+
+Last version which supports Keras 2 is 1.0.7
+
+`pip install segmentation-models-3D==1.0.7`
+
 ## Citation
 
 For more details, please refer to the publication: https://doi.org/10.1016/j.compbiomed.2021.105089
 
 If you find this code useful, please cite it as:
 ```
 @article{solovyev20223d,
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/__init__.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,160 @@
-import os
-import functools
-from .__version__ import __version__
-from . import base
-
-_KERAS_FRAMEWORK_NAME = 'keras'
-_TF_KERAS_FRAMEWORK_NAME = 'tf.keras'
-
-_DEFAULT_KERAS_FRAMEWORK = _TF_KERAS_FRAMEWORK_NAME
-_KERAS_FRAMEWORK = None
-_KERAS_BACKEND = None
-_KERAS_LAYERS = None
-_KERAS_MODELS = None
-_KERAS_UTILS = None
-_KERAS_LOSSES = None
-
-
-def inject_global_losses(func):
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        kwargs['losses'] = _KERAS_LOSSES
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def inject_global_submodules(func):
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        kwargs['backend'] = _KERAS_BACKEND
-        kwargs['layers'] = _KERAS_LAYERS
-        kwargs['models'] = _KERAS_MODELS
-        kwargs['utils'] = _KERAS_UTILS
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def filter_kwargs(func):
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        new_kwargs = {k: v for k, v in kwargs.items() if k in ['backend', 'layers', 'models', 'utils']}
-        return func(*args, **new_kwargs)
-
-    return wrapper
-
-
-def framework():
-    """Return name of Segmentation Models framework"""
-    return _KERAS_FRAMEWORK
-
-
-def set_framework(name):
-    """Set framework for Segmentation Models
-
-    Args:
-        name (str): one of ``keras``, ``tf.keras``, case insensitive.
-
-    Raises:
-        ValueError: in case of incorrect framework name.
-        ImportError: in case framework is not installed.
-
-    """
-    name = name.lower()
-
-    if name == _KERAS_FRAMEWORK_NAME:
-        import keras
-    elif name == _TF_KERAS_FRAMEWORK_NAME:
-        from tensorflow import keras
-    else:
-        raise ValueError('Not correct module name `{}`, use `{}` or `{}`'.format(
-            name, _KERAS_FRAMEWORK_NAME, _TF_KERAS_FRAMEWORK_NAME))
-
-    global _KERAS_BACKEND, _KERAS_LAYERS, _KERAS_MODELS
-    global _KERAS_UTILS, _KERAS_LOSSES, _KERAS_FRAMEWORK
-
-    _KERAS_FRAMEWORK = name
-    _KERAS_BACKEND = keras.backend
-    _KERAS_LAYERS = keras.layers
-    _KERAS_MODELS = keras.models
-    _KERAS_UTILS = keras.utils
-    _KERAS_LOSSES = keras.losses
-
-    # allow losses/metrics get keras submodules
-    base.KerasObject.set_submodules(
-        backend=keras.backend,
-        layers=keras.layers,
-        models=keras.models,
-        utils=keras.utils,
-    )
-
-
-# set default framework
-_framework = os.environ.get('SM_FRAMEWORK', _DEFAULT_KERAS_FRAMEWORK)
-try:
-    set_framework(_framework)
-except ImportError:
-    other = _TF_KERAS_FRAMEWORK_NAME if _framework == _KERAS_FRAMEWORK_NAME else _KERAS_FRAMEWORK_NAME
-    set_framework(other)
-
-print('Segmentation Models: using `{}` framework.'.format(_KERAS_FRAMEWORK))
-
-# import helper modules
-from . import losses
-from . import metrics
-from . import utils
-
-# wrap segmentation models with framework modules
-from .backbones.backbones_factory import Backbones
-from .models.unet import Unet as _Unet
-from .models.pspnet import PSPNet as _PSPNet
-from .models.linknet import Linknet as _Linknet
-from .models.fpn import FPN as _FPN
-
-Unet = inject_global_submodules(_Unet)
-PSPNet = inject_global_submodules(_PSPNet)
-Linknet = inject_global_submodules(_Linknet)
-FPN = inject_global_submodules(_FPN)
-get_available_backbone_names = Backbones.models_names
-
-
-def get_preprocessing(name):
-    preprocess_input = Backbones.get_preprocessing(name)
-    # add bakcend, models, layers, utils submodules in kwargs
-    preprocess_input = inject_global_submodules(preprocess_input)
-    # delete other kwargs
-    # keras-applications preprocessing raise an error if something
-    # except `backend`, `layers`, `models`, `utils` passed in kwargs
-    preprocess_input = filter_kwargs(preprocess_input)
-    return preprocess_input
-
-
-__all__ = [
-    'Unet', 'PSPNet', 'FPN', 'Linknet',
-    'set_framework', 'framework',
-    'get_preprocessing', 'get_available_backbone_names',
-    'losses', 'metrics', 'utils',
-    '__version__',
-]
+import os
+import functools
+from .__version__ import __version__
+from . import base
+
+_KERAS_FRAMEWORK_NAME = 'keras'
+_TF_KERAS_FRAMEWORK_NAME = 'tf.keras'
+
+_DEFAULT_KERAS_FRAMEWORK = _TF_KERAS_FRAMEWORK_NAME
+_KERAS_FRAMEWORK = None
+_KERAS_BACKEND = None
+_KERAS_LAYERS = None
+_KERAS_MODELS = None
+_KERAS_UTILS = None
+_KERAS_LOSSES = None
+_KERAS_OPS = None
+_KERAS_METRICS = None
+
+
+def get_submodules_from_kwargs(kwargs):
+    backend = kwargs.get('backend', _KERAS_BACKEND)
+    layers = kwargs.get('layers', _KERAS_LAYERS)
+    models = kwargs.get('models', _KERAS_MODELS)
+    utils = kwargs.get('utils', _KERAS_UTILS)
+    ops = kwargs.get('ops', _KERAS_OPS)
+    metrics = kwargs.get('metrics', _KERAS_METRICS)
+    for key in kwargs.keys():
+        if key not in ['backend', 'layers', 'models', 'utils', 'ops', 'metrics']:
+            raise TypeError('Invalid keyword argument: %s', key)
+    return backend, layers, models, utils, ops, metrics
+
+
+def inject_global_losses(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        kwargs['losses'] = _KERAS_LOSSES
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def inject_global_submodules(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        kwargs['backend'] = _KERAS_BACKEND
+        kwargs['layers'] = _KERAS_LAYERS
+        kwargs['models'] = _KERAS_MODELS
+        kwargs['utils'] = _KERAS_UTILS
+        kwargs['ops'] = _KERAS_OPS
+        kwargs['metrics'] = _KERAS_METRICS
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def filter_kwargs(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        new_kwargs = {k: v for k, v in kwargs.items() if k in ['backend', 'layers', 'models', 'utils', 'ops', 'metrics']}
+        return func(*args, **new_kwargs)
+
+    return wrapper
+
+
+def framework():
+    """Return name of Segmentation Models framework"""
+    return _KERAS_FRAMEWORK
+
+
+def set_framework(name):
+    """Set framework for Segmentation Models
+
+    Args:
+        name (str): one of ``keras``, ``tf.keras``, case insensitive.
+
+    Raises:
+        ValueError: in case of incorrect framework name.
+        ImportError: in case framework is not installed.
+
+    """
+    name = name.lower()
+
+    if name == _KERAS_FRAMEWORK_NAME:
+        import keras
+    elif name == _TF_KERAS_FRAMEWORK_NAME:
+        from tensorflow import keras
+    else:
+        raise ValueError('Not correct module name `{}`, use `{}` or `{}`'.format(
+            name, _KERAS_FRAMEWORK_NAME, _TF_KERAS_FRAMEWORK_NAME))
+
+    global _KERAS_BACKEND, _KERAS_LAYERS, _KERAS_MODELS, _KERAS_OPS, _KERAS_METRICS
+    global _KERAS_UTILS, _KERAS_LOSSES, _KERAS_FRAMEWORK
+
+    _KERAS_FRAMEWORK = name
+    _KERAS_BACKEND = keras.backend
+    _KERAS_LAYERS = keras.layers
+    _KERAS_MODELS = keras.models
+    _KERAS_UTILS = keras.utils
+    _KERAS_LOSSES = keras.losses
+    _KERAS_OPS = keras.ops
+    _KERAS_METRICS = keras.metrics
+
+    # allow losses/metrics get keras submodules
+    base.KerasObject.set_submodules(
+        backend=keras.backend,
+        layers=keras.layers,
+        models=keras.models,
+        utils=keras.utils,
+        ops=keras.ops,
+        metrics=keras.metrics
+    )
+
+
+# set default framework
+_framework = os.environ.get('SM_FRAMEWORK', _DEFAULT_KERAS_FRAMEWORK)
+try:
+    set_framework(_framework)
+except ImportError:
+    other = _TF_KERAS_FRAMEWORK_NAME if _framework == _KERAS_FRAMEWORK_NAME else _KERAS_FRAMEWORK_NAME
+    set_framework(other)
+
+print('Segmentation Models: using `{}` framework.'.format(_KERAS_FRAMEWORK))
+
+# import helper modules
+from . import losses
+from . import metrics
+from . import utils
+
+# wrap segmentation models with framework modules
+from .backbones.backbones_factory import Backbones
+from .models.unet import Unet as _Unet
+from .models.pspnet import PSPNet as _PSPNet
+from .models.linknet import Linknet as _Linknet
+from .models.fpn import FPN as _FPN
+
+Unet = inject_global_submodules(_Unet)
+PSPNet = inject_global_submodules(_PSPNet)
+Linknet = inject_global_submodules(_Linknet)
+FPN = inject_global_submodules(_FPN)
+get_available_backbone_names = Backbones.models_names
+
+
+def get_preprocessing(name):
+    preprocess_input = Backbones.get_preprocessing(name)
+    # add bakcend, models, layers, utils submodules in kwargs
+    preprocess_input = inject_global_submodules(preprocess_input)
+    # delete other kwargs
+    # keras-applications preprocessing raise an error if something
+    # except `backend`, `layers`, `models`, `utils` passed in kwargs
+    preprocess_input = filter_kwargs(preprocess_input)
+    return preprocess_input
+
+
+__all__ = [
+    'Unet', 'PSPNet', 'FPN', 'Linknet',
+    'set_framework', 'framework',
+    'get_preprocessing', 'get_available_backbone_names',
+    'losses', 'metrics', 'utils',
+    '__version__',
+]
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/backbones/backbones_factory.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/backbones/backbones_factory.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/base/functional.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/base/functional.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,308 +1,314 @@
-SMOOTH = 1e-5
-
-
-# ----------------------------------------------------------------
-#   Helpers
-# ----------------------------------------------------------------
-
-def _gather_channels(x, indexes, **kwargs):
-    """Slice tensor along channels axis by given indexes"""
-    backend = kwargs['backend']
-    if backend.image_data_format() == 'channels_last':
-        x = backend.permute_dimensions(x, (4, 0, 1, 2, 3))
-        x = backend.gather(x, indexes)
-        x = backend.permute_dimensions(x, (1, 2, 3, 4, 0))
-    else:
-        x = backend.permute_dimensions(x, (1, 0, 2, 3, 4))
-        x = backend.gather(x, indexes)
-        x = backend.permute_dimensions(x, (1, 0, 2, 3, 4))
-    return x
-
-
-def get_reduce_axes(per_image, **kwargs):
-    backend = kwargs['backend']
-    axes = [1, 2, 3] if backend.image_data_format() == 'channels_last' else [2, 3, 4]
-    if not per_image:
-        axes.insert(0, 0)
-    return axes
-
-
-def gather_channels(*xs, indexes=None, **kwargs):
-    """Slice tensors along channels axis by given indexes"""
-    if indexes is None:
-        return xs
-    elif isinstance(indexes, (int)):
-        indexes = [indexes]
-    xs = [_gather_channels(x, indexes=indexes, **kwargs) for x in xs]
-    return xs
-
-
-def round_if_needed(x, threshold, **kwargs):
-    backend = kwargs['backend']
-    if threshold is not None:
-        x = backend.greater(x, threshold)
-        x = backend.cast(x, backend.floatx())
-    return x
-
-
-def average(x, per_image=False, class_weights=None, **kwargs):
-    backend = kwargs['backend']
-    if per_image:
-        x = backend.mean(x, axis=0)
-    if class_weights is not None:
-        x = x * class_weights
-    return backend.mean(x)
-
-
-# ----------------------------------------------------------------
-#   Metric Functions
-# ----------------------------------------------------------------
-
-def iou_score(gt, pr, class_weights=1., class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
-    r""" The `Jaccard index`_, also known as Intersection over Union and the Jaccard similarity coefficient
-    (originally coined coefficient de communauté by Paul Jaccard), is a statistic used for comparing the
-    similarity and diversity of sample sets. The Jaccard coefficient measures similarity between finite sample sets,
-    and is defined as the size of the intersection divided by the size of the union of the sample sets:
-
-    .. math:: J(A, B) = \frac{A \cap B}{A \cup B}
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        class_weights: 1. or list of class weights, len(weights) = C
-        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
-        smooth: value to avoid division by zero
-        per_image: if ``True``, metric is calculated as mean over images in batch (B),
-            else over whole batch
-        threshold: value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round
-
-    Returns:
-        IoU/Jaccard score in range [0, 1]
-
-    .. _`Jaccard index`: https://en.wikipedia.org/wiki/Jaccard_index
-
-    """
-
-    backend = kwargs['backend']
-
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-    pr = round_if_needed(pr, threshold, **kwargs)
-    axes = get_reduce_axes(per_image, **kwargs)
-
-    # score calculation
-    intersection = backend.sum(gt * pr, axis=axes)
-    union = backend.sum(gt + pr, axis=axes) - intersection
-
-    score = (intersection + smooth) / (union + smooth)
-    score = average(score, per_image, class_weights, **kwargs)
-
-    return score
-
-
-def f_score(gt, pr, beta=1, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None,
-            **kwargs):
-    r"""The F-score (Dice coefficient) can be interpreted as a weighted average of the precision and recall,
-    where an F-score reaches its best value at 1 and worst score at 0.
-    The relative contribution of ``precision`` and ``recall`` to the F1-score are equal.
-    The formula for the F score is:
-
-    .. math:: F_\beta(precision, recall) = (1 + \beta^2) \frac{precision \cdot recall}
-        {\beta^2 \cdot precision + recall}
-
-    The formula in terms of *Type I* and *Type II* errors:
-
-    .. math:: F_\beta(A, B) = \frac{(1 + \beta^2) TP} {(1 + \beta^2) TP + \beta^2 FN + FP}
-
-
-    where:
-        TP - true positive;
-        FP - false positive;
-        FN - false negative;
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        class_weights: 1. or list of class weights, len(weights) = C
-        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
-        beta: f-score coefficient
-        smooth: value to avoid division by zero
-        per_image: if ``True``, metric is calculated as mean over images in batch (B),
-            else over whole batch
-        threshold: value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round
-
-    Returns:
-        F-score in range [0, 1]
-
-    """
-
-    backend = kwargs['backend']
-
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-    pr = round_if_needed(pr, threshold, **kwargs)
-    axes = get_reduce_axes(per_image, **kwargs)
-
-    # calculate score
-    tp = backend.sum(gt * pr, axis=axes)
-    fp = backend.sum(pr, axis=axes) - tp
-    fn = backend.sum(gt, axis=axes) - tp
-
-    score = ((1 + beta ** 2) * tp + smooth) \
-            / ((1 + beta ** 2) * tp + beta ** 2 * fn + fp + smooth)
-    score = average(score, per_image, class_weights, **kwargs)
-
-    return score
-
-
-def precision(gt, pr, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
-    r"""Calculate precision between the ground truth (gt) and the prediction (pr).
-
-    .. math:: F_\beta(tp, fp) = \frac{tp} {(tp + fp)}
-
-    where:
-         - tp - true positives;
-         - fp - false positives;
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        class_weights: 1. or ``np.array`` of class weights (``len(weights) = num_classes``)
-        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
-        smooth: Float value to avoid division by zero.
-        per_image: If ``True``, metric is calculated as mean over images in batch (B),
-            else over whole batch.
-        threshold: Float value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round.
-        name: Optional string, if ``None`` default ``precision`` name is used.
-
-    Returns:
-        float: precision score
-    """
-    backend = kwargs['backend']
-
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-    pr = round_if_needed(pr, threshold, **kwargs)
-    axes = get_reduce_axes(per_image, **kwargs)
-
-    # score calculation
-    tp = backend.sum(gt * pr, axis=axes)
-    fp = backend.sum(pr, axis=axes) - tp
-    
-    score = (tp + smooth) / (tp + fp + smooth)
-    score = average(score, per_image, class_weights, **kwargs)
-
-    return score
-
-
-def recall(gt, pr, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
-    r"""Calculate recall between the ground truth (gt) and the prediction (pr).
-
-    .. math:: F_\beta(tp, fn) = \frac{tp} {(tp + fn)}
-
-    where:
-         - tp - true positives;
-         - fp - false positives;
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        class_weights: 1. or ``np.array`` of class weights (``len(weights) = num_classes``)
-        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
-        smooth: Float value to avoid division by zero.
-        per_image: If ``True``, metric is calculated as mean over images in batch (B),
-            else over whole batch.
-        threshold: Float value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round.
-        name: Optional string, if ``None`` default ``precision`` name is used.
-
-    Returns:
-        float: recall score
-    """
-    backend = kwargs['backend']
-
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-    pr = round_if_needed(pr, threshold, **kwargs)
-    axes = get_reduce_axes(per_image, **kwargs)
-
-    tp = backend.sum(gt * pr, axis=axes)
-    fn = backend.sum(gt, axis=axes) - tp
-
-    score = (tp + smooth) / (tp + fn + smooth)
-    score = average(score, per_image, class_weights, **kwargs)
-
-    return score
-
-
-# ----------------------------------------------------------------
-#   Loss Functions
-# ----------------------------------------------------------------
-
-def categorical_crossentropy(gt, pr, class_weights=1., class_indexes=None, **kwargs):
-    backend = kwargs['backend']
-
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-
-    # scale predictions so that the class probas of each sample sum to 1
-    axis = 4 if backend.image_data_format() == 'channels_last' else 1
-    pr /= backend.sum(pr, axis=axis, keepdims=True)
-
-    # clip to prevent NaN's and Inf's
-    pr = backend.clip(pr, backend.epsilon(), 1 - backend.epsilon())
-
-    # calculate loss
-    output = gt * backend.log(pr) * class_weights
-    return - backend.mean(output)
-
-
-def binary_crossentropy(gt, pr, **kwargs):
-    backend = kwargs['backend']
-    return backend.mean(backend.binary_crossentropy(gt, pr))
-
-
-def categorical_focal_loss(gt, pr, gamma=2.0, alpha=0.25, class_indexes=None, **kwargs):
-    r"""Implementation of Focal Loss from the paper in multiclass classification
-
-    Formula:
-        loss = - gt * alpha * ((1 - pr)^gamma) * log(pr)
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        alpha: the same as weighting factor in balanced cross entropy, default 0.25
-        gamma: focusing parameter for modulating factor (1-p), default 2.0
-        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
-
-    """
-
-    backend = kwargs['backend']
-    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
-
-    # clip to prevent NaN's and Inf's
-    pr = backend.clip(pr, backend.epsilon(), 1.0 - backend.epsilon())
-
-    # Calculate focal loss
-    loss = - gt * (alpha * backend.pow((1 - pr), gamma) * backend.log(pr))
-
-    return backend.mean(loss)
-
-
-def binary_focal_loss(gt, pr, gamma=2.0, alpha=0.25, **kwargs):
-    r"""Implementation of Focal Loss from the paper in binary classification
-
-    Formula:
-        loss = - gt * alpha * ((1 - pr)^gamma) * log(pr) \
-               - (1 - gt) * alpha * (pr^gamma) * log(1 - pr)
-
-    Args:
-        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
-        alpha: the same as weighting factor in balanced cross entropy, default 0.25
-        gamma: focusing parameter for modulating factor (1-p), default 2.0
-
-    """
-    backend = kwargs['backend']
-
-    # clip to prevent NaN's and Inf's
-    pr = backend.clip(pr, backend.epsilon(), 1.0 - backend.epsilon())
-
-    loss_1 = - gt * (alpha * backend.pow((1 - pr), gamma) * backend.log(pr))
-    loss_0 = - (1 - gt) * ((1 - alpha) * backend.pow((pr), gamma) * backend.log(1 - pr))
-    loss = backend.mean(loss_0 + loss_1)
-    return loss
+SMOOTH = 1e-5
+
+
+# ----------------------------------------------------------------
+#   Helpers
+# ----------------------------------------------------------------
+
+def _gather_channels(x, indexes, **kwargs):
+    """Slice tensor along channels axis by given indexes"""
+    backend = kwargs['backend']
+    ops = kwargs['ops']
+    if backend.image_data_format() == 'channels_last':
+        x = ops.transpose(x, (4, 0, 1, 2, 3))
+        x = ops.take(x, indexes, axis=0)
+        x = ops.transpose(x, (1, 2, 3, 4, 0))
+    else:
+        x = ops.transpose(x, (1, 0, 2, 3, 4))
+        x = ops.take(x, indexes, axis=0)
+        x = ops.transpose(x, (1, 0, 2, 3, 4))
+    return x
+
+
+def get_reduce_axes(per_image, **kwargs):
+    backend = kwargs['backend']
+    axes = [1, 2, 3] if backend.image_data_format() == 'channels_last' else [2, 3, 4]
+    if not per_image:
+        axes.insert(0, 0)
+    return axes
+
+
+def gather_channels(*xs, indexes=None, **kwargs):
+    """Slice tensors along channels axis by given indexes"""
+    if indexes is None:
+        return xs
+    elif isinstance(indexes, (int)):
+        indexes = [indexes]
+    xs = [_gather_channels(x, indexes=indexes, **kwargs) for x in xs]
+    return xs
+
+
+def round_if_needed(x, threshold, **kwargs):
+    backend = kwargs['backend']
+    ops = kwargs['ops']
+    if threshold is not None:
+        x = ops.greater(x, threshold)
+        x = ops.cast(x, backend.floatx())
+    return x
+
+
+def average(x, per_image=False, class_weights=None, **kwargs):
+    ops = kwargs['ops']
+    if per_image:
+        x = ops.mean(x, axis=0)
+    if class_weights is not None:
+        x = x * class_weights
+    return ops.mean(x)
+
+
+# ----------------------------------------------------------------
+#   Metric Functions
+# ----------------------------------------------------------------
+
+def iou_score(gt, pr, class_weights=1., class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
+    r""" The `Jaccard index`_, also known as Intersection over Union and the Jaccard similarity coefficient
+    (originally coined coefficient de communauté by Paul Jaccard), is a statistic used for comparing the
+    similarity and diversity of sample sets. The Jaccard coefficient measures similarity between finite sample sets,
+    and is defined as the size of the intersection divided by the size of the union of the sample sets:
+
+    .. math:: J(A, B) = \frac{A \cap B}{A \cup B}
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        class_weights: 1. or list of class weights, len(weights) = C
+        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
+        smooth: value to avoid division by zero
+        per_image: if ``True``, metric is calculated as mean over images in batch (B),
+            else over whole batch
+        threshold: value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round
+
+    Returns:
+        IoU/Jaccard score in range [0, 1]
+
+    .. _`Jaccard index`: https://en.wikipedia.org/wiki/Jaccard_index
+
+    """
+
+    ops = kwargs['ops']
+
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+    pr = round_if_needed(pr, threshold, **kwargs)
+    axes = get_reduce_axes(per_image, **kwargs)
+
+    # score calculation
+    intersection = ops.sum(gt * pr, axis=axes)
+    union = ops.sum(gt + pr, axis=axes) - intersection
+
+    score = (intersection + smooth) / (union + smooth)
+    score = average(score, per_image, class_weights, **kwargs)
+
+    return score
+
+
+def f_score(gt, pr, beta=1, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None,
+            **kwargs):
+    r"""The F-score (Dice coefficient) can be interpreted as a weighted average of the precision and recall,
+    where an F-score reaches its best value at 1 and worst score at 0.
+    The relative contribution of ``precision`` and ``recall`` to the F1-score are equal.
+    The formula for the F score is:
+
+    .. math:: F_\beta(precision, recall) = (1 + \beta^2) \frac{precision \cdot recall}
+        {\beta^2 \cdot precision + recall}
+
+    The formula in terms of *Type I* and *Type II* errors:
+
+    .. math:: F_\beta(A, B) = \frac{(1 + \beta^2) TP} {(1 + \beta^2) TP + \beta^2 FN + FP}
+
+
+    where:
+        TP - true positive;
+        FP - false positive;
+        FN - false negative;
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        class_weights: 1. or list of class weights, len(weights) = C
+        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
+        beta: f-score coefficient
+        smooth: value to avoid division by zero
+        per_image: if ``True``, metric is calculated as mean over images in batch (B),
+            else over whole batch
+        threshold: value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round
+
+    Returns:
+        F-score in range [0, 1]
+
+    """
+
+    ops = kwargs['ops']
+
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+    pr = round_if_needed(pr, threshold, **kwargs)
+    axes = get_reduce_axes(per_image, **kwargs)
+
+    # calculate score
+    tp = ops.sum(gt * pr, axis=axes)
+    fp = ops.sum(pr, axis=axes) - tp
+    fn = ops.sum(gt, axis=axes) - tp
+
+    score = ((1 + beta ** 2) * tp + smooth) \
+            / ((1 + beta ** 2) * tp + beta ** 2 * fn + fp + smooth)
+    score = average(score, per_image, class_weights, **kwargs)
+
+    return score
+
+
+def precision(gt, pr, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
+    r"""Calculate precision between the ground truth (gt) and the prediction (pr).
+
+    .. math:: F_\beta(tp, fp) = \frac{tp} {(tp + fp)}
+
+    where:
+         - tp - true positives;
+         - fp - false positives;
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        class_weights: 1. or ``np.array`` of class weights (``len(weights) = num_classes``)
+        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
+        smooth: Float value to avoid division by zero.
+        per_image: If ``True``, metric is calculated as mean over images in batch (B),
+            else over whole batch.
+        threshold: Float value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round.
+        name: Optional string, if ``None`` default ``precision`` name is used.
+
+    Returns:
+        float: precision score
+    """
+    ops = kwargs['ops']
+
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+    pr = round_if_needed(pr, threshold, **kwargs)
+    axes = get_reduce_axes(per_image, **kwargs)
+
+    # score calculation
+    tp = ops.sum(gt * pr, axis=axes)
+    fp = ops.sum(pr, axis=axes) - tp
+    
+    score = (tp + smooth) / (tp + fp + smooth)
+    score = average(score, per_image, class_weights, **kwargs)
+
+    return score
+
+
+def recall(gt, pr, class_weights=1, class_indexes=None, smooth=SMOOTH, per_image=False, threshold=None, **kwargs):
+    r"""Calculate recall between the ground truth (gt) and the prediction (pr).
+
+    .. math:: F_\beta(tp, fn) = \frac{tp} {(tp + fn)}
+
+    where:
+         - tp - true positives;
+         - fp - false positives;
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        class_weights: 1. or ``np.array`` of class weights (``len(weights) = num_classes``)
+        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
+        smooth: Float value to avoid division by zero.
+        per_image: If ``True``, metric is calculated as mean over images in batch (B),
+            else over whole batch.
+        threshold: Float value to round predictions (use ``>`` comparison), if ``None`` prediction will not be round.
+        name: Optional string, if ``None`` default ``precision`` name is used.
+
+    Returns:
+        float: recall score
+    """
+    ops = kwargs['ops']
+
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+    pr = round_if_needed(pr, threshold, **kwargs)
+    axes = get_reduce_axes(per_image, **kwargs)
+
+    tp = ops.sum(gt * pr, axis=axes)
+    fn = ops.sum(gt, axis=axes) - tp
+
+    score = (tp + smooth) / (tp + fn + smooth)
+    score = average(score, per_image, class_weights, **kwargs)
+
+    return score
+
+
+# ----------------------------------------------------------------
+#   Loss Functions
+# ----------------------------------------------------------------
+
+def categorical_crossentropy(gt, pr, class_weights=1., class_indexes=None, **kwargs):
+    backend = kwargs['backend']
+    ops = kwargs['ops']
+
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+
+    # scale predictions so that the class probas of each sample sum to 1
+    axis = 4 if backend.image_data_format() == 'channels_last' else 1
+    pr /= ops.sum(pr, axis=axis, keepdims=True)
+
+    # clip to prevent NaN's and Inf's
+    pr = ops.clip(pr, backend.epsilon(), 1 - backend.epsilon())
+
+    # calculate loss
+    output = gt * ops.log(pr) * class_weights
+    return - ops.mean(output)
+
+
+def binary_crossentropy(gt, pr, **kwargs):
+    metrics = kwargs['metrics']
+    ops = kwargs['ops']
+    return ops.mean(metrics.binary_crossentropy(gt, pr))
+
+
+def categorical_focal_loss(gt, pr, gamma=2.0, alpha=0.25, class_indexes=None, **kwargs):
+    r"""Implementation of Focal Loss from the paper in multiclass classification
+
+    Formula:
+        loss = - gt * alpha * ((1 - pr)^gamma) * log(pr)
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        alpha: the same as weighting factor in balanced cross entropy, default 0.25
+        gamma: focusing parameter for modulating factor (1-p), default 2.0
+        class_indexes: Optional integer or list of integers, classes to consider, if ``None`` all classes are used.
+
+    """
+
+    backend = kwargs['backend']
+    ops = kwargs['ops']
+    gt, pr = gather_channels(gt, pr, indexes=class_indexes, **kwargs)
+
+    # clip to prevent NaN's and Inf's
+    pr = ops.clip(pr, backend.epsilon(), 1.0 - backend.epsilon())
+
+    # Calculate focal loss
+    loss = - gt * (alpha * ops.pow((1 - pr), gamma) * ops.log(pr))
+
+    return ops.mean(loss)
+
+
+def binary_focal_loss(gt, pr, gamma=2.0, alpha=0.25, **kwargs):
+    r"""Implementation of Focal Loss from the paper in binary classification
+
+    Formula:
+        loss = - gt * alpha * ((1 - pr)^gamma) * log(pr) \
+               - (1 - gt) * alpha * (pr^gamma) * log(1 - pr)
+
+    Args:
+        gt: ground truth 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        pr: prediction 4D keras tensor (B, H, W, C) or (B, C, H, W)
+        alpha: the same as weighting factor in balanced cross entropy, default 0.25
+        gamma: focusing parameter for modulating factor (1-p), default 2.0
+
+    """
+    backend = kwargs['backend']
+    ops = kwargs['ops']
+
+    # clip to prevent NaN's and Inf's
+    pr = ops.clip(pr, backend.epsilon(), 1.0 - backend.epsilon())
+
+    loss_1 = - gt * (alpha * ops.pow((1 - pr), gamma) * ops.log(pr))
+    loss_0 = - (1 - gt) * ((1 - alpha) * ops.pow((pr), gamma) * ops.log(1 - pr))
+    loss = ops.mean(loss_0 + loss_1)
+    return loss
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/base/objects.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/base/objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,130 @@
-class KerasObject:
-    _backend = None
-    _models = None
-    _layers = None
-    _utils = None
-
-    def __init__(self, name=None):
-        if (self.backend is None or
-                self.utils is None or
-                self.models is None or
-                self.layers is None):
-            raise RuntimeError('You cannot use `KerasObjects` with None submodules.')
-
-        self._name = name
-
-    @property
-    def __name__(self):
-        if self._name is None:
-            return self.__class__.__name__
-        return self._name
-
-    @property
-    def name(self):
-        return self.__name__
-
-    @name.setter
-    def name(self, name):
-        self._name = name
-
-    @classmethod
-    def set_submodules(cls, backend, layers, models, utils):
-        cls._backend = backend
-        cls._layers = layers
-        cls._models = models
-        cls._utils = utils
-
-    @property
-    def submodules(self):
-        return {
-            'backend': self.backend,
-            'layers': self.layers,
-            'models': self.models,
-            'utils': self.utils,
-        }
-
-    @property
-    def backend(self):
-        return self._backend
-
-    @property
-    def layers(self):
-        return self._layers
-
-    @property
-    def models(self):
-        return self._models
-
-    @property
-    def utils(self):
-        return self._utils
-
-
-class Metric(KerasObject):
-    pass
-
-
-class Loss(KerasObject):
-
-    def __add__(self, other):
-        if isinstance(other, Loss):
-            return SumOfLosses(self, other)
-        else:
-            raise ValueError('Loss should be inherited from `Loss` class')
-
-    def __radd__(self, other):
-        return self.__add__(other)
-
-    def __mul__(self, value):
-        if isinstance(value, (int, float)):
-            return MultipliedLoss(self, value)
-        else:
-            raise ValueError('Loss should be inherited from `BaseLoss` class')
-
-    def __rmul__(self, other):
-        return self.__mul__(other)
-
-
-class MultipliedLoss(Loss):
-
-    def __init__(self, loss, multiplier):
-
-        # resolve name
-        if len(loss.__name__.split('+')) > 1:
-            name = '{}({})'.format(multiplier, loss.__name__)
-        else:
-            name = '{}{}'.format(multiplier, loss.__name__)
-        super().__init__(name=name)
-        self.loss = loss
-        self.multiplier = multiplier
-
-    def __call__(self, gt, pr):
-        return self.multiplier * self.loss(gt, pr)
-
-
-class SumOfLosses(Loss):
-
-    def __init__(self, l1, l2):
-        name = '{}_plus_{}'.format(l1.__name__, l2.__name__)
-        super().__init__(name=name)
-        self.l1 = l1
-        self.l2 = l2
-
-    def __call__(self, gt, pr):
-        return self.l1(gt, pr) + self.l2(gt, pr)
+class KerasObject:
+    _backend = None
+    _models = None
+    _layers = None
+    _utils = None
+    _ops = None
+    _metrics = None
+
+    def __init__(self, name=None):
+        if (self.backend is None or
+                self.utils is None or
+                self.models is None or
+                self.layers is None or
+                self.ops is None or
+                self.metrics is None):
+            raise RuntimeError('You cannot use `KerasObjects` with None submodules.')
+
+        self._name = name
+
+    @property
+    def __name__(self):
+        if self._name is None:
+            return self.__class__.__name__
+        return self._name
+
+    @property
+    def name(self):
+        return self.__name__
+
+    @name.setter
+    def name(self, name):
+        self._name = name
+
+    @classmethod
+    def set_submodules(cls, backend, layers, models, utils, ops, metrics):
+        cls._backend = backend
+        cls._layers = layers
+        cls._models = models
+        cls._utils = utils
+        cls._ops = ops
+        cls._metrics = metrics
+
+    @property
+    def submodules(self):
+        return {
+            'backend': self.backend,
+            'layers': self.layers,
+            'models': self.models,
+            'utils': self.utils,
+            'ops': self.ops,
+            'metrics': self.metrics
+        }
+
+    @property
+    def backend(self):
+        return self._backend
+
+    @property
+    def layers(self):
+        return self._layers
+
+    @property
+    def models(self):
+        return self._models
+
+    @property
+    def utils(self):
+        return self._utils
+
+    @property
+    def ops(self):
+        return self._ops
+
+    @property
+    def metrics(self):
+        return self._metrics
+
+
+class Metric(KerasObject):
+    pass
+
+
+class Loss(KerasObject):
+
+    def __add__(self, other):
+        if isinstance(other, Loss):
+            return SumOfLosses(self, other)
+        else:
+            raise ValueError('Loss should be inherited from `Loss` class')
+
+    def __radd__(self, other):
+        return self.__add__(other)
+
+    def __mul__(self, value):
+        if isinstance(value, (int, float)):
+            return MultipliedLoss(self, value)
+        else:
+            raise ValueError('Loss should be inherited from `BaseLoss` class')
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
+
+class MultipliedLoss(Loss):
+
+    def __init__(self, loss, multiplier):
+
+        # resolve name
+        if len(loss.__name__.split('+')) > 1:
+            name = '{}({})'.format(multiplier, loss.__name__)
+        else:
+            name = '{}{}'.format(multiplier, loss.__name__)
+        super().__init__(name=name)
+        self.loss = loss
+        self.multiplier = multiplier
+
+    def __call__(self, gt, pr):
+        return self.multiplier * self.loss(gt, pr)
+
+
+class SumOfLosses(Loss):
+
+    def __init__(self, l1, l2):
+        name = '{}_plus_{}'.format(l1.__name__, l2.__name__)
+        super().__init__(name=name)
+        self.l1 = l1
+        self.l2 = l2
+
+    def __call__(self, gt, pr):
+        return self.l1(gt, pr) + self.l2(gt, pr)
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/losses.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/losses.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/metrics.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/metrics.py`

 * *Files identical despite different names*

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/models/fpn.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/models/fpn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,256 +1,257 @@
-from keras_applications import get_submodules_from_kwargs
-
-from ._common_blocks import Conv3dBn
-from ._utils import freeze_model
-from ..backbones.backbones_factory import Backbones
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-# ---------------------------------------------------------------------
-#  Utility functions
-# ---------------------------------------------------------------------
-
-def get_submodules():
-    return {
-        'backend': backend,
-        'models': models,
-        'layers': layers,
-        'utils': keras_utils,
-    }
-
-
-# ---------------------------------------------------------------------
-#  Blocks
-# ---------------------------------------------------------------------
-
-def Conv3x3BnReLU(filters, use_batchnorm, name=None):
-    kwargs = get_submodules()
-
-    def wrapper(input_tensor):
-        return Conv3dBn(
-            filters,
-            kernel_size=3,
-            activation='relu',
-            kernel_initializer='he_uniform',
-            padding='same',
-            use_batchnorm=use_batchnorm,
-            name=name,
-            **kwargs
-        )(input_tensor)
-
-    return wrapper
-
-
-def DoubleConv3x3BnReLU(filters, use_batchnorm, name=None):
-    name1, name2 = None, None
-    if name is not None:
-        name1 = name + 'a'
-        name2 = name + 'b'
-
-    def wrapper(input_tensor):
-        x = Conv3x3BnReLU(filters, use_batchnorm, name=name1)(input_tensor)
-        x = Conv3x3BnReLU(filters, use_batchnorm, name=name2)(x)
-        return x
-
-    return wrapper
-
-
-def FPNBlock(pyramid_filters, stage):
-    conv0_name = 'fpn_stage_p{}_pre_conv'.format(stage)
-    conv1_name = 'fpn_stage_p{}_conv'.format(stage)
-    add_name = 'fpn_stage_p{}_add'.format(stage)
-    up_name = 'fpn_stage_p{}_upsampling'.format(stage)
-
-    channels_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    def wrapper(input_tensor, skip):
-        # if input tensor channels not equal to pyramid channels
-        # we will not be able to sum input tensor and skip
-        # so add extra conv layer to transform it
-        input_filters = backend.int_shape(input_tensor)[channels_axis]
-        if input_filters != pyramid_filters:
-            input_tensor = layers.Conv3D(
-                filters=pyramid_filters,
-                kernel_size=(1, 1, 1),
-                kernel_initializer='he_uniform',
-                name=conv0_name,
-            )(input_tensor)
-
-        skip = layers.Conv3D(
-            filters=pyramid_filters,
-            kernel_size=(1, 1, 1),
-            kernel_initializer='he_uniform',
-            name=conv1_name,
-        )(skip)
-
-        x = layers.UpSampling3D((2, 2, 2), name=up_name)(input_tensor)
-        x = layers.Add(name=add_name)([x, skip])
-
-        return x
-
-    return wrapper
-
-
-# ---------------------------------------------------------------------
-#  FPN Decoder
-# ---------------------------------------------------------------------
-
-def build_fpn(
-        backbone,
-        skip_connection_layers,
-        pyramid_filters=256,
-        segmentation_filters=128,
-        classes=1,
-        activation='sigmoid',
-        use_batchnorm=True,
-        aggregation='sum',
-        dropout=None,
-):
-    # from keras.layers import UpSampling3D
-    input_ = backbone.input
-    x = backbone.output
-
-    # building decoder blocks with skip connections
-    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
-              else backbone.get_layer(index=i).output for i in skip_connection_layers])
-
-    # build FPN pyramid
-    p5 = FPNBlock(pyramid_filters, stage=5)(x, skips[0])
-    p4 = FPNBlock(pyramid_filters, stage=4)(p5, skips[1])
-    p3 = FPNBlock(pyramid_filters, stage=3)(p4, skips[2])
-    p2 = FPNBlock(pyramid_filters, stage=2)(p3, skips[3])
-
-    # add segmentation head to each
-    s5 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage5')(p5)
-    s4 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage4')(p4)
-    s3 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage3')(p3)
-    s2 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage2')(p2)
-
-    # upsampling to same resolution
-    s5 = layers.UpSampling3D((8, 8, 8), name='upsampling_stage5')(s5)
-    s4 = layers.UpSampling3D((4, 4, 4), name='upsampling_stage4')(s4)
-    s3 = layers.UpSampling3D((2, 2, 2), name='upsampling_stage3')(s3)
-
-    # aggregating results
-    if aggregation == 'sum':
-        x = layers.Add(name='aggregation_sum')([s2, s3, s4, s5])
-    elif aggregation == 'concat':
-        concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-        x = layers.Concatenate(axis=concat_axis, name='aggregation_concat')([s2, s3, s4, s5])
-    else:
-        raise ValueError('Aggregation parameter should be in ("sum", "concat"), '
-                         'got {}'.format(aggregation))
-
-    if dropout:
-        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
-
-    # final stage
-    x = Conv3x3BnReLU(segmentation_filters, use_batchnorm, name='final_stage')(x)
-    # x = layers.UpSampling3D(size=(2, 2, 2), interpolation='bilinear', name='final_upsampling')(x)
-    # TODO: Find how to make bilinear interpolation in 3D
-    x = layers.UpSampling3D(size=(2, 2, 2), name='final_upsampling')(x)
-
-    # model head (define number of output classes)
-    x = layers.Conv3D(
-        filters=classes,
-        kernel_size=(3, 3, 3),
-        padding='same',
-        use_bias=True,
-        kernel_initializer='glorot_uniform',
-        name='head_conv',
-    )(x)
-    x = layers.Activation(activation, name=activation)(x)
-
-    # create keras model instance
-    model = models.Model(input_, x)
-
-    return model
-
-
-# ---------------------------------------------------------------------
-#  FPN Model
-# ---------------------------------------------------------------------
-
-def FPN(
-        backbone_name='vgg16',
-        input_shape=(None, None, None, 3),
-        classes=21,
-        activation='softmax',
-        weights=None,
-        encoder_weights='imagenet',
-        encoder_freeze=False,
-        encoder_features='default',
-        pyramid_block_filters=256,
-        pyramid_use_batchnorm=True,
-        pyramid_aggregation='concat',
-        pyramid_dropout=None,
-        **kwargs
-):
-    """FPN_ is a fully convolution neural network for image semantic segmentation
-
-    Args:
-        backbone_name: name of classification model (without last dense layers) used as feature
-                extractor to build segmentation model.
-        input_shape: shape of input data/image ``(H, W, C)``, in general
-                case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
-                able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
-        classes: a number of classes for output (output shape - ``(h, w, classes)``).
-        weights: optional, path to model weights.
-        activation: name of one of ``keras.activations`` for last model layer (e.g. ``sigmoid``, ``softmax``, ``linear``).
-        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
-        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
-        encoder_features: a list of layer numbers or names starting from top of the model.
-                Each of these layers will be used to build features pyramid. If ``default`` is used
-                layer names are taken from ``DEFAULT_FEATURE_PYRAMID_LAYERS``.
-        pyramid_block_filters: a number of filters in Feature Pyramid Block of FPN_.
-        pyramid_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
-                is used.
-        pyramid_aggregation: one of 'sum' or 'concat'. The way to aggregate pyramid blocks.
-        pyramid_dropout: spatial dropout rate for feature pyramid in range (0, 1).
-
-    Returns:
-        ``keras.models.Model``: **FPN**
-
-    .. _FPN:
-        http://presentations.cocodataset.org/COCO17-Stuff-FAIR.pdf
-
-    """
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    backbone = Backbones.get_backbone(
-        backbone_name,
-        input_shape=input_shape,
-        weights=encoder_weights,
-        include_top=False,
-        **kwargs,
-    )
-
-    if encoder_features == 'default':
-        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
-
-    model = build_fpn(
-        backbone=backbone,
-        skip_connection_layers=encoder_features,
-        pyramid_filters=pyramid_block_filters,
-        segmentation_filters=pyramid_block_filters // 2,
-        use_batchnorm=pyramid_use_batchnorm,
-        dropout=pyramid_dropout,
-        activation=activation,
-        classes=classes,
-        aggregation=pyramid_aggregation,
-    )
-
-    # lock encoder weights for fine-tuning
-    if encoder_freeze:
-        freeze_model(backbone, **kwargs)
-
-    # loading model weights
-    if weights is not None:
-        model.load_weights(weights)
-
-    return model
+from .. import get_submodules_from_kwargs
+
+from ._common_blocks import Conv3dBn
+from ._utils import freeze_model
+from ..backbones.backbones_factory import Backbones
+from keras.src.legacy.backend import int_shape
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+# ---------------------------------------------------------------------
+#  Utility functions
+# ---------------------------------------------------------------------
+
+def get_submodules():
+    return {
+        'backend': backend,
+        'models': models,
+        'layers': layers,
+        'utils': keras_utils,
+    }
+
+
+# ---------------------------------------------------------------------
+#  Blocks
+# ---------------------------------------------------------------------
+
+def Conv3x3BnReLU(filters, use_batchnorm, name=None):
+    kwargs = get_submodules()
+
+    def wrapper(input_tensor):
+        return Conv3dBn(
+            filters,
+            kernel_size=3,
+            activation='relu',
+            kernel_initializer='he_uniform',
+            padding='same',
+            use_batchnorm=use_batchnorm,
+            name=name,
+            **kwargs
+        )(input_tensor)
+
+    return wrapper
+
+
+def DoubleConv3x3BnReLU(filters, use_batchnorm, name=None):
+    name1, name2 = None, None
+    if name is not None:
+        name1 = name + 'a'
+        name2 = name + 'b'
+
+    def wrapper(input_tensor):
+        x = Conv3x3BnReLU(filters, use_batchnorm, name=name1)(input_tensor)
+        x = Conv3x3BnReLU(filters, use_batchnorm, name=name2)(x)
+        return x
+
+    return wrapper
+
+
+def FPNBlock(pyramid_filters, stage):
+    conv0_name = 'fpn_stage_p{}_pre_conv'.format(stage)
+    conv1_name = 'fpn_stage_p{}_conv'.format(stage)
+    add_name = 'fpn_stage_p{}_add'.format(stage)
+    up_name = 'fpn_stage_p{}_upsampling'.format(stage)
+
+    channels_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    def wrapper(input_tensor, skip):
+        # if input tensor channels not equal to pyramid channels
+        # we will not be able to sum input tensor and skip
+        # so add extra conv layer to transform it
+        input_filters = int_shape(input_tensor)[channels_axis]
+        if input_filters != pyramid_filters:
+            input_tensor = layers.Conv3D(
+                filters=pyramid_filters,
+                kernel_size=(1, 1, 1),
+                kernel_initializer='he_uniform',
+                name=conv0_name,
+            )(input_tensor)
+
+        skip = layers.Conv3D(
+            filters=pyramid_filters,
+            kernel_size=(1, 1, 1),
+            kernel_initializer='he_uniform',
+            name=conv1_name,
+        )(skip)
+
+        x = layers.UpSampling3D((2, 2, 2), name=up_name)(input_tensor)
+        x = layers.Add(name=add_name)([x, skip])
+
+        return x
+
+    return wrapper
+
+
+# ---------------------------------------------------------------------
+#  FPN Decoder
+# ---------------------------------------------------------------------
+
+def build_fpn(
+        backbone,
+        skip_connection_layers,
+        pyramid_filters=256,
+        segmentation_filters=128,
+        classes=1,
+        activation='sigmoid',
+        use_batchnorm=True,
+        aggregation='sum',
+        dropout=None,
+):
+    # from keras.layers import UpSampling3D
+    input_ = backbone.input
+    x = backbone.output
+
+    # building decoder blocks with skip connections
+    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
+              else backbone.get_layer(index=i).output for i in skip_connection_layers])
+
+    # build FPN pyramid
+    p5 = FPNBlock(pyramid_filters, stage=5)(x, skips[0])
+    p4 = FPNBlock(pyramid_filters, stage=4)(p5, skips[1])
+    p3 = FPNBlock(pyramid_filters, stage=3)(p4, skips[2])
+    p2 = FPNBlock(pyramid_filters, stage=2)(p3, skips[3])
+
+    # add segmentation head to each
+    s5 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage5')(p5)
+    s4 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage4')(p4)
+    s3 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage3')(p3)
+    s2 = DoubleConv3x3BnReLU(segmentation_filters, use_batchnorm, name='segm_stage2')(p2)
+
+    # upsampling to same resolution
+    s5 = layers.UpSampling3D((8, 8, 8), name='upsampling_stage5')(s5)
+    s4 = layers.UpSampling3D((4, 4, 4), name='upsampling_stage4')(s4)
+    s3 = layers.UpSampling3D((2, 2, 2), name='upsampling_stage3')(s3)
+
+    # aggregating results
+    if aggregation == 'sum':
+        x = layers.Add(name='aggregation_sum')([s2, s3, s4, s5])
+    elif aggregation == 'concat':
+        concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+        x = layers.Concatenate(axis=concat_axis, name='aggregation_concat')([s2, s3, s4, s5])
+    else:
+        raise ValueError('Aggregation parameter should be in ("sum", "concat"), '
+                         'got {}'.format(aggregation))
+
+    if dropout:
+        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
+
+    # final stage
+    x = Conv3x3BnReLU(segmentation_filters, use_batchnorm, name='final_stage')(x)
+    # x = layers.UpSampling3D(size=(2, 2, 2), interpolation='bilinear', name='final_upsampling')(x)
+    # TODO: Find how to make bilinear interpolation in 3D
+    x = layers.UpSampling3D(size=(2, 2, 2), name='final_upsampling')(x)
+
+    # model head (define number of output classes)
+    x = layers.Conv3D(
+        filters=classes,
+        kernel_size=(3, 3, 3),
+        padding='same',
+        use_bias=True,
+        kernel_initializer='glorot_uniform',
+        name='head_conv',
+    )(x)
+    x = layers.Activation(activation, name=activation)(x)
+
+    # create keras model instance
+    model = models.Model(input_, x)
+
+    return model
+
+
+# ---------------------------------------------------------------------
+#  FPN Model
+# ---------------------------------------------------------------------
+
+def FPN(
+        backbone_name='vgg16',
+        input_shape=(None, None, None, 3),
+        classes=21,
+        activation='softmax',
+        weights=None,
+        encoder_weights='imagenet',
+        encoder_freeze=False,
+        encoder_features='default',
+        pyramid_block_filters=256,
+        pyramid_use_batchnorm=True,
+        pyramid_aggregation='concat',
+        pyramid_dropout=None,
+        **kwargs
+):
+    """FPN_ is a fully convolution neural network for image semantic segmentation
+
+    Args:
+        backbone_name: name of classification model (without last dense layers) used as feature
+                extractor to build segmentation model.
+        input_shape: shape of input data/image ``(H, W, C)``, in general
+                case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
+                able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
+        classes: a number of classes for output (output shape - ``(h, w, classes)``).
+        weights: optional, path to model weights.
+        activation: name of one of ``keras.activations`` for last model layer (e.g. ``sigmoid``, ``softmax``, ``linear``).
+        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
+        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
+        encoder_features: a list of layer numbers or names starting from top of the model.
+                Each of these layers will be used to build features pyramid. If ``default`` is used
+                layer names are taken from ``DEFAULT_FEATURE_PYRAMID_LAYERS``.
+        pyramid_block_filters: a number of filters in Feature Pyramid Block of FPN_.
+        pyramid_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
+                is used.
+        pyramid_aggregation: one of 'sum' or 'concat'. The way to aggregate pyramid blocks.
+        pyramid_dropout: spatial dropout rate for feature pyramid in range (0, 1).
+
+    Returns:
+        ``keras.models.Model``: **FPN**
+
+    .. _FPN:
+        http://presentations.cocodataset.org/COCO17-Stuff-FAIR.pdf
+
+    """
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils, _, _ = get_submodules_from_kwargs(kwargs)
+
+    backbone = Backbones.get_backbone(
+        backbone_name,
+        input_shape=input_shape,
+        weights=encoder_weights,
+        include_top=False,
+        **kwargs,
+    )
+
+    if encoder_features == 'default':
+        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
+
+    model = build_fpn(
+        backbone=backbone,
+        skip_connection_layers=encoder_features,
+        pyramid_filters=pyramid_block_filters,
+        segmentation_filters=pyramid_block_filters // 2,
+        use_batchnorm=pyramid_use_batchnorm,
+        dropout=pyramid_dropout,
+        activation=activation,
+        classes=classes,
+        aggregation=pyramid_aggregation,
+    )
+
+    # lock encoder weights for fine-tuning
+    if encoder_freeze:
+        freeze_model(backbone, **kwargs)
+
+    # loading model weights
+    if weights is not None:
+        model.load_weights(weights)
+
+    return model
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/models/linknet.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/models/unet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,282 +1,257 @@
-from keras_applications import get_submodules_from_kwargs
-
-from ._common_blocks import Conv3dBn
-from ._utils import freeze_model
-from ..backbones.backbones_factory import Backbones
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-# ---------------------------------------------------------------------
-#  Utility functions
-# ---------------------------------------------------------------------
-
-def get_submodules():
-    return {
-        'backend': backend,
-        'models': models,
-        'layers': layers,
-        'utils': keras_utils,
-    }
-
-
-# ---------------------------------------------------------------------
-#  Blocks
-# ---------------------------------------------------------------------
-
-def Conv3x3BnReLU(filters, use_batchnorm, name=None):
-    kwargs = get_submodules()
-
-    def wrapper(input_tensor):
-        return Conv3dBn(
-            filters,
-            kernel_size=3,
-            activation='relu',
-            kernel_initializer='he_uniform',
-            padding='same',
-            use_batchnorm=use_batchnorm,
-            name=name,
-            **kwargs
-        )(input_tensor)
-
-    return wrapper
-
-
-def Conv1x1BnReLU(filters, use_batchnorm, name=None):
-    kwargs = get_submodules()
-
-    def wrapper(input_tensor):
-        return Conv3dBn(
-            filters,
-            kernel_size=1,
-            activation='relu',
-            kernel_initializer='he_uniform',
-            padding='same',
-            use_batchnorm=use_batchnorm,
-            name=name,
-            **kwargs
-        )(input_tensor)
-
-    return wrapper
-
-
-def DecoderUpsamplingX2Block(filters, stage, use_batchnorm):
-    conv_block1_name = 'decoder_stage{}a'.format(stage)
-    conv_block2_name = 'decoder_stage{}b'.format(stage)
-    conv_block3_name = 'decoder_stage{}c'.format(stage)
-    up_name = 'decoder_stage{}_upsampling'.format(stage)
-    add_name = 'decoder_stage{}_add'.format(stage)
-
-    channels_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    def wrapper(input_tensor, skip=None):
-        input_filters = backend.int_shape(input_tensor)[channels_axis]
-        output_filters = backend.int_shape(skip)[channels_axis] if skip is not None else filters
-
-        x = Conv1x1BnReLU(input_filters // 4, use_batchnorm, name=conv_block1_name)(input_tensor)
-        x = layers.UpSampling3D((2, 2, 2), name=up_name)(x)
-        x = Conv3x3BnReLU(input_filters // 4, use_batchnorm, name=conv_block2_name)(x)
-        x = Conv1x1BnReLU(output_filters, use_batchnorm, name=conv_block3_name)(x)
-
-        if skip is not None:
-            x = layers.Add(name=add_name)([x, skip])
-        return x
-
-    return wrapper
-
-
-def DecoderTransposeX2Block(filters, stage, use_batchnorm):
-    conv_block1_name = 'decoder_stage{}a'.format(stage)
-    transpose_name = 'decoder_stage{}b_transpose'.format(stage)
-    bn_name = 'decoder_stage{}b_bn'.format(stage)
-    relu_name = 'decoder_stage{}b_relu'.format(stage)
-    conv_block3_name = 'decoder_stage{}c'.format(stage)
-    add_name = 'decoder_stage{}_add'.format(stage)
-
-    channels_axis = bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    def wrapper(input_tensor, skip=None):
-        input_filters = backend.int_shape(input_tensor)[channels_axis]
-        output_filters = backend.int_shape(skip)[channels_axis] if skip is not None else filters
-
-        x = Conv1x1BnReLU(input_filters // 4, use_batchnorm, name=conv_block1_name)(input_tensor)
-        x = layers.Conv3DTranspose(
-            filters=input_filters // 4,
-            kernel_size=(4, 4, 4),
-            strides=(2, 2, 2),
-            padding='same',
-            name=transpose_name,
-            use_bias=not use_batchnorm,
-        )(x)
-
-        if use_batchnorm:
-            x = layers.BatchNormalization(axis=bn_axis, name=bn_name)(x)
-
-        x = layers.Activation('relu', name=relu_name)(x)
-        x = Conv1x1BnReLU(output_filters, use_batchnorm, name=conv_block3_name)(x)
-
-        if skip is not None:
-            x = layers.Add(name=add_name)([x, skip])
-
-        return x
-
-    return wrapper
-
-
-# ---------------------------------------------------------------------
-#  LinkNet Decoder
-# ---------------------------------------------------------------------
-
-def build_linknet(
-        backbone,
-        decoder_block,
-        skip_connection_layers,
-        decoder_filters=(256, 128, 64, 32, 16),
-        n_upsample_blocks=5,
-        classes=1,
-        activation='sigmoid',
-        use_batchnorm=True,
-        dropout=None,
-):
-    input_ = backbone.input
-    x = backbone.output
-
-    # extract skip connections
-    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
-              else backbone.get_layer(index=i).output for i in skip_connection_layers])
-
-    # add center block if previous operation was maxpooling (for vgg models)
-    if isinstance(backbone.layers[-1], layers.MaxPooling2D):
-        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block1')(x)
-        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block2')(x)
-
-    # building decoder blocks
-    for i in range(n_upsample_blocks):
-
-        if i < len(skips):
-            skip = skips[i]
-        else:
-            skip = None
-
-        x = decoder_block(decoder_filters[i], stage=i, use_batchnorm=use_batchnorm)(x, skip)
-
-    if dropout:
-        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
-
-    # model head (define number of output classes)
-    x = layers.Conv3D(
-        filters=classes,
-        kernel_size=(3, 3, 3),
-        padding='same',
-        use_bias=True,
-        kernel_initializer='glorot_uniform'
-    )(x)
-    x = layers.Activation(activation, name=activation)(x)
-
-    # create keras model instance
-    model = models.Model(input_, x)
-
-    return model
-
-
-# ---------------------------------------------------------------------
-#  LinkNet Model
-# ---------------------------------------------------------------------
-
-def Linknet(
-        backbone_name='vgg16',
-        input_shape=(None, None, 3),
-        classes=1,
-        activation='sigmoid',
-        weights=None,
-        encoder_weights='imagenet',
-        encoder_freeze=False,
-        encoder_features='default',
-        decoder_block_type='upsampling',
-        decoder_filters=(None, None, None, None, 16),
-        decoder_use_batchnorm=True,
-        dropout=None,
-        **kwargs
-):
-    """Linknet_ is a fully convolution neural network for fast image semantic segmentation
-
-    Note:
-        This implementation by default has 4 skip connections (original - 3).
-
-    Args:
-        backbone_name: name of classification model (without last dense layers) used as feature
-                    extractor to build segmentation model.
-        input_shape: shape of input data/image ``(H, W, C)``, in general
-                case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
-                able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
-        classes: a number of classes for output (output shape - ``(h, w, classes)``).
-        activation: name of one of ``keras.activations`` for last model layer
-            (e.g. ``sigmoid``, ``softmax``, ``linear``).
-        weights: optional, path to model weights.
-        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
-        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
-        encoder_features: a list of layer numbers or names starting from top of the model.
-                    Each of these layers will be concatenated with corresponding decoder block. If ``default`` is used
-                    layer names are taken from ``DEFAULT_SKIP_CONNECTIONS``.
-        decoder_filters: list of numbers of ``Conv2D`` layer filters in decoder blocks,
-            for block with skip connection a number of filters is equal to number of filters in
-            corresponding encoder block (estimates automatically and can be passed as ``None`` value).
-        decoder_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
-                    is used.
-        decoder_block_type: one of
-                    - `upsampling`:  use ``UpSampling2D`` keras layer
-                    - `transpose`:   use ``Transpose2D`` keras layer
-
-    Returns:
-        ``keras.models.Model``: **Linknet**
-
-    .. _Linknet:
-        https://arxiv.org/pdf/1707.03718.pdf
-    """
-
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if decoder_block_type == 'upsampling':
-        decoder_block = DecoderUpsamplingX2Block
-    elif decoder_block_type == 'transpose':
-        decoder_block = DecoderTransposeX2Block
-    else:
-        raise ValueError('Decoder block type should be in ("upsampling", "transpose"). '
-                         'Got: {}'.format(decoder_block_type))
-
-    backbone = Backbones.get_backbone(
-        backbone_name,
-        input_shape=input_shape,
-        weights=encoder_weights,
-        include_top=False,
-        **kwargs,
-    )
-
-    if encoder_features == 'default':
-        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
-
-    model = build_linknet(
-        backbone=backbone,
-        decoder_block=decoder_block,
-        skip_connection_layers=encoder_features,
-        decoder_filters=decoder_filters,
-        classes=classes,
-        activation=activation,
-        n_upsample_blocks=len(decoder_filters),
-        use_batchnorm=decoder_use_batchnorm,
-        dropout=dropout,
-    )
-
-    # lock encoder weights for fine-tuning
-    if encoder_freeze:
-        freeze_model(backbone, **kwargs)
-
-    # loading model weights
-    if weights is not None:
-        model.load_weights(weights)
-
-    return model
+from .. import get_submodules_from_kwargs
+
+from ._common_blocks import Conv3dBn
+from ._utils import freeze_model
+from ..backbones.backbones_factory import Backbones
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+# ---------------------------------------------------------------------
+#  Utility functions
+# ---------------------------------------------------------------------
+
+def get_submodules():
+    return {
+        'backend': backend,
+        'models': models,
+        'layers': layers,
+        'utils': keras_utils,
+    }
+
+
+# ---------------------------------------------------------------------
+#  Blocks
+# ---------------------------------------------------------------------
+
+def Conv3x3BnReLU(filters, use_batchnorm, name=None):
+    kwargs = get_submodules()
+
+    def wrapper(input_tensor):
+        return Conv3dBn(
+            filters,
+            kernel_size=3,
+            activation='relu',
+            kernel_initializer='he_uniform',
+            padding='same',
+            use_batchnorm=use_batchnorm,
+            name=name,
+            **kwargs
+        )(input_tensor)
+
+    return wrapper
+
+
+def DecoderUpsamplingX2Block(filters, stage, use_batchnorm=False):
+    up_name = 'decoder_stage{}_upsampling'.format(stage)
+    conv1_name = 'decoder_stage{}a'.format(stage)
+    conv2_name = 'decoder_stage{}b'.format(stage)
+    concat_name = 'decoder_stage{}_concat'.format(stage)
+
+    concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    def wrapper(input_tensor, skip=None):
+        x = layers.UpSampling3D(size=2, name=up_name)(input_tensor)
+
+        if skip is not None:
+            x = layers.Concatenate(axis=concat_axis, name=concat_name)([x, skip])
+
+        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv1_name)(x)
+        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv2_name)(x)
+
+        return x
+
+    return wrapper
+
+
+def DecoderTransposeX2Block(filters, stage, use_batchnorm=False):
+    transp_name = 'decoder_stage{}a_transpose'.format(stage)
+    bn_name = 'decoder_stage{}a_bn'.format(stage)
+    relu_name = 'decoder_stage{}a_relu'.format(stage)
+    conv_block_name = 'decoder_stage{}b'.format(stage)
+    concat_name = 'decoder_stage{}_concat'.format(stage)
+
+    concat_axis = bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    def layer(input_tensor, skip=None):
+
+        x = layers.Conv3DTranspose(
+            filters,
+            kernel_size=(4, 4, 4),
+            strides=(2, 2, 2),
+            padding='same',
+            name=transp_name,
+            use_bias=not use_batchnorm,
+        )(input_tensor)
+
+        if use_batchnorm:
+            x = layers.BatchNormalization(axis=bn_axis, name=bn_name)(x)
+
+        x = layers.Activation('relu', name=relu_name)(x)
+
+        if skip is not None:
+            x = layers.Concatenate(axis=concat_axis, name=concat_name)([x, skip])
+
+        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv_block_name)(x)
+
+        return x
+
+    return layer
+
+
+# ---------------------------------------------------------------------
+#  Unet Decoder
+# ---------------------------------------------------------------------
+
+def build_unet(
+        backbone,
+        decoder_block,
+        skip_connection_layers,
+        decoder_filters=(256, 128, 64, 32, 16),
+        n_upsample_blocks=5,
+        classes=1,
+        activation='sigmoid',
+        use_batchnorm=True,
+        dropout=None,
+):
+    input_ = backbone.input
+    x = backbone.output
+
+    # extract skip connections
+    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
+              else backbone.get_layer(index=i).output for i in skip_connection_layers])
+
+    # add center block if previous operation was maxpooling (for vgg models)
+    if isinstance(backbone.layers[-1], layers.MaxPooling3D):
+        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block1')(x)
+        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block2')(x)
+
+    # building decoder blocks
+    for i in range(n_upsample_blocks):
+
+        if i < len(skips):
+            skip = skips[i]
+        else:
+            skip = None
+
+        x = decoder_block(decoder_filters[i], stage=i, use_batchnorm=use_batchnorm)(x, skip)
+
+    if dropout:
+        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
+
+    # model head (define number of output classes)
+    x = layers.Conv3D(
+        filters=classes,
+        kernel_size=(3, 3, 3),
+        padding='same',
+        use_bias=True,
+        kernel_initializer='glorot_uniform',
+        name='final_conv',
+    )(x)
+    x = layers.Activation(activation, name=activation)(x)
+
+    # create keras model instance
+    model = models.Model(input_, x)
+
+    return model
+
+
+# ---------------------------------------------------------------------
+#  Unet Model
+# ---------------------------------------------------------------------
+
+def Unet(
+        backbone_name='vgg16',
+        input_shape=(None, None, 3),
+        classes=1,
+        activation='sigmoid',
+        weights=None,
+        encoder_weights='imagenet',
+        encoder_freeze=False,
+        encoder_features='default',
+        decoder_block_type='upsampling',
+        decoder_filters=(256, 128, 64, 32, 16),
+        decoder_use_batchnorm=True,
+        dropout=None,
+        **kwargs
+):
+    """ Unet_ is a fully convolution neural network for image semantic segmentation
+
+    Args:
+        backbone_name: name of classification model (without last dense layers) used as feature
+            extractor to build segmentation model.
+        input_shape: shape of input data/image ``(H, W, C)``, in general
+            case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
+            able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
+        classes: a number of classes for output (output shape - ``(h, w, classes)``).
+        activation: name of one of ``keras.activations`` for last model layer
+            (e.g. ``sigmoid``, ``softmax``, ``linear``).
+        weights: optional, path to model weights.
+        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
+        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
+        encoder_features: a list of layer numbers or names starting from top of the model.
+            Each of these layers will be concatenated with corresponding decoder block. If ``default`` is used
+            layer names are taken from ``DEFAULT_SKIP_CONNECTIONS``.
+        decoder_block_type: one of blocks with following layers structure:
+
+            - `upsampling`:  ``UpSampling2D`` -> ``Conv2D`` -> ``Conv2D``
+            - `transpose`:   ``Transpose2D`` -> ``Conv2D``
+
+        decoder_filters: list of numbers of ``Conv2D`` layer filters in decoder blocks
+        decoder_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
+            is used.
+
+    Returns:
+        ``keras.models.Model``: **Unet**
+
+    .. _Unet:
+        https://arxiv.org/pdf/1505.04597
+
+    """
+
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils, _, _ = get_submodules_from_kwargs(kwargs)
+
+    if decoder_block_type == 'upsampling':
+        decoder_block = DecoderUpsamplingX2Block
+    elif decoder_block_type == 'transpose':
+        decoder_block = DecoderTransposeX2Block
+    else:
+        raise ValueError('Decoder block type should be in ("upsampling", "transpose"). '
+                         'Got: {}'.format(decoder_block_type))
+
+    backbone = Backbones.get_backbone(
+        backbone_name,
+        input_shape=input_shape,
+        weights=encoder_weights,
+        include_top=False,
+        **kwargs,
+    )
+
+    if encoder_features == 'default':
+        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
+
+    model = build_unet(
+        backbone=backbone,
+        decoder_block=decoder_block,
+        skip_connection_layers=encoder_features,
+        decoder_filters=decoder_filters,
+        classes=classes,
+        activation=activation,
+        n_upsample_blocks=len(decoder_filters),
+        use_batchnorm=decoder_use_batchnorm,
+        dropout=dropout,
+    )
+
+    # lock encoder weights for fine-tuning
+    if encoder_freeze:
+        freeze_model(backbone, **kwargs)
+
+    # loading model weights
+    if weights is not None:
+        model.load_weights(weights)
+
+    return model
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/models/pspnet.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/models/pspnet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,248 +1,249 @@
-from keras_applications import get_submodules_from_kwargs
-
-from ._common_blocks import Conv3dBn
-from ._utils import freeze_model
-from ..backbones.backbones_factory import Backbones
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-# ---------------------------------------------------------------------
-#  Utility functions
-# ---------------------------------------------------------------------
-
-def get_submodules():
-    return {
-        'backend': backend,
-        'models': models,
-        'layers': layers,
-        'utils': keras_utils,
-    }
-
-
-def check_input_shape(input_shape, factor):
-    if input_shape is None:
-        raise ValueError("Input shape should be a tuple of 3 integers, not None!")
-
-    h, w = input_shape[:2] if backend.image_data_format() == 'channels_last' else input_shape[1:]
-    min_size = factor * 6
-
-    is_wrong_shape = (
-            h % min_size != 0 or w % min_size != 0 or
-            h < min_size or w < min_size
-    )
-
-    if is_wrong_shape:
-        raise ValueError('Wrong shape {}, input H and W should '.format(input_shape) +
-                         'be divisible by `{}`'.format(min_size))
-
-
-# ---------------------------------------------------------------------
-#  Blocks
-# ---------------------------------------------------------------------
-
-def Conv1x1BnReLU(filters, use_batchnorm, name=None):
-    kwargs = get_submodules()
-
-    def wrapper(input_tensor):
-        return Conv3dBn(
-            filters,
-            kernel_size=1,
-            activation='relu',
-            kernel_initializer='he_uniform',
-            padding='same',
-            use_batchnorm=use_batchnorm,
-            name=name,
-            **kwargs
-        )(input_tensor)
-
-    return wrapper
-
-
-def SpatialContextBlock(
-        level,
-        conv_filters=512,
-        pooling_type='avg',
-        use_batchnorm=True,
-):
-    if pooling_type not in ('max', 'avg'):
-        raise ValueError('Unsupported pooling type - `{}`.'.format(pooling_type) +
-                         'Use `avg` or `max`.')
-
-    Pooling3D = layers.MaxPool3D if pooling_type == 'max' else layers.AveragePooling3D
-
-    pooling_name = 'psp_level{}_pooling'.format(level)
-    conv_block_name = 'psp_level{}'.format(level)
-    upsampling_name = 'psp_level{}_upsampling'.format(level)
-
-    def wrapper(input_tensor):
-        # extract input feature maps size (h, and w dimensions)
-        input_shape = backend.int_shape(input_tensor)
-        spatial_size = input_shape[1:4] if backend.image_data_format() == 'channels_last' else input_shape[2:]
-
-        # Compute the kernel and stride sizes according to how large the final feature map will be
-        # When the kernel factor and strides are equal, then we can compute the final feature map factor
-        # by simply dividing the current factor by the kernel or stride factor
-        # The final feature map sizes are 1x1, 2x2, 3x3, and 6x6.
-        pool_size = up_size = [spatial_size[0] // level, spatial_size[1] // level, spatial_size[2] // level]
-
-        x = Pooling3D(pool_size, strides=pool_size, padding='same', name=pooling_name)(input_tensor)
-        x = Conv1x1BnReLU(conv_filters, use_batchnorm, name=conv_block_name)(x)
-        # x = layers.UpSampling3D(up_size, interpolation='bilinear', name=upsampling_name)(x)
-        # TODO Find a way to do linear interpolation in 3D
-        x = layers.UpSampling3D(up_size, name=upsampling_name)(x)
-        return x
-
-    return wrapper
-
-
-# ---------------------------------------------------------------------
-#  PSP Decoder
-# ---------------------------------------------------------------------
-
-def build_psp(
-        backbone,
-        psp_layer_idx,
-        pooling_type='avg',
-        conv_filters=512,
-        use_batchnorm=True,
-        final_upsampling_factor=8,
-        classes=21,
-        activation='softmax',
-        dropout=None,
-):
-    input_ = backbone.input
-    x = (backbone.get_layer(name=psp_layer_idx).output if isinstance(psp_layer_idx, str)
-         else backbone.get_layer(index=psp_layer_idx).output)
-
-    # build spatial pyramid
-    x1 = SpatialContextBlock(1, conv_filters, pooling_type, use_batchnorm)(x)
-    x2 = SpatialContextBlock(2, conv_filters, pooling_type, use_batchnorm)(x)
-    x3 = SpatialContextBlock(3, conv_filters, pooling_type, use_batchnorm)(x)
-    x6 = SpatialContextBlock(6, conv_filters, pooling_type, use_batchnorm)(x)
-
-    # aggregate spatial pyramid
-    concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-    x = layers.Concatenate(axis=concat_axis, name='psp_concat')([x, x1, x2, x3, x6])
-    x = Conv1x1BnReLU(conv_filters, use_batchnorm, name='aggregation')(x)
-
-    # model regularization
-    if dropout is not None:
-        x = layers.SpatialDropout3D(dropout, name='spatial_dropout')(x)
-
-    # model head
-    x = layers.Conv3D(
-        filters=classes,
-        kernel_size=(3, 3, 3),
-        padding='same',
-        kernel_initializer='glorot_uniform',
-        name='final_conv',
-    )(x)
-
-    # x = layers.UpSampling3D(final_upsampling_factor, name='final_upsampling', interpolation='bilinear')(x)
-    # TODO: Find 3D interpolation
-    x = layers.UpSampling3D(final_upsampling_factor, name='final_upsampling')(x)
-    x = layers.Activation(activation, name=activation)(x)
-
-    model = models.Model(input_, x)
-
-    return model
-
-
-# ---------------------------------------------------------------------
-#  PSP Model
-# ---------------------------------------------------------------------
-
-def PSPNet(
-        backbone_name='vgg16',
-        input_shape=(32, 32, 32, 3),
-        classes=21,
-        activation='softmax',
-        weights=None,
-        encoder_weights='imagenet',
-        encoder_freeze=False,
-        downsample_factor=8,
-        psp_conv_filters=512,
-        psp_pooling_type='avg',
-        psp_use_batchnorm=True,
-        psp_dropout=None,
-        **kwargs
-):
-    """PSPNet_ is a fully convolution neural network for image semantic segmentation
-
-    Args:
-        backbone_name: name of classification model used as feature
-                extractor to build segmentation model.
-        input_shape: shape of input data/image ``(H, W, C)``.
-            ``H`` and ``W`` should be divisible by ``6 * downsample_factor`` and **NOT** ``None``!
-        classes: a number of classes for output (output shape - ``(h, w, classes)``).
-        activation: name of one of ``keras.activations`` for last model layer
-                (e.g. ``sigmoid``, ``softmax``, ``linear``).
-        weights: optional, path to model weights.
-        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
-        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
-        downsample_factor: one of 4, 8 and 16. Downsampling rate or in other words backbone depth
-            to construct PSP module on it.
-        psp_conv_filters: number of filters in ``Conv2D`` layer in each PSP block.
-        psp_pooling_type: one of 'avg', 'max'. PSP block pooling type (maximum or average).
-        psp_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
-                is used.
-        psp_dropout: dropout rate between 0 and 1.
-
-    Returns:
-        ``keras.models.Model``: **PSPNet**
-
-    .. _PSPNet:
-        https://arxiv.org/pdf/1612.01105.pdf
-
-    """
-
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    # control image input shape
-    check_input_shape(input_shape, downsample_factor)
-
-    backbone = Backbones.get_backbone(
-        backbone_name,
-        input_shape=input_shape,
-        weights=encoder_weights,
-        include_top=False,
-        **kwargs
-    )
-
-    feature_layers = Backbones.get_feature_layers(backbone_name, n=3)
-
-    if downsample_factor == 16:
-        psp_layer_idx = feature_layers[0]
-    elif downsample_factor == 8:
-        psp_layer_idx = feature_layers[1]
-    elif downsample_factor == 4:
-        psp_layer_idx = feature_layers[2]
-    else:
-        raise ValueError('Unsupported factor - `{}`, Use 4, 8 or 16.'.format(downsample_factor))
-
-    model = build_psp(
-        backbone,
-        psp_layer_idx,
-        pooling_type=psp_pooling_type,
-        conv_filters=psp_conv_filters,
-        use_batchnorm=psp_use_batchnorm,
-        final_upsampling_factor=downsample_factor,
-        classes=classes,
-        activation=activation,
-        dropout=psp_dropout,
-    )
-
-    # lock encoder weights for fine-tuning
-    if encoder_freeze:
-        freeze_model(backbone, **kwargs)
-
-    # loading model weights
-    if weights is not None:
-        model.load_weights(weights)
-
-    return model
+from .. import get_submodules_from_kwargs
+
+from ._common_blocks import Conv3dBn
+from ._utils import freeze_model
+from ..backbones.backbones_factory import Backbones
+from keras.src.legacy.backend import int_shape
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+# ---------------------------------------------------------------------
+#  Utility functions
+# ---------------------------------------------------------------------
+
+def get_submodules():
+    return {
+        'backend': backend,
+        'models': models,
+        'layers': layers,
+        'utils': keras_utils,
+    }
+
+
+def check_input_shape(input_shape, factor):
+    if input_shape is None:
+        raise ValueError("Input shape should be a tuple of 3 integers, not None!")
+
+    h, w = input_shape[:2] if backend.image_data_format() == 'channels_last' else input_shape[1:]
+    min_size = factor * 6
+
+    is_wrong_shape = (
+            h % min_size != 0 or w % min_size != 0 or
+            h < min_size or w < min_size
+    )
+
+    if is_wrong_shape:
+        raise ValueError('Wrong shape {}, input H and W should '.format(input_shape) +
+                         'be divisible by `{}`'.format(min_size))
+
+
+# ---------------------------------------------------------------------
+#  Blocks
+# ---------------------------------------------------------------------
+
+def Conv1x1BnReLU(filters, use_batchnorm, name=None):
+    kwargs = get_submodules()
+
+    def wrapper(input_tensor):
+        return Conv3dBn(
+            filters,
+            kernel_size=1,
+            activation='relu',
+            kernel_initializer='he_uniform',
+            padding='same',
+            use_batchnorm=use_batchnorm,
+            name=name,
+            **kwargs
+        )(input_tensor)
+
+    return wrapper
+
+
+def SpatialContextBlock(
+        level,
+        conv_filters=512,
+        pooling_type='avg',
+        use_batchnorm=True,
+):
+    if pooling_type not in ('max', 'avg'):
+        raise ValueError('Unsupported pooling type - `{}`.'.format(pooling_type) +
+                         'Use `avg` or `max`.')
+
+    Pooling3D = layers.MaxPool3D if pooling_type == 'max' else layers.AveragePooling3D
+
+    pooling_name = 'psp_level{}_pooling'.format(level)
+    conv_block_name = 'psp_level{}'.format(level)
+    upsampling_name = 'psp_level{}_upsampling'.format(level)
+
+    def wrapper(input_tensor):
+        # extract input feature maps size (h, and w dimensions)
+        input_shape = int_shape(input_tensor)
+        spatial_size = input_shape[1:4] if backend.image_data_format() == 'channels_last' else input_shape[2:]
+
+        # Compute the kernel and stride sizes according to how large the final feature map will be
+        # When the kernel factor and strides are equal, then we can compute the final feature map factor
+        # by simply dividing the current factor by the kernel or stride factor
+        # The final feature map sizes are 1x1, 2x2, 3x3, and 6x6.
+        pool_size = up_size = [spatial_size[0] // level, spatial_size[1] // level, spatial_size[2] // level]
+
+        x = Pooling3D(pool_size, strides=pool_size, padding='same', name=pooling_name)(input_tensor)
+        x = Conv1x1BnReLU(conv_filters, use_batchnorm, name=conv_block_name)(x)
+        # x = layers.UpSampling3D(up_size, interpolation='bilinear', name=upsampling_name)(x)
+        # TODO Find a way to do linear interpolation in 3D
+        x = layers.UpSampling3D(up_size, name=upsampling_name)(x)
+        return x
+
+    return wrapper
+
+
+# ---------------------------------------------------------------------
+#  PSP Decoder
+# ---------------------------------------------------------------------
+
+def build_psp(
+        backbone,
+        psp_layer_idx,
+        pooling_type='avg',
+        conv_filters=512,
+        use_batchnorm=True,
+        final_upsampling_factor=8,
+        classes=21,
+        activation='softmax',
+        dropout=None,
+):
+    input_ = backbone.input
+    x = (backbone.get_layer(name=psp_layer_idx).output if isinstance(psp_layer_idx, str)
+         else backbone.get_layer(index=psp_layer_idx).output)
+
+    # build spatial pyramid
+    x1 = SpatialContextBlock(1, conv_filters, pooling_type, use_batchnorm)(x)
+    x2 = SpatialContextBlock(2, conv_filters, pooling_type, use_batchnorm)(x)
+    x3 = SpatialContextBlock(3, conv_filters, pooling_type, use_batchnorm)(x)
+    x6 = SpatialContextBlock(6, conv_filters, pooling_type, use_batchnorm)(x)
+
+    # aggregate spatial pyramid
+    concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+    x = layers.Concatenate(axis=concat_axis, name='psp_concat')([x, x1, x2, x3, x6])
+    x = Conv1x1BnReLU(conv_filters, use_batchnorm, name='aggregation')(x)
+
+    # model regularization
+    if dropout is not None:
+        x = layers.SpatialDropout3D(dropout, name='spatial_dropout')(x)
+
+    # model head
+    x = layers.Conv3D(
+        filters=classes,
+        kernel_size=(3, 3, 3),
+        padding='same',
+        kernel_initializer='glorot_uniform',
+        name='final_conv',
+    )(x)
+
+    # x = layers.UpSampling3D(final_upsampling_factor, name='final_upsampling', interpolation='bilinear')(x)
+    # TODO: Find 3D interpolation
+    x = layers.UpSampling3D(final_upsampling_factor, name='final_upsampling')(x)
+    x = layers.Activation(activation, name=activation)(x)
+
+    model = models.Model(input_, x)
+
+    return model
+
+
+# ---------------------------------------------------------------------
+#  PSP Model
+# ---------------------------------------------------------------------
+
+def PSPNet(
+        backbone_name='vgg16',
+        input_shape=(32, 32, 32, 3),
+        classes=21,
+        activation='softmax',
+        weights=None,
+        encoder_weights='imagenet',
+        encoder_freeze=False,
+        downsample_factor=8,
+        psp_conv_filters=512,
+        psp_pooling_type='avg',
+        psp_use_batchnorm=True,
+        psp_dropout=None,
+        **kwargs
+):
+    """PSPNet_ is a fully convolution neural network for image semantic segmentation
+
+    Args:
+        backbone_name: name of classification model used as feature
+                extractor to build segmentation model.
+        input_shape: shape of input data/image ``(H, W, C)``.
+            ``H`` and ``W`` should be divisible by ``6 * downsample_factor`` and **NOT** ``None``!
+        classes: a number of classes for output (output shape - ``(h, w, classes)``).
+        activation: name of one of ``keras.activations`` for last model layer
+                (e.g. ``sigmoid``, ``softmax``, ``linear``).
+        weights: optional, path to model weights.
+        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
+        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
+        downsample_factor: one of 4, 8 and 16. Downsampling rate or in other words backbone depth
+            to construct PSP module on it.
+        psp_conv_filters: number of filters in ``Conv2D`` layer in each PSP block.
+        psp_pooling_type: one of 'avg', 'max'. PSP block pooling type (maximum or average).
+        psp_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
+                is used.
+        psp_dropout: dropout rate between 0 and 1.
+
+    Returns:
+        ``keras.models.Model``: **PSPNet**
+
+    .. _PSPNet:
+        https://arxiv.org/pdf/1612.01105.pdf
+
+    """
+
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils, _, _ = get_submodules_from_kwargs(kwargs)
+
+    # control image input shape
+    check_input_shape(input_shape, downsample_factor)
+
+    backbone = Backbones.get_backbone(
+        backbone_name,
+        input_shape=input_shape,
+        weights=encoder_weights,
+        include_top=False,
+        **kwargs
+    )
+
+    feature_layers = Backbones.get_feature_layers(backbone_name, n=3)
+
+    if downsample_factor == 16:
+        psp_layer_idx = feature_layers[0]
+    elif downsample_factor == 8:
+        psp_layer_idx = feature_layers[1]
+    elif downsample_factor == 4:
+        psp_layer_idx = feature_layers[2]
+    else:
+        raise ValueError('Unsupported factor - `{}`, Use 4, 8 or 16.'.format(downsample_factor))
+
+    model = build_psp(
+        backbone,
+        psp_layer_idx,
+        pooling_type=psp_pooling_type,
+        conv_filters=psp_conv_filters,
+        use_batchnorm=psp_use_batchnorm,
+        final_upsampling_factor=downsample_factor,
+        classes=classes,
+        activation=activation,
+        dropout=psp_dropout,
+    )
+
+    # lock encoder weights for fine-tuning
+    if encoder_freeze:
+        freeze_model(backbone, **kwargs)
+
+    # loading model weights
+    if weights is not None:
+        model.load_weights(weights)
+
+    return model
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D/models/unet.py` & `segmentation_models_3D-1.1.0/segmentation_models_3D/models/linknet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,257 +1,283 @@
-from keras_applications import get_submodules_from_kwargs
-
-from ._common_blocks import Conv3dBn
-from ._utils import freeze_model
-from ..backbones.backbones_factory import Backbones
-
-backend = None
-layers = None
-models = None
-keras_utils = None
-
-
-# ---------------------------------------------------------------------
-#  Utility functions
-# ---------------------------------------------------------------------
-
-def get_submodules():
-    return {
-        'backend': backend,
-        'models': models,
-        'layers': layers,
-        'utils': keras_utils,
-    }
-
-
-# ---------------------------------------------------------------------
-#  Blocks
-# ---------------------------------------------------------------------
-
-def Conv3x3BnReLU(filters, use_batchnorm, name=None):
-    kwargs = get_submodules()
-
-    def wrapper(input_tensor):
-        return Conv3dBn(
-            filters,
-            kernel_size=3,
-            activation='relu',
-            kernel_initializer='he_uniform',
-            padding='same',
-            use_batchnorm=use_batchnorm,
-            name=name,
-            **kwargs
-        )(input_tensor)
-
-    return wrapper
-
-
-def DecoderUpsamplingX2Block(filters, stage, use_batchnorm=False):
-    up_name = 'decoder_stage{}_upsampling'.format(stage)
-    conv1_name = 'decoder_stage{}a'.format(stage)
-    conv2_name = 'decoder_stage{}b'.format(stage)
-    concat_name = 'decoder_stage{}_concat'.format(stage)
-
-    concat_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    def wrapper(input_tensor, skip=None):
-        x = layers.UpSampling3D(size=2, name=up_name)(input_tensor)
-
-        if skip is not None:
-            x = layers.Concatenate(axis=concat_axis, name=concat_name)([x, skip])
-
-        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv1_name)(x)
-        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv2_name)(x)
-
-        return x
-
-    return wrapper
-
-
-def DecoderTransposeX2Block(filters, stage, use_batchnorm=False):
-    transp_name = 'decoder_stage{}a_transpose'.format(stage)
-    bn_name = 'decoder_stage{}a_bn'.format(stage)
-    relu_name = 'decoder_stage{}a_relu'.format(stage)
-    conv_block_name = 'decoder_stage{}b'.format(stage)
-    concat_name = 'decoder_stage{}_concat'.format(stage)
-
-    concat_axis = bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
-
-    def layer(input_tensor, skip=None):
-
-        x = layers.Conv3DTranspose(
-            filters,
-            kernel_size=(4, 4, 4),
-            strides=(2, 2, 2),
-            padding='same',
-            name=transp_name,
-            use_bias=not use_batchnorm,
-        )(input_tensor)
-
-        if use_batchnorm:
-            x = layers.BatchNormalization(axis=bn_axis, name=bn_name)(x)
-
-        x = layers.Activation('relu', name=relu_name)(x)
-
-        if skip is not None:
-            x = layers.Concatenate(axis=concat_axis, name=concat_name)([x, skip])
-
-        x = Conv3x3BnReLU(filters, use_batchnorm, name=conv_block_name)(x)
-
-        return x
-
-    return layer
-
-
-# ---------------------------------------------------------------------
-#  Unet Decoder
-# ---------------------------------------------------------------------
-
-def build_unet(
-        backbone,
-        decoder_block,
-        skip_connection_layers,
-        decoder_filters=(256, 128, 64, 32, 16),
-        n_upsample_blocks=5,
-        classes=1,
-        activation='sigmoid',
-        use_batchnorm=True,
-        dropout=None,
-):
-    input_ = backbone.input
-    x = backbone.output
-
-    # extract skip connections
-    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
-              else backbone.get_layer(index=i).output for i in skip_connection_layers])
-
-    # add center block if previous operation was maxpooling (for vgg models)
-    if isinstance(backbone.layers[-1], layers.MaxPooling3D):
-        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block1')(x)
-        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block2')(x)
-
-    # building decoder blocks
-    for i in range(n_upsample_blocks):
-
-        if i < len(skips):
-            skip = skips[i]
-        else:
-            skip = None
-
-        x = decoder_block(decoder_filters[i], stage=i, use_batchnorm=use_batchnorm)(x, skip)
-
-    if dropout:
-        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
-
-    # model head (define number of output classes)
-    x = layers.Conv3D(
-        filters=classes,
-        kernel_size=(3, 3, 3),
-        padding='same',
-        use_bias=True,
-        kernel_initializer='glorot_uniform',
-        name='final_conv',
-    )(x)
-    x = layers.Activation(activation, name=activation)(x)
-
-    # create keras model instance
-    model = models.Model(input_, x)
-
-    return model
-
-
-# ---------------------------------------------------------------------
-#  Unet Model
-# ---------------------------------------------------------------------
-
-def Unet(
-        backbone_name='vgg16',
-        input_shape=(None, None, 3),
-        classes=1,
-        activation='sigmoid',
-        weights=None,
-        encoder_weights='imagenet',
-        encoder_freeze=False,
-        encoder_features='default',
-        decoder_block_type='upsampling',
-        decoder_filters=(256, 128, 64, 32, 16),
-        decoder_use_batchnorm=True,
-        dropout=None,
-        **kwargs
-):
-    """ Unet_ is a fully convolution neural network for image semantic segmentation
-
-    Args:
-        backbone_name: name of classification model (without last dense layers) used as feature
-            extractor to build segmentation model.
-        input_shape: shape of input data/image ``(H, W, C)``, in general
-            case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
-            able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
-        classes: a number of classes for output (output shape - ``(h, w, classes)``).
-        activation: name of one of ``keras.activations`` for last model layer
-            (e.g. ``sigmoid``, ``softmax``, ``linear``).
-        weights: optional, path to model weights.
-        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
-        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
-        encoder_features: a list of layer numbers or names starting from top of the model.
-            Each of these layers will be concatenated with corresponding decoder block. If ``default`` is used
-            layer names are taken from ``DEFAULT_SKIP_CONNECTIONS``.
-        decoder_block_type: one of blocks with following layers structure:
-
-            - `upsampling`:  ``UpSampling2D`` -> ``Conv2D`` -> ``Conv2D``
-            - `transpose`:   ``Transpose2D`` -> ``Conv2D``
-
-        decoder_filters: list of numbers of ``Conv2D`` layer filters in decoder blocks
-        decoder_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
-            is used.
-
-    Returns:
-        ``keras.models.Model``: **Unet**
-
-    .. _Unet:
-        https://arxiv.org/pdf/1505.04597
-
-    """
-
-    global backend, layers, models, keras_utils
-    backend, layers, models, keras_utils = get_submodules_from_kwargs(kwargs)
-
-    if decoder_block_type == 'upsampling':
-        decoder_block = DecoderUpsamplingX2Block
-    elif decoder_block_type == 'transpose':
-        decoder_block = DecoderTransposeX2Block
-    else:
-        raise ValueError('Decoder block type should be in ("upsampling", "transpose"). '
-                         'Got: {}'.format(decoder_block_type))
-
-    backbone = Backbones.get_backbone(
-        backbone_name,
-        input_shape=input_shape,
-        weights=encoder_weights,
-        include_top=False,
-        **kwargs,
-    )
-
-    if encoder_features == 'default':
-        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
-
-    model = build_unet(
-        backbone=backbone,
-        decoder_block=decoder_block,
-        skip_connection_layers=encoder_features,
-        decoder_filters=decoder_filters,
-        classes=classes,
-        activation=activation,
-        n_upsample_blocks=len(decoder_filters),
-        use_batchnorm=decoder_use_batchnorm,
-        dropout=dropout,
-    )
-
-    # lock encoder weights for fine-tuning
-    if encoder_freeze:
-        freeze_model(backbone, **kwargs)
-
-    # loading model weights
-    if weights is not None:
-        model.load_weights(weights)
-
-    return model
+from .. import get_submodules_from_kwargs
+
+from ._common_blocks import Conv3dBn
+from ._utils import freeze_model
+from ..backbones.backbones_factory import Backbones
+from keras.src.legacy.backend import int_shape
+
+backend = None
+layers = None
+models = None
+keras_utils = None
+
+
+# ---------------------------------------------------------------------
+#  Utility functions
+# ---------------------------------------------------------------------
+
+def get_submodules():
+    return {
+        'backend': backend,
+        'models': models,
+        'layers': layers,
+        'utils': keras_utils,
+    }
+
+
+# ---------------------------------------------------------------------
+#  Blocks
+# ---------------------------------------------------------------------
+
+def Conv3x3BnReLU(filters, use_batchnorm, name=None):
+    kwargs = get_submodules()
+
+    def wrapper(input_tensor):
+        return Conv3dBn(
+            filters,
+            kernel_size=3,
+            activation='relu',
+            kernel_initializer='he_uniform',
+            padding='same',
+            use_batchnorm=use_batchnorm,
+            name=name,
+            **kwargs
+        )(input_tensor)
+
+    return wrapper
+
+
+def Conv1x1BnReLU(filters, use_batchnorm, name=None):
+    kwargs = get_submodules()
+
+    def wrapper(input_tensor):
+        return Conv3dBn(
+            filters,
+            kernel_size=1,
+            activation='relu',
+            kernel_initializer='he_uniform',
+            padding='same',
+            use_batchnorm=use_batchnorm,
+            name=name,
+            **kwargs
+        )(input_tensor)
+
+    return wrapper
+
+
+def DecoderUpsamplingX2Block(filters, stage, use_batchnorm):
+    conv_block1_name = 'decoder_stage{}a'.format(stage)
+    conv_block2_name = 'decoder_stage{}b'.format(stage)
+    conv_block3_name = 'decoder_stage{}c'.format(stage)
+    up_name = 'decoder_stage{}_upsampling'.format(stage)
+    add_name = 'decoder_stage{}_add'.format(stage)
+
+    channels_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    def wrapper(input_tensor, skip=None):
+        input_filters = int_shape(input_tensor)[channels_axis]
+        output_filters = int_shape(skip)[channels_axis] if skip is not None else filters
+
+        x = Conv1x1BnReLU(input_filters // 4, use_batchnorm, name=conv_block1_name)(input_tensor)
+        x = layers.UpSampling3D((2, 2, 2), name=up_name)(x)
+        x = Conv3x3BnReLU(input_filters // 4, use_batchnorm, name=conv_block2_name)(x)
+        x = Conv1x1BnReLU(output_filters, use_batchnorm, name=conv_block3_name)(x)
+
+        if skip is not None:
+            x = layers.Add(name=add_name)([x, skip])
+        return x
+
+    return wrapper
+
+
+def DecoderTransposeX2Block(filters, stage, use_batchnorm):
+    conv_block1_name = 'decoder_stage{}a'.format(stage)
+    transpose_name = 'decoder_stage{}b_transpose'.format(stage)
+    bn_name = 'decoder_stage{}b_bn'.format(stage)
+    relu_name = 'decoder_stage{}b_relu'.format(stage)
+    conv_block3_name = 'decoder_stage{}c'.format(stage)
+    add_name = 'decoder_stage{}_add'.format(stage)
+
+    channels_axis = bn_axis = 4 if backend.image_data_format() == 'channels_last' else 1
+
+    def wrapper(input_tensor, skip=None):
+        input_filters = int_shape(input_tensor)[channels_axis]
+        output_filters = int_shape(skip)[channels_axis] if skip is not None else filters
+
+        x = Conv1x1BnReLU(input_filters // 4, use_batchnorm, name=conv_block1_name)(input_tensor)
+        x = layers.Conv3DTranspose(
+            filters=input_filters // 4,
+            kernel_size=(4, 4, 4),
+            strides=(2, 2, 2),
+            padding='same',
+            name=transpose_name,
+            use_bias=not use_batchnorm,
+        )(x)
+
+        if use_batchnorm:
+            x = layers.BatchNormalization(axis=bn_axis, name=bn_name)(x)
+
+        x = layers.Activation('relu', name=relu_name)(x)
+        x = Conv1x1BnReLU(output_filters, use_batchnorm, name=conv_block3_name)(x)
+
+        if skip is not None:
+            x = layers.Add(name=add_name)([x, skip])
+
+        return x
+
+    return wrapper
+
+
+# ---------------------------------------------------------------------
+#  LinkNet Decoder
+# ---------------------------------------------------------------------
+
+def build_linknet(
+        backbone,
+        decoder_block,
+        skip_connection_layers,
+        decoder_filters=(256, 128, 64, 32, 16),
+        n_upsample_blocks=5,
+        classes=1,
+        activation='sigmoid',
+        use_batchnorm=True,
+        dropout=None,
+):
+    input_ = backbone.input
+    x = backbone.output
+
+    # extract skip connections
+    skips = ([backbone.get_layer(name=i).output if isinstance(i, str)
+              else backbone.get_layer(index=i).output for i in skip_connection_layers])
+
+    # add center block if previous operation was maxpooling (for vgg models)
+    if isinstance(backbone.layers[-1], layers.MaxPooling2D):
+        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block1')(x)
+        x = Conv3x3BnReLU(512, use_batchnorm, name='center_block2')(x)
+
+    # building decoder blocks
+    for i in range(n_upsample_blocks):
+
+        if i < len(skips):
+            skip = skips[i]
+        else:
+            skip = None
+
+        x = decoder_block(decoder_filters[i], stage=i, use_batchnorm=use_batchnorm)(x, skip)
+
+    if dropout:
+        x = layers.SpatialDropout3D(dropout, name='pyramid_dropout')(x)
+
+    # model head (define number of output classes)
+    x = layers.Conv3D(
+        filters=classes,
+        kernel_size=(3, 3, 3),
+        padding='same',
+        use_bias=True,
+        kernel_initializer='glorot_uniform'
+    )(x)
+    x = layers.Activation(activation, name=activation)(x)
+
+    # create keras model instance
+    model = models.Model(input_, x)
+
+    return model
+
+
+# ---------------------------------------------------------------------
+#  LinkNet Model
+# ---------------------------------------------------------------------
+
+def Linknet(
+        backbone_name='vgg16',
+        input_shape=(None, None, 3),
+        classes=1,
+        activation='sigmoid',
+        weights=None,
+        encoder_weights='imagenet',
+        encoder_freeze=False,
+        encoder_features='default',
+        decoder_block_type='upsampling',
+        decoder_filters=(None, None, None, None, 16),
+        decoder_use_batchnorm=True,
+        dropout=None,
+        **kwargs
+):
+    """Linknet_ is a fully convolution neural network for fast image semantic segmentation
+
+    Note:
+        This implementation by default has 4 skip connections (original - 3).
+
+    Args:
+        backbone_name: name of classification model (without last dense layers) used as feature
+                    extractor to build segmentation model.
+        input_shape: shape of input data/image ``(H, W, C)``, in general
+                case you do not need to set ``H`` and ``W`` shapes, just pass ``(None, None, C)`` to make your model be
+                able to process images af any size, but ``H`` and ``W`` of input images should be divisible by factor ``32``.
+        classes: a number of classes for output (output shape - ``(h, w, classes)``).
+        activation: name of one of ``keras.activations`` for last model layer
+            (e.g. ``sigmoid``, ``softmax``, ``linear``).
+        weights: optional, path to model weights.
+        encoder_weights: one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
+        encoder_freeze: if ``True`` set all layers of encoder (backbone model) as non-trainable.
+        encoder_features: a list of layer numbers or names starting from top of the model.
+                    Each of these layers will be concatenated with corresponding decoder block. If ``default`` is used
+                    layer names are taken from ``DEFAULT_SKIP_CONNECTIONS``.
+        decoder_filters: list of numbers of ``Conv2D`` layer filters in decoder blocks,
+            for block with skip connection a number of filters is equal to number of filters in
+            corresponding encoder block (estimates automatically and can be passed as ``None`` value).
+        decoder_use_batchnorm: if ``True``, ``BatchNormalisation`` layer between ``Conv2D`` and ``Activation`` layers
+                    is used.
+        decoder_block_type: one of
+                    - `upsampling`:  use ``UpSampling2D`` keras layer
+                    - `transpose`:   use ``Transpose2D`` keras layer
+
+    Returns:
+        ``keras.models.Model``: **Linknet**
+
+    .. _Linknet:
+        https://arxiv.org/pdf/1707.03718.pdf
+    """
+
+    global backend, layers, models, keras_utils
+    backend, layers, models, keras_utils, _, _ = get_submodules_from_kwargs(kwargs)
+
+    if decoder_block_type == 'upsampling':
+        decoder_block = DecoderUpsamplingX2Block
+    elif decoder_block_type == 'transpose':
+        decoder_block = DecoderTransposeX2Block
+    else:
+        raise ValueError('Decoder block type should be in ("upsampling", "transpose"). '
+                         'Got: {}'.format(decoder_block_type))
+
+    backbone = Backbones.get_backbone(
+        backbone_name,
+        input_shape=input_shape,
+        weights=encoder_weights,
+        include_top=False,
+        **kwargs,
+    )
+
+    if encoder_features == 'default':
+        encoder_features = Backbones.get_feature_layers(backbone_name, n=4)
+
+    model = build_linknet(
+        backbone=backbone,
+        decoder_block=decoder_block,
+        skip_connection_layers=encoder_features,
+        decoder_filters=decoder_filters,
+        classes=classes,
+        activation=activation,
+        n_upsample_blocks=len(decoder_filters),
+        use_batchnorm=decoder_use_batchnorm,
+        dropout=dropout,
+    )
+
+    # lock encoder weights for fine-tuning
+    if encoder_freeze:
+        freeze_model(backbone, **kwargs)
+
+    # loading model weights
+    if weights is not None:
+        model.load_weights(weights)
+
+    return model
```

### Comparing `segmentation_models_3D-1.0.7/segmentation_models_3D.egg-info/SOURCES.txt` & `segmentation_models_3D-1.1.0/segmentation_models_3D.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 segmentation_models_3D.egg-info/PKG-INFO
 segmentation_models_3D.egg-info/SOURCES.txt
 segmentation_models_3D.egg-info/dependency_links.txt
 segmentation_models_3D.egg-info/requires.txt
 segmentation_models_3D.egg-info/top_level.txt
 segmentation_models_3D/backbones/__init__.py
 segmentation_models_3D/backbones/backbones_factory.py
+segmentation_models_3D/backbones/inception_resnet_v2.py
+segmentation_models_3D/backbones/inception_v3.py
 segmentation_models_3D/base/__init__.py
 segmentation_models_3D/base/functional.py
 segmentation_models_3D/base/objects.py
 segmentation_models_3D/models/__init__.py
 segmentation_models_3D/models/_common_blocks.py
 segmentation_models_3D/models/_utils.py
 segmentation_models_3D/models/fpn.py
```

### Comparing `segmentation_models_3D-1.0.7/setup.py` & `segmentation_models_3D-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='segmentation_models_3D',
-    version='1.0.7',
+    version='1.1.0',
     author='Roman Sol (ZFTurbo)',
     packages=['segmentation_models_3D', 'segmentation_models_3D/backbones', 'segmentation_models_3D/base', 'segmentation_models_3D/models'],
     url='https://github.com/ZFTurbo/segmentation_models_3D',
     description='Set of Keras models for segmentation of 3D volumes .',
     long_description='3D variants of popular models for segmentation like FPN, Unet, Linknet and PSPNet.'
-                     'Models work with keras and tensorflow.keras.'
+                     'Models work with keras (version 3).'
                      'More details: https://github.com/ZFTurbo/segmentation_models_3D',
     install_requires=[
-        'tensorflow>=2.13.0,<=2.15.0',
-        'keras==2.13.1',
-        "keras_applications==1.0.8",
-        "classification_models_3D==1.0.10",
+        'keras==3.3.3',
+        "classification_models_3D==1.1.0",
     ],
 )
```

