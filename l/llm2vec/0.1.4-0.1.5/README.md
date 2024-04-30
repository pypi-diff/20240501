# Comparing `tmp/llm2vec-0.1.4.tar.gz` & `tmp/llm2vec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.4.tar", last modified: Wed Apr 17 17:33:10 2024, max compression
+gzip compressed data, was "llm2vec-0.1.5.tar", last modified: Tue Apr 30 22:32:19 2024, max compression
```

## Comparing `llm2vec-0.1.4.tar` & `llm2vec-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.747887 llm2vec-0.1.4/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.4/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6673 2024-04-17 17:33:10.748045 llm2vec-0.1.4/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6223 2024-04-17 17:32:47.000000 llm2vec-0.1.4/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.721327 llm2vec-0.1.4/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14576 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/llm2vec.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.747439 llm2vec-0.1.4/llm2vec/models/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/models/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.4/llm2vec/models/attn_mask_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7678 2024-04-17 17:32:47.000000 llm2vec-0.1.4/llm2vec/models/bidirectional_llama.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.4/llm2vec/models/bidirectional_mistral.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-17 17:33:01.000000 llm2vec-0.1.4/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-17 17:33:10.744124 llm2vec-0.1.4/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6673 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      417 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.4/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-17 17:33:10.000000 llm2vec-0.1.4/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-17 17:33:10.748655 llm2vec-0.1.4/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.4/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.870986 llm2vec-0.1.5/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.5/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8941 2024-04-30 22:32:19.871323 llm2vec-0.1.5/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8491 2024-04-30 22:31:54.000000 llm2vec-0.1.5/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.852001 llm2vec-0.1.5/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/__init__.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.861701 llm2vec-0.1.5/llm2vec/dataset/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6340 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/E5Data.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       26 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1123 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/dataset.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      723 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/experiment_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    15447 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.865363 llm2vec-0.1.5/llm2vec/loss/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/HardNegativeNLLLoss.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/loss_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/utils.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.869896 llm2vec-0.1.5/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7760 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.5/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.857753 llm2vec-0.1.5/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8941 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      661 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.5/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-30 22:32:19.872548 llm2vec-0.1.5/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.5/setup.py
```

### Comparing `llm2vec-0.1.4/LICENSE` & `llm2vec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.4/PKG-INFO` & `llm2vec-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.4
+Version: 0.1.5
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,19 @@
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
+**************************** **Updates** ****************************
+
+
+* 30/04: We release LLM2Vec transformed Meta-Llama-3 checkpoints. See our [HuggingFace collection](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34) for both [supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) and [unsupervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse) variants.
+
 ## Installation
 To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
 pip install flash-attn --no-build-isolation
 ```
@@ -39,18 +44,18 @@
 
 ```bash
 pip install -e .
 pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
-LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
+LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
-Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
+Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
 Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
@@ -107,30 +112,60 @@
 print(cos_sim)
 """
 tensor([[0.5485, 0.0551],
         [0.0565, 0.5425]])
 """
 ```
 
+More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
+
 ## Model List
+- ### Meta-Llama-3-8B
+  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp)
+  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
 - ### Mistral-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse) (Unsupervised state-of-the-art on MTEB)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised)
 - ### Llama-2-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised)
 - ### Sheared-Llama-1.3B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised)
 
 ## Training 
-Training code will be available soon.
+### MNTP training
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+
+```bash
+python experiments/run_mntp.py train_configs/mntp/Mistral.json
+```
+
+The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "dataset_name": "wikitext",
+    "dataset_config_name": "wikitext-103-raw-v1",
+    "mask_token_type": "blank",
+    "data_collator_type": "all_mask",
+    "mlm_probability": 0.8,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2"
+    // ....
+}
+```
+
+Similar configurations are also available for [Llama-2-7B](train_configs/mntp/Llama.json) and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ## Citation
 If you find our work helpful, please cite us:
 ```bibtex
 @article{llm2vec,
       title={{LLM2Vec}: {L}arge Language Models Are Secretly Powerful Text Encoders}, 
       author={Parishad BehnamGhader and Vaibhav Adlakha and Marius Mosbach and Dzmitry Bahdanau and Nicolas Chapados and Siva Reddy},
```

### Comparing `llm2vec-0.1.4/README.md` & `llm2vec-0.1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
+**************************** **Updates** ****************************
+
+
+* 30/04: We release LLM2Vec transformed Meta-Llama-3 checkpoints. See our [HuggingFace collection](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34) for both [supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) and [unsupervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse) variants.
+
 ## Installation
 To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
 pip install flash-attn --no-build-isolation
 ```
@@ -24,18 +29,18 @@
 
 ```bash
 pip install -e .
 pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
-LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
+LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
-Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
+Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
 Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
@@ -92,30 +97,60 @@
 print(cos_sim)
 """
 tensor([[0.5485, 0.0551],
         [0.0565, 0.5425]])
 """
 ```
 
+More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
+
 ## Model List
+- ### Meta-Llama-3-8B
+  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp)
+  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
 - ### Mistral-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse) (Unsupervised state-of-the-art on MTEB)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised)
 - ### Llama-2-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised)
 - ### Sheared-Llama-1.3B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised)
 
 ## Training 
-Training code will be available soon.
+### MNTP training
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+
+```bash
+python experiments/run_mntp.py train_configs/mntp/Mistral.json
+```
+
+The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "dataset_name": "wikitext",
+    "dataset_config_name": "wikitext-103-raw-v1",
+    "mask_token_type": "blank",
+    "data_collator_type": "all_mask",
+    "mlm_probability": 0.8,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2"
+    // ....
+}
+```
+
+Similar configurations are also available for [Llama-2-7B](train_configs/mntp/Llama.json) and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ## Citation
 If you find our work helpful, please cite us:
 ```bibtex
 @article{llm2vec,
       title={{LLM2Vec}: {L}arge Language Models Are Secretly Powerful Text Encoders}, 
       author={Parishad BehnamGhader and Vaibhav Adlakha and Marius Mosbach and Dzmitry Bahdanau and Nicolas Chapados and Siva Reddy},
```

### Comparing `llm2vec-0.1.4/llm2vec/llm2vec.py` & `llm2vec-0.1.5/llm2vec/llm2vec.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,36 @@
         super().__init__()
         self.model = model
         self.tokenizer = tokenizer
         self.pooling_mode = pooling_mode
         self.skip_instruction = skip_instruction
         self.max_length = max_length
         self.doc_max_length = doc_max_length
+        self.config = model.config
 
     @classmethod
-    def _get_model_class(cls, config_class_name):
+    def _get_model_class(cls, config_class_name, enable_bidirectional):
+        if not enable_bidirectional:
+            return AutoModel
         if config_class_name == "MistralConfig":
             return MistralBiModel
         elif config_class_name == "LlamaConfig":
             return LlamaBiModel
         else:
-            raise ValueError(f"{config_class_name} is not supported yet.")
+            raise ValueError(
+                f"{config_class_name} is not supported yet with bidirectional models."
+            )
 
     @classmethod
     def from_pretrained(
         cls,
         base_model_name_or_path,
         peft_model_name_or_path=None,
+        merge_peft=False,
+        enable_bidirectional=True,
         **kwargs,
     ):
         # pop out encoder args
         keys = ["pooling_mode", "max_length", "doc_max_length", "skip_instruction"]
         encoder_args = {
             key: kwargs.pop(key, None) for key in keys if kwargs.get(key) is not None
         }
@@ -79,15 +86,17 @@
         tokenizer = AutoTokenizer.from_pretrained(base_model_name_or_path)
         tokenizer.pad_token = tokenizer.eos_token
         tokenizer.padding_side = "left"
 
         config = AutoConfig.from_pretrained(base_model_name_or_path)
         config_class_name = config.__class__.__name__
 
