# Comparing `tmp/bioimageio.core-0.6.1.tar.gz` & `tmp/bioimageio.core-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.6.1.tar", last modified: Fri Apr 26 08:10:14 2024, max compression
+gzip compressed data, was "bioimageio.core-0.6.2.tar", last modified: Tue Apr 30 23:23:18 2024, max compression
```

## Comparing `bioimageio.core-0.6.1.tar` & `bioimageio.core-0.6.2.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.347664 bioimageio.core-0.6.1/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.351664 bioimageio.core-0.6.1/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_magic_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_op_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/block_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-26 08:10:11.000000 bioimageio.core-0.6.1/bioimageio/core/digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/model_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/proc_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.351664 bioimageio.core-0.6.1/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 08:10:14.000000 bioimageio.core-0.6.1/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/scripts/setup_dev_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/scripts/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.355664 bioimageio.core-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_any_model_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_prediction_pipeline_device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/keras/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/test_add_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:10:14.359664 bioimageio.core-0.6.1/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-26 08:09:44.000000 bioimageio.core-0.6.1/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.930637 bioimageio.core-0.6.2/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.934637 bioimageio.core-0.6.2/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.6.1/LICENSE` & `bioimageio.core-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/PKG-INFO` & `bioimageio.core-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
-        Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
+        Python specific core utilities for bioimage.io resources (in particular models).
         
         ## Installation
         
         ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
         
@@ -74,15 +74,15 @@
         mamba env create -f dev/env.yaml
         mamba activate core
         pip install -e . --no-deps
         ```
         
         There are different environment files available that only install tensorflow or pytorch as dependencies.
         
-        ## 💻 Command Line
+        ## 💻 Use the Command Line Interface
         
         `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
         You can list all the available commands via:
         
         ```console
         bioimageio
         ```
@@ -109,32 +109,38 @@
         
         ```console
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
         
         `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
