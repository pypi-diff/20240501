# Comparing `tmp/beit3_gml-0.1.1-py3-none-any.whl.zip` & `tmp/beit3_gml-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 44386 bytes, number of entries: 16
+Zip file size: 44391 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 23:52 beit3/__init__.py
 -rw-rw-r--  2.0 unx    33661 b- defN 24-Apr-08 23:52 beit3/datasets.py
 -rw-rw-r--  2.0 unx    25579 b- defN 24-Apr-08 23:52 beit3/engine_for_finetuning.py
 -rw-rw-r--  2.0 unx     4435 b- defN 24-Apr-08 23:52 beit3/glossary.py
 -rw-rw-r--  2.0 unx    13377 b- defN 24-Apr-08 23:52 beit3/modeling_finetune.py
 -rw-rw-r--  2.0 unx     3004 b- defN 24-Apr-08 23:52 beit3/modeling_utils.py
 -rw-rw-r--  2.0 unx     4497 b- defN 24-Apr-08 23:52 beit3/optim_factory.py
 -rw-rw-r--  2.0 unx     9786 b- defN 24-Apr-08 23:52 beit3/randaug.py
 -rw-rw-r--  2.0 unx    21898 b- defN 24-Apr-09 16:55 beit3/run_beit3_finetuning.py
 -rw-rw-r--  2.0 unx    33136 b- defN 24-Apr-08 23:52 beit3/utils.py
--rw-rw-r--  2.0 unx     1104 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      897 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx    12138 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/NOTICE.md
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1270 b- defN 24-Apr-09 16:55 beit3_gml-0.1.1.dist-info/RECORD
-16 files, 164880 bytes uncompressed, 42318 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx     1104 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      906 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx    12138 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/NOTICE.md
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1270 b- defN 24-Apr-30 23:57 beit3_gml-0.1.2.dist-info/RECORD
+16 files, 164889 bytes uncompressed, 42323 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: beit3/run_beit3_finetuning.py
 Comment: 
 
 Filename: beit3/utils.py
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/LICENSE
+Filename: beit3_gml-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/METADATA
+Filename: beit3_gml-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/NOTICE.md
+Filename: beit3_gml-0.1.2.dist-info/NOTICE.md
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/WHEEL
+Filename: beit3_gml-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/top_level.txt
+Filename: beit3_gml-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: beit3_gml-0.1.1.dist-info/RECORD
+Filename: beit3_gml-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `beit3_gml-0.1.1.dist-info/LICENSE` & `beit3_gml-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beit3_gml-0.1.1.dist-info/METADATA` & `beit3_gml-0.1.2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beit3-gml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for beit3, part of UniLM by Microsoft, customized for GML tasks
 Home-page: https://github.com/gimletlabs/unilm
 Author: Gimlet Labs
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Requires-Dist: mypy
 Requires-Dist: numpy
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: einops
 Requires-Dist: scipy
 Requires-Dist: ftfy
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: sentencepiece
 Requires-Dist: pyarrow
 Requires-Dist: transformers
 Requires-Dist: pycocotools
 Requires-Dist: pycocoevalcap
 Requires-Dist: torchscale-gml ==0.2.1
```

## Comparing `beit3_gml-0.1.1.dist-info/NOTICE.md` & `beit3_gml-0.1.2.dist-info/NOTICE.md`

 * *Files identical despite different names*

## Comparing `beit3_gml-0.1.1.dist-info/RECORD` & `beit3_gml-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 beit3/glossary.py,sha256=ffLuG4g0piUuu0eGRcJeF9-G0C4c_kPEUl19ZJID1s8,4435
 beit3/modeling_finetune.py,sha256=n7BwTkbVmjHiI3ks-YrfzoyQt9Y65JvDU1i2IEP2W5Y,13377
 beit3/modeling_utils.py,sha256=zAS3YrLAujLrgtZaXlQ62toVbONYSjUbVsh-s94pOic,3004
 beit3/optim_factory.py,sha256=mJFg5j2fNaHeTxZ-VaH66TFjcMin7vqRgoMmRIE2LAM,4497
 beit3/randaug.py,sha256=8ohyROB3RiXMSmqQqWkAo2sPaWVhx3oZqNpMv0LfVPQ,9786
 beit3/run_beit3_finetuning.py,sha256=BfN0Thop-vetm3Q9AUSEag4df71SzsGtfb3TJHy4INE,21898
 beit3/utils.py,sha256=zexFVeFpFK_L1l2xmrR4Rz9uZ0c1qHBIF4DP9z_955Q,33136
-beit3_gml-0.1.1.dist-info/LICENSE,sha256=kE3E2HSYd_Hboc2kggDSRi3MvrfBNNXk72-nXgGYyP4,1104
-beit3_gml-0.1.1.dist-info/METADATA,sha256=GrUkld3bNYj9n0l-PBJ_odxyZ1PSK6iOMJdB5qamFB0,897
-beit3_gml-0.1.1.dist-info/NOTICE.md,sha256=NW1pFnNsA_1iFE77AbwEXmm51Bh1oJ8E8wylcZUclFk,12138
-beit3_gml-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-beit3_gml-0.1.1.dist-info/top_level.txt,sha256=MixI3PwKGE_Bz-KKNddLOz0Xux3yw-TnLhsxQBO42CI,6
-beit3_gml-0.1.1.dist-info/RECORD,,
+beit3_gml-0.1.2.dist-info/LICENSE,sha256=kE3E2HSYd_Hboc2kggDSRi3MvrfBNNXk72-nXgGYyP4,1104
+beit3_gml-0.1.2.dist-info/METADATA,sha256=tmN_4GVEiim-80ZiJPIidoFPyyl0PA3bFZzXvpK09Dg,906
+beit3_gml-0.1.2.dist-info/NOTICE.md,sha256=NW1pFnNsA_1iFE77AbwEXmm51Bh1oJ8E8wylcZUclFk,12138
+beit3_gml-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+beit3_gml-0.1.2.dist-info/top_level.txt,sha256=MixI3PwKGE_Bz-KKNddLOz0Xux3yw-TnLhsxQBO42CI,6
+beit3_gml-0.1.2.dist-info/RECORD,,
```

