# Comparing `tmp/mlx_whisper-0.0.0.dev0.tar.gz` & `tmp/mlx_whisper-0.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_whisper-0.0.0.dev0.tar", last modified: Wed May  1 15:27:41 2024, max compression
+gzip compressed data, was "mlx_whisper-0.0.0.dev1.tar", last modified: Wed May  1 15:50:19 2024, max compression
```

## Comparing `mlx_whisper-0.0.0.dev0.tar` & `mlx_whisper-0.0.0.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:27:41.431222 mlx_whisper-0.0.0.dev0/
--rw-r--r--   0 awnihannun   (504) staff       (20)      170 2024-05-01 15:27:36.000000 mlx_whisper-0.0.0.dev0/MANIFEST.in
--rw-r--r--   0 awnihannun   (504) staff       (20)     3472 2024-05-01 15:27:41.430931 mlx_whisper-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 awnihannun   (504) staff       (20)     2933 2024-05-01 15:07:15.000000 mlx_whisper-0.0.0.dev0/README.md
-drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:27:41.426593 mlx_whisper-0.0.0.dev0/mlx_whisper/
--rw-r--r--   0 awnihannun   (504) staff       (20)      148 2024-05-01 14:38:47.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/__init__.py
-drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:27:41.429637 mlx_whisper-0.0.0.dev0/mlx_whisper/assets/
--rw-r--r--   0 awnihannun   (504) staff       (20)   835554 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/assets/gpt2.tiktoken
--rw-r--r--   0 awnihannun   (504) staff       (20)     4271 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/assets/mel_filters.npz
--rw-r--r--   0 awnihannun   (504) staff       (20)   816730 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/assets/multilingual.tiktoken
--rw-r--r--   0 awnihannun   (504) staff       (20)     5080 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/audio.py
--rw-r--r--   0 awnihannun   (504) staff       (20)    28161 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/decoding.py
--rw-r--r--   0 awnihannun   (504) staff       (20)     1190 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/load_models.py
--rw-r--r--   0 awnihannun   (504) staff       (20)       79 2024-05-01 15:09:47.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/requirements.txt
--rw-r--r--   0 awnihannun   (504) staff       (20)    10880 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/timing.py
--rw-r--r--   0 awnihannun   (504) staff       (20)    12407 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/tokenizer.py
--rw-r--r--   0 awnihannun   (504) staff       (20)    10592 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/torch_whisper.py
--rw-r--r--   0 awnihannun   (504) staff       (20)    22942 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/transcribe.py
--rw-r--r--   0 awnihannun   (504) staff       (20)       63 2024-05-01 15:19:06.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/version.py
--rw-r--r--   0 awnihannun   (504) staff       (20)     8669 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev0/mlx_whisper/whisper.py
-drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:27:41.430586 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/
--rw-r--r--   0 awnihannun   (504) staff       (20)     3472 2024-05-01 15:27:41.000000 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (504) staff       (20)      586 2024-05-01 15:27:41.000000 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (504) staff       (20)        1 2024-05-01 15:27:41.000000 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (504) staff       (20)       79 2024-05-01 15:27:41.000000 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (504) staff       (20)       12 2024-05-01 15:27:41.000000 mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (504) staff       (20)       38 2024-05-01 15:27:41.431278 mlx_whisper-0.0.0.dev0/setup.cfg
--rw-r--r--   0 awnihannun   (504) staff       (20)      865 2024-05-01 15:27:39.000000 mlx_whisper-0.0.0.dev0/setup.py
+drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:50:19.852034 mlx_whisper-0.0.0.dev1/
+-rw-r--r--   0 awnihannun   (504) staff       (20)      170 2024-05-01 15:49:20.000000 mlx_whisper-0.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 awnihannun   (504) staff       (20)     3472 2024-05-01 15:50:19.851698 mlx_whisper-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0 awnihannun   (504) staff       (20)     2933 2024-05-01 15:07:15.000000 mlx_whisper-0.0.0.dev1/README.md
+drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:50:19.848558 mlx_whisper-0.0.0.dev1/mlx_whisper/
+-rw-r--r--   0 awnihannun   (504) staff       (20)      148 2024-05-01 14:38:47.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/__init__.py
+drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:50:19.850855 mlx_whisper-0.0.0.dev1/mlx_whisper/assets/
+-rw-r--r--   0 awnihannun   (504) staff       (20)   835554 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/assets/gpt2.tiktoken
+-rw-r--r--   0 awnihannun   (504) staff       (20)     4271 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/assets/mel_filters.npz
+-rw-r--r--   0 awnihannun   (504) staff       (20)   816730 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/assets/multilingual.tiktoken
+-rw-r--r--   0 awnihannun   (504) staff       (20)     5080 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/audio.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)    28161 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/decoding.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)     1190 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/load_models.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)       79 2024-05-01 15:09:47.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/requirements.txt
+-rw-r--r--   0 awnihannun   (504) staff       (20)    10880 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/timing.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)    12407 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/tokenizer.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)    10592 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/torch_whisper.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)    22942 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/transcribe.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)       64 2024-05-01 15:50:16.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/version.py
+-rw-r--r--   0 awnihannun   (504) staff       (20)     8669 2024-05-01 14:38:10.000000 mlx_whisper-0.0.0.dev1/mlx_whisper/whisper.py
+drwxr-xr-x   0 awnihannun   (504) staff       (20)        0 2024-05-01 15:50:19.851492 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/
+-rw-r--r--   0 awnihannun   (504) staff       (20)     3472 2024-05-01 15:50:19.000000 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (504) staff       (20)      586 2024-05-01 15:50:19.000000 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (504) staff       (20)        1 2024-05-01 15:50:19.000000 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (504) staff       (20)       79 2024-05-01 15:50:19.000000 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (504) staff       (20)       12 2024-05-01 15:50:19.000000 mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (504) staff       (20)       38 2024-05-01 15:50:19.852075 mlx_whisper-0.0.0.dev1/setup.cfg
+-rw-r--r--   0 awnihannun   (504) staff       (20)      896 2024-05-01 15:49:27.000000 mlx_whisper-0.0.0.dev1/setup.py
```

### Comparing `mlx_whisper-0.0.0.dev0/PKG-INFO` & `mlx_whisper-0.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-whisper
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Summary: OpenAI Whisper on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_whisper-0.0.0.dev0/README.md` & `mlx_whisper-0.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/assets/gpt2.tiktoken` & `mlx_whisper-0.0.0.dev1/mlx_whisper/assets/gpt2.tiktoken`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/assets/mel_filters.npz` & `mlx_whisper-0.0.0.dev1/mlx_whisper/assets/mel_filters.npz`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/assets/multilingual.tiktoken` & `mlx_whisper-0.0.0.dev1/mlx_whisper/assets/multilingual.tiktoken`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/audio.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/decoding.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/decoding.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/load_models.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/load_models.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/timing.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/tokenizer.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/torch_whisper.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/torch_whisper.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/transcribe.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper/whisper.py` & `mlx_whisper-0.0.0.dev1/mlx_whisper/whisper.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/PKG-INFO` & `mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-whisper
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Summary: OpenAI Whisper on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_whisper-0.0.0.dev0/mlx_whisper.egg-info/SOURCES.txt` & `mlx_whisper-0.0.0.dev1/mlx_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.0.0.dev0/setup.py` & `mlx_whisper-0.0.0.dev1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,10 @@
     readme="README.md",
     author_email="mlx@group.apple.com",
     author="MLX Contributors",
     url="https://github.com/ml-explore/mlx-examples",
     license="MIT",
     install_requires=requirements,
     packages=find_packages(),
+    include_package_data=True,
     python_requires=">=3.8",
 )
```