-        ## From python
+        ## 🐍 Use in Python
         
         `bioimageio.core` is a python package that implements prediction with bioimageio models
         including standardized pre- and postprocessing operations.
         These models are described by---and can be loaded with---the bioimageio.spec package.
         
         In addition bioimageio.core provides functionality to convert model weight formats.
         
         To get an overview of this functionality, check out these example notebooks:
         
         * [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
         
+        and the [developer documentation](https://bioimage-io.github.io/core-bioimage-io-python/bioimageio/core.html).
+        
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.2
+        
+        * Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
+        
         ### 0.6.1
         
         * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
         
         ### 0.6.0
         
         * add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
```

### Comparing `bioimageio.core-0.6.1/README.md` & `bioimageio.core-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # core-bioimage-io-python
 
-Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
+Python specific core utilities for bioimage.io resources (in particular models).
 
 ## Installation
 
 ### Via Mamba/Conda
 
 The `bioimageio.core` package can be installed from conda-forge via
 
@@ -65,15 +65,15 @@
 mamba env create -f dev/env.yaml
 mamba activate core
 pip install -e . --no-deps
 ```
 
 There are different environment files available that only install tensorflow or pytorch as dependencies.
 
-## 💻 Command Line
+## 💻 Use the Command Line Interface
 
 `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
 You can list all the available commands via:
 
 ```console
 bioimageio
 ```
@@ -100,32 +100,38 @@
 
 ```console
 bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
 ```
 
 `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
 
-## From python
+## 🐍 Use in Python
 
 `bioimageio.core` is a python package that implements prediction with bioimageio models
 including standardized pre- and postprocessing operations.
 These models are described by---and can be loaded with---the bioimageio.spec package.
 
 In addition bioimageio.core provides functionality to convert model weight formats.
 
 To get an overview of this functionality, check out these example notebooks:
 
 * [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
 
+and the [developer documentation](https://bioimage-io.github.io/core-bioimage-io-python/bioimageio/core.html).
+
 ## Model Specification
 
 The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
 
 ## Changelog
 
+### 0.6.2
+
+* Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
+
 ### 0.6.1
 
 * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
 
 ### 0.6.0
 
 * add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
```

### Comparing `bioimageio.core-0.6.1/bioimageio/core/__init__.py` & `bioimageio.core-0.6.2/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/__main__.py` & `bioimageio.core-0.6.2/bioimageio/core/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""The `Bioimageio` class defined here has static methods that constitute the `bioimageio` command line interface (using fire)"""
+
 import sys
 from pathlib import Path
 from typing import List, Optional, Union
 
 import fire
 
 from bioimageio.core import __version__, test_description
@@ -10,16 +12,18 @@
 from bioimageio.spec.dataset import DatasetDescr
 from bioimageio.spec.model import ModelDescr
 from bioimageio.spec.model.v0_5 import WeightsFormat
 from bioimageio.spec.notebook import NotebookDescr
 
 
 class Bioimageio:
+    """🦒 CLI to work with resources shared on bioimage.io"""
+
+    @staticmethod
     def package(
-        self,
         source: str,
         path: Path = Path("bioimageio-package.zip"),
         weight_format: Optional[WeightsFormat] = None,
     ):
         """Package a bioimageio resource as a zip file
 
         Args:
@@ -29,16 +33,16 @@
         """
         _ = save_bioimageio_package(
             source,
             output_path=path,
             weights_priority_order=None if weight_format is None else (weight_format,),
         )
 
+    @staticmethod
     def test(
-        self,
         source: str,
         weight_format: Optional[WeightsFormat] = None,
         *,
         devices: Optional[Union[str, List[str]]] = None,
         decimal: int = 4,
     ):
         """test a bioimageio resource
@@ -57,16 +61,16 @@
             decimal=decimal,
         )
         print(f"\ntesting model {source}...")
         print(summary.format())
         sys.exit(0 if summary.status == "passed" else 1)
 
 
-Bioimageio.__doc__ = f"""
-work with resources shared on bioimage.io
+assert isinstance(Bioimageio.__doc__, str)
+Bioimageio.__doc__ += f"""
 
 library versions:
   bioimageio.core {__version__}
   bioimageio.spec {__version__}
 
 spec format versions:
         model RDF {ModelDescr.implemented_format_version}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bioimageio.core-0.6.1/bioimageio/core/_magic_tensor_ops.py` & `bioimageio.core-0.6.2/bioimageio/core/_magic_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/_op_base.py` & `bioimageio.core-0.6.2/bioimageio/core/_op_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/_prediction_pipeline.py` & `bioimageio.core-0.6.2/bioimageio/core/_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/_resource_tests.py` & `bioimageio.core-0.6.2/bioimageio/core/_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/axis.py` & `bioimageio.core-0.6.2/bioimageio/core/axis.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/block.py` & `bioimageio.core-0.6.2/bioimageio/core/block.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from .axis import PerAxis
 from .block_meta import BlockMeta, LinearAxisTransform, split_shape_into_blocks
 from .common import (
     Halo,
     HaloLike,
     PadMode,
+    SliceInfo,
     TotalNumberOfBlocks,
 )
 from .tensor import Tensor
 
 
 @dataclass(frozen=True)
 class Block(BlockMeta):
@@ -30,14 +31,15 @@
 
     @property
     def inner_data(self):
         return self.data[self.local_slice]
 
     def __post_init__(self):
         super().__post_init__()
+        assert not any(v == -1 for v in self.sample_shape.values()), self.sample_shape
         for a, s in self.data.sizes.items():
             slice_ = self.inner_slice[a]
             halo = self.halo.get(a, Halo(0, 0))
             assert s == halo.left + (slice_.stop - slice_.start) + halo.right, (
                 s,
                 slice_,
                 halo,
@@ -61,14 +63,35 @@
         )
 
     def get_transformed(
         self, new_axes: PerAxis[Union[LinearAxisTransform, int]]
     ) -> Self:
         raise NotImplementedError
 
+    @classmethod
+    def from_meta(cls, meta: BlockMeta, data: Tensor) -> Self:
+        return cls(
+            sample_shape={
+                k: data.tagged_shape[k] if v == -1 else v
+                for k, v in meta.sample_shape.items()
+            },
+            inner_slice={
+                k: (
+                    SliceInfo(start=v.start, stop=data.tagged_shape[k])
+                    if v.stop == -1
+                    else v
+                )
+                for k, v in meta.inner_slice.items()
+            },
+            halo=meta.halo,
+            block_index=meta.block_index,
+            blocks_in_sample=meta.blocks_in_sample,
+            data=data,
+        )
+
 
 def split_tensor_into_blocks(
     tensor: Tensor,
     block_shape: PerAxis[int],
     *,
     halo: PerAxis[HaloLike],
     stride: Optional[PerAxis[int]] = None,
```

### Comparing `bioimageio.core-0.6.1/bioimageio/core/block_meta.py` & `bioimageio.core-0.6.2/bioimageio/core/block_meta.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/common.py` & `bioimageio.core-0.6.2/bioimageio/core/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/digest_spec.py` & `bioimageio.core-0.6.2/bioimageio/core/digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/io.py` & `bioimageio.core-0.6.2/bioimageio/core/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_keras_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_pytorch_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_tensorflow_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_torchscript_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/proc_ops.py` & `bioimageio.core-0.6.2/bioimageio/core/proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/proc_setup.py` & `bioimageio.core-0.6.2/bioimageio/core/proc_setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/sample.py` & `bioimageio.core-0.6.2/bioimageio/core/sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,26 +247,24 @@
             sample_id=self.sample_id,
             block_index=self.block_index,
             blocks_in_sample=self.blocks_in_sample,
         )
 
     def with_data(self, data: PerMember[Tensor], *, stat: Stat) -> SampleBlock:
         return SampleBlock(
-            sample_shape=self.sample_shape,
+            sample_shape={
+                m: {
+                    a: data[m].tagged_shape[a] if s == -1 else s
+                    for a, s in member_shape.items()
+                }
+                for m, member_shape in self.sample_shape.items()
+            },
             sample_id=self.sample_id,
             blocks={
-                m: Block(
-                    sample_shape=self.sample_shape[m],
-                    inner_slice=b.inner_slice,
-                    halo=b.halo,
-                    block_index=b.block_index,
-                    blocks_in_sample=b.blocks_in_sample,
-                    data=data[m],
-                )
-                for m, b in self.blocks.items()
+                m: Block.from_meta(b, data=data[m]) for m, b in self.blocks.items()
             },
             stat=stat,
             block_index=self.block_index,
             blocks_in_sample=self.blocks_in_sample,
         )
```

### Comparing `bioimageio.core-0.6.1/bioimageio/core/stat_calculators.py` & `bioimageio.core-0.6.2/bioimageio/core/stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/stat_measures.py` & `bioimageio.core-0.6.2/bioimageio/core/stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/tensor.py` & `bioimageio.core-0.6.2/bioimageio/core/tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/utils/testing.py` & `bioimageio.core-0.6.2/bioimageio/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/weight_converter/keras/_tensorflow.py` & `bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_onnx.py` & `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_torchscript.py` & `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio/core/weight_converter/torch/_utils.py` & `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.2/bioimageio.core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
-        Python specific core utilities for [bioimage.io]("https://bioimage.io") resources (in particular models).
+        Python specific core utilities for bioimage.io resources (in particular models).
         
         ## Installation
         
         ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
         
@@ -74,15 +74,15 @@
         mamba env create -f dev/env.yaml
         mamba activate core
         pip install -e . --no-deps
         ```
         
         There are different environment files available that only install tensorflow or pytorch as dependencies.
         
-        ## 💻 Command Line
+        ## 💻 Use the Command Line Interface
         
         `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
         You can list all the available commands via:
         
         ```console
         bioimageio
         ```
@@ -109,32 +109,38 @@
         
         ```console
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
         
         `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
-        ## From python
+        ## 🐍 Use in Python
         
         `bioimageio.core` is a python package that implements prediction with bioimageio models
         including standardized pre- and postprocessing operations.
         These models are described by---and can be loaded with---the bioimageio.spec package.
         
         In addition bioimageio.core provides functionality to convert model weight formats.
         
         To get an overview of this functionality, check out these example notebooks:
         
         * [model creation/loading with bioimageio.spec](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_use/load_model_and_create_your_own.ipynb)
         
+        and the [developer documentation](https://bioimage-io.github.io/core-bioimage-io-python/bioimageio/core.html).
+        
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.2
+        
+        * Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
+        
         ### 0.6.1
         
         * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
         
         ### 0.6.0
         
         * add compatibility with new bioimageio.spec 0.5 (0.5.2post1)
```

### Comparing `bioimageio.core-0.6.1/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.6.2/bioimageio.core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 bioimageio/core/_op_base.py
 bioimageio/core/_prediction_pipeline.py
 bioimageio/core/_resource_tests.py
 bioimageio/core/_settings.py
 bioimageio/core/axis.py
 bioimageio/core/block.py
 bioimageio/core/block_meta.py
+bioimageio/core/commands.py
 bioimageio/core/common.py
 bioimageio/core/dataset.py
 bioimageio/core/digest_spec.py
 bioimageio/core/io.py
 bioimageio/core/prediction.py
 bioimageio/core/proc_ops.py
 bioimageio/core/proc_setup.py
```

### Comparing `bioimageio.core-0.6.1/pyproject.toml` & `bioimageio.core-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/scripts/setup_dev_env.py` & `bioimageio.core-0.6.2/scripts/setup_dev_env.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/scripts/show_diff.py` & `bioimageio.core-0.6.2/scripts/show_diff.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/setup.py` & `bioimageio.core-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         "fire",
         "imageio>=2.5",
         "loguru",
         "numpy",
         "pydantic-settings",
         "pydantic",
         "python-dotenv",
+        "requests",
         "ruyaml",
         "tqdm",
         "typing-extensions",
         "xarray",
     ],
     include_package_data=True,
     extras_require={
```

### Comparing `bioimageio.core-0.6.1/tests/test_bioimageio_spec_version.py` & `bioimageio.core-0.6.2/tests/test_bioimageio_spec_version.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_cli.py` & `bioimageio.core-0.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_digest_spec.py` & `bioimageio.core-0.6.2/tests/test_digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_prediction.py` & `bioimageio.core-0.6.2/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_prediction_pipeline.py` & `bioimageio.core-0.6.2/tests/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_prediction_pipeline_device_management.py` & `bioimageio.core-0.6.2/tests/test_prediction_pipeline_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_proc_ops.py` & `bioimageio.core-0.6.2/tests/test_proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_resource_tests.py` & `bioimageio.core-0.6.2/tests/test_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_stat_calculators.py` & `bioimageio.core-0.6.2/tests/test_stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_stat_measures.py` & `bioimageio.core-0.6.2/tests/test_stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/test_tensor.py` & `bioimageio.core-0.6.2/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.6.2/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/weight_converter/test_add_weights.py` & `bioimageio.core-0.6.2/tests/weight_converter/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/weight_converter/torch/test_onnx.py` & `bioimageio.core-0.6.2/tests/weight_converter/torch/test_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.1/tests/weight_converter/torch/test_torchscript.py` & `bioimageio.core-0.6.2/tests/weight_converter/torch/test_torchscript.py`

 * *Files identical despite different names*

