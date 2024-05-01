# Comparing `tmp/efficientvit_gml-0.1.7-py3-none-any.whl.zip` & `tmp/efficientvit_gml-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,83 +1,83 @@
-Zip file size: 114932 bytes, number of entries: 81
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 demo/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 demo/sam/__init__.py
--rw-rw-r--  2.0 unx     9056 b- defN 24-Apr-01 05:12 demo/sam/gradio_web_server.py
--rw-rw-r--  2.0 unx     1972 b- defN 24-Apr-01 05:12 demo/sam/process_prompts.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 demo/sam/helpers/__init__.py
--rw-rw-r--  2.0 unx     3580 b- defN 24-Apr-01 05:12 demo/sam/helpers/auto_mask_generator.py
--rw-rw-r--  2.0 unx     5257 b- defN 24-Apr-01 05:12 demo/sam/helpers/utils.py
--rw-rw-r--  2.0 unx       66 b- defN 24-Apr-01 05:12 demo/sam/helpers/predictors/__init__.py
--rw-rw-r--  2.0 unx     3894 b- defN 24-Apr-01 05:12 demo/sam/helpers/predictors/effvit_sam_onnx.py
--rw-rw-r--  2.0 unx     4478 b- defN 24-Apr-01 05:12 demo/sam/helpers/predictors/effvit_sam_pytorch.py
--rw-rw-r--  2.0 unx     5855 b- defN 24-Apr-01 05:12 demo/sam/helpers/predictors/effvit_sam_tensorrt.py
--rw-rw-r--  2.0 unx      115 b- defN 24-Apr-01 05:12 demo/sam/helpers/segmentation/__init__.py
--rw-rw-r--  2.0 unx     3409 b- defN 24-Apr-01 05:12 demo/sam/helpers/segmentation/process_prompts_onnx.py
--rw-rw-r--  2.0 unx     3938 b- defN 24-Apr-01 05:12 demo/sam/helpers/segmentation/process_prompts_pytorch.py
--rw-rw-r--  2.0 unx     5259 b- defN 24-Apr-01 05:12 demo/sam/helpers/segmentation/process_prompts_tensorrt.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 deployment/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 deployment/sam/__init__.py
--rw-rw-r--  2.0 unx       85 b- defN 24-Apr-01 05:12 deployment/sam/onnx/__init__.py
--rw-rw-r--  2.0 unx     6119 b- defN 24-Apr-01 05:12 deployment/sam/onnx/export_decoder.py
--rw-rw-r--  2.0 unx     4178 b- defN 24-Apr-01 05:12 deployment/sam/onnx/export_encoder.py
--rw-rw-r--  2.0 unx     9867 b- defN 24-Apr-01 05:12 deployment/sam/onnx/inference.py
--rw-rw-r--  2.0 unx       25 b- defN 24-Apr-01 05:12 deployment/sam/tensorrt/__init__.py
--rw-rw-r--  2.0 unx     9235 b- defN 24-Apr-01 05:12 deployment/sam/tensorrt/inference.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 efficientvit/__init__.py
--rw-rw-r--  2.0 unx     3096 b- defN 24-Apr-01 05:12 efficientvit/cls_model_zoo.py
--rw-rw-r--  2.0 unx     1715 b- defN 24-Apr-01 05:12 efficientvit/sam_model_zoo.py
--rw-rw-r--  2.0 unx     2455 b- defN 24-Apr-01 05:12 efficientvit/seg_model_zoo.py
--rw-rw-r--  2.0 unx       22 b- defN 24-Apr-01 17:58 efficientvit/version.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 efficientvit/apps/__init__.py
--rw-rw-r--  2.0 unx     4537 b- defN 24-Apr-01 05:12 efficientvit/apps/setup.py
--rw-rw-r--  2.0 unx      271 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/__init__.py
--rw-rw-r--  2.0 unx     7784 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/base.py
--rw-rw-r--  2.0 unx      240 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/augment/__init__.py
--rw-rw-r--  2.0 unx      786 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/augment/bbox.py
--rw-rw-r--  2.0 unx     2523 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/augment/color_aug.py
--rw-rw-r--  2.0 unx      273 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/random_resolution/__init__.py
--rw-rw-r--  2.0 unx    75054 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/random_resolution/_data_loader.py
--rw-rw-r--  2.0 unx    13589 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/random_resolution/_data_worker.py
--rw-rw-r--  2.0 unx     2973 b- defN 24-Apr-01 05:12 efficientvit/apps/data_provider/random_resolution/controller.py
--rw-rw-r--  2.0 unx      241 b- defN 24-Apr-01 05:12 efficientvit/apps/trainer/__init__.py
--rw-rw-r--  2.0 unx    10759 b- defN 24-Apr-01 05:12 efficientvit/apps/trainer/base.py
--rw-rw-r--  2.0 unx     4245 b- defN 24-Apr-01 05:12 efficientvit/apps/trainer/run_config.py
--rw-rw-r--  2.0 unx      355 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/__init__.py
--rw-rw-r--  2.0 unx     1872 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/dist.py
--rw-rw-r--  2.0 unx     1520 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/ema.py
--rw-rw-r--  2.0 unx     1385 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/export.py
--rw-rw-r--  2.0 unx     2628 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/init.py
--rw-rw-r--  2.0 unx     1610 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/lr.py
--rw-rw-r--  2.0 unx     1193 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/metric.py
--rw-rw-r--  2.0 unx     3325 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/misc.py
--rw-rw-r--  2.0 unx     1137 b- defN 24-Apr-01 05:12 efficientvit/apps/utils/opt.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 efficientvit/clscore/__init__.py
--rw-rw-r--  2.0 unx      219 b- defN 24-Apr-01 05:12 efficientvit/clscore/data_provider/__init__.py
--rw-rw-r--  2.0 unx     4403 b- defN 24-Apr-01 05:12 efficientvit/clscore/data_provider/imagenet.py
--rw-rw-r--  2.0 unx      252 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/__init__.py
--rw-rw-r--  2.0 unx      529 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/cls_run_config.py
--rw-rw-r--  2.0 unx     9198 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/cls_trainer.py
--rw-rw-r--  2.0 unx      266 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/utils/__init__.py
--rw-rw-r--  2.0 unx      678 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/utils/label_smooth.py
--rw-rw-r--  2.0 unx      750 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/utils/metric.py
--rw-rw-r--  2.0 unx     1897 b- defN 24-Apr-01 05:12 efficientvit/clscore/trainer/utils/mixup.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 05:12 efficientvit/models/__init__.py
--rw-rw-r--  2.0 unx      276 b- defN 24-Apr-01 05:12 efficientvit/models/efficientvit/__init__.py
--rw-rw-r--  2.0 unx    12527 b- defN 24-Apr-01 05:12 efficientvit/models/efficientvit/backbone.py
--rw-rw-r--  2.0 unx     4714 b- defN 24-Apr-01 05:12 efficientvit/models/efficientvit/cls.py
--rw-rw-r--  2.0 unx    23011 b- defN 24-Apr-01 05:12 efficientvit/models/efficientvit/sam.py
--rw-rw-r--  2.0 unx    10590 b- defN 24-Apr-01 05:12 efficientvit/models/efficientvit/seg.py
--rw-rw-r--  2.0 unx      273 b- defN 24-Apr-01 05:12 efficientvit/models/nn/__init__.py
--rw-rw-r--  2.0 unx      818 b- defN 24-Apr-01 05:12 efficientvit/models/nn/act.py
--rw-rw-r--  2.0 unx     2923 b- defN 24-Apr-01 05:12 efficientvit/models/nn/drop.py
--rw-rw-r--  2.0 unx     5098 b- defN 24-Apr-01 05:12 efficientvit/models/nn/norm.py
--rw-rw-r--  2.0 unx    16077 b- defN 24-Apr-01 05:12 efficientvit/models/nn/ops.py
--rw-rw-r--  2.0 unx      260 b- defN 24-Apr-01 05:12 efficientvit/models/utils/__init__.py
--rw-rw-r--  2.0 unx     1378 b- defN 24-Apr-01 05:12 efficientvit/models/utils/list.py
--rw-rw-r--  2.0 unx     2219 b- defN 24-Apr-01 05:12 efficientvit/models/utils/network.py
--rw-rw-r--  2.0 unx     2143 b- defN 24-Apr-01 05:12 efficientvit/models/utils/random.py
--rw-rw-r--  2.0 unx    11341 b- defN 24-Apr-01 17:58 efficientvit_gml-0.1.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx    13652 b- defN 24-Apr-01 17:58 efficientvit_gml-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-01 17:58 efficientvit_gml-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       29 b- defN 24-Apr-01 17:58 efficientvit_gml-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7583 b- defN 24-Apr-01 17:58 efficientvit_gml-0.1.7.dist-info/RECORD
-81 files, 355172 bytes uncompressed, 102620 bytes compressed:  71.1%
+Zip file size: 114934 bytes, number of entries: 81
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 demo/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 demo/sam/__init__.py
+-rw-rw-r--  2.0 unx     9056 b- defN 24-Apr-30 23:58 demo/sam/gradio_web_server.py
+-rw-rw-r--  2.0 unx     1972 b- defN 24-Apr-30 23:58 demo/sam/process_prompts.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 demo/sam/helpers/__init__.py
+-rw-rw-r--  2.0 unx     3580 b- defN 24-Apr-30 23:58 demo/sam/helpers/auto_mask_generator.py
+-rw-rw-r--  2.0 unx     5257 b- defN 24-Apr-30 23:58 demo/sam/helpers/utils.py
+-rw-rw-r--  2.0 unx       66 b- defN 24-Apr-30 23:58 demo/sam/helpers/predictors/__init__.py
+-rw-rw-r--  2.0 unx     3894 b- defN 24-Apr-30 23:58 demo/sam/helpers/predictors/effvit_sam_onnx.py
+-rw-rw-r--  2.0 unx     4478 b- defN 24-Apr-30 23:58 demo/sam/helpers/predictors/effvit_sam_pytorch.py
+-rw-rw-r--  2.0 unx     5855 b- defN 24-Apr-30 23:58 demo/sam/helpers/predictors/effvit_sam_tensorrt.py
+-rw-rw-r--  2.0 unx      115 b- defN 24-Apr-30 23:58 demo/sam/helpers/segmentation/__init__.py
+-rw-rw-r--  2.0 unx     3409 b- defN 24-Apr-30 23:58 demo/sam/helpers/segmentation/process_prompts_onnx.py
+-rw-rw-r--  2.0 unx     3938 b- defN 24-Apr-30 23:58 demo/sam/helpers/segmentation/process_prompts_pytorch.py
+-rw-rw-r--  2.0 unx     5259 b- defN 24-Apr-30 23:58 demo/sam/helpers/segmentation/process_prompts_tensorrt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 deployment/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 deployment/sam/__init__.py
+-rw-rw-r--  2.0 unx       85 b- defN 24-Apr-30 23:58 deployment/sam/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6119 b- defN 24-Apr-30 23:58 deployment/sam/onnx/export_decoder.py
+-rw-rw-r--  2.0 unx     4178 b- defN 24-Apr-30 23:58 deployment/sam/onnx/export_encoder.py
+-rw-rw-r--  2.0 unx     9867 b- defN 24-Apr-30 23:58 deployment/sam/onnx/inference.py
+-rw-rw-r--  2.0 unx       25 b- defN 24-Apr-30 23:58 deployment/sam/tensorrt/__init__.py
+-rw-rw-r--  2.0 unx     9235 b- defN 24-Apr-30 23:58 deployment/sam/tensorrt/inference.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 efficientvit/__init__.py
+-rw-rw-r--  2.0 unx     3096 b- defN 24-Apr-30 23:58 efficientvit/cls_model_zoo.py
+-rw-rw-r--  2.0 unx     1715 b- defN 24-Apr-30 23:58 efficientvit/sam_model_zoo.py
+-rw-rw-r--  2.0 unx     2455 b- defN 24-Apr-30 23:58 efficientvit/seg_model_zoo.py
+-rw-rw-r--  2.0 unx       22 b- defN 24-May-01 00:00 efficientvit/version.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 efficientvit/apps/__init__.py
+-rw-rw-r--  2.0 unx     4537 b- defN 24-Apr-30 23:58 efficientvit/apps/setup.py
+-rw-rw-r--  2.0 unx      271 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/__init__.py
+-rw-rw-r--  2.0 unx     7784 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/base.py
+-rw-rw-r--  2.0 unx      240 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/augment/__init__.py
+-rw-rw-r--  2.0 unx      786 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/augment/bbox.py
+-rw-rw-r--  2.0 unx     2523 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/augment/color_aug.py
+-rw-rw-r--  2.0 unx      273 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/random_resolution/__init__.py
+-rw-rw-r--  2.0 unx    75054 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/random_resolution/_data_loader.py
+-rw-rw-r--  2.0 unx    13589 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/random_resolution/_data_worker.py
+-rw-rw-r--  2.0 unx     2973 b- defN 24-Apr-30 23:58 efficientvit/apps/data_provider/random_resolution/controller.py
+-rw-rw-r--  2.0 unx      241 b- defN 24-Apr-30 23:58 efficientvit/apps/trainer/__init__.py
+-rw-rw-r--  2.0 unx    10759 b- defN 24-Apr-30 23:58 efficientvit/apps/trainer/base.py
+-rw-rw-r--  2.0 unx     4245 b- defN 24-Apr-30 23:58 efficientvit/apps/trainer/run_config.py
+-rw-rw-r--  2.0 unx      355 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/__init__.py
+-rw-rw-r--  2.0 unx     1872 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/dist.py
+-rw-rw-r--  2.0 unx     1520 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/ema.py
+-rw-rw-r--  2.0 unx     1385 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/export.py
+-rw-rw-r--  2.0 unx     2628 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/init.py
+-rw-rw-r--  2.0 unx     1610 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/lr.py
+-rw-rw-r--  2.0 unx     1193 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/metric.py
+-rw-rw-r--  2.0 unx     3325 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/misc.py
+-rw-rw-r--  2.0 unx     1137 b- defN 24-Apr-30 23:58 efficientvit/apps/utils/opt.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 efficientvit/clscore/__init__.py
+-rw-rw-r--  2.0 unx      219 b- defN 24-Apr-30 23:58 efficientvit/clscore/data_provider/__init__.py
+-rw-rw-r--  2.0 unx     4403 b- defN 24-Apr-30 23:58 efficientvit/clscore/data_provider/imagenet.py
+-rw-rw-r--  2.0 unx      252 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/__init__.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/cls_run_config.py
+-rw-rw-r--  2.0 unx     9198 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/cls_trainer.py
+-rw-rw-r--  2.0 unx      266 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/utils/__init__.py
+-rw-rw-r--  2.0 unx      678 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/utils/label_smooth.py
+-rw-rw-r--  2.0 unx      750 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/utils/metric.py
+-rw-rw-r--  2.0 unx     1897 b- defN 24-Apr-30 23:58 efficientvit/clscore/trainer/utils/mixup.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:58 efficientvit/models/__init__.py
+-rw-rw-r--  2.0 unx      276 b- defN 24-Apr-30 23:58 efficientvit/models/efficientvit/__init__.py
+-rw-rw-r--  2.0 unx    12527 b- defN 24-Apr-30 23:58 efficientvit/models/efficientvit/backbone.py
+-rw-rw-r--  2.0 unx     4714 b- defN 24-Apr-30 23:58 efficientvit/models/efficientvit/cls.py
+-rw-rw-r--  2.0 unx    23011 b- defN 24-Apr-30 23:58 efficientvit/models/efficientvit/sam.py
+-rw-rw-r--  2.0 unx    10590 b- defN 24-Apr-30 23:58 efficientvit/models/efficientvit/seg.py
+-rw-rw-r--  2.0 unx      273 b- defN 24-Apr-30 23:58 efficientvit/models/nn/__init__.py
+-rw-rw-r--  2.0 unx      818 b- defN 24-Apr-30 23:58 efficientvit/models/nn/act.py
+-rw-rw-r--  2.0 unx     2923 b- defN 24-Apr-30 23:58 efficientvit/models/nn/drop.py
+-rw-rw-r--  2.0 unx     5098 b- defN 24-Apr-30 23:58 efficientvit/models/nn/norm.py
+-rw-rw-r--  2.0 unx    16077 b- defN 24-Apr-30 23:58 efficientvit/models/nn/ops.py
+-rw-rw-r--  2.0 unx      260 b- defN 24-Apr-30 23:58 efficientvit/models/utils/__init__.py
+-rw-rw-r--  2.0 unx     1378 b- defN 24-Apr-30 23:58 efficientvit/models/utils/list.py
+-rw-rw-r--  2.0 unx     2219 b- defN 24-Apr-30 23:58 efficientvit/models/utils/network.py
+-rw-rw-r--  2.0 unx     2143 b- defN 24-Apr-30 23:58 efficientvit/models/utils/random.py
+-rw-rw-r--  2.0 unx    11341 b- defN 24-May-01 00:00 efficientvit_gml-0.1.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    13661 b- defN 24-May-01 00:00 efficientvit_gml-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-01 00:00 efficientvit_gml-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       29 b- defN 24-May-01 00:00 efficientvit_gml-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7583 b- defN 24-May-01 00:00 efficientvit_gml-0.1.8.dist-info/RECORD
+81 files, 355181 bytes uncompressed, 102622 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -222,23 +222,23 @@
 
 Filename: efficientvit/models/utils/network.py
 Comment: 
 
 Filename: efficientvit/models/utils/random.py
 Comment: 
 
