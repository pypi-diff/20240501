# Comparing `tmp/umbrela-0.0.2-py3-none-any.whl.zip` & `tmp/umbrela-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 16104 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 prompts/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 24-May-01 01:05 prompts/qrel_fewshot_bing.txt
+Zip file size: 16000 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:11 umbrela/__init__.py
--rw-r--r--  2.0 unx     2648 b- defN 24-May-01 01:04 umbrela/gpt_judge.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-01 18:24 umbrela/gpt_judge.py
 -rw-r--r--  2.0 unx      751 b- defN 24-Apr-30 23:41 umbrela/llm_judge.py
--rw-r--r--  2.0 unx     2377 b- defN 24-May-01 01:04 umbrela/osllm_judge.py
--rw-r--r--  2.0 unx     3315 b- defN 24-May-01 01:04 umbrela/vicuna_judge.py
+-rw-r--r--  2.0 unx     2385 b- defN 24-May-01 18:24 umbrela/osllm_judge.py
+-rw-r--r--  2.0 unx     3323 b- defN 24-May-01 18:24 umbrela/vicuna_judge.py
+-rw-r--r--  2.0 unx     1231 b- defN 24-May-01 01:05 umbrela/prompts/qrel_fewshot_bing.txt
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 umbrela/utils/__init__.py
 -rw-r--r--  2.0 unx     1884 b- defN 24-May-01 01:04 umbrela/utils/common_utils.py
 -rw-r--r--  2.0 unx     3040 b- defN 24-May-01 18:15 umbrela/utils/qrel_utils.py
--rw-r--r--  2.0 unx    10766 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13073 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1181 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/RECORD
-15 files, 40374 bytes uncompressed, 14158 bytes compressed:  64.9%
+-rw-r--r--  2.0 unx    10766 b- defN 24-May-01 18:25 umbrela-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13073 b- defN 24-May-01 18:25 umbrela-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 18:25 umbrela-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-01 18:25 umbrela-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 24-May-01 18:25 umbrela-0.0.3.dist-info/RECORD
+14 files, 40324 bytes uncompressed, 14152 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,13 +1,7 @@
-Filename: prompts/__init__.py
-Comment: 
-
-Filename: prompts/qrel_fewshot_bing.txt
-Comment: 
-
 Filename: umbrela/__init__.py
 Comment: 
 
 Filename: umbrela/gpt_judge.py
 Comment: 
 
 Filename: umbrela/llm_judge.py
@@ -15,32 +9,35 @@
 
 Filename: umbrela/osllm_judge.py
 Comment: 
 
 Filename: umbrela/vicuna_judge.py
 Comment: 
 
+Filename: umbrela/prompts/qrel_fewshot_bing.txt
+Comment: 
+
 Filename: umbrela/utils/__init__.py
 Comment: 
 
 Filename: umbrela/utils/common_utils.py
 Comment: 
 
 Filename: umbrela/utils/qrel_utils.py
 Comment: 
 
-Filename: umbrela-0.0.2.dist-info/LICENSE
+Filename: umbrela-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: umbrela-0.0.2.dist-info/METADATA
+Filename: umbrela-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: umbrela-0.0.2.dist-info/WHEEL
+Filename: umbrela-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: umbrela-0.0.2.dist-info/top_level.txt
+Filename: umbrela-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: umbrela-0.0.2.dist-info/RECORD
+Filename: umbrela-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## umbrela/gpt_judge.py

```diff
@@ -8,15 +8,15 @@
 from umbrela.utils import common_utils
 
 
 class GPTJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
-        prompt_file="prompts/qrel_fewshot_bing.txt",
+        prompt_file="umbrela/prompts/qrel_fewshot_bing.txt",
         few_shot_count: int = 2,
         engine=""
     ) -> None:
         model_name = engine if engine else "gpt"
         super().__init__(qrel, prompt_file, model_name, few_shot_count)
         self.create_openai_client()
```

## umbrela/osllm_judge.py

```diff
@@ -7,15 +7,15 @@
 from umbrela.utils import common_utils
 
 class OSLLMJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
         model_name: str,
-        prompt_file: str = "prompts/qrel_fewshot_bing.txt",
+        prompt_file: str = "umbrela/prompts/qrel_fewshot_bing.txt",
         few_shot_count: int = 2,
         device: str = "cuda",
         num_gpus: int = 1,
     ) -> None:
         super().__init__(qrel, prompt_file, model_name, few_shot_count)
         self._device = device
         if self._device == "cuda":
```

