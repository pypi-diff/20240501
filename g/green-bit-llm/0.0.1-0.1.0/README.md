# Comparing `tmp/green-bit-llm-0.0.1.tar.gz` & `tmp/green-bit-llm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green-bit-llm-0.0.1.tar", last modified: Mon Apr 15 07:28:05 2024, max compression
+gzip compressed data, was "green-bit-llm-0.1.0.tar", last modified: Wed May  1 10:53:36 2024, max compression
```

## Comparing `green-bit-llm-0.0.1.tar` & `green-bit-llm-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,47 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-15 07:28:05.523733 green-bit-llm-0.0.1/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-04-07 20:16:16.000000 green-bit-llm-0.0.1/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     2912 2024-04-15 07:28:05.523505 green-bit-llm-0.0.1/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     2175 2024-04-15 07:26:17.000000 green-bit-llm-0.0.1/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-15 07:28:05.522672 green-bit-llm-0.0.1/green_bit_llm/
--rw-r--r--   0 haojin     (501) staff       (20)       33 2024-04-13 21:36:23.000000 green-bit-llm-0.0.1/green_bit_llm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      156 2024-04-11 12:54:16.000000 green-bit-llm-0.0.1/green_bit_llm/enum.py
--rw-r--r--   0 haojin     (501) staff       (20)    17181 2024-04-15 07:26:17.000000 green-bit-llm-0.0.1/green_bit_llm/model.py
--rw-r--r--   0 haojin     (501) staff       (20)     6804 2024-04-11 12:03:59.000000 green-bit-llm-0.0.1/green_bit_llm/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-13 21:36:23.000000 green-bit-llm-0.0.1/green_bit_llm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-15 07:28:05.523239 green-bit-llm-0.0.1/green_bit_llm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     2912 2024-04-15 07:28:05.000000 green-bit-llm-0.0.1/green_bit_llm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)      329 2024-04-15 07:28:05.000000 green-bit-llm-0.0.1/green_bit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-15 07:28:05.000000 green-bit-llm-0.0.1/green_bit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)      165 2024-04-15 07:28:05.000000 green-bit-llm-0.0.1/green_bit_llm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)       14 2024-04-15 07:28:05.000000 green-bit-llm-0.0.1/green_bit_llm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-15 07:28:05.523786 green-bit-llm-0.0.1/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      850 2024-04-15 06:50:03.000000 green-bit-llm-0.0.1/setup.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.982233 green-bit-llm-0.1.0/
+-rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-04-07 20:16:16.000000 green-bit-llm-0.1.0/LICENSE
+-rw-r--r--   0 haojin     (501) staff       (20)     8583 2024-05-01 10:53:36.982076 green-bit-llm-0.1.0/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     8219 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/README.md
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.976235 green-bit-llm-0.1.0/green_bit_llm/
+-rw-r--r--   0 haojin     (501) staff       (20)       33 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     1920 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/args_parser.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.977611 green-bit-llm-0.1.0/green_bit_llm/common/
+-rw-r--r--   0 haojin     (501) staff       (20)       34 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)      156 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/enum.py
+-rw-r--r--   0 haojin     (501) staff       (20)    17313 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/model.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6826 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/common/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.978731 green-bit-llm-0.1.0/green_bit_llm/evaluation/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9588 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/datautils.py
+-rw-r--r--   0 haojin     (501) staff       (20)     7587 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/evaluate.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4569 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/lmclass.py
+-rw-r--r--   0 haojin     (501) staff       (20)     2840 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/evaluation/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.980034 green-bit-llm-0.1.0/green_bit_llm/inference/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)    21289 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/chat_base.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5319 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/chat_cli.py
+-rw-r--r--   0 haojin     (501) staff       (20)    18476 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/conversation.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4195 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/sim_gen.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4536 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/inference/utils.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.980685 green-bit-llm-0.1.0/green_bit_llm/sft/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4458 2024-05-01 10:29:45.000000 green-bit-llm-0.1.0/green_bit_llm/sft/finetune.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.981254 green-bit-llm-0.1.0/green_bit_llm/sft/optim/
+-rw-r--r--   0 haojin     (501) staff       (20)       32 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6259 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/adamw8bit.py
+-rw-r--r--   0 haojin     (501) staff       (20)    21387 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/optim/bnb_optimizer.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4160 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_lora.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.981870 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)     9361 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/gba_lora.py
+-rw-r--r--   0 haojin     (501) staff       (20)     2662 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/peft_utils/model.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5587 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/sft/utils.py
+-rw-r--r--   0 haojin     (501) staff       (20)       22 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/green_bit_llm/version.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-01 10:53:36.976835 green-bit-llm-0.1.0/green_bit_llm.egg-info/
+-rw-r--r--   0 haojin     (501) staff       (20)     8583 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     1163 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        1 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 haojin     (501) staff       (20)      162 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/requires.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       14 2024-05-01 10:53:36.000000 green-bit-llm-0.1.0/green_bit_llm.egg-info/top_level.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       38 2024-05-01 10:53:36.982281 green-bit-llm-0.1.0/setup.cfg
+-rw-r--r--   0 haojin     (501) staff       (20)      865 2024-04-27 11:19:52.000000 green-bit-llm-0.1.0/setup.py
```

### Comparing `green-bit-llm-0.0.1/LICENSE` & `green-bit-llm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.0.1/green_bit_llm/model.py` & `green-bit-llm-0.1.0/green_bit_llm/common/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     print(f"Error: Module not found: {e}.")
 
 from colorama import init, Fore, Style
 init(autoreset=True)
 
 STRATEGY_FILE_NAME = "quant_strategy.json"
 MODEL_TYPE_QWEN2 = "qwen2"