-Filename: efficientvit_gml-0.1.7.dist-info/LICENSE
+Filename: efficientvit_gml-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: efficientvit_gml-0.1.7.dist-info/METADATA
+Filename: efficientvit_gml-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: efficientvit_gml-0.1.7.dist-info/WHEEL
+Filename: efficientvit_gml-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: efficientvit_gml-0.1.7.dist-info/top_level.txt
+Filename: efficientvit_gml-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: efficientvit_gml-0.1.7.dist-info/RECORD
+Filename: efficientvit_gml-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## efficientvit/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.7'
+__version__ = '0.1.8'
```

## Comparing `efficientvit_gml-0.1.7.dist-info/LICENSE` & `efficientvit_gml-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `efficientvit_gml-0.1.7.dist-info/METADATA` & `efficientvit_gml-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficientvit-gml
-Version: 0.1.7
+Version: 0.1.8
 Summary: open-set object detector
 Home-page: https://github.com/mit-han-lab/efficientvit
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: einops
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: timm
 Requires-Dist: tqdm
 Requires-Dist: torchprofile
 Requires-Dist: matplotlib
 Requires-Dist: transformers
 Requires-Dist: onnx
 Requires-Dist: onnxsim
```

## Comparing `efficientvit_gml-0.1.7.dist-info/RECORD` & `efficientvit_gml-0.1.8.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 deployment/sam/onnx/inference.py,sha256=msCQSy_gQJ__dW2WqqpAOzYEm_2Zay25NuIRxvsrrgc,9867
 deployment/sam/tensorrt/__init__.py,sha256=TaUXX4Zb7OqaX-OA4e05RZKUbMNY5XlCgvBxgcvuSAA,25
 deployment/sam/tensorrt/inference.py,sha256=LqEXOdALrnEA6p6rx2PNvFjO48YJkg81AXP3Sf9DBC8,9235
 efficientvit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 efficientvit/cls_model_zoo.py,sha256=S64ntHMzYPWF9_-C6lNqyhwNUEOLfPymzaRZ_7_fKHw,3096
 efficientvit/sam_model_zoo.py,sha256=mYRpO0BqeSybjwXnoDuRC004aEyybpNpPufAeVyd35M,1715
 efficientvit/seg_model_zoo.py,sha256=FrcPKTjI1NVI7kEorremO3H1UZPzI9wcAVd1jJ2swWc,2455
