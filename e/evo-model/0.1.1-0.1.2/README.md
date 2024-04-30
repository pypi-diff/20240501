# Comparing `tmp/evo-model-0.1.1.tar.gz` & `tmp/evo_model-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo-model-0.1.1.tar", last modified: Tue Feb 27 09:53:48 2024, max compression
+gzip compressed data, was "evo_model-0.1.2.tar", last modified: Tue Apr 30 22:36:34 2024, max compression
```

## Comparing `evo-model-0.1.1.tar` & `evo_model-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 cirrascale  (1000) cirrascale  (1000)        0 2024-02-27 09:53:48.180411 evo-model-0.1.1/
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)    11338 2024-02-27 08:39:44.000000 evo-model-0.1.1/LICENSE
--rw-r--r--   0 cirrascale  (1000) cirrascale  (1000)     6193 2024-02-27 09:53:48.178411 evo-model-0.1.1/PKG-INFO
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     5824 2024-02-27 08:39:44.000000 evo-model-0.1.1/README.md
-drwxrwxr-x   0 cirrascale  (1000) cirrascale  (1000)        0 2024-02-27 09:53:48.098415 evo-model-0.1.1/evo/
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)      162 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/__init__.py
-drwxrwxr-x   0 cirrascale  (1000) cirrascale  (1000)        0 2024-02-27 09:53:48.118414 evo-model-0.1.1/evo/configs/
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     1592 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/configs/evo-1-131k-base_inference.yml
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     1421 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/configs/evo-1-8k-base_inference.yml
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     3109 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/generation.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     2796 2024-02-27 09:53:28.000000 evo-model-0.1.1/evo/models.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     4349 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/scoring.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     5197 2024-02-27 08:39:44.000000 evo-model-0.1.1/evo/utils.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)       18 2024-02-27 09:53:28.000000 evo-model-0.1.1/evo/version.py
-drwxrwxr-x   0 cirrascale  (1000) cirrascale  (1000)        0 2024-02-27 09:53:48.167412 evo-model-0.1.1/evo_model.egg-info/
--rw-r--r--   0 cirrascale  (1000) cirrascale  (1000)     6193 2024-02-27 09:53:48.000000 evo-model-0.1.1/evo_model.egg-info/PKG-INFO
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)      462 2024-02-27 09:53:48.000000 evo-model-0.1.1/evo_model.egg-info/SOURCES.txt
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)        1 2024-02-27 09:53:48.000000 evo-model-0.1.1/evo_model.egg-info/dependency_links.txt
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)       37 2024-02-27 09:53:48.000000 evo-model-0.1.1/evo_model.egg-info/requires.txt
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)        4 2024-02-27 09:53:48.000000 evo-model-0.1.1/evo_model.egg-info/top_level.txt
-drwxrwxr-x   0 cirrascale  (1000) cirrascale  (1000)        0 2024-02-27 09:53:48.163412 evo-model-0.1.1/scripts/
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     1187 2024-02-27 08:39:44.000000 evo-model-0.1.1/scripts/example_inference.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     2413 2024-02-27 08:39:44.000000 evo-model-0.1.1/scripts/generate.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     5485 2024-02-27 08:39:44.000000 evo-model-0.1.1/scripts/generation_to_folding.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)     2014 2024-02-27 08:39:44.000000 evo-model-0.1.1/scripts/score.py
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)       38 2024-02-27 09:53:48.180411 evo-model-0.1.1/setup.cfg
--rw-rw-r--   0 cirrascale  (1000) cirrascale  (1000)      800 2024-02-27 09:53:28.000000 evo-model-0.1.1/setup.py
+drwxr-xr-x   0 brianhie (10009) hielab   (10004)        0 2024-04-30 22:36:34.001040 evo_model-0.1.2/
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)    11338 2024-02-27 08:39:44.000000 evo_model-0.1.2/LICENSE
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     7235 2024-04-30 22:36:33.997040 evo_model-0.1.2/PKG-INFO
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     6867 2024-04-28 22:42:33.000000 evo_model-0.1.2/README.md
+drwxr-xr-x   0 brianhie (10009) hielab   (10004)        0 2024-04-30 22:36:33.945042 evo_model-0.1.2/evo/
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)      162 2024-02-27 08:39:44.000000 evo_model-0.1.2/evo/__init__.py
+drwxr-xr-x   0 brianhie (10009) hielab   (10004)        0 2024-04-30 22:36:33.954042 evo_model-0.1.2/evo/configs/
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     1292 2024-04-28 22:42:33.000000 evo_model-0.1.2/evo/configs/evo-1-131k-base_inference.yml
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     1108 2024-04-28 22:42:33.000000 evo_model-0.1.2/evo/configs/evo-1-8k-base_inference.yml
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     3109 2024-02-27 08:39:44.000000 evo_model-0.1.2/evo/generation.py
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     2875 2024-04-30 22:34:08.000000 evo_model-0.1.2/evo/models.py
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     4349 2024-04-05 20:16:21.000000 evo_model-0.1.2/evo/scoring.py
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     5197 2024-02-27 08:39:44.000000 evo_model-0.1.2/evo/utils.py
+-rw-r--r--   0 brianhie (10009) hielab   (10004)       18 2024-04-30 22:34:08.000000 evo_model-0.1.2/evo/version.py
+drwxr-xr-x   0 brianhie (10009) hielab   (10004)        0 2024-04-30 22:36:33.993040 evo_model-0.1.2/evo_model.egg-info/
+-rw-r--r--   0 brianhie (10009) hielab   (10004)     7235 2024-04-30 22:36:33.000000 evo_model-0.1.2/evo_model.egg-info/PKG-INFO
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)      462 2024-04-30 22:36:33.000000 evo_model-0.1.2/evo_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)        1 2024-04-30 22:36:33.000000 evo_model-0.1.2/evo_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)       37 2024-04-30 22:36:33.000000 evo_model-0.1.2/evo_model.egg-info/requires.txt
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)        4 2024-04-30 22:36:33.000000 evo_model-0.1.2/evo_model.egg-info/top_level.txt
+drwxr-xr-x   0 brianhie (10009) hielab   (10004)        0 2024-04-30 22:36:33.987041 evo_model-0.1.2/scripts/
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     1187 2024-02-27 08:39:44.000000 evo_model-0.1.2/scripts/example_inference.py
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     2413 2024-02-27 08:39:44.000000 evo_model-0.1.2/scripts/generate.py
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     5485 2024-02-27 08:39:44.000000 evo_model-0.1.2/scripts/generation_to_folding.py
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)     2014 2024-02-27 08:39:44.000000 evo_model-0.1.2/scripts/score.py
+-rw-r--r--   0 brianhie (10009) hielab   (10004)       38 2024-04-30 22:36:34.001040 evo_model-0.1.2/setup.cfg
+-rw-rw-r--   0 brianhie (10009) hielab   (10004)      800 2024-02-27 09:53:28.000000 evo_model-0.1.2/setup.py
```

### Comparing `evo-model-0.1.1/LICENSE` & `evo_model-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/PKG-INFO` & `evo_model-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-Metadata-Version: 2.1
-Name: evo-model
-Version: 0.1.1
-Summary: DNA foundation modeling from molecular to genome scale.
-Home-page: https://github.com/evo-design/evo
-Author: Team Evo
-License: Apache-2.0
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: stripedhyena==0.2.2
-Requires-Dist: biopython
-Requires-Dist: pandas
-
 # Evo: DNA foundation modeling from molecular to genome scale
 
 ![Evo](evo.jpg)
 
 Evo is a biological foundation model capable of long-context modeling and design.
 Evo uses the [StripedHyena architecture](https://github.com/togethercomputer/stripedhyena) to enable modeling of sequences at a single-nucleotide, byte-level resolution with near-linear scaling of compute and memory relative to context length.
 Evo has 7 billion parameters and is trained on OpenGenome, a prokaryotic whole-genome dataset containing ~300 billion tokens.
 
-We describe Evo in the the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://arcinstitute.org/manuscripts/Evo) and in the [accompanying blog post]().
+We describe Evo in the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://www.biorxiv.org/content/10.1101/2024.02.27.582234v1) and in the [accompanying blog post](https://arcinstitute.org/news/blog/evo).
 
 We provide the following model checkpoints:
 | Checkpoint Name                        | Description |
 |----------------------------------------|-------------|
 | `evo-1-8k-base`     | A model pretrained with 8,192 context. We use this model as the base model for molecular-scale finetuning tasks. |
 | `evo-1-131k-base`   | A model pretrained with 131,072 context using `evo-1-8k-base` as the base model. We use this model to reason about and generate sequences at the genome scale. |
 
+## News
+
+
+We identified and fixed an issue related to a wrong permutation of some projections, which affects generation quality. To use the new model revision with HuggingFace, please load as follows:
+```python
+config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, revision="1.1_fix")
+model = AutoModelForCausalLM.from_pretrained(
+    model_name,
+    config=config,
+    trust_remote_code=True,
+    revision="1.1_fix"
+)
+```
+
 ## Contents
 
 - [Setup](#setup)
   - [Requirements](#requirements)
   - [Installation](#installation)
 - [Usage](#usage)
 - [HuggingFace](#huggingface)
+- [Together web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base)
 - [Together API](#together-api)
+- [colab](https://colab.research.google.com/github/evo-design/evo/blob/main/scripts/hello_evo.ipynb)
+- [Playground wrapper](https://evo.nitro.bio/)
 - [Citation](#citation)
 
 ## Setup
 
 ### Requirements
 
 Evo is based on [StripedHyena](https://github.com/togethercomputer/stripedhyena/tree/main).
 
 Evo uses [FlashAttention-2](https://github.com/Dao-AILab/flash-attention), which may not work on all GPU architectures.
 Please consult the [FlashAttention GitHub repository](https://github.com/Dao-AILab/flash-attention#installation-and-features) for the current list of supported GPUs.
 
-Make sure to install the correct [PyTorch version is installed](https://pytorch.org/) on your system.
+Make sure to install the correct [PyTorch version](https://pytorch.org/) on your system.
 
 ### Installation
 
 You can install Evo using `pip`
 ```bash
 pip install evo-model
 ```
@@ -105,15 +108,15 @@
     --n-samples 10 \
     --n-tokens 100 \
     --temperature 1. \
     --top-k 4 \
     --device cuda:0
 ```
 
-We also provide an [example script](scripts/generate.py) for using the model to score the log-likelihoods of a set of sequences.
+We also provide an [example script](scripts/score.py) for using the model to score the log-likelihoods of a set of sequences.
 ```bash
 python -m scripts.score \
     --input-fasta examples/example_seqs.fasta \
     --output-tsv scores.tsv \
     --model-name 'evo-1-131k-base' \
     --device cuda:0
 ```
@@ -135,15 +138,18 @@
     trust_remote_code=True,
 )
 ```
 
 
 ## Together API
 
-Evo is also available via an API by [TogetherAI](https://www.together.ai/).
+Evo is available through Together AI with a [web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base), where you can generate DNA sequences with a chat-like interface.
+
+For more detailed or batch workflows, you can call the Together API with a simple example below.
+
 
 ```python
 import openai
 import os
 
 # Fill in your API information here.
 client = openai.OpenAI(
@@ -173,15 +179,17 @@
 ```
 
 ## Citation
 
 Please cite the following preprint when referencing Evo.
 
 ```
-@article{nguyen2024sequence,
-   author = {Eric Nguyen and Michael Poli and Matthew G. Durrant and Armin W. Thomas and Brian Kang and Jeremy Sullivan and Madelena Y. Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A. Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D. Hsu and Brian L. Hie},
-   journal = {Arc Institute manuscripts},
-   title = {Sequence modeling and design from molecular to genome scale with Evo},
-   url = {https://arcinstitute.org/manuscripts/Evo},
-   year = {2024},
+@article {nguyen2024sequence,
+    author = {Eric Nguyen and Michael Poli and Matthew G Durrant and Armin W Thomas and Brian Kang and Jeremy Sullivan and Madelena Y Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D Hsu and Brian L Hie},
+    title = {Sequence modeling and design from molecular to genome scale with Evo},
+    year = {2024},
+    doi = {10.1101/2024.02.27.582234},
+    publisher = {Cold Spring Harbor Laboratory},
+    URL = {https://www.biorxiv.org/content/early/2024/02/27/2024.02.27.582234},
+    journal = {bioRxiv}
 }
 ```
```

### Comparing `evo-model-0.1.1/README.md` & `evo_model-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,74 @@
+Metadata-Version: 2.1
+Name: evo-model
+Version: 0.1.2
+Summary: DNA foundation modeling from molecular to genome scale.
+Home-page: https://github.com/evo-design/evo
+Author: Team Evo
+License: Apache-2.0
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: stripedhyena==0.2.2
+Requires-Dist: biopython
+Requires-Dist: pandas
+
 # Evo: DNA foundation modeling from molecular to genome scale
 
 ![Evo](evo.jpg)
 
 Evo is a biological foundation model capable of long-context modeling and design.
 Evo uses the [StripedHyena architecture](https://github.com/togethercomputer/stripedhyena) to enable modeling of sequences at a single-nucleotide, byte-level resolution with near-linear scaling of compute and memory relative to context length.
 Evo has 7 billion parameters and is trained on OpenGenome, a prokaryotic whole-genome dataset containing ~300 billion tokens.
 
-We describe Evo in the the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://arcinstitute.org/manuscripts/Evo) and in the [accompanying blog post]().
+We describe Evo in the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://www.biorxiv.org/content/10.1101/2024.02.27.582234v1) and in the [accompanying blog post](https://arcinstitute.org/news/blog/evo).
 
 We provide the following model checkpoints:
 | Checkpoint Name                        | Description |
 |----------------------------------------|-------------|
 | `evo-1-8k-base`     | A model pretrained with 8,192 context. We use this model as the base model for molecular-scale finetuning tasks. |
 | `evo-1-131k-base`   | A model pretrained with 131,072 context using `evo-1-8k-base` as the base model. We use this model to reason about and generate sequences at the genome scale. |
 
+## News
+
+
+We identified and fixed an issue related to a wrong permutation of some projections, which affects generation quality. To use the new model revision with HuggingFace, please load as follows:
+```python
+config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, revision="1.1_fix")
+model = AutoModelForCausalLM.from_pretrained(
+    model_name,
+    config=config,
+    trust_remote_code=True,
+    revision="1.1_fix"
+)
+```
+
 ## Contents
 
 - [Setup](#setup)
   - [Requirements](#requirements)
   - [Installation](#installation)
 - [Usage](#usage)
 - [HuggingFace](#huggingface)
+- [Together web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base)
 - [Together API](#together-api)
+- [colab](https://colab.research.google.com/github/evo-design/evo/blob/main/scripts/hello_evo.ipynb)
+- [Playground wrapper](https://evo.nitro.bio/)
 - [Citation](#citation)
 
 ## Setup
 
 ### Requirements
 
 Evo is based on [StripedHyena](https://github.com/togethercomputer/stripedhyena/tree/main).
 
 Evo uses [FlashAttention-2](https://github.com/Dao-AILab/flash-attention), which may not work on all GPU architectures.
 Please consult the [FlashAttention GitHub repository](https://github.com/Dao-AILab/flash-attention#installation-and-features) for the current list of supported GPUs.
 
-Make sure to install the correct [PyTorch version is installed](https://pytorch.org/) on your system.
+Make sure to install the correct [PyTorch version](https://pytorch.org/) on your system.
 
 ### Installation
 
 You can install Evo using `pip`
 ```bash
 pip install evo-model
 ```
@@ -91,15 +122,15 @@
     --n-samples 10 \
     --n-tokens 100 \
     --temperature 1. \
     --top-k 4 \
     --device cuda:0
 ```
 
-We also provide an [example script](scripts/generate.py) for using the model to score the log-likelihoods of a set of sequences.
+We also provide an [example script](scripts/score.py) for using the model to score the log-likelihoods of a set of sequences.
 ```bash
 python -m scripts.score \
     --input-fasta examples/example_seqs.fasta \
     --output-tsv scores.tsv \
     --model-name 'evo-1-131k-base' \
     --device cuda:0
 ```
@@ -121,15 +152,18 @@
     trust_remote_code=True,
 )
 ```
 
 
 ## Together API
 
-Evo is also available via an API by [TogetherAI](https://www.together.ai/).
+Evo is available through Together AI with a [web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base), where you can generate DNA sequences with a chat-like interface.
+
+For more detailed or batch workflows, you can call the Together API with a simple example below.
+
 
 ```python
 import openai
 import os
 
 # Fill in your API information here.
 client = openai.OpenAI(
@@ -159,15 +193,17 @@
 ```
 
 ## Citation
 
 Please cite the following preprint when referencing Evo.
 
 ```
-@article{nguyen2024sequence,
-   author = {Eric Nguyen and Michael Poli and Matthew G. Durrant and Armin W. Thomas and Brian Kang and Jeremy Sullivan and Madelena Y. Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A. Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D. Hsu and Brian L. Hie},
-   journal = {Arc Institute manuscripts},
-   title = {Sequence modeling and design from molecular to genome scale with Evo},
-   url = {https://arcinstitute.org/manuscripts/Evo},
-   year = {2024},
+@article {nguyen2024sequence,
+    author = {Eric Nguyen and Michael Poli and Matthew G Durrant and Armin W Thomas and Brian Kang and Jeremy Sullivan and Madelena Y Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D Hsu and Brian L Hie},
+    title = {Sequence modeling and design from molecular to genome scale with Evo},
+    year = {2024},
+    doi = {10.1101/2024.02.27.582234},
+    publisher = {Cold Spring Harbor Laboratory},
+    URL = {https://www.biorxiv.org/content/early/2024/02/27/2024.02.27.582234},
+    journal = {bioRxiv}
 }
-```
+```
```

### Comparing `evo-model-0.1.1/evo/configs/evo-1-131k-base_inference.yml` & `evo_model-0.1.2/evo/configs/evo-1-131k-base_inference.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 vocab_size: 512
 hidden_size: 4096
 num_filters: 4096
 max_sequence_len: 8192
 attn_layer_idxs: [8, 16, 24]
 hyena_layer_idxs: [0, 1, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13, 14, 15, 17, 18, 19, 20, 21, 22, 23, 25, 26, 27, 28, 29, 30, 31]
 num_layers: 32
-short_filter_length: 3  # change name
+short_filter_length: 3  
 num_attention_heads: 32
 short_filter_bias: True
 mlp_init_method: torch.nn.init.zeros_
 mlp_output_init_method: torch.nn.init.zeros_
-eps: 1.0e-6 # 0.00001
-state_size: 8  # state size
-inner_size_multiple_of: 16  # for gated mlp.  for SH 7B it's 16 (default)
-smeared_gqa: False  # what is this???
+eps: 1.0e-6 
+state_size: 8 
+inner_size_multiple_of: 16  # force GLU inner_size to be a multiple of 
+smeared_gqa: False  
 make_vocab_size_divisible_by: 8
 log_intermediate_values: False
-proj_groups: 1  # dont use
-hyena_filter_groups: 1  # dont use
-split_k0: True  # dummy
+proj_groups: 1  # GQA
+hyena_filter_groups: 1  
+split_k0: True  
 model_parallel_size: 1
 pile_parallel_size: 1
-tie_embeddings: True  # we do use
+tie_embeddings: True  
 inner_mlp_size: null  # set to None, so it auto-fills
 mha_out_proj_bias: True
 qkv_proj_bias: True
-final_norm: True  # need, it's post norm true
+final_norm: True  
 rng_fork: False
 use_flash_attn: True
-use_flash_rmsnorm: False  # not sure about this one, may not matter
-use_flash_depthwise: False  # dont use
-use_flashfft: False  # dont use
-column_split: True  # False  Doesnt seem to make a diff
+use_flash_rmsnorm: False  
+use_flash_depthwise: False 
+use_flashfft: False
+column_split: True  # only affects outputs when proj_groups > 1
 inference_mode: True
-tokenizer_type: CharLevelTokenizer  # HFAutoTokenizer
-# vocab_file: "/mnt/spring/tmp/recurrent-inference/tokenizers/mistral/"  # look into savanna tokenizer init
-prefill_style: fft  # need to try out
+tokenizer_type: CharLevelTokenizer  
+prefill_style: fft  
 mlp_activation: gelu
 use_interpolated_rotary_pos_emb: true  # turn this one for linear interpolated context extension
-rotary_emb_scaling_factor: 16  # extension factor over pretraining length
+rotary_emb_scaling_factor: 16  # scaling factor for time indices in rotary embeddings
```

### Comparing `evo-model-0.1.1/evo/configs/evo-1-8k-base_inference.yml` & `evo_model-0.1.2/evo/configs/evo-1-8k-base_inference.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 vocab_size: 512
 hidden_size: 4096
 num_filters: 4096
 max_sequence_len: 8192
 attn_layer_idxs: [8, 16, 24]
 hyena_layer_idxs: [0, 1, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13, 14, 15, 17, 18, 19, 20, 21, 22, 23, 25, 26, 27, 28, 29, 30, 31]
 num_layers: 32
-short_filter_length: 3  # change name
+short_filter_length: 3  
 num_attention_heads: 32
 short_filter_bias: True
 mlp_init_method: torch.nn.init.zeros_
 mlp_output_init_method: torch.nn.init.zeros_
-eps: 1.0e-6 # 0.00001
-state_size: 8  # state size
-inner_size_multiple_of: 16  # for gated mlp.  for SH 7B it's 16 (default)
-smeared_gqa: False  # what is this???
+eps: 1.0e-6 
+state_size: 8 
+inner_size_multiple_of: 16  # force GLU inner_size to be a multiple of
+smeared_gqa: False  
 make_vocab_size_divisible_by: 8
 log_intermediate_values: False
-proj_groups: 1  # dont use
-hyena_filter_groups: 1  # dont use
-split_k0: True  # dummy
+proj_groups: 1  # GQA
+hyena_filter_groups: 1  
+split_k0: True  
 model_parallel_size: 1
 pile_parallel_size: 1
-tie_embeddings: True  # we do use
+tie_embeddings: True  
 inner_mlp_size: null  # set to None, so it auto-fills
 mha_out_proj_bias: True
 qkv_proj_bias: True
-final_norm: True  # need, it's post norm true
+final_norm: True  
 rng_fork: False
 use_flash_attn: True
-use_flash_rmsnorm: False  # not sure about this one, may not matter
-use_flash_depthwise: False  # dont use
-use_flashfft: False  # dont use
-column_split: True  # False  Doesnt seem to make a diff
+use_flash_rmsnorm: False  
+use_flash_depthwise: False 
+use_flashfft: False
+column_split: True  # only affects outputs when proj_groups > 1
 inference_mode: True
-tokenizer_type: CharLevelTokenizer  # HFAutoTokenizer
-# vocab_file: "/mnt/spring/tmp/recurrent-inference/tokenizers/mistral/"  # look into savanna tokenizer init
-prefill_style: fft  # need to try out
+tokenizer_type: CharLevelTokenizer  
+prefill_style: fft  
 mlp_activation: gelu
```

### Comparing `evo-model-0.1.1/evo/generation.py` & `evo_model-0.1.2/evo/generation.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/evo/models.py` & `evo_model-0.1.2/evo/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,23 +67,28 @@
 
     # Map model name to HuggingFace model name.
 
     hf_model_name = HF_MODEL_NAME_MAP[model_name]
 
     # Load model config.
 
-    model_config = AutoConfig.from_pretrained(hf_model_name, trust_remote_code=True)
+    model_config = AutoConfig.from_pretrained(
+        hf_model_name,
+        trust_remote_code=True,
+        revision='1.1_fix',
+    )
     model_config.use_cache = True
 
     # Load model.
 
     model = AutoModelForCausalLM.from_pretrained(
         hf_model_name,
         config=model_config,
         trust_remote_code=True,
+        revision='1.1_fix',
     )
 
     # Load model state dict & cleanup.
 
     state_dict = model.backbone.state_dict()
     del model
     del model_config
```

### Comparing `evo-model-0.1.1/evo/scoring.py` & `evo_model-0.1.2/evo/scoring.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/evo/utils.py` & `evo_model-0.1.2/evo/utils.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/evo_model.egg-info/PKG-INFO` & `evo_model-0.1.2/evo_model.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-model
-Version: 0.1.1
+Version: 0.1.2
 Summary: DNA foundation modeling from molecular to genome scale.
 Home-page: https://github.com/evo-design/evo
 Author: Team Evo
 License: Apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,42 +16,59 @@
 
 ![Evo](evo.jpg)
 
 Evo is a biological foundation model capable of long-context modeling and design.
 Evo uses the [StripedHyena architecture](https://github.com/togethercomputer/stripedhyena) to enable modeling of sequences at a single-nucleotide, byte-level resolution with near-linear scaling of compute and memory relative to context length.
 Evo has 7 billion parameters and is trained on OpenGenome, a prokaryotic whole-genome dataset containing ~300 billion tokens.
 
-We describe Evo in the the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://arcinstitute.org/manuscripts/Evo) and in the [accompanying blog post]().
+We describe Evo in the paper [“Sequence modeling and design from molecular to genome scale with Evo”](https://www.biorxiv.org/content/10.1101/2024.02.27.582234v1) and in the [accompanying blog post](https://arcinstitute.org/news/blog/evo).
 
 We provide the following model checkpoints:
 | Checkpoint Name                        | Description |
 |----------------------------------------|-------------|
 | `evo-1-8k-base`     | A model pretrained with 8,192 context. We use this model as the base model for molecular-scale finetuning tasks. |
 | `evo-1-131k-base`   | A model pretrained with 131,072 context using `evo-1-8k-base` as the base model. We use this model to reason about and generate sequences at the genome scale. |
 
+## News
+
+
+We identified and fixed an issue related to a wrong permutation of some projections, which affects generation quality. To use the new model revision with HuggingFace, please load as follows:
+```python
+config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, revision="1.1_fix")
+model = AutoModelForCausalLM.from_pretrained(
+    model_name,
+    config=config,
+    trust_remote_code=True,
+    revision="1.1_fix"
+)
+```
+
 ## Contents
 
 - [Setup](#setup)
   - [Requirements](#requirements)
   - [Installation](#installation)
 - [Usage](#usage)
 - [HuggingFace](#huggingface)
+- [Together web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base)
 - [Together API](#together-api)
+- [colab](https://colab.research.google.com/github/evo-design/evo/blob/main/scripts/hello_evo.ipynb)
+- [Playground wrapper](https://evo.nitro.bio/)
 - [Citation](#citation)
 
 ## Setup
 
 ### Requirements
 
 Evo is based on [StripedHyena](https://github.com/togethercomputer/stripedhyena/tree/main).
 
 Evo uses [FlashAttention-2](https://github.com/Dao-AILab/flash-attention), which may not work on all GPU architectures.
 Please consult the [FlashAttention GitHub repository](https://github.com/Dao-AILab/flash-attention#installation-and-features) for the current list of supported GPUs.
 
-Make sure to install the correct [PyTorch version is installed](https://pytorch.org/) on your system.
+Make sure to install the correct [PyTorch version](https://pytorch.org/) on your system.
 
 ### Installation
 
 You can install Evo using `pip`
 ```bash
 pip install evo-model
 ```
@@ -105,15 +122,15 @@
     --n-samples 10 \
     --n-tokens 100 \
     --temperature 1. \
     --top-k 4 \
     --device cuda:0
 ```
 
-We also provide an [example script](scripts/generate.py) for using the model to score the log-likelihoods of a set of sequences.
+We also provide an [example script](scripts/score.py) for using the model to score the log-likelihoods of a set of sequences.
 ```bash
 python -m scripts.score \
     --input-fasta examples/example_seqs.fasta \
     --output-tsv scores.tsv \
     --model-name 'evo-1-131k-base' \
     --device cuda:0
 ```
@@ -135,15 +152,18 @@
     trust_remote_code=True,
 )
 ```
 
 
 ## Together API
 
-Evo is also available via an API by [TogetherAI](https://www.together.ai/).
+Evo is available through Together AI with a [web UI](https://api.together.xyz/playground/language/togethercomputer/evo-1-131k-base), where you can generate DNA sequences with a chat-like interface.
+
+For more detailed or batch workflows, you can call the Together API with a simple example below.
+
 
 ```python
 import openai
 import os
 
 # Fill in your API information here.
 client = openai.OpenAI(
@@ -173,15 +193,17 @@
 ```
 
 ## Citation
 
 Please cite the following preprint when referencing Evo.
 
 ```
-@article{nguyen2024sequence,
-   author = {Eric Nguyen and Michael Poli and Matthew G. Durrant and Armin W. Thomas and Brian Kang and Jeremy Sullivan and Madelena Y. Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A. Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D. Hsu and Brian L. Hie},
-   journal = {Arc Institute manuscripts},
-   title = {Sequence modeling and design from molecular to genome scale with Evo},
-   url = {https://arcinstitute.org/manuscripts/Evo},
-   year = {2024},
+@article {nguyen2024sequence,
+    author = {Eric Nguyen and Michael Poli and Matthew G Durrant and Armin W Thomas and Brian Kang and Jeremy Sullivan and Madelena Y Ng and Ashley Lewis and Aman Patel and Aaron Lou and Stefano Ermon and Stephen A Baccus and Tina Hernandez-Boussard and Christopher Ré and Patrick D Hsu and Brian L Hie},
+    title = {Sequence modeling and design from molecular to genome scale with Evo},
+    year = {2024},
+    doi = {10.1101/2024.02.27.582234},
+    publisher = {Cold Spring Harbor Laboratory},
+    URL = {https://www.biorxiv.org/content/early/2024/02/27/2024.02.27.582234},
+    journal = {bioRxiv}
 }
 ```
```

### Comparing `evo-model-0.1.1/scripts/example_inference.py` & `evo_model-0.1.2/scripts/example_inference.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/scripts/generate.py` & `evo_model-0.1.2/scripts/generate.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/scripts/generation_to_folding.py` & `evo_model-0.1.2/scripts/generation_to_folding.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/scripts/score.py` & `evo_model-0.1.2/scripts/score.py`

 * *Files identical despite different names*

### Comparing `evo-model-0.1.1/setup.py` & `evo_model-0.1.2/setup.py`

 * *Files identical despite different names*

