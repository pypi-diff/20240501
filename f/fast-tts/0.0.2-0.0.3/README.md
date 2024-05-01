# Comparing `tmp/fast_tts-0.0.2.tar.gz` & `tmp/fast_tts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tts-0.0.2.tar", last modified: Tue Apr 30 19:49:09 2024, max compression
+gzip compressed data, was "fast_tts-0.0.3.tar", last modified: Wed May  1 19:00:45 2024, max compression
```

## Comparing `fast_tts-0.0.2.tar` & `fast_tts-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:49:09.120856 fast_tts-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 19:49:05.000000 fast_tts-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 19:49:09.120856 fast_tts-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 19:49:05.000000 fast_tts-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:49:09.120856 fast_tts-0.0.2/fast_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:49:09.120856 fast_tts-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 19:49:05.000000 fast_tts-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.994172 fast_tts-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 19:00:39.000000 fast_tts-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-01 19:00:45.994172 fast_tts-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-01 19:00:39.000000 fast_tts-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.982172 fast_tts-0.0.3/fast_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/fast_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.982172 fast_tts-0.0.3/fast_tts/rvc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.982172 fast_tts-0.0.3/fast_tts/rvc/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/configs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/configs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/configs/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/configs/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/configs/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/audio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50965 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/infer_pack/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/lib/jit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/jit/get_rmvpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/lib/rmvpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/modules/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/train/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/rvc/infer/modules/vc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/vc/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/vc/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/infer/modules/vc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/rvc/rvc_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.986172 fast_tts-0.0.3/fast_tts/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37808 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/api_fast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.990172 fast_tts-0.0.3/fast_tts/tortoise/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.990172 fast_tts-0.0.3/fast_tts/tortoise/models/alias_free_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/alias_free_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/alias_free_torch/act.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/alias_free_torch/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/alias_free_torch/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/arch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27178 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/autoregressive_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/bigvgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/clvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/cvvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/diffusion_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/hifigan_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/random_latent_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48681 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/stream_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42405 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/models/xtransformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/tortoise_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.994172 fast_tts-0.0.3/fast_tts/tortoise/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49438 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/stft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/torch_intermediary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/typical_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-01 19:00:39.000000 fast_tts-0.0.3/fast_tts/tortoise/utils/wav2vec_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.994172 fast_tts-0.0.3/fast_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-01 19:00:45.000000 fast_tts-0.0.3/fast_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-01 19:00:45.000000 fast_tts-0.0.3/fast_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:00:45.000000 fast_tts-0.0.3/fast_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-01 19:00:45.000000 fast_tts-0.0.3/fast_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 19:00:45.000000 fast_tts-0.0.3/fast_tts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:00:45.994172 fast_tts-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-01 19:00:39.000000 fast_tts-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:00:45.994172 fast_tts-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-01 19:00:39.000000 fast_tts-0.0.3/tests/test.py
```

### Comparing `fast_tts-0.0.2/LICENSE` & `fast_tts-0.0.3/LICENSE`

 * *Files identical despite different names*