-efficientvit/version.py,sha256=mFY0GwwuN-a3M8w93_mskS6GZIvv9SNdjLfJaWNsm-I,22
+efficientvit/version.py,sha256=rq5OMW-khxQo_5FAvSrPaAS1lRfG9aG2hSuo-KK2Yfk,22
 efficientvit/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 efficientvit/apps/setup.py,sha256=kf3tn_EOl6faGawkPRlJvz3DcCy2rSekcs62DgPtLrg,4537
 efficientvit/apps/data_provider/__init__.py,sha256=pcOnpUKbwiOBGmJCpZ1K9bxo5G3gIpyir_fpiw05F6c,271
 efficientvit/apps/data_provider/base.py,sha256=xKCgyptnretINe0ukxFnnSXIx3soBfX38BBmUaTbRNU,7784
 efficientvit/apps/data_provider/augment/__init__.py,sha256=-V1vKEWaYDyHau7BmDmmpd8D8EuXPNZOHM5C-8CDwOM,240
 efficientvit/apps/data_provider/augment/bbox.py,sha256=yyBAc6BjWGzevM3nrrM5HGvrRBYXyHS7iEBKKKp5Yu0,786
 efficientvit/apps/data_provider/augment/color_aug.py,sha256=Gc09SbdlZdtvOfxDVDY29LYFviVw7Oa2i_r00jt38R0,2523