## umbrela/vicuna_judge.py

```diff
@@ -8,15 +8,15 @@
 from umbrela.utils import common_utils
 
 
 class VicunaJudge(LLMJudge):
     def __init__(
         self,
         qrel: str,
-        prompt_file: str = "prompts/qrel_fewshot_bing.txt",
+        prompt_file: str = "umbrela/prompts/qrel_fewshot_bing.txt",
         few_shot_count: int = 2,
         device: str = "cuda",
         num_gpus: int = 1,
     ) -> None:
         super().__init__(qrel, prompt_file, "lmsys/vicuna-7b-v1.5-16k", few_shot_count)
         self._device = device
         if self._device == "cuda":
```

## Comparing `prompts/qrel_fewshot_bing.txt` & `umbrela/prompts/qrel_fewshot_bing.txt`

 * *Files identical despite different names*

## Comparing `umbrela-0.0.2.dist-info/LICENSE` & `umbrela-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `umbrela-0.0.2.dist-info/METADATA` & `umbrela-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbrela
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Package for generating query-passage relevance assessment labels.
 Author-email: Shivani Upadhyay <sjupadhyay@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `umbrela-0.0.2.dist-info/RECORD` & `umbrela-0.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-prompts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-prompts/qrel_fewshot_bing.txt,sha256=9Z1aw7tOHhbAuaLuUf5mjusxFNdNSZJaZzYIbCCLHuk,1231
 umbrela/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-umbrela/gpt_judge.py,sha256=CVlVAPaIGVG71bngQdg_h1OACG9maVQeD-2j74QqAIE,2648
+umbrela/gpt_judge.py,sha256=VOZ-dBTHD0PdkFdlyeZ2uwrUrXGtIKvdNwn93wR69Wc,2656
 umbrela/llm_judge.py,sha256=7uC-GFZvw_vQom4jekvc_Z5NYNH8CJLoVGgL8LLosu0,751
-umbrela/osllm_judge.py,sha256=qgmLpz77lvFkulf8k4LZmEYdKLyP7I_ICuBM874kgYg,2377
-umbrela/vicuna_judge.py,sha256=68ZnBIK-sUbKAAYG-oaoEllpvmoEDo_faGNu2IvAkeU,3315
+umbrela/osllm_judge.py,sha256=0o0mjLqBV80aSS4ZZu2VrGIgaMhH9XO6LbG1nPM2aq8,2385
+umbrela/vicuna_judge.py,sha256=cf4YFmlS-b_eAmrS0TU-iIP74fodT0_JJaf_OdS-7cg,3323
+umbrela/prompts/qrel_fewshot_bing.txt,sha256=9Z1aw7tOHhbAuaLuUf5mjusxFNdNSZJaZzYIbCCLHuk,1231
 umbrela/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 umbrela/utils/common_utils.py,sha256=6AdK9cKsYZ773yTeUb8X_aQfoPi8cMTyxxfuAtBFH_M,1884
 umbrela/utils/qrel_utils.py,sha256=JeGZiVbUaZCY-l98T9ASPf6BWTZK9H2aIsNU3aaYaFk,3040
-umbrela-0.0.2.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
-umbrela-0.0.2.dist-info/METADATA,sha256=9r7n7FhpVhGeudOvEgm8zer782MNFw2qzvsLFBgPIdI,13073
-umbrela-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-umbrela-0.0.2.dist-info/top_level.txt,sha256=nPc9ofEXItuJUl8Kqhr2rIIAcTj1xTzb8-j4XvmcdjU,16
-umbrela-0.0.2.dist-info/RECORD,,
+umbrela-0.0.3.dist-info/LICENSE,sha256=5xLBDUMjnrK1STpg2CvThfuHUKCCFxoSozCIGAx56Pk,10766
+umbrela-0.0.3.dist-info/METADATA,sha256=mr1_U1jnGPda5dGLlfoun5yzID3BQfQyi5bh7ShUqBY,13073
+umbrela-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+umbrela-0.0.3.dist-info/top_level.txt,sha256=E6ASKK6PNcJWJAC6mYtbt91P5fKJrAkJtRoGthCaYUI,8
+umbrela-0.0.3.dist-info/RECORD,,
```