+STRATEGY_FILE_JSON_ROOT = "measurement"
 
 
 def engine_layer_prepare(model: torch.nn.Module):
     """
     Define the function that prepares the engine layer.
 
     Args:
@@ -45,18 +46,21 @@
 
 
 def apply_quant_strategy(name_attr: str, quant_strategy: Dict):
     """
     Apply quantization strategy based on the layer's name and the provided strategy.
     """
     strategy = None
-    for key in ['q_proj', 'k_proj', 'v_proj', 'o_proj', 'gate_proj', 'up_proj', 'down_proj']:
+    for key in ['q_proj', 'k_proj', 'v_proj', 'o_proj', 'gate_proj', 'up_proj', 'down_proj', 'qkv_proj', 'gate_up_proj']:
         if key in name_attr:
-            strategy = quant_strategy[key]
-            break
+            try:
+                strategy = quant_strategy[key]
+                break
+            except KeyError:
+                pass
     return strategy
 
 
 def get_disable_bias(name_attr: str, model_type) -> bool:
     """
     Usually the linear layer of llm disables bias. The three components 'q_proj', 'k_proj', and 'v_proj' in the qwen2 model attention module are exceptions.
     """
@@ -154,35 +158,33 @@
 
     # Load quantization strategy if applicable
     strategy = {}
     if layer_mode in (LayerMode.LAYER_MIX, LayerMode.CHANNEL_MIX):
         strategy_path = model_path / STRATEGY_FILE_NAME
         try:
             with open(strategy_path, "r") as file:
-                strategy = json.load(file)["measurement"]
+                strategy = json.load(file)[STRATEGY_FILE_JSON_ROOT]
         except FileNotFoundError:
             raise FileNotFoundError(f"Error: Strategy config file not found in {model_path}")
 
     # Initialize model with empty weights and load configuration
     with accelerate.init_empty_weights():
-        config = AutoConfig.from_pretrained(model_path)
+        config = AutoConfig.from_pretrained(model_path, trust_remote_code=True)
         model = AutoModelForCausalLM.from_pretrained(model_path, config=config, torch_dtype=dtype, **model_config).eval()
 
         # Quantize layers as necessary
         for i, layer in enumerate(model.model.layers):
             layers = find_layers(layer)
             layers_to_quantize = {name: layer for name, layer in layers.items() if name != 'lm_head'}
 
             strategy_per_block = strategy.get(f"model.layers.{i}") if strategy else None
 
             make_quant(layer, layers_to_quantize, layer_mode=layer_mode, group_size=group_size, bits=bits, dtype=dtype,
                        quant_strategy=strategy_per_block, model_type=config.model_type, requires_grad=requires_grad)
 
-    # model.tie_weights()
-    # print(model)
     # Load checkpoint, dispatch model, and apply post-initialization configurations
     model = accelerate.load_checkpoint_and_dispatch(model=model, checkpoint=model_path, device_map=device_map,
                                                     no_split_module_classes=["LlamaDecoderLayer"])
     model.seqlen = seqlen
     engine_layer_prepare(model)  # Assuming this prepares the model's engine layers post-initialization
     apply_dtype_to(model, dtype)  # Assuming this function applies the dtype to all model parameters
```

### Comparing `green-bit-llm-0.0.1/green_bit_llm/utils.py` & `green-bit-llm-0.1.0/green_bit_llm/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Returns True if the modules are found, False otherwise.
     """
     try:
         from bitorch_engine.layers.qlinear.nbit import MPQLinearBase
         from bitorch_engine.layers.qlinear.nbit.cuda import MPQLinearCuda, MBWQLinearCuda
     except ModuleNotFoundError as e:
         print(f"Error: Module not found: {e}.")
+        return False
     return True
 
 
 def match_model_pattern(model_name: str) -> tuple:
     """
     Matches the model name against known patterns and extracts relevant details.
 
@@ -182,8 +183,8 @@
     elif dtype is torch.bfloat16:
         model.bfloat16()
     # Additional condition for full precision (float32).
     elif dtype is torch.float:
         model.float()
     else:
         # If the dtype is not supported, raise an error.
-        raise ValueError("Unsupported dtype specified. Supported dtypes are torch.float, torch.half, and torch.bfloat16.")
+        raise ValueError("Unsupported dtype specified. Supported dtypes are torch.float, torch.half, and torch.bfloat16.")
```

### Comparing `green-bit-llm-0.0.1/setup.py` & `green-bit-llm-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 from pathlib import Path
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 package_dir = Path(__file__).parent / "green_bit_llm"
 with open(Path(__file__).parent / "requirements.txt") as fid:
     requirements = [l.strip() for l in fid.readlines()]
 
 sys.path.append(str(package_dir))
 from version import __version__
 
 setup(
     name="green-bit-llm",
     version=__version__,
-    description="A toolkit for fine-tuning, inference, and evaluating GreenBitAI's LLMs.",
+    description="A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email="team@greenbit.ai",
     author="GreenBitAI Contributors",
     url="https://github.com/GreenBitAI/green-bit-llm",
     license="Apache-2.0",
     install_requires=requirements,
-    packages=["green_bit_llm"],
+    packages=find_packages(),
     python_requires=">=3.9",
 )
```