@@ -70,12 +70,12 @@
 efficientvit/models/nn/drop.py,sha256=fAYkeh89teYCnw7tpUuyWUUkNBcHmtV4E3teHzwHgsc,2923
 efficientvit/models/nn/norm.py,sha256=1dHJBrjHIWMcTNiEdbkZ-GH_60IeQqawBdiL3OZJACU,5098
 efficientvit/models/nn/ops.py,sha256=ZOlQqTLAW5VoM9dJ_iredCY6JqAgvH-LubY9TsL0UoA,16077
 efficientvit/models/utils/__init__.py,sha256=ewgctZyjabYC2EcwLLW87269zFSahR7n3cpxjxi6DY4,260
 efficientvit/models/utils/list.py,sha256=fjUuP0itwrPUofAMxYqCh52BapsjLBMmHKes_3veWAA,1378
 efficientvit/models/utils/network.py,sha256=yp4MIIx7kDexg27ovsXnrPPRG9YuNw92sDjCy9jt55E,2219
 efficientvit/models/utils/random.py,sha256=vMuJXp0A50SUF1jV_Sfrf2XsQn4IFnSs-M2TE0gwyl0,2143
-efficientvit_gml-0.1.7.dist-info/LICENSE,sha256=PDl2qKehHImbLc33HLYRmMswLpVCzZnNrV8dXQr-OAM,11341
-efficientvit_gml-0.1.7.dist-info/METADATA,sha256=wQf8cqG1tHxJaPRBZqrMlt4zA6YhDPe8f_Tchmg_uwk,13652
-efficientvit_gml-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-efficientvit_gml-0.1.7.dist-info/top_level.txt,sha256=oxkFMxN3x_mQn-XoX03AJ5OQWv9bw4Eyqaz5cc4AIEQ,29
-efficientvit_gml-0.1.7.dist-info/RECORD,,
+efficientvit_gml-0.1.8.dist-info/LICENSE,sha256=PDl2qKehHImbLc33HLYRmMswLpVCzZnNrV8dXQr-OAM,11341
+efficientvit_gml-0.1.8.dist-info/METADATA,sha256=KH8XPGj0UGEHNma9Nznp7w0kvJGxkTNNCgdP6y5T7cc,13661
+efficientvit_gml-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+efficientvit_gml-0.1.8.dist-info/top_level.txt,sha256=oxkFMxN3x_mQn-XoX03AJ5OQWv9bw4Eyqaz5cc4AIEQ,29
+efficientvit_gml-0.1.8.dist-info/RECORD,,
```