-        model_class = cls._get_model_class(config_class_name)
+        model_class = cls._get_model_class(
+            config_class_name, enable_bidirectional=enable_bidirectional
+        )
         model = model_class.from_pretrained(base_model_name_or_path, **kwargs)
 
         # For special case where config.json and adapter weights are in the same directory
         if hasattr(model, "peft_config"):
             model = PeftModel.from_pretrained(
                 model,
                 base_model_name_or_path,
@@ -95,14 +104,16 @@
             model = model.merge_and_unload()
 
         if peft_model_name_or_path is not None:
             model = PeftModel.from_pretrained(
                 model,
                 peft_model_name_or_path,
             )
+            if merge_peft:
+                model = model.merge_and_unload()
 
         config = {}
         config_addr = (
             peft_model_name_or_path
             if peft_model_name_or_path is not None
             else base_model_name_or_path
         )
@@ -113,28 +124,34 @@
 
         for key, value in encoder_args.items():
             config[key] = value
 
         return cls(model=model, tokenizer=tokenizer, **config)
 
     def prepare_for_tokenization(self, text):
-        def _is_instruct(name):
-            return (
-                ("chat" in name.lower())
-                or ("instruct" in name.lower())
-                or ("sharegpt" in name.lower())
+        if self.model.config._name_or_path == "meta-llama/Meta-Llama-3-8B-Instruct":
+            text = (
+                "<|start_header_id|>user<|end_header_id|>\n\n"
+                + text.strip()
+                + "<|eot_id|>"
             )
-
-        if _is_instruct(self.model.config._name_or_path):
+            return text
+        if self.model.config._name_or_path in [
+            "mistralai/Mistral-7B-Instruct-v0.2",
+            "meta-llama/Llama-2-7b-chat-hf",
+        ]:
             text = "[INST] " + text.strip() + " [/INST]"
-        if (
-            isinstance(self.model.config, LlamaConfig)
-            or isinstance(self.model.config, MistralConfig)
-        ) and self.pooling_mode == "eos_token":
-            text = text.strip() + " </s>"
+        if self.pooling_mode == "eos_token":
+            if self.model.config._name_or_path == "meta-llama/Meta-Llama-3-8B":
+                text = text.strip() + "<|end_of_text|>"
+            elif isinstance(self.model.config, LlamaConfig) or isinstance(
+                self.model.config, MistralConfig
+            ):
+                text = text.strip() + " </s>"
+
         return text
 
     def tokenize(self, texts):
         texts_2 = []
         original_texts = []
         for text in texts:
             t = text.split("!@#$%^&*()")
@@ -273,15 +290,14 @@
             assert isinstance(sentence[1], str)
             concatenated_input_texts.append(
                 self._convert_to_str(sentence[0], sentence[1])
             )
         sentences = concatenated_input_texts
 
         self.eval()
-        show_progress_bar = True
 
         if convert_to_tensor:
             convert_to_numpy = False
 
         length_sorted_idx = np.argsort([-self._text_length(sen) for sen in sentences])
         sentences_sorted = [sentences[idx] for idx in length_sorted_idx]
         all_embeddings = []
@@ -393,7 +409,12 @@
         self,
         new_num_tokens: Optional[int] = None,
         pad_to_multiple_of: Optional[int] = None,
     ) -> nn.Embedding:
         return self.model.resize_token_embeddings(
             new_num_tokens=new_num_tokens, pad_to_multiple_of=pad_to_multiple_of
         )
+
+    def gradient_checkpointing_enable(self, gradient_checkpointing_kwargs=None):
+        self.model.gradient_checkpointing_enable(
+            gradient_checkpointing_kwargs=gradient_checkpointing_kwargs
+        )
```

### Comparing `llm2vec-0.1.4/llm2vec/models/attn_mask_utils.py` & `llm2vec-0.1.5/llm2vec/models/attn_mask_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.4/llm2vec/models/bidirectional_llama.py` & `llm2vec-0.1.5/llm2vec/models/bidirectional_llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,22 @@
     if not _is_package_available("transformers"):
         return False
 
     return version.parse(importlib.metadata.version("transformers")) >= version.parse(
         "4.38.0"
     )
 
+def is_transformers_attn_greater_or_equal_4_40():
+    if not _is_package_available("transformers"):
+        return False
+
+    return version.parse(importlib.metadata.version("transformers")) >= version.parse(
+        "4.40.0"
+    )
+
 
 class ModifiedLlamaAttention(LlamaAttention):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.is_causal = False
 
 
@@ -95,32 +103,40 @@
         )
         self.norm = LlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.gradient_checkpointing = False
 
         # Initialize weights and apply final processing
         self.post_init()
 
-    def _update_causal_mask(self, attention_mask, input_tensor, cache_position):
+    def _update_causal_mask(self, attention_mask, input_tensor, cache_position, past_seen_tokens=None):
         if self.config._attn_implementation == "flash_attention_2":
             if attention_mask is not None and 0.0 in attention_mask:
                 return attention_mask
             return None
 
+        if is_transformers_attn_greater_or_equal_4_40() and self.config._attn_implementation == "sdpa":
+            # For SDPA, when possible, we will rely on its `is_causal` argument instead of its `attn_mask` argument,
+            # in order to dispatch on Flash Attention 2.
+            if AttentionMaskConverter._ignore_causal_mask_sdpa(
+                attention_mask, inputs_embeds=input_tensor, past_key_values_length=past_seen_tokens
+            ):
+                return None
+
         dtype, device = input_tensor.dtype, input_tensor.device
         min_dtype = torch.finfo(dtype).min
         sequence_length = input_tensor.shape[1]
         if hasattr(
             getattr(self.layers[0], "self_attn", {}), "past_key_value"
         ):  # static cache
             target_length = self.config.max_position_embeddings
         else:  # dynamic cache
             target_length = (
                 attention_mask.shape[-1]
                 if isinstance(attention_mask, torch.Tensor)
-                else cache_position[-1] + 1
+                else (cache_position[-1] + 1 if not is_transformers_attn_greater_or_equal_4_40() else past_seen_tokens + sequence_length + 1)
             )
 
         causal_mask = torch.zeros(
             (sequence_length, target_length), dtype=dtype, device=device
         )  # in original implementation - torch.full((sequence_length, target_length), fill_value=min_dtype, dtype=dtype, device=device)
         # Commenting out next 2 lines to disable causal masking
         # if sequence_length != 1:
@@ -160,27 +176,17 @@
                 ] = mask_slice
 
         if (
             self.config._attn_implementation == "sdpa"
             and attention_mask is not None
             and attention_mask.device.type == "cuda"
         ):
-            # TODO: For dynamo, rather use a check on fullgraph=True once this is possible (https://github.com/pytorch/pytorch/pull/120400).
-            is_tracing = (
-                torch.jit.is_tracing()
-                or isinstance(input_tensor, torch.fx.Proxy)
-                or (hasattr(torch, "_dynamo") and torch._dynamo.is_compiling())
+            causal_mask = AttentionMaskConverter._unmask_unattended(
+                causal_mask, min_dtype
             )
-            if not is_tracing and torch.any(attention_mask != 1):
-                # Attend to all tokens in fully masked rows in the causal_mask, for example the relevant first rows when
-                # using left padding. This is required by F.scaled_dot_product_attention memory-efficient attention path.
-                # Details: https://github.com/pytorch/pytorch/issues/110213
-                causal_mask = AttentionMaskConverter._unmask_unattended(
-                    causal_mask, min_dtype
-                )
 
         return causal_mask
 
 
 class LlamaBiForMNTP(LlamaForCausalLM):
     def __init__(self, config):
         LlamaPreTrainedModel.__init__(self, config)
```

### Comparing `llm2vec-0.1.4/llm2vec/models/bidirectional_mistral.py` & `llm2vec-0.1.5/llm2vec/models/bidirectional_mistral.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.4/llm2vec.egg-info/PKG-INFO` & `llm2vec-0.1.5/llm2vec.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.4
+Version: 0.1.5
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,19 @@
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
+**************************** **Updates** ****************************
+
+
+* 30/04: We release LLM2Vec transformed Meta-Llama-3 checkpoints. See our [HuggingFace collection](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34) for both [supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) and [unsupervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse) variants.
+
 ## Installation
 To use LLM2Vec, first install the llm2vec package from PyPI, followed by installing flash-attention:
 
 ```bash
 pip install llm2vec
 pip install flash-attn --no-build-isolation
 ```
@@ -39,18 +44,18 @@
 
 ```bash
 pip install -e .
 pip install flash-attn --no-build-isolation
 ```
 
 ## Getting Started
-LLM2Vec class is a wrapper on top of HuggingFace models to support sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
+LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
-Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method (make sure the `llm2vec` package version is `>=0.1.3`).
+Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
 Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
@@ -107,30 +112,60 @@
 print(cos_sim)
 """
 tensor([[0.5485, 0.0551],
         [0.0565, 0.5425]])
 """
 ```
 
+More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
+
 ## Model List
+- ### Meta-Llama-3-8B
+  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp)
+  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
 - ### Mistral-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse) (Unsupervised state-of-the-art on MTEB)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
+  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised)
 - ### Llama-2-7B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised)
 - ### Sheared-Llama-1.3B
   - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp)
   - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse)
   - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised)
 
 ## Training 
-Training code will be available soon.
+### MNTP training
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+
+```bash
+python experiments/run_mntp.py train_configs/mntp/Mistral.json
+```
+
+The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "dataset_name": "wikitext",
+    "dataset_config_name": "wikitext-103-raw-v1",
+    "mask_token_type": "blank",
+    "data_collator_type": "all_mask",
+    "mlm_probability": 0.8,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2"
+    // ....
+}
+```
+
+Similar configurations are also available for [Llama-2-7B](train_configs/mntp/Llama.json) and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ## Citation
 If you find our work helpful, please cite us:
 ```bibtex
 @article{llm2vec,
       title={{LLM2Vec}: {L}arge Language Models Are Secretly Powerful Text Encoders}, 
       author={Parishad BehnamGhader and Vaibhav Adlakha and Marius Mosbach and Dzmitry Bahdanau and Nicolas Chapados and Siva Reddy},
```

### Comparing `llm2vec-0.1.4/setup.py` & `llm2vec-0.1.5/setup.py`

 * *Files identical despite different names*

