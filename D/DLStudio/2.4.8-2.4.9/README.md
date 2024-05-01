# Comparing `tmp/DLStudio-2.4.8.tar.gz` & `tmp/DLStudio-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLStudio-2.4.8.tar", last modified: Sat Apr 27 21:46:25 2024, max compression
+gzip compressed data, was "DLStudio-2.4.9.tar", last modified: Wed May  1 17:11:46 2024, max compression
```

## Comparing `DLStudio-2.4.8.tar` & `DLStudio-2.4.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/AdversarialLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    91752 2024-04-27 18:19:47.000000 DLStudio-2.4.8/AdversarialLearning/AdversarialLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      609 2023-12-06 04:36:12.000000 DLStudio-2.4.8/AdversarialLearning/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/DLStudio/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   346678 2024-04-27 20:57:17.000000 DLStudio-2.4.8/DLStudio/DLStudio.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      555 2023-12-06 04:36:12.000000 DLStudio-2.4.8/DLStudio/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)   312388 2024-04-27 21:32:24.000000 DLStudio-2.4.8/DLStudio-2.4.8.html
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.680817 DLStudio-2.4.8/DLStudio.egg-info/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2108 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/PKG-INFO
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2281 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/SOURCES.txt
--rwxr-xr-x   0 kak       (1000) kak       (1000)        1 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/dependency_links.txt
--rwxr-xr-x   0 kak       (1000) kak       (1000)      108 2024-04-27 21:46:25.000000 DLStudio-2.4.8/DLStudio.egg-info/top_level.txt
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/DataPrediction/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    34515 2024-04-27 18:21:48.000000 DLStudio-2.4.8/DataPrediction/DataPrediction.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:12.000000 DLStudio-2.4.8/DataPrediction/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Examples/
--rw-r--r--   0 kak       (1000) kak       (1000)      516 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/README
--rw-r--r--   0 kak       (1000) kak       (1000)     2372 2024-02-17 00:32:47.000000 DLStudio-2.4.8/Examples/custom_data_loading.py
--rw-r--r--   0 kak       (1000) kak       (1000)     4822 2024-02-17 00:35:53.000000 DLStudio-2.4.8/Examples/noisy_object_detection_and_localization.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3518 2024-02-19 18:49:38.000000 DLStudio-2.4.8/Examples/object_detection_and_localization.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3513 2024-03-16 11:10:34.000000 DLStudio-2.4.8/Examples/object_detection_and_localization_iou.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1900 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_cifar10.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2179 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_reconfig.py
--rw-r--r--   0 kak       (1000) kak       (1000)     1652 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/playing_with_sequential.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2161 2024-02-17 00:29:28.000000 DLStudio-2.4.8/Examples/playing_with_skip_connections.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3067 2024-03-17 20:04:07.000000 DLStudio-2.4.8/Examples/semantic_segmentation.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2939 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_GRU.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3070 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_GRU_word2vec.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2770 2024-03-26 13:53:50.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnet.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3139 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3172 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2_word2vec.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3084 2023-12-06 04:36:23.000000 DLStudio-2.4.8/Examples/text_classification_with_TEXTnet_word2vec.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesAdversarialLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3140 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/README
--rw-r--r--   0 kak       (1000) kak       (1000)     4755 2024-03-23 17:28:17.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG1.py
--rw-r--r--   0 kak       (1000) kak       (1000)     5181 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG2.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3969 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_CG1.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3756 2023-12-06 04:36:12.000000 DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_with_gp_CG2.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesDataPrediction/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3497 2023-12-06 04:36:25.000000 DLStudio-2.4.8/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesDiffusion/
--rw-r--r--   0 kak       (1000) kak       (1000)     3450 2024-03-20 04:39:10.000000 DLStudio-2.4.8/ExamplesDiffusion/GenerateNewImageSamples.py
--rw-rw-r--   0 kak       (1000) kak       (1000)     5361 2024-03-16 14:36:21.000000 DLStudio-2.4.8/ExamplesDiffusion/README
--rw-r--r--   0 kak       (1000) kak       (1000)     3201 2024-03-23 21:29:29.000000 DLStudio-2.4.8/ExamplesDiffusion/RunCodeForDiffusion.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2442 2024-03-23 17:07:15.000000 DLStudio-2.4.8/ExamplesDiffusion/VisualizeSamples.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesMetricLearning/
--rw-r--r--   0 kak       (1000) kak       (1000)     2436 2023-12-06 04:36:23.000000 DLStudio-2.4.8/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2182 2023-12-06 04:36:23.000000 DLStudio-2.4.8/ExamplesMetricLearning/example_for_triplet_loss.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesSeq2SeqLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2804 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)     3826 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/ExamplesTransformers/
--rw-r--r--   0 kak       (1000) kak       (1000)     2451 2024-04-27 20:50:21.000000 DLStudio-2.4.8/ExamplesTransformers/image_recog_with_visTransformer.py
--rw-r--r--   0 kak       (1000) kak       (1000)     5080 2024-04-27 14:48:55.000000 DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerFG.py
--rw-r--r--   0 kak       (1000) kak       (1000)     4840 2024-04-27 14:49:07.000000 DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerPreLN.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2909 2024-04-26 03:59:11.000000 DLStudio-2.4.8/ExamplesTransformers/test_checkpoint_for_visTransformer.py
--rw-r--r--   0 kak       (1000) kak       (1000)     3822 2023-12-06 04:36:11.000000 DLStudio-2.4.8/ExamplesTransformers/upgrade_model.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/GenerativeDiffusion/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    66182 2024-04-27 18:25:02.000000 DLStudio-2.4.8/GenerativeDiffusion/GenerativeDiffusion.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      854 2024-03-09 18:01:26.000000 DLStudio-2.4.8/GenerativeDiffusion/__init__.py
--rw-r--r--   0 kak       (1000) kak       (1000)     2548 2024-04-27 21:04:33.000000 DLStudio-2.4.8/MANIFEST.in
--rw-r--r--   0 kak       (1000) kak       (1000)     1120 2023-12-06 04:36:12.000000 DLStudio-2.4.8/Makefile
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/MetricLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    39645 2024-04-27 18:24:24.000000 DLStudio-2.4.8/MetricLearning/MetricLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:25.000000 DLStudio-2.4.8/MetricLearning/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)     2108 2024-04-27 21:46:25.684817 DLStudio-2.4.8/PKG-INFO
--rw-r--r--   0 kak       (1000) kak       (1000)     1032 2023-12-06 04:36:12.000000 DLStudio-2.4.8/README
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Seq2SeqLearning/
--rwxr-xr-x   0 kak       (1000) kak       (1000)    80633 2024-04-27 18:20:35.000000 DLStudio-2.4.8/Seq2SeqLearning/Seq2SeqLearning.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      589 2023-12-06 04:36:12.000000 DLStudio-2.4.8/Seq2SeqLearning/__init__.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/TestDLStudio/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   346678 2024-04-27 21:02:42.000000 DLStudio-2.4.8/TestDLStudio/DLStudio.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      585 2023-12-06 04:36:23.000000 DLStudio-2.4.8/TestDLStudio/Test.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      828 2023-12-06 04:36:23.000000 DLStudio-2.4.8/TestDLStudio/TestInstanceCreation.py
-drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-04-27 21:46:25.684817 DLStudio-2.4.8/Transformers/
--rwxr-xr-x   0 kak       (1000) kak       (1000)   191880 2024-04-27 18:23:27.000000 DLStudio-2.4.8/Transformers/Transformers.py
--rwxr-xr-x   0 kak       (1000) kak       (1000)      553 2024-03-28 13:14:29.000000 DLStudio-2.4.8/Transformers/__init__.py
--rw-rw-r--   0 kak       (1000) kak       (1000)       38 2024-04-27 21:46:25.684817 DLStudio-2.4.8/setup.cfg
--rwxr-xr-x   0 kak       (1000) kak       (1000)     2428 2024-04-27 06:52:24.000000 DLStudio-2.4.8/setup.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.037561 DLStudio-2.4.9/
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.029560 DLStudio-2.4.9/AdversarialLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    91747 2024-05-01 16:16:08.000000 DLStudio-2.4.9/AdversarialLearning/AdversarialLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      609 2023-12-06 04:36:12.000000 DLStudio-2.4.9/AdversarialLearning/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.029560 DLStudio-2.4.9/DLStudio/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   346955 2024-05-01 16:49:34.000000 DLStudio-2.4.9/DLStudio/DLStudio.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      555 2023-12-06 04:36:12.000000 DLStudio-2.4.9/DLStudio/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)   312998 2024-05-01 17:04:35.000000 DLStudio-2.4.9/DLStudio-2.4.9.html
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/DLStudio.egg-info/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2108 2024-05-01 17:11:46.000000 DLStudio-2.4.9/DLStudio.egg-info/PKG-INFO
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2281 2024-05-01 17:11:46.000000 DLStudio-2.4.9/DLStudio.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kak       (1000) kak       (1000)        1 2024-05-01 17:11:46.000000 DLStudio-2.4.9/DLStudio.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      108 2024-05-01 17:11:46.000000 DLStudio-2.4.9/DLStudio.egg-info/top_level.txt
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/DataPrediction/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    34510 2024-05-01 16:17:14.000000 DLStudio-2.4.9/DataPrediction/DataPrediction.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:12.000000 DLStudio-2.4.9/DataPrediction/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/Examples/
+-rw-r--r--   0 kak       (1000) kak       (1000)      516 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     2372 2024-02-17 00:32:47.000000 DLStudio-2.4.9/Examples/custom_data_loading.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     4822 2024-02-17 00:35:53.000000 DLStudio-2.4.9/Examples/noisy_object_detection_and_localization.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3518 2024-02-19 18:49:38.000000 DLStudio-2.4.9/Examples/object_detection_and_localization.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3513 2024-03-16 11:10:34.000000 DLStudio-2.4.9/Examples/object_detection_and_localization_iou.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     1900 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/playing_with_cifar10.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2179 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/playing_with_reconfig.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     1652 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/playing_with_sequential.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2161 2024-05-01 16:48:30.000000 DLStudio-2.4.9/Examples/playing_with_skip_connections.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3067 2024-03-17 20:04:07.000000 DLStudio-2.4.9/Examples/semantic_segmentation.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2939 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/text_classification_with_GRU.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3070 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/text_classification_with_GRU_word2vec.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2770 2024-03-26 13:53:50.000000 DLStudio-2.4.9/Examples/text_classification_with_TEXTnet.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3139 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/text_classification_with_TEXTnetOrder2.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3172 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/text_classification_with_TEXTnetOrder2_word2vec.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3084 2023-12-06 04:36:23.000000 DLStudio-2.4.9/Examples/text_classification_with_TEXTnet_word2vec.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesAdversarialLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3140 2023-12-06 04:36:12.000000 DLStudio-2.4.9/ExamplesAdversarialLearning/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     4755 2024-03-23 17:28:17.000000 DLStudio-2.4.9/ExamplesAdversarialLearning/dcgan_DG1.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     5181 2023-12-06 04:36:12.000000 DLStudio-2.4.9/ExamplesAdversarialLearning/dcgan_DG2.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3969 2023-12-06 04:36:12.000000 DLStudio-2.4.9/ExamplesAdversarialLearning/wgan_CG1.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3756 2023-12-06 04:36:12.000000 DLStudio-2.4.9/ExamplesAdversarialLearning/wgan_with_gp_CG2.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesDataPrediction/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3497 2023-12-06 04:36:25.000000 DLStudio-2.4.9/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesDiffusion/
+-rw-r--r--   0 kak       (1000) kak       (1000)     3450 2024-03-20 04:39:10.000000 DLStudio-2.4.9/ExamplesDiffusion/GenerateNewImageSamples.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)     5361 2024-03-16 14:36:21.000000 DLStudio-2.4.9/ExamplesDiffusion/README
+-rw-r--r--   0 kak       (1000) kak       (1000)     3201 2024-03-23 21:29:29.000000 DLStudio-2.4.9/ExamplesDiffusion/RunCodeForDiffusion.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2442 2024-03-23 17:07:15.000000 DLStudio-2.4.9/ExamplesDiffusion/VisualizeSamples.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesMetricLearning/
+-rw-r--r--   0 kak       (1000) kak       (1000)     2436 2023-12-06 04:36:23.000000 DLStudio-2.4.9/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2182 2023-12-06 04:36:23.000000 DLStudio-2.4.9/ExamplesMetricLearning/example_for_triplet_loss.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesSeq2SeqLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2804 2023-12-06 04:36:11.000000 DLStudio-2.4.9/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     3826 2023-12-06 04:36:11.000000 DLStudio-2.4.9/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/ExamplesTransformers/
+-rw-r--r--   0 kak       (1000) kak       (1000)     2466 2024-05-01 16:09:49.000000 DLStudio-2.4.9/ExamplesTransformers/image_recog_with_visTransformer.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     5880 2024-05-01 16:02:59.000000 DLStudio-2.4.9/ExamplesTransformers/seq2seq_with_transformerFG.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     5617 2024-05-01 16:02:18.000000 DLStudio-2.4.9/ExamplesTransformers/seq2seq_with_transformerPreLN.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2909 2024-04-26 03:59:11.000000 DLStudio-2.4.9/ExamplesTransformers/test_checkpoint_for_visTransformer.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     3822 2023-12-06 04:36:11.000000 DLStudio-2.4.9/ExamplesTransformers/upgrade_model.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/GenerativeDiffusion/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    66177 2024-05-01 16:18:51.000000 DLStudio-2.4.9/GenerativeDiffusion/GenerativeDiffusion.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      854 2024-03-09 18:01:26.000000 DLStudio-2.4.9/GenerativeDiffusion/__init__.py
+-rw-r--r--   0 kak       (1000) kak       (1000)     2548 2024-04-28 15:58:14.000000 DLStudio-2.4.9/MANIFEST.in
+-rw-r--r--   0 kak       (1000) kak       (1000)     1120 2023-12-06 04:36:12.000000 DLStudio-2.4.9/Makefile
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/MetricLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    39642 2024-05-01 16:18:15.000000 DLStudio-2.4.9/MetricLearning/MetricLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      584 2023-12-06 04:36:25.000000 DLStudio-2.4.9/MetricLearning/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)     2108 2024-05-01 17:11:46.037561 DLStudio-2.4.9/PKG-INFO
+-rw-r--r--   0 kak       (1000) kak       (1000)     1032 2023-12-06 04:36:12.000000 DLStudio-2.4.9/README
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/Seq2SeqLearning/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)    80628 2024-05-01 16:16:33.000000 DLStudio-2.4.9/Seq2SeqLearning/Seq2SeqLearning.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      589 2023-12-06 04:36:12.000000 DLStudio-2.4.9/Seq2SeqLearning/__init__.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.033561 DLStudio-2.4.9/TestDLStudio/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   346955 2024-05-01 16:50:52.000000 DLStudio-2.4.9/TestDLStudio/DLStudio.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      585 2023-12-06 04:36:23.000000 DLStudio-2.4.9/TestDLStudio/Test.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      828 2023-12-06 04:36:23.000000 DLStudio-2.4.9/TestDLStudio/TestInstanceCreation.py
+drwxrwxr-x   0 kak       (1000) kak       (1000)        0 2024-05-01 17:11:46.037561 DLStudio-2.4.9/Transformers/
+-rwxr-xr-x   0 kak       (1000) kak       (1000)   194680 2024-05-01 16:10:24.000000 DLStudio-2.4.9/Transformers/Transformers.py
+-rwxr-xr-x   0 kak       (1000) kak       (1000)      553 2024-03-28 13:14:29.000000 DLStudio-2.4.9/Transformers/__init__.py
+-rw-rw-r--   0 kak       (1000) kak       (1000)       38 2024-05-01 17:11:46.037561 DLStudio-2.4.9/setup.cfg
+-rwxr-xr-x   0 kak       (1000) kak       (1000)     2428 2024-04-28 15:57:56.000000 DLStudio-2.4.9/setup.py
```

### Comparing `DLStudio-2.4.8/AdversarialLearning/AdversarialLearning.py` & `DLStudio-2.4.9/AdversarialLearning/AdversarialLearning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
-  You are looking at the AdversarialLearning co-class file in the DLStudio platform.
+  You are looking at the AdversarialLearning module file in the DLStudio platform.
   For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
 
 INTRODUCTION TO ADVERSARIAL LEARNING FOR DATA MODELING:
```

### Comparing `DLStudio-2.4.8/AdversarialLearning/__init__.py` & `DLStudio-2.4.9/AdversarialLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/DLStudio/DLStudio.py` & `DLStudio-2.4.9/DLStudio/DLStudio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
-
 __doc__ = '''
 
 DLStudio.py
 
 Version: ''' + __version__ + '''
    
 Author: Avinash Kak (kak@purdue.edu)
 
 Date: ''' + __date__ + '''
 
 
 @tag_changes
 CHANGE LOG:
 
+  Version 2.4.9:
+
+    This version contains fixes for the pathname errors in the Transformers module
+    of DLStudio. The errors were related to where the models and the checkpoints
+    were supposed to be stored during training.
+
   Version 2.4.8:
 
     In this version, I have made two important changes to the Transformers module
     in DLStudio: (1) The Transformers module now includes a new class that I have
     named visTransformer that works like the famous Vision Transformer (ViT)
     proposed by Dosovitskiy et al. And (2) I have made changes to the QKV code for
     the calculation of self and cross attention in all of the Transformer classes
@@ -45,17 +50,17 @@
     GenerateNewImageSamples.py.  Other changes include minor clean-up of the main
     doc page for GenerativeDiffusion module and of a couple of the functions in
     the module.
 
   Version 2.4.2:
 
     DLStudio now includes a new module devoted to data modeling with diffusion.
-    This module, named GenerativeDiffusion, is a co-class of DLStudio.  That is,
-    GenerativeDiffusion resides at the same level of software abstraction as the
-    main DLStudio class in the platform.  See the README in the new
+    This module, named GenerativeDiffusion, is a module in the overall DLStudio 
+    platform.  The GenerativeDiffusion class resides at the same level of software 
+    abstraction as the main DLStudio class in the platform.  See the README in the
     ExamplesDiffusion directory of the distribution for how to experiment with the
     diffusion based code in DLStudio.
 
   Version 2.3.6:
 
     Gets rid of the inadvertently hardcoded value for the batch size in the
     testing part of the code for Semantic Segmentation.
@@ -159,16 +164,16 @@
     these loss functions is the script object_detection_and_localization_iou.py in
     the Examples directory of DLStudio.
 
   Version 2.2.2:
 
     This version of DLStudio presents my implementation of transformers in deep
     learning. You will find two transformer implementations in the Transformers
-    co-class of DLStudio in the distribution directory: TransformerFG and
-    TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
+    module of the DLStudio platform in the distribution directory: TransformerFG 
+    and TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
     Generation"; it is my implementation of the architecture presented originally
     in the seminal paper "Attention is All You Need" by Vaswani et el.  And the
     second, TransformerPreLN ("PreLN" stands for "Pre Layer Norm") is a small but
     important modification of the original idea that is based on the paper "On
     Layer Normalization in the Transformer Architecture" by Xiong et al.  I could
     have easily combined the two implementations with a small number of
     conditional statements to account for the differences, however I have chosen
@@ -182,22 +187,22 @@
     components of a transformer for educational purposes.  As things stand, these
     versions contain features that did not make into the public release version
     2.2.2 on account of inadequate testing.  I may include those features in
     versions of DLStudio after 2.2.2.
 
   Version 2.1.6:
 
-    All the changes are confined to the DataPrediction co-class of the DLStudio
-    module.  After posting the previous version, I noticed that the quality of the
-    code in DataPrediction was not up to par.  The new version presents a
+    All the changes are confined to the DataPrediction module in the DLStudio
+    platform.  After posting the previous version, I noticed that the quality of 
+    the code in DataPrediction was not up to par.  The new version presents a
     cleaned-up version of the DataPrediction class.
 
   Version 2.1.5:
 
-    DLStudio has now been equipped with a new co-class named DataPrediction whose
+    DLStudio has now been equipped with a new module named DataPrediction whose
     focus is solely on solving data prediction problems for time-series data.  A
     time-series consists of a sequence of observations recorded at regular
     intervals.  These could, for example, be the price of a stock share recorded
     every hour; the hourly recordings of electrical load at your local power
     utility company; the mean average temperature recorded on an annual basis; and
     so on.  We want to use the past observations to predict the value of the next
     one.  While data prediction has much in common with other forms of sequence
@@ -235,16 +240,16 @@
     classes AdversarialNetworks and Seq2SeqNetworks to AdversarialLearning and
     Seq2SeqLearning, respectively.
 
   Version 2.1.0:
 
     I have reorganized the code base a bit to make it easier for DLStudio to grow
     in the future.  This I did by moving the sequence-to-sequence learning
-    (seq2seq) code to a separate co-class of the main DLStudio class.  The name of
-    the new class is Seq2SeqLearning and it resides at the top level of the
+    (seq2seq) code to a separate module of the DLStudio platform.  The name of
+    the new module is Seq2SeqLearning and it resides at the top level of the
     distribution.
 
   Version 2.0.9:
 
     With this version, DLStudio comes with educational material on
     sequence-to-sequence learning (seq2seq). To that end, I have included the
     following two new classes in DLStudio: (1) Seq2SeqWithLearnableEmbeddings for
@@ -434,32 +439,33 @@
     key features of neural network architectures.  These implementations, along
     with their explanations through detailed slide presentations at our Deep
     Learning class website at Purdue, result in an educational framework that is
     much more efficient in what it can deliver within the time constraints of a
     single semester.
 
     DLStudio facilitates learning through a combination of inner classes of the
-    main module class --- called DLStudio naturally --- and several co-classes of
-    the main class that deal with adversarial learning, sequence-to-sequence
-    learning, data prediction, text analysis, and transformers.
+    main module class --- called DLStudio naturally --- and several modules of
+    the overall platform.  These modules deal with Adversarial Learning, 
+    Sequence-to-Sequence Learning, Diffusion, Data Prediction, Text Analysis, 
+    and Transformers.
 
     For the most part, the common code that you'd need in different scenarios for
     using neural networks has been placed inside the definition of the main
     DLStudio class in a file named DLStudio.py in the distribution.  That makes
     more compact the definition of the other inner classes within DLStudio. And,
     to a certain extent, that also results in a bit more compact code in the
-    co-classes of DLStudio.
+    different modules in the DLStudio platform.
 
 @tag2_skip
     SKIP CONNECTIONS:
 
     You can use DLStudio's inner class BMEnet to experiment with connection
     skipping in a deep network. Connection skipping means to provide shortcuts in
     a computational graph around the commonly used network components like
-    convolutional and other types of layers.  In the absence of such shortcuits,
+    convolutional and other types of layers.  In the absence of such shortcuts,
     deep networks suffer from the problem of vanishing gradients that degrades
     their performance.  Vanishing gradients means that the gradients of the loss
     calculated in the early layers of a network become increasingly muted as the
     network becomes deeper.  An important mitigation strategy for addressing this
     problem consists of creating a CNN using blocks with skip connections.
 
     As shown in the script playing_with_skip_connections.py in the Examples
@@ -669,15 +675,15 @@
     The pre-trained word2vec embeddings used in these scripts are accessed
     through the popular gensim library.
 
 
 @tag2_adversarial
     DATA MODELING WITH ADVERSARIAL LEARNING:
 
-    Starting with version 2.0.3, DLStudio includes a separate co-class named
+    Starting with version 2.0.3, DLStudio includes a separate module named
     AdversarialLearning for experimenting with different adversarial learning
     approaches for data modeling.  Adversarial Learning consists of simultaneously
     training a Generator and a Discriminator (or, a Generator and a Critic) with
     the goal of getting the Generator to produce from pure noise images that look
     like those in the training dataset.  When Generator-Discriminator pairs are
     used, the Discriminator's job is to become an expert at recognizing the
     training images so it can let us know when the generator produces an image
@@ -770,15 +776,15 @@
     options shown in the scripts) are included in a subdirectory named
     RVLCloud_based_results.
 
 
 @tag2_diffusion
     DATA MODELING WITH DIFFUSION:
 
-    Starting with Version 2.4.2, DLStudio includes a co-class named
+    Starting with Version 2.4.2, DLStudio includes a new module named
     GenerativeDiffusion for experimenting with what's known as "Denoising
     Diffusion".  The Denoising Diffusion approach to data modeling is based on the
     interaction between two Markov Chains: A forward chain called the q-chain and
     a reverse chain called the p-chain.  Both chains operate concurrently as
     follows and involved T timesteps where the value of T is a user-specified
     parameter.
 
@@ -873,17 +879,16 @@
 
     Sequence-to-sequence learning (seq2seq) is about predicting an outcome
     sequence from a causation sequence, or, said another way, a target sequence
     from a source sequence.  Automatic machine translation is probably one of the
     most popular applications of seq2seq.  DLStudio uses English-to-Spanish
     translation to illustrate the programming idioms and the PyTorch structures
     you need for seq2seq.  To that end, Version 2.1.0 of DLStudio includes a
-    co-class (meaning a class that resides at the top level in the distribution)
-    named Seq2SeqLearning that consists of the following two demonstration
-    classes:
+    new module named Seq2SeqLearning that consists of the following two 
+    demonstration classes:
 
         1.  Seq2SeqWithLearnableEmbeddings
 
         2.  Seq2SeqWithPretrainedEmbeddings
 
     As their names imply, the first is for seq2seq with learnable embeddings and
     the second for seq2seq with pre-trained embeddings like word2vec or fasttext.
@@ -929,16 +934,16 @@
     DATA PREDICTION
 
     Let's say you have a sequence of observations recorded at regular intervals.
     These could, for example, be the price of a stock share recorded every hour;
     the hourly recordings of electrical load at your local power utility company;
     the mean average temperature recorded on an annual basis; and so on.  We want
     to use the past observations to predict the value of the next one.  Solving
-    these types of problems is the focus of the DataPrediction co-class of
-    DLStudio.
+    these types of problems is the focus of the DataPrediction module in the
+    DLStudio platform.
 
     As a problem, data prediction has much in common with text analytics and
     seq2seq processing, in the sense that the prediction at the next time instant
     must be based on the previous observations in a manner similar to what we do
     in text analytics where the next word is understood taking into account all
     the previous words in a sentence.  However, there are three significant
     differences between purely numerical data prediction problems and text-based
@@ -998,15 +1003,15 @@
     the Reset gates of a regular GRU into a single gate called the Forget Gate.
     You could say that pmGRU is a lightweight version of a regular GRU and its use
     may therefore lead to a slight loss of accuracy in the predictions.  You will
     find it educational to compare the performance you get with my pmGRU-based
     implementation with an implementation that uses PyTorch's GRU for the same
     dataset.
 
-    Your main entry point for experimenting with the DataPrediction co-class is
+    Your main entry point for experimenting with the DataPrediction module is
     the following script in the ExamplesDataPrediction directory of the DLStudio
     distribution:
 
         power_load_prediction_with_pmGRU.py
 
     Before you can run this script, you would need to download the training
     dataset used in this example.  See the "For Data Prediction" part of the "The
@@ -1046,15 +1051,15 @@
     part of the logic in a visTransformer is identical to what it is in a
     transformer class for Seq2SeqLearning learning.  That logic kicks in after you
     have divided an image into patches and you represent each patch by an
     embedding vector --- in exactly the same as when you represent a word or a
     token in a sentence by an embedding vector.
 
     You will see three different implementations of the transformer architecture in
-    the Transformers co-class of DLStudio:
+    the Transformers module of the DLStudio platform:
 
           TransformerFG
 
           TransformerPreLN
 
           visTransformer
 
@@ -1066,15 +1071,15 @@
     the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
     the same architecture but with the modification suggested by Xiong et al. for
     more stable learning.  Since, the modification is small from an architectural
     standpoint, I could have combined both transformer types in the same
     implementation with some conditional logic to account for the differences.
     However, I have chosen to keep them separate mostly for educational purposes.
     Further details on these implementations are in the documentation blocks in
-    the Transformers co-class.  
+    the Transformers module.
 
     The visTransformer implementation is based on the paper "An Image is Worth
     16x16 Words: Transformers for Image Recognition at Scale'' by Dosovitskiy et
     al.
  
     If you want to use my code for learning the main ideas related to how to
     create purely attention based networks, your starting point for that should be
@@ -1393,17 +1398,16 @@
 
 
 @tag_inner_classes
 THE MAIN INNER CLASSES OF THE DLStudio CLASS:
 
     By "inner classes" I mean the classes that are defined within the class file
     DLStudio.py in the DLStudio directory of the distribution.  The DLStudio
-    platform also includes what I have referred to as the Co-Classes in the next
-    section.  A Co-Class resides at the same level of abstraction as the main
-    DLStudio class defined in the DLStudio.py file.
+    platform also includes several modules that reside at the same level of 
+    software abstraction as the main DLStudio class defined in the DLStudio.py file.
 
     The purpose of the following two inner classes is to demonstrate how you can
     create a custom class for your own network and test it within the framework
     provided by DLStudio.
 
     (1)  class ExperimentsWithSequential
 
@@ -1498,24 +1502,25 @@
          this inner class uses the pre-trained 300-element word2vec embeddings as
          made available by Google for 3 million words and phrases drawn from the
          Google News dataset. In DLStudio, we access these embeddings through the
          popular gensim library.
 
 
 @tag_coclasses
-CO-CLASSES IN THE DLStudio PLATFORM:
+MODULES IN THE DLStudio PLATFORM:
 
-    As stated at the beginning of the previous section, a Co-Class resides at the
-    same level of abstraction in the distribution directory as the main DLStudio
-    platform. Each Co-Class is defined in a separate subdirectory at the top level
-    of the distribution directory.  While the main DLStudio class is defined in a
-    subdirectory of the same name, the other subdirectories that contain
-    definitions for the co-classes are named AdversarialLearning, Seq2SeqLearning,
-    DataPrediction, Transformers, and MetricLearning.  What follows in this
-    section are additional details regarding these co-classes:
+    As stated at the beginning of the previous section, a module resides at the
+    same level of software abstraction in the distribution directory as the main
+    DLStudio class in the platform. Each module is defined in a separate
+    subdirectory at the top level of the distribution directory.  While the main
+    DLStudio class is defined in a subdirectory of the same name, the other
+    subdirectories that contain the definitions for the modules are named
+    AdversarialLearning, Seq2SeqLearning, DataPrediction, Transformers,
+    GenerativeDiffusion, and MetricLearning.  What follows in this section are
+    additional details regarding these co-classes:
 
 
 @tag_coclass1
     ===================
     AdversarialLearning:
     ===================
 
@@ -1571,15 +1576,15 @@
     The former is called the q-chain and the latter the p-chain.  The incremental
     diffusion in the q-chain is with known amount of Gaussian isotropic noise.  In
     the p-chain, on the other hand, the goal is for a neural network to learn from
     the diffusion carried out in the q-chain how to carry out a denoising
     operation that would amount to a reversal of that diffusion.
 
     All of the key elements of the code that I have presented in the
-    GenerativeDiffusion co-class are extracted from OpenAI's "Improved Diffusion"
+    GenerativeDiffusion module are extracted from OpenAI's "Improved Diffusion"
     project at GitHub that presents a PyTorch implementation of the work authored
     by Nichol and Dhariwal in their very famous paper "Improved Denoising
     Diffusion Probabilistic Models". See the beginning part of the doc page for
     the GenerativeDiffusion module for URLs to the GitHub code and their
     publication.
 
     If you want to play with the code in GenerativeDiffusion, your starting point
@@ -1611,15 +1616,15 @@
     your overall network learn on its own what are known as vector embeddings for
     the words; or (2) Use pre-trained embeddings as provided by word2vec or
     Fasttext.
 
     After you have resolved the issue of word representation, your next challenge
     is how to implement the attention mechanism that you're going to need for
     aligning the similar grammatical units in the two languages. The seq2seq code
-    demonstrated in this co-class uses the attention model proposed by Bahdanau,
+    demonstrated in this module uses the attention model proposed by Bahdanau,
     Cho, and Bengio in the form of a separate Attention class.  The name of this
     attention class is Attention_BCB.  In a separate attention class named
     Attention_SR, I have also included the attention mechanism used by Sean
     Robertson in his very popular NLP tutorial at the main PyTorch website.
 
     Seq2SeqLearning contains the following two inner classes for illustrating
     seq2seq:
@@ -1707,15 +1712,15 @@
     TransformerPreLN is my implementation of the original idea along with the
     modifications suggested by Xiong et al. in their paper "On Layer Normalization
     in the Transformer Architecture" for more stable learning.  The two versions
     of transformers differ in only one respect: The placement of the LayerNorm in
     relation to the architectural components related to attention and the
     feedforward network.  Literally, the difference is small, yet its consequences
     are significant regarding the stability of learning.  Finally, visTransformer
-    is my implementation of the Vision Transformer as presented in the famou paper
+    is my implementation of the Vision Transformer as presented in the famous paper
     "An Image is Worth 16x16$ Words: Transformers for Image Recognition at Scale''
     by Dosovitskiy et al.
 
     The fundamentals of how the attention works in all three transformer based
     implementations in the Transformers module are exactly the same.  For
     self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
     each word w_i in a sentence.  For a given w_i, the dot product of its Q_i with
@@ -1830,15 +1835,15 @@
     triplets (i,j,k) in which two indices are the same.  If B is the batch size,
     this is easily done by first forming a BxB array that is the logical negation
     of a Boolean array of the same size whose True values are only on the
     diagonal.  We can reshape this BxB Boolean array into three BxBxB shaped
     Boolean arrays, the first in which the True values exist only where i and j
     values are not the same, the second in which the True values occur only when i
     and k index values are not the same, and the third that has True values only
-    when the j and k index values are not the same.  By taking a logial AND of all
+    when the j and k index values are not the same.  By taking a logical AND of all
     three BxBxB Boolean arrays, we get the result we want.  Next, we construct a
     BxBxB Boolean tensor in which the True values occur only where the first two
     index values imply that their corresponding labels are identical and where the
     last index corresponds to a label that does not agree with that for the first
     two index values.
 
     Even after you have formed the triplets, your next mini-challenge is to
@@ -1868,15 +1873,15 @@
 Examples DIRECTORY:
 
     The Examples subdirectory in the distribution contains the following scripts:
 
     (1)  playing_with_reconfig.py
 
          Shows how you can specify a convolution network with a configuration
-         string.  The DLStudio module parses the string constructs the network.
+         string.  The main DLStudio class parses the string constructs the network.
 
     (2)  playing_with_sequential.py
 
          Shows you how you can call on a custom inner class of the 'DLStudio'
          module that is meant to experiment with your own network.  The name of
          the inner class in this example script is ExperimentsWithSequential
 
@@ -1895,22 +1900,22 @@
          directly illustrate in a classroom setting the improvement you can get
          with skip connections.  And by giving an appropriate value to the "depth"
          option, you can show results for networks of different depths.
 
     (6)  custom_data_loading.py
 
          This script shows how to use the custom dataloader in the inner class
-         CustomDataLoading of the DLStudio module.  That custom dataloader is
+         CustomDataLoading of the main DLStudio class.  That custom dataloader is
          meant specifically for the PurdueShapes5 dataset that is used in object
          detection and localization experiments in DLStudio.
 
     (7)  object_detection_and_localization.py
 
          This script shows how you can use the functionality provided by the inner
-         class DetectAndLocalize of the DLStudio module for experimenting with
+         class DetectAndLocalize of the main DLStudio class for experimenting with
          object detection and localization.  Detecting and localizing (D&L)
          objects in images is a more difficult problem than just classifying the
          objects.  D&L requires that your CNN make two different types of
          inferences simultaneously, one for classification and the other for
          localization.  For the localization part, the CNN must carry out what is
          known as regression. What that means is that the CNN must output the
          numerical values for the bounding box that encloses the object that was
@@ -2075,23 +2080,23 @@
          is explained in the main comment doc associated with the class
          Seq2SeqWithPretrainedEmbeddings.
 
 
 @tag_examples_predict
 ExamplesDataPrediction DIRECTORY:
 
-    The ExampsleDataPrediction directory of the distribution contains the
+    The ExamplesDataPrediction directory of the distribution contains the
     following script for demonstrating data prediction for time-series data:
 
         power_load_prediction_with_pmGRU.py
 
     This script uses a subset of the dataset provided by Kaggle for one of their
     machine learning competitions.  The dataset consists of over 10-years worth of
     hourly electric load recordings made available by several utilities in the
-    east and the midwest of the United States.  You can download this dataset from
+    east and the Midwest of the United States.  You can download this dataset from
     a link at the top of the main DLStudio doc page.
 
 
 @tag_examples_xform
 ExamplesTransformers DIRECTORY:
 
     The ExamplesTransformers directory of the distribution contains the following
@@ -2101,16 +2106,16 @@
         seq2seq_with_transformerPreLN.py         
 
         image_recog_with_visTransformer.py
         test_checkpoint_for_visTransformer.py 
 
 
     The first two scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
-    the example scripts associated with that co-class. The last two relate to my
+    similar to what's demonstrated by the code in the Seq2SeqLearning module and
+    the example scripts associated with that module. The last two relate to my
     demonstration of image recognition with a transformer based implementation.  I
     have used the CFAR10 dataset for image recognition.
 
 
 @tag_examples_metric
 ExamplesMetricLearning DIRECTORY:
 
@@ -2130,15 +2135,15 @@
 
 @tag_datasets
 THE DATASETS INCLUDED: 
 
     [must be downloaded separately]
 
 @tag2_main_dlstudio
-    FOR THE MAIN DLStudio MODULE:
+    FOR THE MAIN DLStudio CLASS and its INNER CLASSES:
 
         Download the dataset archive 'datasets_for_DLStudio.tar.gz' through the
         link "Download the image datasets for the main DLStudio Class" provided at
         the top of this documentation page and store it in the 'Example' directory
         of the distribution.  Subsequently, execute the following command in the
         'Examples' directory:
     
@@ -2364,15 +2369,15 @@
         That will create a 'data' subdirectory in the ExamplesTransformers
         directory and deposit in that subdirectory the following archives
 
             en_es_xformer_8_10000.tar.gz
             en_es_xformer_8_90000.tar.gz
 
         These are both derived from the same data source as in the dataset for the
-        examples associated with the Seq2SeqLearning co-class.  The first has only
+        examples associated with the Seq2SeqLearning module.  The first has only
         10,000 pars of English-Spanish sentences and meant primarily for debugging
         purposes.  The second contains 90000 pairs of such sentences.  The number
         '8' in the dataset names means that no sentence contains more than 8 real
         words.  With the "SOS" and "EOS" tokens used as sentence delimiters, the
         maximum number of words in each sentence in either language is 10.
 
 
@@ -2407,15 +2412,15 @@
     Version 2.2.2: My laboratory's (RVL) journey into the world of transformers
     began with a series of lab seminars by Constantine Roros and Rahul Deshmukh.
     Several subsequent conversations with them were instrumental in helping me
     improve the understanding I had gained from the seminars.  Additional
     conversations with Rahul about the issue of masking were important to how I
     eventually implemented those ideas in my code.
 
-    Rahul Deshmukh discovered the reason as to why my implmentation of the skip
+    Rahul Deshmukh discovered the reason as to why my implementation of the skip
     connection code was not working with the more recent versions of PyTorch.  My
     problem was using in-place operations in the forward() of the networks that
     called for connection skipping. This led to the release of Version 2.3.3 of
     DLStudio.
 
     The main reason for Version 2.3.4 was my new design for the SkipBlock class
     and also my easier-to-understand code for the BMEnet class that showcases the
@@ -2424,15 +2429,15 @@
     Cheng-Hao Chen reported that when a SkipBlock was asked to change the channels
     from its input to its output but without downsampling the input, that elicited
     an error from the system.  Cheng-Hao also provided a correction for the error.
     Thanks, Cheng-Hao!
 
     Aditya Chauhan proved to be a great sounding board in my journey into the land
     of diffusion that led to Version 2.4.2.  I particularly appreciated Aditya's
-    help in understanding how the attention mechanism worked in the OpanAI code
+    help in understanding how the attention mechanism worked in the OpenAI code
     library at GitHub.  Aditya is working for his PhD in RVL.  Thanks, Aditya!
 
 
 @tag_about_the_author
 ABOUT THE AUTHOR:
 
     The author, Avinash Kak, is a professor of Electrical and Computer Engineering
@@ -3261,16 +3266,16 @@
         designing a custom data loader.  Ordinarily, if the basic format of how the dataset
         is stored is similar to one of the datasets that the Torchvision module knows about,
         you can go ahead and use that for your own dataset.  At worst, you may need to carry
         out some light customizations depending on the number of classes involved, etc.
 
         However, if the underlying dataset is stored in a manner that does not look like
         anything in Torchvision, you have no choice but to supply yourself all of the data
-        loading infrastructure.  That is what this inner class of the DLStudio module is all
-        about.
+        loading infrastructure.  That is what this inner class of the main DLStudio class 
+        is all about.
 
         The custom data loading exercise here is related to a dataset called PurdueShapes5
         that contains 32x32 images of binary shapes belonging to the following five classes:
 
                        1.  rectangle
                        2.  triangle
                        3.  disk
@@ -4484,15 +4489,15 @@
 
     ###%%%
     ########################################################################################
     ##################  Start Definition of Inner Class SemanticSegmentation  ##############
 
     class SemanticSegmentation(nn.Module):             
         """
-        The purpose of this inner class is to be able to use the DLStudio module for
+        The purpose of this inner class is to be able to use the DLStudio platform for
         experiments with semantic segmentation.  At its simplest level, the purpose of
         semantic segmentation is to assign correct labels to the different objects in a
         scene, while localizing them at the same time.  At a more sophisticated level, a
         system that carries out semantic segmentation should also output a symbolic
         expression based on the objects found in the image and their spatial relationships
         with one another.
 
@@ -5054,15 +5059,15 @@
 
     ###%%%
     ########################################################################################
     ##################  Start Definition of Inner Class TextClassification  ################
 
     class TextClassification(nn.Module):             
         """
-        The purpose of this inner class is to be able to use the DLStudio module for simple 
+        The purpose of this inner class is to be able to use the DLStudio platform for simple 
         experiments in text classification.  Consider, for example, the problem of automatic 
         classification of variable-length user feedback: you want to create a neural network
         that can label an uploaded product review of arbitrary length as positive or negative.  
         One way to solve this problem is with a recurrent neural network in which you use a 
         hidden state for characterizing a variable-length product review with a fixed-length 
         state vector.  This inner class allows you to carry out such experiments.
```

### Comparing `DLStudio-2.4.8/DLStudio/__init__.py` & `DLStudio-2.4.9/DLStudio/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/DLStudio-2.4.8.html` & `DLStudio-2.4.9/DLStudio-2.4.9.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
 <head>
 <title>
-DLStudio-2.4.8.html
+DLStudio-2.4.9.html
 </title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 <style type="text/css">
 p.morelinespace {
     line-height: 130%;
     font-weight: bold;
 }
@@ -21,32 +21,32 @@
 </style>
 </head>
 
 <body>  
 <hr class="myhr1">
 <div style="color:blue; font-size:300%">  
   <strong>DLStudio</strong></div>
-<div style="color:blue; font-size:150%"> Version 2.4.8, &nbsp; 2024-April-27<br>
+<div style="color:blue; font-size:150%"> Version 2.4.9, &nbsp; 2024-May-1<br>
 <font="-1">A software platform for teaching the Deep Learning class at Purdue University</font><br>
 </div>
 <hr class="myhr1">
 <br>
 <div style="font-size:125%; line-height:130%; font-weight: bold">
 DLStudio.py<br>
-Version:&nbsp;&nbsp;2.4.8<br>
+Version:&nbsp;&nbsp;2.4.9<br>
 Author:&nbsp;&nbsp;Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)<br>
-Date:&nbsp;&nbsp;2024-April-27<br>
+Date:&nbsp;&nbsp;2024-May-1<br>
 </div>
 <br>
 <table>
 <tr>
 <th style="text-align:left vertical-align:top">
 <div style="font-size:125%">
-<b>Download Version 2.4.8:</b>&nbsp;&nbsp;&nbsp;&nbsp;    
-<a HREF="https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz?download">gztar</a> 
+<b>Download Version 2.4.9:</b>&nbsp;&nbsp;&nbsp;&nbsp;    
+<a HREF="https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.tar.gz?download">gztar</a> 
 </div>
 <br>
 <br>
 <br>
 </th>
 <td style="text-align:center vertical-align:top padding:0">
 <div style="text-align:center">
@@ -74,27 +74,27 @@
 </div>
 </div>
 </td>
 </tr>
 <tr>
 <td>
 <div style="color:red">
-<a HREF="DLStudio-2.4.8_CodeOnly.html">View the main module code file in your browser</a> 
+<a HREF="DLStudio-2.4.9_CodeOnly.html">View the main module code file in your browser</a> 
 &nbsp;<br>
-<a HREF="AdversarialLearning-2.4.8_CodeOnly.html">View the Adversarial Learning code file in your browser</a>&nbsp;
+<a HREF="AdversarialLearning-2.4.9_CodeOnly.html">View the Adversarial Learning code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="Seq2SeqLearning-2.4.8_CodeOnly.html">View the Seq2Seq Learning code file in your browser</a>
+<a HREF="Seq2SeqLearning-2.4.9_CodeOnly.html">View the Seq2Seq Learning code file in your browser</a>
 &nbsp;<br>
-<a HREF="DataPrediction-2.4.8_CodeOnly.html">View the Data Prediction code file in your browser</a>&nbsp;
+<a HREF="DataPrediction-2.4.9_CodeOnly.html">View the Data Prediction code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="Transformers-2.4.8_CodeOnly.html">View the Transformers code file in your browser</a>&nbsp;
+<a HREF="Transformers-2.4.9_CodeOnly.html">View the Transformers code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="MetricLearning-2.4.8_CodeOnly.html">View the Metric Learning code file in your browser</a>&nbsp;
+<a HREF="MetricLearning-2.4.9_CodeOnly.html">View the Metric Learning code file in your browser</a>&nbsp;
 &nbsp;<br>
-<a HREF="GenerativeDiffusion-2.4.8_CodeOnly.html">View the Generative Diffusion code file in your browser</a>&nbsp;<br> 
+<a HREF="GenerativeDiffusion-2.4.9_CodeOnly.html">View the Generative Diffusion code file in your browser</a>&nbsp;<br> 
 &nbsp;<br>
 <a HREF="datasets_for_DLStudio.tar.gz">Download the image datasets for the main DLStudio module</a> 
 &nbsp;<br>
 <a HREF="datasets_for_AdversarialNetworks.tar.gz">Download the image datasets for adversarial learning and diffusion</a> 
 &nbsp;<br>
 <a HREF="text_datasets_for_DLStudio.tar.gz">Download the datasets for text classification</a> 
 &nbsp;<br>
@@ -113,17 +113,23 @@
 <br>
 <br>
 <span style="color:red; font-size:150%"><strong>CONTENTS:</strong></span>
 <br>
 <br>
 <div style="font-size:100%; line-height:180%; font-weight: bold">
 
-<a href=#100>CHANGE&nbsp;LOG</a><br><a href=#101>INTRODUCTION</a><br><a href=#102>&nbsp;&nbsp;&nbsp;&nbsp;SKIP&nbsp;CONNECTIONS</a><br><a href=#103>&nbsp;&nbsp;&nbsp;&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#104>&nbsp;&nbsp;&nbsp;&nbsp;NOISY&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#105>&nbsp;&nbsp;&nbsp;&nbsp;IoU&nbsp;REGRESSION&nbsp;FOR&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#106>&nbsp;&nbsp;&nbsp;&nbsp;SEMANTIC&nbsp;SEGMENTATION</a><br><a href=#107>&nbsp;&nbsp;&nbsp;&nbsp;TEXT&nbsp;CLASSIFICATION</a><br><a href=#108>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;ADVERSARIAL&nbsp;LEARNING</a><br><a href=#109>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;DIFFUSION</a><br><a href=#110>&nbsp;&nbsp;&nbsp;&nbsp;SEQUENCE-TO-SEQUENCE&nbsp;LEARNING&nbsp;WITH&nbsp;ATTENTION</a><br><a href=#111>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#112>&nbsp;&nbsp;&nbsp;&nbsp;TRANSFORMERS</a><br><a href=#113>&nbsp;&nbsp;&nbsp;&nbsp;METRIC&nbsp;LEARNING</a><br><a href=#114>INSTALLATION</a><br><a href=#115>USAGE</a><br><a href=#116>CONSTRUCTOR&nbsp;PARAMETERS</a><br><a href=#117>PUBLIC&nbsp;METHODS</a><br><a href=#118>THE&nbsp;MAIN&nbsp;INNER&nbsp;CLASSES&nbsp;OF&nbsp;THE&nbsp;DLStudio&nbsp;CLASS</a><br><a href=#119>CO-CLASSES&nbsp;IN&nbsp;THE&nbsp;DLStudio&nbsp;PLATFORM</a><br><a href=#120>Examples&nbsp;DIRECTORY</a><br><a href=#121>ExamplesAdversarialLearning&nbsp;DIRECTORY</a><br><a href=#122>ExamplesDiffusion&nbsp;DIRECTORY</a><br><a href=#123>ExamplesSeq2SeqLearning&nbsp;DIRECTORY</a><br><a href=#124>ExamplesDataPrediction&nbsp;DIRECTORY</a><br><a href=#125>ExamplesTransformers&nbsp;DIRECTORY</a><br><a href=#126>ExamplesMetricLearning&nbsp;DIRECTORY</a><br><a href=#127>THE&nbsp;DATASETS&nbsp;INCLUDED</a><br><a href=#128>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;THE&nbsp;MAIN&nbsp;DLStudio&nbsp;MODULE</a><br><a href=#129>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;Seq2Seq&nbsp;LEARNING</a><br><a href=#130>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;ADVERSARIAL&nbsp;LEARNING&nbsp;AND&nbsp;DIFFUSION</a><br><a href=#131>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#132>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;TRANSFORMERS</a><br><a href=#133>BUGS</a><br><a href=#134>ACKNOWLEDGMENTS</a><br><a href=#135>ABOUT&nbsp;THE&nbsp;AUTHOR</a><br><a href=#136>COPYRIGHT</a><br><br></div>
+<a href=#100>CHANGE&nbsp;LOG</a><br><a href=#101>INTRODUCTION</a><br><a href=#102>&nbsp;&nbsp;&nbsp;&nbsp;SKIP&nbsp;CONNECTIONS</a><br><a href=#103>&nbsp;&nbsp;&nbsp;&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#104>&nbsp;&nbsp;&nbsp;&nbsp;NOISY&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#105>&nbsp;&nbsp;&nbsp;&nbsp;IoU&nbsp;REGRESSION&nbsp;FOR&nbsp;OBJECT&nbsp;DETECTION&nbsp;AND&nbsp;LOCALIZATION</a><br><a href=#106>&nbsp;&nbsp;&nbsp;&nbsp;SEMANTIC&nbsp;SEGMENTATION</a><br><a href=#107>&nbsp;&nbsp;&nbsp;&nbsp;TEXT&nbsp;CLASSIFICATION</a><br><a href=#108>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;ADVERSARIAL&nbsp;LEARNING</a><br><a href=#109>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;MODELING&nbsp;WITH&nbsp;DIFFUSION</a><br><a href=#110>&nbsp;&nbsp;&nbsp;&nbsp;SEQUENCE-TO-SEQUENCE&nbsp;LEARNING&nbsp;WITH&nbsp;ATTENTION</a><br><a href=#111>&nbsp;&nbsp;&nbsp;&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#112>&nbsp;&nbsp;&nbsp;&nbsp;TRANSFORMERS</a><br><a href=#113>&nbsp;&nbsp;&nbsp;&nbsp;METRIC&nbsp;LEARNING</a><br><a href=#114>INSTALLATION</a><br><a href=#115>USAGE</a><br><a href=#116>CONSTRUCTOR&nbsp;PARAMETERS</a><br><a href=#117>PUBLIC&nbsp;METHODS</a><br><a href=#118>THE&nbsp;MAIN&nbsp;INNER&nbsp;CLASSES&nbsp;OF&nbsp;THE&nbsp;DLStudio&nbsp;CLASS</a><br><a href=#119>MODULES&nbsp;IN&nbsp;THE&nbsp;DLStudio&nbsp;PLATFORM</a><br><a href=#120>Examples&nbsp;DIRECTORY</a><br><a href=#121>ExamplesAdversarialLearning&nbsp;DIRECTORY</a><br><a href=#122>ExamplesDiffusion&nbsp;DIRECTORY</a><br><a href=#123>ExamplesSeq2SeqLearning&nbsp;DIRECTORY</a><br><a href=#124>ExamplesDataPrediction&nbsp;DIRECTORY</a><br><a href=#125>ExamplesTransformers&nbsp;DIRECTORY</a><br><a href=#126>ExamplesMetricLearning&nbsp;DIRECTORY</a><br><a href=#127>THE&nbsp;DATASETS&nbsp;INCLUDED</a><br><a href=#128>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;THE&nbsp;MAIN&nbsp;DLStudio&nbsp;CLASS&nbsp;and&nbsp;its&nbsp;INNER&nbsp;CLASSES</a><br><a href=#129>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;Seq2Seq&nbsp;LEARNING</a><br><a href=#130>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;ADVERSARIAL&nbsp;LEARNING&nbsp;AND&nbsp;DIFFUSION</a><br><a href=#131>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;DATA&nbsp;PREDICTION</a><br><a href=#132>&nbsp;&nbsp;&nbsp;&nbsp;FOR&nbsp;TRANSFORMERS</a><br><a href=#133>BUGS</a><br><a href=#134>ACKNOWLEDGMENTS</a><br><a href=#135>ABOUT&nbsp;THE&nbsp;AUTHOR</a><br><a href=#136>COPYRIGHT</a><br><br></div>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="100">CHANGE LOG</a></strong></span><br>&nbsp;<br>
+&nbsp;&nbsp;Version&nbsp;2.4.9:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;contains&nbsp;fixes&nbsp;for&nbsp;the&nbsp;pathname&nbsp;errors&nbsp;in&nbsp;the&nbsp;Transformers&nbsp;module<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;DLStudio.&nbsp;The&nbsp;errors&nbsp;were&nbsp;related&nbsp;to&nbsp;where&nbsp;the&nbsp;models&nbsp;and&nbsp;the&nbsp;checkpoints<br>
+&nbsp;&nbsp;&nbsp;&nbsp;were&nbsp;supposed&nbsp;to&nbsp;be&nbsp;stored&nbsp;during&nbsp;training.<br>
+&nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.4.8:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;this&nbsp;version,&nbsp;I&nbsp;have&nbsp;made&nbsp;two&nbsp;important&nbsp;changes&nbsp;to&nbsp;the&nbsp;Transformers&nbsp;module<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;DLStudio:&nbsp;(1)&nbsp;The&nbsp;Transformers&nbsp;module&nbsp;now&nbsp;includes&nbsp;a&nbsp;new&nbsp;class&nbsp;that&nbsp;I&nbsp;have<br>
 &nbsp;&nbsp;&nbsp;&nbsp;named&nbsp;visTransformer&nbsp;that&nbsp;works&nbsp;like&nbsp;the&nbsp;famous&nbsp;Vision&nbsp;Transformer&nbsp;(ViT)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;proposed&nbsp;by&nbsp;Dosovitskiy&nbsp;et&nbsp;al.&nbsp;And&nbsp;(2)&nbsp;I&nbsp;have&nbsp;made&nbsp;changes&nbsp;to&nbsp;the&nbsp;QKV&nbsp;code&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;calculation&nbsp;of&nbsp;self&nbsp;and&nbsp;cross&nbsp;attention&nbsp;in&nbsp;all&nbsp;of&nbsp;the&nbsp;Transformer&nbsp;classes<br>
@@ -143,17 +149,17 @@
 &nbsp;&nbsp;&nbsp;&nbsp;GenerateNewImageSamples.py.&nbsp;&nbsp;Other&nbsp;changes&nbsp;include&nbsp;minor&nbsp;clean-up&nbsp;of&nbsp;the&nbsp;main<br>
 &nbsp;&nbsp;&nbsp;&nbsp;doc&nbsp;page&nbsp;for&nbsp;GenerativeDiffusion&nbsp;module&nbsp;and&nbsp;of&nbsp;a&nbsp;couple&nbsp;of&nbsp;the&nbsp;functions&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;module.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.4.2:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;now&nbsp;includes&nbsp;a&nbsp;new&nbsp;module&nbsp;devoted&nbsp;to&nbsp;data&nbsp;modeling&nbsp;with&nbsp;diffusion.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module,&nbsp;named&nbsp;GenerativeDiffusion,&nbsp;is&nbsp;a&nbsp;co-class&nbsp;of&nbsp;DLStudio.&nbsp;&nbsp;That&nbsp;is,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion&nbsp;resides&nbsp;at&nbsp;the&nbsp;same&nbsp;level&nbsp;of&nbsp;software&nbsp;abstraction&nbsp;as&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;in&nbsp;the&nbsp;platform.&nbsp;&nbsp;See&nbsp;the&nbsp;README&nbsp;in&nbsp;the&nbsp;new<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module,&nbsp;named&nbsp;GenerativeDiffusion,&nbsp;is&nbsp;a&nbsp;module&nbsp;in&nbsp;the&nbsp;overall&nbsp;DLStudio&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;platform.&nbsp;&nbsp;The&nbsp;GenerativeDiffusion&nbsp;class&nbsp;resides&nbsp;at&nbsp;the&nbsp;same&nbsp;level&nbsp;of&nbsp;software&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;abstraction&nbsp;as&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;in&nbsp;the&nbsp;platform.&nbsp;&nbsp;See&nbsp;the&nbsp;README&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;ExamplesDiffusion&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution&nbsp;for&nbsp;how&nbsp;to&nbsp;experiment&nbsp;with&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;diffusion&nbsp;based&nbsp;code&nbsp;in&nbsp;DLStudio.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.3.6:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Gets&nbsp;rid&nbsp;of&nbsp;the&nbsp;inadvertently&nbsp;hardcoded&nbsp;value&nbsp;for&nbsp;the&nbsp;batch&nbsp;size&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;testing&nbsp;part&nbsp;of&nbsp;the&nbsp;code&nbsp;for&nbsp;Semantic&nbsp;Segmentation.<br>
@@ -257,16 +263,16 @@
 &nbsp;&nbsp;&nbsp;&nbsp;these&nbsp;loss&nbsp;functions&nbsp;is&nbsp;the&nbsp;script&nbsp;object_detection_and_localization_iou.py&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;of&nbsp;DLStudio.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.2.2:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;of&nbsp;DLStudio&nbsp;presents&nbsp;my&nbsp;implementation&nbsp;of&nbsp;transformers&nbsp;in&nbsp;deep<br>
 &nbsp;&nbsp;&nbsp;&nbsp;learning.&nbsp;You&nbsp;will&nbsp;find&nbsp;two&nbsp;transformer&nbsp;implementations&nbsp;in&nbsp;the&nbsp;Transformers<br>
-&nbsp;&nbsp;&nbsp;&nbsp;co-class&nbsp;of&nbsp;DLStudio&nbsp;in&nbsp;the&nbsp;distribution&nbsp;directory:&nbsp;TransformerFG&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN.&nbsp;&nbsp;"FG"&nbsp;in&nbsp;TransformerFG&nbsp;stands&nbsp;for&nbsp;"Transformer&nbsp;First<br>
+&nbsp;&nbsp;&nbsp;&nbsp;module&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;platform&nbsp;in&nbsp;the&nbsp;distribution&nbsp;directory:&nbsp;TransformerFG&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;TransformerPreLN.&nbsp;&nbsp;"FG"&nbsp;in&nbsp;TransformerFG&nbsp;stands&nbsp;for&nbsp;"Transformer&nbsp;First<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Generation";&nbsp;it&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;architecture&nbsp;presented&nbsp;originally<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;seminal&nbsp;paper&nbsp;"Attention&nbsp;is&nbsp;All&nbsp;You&nbsp;Need"&nbsp;by&nbsp;Vaswani&nbsp;et&nbsp;el.&nbsp;&nbsp;And&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;second,&nbsp;TransformerPreLN&nbsp;("PreLN"&nbsp;stands&nbsp;for&nbsp;"Pre&nbsp;Layer&nbsp;Norm")&nbsp;is&nbsp;a&nbsp;small&nbsp;but<br>
 &nbsp;&nbsp;&nbsp;&nbsp;important&nbsp;modification&nbsp;of&nbsp;the&nbsp;original&nbsp;idea&nbsp;that&nbsp;is&nbsp;based&nbsp;on&nbsp;the&nbsp;paper&nbsp;"On<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Layer&nbsp;Normalization&nbsp;in&nbsp;the&nbsp;Transformer&nbsp;Architecture"&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;&nbsp;I&nbsp;could<br>
 &nbsp;&nbsp;&nbsp;&nbsp;have&nbsp;easily&nbsp;combined&nbsp;the&nbsp;two&nbsp;implementations&nbsp;with&nbsp;a&nbsp;small&nbsp;number&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;conditional&nbsp;statements&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;differences,&nbsp;however&nbsp;I&nbsp;have&nbsp;chosen<br>
@@ -280,22 +286,22 @@
 &nbsp;&nbsp;&nbsp;&nbsp;components&nbsp;of&nbsp;a&nbsp;transformer&nbsp;for&nbsp;educational&nbsp;purposes.&nbsp;&nbsp;As&nbsp;things&nbsp;stand,&nbsp;these<br>
 &nbsp;&nbsp;&nbsp;&nbsp;versions&nbsp;contain&nbsp;features&nbsp;that&nbsp;did&nbsp;not&nbsp;make&nbsp;into&nbsp;the&nbsp;public&nbsp;release&nbsp;version<br>
 &nbsp;&nbsp;&nbsp;&nbsp;2.2.2&nbsp;on&nbsp;account&nbsp;of&nbsp;inadequate&nbsp;testing.&nbsp;&nbsp;I&nbsp;may&nbsp;include&nbsp;those&nbsp;features&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;versions&nbsp;of&nbsp;DLStudio&nbsp;after&nbsp;2.2.2.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.1.6:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;All&nbsp;the&nbsp;changes&nbsp;are&nbsp;confined&nbsp;to&nbsp;the&nbsp;DataPrediction&nbsp;co-class&nbsp;of&nbsp;the&nbsp;DLStudio<br>
-&nbsp;&nbsp;&nbsp;&nbsp;module.&nbsp;&nbsp;After&nbsp;posting&nbsp;the&nbsp;previous&nbsp;version,&nbsp;I&nbsp;noticed&nbsp;that&nbsp;the&nbsp;quality&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;code&nbsp;in&nbsp;DataPrediction&nbsp;was&nbsp;not&nbsp;up&nbsp;to&nbsp;par.&nbsp;&nbsp;The&nbsp;new&nbsp;version&nbsp;presents&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;All&nbsp;the&nbsp;changes&nbsp;are&nbsp;confined&nbsp;to&nbsp;the&nbsp;DataPrediction&nbsp;module&nbsp;in&nbsp;the&nbsp;DLStudio<br>
+&nbsp;&nbsp;&nbsp;&nbsp;platform.&nbsp;&nbsp;After&nbsp;posting&nbsp;the&nbsp;previous&nbsp;version,&nbsp;I&nbsp;noticed&nbsp;that&nbsp;the&nbsp;quality&nbsp;of&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;code&nbsp;in&nbsp;DataPrediction&nbsp;was&nbsp;not&nbsp;up&nbsp;to&nbsp;par.&nbsp;&nbsp;The&nbsp;new&nbsp;version&nbsp;presents&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;cleaned-up&nbsp;version&nbsp;of&nbsp;the&nbsp;DataPrediction&nbsp;class.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.1.5:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;has&nbsp;now&nbsp;been&nbsp;equipped&nbsp;with&nbsp;a&nbsp;new&nbsp;co-class&nbsp;named&nbsp;DataPrediction&nbsp;whose<br>
+&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;has&nbsp;now&nbsp;been&nbsp;equipped&nbsp;with&nbsp;a&nbsp;new&nbsp;module&nbsp;named&nbsp;DataPrediction&nbsp;whose<br>
 &nbsp;&nbsp;&nbsp;&nbsp;focus&nbsp;is&nbsp;solely&nbsp;on&nbsp;solving&nbsp;data&nbsp;prediction&nbsp;problems&nbsp;for&nbsp;time-series&nbsp;data.&nbsp;&nbsp;A<br>
 &nbsp;&nbsp;&nbsp;&nbsp;time-series&nbsp;consists&nbsp;of&nbsp;a&nbsp;sequence&nbsp;of&nbsp;observations&nbsp;recorded&nbsp;at&nbsp;regular<br>
 &nbsp;&nbsp;&nbsp;&nbsp;intervals.&nbsp;&nbsp;These&nbsp;could,&nbsp;for&nbsp;example,&nbsp;be&nbsp;the&nbsp;price&nbsp;of&nbsp;a&nbsp;stock&nbsp;share&nbsp;recorded<br>
 &nbsp;&nbsp;&nbsp;&nbsp;every&nbsp;hour;&nbsp;the&nbsp;hourly&nbsp;recordings&nbsp;of&nbsp;electrical&nbsp;load&nbsp;at&nbsp;your&nbsp;local&nbsp;power<br>
 &nbsp;&nbsp;&nbsp;&nbsp;utility&nbsp;company;&nbsp;the&nbsp;mean&nbsp;average&nbsp;temperature&nbsp;recorded&nbsp;on&nbsp;an&nbsp;annual&nbsp;basis;&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;so&nbsp;on.&nbsp;&nbsp;We&nbsp;want&nbsp;to&nbsp;use&nbsp;the&nbsp;past&nbsp;observations&nbsp;to&nbsp;predict&nbsp;the&nbsp;value&nbsp;of&nbsp;the&nbsp;next<br>
 &nbsp;&nbsp;&nbsp;&nbsp;one.&nbsp;&nbsp;While&nbsp;data&nbsp;prediction&nbsp;has&nbsp;much&nbsp;in&nbsp;common&nbsp;with&nbsp;other&nbsp;forms&nbsp;of&nbsp;sequence<br>
@@ -333,16 +339,16 @@
 &nbsp;&nbsp;&nbsp;&nbsp;classes&nbsp;AdversarialNetworks&nbsp;and&nbsp;Seq2SeqNetworks&nbsp;to&nbsp;AdversarialLearning&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Seq2SeqLearning,&nbsp;respectively.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.1.0:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;I&nbsp;have&nbsp;reorganized&nbsp;the&nbsp;code&nbsp;base&nbsp;a&nbsp;bit&nbsp;to&nbsp;make&nbsp;it&nbsp;easier&nbsp;for&nbsp;DLStudio&nbsp;to&nbsp;grow<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;future.&nbsp;&nbsp;This&nbsp;I&nbsp;did&nbsp;by&nbsp;moving&nbsp;the&nbsp;sequence-to-sequence&nbsp;learning<br>
-&nbsp;&nbsp;&nbsp;&nbsp;(seq2seq)&nbsp;code&nbsp;to&nbsp;a&nbsp;separate&nbsp;co-class&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class.&nbsp;&nbsp;The&nbsp;name&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;new&nbsp;class&nbsp;is&nbsp;Seq2SeqLearning&nbsp;and&nbsp;it&nbsp;resides&nbsp;at&nbsp;the&nbsp;top&nbsp;level&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(seq2seq)&nbsp;code&nbsp;to&nbsp;a&nbsp;separate&nbsp;module&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;platform.&nbsp;&nbsp;The&nbsp;name&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;new&nbsp;module&nbsp;is&nbsp;Seq2SeqLearning&nbsp;and&nbsp;it&nbsp;resides&nbsp;at&nbsp;the&nbsp;top&nbsp;level&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.9:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;With&nbsp;this&nbsp;version,&nbsp;DLStudio&nbsp;comes&nbsp;with&nbsp;educational&nbsp;material&nbsp;on<br>
 &nbsp;&nbsp;&nbsp;&nbsp;sequence-to-sequence&nbsp;learning&nbsp;(seq2seq).&nbsp;To&nbsp;that&nbsp;end,&nbsp;I&nbsp;have&nbsp;included&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;following&nbsp;two&nbsp;new&nbsp;classes&nbsp;in&nbsp;DLStudio:&nbsp;(1)&nbsp;Seq2SeqWithLearnableEmbeddings&nbsp;for<br>
@@ -530,30 +536,31 @@
 &nbsp;&nbsp;&nbsp;&nbsp;key&nbsp;features&nbsp;of&nbsp;neural&nbsp;network&nbsp;architectures.&nbsp;&nbsp;These&nbsp;implementations,&nbsp;along<br>
 &nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;their&nbsp;explanations&nbsp;through&nbsp;detailed&nbsp;slide&nbsp;presentations&nbsp;at&nbsp;our&nbsp;Deep<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Learning&nbsp;class&nbsp;website&nbsp;at&nbsp;Purdue,&nbsp;result&nbsp;in&nbsp;an&nbsp;educational&nbsp;framework&nbsp;that&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;much&nbsp;more&nbsp;efficient&nbsp;in&nbsp;what&nbsp;it&nbsp;can&nbsp;deliver&nbsp;within&nbsp;the&nbsp;time&nbsp;constraints&nbsp;of&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;single&nbsp;semester.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;facilitates&nbsp;learning&nbsp;through&nbsp;a&nbsp;combination&nbsp;of&nbsp;inner&nbsp;classes&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;main&nbsp;module&nbsp;class&nbsp;---&nbsp;called&nbsp;DLStudio&nbsp;naturally&nbsp;---&nbsp;and&nbsp;several&nbsp;co-classes&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;main&nbsp;class&nbsp;that&nbsp;deal&nbsp;with&nbsp;adversarial&nbsp;learning,&nbsp;sequence-to-sequence<br>
-&nbsp;&nbsp;&nbsp;&nbsp;learning,&nbsp;data&nbsp;prediction,&nbsp;text&nbsp;analysis,&nbsp;and&nbsp;transformers.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;main&nbsp;module&nbsp;class&nbsp;---&nbsp;called&nbsp;DLStudio&nbsp;naturally&nbsp;---&nbsp;and&nbsp;several&nbsp;modules&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;overall&nbsp;platform.&nbsp;&nbsp;These&nbsp;modules&nbsp;deal&nbsp;with&nbsp;Adversarial&nbsp;Learning,&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Sequence-to-Sequence&nbsp;Learning,&nbsp;Diffusion,&nbsp;Data&nbsp;Prediction,&nbsp;Text&nbsp;Analysis,&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;Transformers.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;For&nbsp;the&nbsp;most&nbsp;part,&nbsp;the&nbsp;common&nbsp;code&nbsp;that&nbsp;you'd&nbsp;need&nbsp;in&nbsp;different&nbsp;scenarios&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;using&nbsp;neural&nbsp;networks&nbsp;has&nbsp;been&nbsp;placed&nbsp;inside&nbsp;the&nbsp;definition&nbsp;of&nbsp;the&nbsp;main<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;class&nbsp;in&nbsp;a&nbsp;file&nbsp;named&nbsp;DLStudio.py&nbsp;in&nbsp;the&nbsp;distribution.&nbsp;&nbsp;That&nbsp;makes<br>
 &nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;compact&nbsp;the&nbsp;definition&nbsp;of&nbsp;the&nbsp;other&nbsp;inner&nbsp;classes&nbsp;within&nbsp;DLStudio.&nbsp;And,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;a&nbsp;certain&nbsp;extent,&nbsp;that&nbsp;also&nbsp;results&nbsp;in&nbsp;a&nbsp;bit&nbsp;more&nbsp;compact&nbsp;code&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;co-classes&nbsp;of&nbsp;DLStudio.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;modules&nbsp;in&nbsp;the&nbsp;DLStudio&nbsp;platform.<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="102">    SKIP CONNECTIONS</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;can&nbsp;use&nbsp;DLStudio's&nbsp;inner&nbsp;class&nbsp;BMEnet&nbsp;to&nbsp;experiment&nbsp;with&nbsp;connection<br>
 &nbsp;&nbsp;&nbsp;&nbsp;skipping&nbsp;in&nbsp;a&nbsp;deep&nbsp;network.&nbsp;Connection&nbsp;skipping&nbsp;means&nbsp;to&nbsp;provide&nbsp;shortcuts&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;computational&nbsp;graph&nbsp;around&nbsp;the&nbsp;commonly&nbsp;used&nbsp;network&nbsp;components&nbsp;like<br>
-&nbsp;&nbsp;&nbsp;&nbsp;convolutional&nbsp;and&nbsp;other&nbsp;types&nbsp;of&nbsp;layers.&nbsp;&nbsp;In&nbsp;the&nbsp;absence&nbsp;of&nbsp;such&nbsp;shortcuits,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;convolutional&nbsp;and&nbsp;other&nbsp;types&nbsp;of&nbsp;layers.&nbsp;&nbsp;In&nbsp;the&nbsp;absence&nbsp;of&nbsp;such&nbsp;shortcuts,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;deep&nbsp;networks&nbsp;suffer&nbsp;from&nbsp;the&nbsp;problem&nbsp;of&nbsp;vanishing&nbsp;gradients&nbsp;that&nbsp;degrades<br>
 &nbsp;&nbsp;&nbsp;&nbsp;their&nbsp;performance.&nbsp;&nbsp;Vanishing&nbsp;gradients&nbsp;means&nbsp;that&nbsp;the&nbsp;gradients&nbsp;of&nbsp;the&nbsp;loss<br>
 &nbsp;&nbsp;&nbsp;&nbsp;calculated&nbsp;in&nbsp;the&nbsp;early&nbsp;layers&nbsp;of&nbsp;a&nbsp;network&nbsp;become&nbsp;increasingly&nbsp;muted&nbsp;as&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;network&nbsp;becomes&nbsp;deeper.&nbsp;&nbsp;An&nbsp;important&nbsp;mitigation&nbsp;strategy&nbsp;for&nbsp;addressing&nbsp;this<br>
 &nbsp;&nbsp;&nbsp;&nbsp;problem&nbsp;consists&nbsp;of&nbsp;creating&nbsp;a&nbsp;CNN&nbsp;using&nbsp;blocks&nbsp;with&nbsp;skip&nbsp;connections.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;shown&nbsp;in&nbsp;the&nbsp;script&nbsp;playing_with_skip_connections.py&nbsp;in&nbsp;the&nbsp;Examples<br>
@@ -751,15 +758,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;text_classification_with_GRU_word2vec.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;pre-trained&nbsp;word2vec&nbsp;embeddings&nbsp;used&nbsp;in&nbsp;these&nbsp;scripts&nbsp;are&nbsp;accessed<br>
 &nbsp;&nbsp;&nbsp;&nbsp;through&nbsp;the&nbsp;popular&nbsp;gensim&nbsp;library.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="108">    DATA MODELING WITH ADVERSARIAL LEARNING</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Starting&nbsp;with&nbsp;version&nbsp;2.0.3,&nbsp;DLStudio&nbsp;includes&nbsp;a&nbsp;separate&nbsp;co-class&nbsp;named<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Starting&nbsp;with&nbsp;version&nbsp;2.0.3,&nbsp;DLStudio&nbsp;includes&nbsp;a&nbsp;separate&nbsp;module&nbsp;named<br>
 &nbsp;&nbsp;&nbsp;&nbsp;AdversarialLearning&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;different&nbsp;adversarial&nbsp;learning<br>
 &nbsp;&nbsp;&nbsp;&nbsp;approaches&nbsp;for&nbsp;data&nbsp;modeling.&nbsp;&nbsp;Adversarial&nbsp;Learning&nbsp;consists&nbsp;of&nbsp;simultaneously<br>
 &nbsp;&nbsp;&nbsp;&nbsp;training&nbsp;a&nbsp;Generator&nbsp;and&nbsp;a&nbsp;Discriminator&nbsp;(or,&nbsp;a&nbsp;Generator&nbsp;and&nbsp;a&nbsp;Critic)&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;goal&nbsp;of&nbsp;getting&nbsp;the&nbsp;Generator&nbsp;to&nbsp;produce&nbsp;from&nbsp;pure&nbsp;noise&nbsp;images&nbsp;that&nbsp;look<br>
 &nbsp;&nbsp;&nbsp;&nbsp;like&nbsp;those&nbsp;in&nbsp;the&nbsp;training&nbsp;dataset.&nbsp;&nbsp;When&nbsp;Generator-Discriminator&nbsp;pairs&nbsp;are<br>
 &nbsp;&nbsp;&nbsp;&nbsp;used,&nbsp;the&nbsp;Discriminator's&nbsp;job&nbsp;is&nbsp;to&nbsp;become&nbsp;an&nbsp;expert&nbsp;at&nbsp;recognizing&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;training&nbsp;images&nbsp;so&nbsp;it&nbsp;can&nbsp;let&nbsp;us&nbsp;know&nbsp;when&nbsp;the&nbsp;generator&nbsp;produces&nbsp;an&nbsp;image<br>
@@ -850,15 +857,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;fourth&nbsp;script&nbsp;includes&nbsp;a&nbsp;gradient&nbsp;penalty&nbsp;in&nbsp;the&nbsp;critic&nbsp;logic&nbsp;called&nbsp;on&nbsp;by&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;third&nbsp;script.&nbsp;&nbsp;The&nbsp;results&nbsp;produced&nbsp;by&nbsp;these&nbsp;scripts&nbsp;(for&nbsp;the&nbsp;constructor<br>
 &nbsp;&nbsp;&nbsp;&nbsp;options&nbsp;shown&nbsp;in&nbsp;the&nbsp;scripts)&nbsp;are&nbsp;included&nbsp;in&nbsp;a&nbsp;subdirectory&nbsp;named<br>
 &nbsp;&nbsp;&nbsp;&nbsp;RVLCloud_based_results.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="109">    DATA MODELING WITH DIFFUSION</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Starting&nbsp;with&nbsp;Version&nbsp;2.4.2,&nbsp;DLStudio&nbsp;includes&nbsp;a&nbsp;co-class&nbsp;named<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Starting&nbsp;with&nbsp;Version&nbsp;2.4.2,&nbsp;DLStudio&nbsp;includes&nbsp;a&nbsp;new&nbsp;module&nbsp;named<br>
 &nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;what's&nbsp;known&nbsp;as&nbsp;"Denoising<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Diffusion".&nbsp;&nbsp;The&nbsp;Denoising&nbsp;Diffusion&nbsp;approach&nbsp;to&nbsp;data&nbsp;modeling&nbsp;is&nbsp;based&nbsp;on&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;interaction&nbsp;between&nbsp;two&nbsp;Markov&nbsp;Chains:&nbsp;A&nbsp;forward&nbsp;chain&nbsp;called&nbsp;the&nbsp;q-chain&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;reverse&nbsp;chain&nbsp;called&nbsp;the&nbsp;p-chain.&nbsp;&nbsp;Both&nbsp;chains&nbsp;operate&nbsp;concurrently&nbsp;as<br>
 &nbsp;&nbsp;&nbsp;&nbsp;follows&nbsp;and&nbsp;involved&nbsp;T&nbsp;timesteps&nbsp;where&nbsp;the&nbsp;value&nbsp;of&nbsp;T&nbsp;is&nbsp;a&nbsp;user-specified<br>
 &nbsp;&nbsp;&nbsp;&nbsp;parameter.<br>
 &nbsp;<br>
@@ -951,17 +958,16 @@
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="110">    SEQUENCE-TO-SEQUENCE LEARNING WITH ATTENTION</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Sequence-to-sequence&nbsp;learning&nbsp;(seq2seq)&nbsp;is&nbsp;about&nbsp;predicting&nbsp;an&nbsp;outcome<br>
 &nbsp;&nbsp;&nbsp;&nbsp;sequence&nbsp;from&nbsp;a&nbsp;causation&nbsp;sequence,&nbsp;or,&nbsp;said&nbsp;another&nbsp;way,&nbsp;a&nbsp;target&nbsp;sequence<br>
 &nbsp;&nbsp;&nbsp;&nbsp;from&nbsp;a&nbsp;source&nbsp;sequence.&nbsp;&nbsp;Automatic&nbsp;machine&nbsp;translation&nbsp;is&nbsp;probably&nbsp;one&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;most&nbsp;popular&nbsp;applications&nbsp;of&nbsp;seq2seq.&nbsp;&nbsp;DLStudio&nbsp;uses&nbsp;English-to-Spanish<br>
 &nbsp;&nbsp;&nbsp;&nbsp;translation&nbsp;to&nbsp;illustrate&nbsp;the&nbsp;programming&nbsp;idioms&nbsp;and&nbsp;the&nbsp;PyTorch&nbsp;structures<br>
 &nbsp;&nbsp;&nbsp;&nbsp;you&nbsp;need&nbsp;for&nbsp;seq2seq.&nbsp;&nbsp;To&nbsp;that&nbsp;end,&nbsp;Version&nbsp;2.1.0&nbsp;of&nbsp;DLStudio&nbsp;includes&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;co-class&nbsp;(meaning&nbsp;a&nbsp;class&nbsp;that&nbsp;resides&nbsp;at&nbsp;the&nbsp;top&nbsp;level&nbsp;in&nbsp;the&nbsp;distribution)<br>
-&nbsp;&nbsp;&nbsp;&nbsp;named&nbsp;Seq2SeqLearning&nbsp;that&nbsp;consists&nbsp;of&nbsp;the&nbsp;following&nbsp;two&nbsp;demonstration<br>
-&nbsp;&nbsp;&nbsp;&nbsp;classes:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;new&nbsp;module&nbsp;named&nbsp;Seq2SeqLearning&nbsp;that&nbsp;consists&nbsp;of&nbsp;the&nbsp;following&nbsp;two&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;demonstration&nbsp;classes:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.&nbsp;&nbsp;Seq2SeqWithLearnableEmbeddings<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.&nbsp;&nbsp;Seq2SeqWithPretrainedEmbeddings<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;their&nbsp;names&nbsp;imply,&nbsp;the&nbsp;first&nbsp;is&nbsp;for&nbsp;seq2seq&nbsp;with&nbsp;learnable&nbsp;embeddings&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;second&nbsp;for&nbsp;seq2seq&nbsp;with&nbsp;pre-trained&nbsp;embeddings&nbsp;like&nbsp;word2vec&nbsp;or&nbsp;fasttext.<br>
@@ -1005,16 +1011,16 @@
 &nbsp;<br>
 <span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="111">    DATA PREDICTION</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Let's&nbsp;say&nbsp;you&nbsp;have&nbsp;a&nbsp;sequence&nbsp;of&nbsp;observations&nbsp;recorded&nbsp;at&nbsp;regular&nbsp;intervals.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;These&nbsp;could,&nbsp;for&nbsp;example,&nbsp;be&nbsp;the&nbsp;price&nbsp;of&nbsp;a&nbsp;stock&nbsp;share&nbsp;recorded&nbsp;every&nbsp;hour;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;hourly&nbsp;recordings&nbsp;of&nbsp;electrical&nbsp;load&nbsp;at&nbsp;your&nbsp;local&nbsp;power&nbsp;utility&nbsp;company;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;mean&nbsp;average&nbsp;temperature&nbsp;recorded&nbsp;on&nbsp;an&nbsp;annual&nbsp;basis;&nbsp;and&nbsp;so&nbsp;on.&nbsp;&nbsp;We&nbsp;want<br>
 &nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;use&nbsp;the&nbsp;past&nbsp;observations&nbsp;to&nbsp;predict&nbsp;the&nbsp;value&nbsp;of&nbsp;the&nbsp;next&nbsp;one.&nbsp;&nbsp;Solving<br>
-&nbsp;&nbsp;&nbsp;&nbsp;these&nbsp;types&nbsp;of&nbsp;problems&nbsp;is&nbsp;the&nbsp;focus&nbsp;of&nbsp;the&nbsp;DataPrediction&nbsp;co-class&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;DLStudio.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;these&nbsp;types&nbsp;of&nbsp;problems&nbsp;is&nbsp;the&nbsp;focus&nbsp;of&nbsp;the&nbsp;DataPrediction&nbsp;module&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;platform.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;a&nbsp;problem,&nbsp;data&nbsp;prediction&nbsp;has&nbsp;much&nbsp;in&nbsp;common&nbsp;with&nbsp;text&nbsp;analytics&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;seq2seq&nbsp;processing,&nbsp;in&nbsp;the&nbsp;sense&nbsp;that&nbsp;the&nbsp;prediction&nbsp;at&nbsp;the&nbsp;next&nbsp;time&nbsp;instant<br>
 &nbsp;&nbsp;&nbsp;&nbsp;must&nbsp;be&nbsp;based&nbsp;on&nbsp;the&nbsp;previous&nbsp;observations&nbsp;in&nbsp;a&nbsp;manner&nbsp;similar&nbsp;to&nbsp;what&nbsp;we&nbsp;do<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;text&nbsp;analytics&nbsp;where&nbsp;the&nbsp;next&nbsp;word&nbsp;is&nbsp;understood&nbsp;taking&nbsp;into&nbsp;account&nbsp;all<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;previous&nbsp;words&nbsp;in&nbsp;a&nbsp;sentence.&nbsp;&nbsp;However,&nbsp;there&nbsp;are&nbsp;three&nbsp;significant<br>
 &nbsp;&nbsp;&nbsp;&nbsp;differences&nbsp;between&nbsp;purely&nbsp;numerical&nbsp;data&nbsp;prediction&nbsp;problems&nbsp;and&nbsp;text-based<br>
@@ -1074,15 +1080,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Reset&nbsp;gates&nbsp;of&nbsp;a&nbsp;regular&nbsp;GRU&nbsp;into&nbsp;a&nbsp;single&nbsp;gate&nbsp;called&nbsp;the&nbsp;Forget&nbsp;Gate.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;could&nbsp;say&nbsp;that&nbsp;pmGRU&nbsp;is&nbsp;a&nbsp;lightweight&nbsp;version&nbsp;of&nbsp;a&nbsp;regular&nbsp;GRU&nbsp;and&nbsp;its&nbsp;use<br>
 &nbsp;&nbsp;&nbsp;&nbsp;may&nbsp;therefore&nbsp;lead&nbsp;to&nbsp;a&nbsp;slight&nbsp;loss&nbsp;of&nbsp;accuracy&nbsp;in&nbsp;the&nbsp;predictions.&nbsp;&nbsp;You&nbsp;will<br>
 &nbsp;&nbsp;&nbsp;&nbsp;find&nbsp;it&nbsp;educational&nbsp;to&nbsp;compare&nbsp;the&nbsp;performance&nbsp;you&nbsp;get&nbsp;with&nbsp;my&nbsp;pmGRU-based<br>
 &nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;with&nbsp;an&nbsp;implementation&nbsp;that&nbsp;uses&nbsp;PyTorch's&nbsp;GRU&nbsp;for&nbsp;the&nbsp;same<br>
 &nbsp;&nbsp;&nbsp;&nbsp;dataset.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Your&nbsp;main&nbsp;entry&nbsp;point&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;the&nbsp;DataPrediction&nbsp;co-class&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Your&nbsp;main&nbsp;entry&nbsp;point&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;the&nbsp;DataPrediction&nbsp;module&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;following&nbsp;script&nbsp;in&nbsp;the&nbsp;ExamplesDataPrediction&nbsp;directory&nbsp;of&nbsp;the&nbsp;DLStudio<br>
 &nbsp;&nbsp;&nbsp;&nbsp;distribution:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;power_load_prediction_with_pmGRU.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Before&nbsp;you&nbsp;can&nbsp;run&nbsp;this&nbsp;script,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;download&nbsp;the&nbsp;training<br>
 &nbsp;&nbsp;&nbsp;&nbsp;dataset&nbsp;used&nbsp;in&nbsp;this&nbsp;example.&nbsp;&nbsp;See&nbsp;the&nbsp;"For&nbsp;Data&nbsp;Prediction"&nbsp;part&nbsp;of&nbsp;the&nbsp;"The<br>
@@ -1120,15 +1126,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;part&nbsp;of&nbsp;the&nbsp;logic&nbsp;in&nbsp;a&nbsp;visTransformer&nbsp;is&nbsp;identical&nbsp;to&nbsp;what&nbsp;it&nbsp;is&nbsp;in&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;transformer&nbsp;class&nbsp;for&nbsp;Seq2SeqLearning&nbsp;learning.&nbsp;&nbsp;That&nbsp;logic&nbsp;kicks&nbsp;in&nbsp;after&nbsp;you<br>
 &nbsp;&nbsp;&nbsp;&nbsp;have&nbsp;divided&nbsp;an&nbsp;image&nbsp;into&nbsp;patches&nbsp;and&nbsp;you&nbsp;represent&nbsp;each&nbsp;patch&nbsp;by&nbsp;an<br>
 &nbsp;&nbsp;&nbsp;&nbsp;embedding&nbsp;vector&nbsp;---&nbsp;in&nbsp;exactly&nbsp;the&nbsp;same&nbsp;as&nbsp;when&nbsp;you&nbsp;represent&nbsp;a&nbsp;word&nbsp;or&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;token&nbsp;in&nbsp;a&nbsp;sentence&nbsp;by&nbsp;an&nbsp;embedding&nbsp;vector.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;see&nbsp;three&nbsp;different&nbsp;implementations&nbsp;of&nbsp;the&nbsp;transformer&nbsp;architecture&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;co-class&nbsp;of&nbsp;DLStudio:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;module&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;platform:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TransformerFG<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;visTransformer<br>
 &nbsp;<br>
@@ -1140,15 +1146,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;famous&nbsp;paper&nbsp;by&nbsp;Vaswani&nbsp;et&nbsp;al.&nbsp;&nbsp;and&nbsp;TransformerPreLN&nbsp;my&nbsp;implementation&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;same&nbsp;architecture&nbsp;but&nbsp;with&nbsp;the&nbsp;modification&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;Since,&nbsp;the&nbsp;modification&nbsp;is&nbsp;small&nbsp;from&nbsp;an&nbsp;architectural<br>
 &nbsp;&nbsp;&nbsp;&nbsp;standpoint,&nbsp;I&nbsp;could&nbsp;have&nbsp;combined&nbsp;both&nbsp;transformer&nbsp;types&nbsp;in&nbsp;the&nbsp;same<br>
 &nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;with&nbsp;some&nbsp;conditional&nbsp;logic&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;differences.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;However,&nbsp;I&nbsp;have&nbsp;chosen&nbsp;to&nbsp;keep&nbsp;them&nbsp;separate&nbsp;mostly&nbsp;for&nbsp;educational&nbsp;purposes.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Further&nbsp;details&nbsp;on&nbsp;these&nbsp;implementations&nbsp;are&nbsp;in&nbsp;the&nbsp;documentation&nbsp;blocks&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;co-class.&nbsp;&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;Transformers&nbsp;module.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;visTransformer&nbsp;implementation&nbsp;is&nbsp;based&nbsp;on&nbsp;the&nbsp;paper&nbsp;"An&nbsp;Image&nbsp;is&nbsp;Worth<br>
 &nbsp;&nbsp;&nbsp;&nbsp;16x16&nbsp;Words:&nbsp;Transformers&nbsp;for&nbsp;Image&nbsp;Recognition&nbsp;at&nbsp;Scale''&nbsp;by&nbsp;Dosovitskiy&nbsp;et<br>
 &nbsp;&nbsp;&nbsp;&nbsp;al.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;use&nbsp;my&nbsp;code&nbsp;for&nbsp;learning&nbsp;the&nbsp;main&nbsp;ideas&nbsp;related&nbsp;to&nbsp;how&nbsp;to<br>
 &nbsp;&nbsp;&nbsp;&nbsp;create&nbsp;purely&nbsp;attention&nbsp;based&nbsp;networks,&nbsp;your&nbsp;starting&nbsp;point&nbsp;for&nbsp;that&nbsp;should&nbsp;be<br>
@@ -1455,17 +1461,16 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;each&nbsp;layer&nbsp;in&nbsp;the&nbsp;network.&nbsp;The&nbsp;method&nbsp;has&nbsp;one&nbsp;input&nbsp;parameter&nbsp;which&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;set&nbsp;to&nbsp;the&nbsp;network&nbsp;whose&nbsp;summary&nbsp;you&nbsp;want&nbsp;to&nbsp;see.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="118">THE MAIN INNER CLASSES OF THE DLStudio CLASS</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;By&nbsp;"inner&nbsp;classes"&nbsp;I&nbsp;mean&nbsp;the&nbsp;classes&nbsp;that&nbsp;are&nbsp;defined&nbsp;within&nbsp;the&nbsp;class&nbsp;file<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio.py&nbsp;in&nbsp;the&nbsp;DLStudio&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution.&nbsp;&nbsp;The&nbsp;DLStudio<br>
-&nbsp;&nbsp;&nbsp;&nbsp;platform&nbsp;also&nbsp;includes&nbsp;what&nbsp;I&nbsp;have&nbsp;referred&nbsp;to&nbsp;as&nbsp;the&nbsp;Co-Classes&nbsp;in&nbsp;the&nbsp;next<br>
-&nbsp;&nbsp;&nbsp;&nbsp;section.&nbsp;&nbsp;A&nbsp;Co-Class&nbsp;resides&nbsp;at&nbsp;the&nbsp;same&nbsp;level&nbsp;of&nbsp;abstraction&nbsp;as&nbsp;the&nbsp;main<br>
-&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;class&nbsp;defined&nbsp;in&nbsp;the&nbsp;DLStudio.py&nbsp;file.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;platform&nbsp;also&nbsp;includes&nbsp;several&nbsp;modules&nbsp;that&nbsp;reside&nbsp;at&nbsp;the&nbsp;same&nbsp;level&nbsp;of&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;software&nbsp;abstraction&nbsp;as&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;defined&nbsp;in&nbsp;the&nbsp;DLStudio.py&nbsp;file.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;purpose&nbsp;of&nbsp;the&nbsp;following&nbsp;two&nbsp;inner&nbsp;classes&nbsp;is&nbsp;to&nbsp;demonstrate&nbsp;how&nbsp;you&nbsp;can<br>
 &nbsp;&nbsp;&nbsp;&nbsp;create&nbsp;a&nbsp;custom&nbsp;class&nbsp;for&nbsp;your&nbsp;own&nbsp;network&nbsp;and&nbsp;test&nbsp;it&nbsp;within&nbsp;the&nbsp;framework<br>
 &nbsp;&nbsp;&nbsp;&nbsp;provided&nbsp;by&nbsp;DLStudio.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp;&nbsp;class&nbsp;ExperimentsWithSequential<br>
 &nbsp;<br>
@@ -1559,23 +1564,24 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;basis&nbsp;of&nbsp;the&nbsp;contextual&nbsp;similarity&nbsp;of&nbsp;the&nbsp;words.&nbsp;The&nbsp;implementation&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;inner&nbsp;class&nbsp;uses&nbsp;the&nbsp;pre-trained&nbsp;300-element&nbsp;word2vec&nbsp;embeddings&nbsp;as<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;made&nbsp;available&nbsp;by&nbsp;Google&nbsp;for&nbsp;3&nbsp;million&nbsp;words&nbsp;and&nbsp;phrases&nbsp;drawn&nbsp;from&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Google&nbsp;News&nbsp;dataset.&nbsp;In&nbsp;DLStudio,&nbsp;we&nbsp;access&nbsp;these&nbsp;embeddings&nbsp;through&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;popular&nbsp;gensim&nbsp;library.<br>
 &nbsp;<br>
 &nbsp;<br>
-<span style="color:red; font-size:150%"><strong><a id="119">CO-CLASSES IN THE DLStudio PLATFORM</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;stated&nbsp;at&nbsp;the&nbsp;beginning&nbsp;of&nbsp;the&nbsp;previous&nbsp;section,&nbsp;a&nbsp;Co-Class&nbsp;resides&nbsp;at&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;same&nbsp;level&nbsp;of&nbsp;abstraction&nbsp;in&nbsp;the&nbsp;distribution&nbsp;directory&nbsp;as&nbsp;the&nbsp;main&nbsp;DLStudio<br>
-&nbsp;&nbsp;&nbsp;&nbsp;platform.&nbsp;Each&nbsp;Co-Class&nbsp;is&nbsp;defined&nbsp;in&nbsp;a&nbsp;separate&nbsp;subdirectory&nbsp;at&nbsp;the&nbsp;top&nbsp;level<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;distribution&nbsp;directory.&nbsp;&nbsp;While&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;is&nbsp;defined&nbsp;in&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;subdirectory&nbsp;of&nbsp;the&nbsp;same&nbsp;name,&nbsp;the&nbsp;other&nbsp;subdirectories&nbsp;that&nbsp;contain<br>
-&nbsp;&nbsp;&nbsp;&nbsp;definitions&nbsp;for&nbsp;the&nbsp;co-classes&nbsp;are&nbsp;named&nbsp;AdversarialLearning,&nbsp;Seq2SeqLearning,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;DataPrediction,&nbsp;Transformers,&nbsp;and&nbsp;MetricLearning.&nbsp;&nbsp;What&nbsp;follows&nbsp;in&nbsp;this<br>
-&nbsp;&nbsp;&nbsp;&nbsp;section&nbsp;are&nbsp;additional&nbsp;details&nbsp;regarding&nbsp;these&nbsp;co-classes:<br>
+<span style="color:red; font-size:150%"><strong><a id="119">MODULES IN THE DLStudio PLATFORM</a></strong></span><br>&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;stated&nbsp;at&nbsp;the&nbsp;beginning&nbsp;of&nbsp;the&nbsp;previous&nbsp;section,&nbsp;a&nbsp;module&nbsp;resides&nbsp;at&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;same&nbsp;level&nbsp;of&nbsp;software&nbsp;abstraction&nbsp;in&nbsp;the&nbsp;distribution&nbsp;directory&nbsp;as&nbsp;the&nbsp;main<br>
+&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;class&nbsp;in&nbsp;the&nbsp;platform.&nbsp;Each&nbsp;module&nbsp;is&nbsp;defined&nbsp;in&nbsp;a&nbsp;separate<br>
+&nbsp;&nbsp;&nbsp;&nbsp;subdirectory&nbsp;at&nbsp;the&nbsp;top&nbsp;level&nbsp;of&nbsp;the&nbsp;distribution&nbsp;directory.&nbsp;&nbsp;While&nbsp;the&nbsp;main<br>
+&nbsp;&nbsp;&nbsp;&nbsp;DLStudio&nbsp;class&nbsp;is&nbsp;defined&nbsp;in&nbsp;a&nbsp;subdirectory&nbsp;of&nbsp;the&nbsp;same&nbsp;name,&nbsp;the&nbsp;other<br>
+&nbsp;&nbsp;&nbsp;&nbsp;subdirectories&nbsp;that&nbsp;contain&nbsp;the&nbsp;definitions&nbsp;for&nbsp;the&nbsp;modules&nbsp;are&nbsp;named<br>
+&nbsp;&nbsp;&nbsp;&nbsp;AdversarialLearning,&nbsp;Seq2SeqLearning,&nbsp;DataPrediction,&nbsp;Transformers,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion,&nbsp;and&nbsp;MetricLearning.&nbsp;&nbsp;What&nbsp;follows&nbsp;in&nbsp;this&nbsp;section&nbsp;are<br>
+&nbsp;&nbsp;&nbsp;&nbsp;additional&nbsp;details&nbsp;regarding&nbsp;these&nbsp;co-classes:<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong>    </strong></span><br>&nbsp;&nbsp;&nbsp;&nbsp;AdversarialLearning:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;===================<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;I&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;Introduction,&nbsp;the&nbsp;purpose&nbsp;of&nbsp;the&nbsp;AdversarialLearning<br>
 &nbsp;&nbsp;&nbsp;&nbsp;class&nbsp;is&nbsp;to&nbsp;demonstrate&nbsp;probabilistic&nbsp;data&nbsp;modeling&nbsp;using&nbsp;Generative<br>
@@ -1627,15 +1633,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;former&nbsp;is&nbsp;called&nbsp;the&nbsp;q-chain&nbsp;and&nbsp;the&nbsp;latter&nbsp;the&nbsp;p-chain.&nbsp;&nbsp;The&nbsp;incremental<br>
 &nbsp;&nbsp;&nbsp;&nbsp;diffusion&nbsp;in&nbsp;the&nbsp;q-chain&nbsp;is&nbsp;with&nbsp;known&nbsp;amount&nbsp;of&nbsp;Gaussian&nbsp;isotropic&nbsp;noise.&nbsp;&nbsp;In<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;p-chain,&nbsp;on&nbsp;the&nbsp;other&nbsp;hand,&nbsp;the&nbsp;goal&nbsp;is&nbsp;for&nbsp;a&nbsp;neural&nbsp;network&nbsp;to&nbsp;learn&nbsp;from<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;diffusion&nbsp;carried&nbsp;out&nbsp;in&nbsp;the&nbsp;q-chain&nbsp;how&nbsp;to&nbsp;carry&nbsp;out&nbsp;a&nbsp;denoising<br>
 &nbsp;&nbsp;&nbsp;&nbsp;operation&nbsp;that&nbsp;would&nbsp;amount&nbsp;to&nbsp;a&nbsp;reversal&nbsp;of&nbsp;that&nbsp;diffusion.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;All&nbsp;of&nbsp;the&nbsp;key&nbsp;elements&nbsp;of&nbsp;the&nbsp;code&nbsp;that&nbsp;I&nbsp;have&nbsp;presented&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion&nbsp;co-class&nbsp;are&nbsp;extracted&nbsp;from&nbsp;OpenAI's&nbsp;"Improved&nbsp;Diffusion"<br>
+&nbsp;&nbsp;&nbsp;&nbsp;GenerativeDiffusion&nbsp;module&nbsp;are&nbsp;extracted&nbsp;from&nbsp;OpenAI's&nbsp;"Improved&nbsp;Diffusion"<br>
 &nbsp;&nbsp;&nbsp;&nbsp;project&nbsp;at&nbsp;GitHub&nbsp;that&nbsp;presents&nbsp;a&nbsp;PyTorch&nbsp;implementation&nbsp;of&nbsp;the&nbsp;work&nbsp;authored<br>
 &nbsp;&nbsp;&nbsp;&nbsp;by&nbsp;Nichol&nbsp;and&nbsp;Dhariwal&nbsp;in&nbsp;their&nbsp;very&nbsp;famous&nbsp;paper&nbsp;"Improved&nbsp;Denoising<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Diffusion&nbsp;Probabilistic&nbsp;Models".&nbsp;See&nbsp;the&nbsp;beginning&nbsp;part&nbsp;of&nbsp;the&nbsp;doc&nbsp;page&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;GenerativeDiffusion&nbsp;module&nbsp;for&nbsp;URLs&nbsp;to&nbsp;the&nbsp;GitHub&nbsp;code&nbsp;and&nbsp;their<br>
 &nbsp;&nbsp;&nbsp;&nbsp;publication.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;play&nbsp;with&nbsp;the&nbsp;code&nbsp;in&nbsp;GenerativeDiffusion,&nbsp;your&nbsp;starting&nbsp;point<br>
@@ -1665,15 +1671,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;your&nbsp;overall&nbsp;network&nbsp;learn&nbsp;on&nbsp;its&nbsp;own&nbsp;what&nbsp;are&nbsp;known&nbsp;as&nbsp;vector&nbsp;embeddings&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;words;&nbsp;or&nbsp;(2)&nbsp;Use&nbsp;pre-trained&nbsp;embeddings&nbsp;as&nbsp;provided&nbsp;by&nbsp;word2vec&nbsp;or<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Fasttext.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;you&nbsp;have&nbsp;resolved&nbsp;the&nbsp;issue&nbsp;of&nbsp;word&nbsp;representation,&nbsp;your&nbsp;next&nbsp;challenge<br>
 &nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;how&nbsp;to&nbsp;implement&nbsp;the&nbsp;attention&nbsp;mechanism&nbsp;that&nbsp;you're&nbsp;going&nbsp;to&nbsp;need&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;aligning&nbsp;the&nbsp;similar&nbsp;grammatical&nbsp;units&nbsp;in&nbsp;the&nbsp;two&nbsp;languages.&nbsp;The&nbsp;seq2seq&nbsp;code<br>
-&nbsp;&nbsp;&nbsp;&nbsp;demonstrated&nbsp;in&nbsp;this&nbsp;co-class&nbsp;uses&nbsp;the&nbsp;attention&nbsp;model&nbsp;proposed&nbsp;by&nbsp;Bahdanau,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;demonstrated&nbsp;in&nbsp;this&nbsp;module&nbsp;uses&nbsp;the&nbsp;attention&nbsp;model&nbsp;proposed&nbsp;by&nbsp;Bahdanau,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Cho,&nbsp;and&nbsp;Bengio&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;separate&nbsp;Attention&nbsp;class.&nbsp;&nbsp;The&nbsp;name&nbsp;of&nbsp;this<br>
 &nbsp;&nbsp;&nbsp;&nbsp;attention&nbsp;class&nbsp;is&nbsp;Attention_BCB.&nbsp;&nbsp;In&nbsp;a&nbsp;separate&nbsp;attention&nbsp;class&nbsp;named<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Attention_SR,&nbsp;I&nbsp;have&nbsp;also&nbsp;included&nbsp;the&nbsp;attention&nbsp;mechanism&nbsp;used&nbsp;by&nbsp;Sean<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Robertson&nbsp;in&nbsp;his&nbsp;very&nbsp;popular&nbsp;NLP&nbsp;tutorial&nbsp;at&nbsp;the&nbsp;main&nbsp;PyTorch&nbsp;website.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Seq2SeqLearning&nbsp;contains&nbsp;the&nbsp;following&nbsp;two&nbsp;inner&nbsp;classes&nbsp;for&nbsp;illustrating<br>
 &nbsp;&nbsp;&nbsp;&nbsp;seq2seq:<br>
@@ -1757,15 +1763,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;TransformerPreLN&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;original&nbsp;idea&nbsp;along&nbsp;with&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;modifications&nbsp;suggested&nbsp;by&nbsp;Xiong&nbsp;et&nbsp;al.&nbsp;in&nbsp;their&nbsp;paper&nbsp;"On&nbsp;Layer&nbsp;Normalization<br>
 &nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;Transformer&nbsp;Architecture"&nbsp;for&nbsp;more&nbsp;stable&nbsp;learning.&nbsp;&nbsp;The&nbsp;two&nbsp;versions<br>
 &nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;transformers&nbsp;differ&nbsp;in&nbsp;only&nbsp;one&nbsp;respect:&nbsp;The&nbsp;placement&nbsp;of&nbsp;the&nbsp;LayerNorm&nbsp;in<br>
 &nbsp;&nbsp;&nbsp;&nbsp;relation&nbsp;to&nbsp;the&nbsp;architectural&nbsp;components&nbsp;related&nbsp;to&nbsp;attention&nbsp;and&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;feedforward&nbsp;network.&nbsp;&nbsp;Literally,&nbsp;the&nbsp;difference&nbsp;is&nbsp;small,&nbsp;yet&nbsp;its&nbsp;consequences<br>
 &nbsp;&nbsp;&nbsp;&nbsp;are&nbsp;significant&nbsp;regarding&nbsp;the&nbsp;stability&nbsp;of&nbsp;learning.&nbsp;&nbsp;Finally,&nbsp;visTransformer<br>
-&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;Vision&nbsp;Transformer&nbsp;as&nbsp;presented&nbsp;in&nbsp;the&nbsp;famou&nbsp;paper<br>
+&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;Vision&nbsp;Transformer&nbsp;as&nbsp;presented&nbsp;in&nbsp;the&nbsp;famous&nbsp;paper<br>
 &nbsp;&nbsp;&nbsp;&nbsp;"An&nbsp;Image&nbsp;is&nbsp;Worth&nbsp;16x16$&nbsp;Words:&nbsp;Transformers&nbsp;for&nbsp;Image&nbsp;Recognition&nbsp;at&nbsp;Scale''<br>
 &nbsp;&nbsp;&nbsp;&nbsp;by&nbsp;Dosovitskiy&nbsp;et&nbsp;al.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;fundamentals&nbsp;of&nbsp;how&nbsp;the&nbsp;attention&nbsp;works&nbsp;in&nbsp;all&nbsp;three&nbsp;transformer&nbsp;based<br>
 &nbsp;&nbsp;&nbsp;&nbsp;implementations&nbsp;in&nbsp;the&nbsp;Transformers&nbsp;module&nbsp;are&nbsp;exactly&nbsp;the&nbsp;same.&nbsp;&nbsp;For<br>
 &nbsp;&nbsp;&nbsp;&nbsp;self-attention,&nbsp;you&nbsp;associate&nbsp;a&nbsp;Query&nbsp;Vector&nbsp;Q_i&nbsp;and&nbsp;a&nbsp;Key&nbsp;Vector&nbsp;K_i&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;each&nbsp;word&nbsp;w_i&nbsp;in&nbsp;a&nbsp;sentence.&nbsp;&nbsp;For&nbsp;a&nbsp;given&nbsp;w_i,&nbsp;the&nbsp;dot&nbsp;product&nbsp;of&nbsp;its&nbsp;Q_i&nbsp;with<br>
@@ -1878,15 +1884,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;triplets&nbsp;(i,j,k)&nbsp;in&nbsp;which&nbsp;two&nbsp;indices&nbsp;are&nbsp;the&nbsp;same.&nbsp;&nbsp;If&nbsp;B&nbsp;is&nbsp;the&nbsp;batch&nbsp;size,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;is&nbsp;easily&nbsp;done&nbsp;by&nbsp;first&nbsp;forming&nbsp;a&nbsp;BxB&nbsp;array&nbsp;that&nbsp;is&nbsp;the&nbsp;logical&nbsp;negation<br>
 &nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;a&nbsp;Boolean&nbsp;array&nbsp;of&nbsp;the&nbsp;same&nbsp;size&nbsp;whose&nbsp;True&nbsp;values&nbsp;are&nbsp;only&nbsp;on&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;diagonal.&nbsp;&nbsp;We&nbsp;can&nbsp;reshape&nbsp;this&nbsp;BxB&nbsp;Boolean&nbsp;array&nbsp;into&nbsp;three&nbsp;BxBxB&nbsp;shaped<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Boolean&nbsp;arrays,&nbsp;the&nbsp;first&nbsp;in&nbsp;which&nbsp;the&nbsp;True&nbsp;values&nbsp;exist&nbsp;only&nbsp;where&nbsp;i&nbsp;and&nbsp;j<br>
 &nbsp;&nbsp;&nbsp;&nbsp;values&nbsp;are&nbsp;not&nbsp;the&nbsp;same,&nbsp;the&nbsp;second&nbsp;in&nbsp;which&nbsp;the&nbsp;True&nbsp;values&nbsp;occur&nbsp;only&nbsp;when&nbsp;i<br>
 &nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;k&nbsp;index&nbsp;values&nbsp;are&nbsp;not&nbsp;the&nbsp;same,&nbsp;and&nbsp;the&nbsp;third&nbsp;that&nbsp;has&nbsp;True&nbsp;values&nbsp;only<br>
-&nbsp;&nbsp;&nbsp;&nbsp;when&nbsp;the&nbsp;j&nbsp;and&nbsp;k&nbsp;index&nbsp;values&nbsp;are&nbsp;not&nbsp;the&nbsp;same.&nbsp;&nbsp;By&nbsp;taking&nbsp;a&nbsp;logial&nbsp;AND&nbsp;of&nbsp;all<br>
+&nbsp;&nbsp;&nbsp;&nbsp;when&nbsp;the&nbsp;j&nbsp;and&nbsp;k&nbsp;index&nbsp;values&nbsp;are&nbsp;not&nbsp;the&nbsp;same.&nbsp;&nbsp;By&nbsp;taking&nbsp;a&nbsp;logical&nbsp;AND&nbsp;of&nbsp;all<br>
 &nbsp;&nbsp;&nbsp;&nbsp;three&nbsp;BxBxB&nbsp;Boolean&nbsp;arrays,&nbsp;we&nbsp;get&nbsp;the&nbsp;result&nbsp;we&nbsp;want.&nbsp;&nbsp;Next,&nbsp;we&nbsp;construct&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BxBxB&nbsp;Boolean&nbsp;tensor&nbsp;in&nbsp;which&nbsp;the&nbsp;True&nbsp;values&nbsp;occur&nbsp;only&nbsp;where&nbsp;the&nbsp;first&nbsp;two<br>
 &nbsp;&nbsp;&nbsp;&nbsp;index&nbsp;values&nbsp;imply&nbsp;that&nbsp;their&nbsp;corresponding&nbsp;labels&nbsp;are&nbsp;identical&nbsp;and&nbsp;where&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;last&nbsp;index&nbsp;corresponds&nbsp;to&nbsp;a&nbsp;label&nbsp;that&nbsp;does&nbsp;not&nbsp;agree&nbsp;with&nbsp;that&nbsp;for&nbsp;the&nbsp;first<br>
 &nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;index&nbsp;values.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Even&nbsp;after&nbsp;you&nbsp;have&nbsp;formed&nbsp;the&nbsp;triplets,&nbsp;your&nbsp;next&nbsp;mini-challenge&nbsp;is&nbsp;to<br>
@@ -1914,15 +1920,15 @@
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="120">Examples DIRECTORY</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;Examples&nbsp;subdirectory&nbsp;in&nbsp;the&nbsp;distribution&nbsp;contains&nbsp;the&nbsp;following&nbsp;scripts:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp;&nbsp;playing_with_reconfig.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Shows&nbsp;how&nbsp;you&nbsp;can&nbsp;specify&nbsp;a&nbsp;convolution&nbsp;network&nbsp;with&nbsp;a&nbsp;configuration<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;string.&nbsp;&nbsp;The&nbsp;DLStudio&nbsp;module&nbsp;parses&nbsp;the&nbsp;string&nbsp;constructs&nbsp;the&nbsp;network.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;string.&nbsp;&nbsp;The&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;parses&nbsp;the&nbsp;string&nbsp;constructs&nbsp;the&nbsp;network.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(2)&nbsp;&nbsp;playing_with_sequential.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Shows&nbsp;you&nbsp;how&nbsp;you&nbsp;can&nbsp;call&nbsp;on&nbsp;a&nbsp;custom&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;'DLStudio'<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;module&nbsp;that&nbsp;is&nbsp;meant&nbsp;to&nbsp;experiment&nbsp;with&nbsp;your&nbsp;own&nbsp;network.&nbsp;&nbsp;The&nbsp;name&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;inner&nbsp;class&nbsp;in&nbsp;this&nbsp;example&nbsp;script&nbsp;is&nbsp;ExperimentsWithSequential<br>
 &nbsp;<br>
@@ -1941,22 +1947,22 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;directly&nbsp;illustrate&nbsp;in&nbsp;a&nbsp;classroom&nbsp;setting&nbsp;the&nbsp;improvement&nbsp;you&nbsp;can&nbsp;get<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;skip&nbsp;connections.&nbsp;&nbsp;And&nbsp;by&nbsp;giving&nbsp;an&nbsp;appropriate&nbsp;value&nbsp;to&nbsp;the&nbsp;"depth"<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;option,&nbsp;you&nbsp;can&nbsp;show&nbsp;results&nbsp;for&nbsp;networks&nbsp;of&nbsp;different&nbsp;depths.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(6)&nbsp;&nbsp;custom_data_loading.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;script&nbsp;shows&nbsp;how&nbsp;to&nbsp;use&nbsp;the&nbsp;custom&nbsp;dataloader&nbsp;in&nbsp;the&nbsp;inner&nbsp;class<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CustomDataLoading&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;module.&nbsp;&nbsp;That&nbsp;custom&nbsp;dataloader&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CustomDataLoading&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class.&nbsp;&nbsp;That&nbsp;custom&nbsp;dataloader&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;meant&nbsp;specifically&nbsp;for&nbsp;the&nbsp;PurdueShapes5&nbsp;dataset&nbsp;that&nbsp;is&nbsp;used&nbsp;in&nbsp;object<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;and&nbsp;localization&nbsp;experiments&nbsp;in&nbsp;DLStudio.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(7)&nbsp;&nbsp;object_detection_and_localization.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;script&nbsp;shows&nbsp;how&nbsp;you&nbsp;can&nbsp;use&nbsp;the&nbsp;functionality&nbsp;provided&nbsp;by&nbsp;the&nbsp;inner<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;class&nbsp;DetectAndLocalize&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;module&nbsp;for&nbsp;experimenting&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;class&nbsp;DetectAndLocalize&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;for&nbsp;experimenting&nbsp;with<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection&nbsp;and&nbsp;localization.&nbsp;&nbsp;Detecting&nbsp;and&nbsp;localizing&nbsp;(D&amp;L)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objects&nbsp;in&nbsp;images&nbsp;is&nbsp;a&nbsp;more&nbsp;difficult&nbsp;problem&nbsp;than&nbsp;just&nbsp;classifying&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objects.&nbsp;&nbsp;D&amp;L&nbsp;requires&nbsp;that&nbsp;your&nbsp;CNN&nbsp;make&nbsp;two&nbsp;different&nbsp;types&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;inferences&nbsp;simultaneously,&nbsp;one&nbsp;for&nbsp;classification&nbsp;and&nbsp;the&nbsp;other&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;localization.&nbsp;&nbsp;For&nbsp;the&nbsp;localization&nbsp;part,&nbsp;the&nbsp;CNN&nbsp;must&nbsp;carry&nbsp;out&nbsp;what&nbsp;is<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;known&nbsp;as&nbsp;regression.&nbsp;What&nbsp;that&nbsp;means&nbsp;is&nbsp;that&nbsp;the&nbsp;CNN&nbsp;must&nbsp;output&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;numerical&nbsp;values&nbsp;for&nbsp;the&nbsp;bounding&nbsp;box&nbsp;that&nbsp;encloses&nbsp;the&nbsp;object&nbsp;that&nbsp;was<br>
@@ -2113,23 +2119,23 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;words&nbsp;in&nbsp;the&nbsp;source-language&nbsp;sentences&nbsp;(English).&nbsp;&nbsp;As&nbsp;to&nbsp;why&nbsp;I&nbsp;have<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;not&nbsp;used&nbsp;at&nbsp;this&nbsp;time&nbsp;the&nbsp;pre-trained&nbsp;embeddings&nbsp;for&nbsp;the&nbsp;target&nbsp;language<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;explained&nbsp;in&nbsp;the&nbsp;main&nbsp;comment&nbsp;doc&nbsp;associated&nbsp;with&nbsp;the&nbsp;class<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Seq2SeqWithPretrainedEmbeddings.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="124">ExamplesDataPrediction DIRECTORY</a></strong></span><br>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExampsleDataPrediction&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution&nbsp;contains&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesDataPrediction&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution&nbsp;contains&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;following&nbsp;script&nbsp;for&nbsp;demonstrating&nbsp;data&nbsp;prediction&nbsp;for&nbsp;time-series&nbsp;data:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;power_load_prediction_with_pmGRU.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;script&nbsp;uses&nbsp;a&nbsp;subset&nbsp;of&nbsp;the&nbsp;dataset&nbsp;provided&nbsp;by&nbsp;Kaggle&nbsp;for&nbsp;one&nbsp;of&nbsp;their<br>
 &nbsp;&nbsp;&nbsp;&nbsp;machine&nbsp;learning&nbsp;competitions.&nbsp;&nbsp;The&nbsp;dataset&nbsp;consists&nbsp;of&nbsp;over&nbsp;10-years&nbsp;worth&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;hourly&nbsp;electric&nbsp;load&nbsp;recordings&nbsp;made&nbsp;available&nbsp;by&nbsp;several&nbsp;utilities&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;east&nbsp;and&nbsp;the&nbsp;midwest&nbsp;of&nbsp;the&nbsp;United&nbsp;States.&nbsp;&nbsp;You&nbsp;can&nbsp;download&nbsp;this&nbsp;dataset&nbsp;from<br>
+&nbsp;&nbsp;&nbsp;&nbsp;east&nbsp;and&nbsp;the&nbsp;Midwest&nbsp;of&nbsp;the&nbsp;United&nbsp;States.&nbsp;&nbsp;You&nbsp;can&nbsp;download&nbsp;this&nbsp;dataset&nbsp;from<br>
 &nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;link&nbsp;at&nbsp;the&nbsp;top&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;doc&nbsp;page.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="125">ExamplesTransformers DIRECTORY</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesTransformers&nbsp;directory&nbsp;of&nbsp;the&nbsp;distribution&nbsp;contains&nbsp;the&nbsp;following<br>
 &nbsp;&nbsp;&nbsp;&nbsp;four&nbsp;scripts&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;transformers&nbsp;in&nbsp;DLStudio:<br>
 &nbsp;<br>
@@ -2137,16 +2143,16 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;seq2seq_with_transformerPreLN.py&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_recog_with_visTransformer.py<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;test_checkpoint_for_visTransformer.py&nbsp;<br>
 &nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;first&nbsp;two&nbsp;scripts&nbsp;deal&nbsp;with&nbsp;English-to-Spanish&nbsp;translation&nbsp;in&nbsp;a&nbsp;manner<br>
-&nbsp;&nbsp;&nbsp;&nbsp;similar&nbsp;to&nbsp;what's&nbsp;demonstrated&nbsp;by&nbsp;the&nbsp;code&nbsp;in&nbsp;the&nbsp;Seq2SeqLearning&nbsp;co-class&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;example&nbsp;scripts&nbsp;associated&nbsp;with&nbsp;that&nbsp;co-class.&nbsp;The&nbsp;last&nbsp;two&nbsp;relate&nbsp;to&nbsp;my<br>
+&nbsp;&nbsp;&nbsp;&nbsp;similar&nbsp;to&nbsp;what's&nbsp;demonstrated&nbsp;by&nbsp;the&nbsp;code&nbsp;in&nbsp;the&nbsp;Seq2SeqLearning&nbsp;module&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;example&nbsp;scripts&nbsp;associated&nbsp;with&nbsp;that&nbsp;module.&nbsp;The&nbsp;last&nbsp;two&nbsp;relate&nbsp;to&nbsp;my<br>
 &nbsp;&nbsp;&nbsp;&nbsp;demonstration&nbsp;of&nbsp;image&nbsp;recognition&nbsp;with&nbsp;a&nbsp;transformer&nbsp;based&nbsp;implementation.&nbsp;&nbsp;I<br>
 &nbsp;&nbsp;&nbsp;&nbsp;have&nbsp;used&nbsp;the&nbsp;CFAR10&nbsp;dataset&nbsp;for&nbsp;image&nbsp;recognition.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="126">ExamplesMetricLearning DIRECTORY</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesMetricLearning&nbsp;directory&nbsp;at&nbsp;top&nbsp;level&nbsp;of&nbsp;the&nbsp;distribution&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;contains&nbsp;the&nbsp;following&nbsp;scripts:<br>
@@ -2161,15 +2167,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;ResNet-50&nbsp;trunk&nbsp;model&nbsp;or&nbsp;the&nbsp;homebrewed&nbsp;network&nbsp;supplied&nbsp;with&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;MetricLearning&nbsp;module.<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="127">THE DATASETS INCLUDED</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;[must&nbsp;be&nbsp;downloaded&nbsp;separately]<br>
 &nbsp;<br>
-<span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="128">    FOR THE MAIN DLStudio MODULE</a></strong></span><br>&nbsp;<br>
+<span style="color:blue; font-size:100%"><strong>&nbsp;&nbsp;<a id="128">    FOR THE MAIN DLStudio CLASS and its INNER CLASSES</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Download&nbsp;the&nbsp;dataset&nbsp;archive&nbsp;'datasets_for_DLStudio.tar.gz'&nbsp;through&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;link&nbsp;"Download&nbsp;the&nbsp;image&nbsp;datasets&nbsp;for&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;Class"&nbsp;provided&nbsp;at<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;top&nbsp;of&nbsp;this&nbsp;documentation&nbsp;page&nbsp;and&nbsp;store&nbsp;it&nbsp;in&nbsp;the&nbsp;'Example'&nbsp;directory<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;distribution.&nbsp;&nbsp;Subsequently,&nbsp;execute&nbsp;the&nbsp;following&nbsp;command&nbsp;in&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'Examples'&nbsp;directory:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cd&nbsp;Examples<br>
@@ -2378,15 +2384,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;That&nbsp;will&nbsp;create&nbsp;a&nbsp;'data'&nbsp;subdirectory&nbsp;in&nbsp;the&nbsp;ExamplesTransformers<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;directory&nbsp;and&nbsp;deposit&nbsp;in&nbsp;that&nbsp;subdirectory&nbsp;the&nbsp;following&nbsp;archives<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;en_es_xformer_8_10000.tar.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;en_es_xformer_8_90000.tar.gz<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;These&nbsp;are&nbsp;both&nbsp;derived&nbsp;from&nbsp;the&nbsp;same&nbsp;data&nbsp;source&nbsp;as&nbsp;in&nbsp;the&nbsp;dataset&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;examples&nbsp;associated&nbsp;with&nbsp;the&nbsp;Seq2SeqLearning&nbsp;co-class.&nbsp;&nbsp;The&nbsp;first&nbsp;has&nbsp;only<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;examples&nbsp;associated&nbsp;with&nbsp;the&nbsp;Seq2SeqLearning&nbsp;module.&nbsp;&nbsp;The&nbsp;first&nbsp;has&nbsp;only<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;10,000&nbsp;pars&nbsp;of&nbsp;English-Spanish&nbsp;sentences&nbsp;and&nbsp;meant&nbsp;primarily&nbsp;for&nbsp;debugging<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;purposes.&nbsp;&nbsp;The&nbsp;second&nbsp;contains&nbsp;90000&nbsp;pairs&nbsp;of&nbsp;such&nbsp;sentences.&nbsp;&nbsp;The&nbsp;number<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'8'&nbsp;in&nbsp;the&nbsp;dataset&nbsp;names&nbsp;means&nbsp;that&nbsp;no&nbsp;sentence&nbsp;contains&nbsp;more&nbsp;than&nbsp;8&nbsp;real<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;words.&nbsp;&nbsp;With&nbsp;the&nbsp;"SOS"&nbsp;and&nbsp;"EOS"&nbsp;tokens&nbsp;used&nbsp;as&nbsp;sentence&nbsp;delimiters,&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;maximum&nbsp;number&nbsp;of&nbsp;words&nbsp;in&nbsp;each&nbsp;sentence&nbsp;in&nbsp;either&nbsp;language&nbsp;is&nbsp;10.<br>
 &nbsp;<br>
 &nbsp;<br>
@@ -2417,15 +2423,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;Version&nbsp;2.2.2:&nbsp;My&nbsp;laboratory's&nbsp;(RVL)&nbsp;journey&nbsp;into&nbsp;the&nbsp;world&nbsp;of&nbsp;transformers<br>
 &nbsp;&nbsp;&nbsp;&nbsp;began&nbsp;with&nbsp;a&nbsp;series&nbsp;of&nbsp;lab&nbsp;seminars&nbsp;by&nbsp;Constantine&nbsp;Roros&nbsp;and&nbsp;Rahul&nbsp;Deshmukh.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Several&nbsp;subsequent&nbsp;conversations&nbsp;with&nbsp;them&nbsp;were&nbsp;instrumental&nbsp;in&nbsp;helping&nbsp;me<br>
 &nbsp;&nbsp;&nbsp;&nbsp;improve&nbsp;the&nbsp;understanding&nbsp;I&nbsp;had&nbsp;gained&nbsp;from&nbsp;the&nbsp;seminars.&nbsp;&nbsp;Additional<br>
 &nbsp;&nbsp;&nbsp;&nbsp;conversations&nbsp;with&nbsp;Rahul&nbsp;about&nbsp;the&nbsp;issue&nbsp;of&nbsp;masking&nbsp;were&nbsp;important&nbsp;to&nbsp;how&nbsp;I<br>
 &nbsp;&nbsp;&nbsp;&nbsp;eventually&nbsp;implemented&nbsp;those&nbsp;ideas&nbsp;in&nbsp;my&nbsp;code.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Rahul&nbsp;Deshmukh&nbsp;discovered&nbsp;the&nbsp;reason&nbsp;as&nbsp;to&nbsp;why&nbsp;my&nbsp;implmentation&nbsp;of&nbsp;the&nbsp;skip<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Rahul&nbsp;Deshmukh&nbsp;discovered&nbsp;the&nbsp;reason&nbsp;as&nbsp;to&nbsp;why&nbsp;my&nbsp;implementation&nbsp;of&nbsp;the&nbsp;skip<br>
 &nbsp;&nbsp;&nbsp;&nbsp;connection&nbsp;code&nbsp;was&nbsp;not&nbsp;working&nbsp;with&nbsp;the&nbsp;more&nbsp;recent&nbsp;versions&nbsp;of&nbsp;PyTorch.&nbsp;&nbsp;My<br>
 &nbsp;&nbsp;&nbsp;&nbsp;problem&nbsp;was&nbsp;using&nbsp;in-place&nbsp;operations&nbsp;in&nbsp;the&nbsp;forward()&nbsp;of&nbsp;the&nbsp;networks&nbsp;that<br>
 &nbsp;&nbsp;&nbsp;&nbsp;called&nbsp;for&nbsp;connection&nbsp;skipping.&nbsp;This&nbsp;led&nbsp;to&nbsp;the&nbsp;release&nbsp;of&nbsp;Version&nbsp;2.3.3&nbsp;of<br>
 &nbsp;&nbsp;&nbsp;&nbsp;DLStudio.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;main&nbsp;reason&nbsp;for&nbsp;Version&nbsp;2.3.4&nbsp;was&nbsp;my&nbsp;new&nbsp;design&nbsp;for&nbsp;the&nbsp;SkipBlock&nbsp;class<br>
 &nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;also&nbsp;my&nbsp;easier-to-understand&nbsp;code&nbsp;for&nbsp;the&nbsp;BMEnet&nbsp;class&nbsp;that&nbsp;showcases&nbsp;the<br>
@@ -2434,15 +2440,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;Cheng-Hao&nbsp;Chen&nbsp;reported&nbsp;that&nbsp;when&nbsp;a&nbsp;SkipBlock&nbsp;was&nbsp;asked&nbsp;to&nbsp;change&nbsp;the&nbsp;channels<br>
 &nbsp;&nbsp;&nbsp;&nbsp;from&nbsp;its&nbsp;input&nbsp;to&nbsp;its&nbsp;output&nbsp;but&nbsp;without&nbsp;downsampling&nbsp;the&nbsp;input,&nbsp;that&nbsp;elicited<br>
 &nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;error&nbsp;from&nbsp;the&nbsp;system.&nbsp;&nbsp;Cheng-Hao&nbsp;also&nbsp;provided&nbsp;a&nbsp;correction&nbsp;for&nbsp;the&nbsp;error.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Thanks,&nbsp;Cheng-Hao!<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Aditya&nbsp;Chauhan&nbsp;proved&nbsp;to&nbsp;be&nbsp;a&nbsp;great&nbsp;sounding&nbsp;board&nbsp;in&nbsp;my&nbsp;journey&nbsp;into&nbsp;the&nbsp;land<br>
 &nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;diffusion&nbsp;that&nbsp;led&nbsp;to&nbsp;Version&nbsp;2.4.2.&nbsp;&nbsp;I&nbsp;particularly&nbsp;appreciated&nbsp;Aditya's<br>
-&nbsp;&nbsp;&nbsp;&nbsp;help&nbsp;in&nbsp;understanding&nbsp;how&nbsp;the&nbsp;attention&nbsp;mechanism&nbsp;worked&nbsp;in&nbsp;the&nbsp;OpanAI&nbsp;code<br>
+&nbsp;&nbsp;&nbsp;&nbsp;help&nbsp;in&nbsp;understanding&nbsp;how&nbsp;the&nbsp;attention&nbsp;mechanism&nbsp;worked&nbsp;in&nbsp;the&nbsp;OpenAI&nbsp;code<br>
 &nbsp;&nbsp;&nbsp;&nbsp;library&nbsp;at&nbsp;GitHub.&nbsp;&nbsp;Aditya&nbsp;is&nbsp;working&nbsp;for&nbsp;his&nbsp;PhD&nbsp;in&nbsp;RVL.&nbsp;&nbsp;Thanks,&nbsp;Aditya!<br>
 &nbsp;<br>
 &nbsp;<br>
 <span style="color:red; font-size:150%"><strong><a id="135">ABOUT THE AUTHOR</a></strong></span><br>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;author,&nbsp;Avinash&nbsp;Kak,&nbsp;is&nbsp;a&nbsp;professor&nbsp;of&nbsp;Electrical&nbsp;and&nbsp;Computer&nbsp;Engineering<br>
 &nbsp;&nbsp;&nbsp;&nbsp;at&nbsp;Purdue&nbsp;University.&nbsp;&nbsp;For&nbsp;all&nbsp;issues&nbsp;related&nbsp;to&nbsp;this&nbsp;module,&nbsp;contact&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;author&nbsp;at&nbsp;kak@purdue.edu.&nbsp;If&nbsp;you&nbsp;send&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string<br>
@@ -2612,16 +2618,16 @@
 designing&nbsp;a&nbsp;custom&nbsp;data&nbsp;loader.&nbsp;&nbsp;Ordinarily,&nbsp;if&nbsp;the&nbsp;basic&nbsp;format&nbsp;of&nbsp;how&nbsp;the&nbsp;dataset<br>
 is&nbsp;stored&nbsp;is&nbsp;similar&nbsp;to&nbsp;one&nbsp;of&nbsp;the&nbsp;datasets&nbsp;that&nbsp;the&nbsp;Torchvision&nbsp;module&nbsp;knows&nbsp;about,<br>
 you&nbsp;can&nbsp;go&nbsp;ahead&nbsp;and&nbsp;use&nbsp;that&nbsp;for&nbsp;your&nbsp;own&nbsp;dataset.&nbsp;&nbsp;At&nbsp;worst,&nbsp;you&nbsp;may&nbsp;need&nbsp;to&nbsp;carry<br>
 out&nbsp;some&nbsp;light&nbsp;customizations&nbsp;depending&nbsp;on&nbsp;the&nbsp;number&nbsp;of&nbsp;classes&nbsp;involved,&nbsp;etc.<br>
 &nbsp;<br>
 However,&nbsp;if&nbsp;the&nbsp;underlying&nbsp;dataset&nbsp;is&nbsp;stored&nbsp;in&nbsp;a&nbsp;manner&nbsp;that&nbsp;does&nbsp;not&nbsp;look&nbsp;like<br>
 anything&nbsp;in&nbsp;Torchvision,&nbsp;you&nbsp;have&nbsp;no&nbsp;choice&nbsp;but&nbsp;to&nbsp;supply&nbsp;yourself&nbsp;all&nbsp;of&nbsp;the&nbsp;data<br>
-loading&nbsp;infrastructure.&nbsp;&nbsp;That&nbsp;is&nbsp;what&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;DLStudio&nbsp;module&nbsp;is&nbsp;all<br>
-about.<br>
+loading&nbsp;infrastructure.&nbsp;&nbsp;That&nbsp;is&nbsp;what&nbsp;this&nbsp;inner&nbsp;class&nbsp;of&nbsp;the&nbsp;main&nbsp;DLStudio&nbsp;class&nbsp;<br>
+is&nbsp;all&nbsp;about.<br>
 &nbsp;<br>
 The&nbsp;custom&nbsp;data&nbsp;loading&nbsp;exercise&nbsp;here&nbsp;is&nbsp;related&nbsp;to&nbsp;a&nbsp;dataset&nbsp;called&nbsp;PurdueShapes5<br>
 that&nbsp;contains&nbsp;32x32&nbsp;images&nbsp;of&nbsp;binary&nbsp;shapes&nbsp;belonging&nbsp;to&nbsp;the&nbsp;following&nbsp;five&nbsp;classes:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.&nbsp;&nbsp;rectangle<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.&nbsp;&nbsp;triangle<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.&nbsp;&nbsp;disk<br>
@@ -2691,15 +2697,15 @@
 
 <dl><dt><strong>ExperimentsWithSequential</strong> = &lt;class 'DLStudio.DLStudio.ExperimentsWithSequential'&gt;<dd><tt>Demonstrates&nbsp;how&nbsp;to&nbsp;use&nbsp;the&nbsp;torch.nn.Sequential&nbsp;container&nbsp;class<br>
 &nbsp;<br>
 Class&nbsp;Path:&nbsp;&nbsp;DLStudio&nbsp;&nbsp;-&gt;&nbsp;&nbsp;ExperimentsWithSequential</tt></dl>
 
 <dl><dt><strong>Net</strong> = &lt;class 'DLStudio.DLStudio.Net'&gt;</dl>
 
-<dl><dt><strong>SemanticSegmentation</strong> = &lt;class 'DLStudio.DLStudio.SemanticSegmentation'&gt;<dd><tt>The&nbsp;purpose&nbsp;of&nbsp;this&nbsp;inner&nbsp;class&nbsp;is&nbsp;to&nbsp;be&nbsp;able&nbsp;to&nbsp;use&nbsp;the&nbsp;DLStudio&nbsp;module&nbsp;for<br>
+<dl><dt><strong>SemanticSegmentation</strong> = &lt;class 'DLStudio.DLStudio.SemanticSegmentation'&gt;<dd><tt>The&nbsp;purpose&nbsp;of&nbsp;this&nbsp;inner&nbsp;class&nbsp;is&nbsp;to&nbsp;be&nbsp;able&nbsp;to&nbsp;use&nbsp;the&nbsp;DLStudio&nbsp;platform&nbsp;for<br>
 experiments&nbsp;with&nbsp;semantic&nbsp;segmentation.&nbsp;&nbsp;At&nbsp;its&nbsp;simplest&nbsp;level,&nbsp;the&nbsp;purpose&nbsp;of<br>
 semantic&nbsp;segmentation&nbsp;is&nbsp;to&nbsp;assign&nbsp;correct&nbsp;labels&nbsp;to&nbsp;the&nbsp;different&nbsp;objects&nbsp;in&nbsp;a<br>
 scene,&nbsp;while&nbsp;localizing&nbsp;them&nbsp;at&nbsp;the&nbsp;same&nbsp;time.&nbsp;&nbsp;At&nbsp;a&nbsp;more&nbsp;sophisticated&nbsp;level,&nbsp;a<br>
 system&nbsp;that&nbsp;carries&nbsp;out&nbsp;semantic&nbsp;segmentation&nbsp;should&nbsp;also&nbsp;output&nbsp;a&nbsp;symbolic<br>
 expression&nbsp;based&nbsp;on&nbsp;the&nbsp;objects&nbsp;found&nbsp;in&nbsp;the&nbsp;image&nbsp;and&nbsp;their&nbsp;spatial&nbsp;relationships<br>
 with&nbsp;one&nbsp;another.<br>
 &nbsp;<br>
@@ -2719,15 +2725,15 @@
 for&nbsp;experimenting&nbsp;with&nbsp;mUnet.&nbsp;&nbsp;Each&nbsp;image&nbsp;in&nbsp;this&nbsp;dataset&nbsp;contains&nbsp;a&nbsp;random&nbsp;number<br>
 of&nbsp;selections&nbsp;from&nbsp;five&nbsp;different&nbsp;shapes,&nbsp;with&nbsp;the&nbsp;shapes&nbsp;being&nbsp;randomly&nbsp;scaled,<br>
 oriented,&nbsp;and&nbsp;located&nbsp;in&nbsp;each&nbsp;image.&nbsp;&nbsp;The&nbsp;five&nbsp;different&nbsp;shapes&nbsp;are:&nbsp;rectangle,<br>
 triangle,&nbsp;disk,&nbsp;oval,&nbsp;and&nbsp;star.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;Class&nbsp;Path:&nbsp;&nbsp;&nbsp;DLStudio&nbsp;&nbsp;-&gt;&nbsp;&nbsp;SemanticSegmentation</tt></dl>
 
-<dl><dt><strong>TextClassification</strong> = &lt;class 'DLStudio.DLStudio.TextClassification'&gt;<dd><tt>The&nbsp;purpose&nbsp;of&nbsp;this&nbsp;inner&nbsp;class&nbsp;is&nbsp;to&nbsp;be&nbsp;able&nbsp;to&nbsp;use&nbsp;the&nbsp;DLStudio&nbsp;module&nbsp;for&nbsp;simple&nbsp;<br>
+<dl><dt><strong>TextClassification</strong> = &lt;class 'DLStudio.DLStudio.TextClassification'&gt;<dd><tt>The&nbsp;purpose&nbsp;of&nbsp;this&nbsp;inner&nbsp;class&nbsp;is&nbsp;to&nbsp;be&nbsp;able&nbsp;to&nbsp;use&nbsp;the&nbsp;DLStudio&nbsp;platform&nbsp;for&nbsp;simple&nbsp;<br>
 experiments&nbsp;in&nbsp;text&nbsp;classification.&nbsp;&nbsp;Consider,&nbsp;for&nbsp;example,&nbsp;the&nbsp;problem&nbsp;of&nbsp;automatic&nbsp;<br>
 classification&nbsp;of&nbsp;variable-length&nbsp;user&nbsp;feedback:&nbsp;you&nbsp;want&nbsp;to&nbsp;create&nbsp;a&nbsp;neural&nbsp;network<br>
 that&nbsp;can&nbsp;label&nbsp;an&nbsp;uploaded&nbsp;product&nbsp;review&nbsp;of&nbsp;arbitrary&nbsp;length&nbsp;as&nbsp;positive&nbsp;or&nbsp;negative.&nbsp;&nbsp;<br>
 One&nbsp;way&nbsp;to&nbsp;solve&nbsp;this&nbsp;problem&nbsp;is&nbsp;with&nbsp;a&nbsp;recurrent&nbsp;neural&nbsp;network&nbsp;in&nbsp;which&nbsp;you&nbsp;use&nbsp;a&nbsp;<br>
 hidden&nbsp;state&nbsp;for&nbsp;characterizing&nbsp;a&nbsp;variable-length&nbsp;product&nbsp;review&nbsp;with&nbsp;a&nbsp;fixed-length&nbsp;<br>
 state&nbsp;vector.&nbsp;&nbsp;This&nbsp;inner&nbsp;class&nbsp;allows&nbsp;you&nbsp;to&nbsp;carry&nbsp;out&nbsp;such&nbsp;experiments.<br>
 &nbsp;<br>
@@ -2757,18 +2763,17 @@
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
     
 <tr><td style="bgcolor:#55aa55;"></td><td>&nbsp;</td>
 <td style="width:100%;"><strong>__author__</strong> = 'Avinash Kak (kak@purdue.edu)'<br>
 <strong>__copyright__</strong> = '(C) 2024 Avinash Kak. Python Software Foundation.'<br>
-<strong>__date__</strong> = '2024-April-27'<br>
-<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.8.html'<br>
-<strong>__version__</strong> = '2.4.8'</td></tr></table>
+<strong>__date__</strong> = '2024-May-1'<br>
+<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.9.html'<br>
+<strong>__version__</strong> = '2.4.9'</td></tr></table>
 <table style="width:100%; border-collapse:collapse; border-spacking:0; padding:2; border:0;">
 <tr style="bgcolor:#7799ee;">
 <td style="colspan:3; vertical-align:bottom;">&nbsp;<br>
 <span style="color:#ffffff; font-family:helvetica, arial; font-size:large;"><strong>Author</strong></big></span></td></tr>
 <tr><td style="bgcolor:#7799ee;"></td><td>&nbsp;</td>
 <td style="width:100%;">Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)</td></tr></table>
 </body></html>
-
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 ===============================================================================
 DDLLSSttuuddiioo
-Version 2.4.8,   2024-April-27
+Version 2.4.9,   2024-May-1
 "-1">A software platform for teaching the Deep Learning class at Purdue
 University
 
 ===============================================================================
 
 DLStudio.py
-Version:  2.4.8
+Version:  2.4.9
 Author:  Avinash Kak (kak@purdue.edu)
-Date:  2024-April-27
+Date:  2024-May-1
 
                                                  Total number of downloads (all
                                         versions) from this website:
                                         file = fopen("HowManyCounts.txt", "r")
                                         or exit("Unable to open file!"); echo
-DDoowwnnllooaadd VVeerrssiioonn 22..44..88::? ? ? ?  _gg_zz_tt_aa_rr       fgets($file); fclose($file); ?>
+DDoowwnnllooaadd VVeerrssiioonn 22..44..99::? ? ? ?  _gg_zz_tt_aa_rr       fgets($file); fclose($file); ?>
                                                     This count is automatically
                                         updated at every rotation of
                                                   the weblogs (normally once
                                         every two to four days)
                                                   Last updated:
                                         file = fopen("LastUpdated.txt", "r") or
                                         exit("Unable to open file!"); echo
@@ -71,36 +71,42 @@
 _ _ _ _ _T_R_A_N_S_F_O_R_M_E_R_S
 _ _ _ _ _M_E_T_R_I_C_ _L_E_A_R_N_I_N_G
 _I_N_S_T_A_L_L_A_T_I_O_N
 _U_S_A_G_E
 _C_O_N_S_T_R_U_C_T_O_R_ _P_A_R_A_M_E_T_E_R_S
 _P_U_B_L_I_C_ _M_E_T_H_O_D_S
 _T_H_E_ _M_A_I_N_ _I_N_N_E_R_ _C_L_A_S_S_E_S_ _O_F_ _T_H_E_ _D_L_S_t_u_d_i_o_ _C_L_A_S_S
-_C_O_-_C_L_A_S_S_E_S_ _I_N_ _T_H_E_ _D_L_S_t_u_d_i_o_ _P_L_A_T_F_O_R_M
+_M_O_D_U_L_E_S_ _I_N_ _T_H_E_ _D_L_S_t_u_d_i_o_ _P_L_A_T_F_O_R_M
 _E_x_a_m_p_l_e_s_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_A_d_v_e_r_s_a_r_i_a_l_L_e_a_r_n_i_n_g_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_D_i_f_f_u_s_i_o_n_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_S_e_q_2_S_e_q_L_e_a_r_n_i_n_g_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_D_a_t_a_P_r_e_d_i_c_t_i_o_n_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_T_r_a_n_s_f_o_r_m_e_r_s_ _D_I_R_E_C_T_O_R_Y
 _E_x_a_m_p_l_e_s_M_e_t_r_i_c_L_e_a_r_n_i_n_g_ _D_I_R_E_C_T_O_R_Y
 _T_H_E_ _D_A_T_A_S_E_T_S_ _I_N_C_L_U_D_E_D
-_ _ _ _ _F_O_R_ _T_H_E_ _M_A_I_N_ _D_L_S_t_u_d_i_o_ _M_O_D_U_L_E
+_ _ _ _ _F_O_R_ _T_H_E_ _M_A_I_N_ _D_L_S_t_u_d_i_o_ _C_L_A_S_S_ _a_n_d_ _i_t_s_ _I_N_N_E_R_ _C_L_A_S_S_E_S
 _ _ _ _ _F_O_R_ _S_e_q_2_S_e_q_ _L_E_A_R_N_I_N_G
 _ _ _ _ _F_O_R_ _A_D_V_E_R_S_A_R_I_A_L_ _L_E_A_R_N_I_N_G_ _A_N_D_ _D_I_F_F_U_S_I_O_N
 _ _ _ _ _F_O_R_ _D_A_T_A_ _P_R_E_D_I_C_T_I_O_N
 _ _ _ _ _F_O_R_ _T_R_A_N_S_F_O_R_M_E_R_S
 _B_U_G_S
 _A_C_K_N_O_W_L_E_D_G_M_E_N_T_S
 _A_B_O_U_T_ _T_H_E_ _A_U_T_H_O_R
 _C_O_P_Y_R_I_G_H_T
 
  
 CCHHAANNGGEE LLOOGG
  
+  Version 2.4.9:
+ 
+    This version contains fixes for the pathname errors in the Transformers module
+    of DLStudio. The errors were related to where the models and the checkpoints
+    were supposed to be stored during training.
+ 
   Version 2.4.8:
  
     In this version, I have made two important changes to the Transformers module
     in DLStudio: 
 (1) The Transformers module now includes a new class that I have
     named visTransformer that works like the famous Vision Transformer (ViT)
     proposed by Dosovitskiy et al. And 
@@ -123,18 +129,17 @@
 up of the main
     doc page for GenerativeDiffusion module and of a couple of the functions in
     the module.
  
   Version 2.4.2:
  
     DLStudio now includes a new module devoted to data modeling with diffusion.
-    This module, named GenerativeDiffusion, is a co-
-class of DLStudio.  That is,
-    GenerativeDiffusion resides at the same level of software abstraction as the
-    main DLStudio class in the platform.  See the README in the new
+    This module, named GenerativeDiffusion, is a module in the overall DLStudio 
+    platform.  The GenerativeDiffusion class resides at the same level of software 
+    abstraction as the main DLStudio class in the platform.  See the README in the
     ExamplesDiffusion directory of the distribution for how to experiment with the
     diffusion based code in DLStudio.
  
   Version 2.3.6:
  
     Gets rid of the inadvertently hardcoded value for the batch size in the
     testing part of the code for Semantic Segmentation.
@@ -241,16 +246,17 @@
     these loss functions is the script object_detection_and_localization_iou.py in
     the Examples directory of DLStudio.
  
   Version 2.2.2:
  
     This version of DLStudio presents my implementation of transformers in deep
     learning. You will find two transformer implementations in the Transformers
-    co-class of DLStudio in the distribution directory: TransformerFG and
-    TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
+    module of the DLStudio platform in the distribution directory:
+ TransformerFG 
+    and TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
     Generation"; it is my implementation of the architecture presented originally
     in the seminal paper "Attention is All You Need" by Vaswani et el.  And the
     second, TransformerPreLN 
 ("PreLN" stands for "Pre Layer Norm") is a small but
     important modification of the original idea that is based on the paper "On
     Layer Normalization in the Transformer Architecture" by Xiong et al.  I could
     have easily combined the two implementations with a small number of
@@ -266,23 +272,22 @@
     components of a transformer for educational purposes.  As things stand, these
     versions contain features that did not make into the public release version
     2.2.2 on account of inadequate testing.  I may include those features in
     versions of DLStudio after 2.2.2.
  
   Version 2.1.6:
  
-    All the changes are confined to the DataPrediction co-class of the DLStudio
-    module.  After posting the previous version, I noticed that the quality of the
-    code in DataPrediction was not up to par.  The new version presents a
+    All the changes are confined to the DataPrediction module in the DLStudio
+    platform.  After posting the previous version, I noticed that the quality of 
+    the code in DataPrediction was not up to par.  The new version presents a
     cleaned-up version of the DataPrediction class.
  
   Version 2.1.5:
  
-    DLStudio has now been equipped with a new co-
-class named DataPrediction whose
+    DLStudio has now been equipped with a new module named DataPrediction whose
     focus is solely on solving data prediction problems for time-
 series data.  A
     time-series consists of a sequence of observations recorded at regular
     intervals.  These could, for example, be the price of a stock share recorded
     every hour; the hourly recordings of electrical load at your local power
     utility company; the mean average temperature recorded on an annual basis; and
     so on.  We want to use the past observations to predict the value of the next
@@ -323,17 +328,16 @@
     classes AdversarialNetworks and Seq2SeqNetworks to AdversarialLearning and
     Seq2SeqLearning, respectively.
  
   Version 2.1.0:
  
     I have reorganized the code base a bit to make it easier for DLStudio to grow
     in the future.  This I did by moving the sequence-to-sequence learning
-    (seq2seq) code to a separate co-
-class of the main DLStudio class.  The name of
-    the new class is Seq2SeqLearning and it resides at the top level of the
+    (seq2seq) code to a separate module of the DLStudio platform.  The name of
+    the new module is Seq2SeqLearning and it resides at the top level of the
     distribution.
  
   Version 2.0.9:
  
     With this version, DLStudio comes with educational material on
     sequence-to-sequence learning (seq2seq). To that end, I have included the
     following two new classes in DLStudio: 
@@ -538,32 +542,32 @@
     key features of neural network architectures.  These implementations, along
     with their explanations through detailed slide presentations at our Deep
     Learning class website at Purdue, result in an educational framework that is
     much more efficient in what it can deliver within the time constraints of a
     single semester.
  
     DLStudio facilitates learning through a combination of inner classes of the
-    main module class --- called DLStudio naturally --- and several co-
-classes of
-    the main class that deal with adversarial learning, sequence-to-sequence
-    learning, data prediction, text analysis, and transformers.
+    main module class --- called DLStudio naturally --- and several modules of
+    the overall platform.  These modules deal with Adversarial Learning, 
+    Sequence-to-Sequence Learning, Diffusion, Data Prediction, Text Analysis, 
+    and Transformers.
  
     For the most part, the common code that you'd need in different scenarios for
     using neural networks has been placed inside the definition of the main
     DLStudio class in a file named DLStudio.py in the distribution.  That makes
     more compact the definition of the other inner classes within DLStudio. And,
     to a certain extent, that also results in a bit more compact code in the
-    co-classes of DLStudio.
+    different modules in the DLStudio platform.
  
 ? ?  SSKKIIPP CCOONNNNEECCTTIIOONNSS
  
     You can use DLStudio's inner class BMEnet to experiment with connection
     skipping in a deep network. Connection skipping means to provide shortcuts in
     a computational graph around the commonly used network components like
-    convolutional and other types of layers.  In the absence of such shortcuits,
+    convolutional and other types of layers.  In the absence of such shortcuts,
     deep networks suffer from the problem of vanishing gradients that degrades
     their performance.  Vanishing gradients means that the gradients of the loss
     calculated in the early layers of a network become increasingly muted as the
     network becomes deeper.  An important mitigation strategy for addressing this
     problem consists of creating a CNN using blocks with skip connections.
  
     As shown in the script playing_with_skip_connections.py in the Examples
@@ -781,15 +785,15 @@
  
     The pre-trained word2vec embeddings used in these scripts are accessed
     through the popular gensim library.
  
  
 ? ?  DDAATTAA MMOODDEELLIINNGG WWIITTHH AADDVVEERRSSAARRIIAALL LLEEAARRNNIINNGG
  
-    Starting with version 2.0.3, DLStudio includes a separate co-class named
+    Starting with version 2.0.3, DLStudio includes a separate module named
     AdversarialLearning for experimenting with different adversarial learning
     approaches for data modeling.  Adversarial Learning consists of simultaneously
     training a Generator and a Discriminator 
 (or, a Generator and a Critic) with
     the goal of getting the Generator to produce from pure noise images that look
     like those in the training dataset.  When Generator-Discriminator pairs are
     used, the Discriminator's job is to become an expert at recognizing the
@@ -888,15 +892,15 @@
     third script.  The results produced by these scripts (for the constructor
     options shown in the scripts) are included in a subdirectory named
     RVLCloud_based_results.
  
  
 ? ?  DDAATTAA MMOODDEELLIINNGG WWIITTHH DDIIFFFFUUSSIIOONN
  
-    Starting with Version 2.4.2, DLStudio includes a co-class named
+    Starting with Version 2.4.2, DLStudio includes a new module named
     GenerativeDiffusion for experimenting with what's known as "Denoising
     Diffusion".  The Denoising Diffusion approach to data modeling is based on the
     interaction between two Markov Chains: A forward chain called the q-
 chain and
     a reverse chain called the p-chain.  Both chains operate concurrently as
     follows and involved T timesteps where the value of T is a user-specified
     parameter.
@@ -1004,18 +1008,16 @@
  
     Sequence-to-sequence learning (seq2seq) is about predicting an outcome
     sequence from a causation sequence, or, said another way, a target sequence
     from a source sequence.  Automatic machine translation is probably one of the
     most popular applications of seq2seq.  DLStudio uses English-to-Spanish
     translation to illustrate the programming idioms and the PyTorch structures
     you need for seq2seq.  To that end, Version 2.1.0 of DLStudio includes a
-    co-class 
-(meaning a class that resides at the top level in the distribution)
-    named Seq2SeqLearning that consists of the following two demonstration
-    classes:
+    new module named Seq2SeqLearning that consists of the following two 
+    demonstration classes:
  
         1.  Seq2SeqWithLearnableEmbeddings
  
         2.  Seq2SeqWithPretrainedEmbeddings
  
     As their names imply, the first is for seq2seq with learnable embeddings and
     the second for seq2seq with pre-
@@ -1062,16 +1064,16 @@
 ? ?  DDAATTAA PPRREEDDIICCTTIIOONN
  
     Let's say you have a sequence of observations recorded at regular intervals.
     These could, for example, be the price of a stock share recorded every hour;
     the hourly recordings of electrical load at your local power utility company;
     the mean average temperature recorded on an annual basis; and so on.  We want
     to use the past observations to predict the value of the next one.  Solving
-    these types of problems is the focus of the DataPrediction co-class of
-    DLStudio.
+    these types of problems is the focus of the DataPrediction module in the
+    DLStudio platform.
  
     As a problem, data prediction has much in common with text analytics and
     seq2seq processing, in the sense that the prediction at the next time instant
     must be based on the previous observations in a manner similar to what we do
     in text analytics where the next word is understood taking into account all
     the previous words in a sentence.  However, there are three significant
     differences between purely numerical data prediction problems and text-
@@ -1141,15 +1143,15 @@
     the Reset gates of a regular GRU into a single gate called the Forget Gate.
     You could say that pmGRU is a lightweight version of a regular GRU and its use
     may therefore lead to a slight loss of accuracy in the predictions.  You will
     find it educational to compare the performance you get with my pmGRU-based
     implementation with an implementation that uses PyTorch's GRU for the same
     dataset.
  
-    Your main entry point for experimenting with the DataPrediction co-class is
+    Your main entry point for experimenting with the DataPrediction module is
     the following script in the ExamplesDataPrediction directory of the DLStudio
     distribution:
  
         power_load_prediction_with_pmGRU.py
  
     Before you can run this script, you would need to download the training
     dataset used in this example.  See the "For Data Prediction" part of the "The
@@ -1195,15 +1197,15 @@
     part of the logic in a visTransformer is identical to what it is in a
     transformer class for Seq2SeqLearning learning.  That logic kicks in after you
     have divided an image into patches and you represent each patch by an
     embedding vector --- in exactly the same as when you represent a word or a
     token in a sentence by an embedding vector.
  
     You will see three different implementations of the transformer architecture in
-    the Transformers co-class of DLStudio:
+    the Transformers module of the DLStudio platform:
  
           TransformerFG
  
           TransformerPreLN
  
           visTransformer
  
@@ -1215,15 +1217,15 @@
     the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
     the same architecture but with the modification suggested by Xiong et al. for
     more stable learning.  Since, the modification is small from an architectural
     standpoint, I could have combined both transformer types in the same
     implementation with some conditional logic to account for the differences.
     However, I have chosen to keep them separate mostly for educational purposes.
     Further details on these implementations are in the documentation blocks in
-    the Transformers co-class.  
+    the Transformers module.
  
     The visTransformer implementation is based on the paper "An Image is Worth
     16x16 Words:
  Transformers for Image Recognition at Scale'' by Dosovitskiy et
     al.
  
     If you want to use my code for learning the main ideas related to how to
@@ -1553,18 +1555,16 @@
          set to the network whose summary you want to see.
  
  
 TTHHEE MMAAIINN IINNNNEERR CCLLAASSSSEESS OOFF TTHHEE DDLLSSttuuddiioo CCLLAASSSS
  
     By "inner classes" I mean the classes that are defined within the class file
     DLStudio.py in the DLStudio directory of the distribution.  The DLStudio
-    platform also includes what I have referred to as the Co-
-Classes in the next
-    section.  A Co-Class resides at the same level of abstraction as the main
-    DLStudio class defined in the DLStudio.py file.
+    platform also includes several modules that reside at the same level of 
+    software abstraction as the main DLStudio class defined in the DLStudio.py file.
  
     The purpose of the following two inner classes is to demonstrate how you can
     create a custom class for your own network and test it within the framework
     provided by DLStudio.
  
     (1)  class ExperimentsWithSequential
  
@@ -1663,27 +1663,25 @@
          this inner class uses the pre-trained 300-
 element word2vec embeddings as
          made available by Google for 3 million words and phrases drawn from the
          Google News dataset. In DLStudio, we access these embeddings through the
          popular gensim library.
  
  
-CCOO--CCLLAASSSSEESS IINN TTHHEE DDLLSSttuuddiioo PPLLAATTFFOORRMM
+MMOODDUULLEESS IINN TTHHEE DDLLSSttuuddiioo PPLLAATTFFOORRMM
  
-    As stated at the beginning of the previous section, a Co-
-Class resides at the
-    same level of abstraction in the distribution directory as the main DLStudio
-    platform. Each Co-
-Class is defined in a separate subdirectory at the top level
-    of the distribution directory.  While the main DLStudio class is defined in a
-    subdirectory of the same name, the other subdirectories that contain
-    definitions for the co-
-classes are named AdversarialLearning, Seq2SeqLearning,
-    DataPrediction, Transformers, and MetricLearning.  What follows in this
-    section are additional details regarding these co-classes:
+    As stated at the beginning of the previous section, a module resides at the
+    same level of software abstraction in the distribution directory as the main
+    DLStudio class in the platform. Each module is defined in a separate
+    subdirectory at the top level of the distribution directory.  While the main
+    DLStudio class is defined in a subdirectory of the same name, the other
+    subdirectories that contain the definitions for the modules are named
+    AdversarialLearning, Seq2SeqLearning, DataPrediction, Transformers,
+    GenerativeDiffusion, and MetricLearning.  What follows in this section are
+    additional details regarding these co-classes:
  
  
 
     AdversarialLearning:
     ===================
  
     As I mentioned in the Introduction, the purpose of the AdversarialLearning
@@ -1745,16 +1743,15 @@
 chain is with known amount of Gaussian isotropic noise.  In
     the p-
 chain, on the other hand, the goal is for a neural network to learn from
     the diffusion carried out in the q-chain how to carry out a denoising
     operation that would amount to a reversal of that diffusion.
  
     All of the key elements of the code that I have presented in the
-    GenerativeDiffusion co-
-class are extracted from OpenAI's "Improved Diffusion"
+    GenerativeDiffusion module are extracted from OpenAI's "Improved Diffusion"
     project at GitHub that presents a PyTorch implementation of the work authored
     by Nichol and Dhariwal in their very famous paper "Improved Denoising
     Diffusion Probabilistic Models". See the beginning part of the doc page for
     the GenerativeDiffusion module for URLs to the GitHub code and their
     publication.
  
     If you want to play with the code in GenerativeDiffusion, your starting point
@@ -1786,16 +1783,15 @@
     your overall network learn on its own what are known as vector embeddings for
     the words; or (2) Use pre-trained embeddings as provided by word2vec or
     Fasttext.
  
     After you have resolved the issue of word representation, your next challenge
     is how to implement the attention mechanism that you're going to need for
     aligning the similar grammatical units in the two languages. The seq2seq code
-    demonstrated in this co-
-class uses the attention model proposed by Bahdanau,
+    demonstrated in this module uses the attention model proposed by Bahdanau,
     Cho, and Bengio in the form of a separate Attention class.  The name of this
     attention class is Attention_BCB.  In a separate attention class named
     Attention_SR, I have also included the attention mechanism used by Sean
     Robertson in his very popular NLP tutorial at the main PyTorch website.
  
     Seq2SeqLearning contains the following two inner classes for illustrating
     seq2seq:
@@ -1888,15 +1884,15 @@
     modifications suggested by Xiong et al. in their paper "On Layer Normalization
     in the Transformer Architecture" for more stable learning.  The two versions
     of transformers differ in only one respect:
  The placement of the LayerNorm in
     relation to the architectural components related to attention and the
     feedforward network.  Literally, the difference is small, yet its consequences
     are significant regarding the stability of learning.  Finally, visTransformer
-    is my implementation of the Vision Transformer as presented in the famou paper
+    is my implementation of the Vision Transformer as presented in the famous paper
     "An Image is Worth 16x16$ Words:
  Transformers for Image Recognition at Scale''
     by Dosovitskiy et al.
  
     The fundamentals of how the attention works in all three transformer based
     implementations in the Transformers module are exactly the same.  For
     self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
@@ -2021,15 +2017,15 @@
 (i,j,k) in which two indices are the same.  If B is the batch size,
     this is easily done by first forming a BxB array that is the logical negation
     of a Boolean array of the same size whose True values are only on the
     diagonal.  We can reshape this BxB Boolean array into three BxBxB shaped
     Boolean arrays, the first in which the True values exist only where i and j
     values are not the same, the second in which the True values occur only when i
     and k index values are not the same, and the third that has True values only
-    when the j and k index values are not the same.  By taking a logial AND of all
+    when the j and k index values are not the same.  By taking a logical AND of all
     three BxBxB Boolean arrays, we get the result we want.  Next, we construct a
     BxBxB Boolean tensor in which the True values occur only where the first two
     index values imply that their corresponding labels are identical and where the
     last index corresponds to a label that does not agree with that for the first
     two index values.
  
     Even after you have formed the triplets, your next mini-challenge is to
@@ -2059,15 +2055,15 @@
 EExxaammpplleess DDIIRREECCTTOORRYY
  
     The Examples subdirectory in the distribution contains the following scripts:
  
     (1)  playing_with_reconfig.py
  
          Shows how you can specify a convolution network with a configuration
-         string.  The DLStudio module parses the string constructs the network.
+         string.  The main DLStudio class parses the string constructs the network.
  
     (2)  playing_with_sequential.py
  
          Shows you how you can call on a custom inner class of the 'DLStudio'
          module that is meant to experiment with your own network.  The name of
          the inner class in this example script is ExperimentsWithSequential
  
@@ -2086,22 +2082,22 @@
          directly illustrate in a classroom setting the improvement you can get
          with skip connections.  And by giving an appropriate value to the "depth"
          option, you can show results for networks of different depths.
  
     (6)  custom_data_loading.py
  
          This script shows how to use the custom dataloader in the inner class
-         CustomDataLoading of the DLStudio module.  That custom dataloader is
+         CustomDataLoading of the main DLStudio class.  That custom dataloader is
          meant specifically for the PurdueShapes5 dataset that is used in object
          detection and localization experiments in DLStudio.
  
     (7)  object_detection_and_localization.py
  
          This script shows how you can use the functionality provided by the inner
-         class DetectAndLocalize of the DLStudio module for experimenting with
+         class DetectAndLocalize of the main DLStudio class for experimenting with
          object detection and localization.  Detecting and localizing (D&L)
          objects in images is a more difficult problem than just classifying the
          objects.  D&L requires that your CNN make two different types of
          inferences simultaneously, one for classification and the other for
          localization.  For the localization part, the CNN must carry out what is
          known as regression. What that means is that the CNN must output the
          numerical values for the bounding box that encloses the object that was
@@ -2269,24 +2265,24 @@
 trained embeddings for the target language
          is explained in the main comment doc associated with the class
          Seq2SeqWithPretrainedEmbeddings.
  
  
 EExxaammpplleessDDaattaaPPrreeddiiccttiioonn DDIIRREECCTTOORRYY
  
-    The ExampsleDataPrediction directory of the distribution contains the
+    The ExamplesDataPrediction directory of the distribution contains the
     following script for demonstrating data prediction for time-series data:
  
         power_load_prediction_with_pmGRU.py
  
     This script uses a subset of the dataset provided by Kaggle for one of their
     machine learning competitions.  The dataset consists of over 10-
 years worth of
     hourly electric load recordings made available by several utilities in the
-    east and the midwest of the United States.  You can download this dataset from
+    east and the Midwest of the United States.  You can download this dataset from
     a link at the top of the main DLStudio doc page.
  
  
 EExxaammpplleessTTrraannssffoorrmmeerrss DDIIRREECCTTOORRYY
  
     The ExamplesTransformers directory of the distribution contains the following
     four scripts for experimenting with transformers in DLStudio:
@@ -2295,18 +2291,16 @@
         seq2seq_with_transformerPreLN.py         
  
         image_recog_with_visTransformer.py
         test_checkpoint_for_visTransformer.py 
  
  
     The first two scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-
-class and
-    the example scripts associated with that co-
-class. The last two relate to my
+    similar to what's demonstrated by the code in the Seq2SeqLearning module and
+    the example scripts associated with that module. The last two relate to my
     demonstration of image recognition with a transformer based implementation.  I
     have used the CFAR10 dataset for image recognition.
  
  
 EExxaammpplleessMMeettrriiccLLeeaarrnniinngg DDIIRREECCTTOORRYY
  
     The ExamplesMetricLearning directory at top level of the distribution 
@@ -2323,15 +2317,15 @@
     MetricLearning module.
  
  
 TTHHEE DDAATTAASSEETTSS IINNCCLLUUDDEEDD
  
     [must be downloaded separately]
  
-? ?  FFOORR TTHHEE MMAAIINN DDLLSSttuuddiioo MMOODDUULLEE
+? ?  FFOORR TTHHEE MMAAIINN DDLLSSttuuddiioo CCLLAASSSS aanndd iittss IINNNNEERR CCLLAASSSSEESS
  
         Download the dataset archive 'datasets_for_DLStudio.tar.gz' through the
         link "Download the image datasets for the main DLStudio Class" provided at
         the top of this documentation page and store it in the 'Example' directory
         of the distribution.  Subsequently, execute the following command in the
         'Examples' directory:
     
@@ -2554,16 +2548,15 @@
         That will create a 'data' subdirectory in the ExamplesTransformers
         directory and deposit in that subdirectory the following archives
  
             en_es_xformer_8_10000.tar.gz
             en_es_xformer_8_90000.tar.gz
  
         These are both derived from the same data source as in the dataset for the
-        examples associated with the Seq2SeqLearning co-
-class.  The first has only
+        examples associated with the Seq2SeqLearning module.  The first has only
         10,000 pars of English-
 Spanish sentences and meant primarily for debugging
         purposes.  The second contains 90000 pairs of such sentences.  The number
         '8' in the dataset names means that no sentence contains more than 8 real
         words.  With the "SOS" and "EOS" tokens used as sentence delimiters, the
         maximum number of words in each sentence in either language is 10.
  
@@ -2597,15 +2590,15 @@
     Version 2.2.2: My laboratory's (RVL) journey into the world of transformers
     began with a series of lab seminars by Constantine Roros and Rahul Deshmukh.
     Several subsequent conversations with them were instrumental in helping me
     improve the understanding I had gained from the seminars.  Additional
     conversations with Rahul about the issue of masking were important to how I
     eventually implemented those ideas in my code.
  
-    Rahul Deshmukh discovered the reason as to why my implmentation of the skip
+    Rahul Deshmukh discovered the reason as to why my implementation of the skip
     connection code was not working with the more recent versions of PyTorch.  My
     problem was using in-place operations in the forward() of the networks that
     called for connection skipping. This led to the release of Version 2.3.3 of
     DLStudio.
  
     The main reason for Version 2.3.4 was my new design for the SkipBlock class
     and also my easier-to-
@@ -2617,15 +2610,15 @@
     from its input to its output but without downsampling the input, that elicited
     an error from the system.  Cheng-
 Hao also provided a correction for the error.
     Thanks, Cheng-Hao!
  
     Aditya Chauhan proved to be a great sounding board in my journey into the land
     of diffusion that led to Version 2.4.2.  I particularly appreciated Aditya's
-    help in understanding how the attention mechanism worked in the OpanAI code
+    help in understanding how the attention mechanism worked in the OpenAI code
     library at GitHub.  Aditya is working for his PhD in RVL.  Thanks, Aditya!
  
  
 AABBOOUUTT TTHHEE AAUUTTHHOORR
  
     The author, Avinash Kak, is a professor of Electrical and Computer Engineering
     at Purdue University.  For all issues related to this module, contact the
@@ -2760,16 +2753,16 @@
                      designing a custom data loader.  Ordinarily, if the basic format of how the dataset
                      is stored is similar to one of the datasets that the Torchvision module knows about,
                      you can go ahead and use that for your own dataset.  At worst, you may need to carry
                      out some light customizations depending on the number of classes involved, etc.
                       
                      However, if the underlying dataset is stored in a manner that does not look like
                      anything in Torchvision, you have no choice but to supply yourself all of the data
-                     loading infrastructure.  That is what this inner class of the DLStudio module is all
-                     about.
+                     loading infrastructure.  That is what this inner class of the main DLStudio class 
+                     is all about.
                       
                      The custom data loading exercise here is related to a dataset called PurdueShapes5
                      that contains 32x32 images of binary shapes belonging to the following five classes:
                       
                                     1.  rectangle
                                     2.  triangle
                                     3.  disk
@@ -2838,15 +2831,15 @@
                      Class Path:  DLStudio  ->  ExperimentsWithCIFAR
                  EExxppeerriimmeennttssWWiitthhSSeeqquueennttiiaall = <class 'DLStudio.DLStudio.ExperimentsWithSequential'>
                      Demonstrates how to use the torch.nn.Sequential container class
                       
                      Class Path:  DLStudio  ->  ExperimentsWithSequential
                  NNeett = <class 'DLStudio.DLStudio.Net'>
                  SSeemmaannttiiccSSeeggmmeennttaattiioonn = <class 'DLStudio.DLStudio.SemanticSegmentation'>
-                     The purpose of this inner class is to be able to use the DLStudio module for
+                     The purpose of this inner class is to be able to use the DLStudio platform for
                      experiments with semantic segmentation.  At its simplest level, the purpose of
                      semantic segmentation is to assign correct labels to the different objects in a
                      scene, while localizing them at the same time.  At a more sophisticated level, a
                      system that carries out semantic segmentation should also output a symbolic
                      expression based on the objects found in the image and their spatial relationships
                      with one another.
                       
@@ -2866,15 +2859,15 @@
                      for experimenting with mUnet.  Each image in this dataset contains a random number
                      of selections from five different shapes, with the shapes being randomly scaled,
                      oriented, and located in each image.  The five different shapes are: rectangle,
                      triangle, disk, oval, and star.
                       
                         Class Path:   DLStudio  ->  SemanticSegmentation
                  TTeexxttCCllaassssiiffiiccaattiioonn = <class 'DLStudio.DLStudio.TextClassification'>
-                     The purpose of this inner class is to be able to use the DLStudio module for simple 
+                     The purpose of this inner class is to be able to use the DLStudio platform for simple 
                      experiments in text classification.  Consider, for example, the problem of automatic 
                      classification of variable-length user feedback: you want to create a neural network
                      that can label an uploaded product review of arbitrary length as positive or negative.  
                      One way to solve this problem is with a recurrent neural network in which you use a 
                      hidden state for characterizing a variable-length product review with a fixed-length 
                      state vector.  This inner class allows you to carry out such experiments.
                       
@@ -2898,13 +2891,13 @@
                      News reports.  I access these embeddings through the popular Gensim library.
                       
                      Class Path:  DLStudio -> TextClassificationWithEmbeddings
  
 DDaattaa
    ____aauutthhoorr____ = 'Avinash Kak (kak@purdue.edu)'
    ____ccooppyyrriigghhtt____ = '(C) 2024 Avinash Kak. Python Software Foundation.'
-   ____ddaattee____ = '2024-April-27'
-   ____uurrll____ = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.8.html'
-   ____vveerrssiioonn____ = '2.4.8'
+   ____ddaattee____ = '2024-May-1'
+   ____uurrll____ = 'https://engineering.purdue.edu/kak/distDT/DLStudio-2.4.9.html'
+   ____vveerrssiioonn____ = '2.4.9'
  
 AAuutthhoorr
          Avinash Kak (kak@purdue.edu)
```

### Comparing `DLStudio-2.4.8/DLStudio.egg-info/PKG-INFO` & `DLStudio-2.4.9/DLStudio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DLStudio
-Version: 2.4.8
+Version: 2.4.9
 Summary: A PyTorch based software platform for teaching the Deep Learning class at Purdue University
-Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
+Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
 Maintainer: Avinash Kak
 Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz
+Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.tar.gz
 Keywords: PyTorch programming
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.10
 
 
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

### Comparing `DLStudio-2.4.8/DLStudio.egg-info/SOURCES.txt` & `DLStudio-2.4.9/DLStudio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DLStudio-2.4.8.html
+DLStudio-2.4.9.html
 MANIFEST.in
 Makefile
 README
 setup.py
 AdversarialLearning/AdversarialLearning.py
 AdversarialLearning/__init__.py
 DLStudio/DLStudio.py
```

### Comparing `DLStudio-2.4.8/DataPrediction/DataPrediction.py` & `DLStudio-2.4.9/DataPrediction/DataPrediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
-  You are looking at the DataPrediction co-class file in the DLStudio platform.
+  You are looking at the DataPrediction module file in the DLStudio platform.
   For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
 
 DATA PREDICTION:
```

### Comparing `DLStudio-2.4.8/DataPrediction/__init__.py` & `DLStudio-2.4.9/DataPrediction/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/README` & `DLStudio-2.4.9/Examples/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/custom_data_loading.py` & `DLStudio-2.4.9/Examples/custom_data_loading.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/noisy_object_detection_and_localization.py` & `DLStudio-2.4.9/Examples/noisy_object_detection_and_localization.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/object_detection_and_localization.py` & `DLStudio-2.4.9/Examples/object_detection_and_localization.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/object_detection_and_localization_iou.py` & `DLStudio-2.4.9/Examples/object_detection_and_localization_iou.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/playing_with_cifar10.py` & `DLStudio-2.4.9/Examples/playing_with_cifar10.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/playing_with_reconfig.py` & `DLStudio-2.4.9/Examples/playing_with_reconfig.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/playing_with_sequential.py` & `DLStudio-2.4.9/Examples/playing_with_sequential.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/playing_with_skip_connections.py` & `DLStudio-2.4.9/Examples/playing_with_skip_connections.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/semantic_segmentation.py` & `DLStudio-2.4.9/Examples/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_GRU.py` & `DLStudio-2.4.9/Examples/text_classification_with_GRU.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_GRU_word2vec.py` & `DLStudio-2.4.9/Examples/text_classification_with_GRU_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_TEXTnet.py` & `DLStudio-2.4.9/Examples/text_classification_with_TEXTnet.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2.py` & `DLStudio-2.4.9/Examples/text_classification_with_TEXTnetOrder2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_TEXTnetOrder2_word2vec.py` & `DLStudio-2.4.9/Examples/text_classification_with_TEXTnetOrder2_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Examples/text_classification_with_TEXTnet_word2vec.py` & `DLStudio-2.4.9/Examples/text_classification_with_TEXTnet_word2vec.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesAdversarialLearning/README` & `DLStudio-2.4.9/ExamplesAdversarialLearning/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG1.py` & `DLStudio-2.4.9/ExamplesAdversarialLearning/dcgan_DG1.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesAdversarialLearning/dcgan_DG2.py` & `DLStudio-2.4.9/ExamplesAdversarialLearning/dcgan_DG2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_CG1.py` & `DLStudio-2.4.9/ExamplesAdversarialLearning/wgan_CG1.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesAdversarialLearning/wgan_with_gp_CG2.py` & `DLStudio-2.4.9/ExamplesAdversarialLearning/wgan_with_gp_CG2.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py` & `DLStudio-2.4.9/ExamplesDataPrediction/power_load_prediction_with_pmGRU.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesDiffusion/GenerateNewImageSamples.py` & `DLStudio-2.4.9/ExamplesDiffusion/GenerateNewImageSamples.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesDiffusion/README` & `DLStudio-2.4.9/ExamplesDiffusion/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesDiffusion/RunCodeForDiffusion.py` & `DLStudio-2.4.9/ExamplesDiffusion/RunCodeForDiffusion.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesDiffusion/VisualizeSamples.py` & `DLStudio-2.4.9/ExamplesDiffusion/VisualizeSamples.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py` & `DLStudio-2.4.9/ExamplesMetricLearning/example_for_pairwise_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesMetricLearning/example_for_triplet_loss.py` & `DLStudio-2.4.9/ExamplesMetricLearning/example_for_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py` & `DLStudio-2.4.9/ExamplesSeq2SeqLearning/seq2seq_with_learnable_embeddings.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py` & `DLStudio-2.4.9/ExamplesSeq2SeqLearning/seq2seq_with_pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesTransformers/image_recog_with_visTransformer.py` & `DLStudio-2.4.9/ExamplesTransformers/image_recog_with_visTransformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ##  image_recog_with_visTransformer.py
 
 """
 This script is for experimenting with visTransformer implementation in the Transformers
 module in DLStudio.
 
 See ny Week 14 slides at Purdue's Deep Learning class for further information regarding
-this part of DLStudio.
+this part of the Transformers module.
 """
 
 """
 seed = 0           
 random.seed(seed)
 torch.manual_seed(seed)
 torch.cuda.manual_seed(seed)
```

### Comparing `DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerFG.py` & `DLStudio-2.4.9/ExamplesTransformers/seq2seq_with_transformerPreLN.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 #!/usr/bin/env python
 
-##  seq2seq_with_transformerFG.py
+##  seq2seq_with_transformerPreLN.py
 
 """
-    This script is for experimenting with TransformerFG.
+    This script is for experimenting with TransformerPreLN.
 
-    For an introduction to TransformerFG, read the large comment block associated
+    For an introduction to TransformerPreLN, read the large comment block associated
     with the definition of this class in the Transformers co-class of DLStudio.
-
-    Also read the doc block associated with the other transformer class, TransformerPreLN,
-    for the difference between TransformerFG and TransformerPreLN.
-
-    To run this example, you will need to have installed at least one of the following
+    That introduction explains the difference between TransformerPreLN and 
+    TransformerFG.
+    
+    To run this example, you will need to have installed at least one of the following 
     two English-to-Spanish translation dataset archives:
 
           en_es_xformer_8_10000.tar.gz
 
           en_es_xformer_8_90000.tar.gz
-
-    The first consists of 10,000 pairs of English-Spanish sentences and the second
-    90,0000 such pairs.
+         
+    The first consists of 10,000 pairs of English-Spanish sentences and the second of
+    90,0000.  
 
     The maximum number of words in any sentence, English or Spanish, is 8.  When you
     include the sentence delimiter tokens SOS and EOS, that makes for a max length of
     10 for the sentences.
+
+    *** RECOMMENDATION ***:
+
+       I recommend that you first try to run this script with exactly the settings
+       that are currently in the script:
+
+              1.  Use the smaller debugging dataset for a faster turn-around from
+                  the code:
+
+                         en_es_xformer_8_10000.tar.gz
+
+              2.  Use the option
+
+                         masking = True      
+
+              3.  epochs =  60
+
+       Note that with the smaller dataset, you will only get one training iteration 
+       per epoch, assuming you are using a batch-size of 50.
+
+       Subsequently, try running the script for the larger dataset.
 """
 
 import random
 import numpy
 import torch
 import os, sys
 
@@ -42,92 +62,89 @@
 
 
 ##  watch -d -n 0.5 nvidia-smi
 
 from DLStudio import *
 from Transformers import *
 
+
 dataroot = "./data/"
 #dataroot = "/home/kak/TextDatasets/en_es_corpus_xformer/"
 #dataroot = "/mnt/cloudNAS3/Avi/TextDatasets/en_es_corpus_xformer/"
 
-data_archive =  "en_es_xformer_8_90000.tar.gz"
+data_archive =  "en_es_xformer_8_10000.tar.gz"                 ##  for debugging only
+#data_archive =  "en_es_xformer_8_90000.tar.gz"
 
 max_seq_length = 10
 
-embedding_size = 256        
+embedding_size = 256               
 #embedding_size = 128
-#embedding_size = 64        
-
-num_basic_encoders = num_basic_decoders = num_atten_heads = 4     
-#num_basic_encoders = num_basic_decoders = num_atten_heads = 2    
+#embedding_size = 64               
 
-#optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-9}
-optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-6}
+num_basic_encoders = num_basic_decoders = num_atten_heads = 4   
+#num_basic_encoders = num_basic_decoders = num_atten_heads = 2  
 
-num_warmup_steps = 4000
-
-#masking = True
-masking = False
+masking = True                    ## For better results
+#masking = False
 
 dls = DLStudio(
                 dataroot = dataroot,
-                path_saved_model = {"encoder" : "./saved_encoder", 
-                                    "decoder" : "./saved_decoder", 
-                                    "embeddings_generator_en" : "./saved_embeddings_generator_en",
-                                    "embeddings_generator_es" : "./saved_embeddings_generator_es",
+                path_saved_model = {"encoder_PreLN" : "./saved_encoder_PreLN", 
+                                    "decoder_PreLN" : "./saved_decoder_PreLN", 
+                                    "embeddings_generator_en_PreLN" : "./saved_embeddings_generator_en_PreLN",
+                                    "embeddings_generator_es_PreLN" : "./saved_embeddings_generator_es_PreLN",
                                    },
+                learning_rate =  1e-5, 
                 batch_size = 50,
                 use_gpu = True,
-                epochs = 40,
-              )
+                epochs = 60,
+      )
 
-xformer = TransformerFG( 
-                        dl_studio = dls,
-                        dataroot = dataroot,
-                        data_archive = data_archive,
-                        max_seq_length = max_seq_length,
-                        embedding_size = embedding_size,
-                        save_checkpoints = True,
-                        num_warmup_steps = num_warmup_steps,
-                        optimizer_params = optimizer_params,
+xformer = TransformerPreLN( 
+                            dl_studio = dls,
+                            dataroot = dataroot,
+                            save_checkpoints = True,
+                            data_archive = data_archive,
+                            max_seq_length = max_seq_length,
+                            embedding_size = embedding_size,
           )
 
-master_encoder = TransformerFG.MasterEncoder(
+master_encoder = TransformerPreLN.MasterEncoder(
                                   dls,
                                   xformer,
                                   num_basic_encoders = num_basic_encoders,
                                   num_atten_heads = num_atten_heads,
                  )    
 
 
-master_decoder = TransformerFG.MasterDecoderWithMasking(
+master_decoder = TransformerPreLN.MasterDecoderWithMasking(
                                   dls,
                                   xformer, 
                                   num_basic_decoders = num_basic_decoders,
                                   num_atten_heads = num_atten_heads,
-                                  masking = masking
+                                  masking = masking,
                  )
 
 
 number_of_learnable_params_in_encoder = sum(p.numel() for p in master_encoder.parameters() if p.requires_grad)
 print("\n\nThe number of learnable parameters in the Master Encoder: %d" % number_of_learnable_params_in_encoder)
 num_layers_encoder = len(list(master_encoder.parameters()))
 print("\nThe number of layers in the Master Encoder: %d\n\n" % num_layers_encoder)
 
 number_of_learnable_params_in_decoder = sum(p.numel() for p in master_decoder.parameters() if p.requires_grad)
 print("\n\nThe number of learnable parameters in the Master Decoder: %d" % number_of_learnable_params_in_decoder)
 num_layers_decoder = len(list(master_decoder.parameters()))
 print("\nThe number of layers in the Master Decoder: %d\n\n" % num_layers_decoder)
 
 if masking:
-    xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
-                                                                                     checkpoints_dir="checkpoints_with_masking_FG")
+    xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
+                                                                        checkpoints_dir="checkpoints_with_masking_PreLN")
 else:
-    xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
-                                                                                        checkpoints_dir="checkpoints_no_masking_FG")
+    xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
+                                                                        checkpoints_dir="checkpoints_no_masking_PreLN")
 
 #import pymsgbox
 #response = pymsgbox.confirm("Finished training.  Start evaluation?")
-
 #if response == "OK": 
-xformer.run_code_for_evaluating_TransformerFG(master_encoder, master_decoder, 'myoutput.txt')
+
+xformer.run_code_for_evaluating_TransformerPreLN(master_encoder, master_decoder)
+
```

### Comparing `DLStudio-2.4.8/ExamplesTransformers/seq2seq_with_transformerPreLN.py` & `DLStudio-2.4.9/ExamplesTransformers/seq2seq_with_transformerFG.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,56 @@
 #!/usr/bin/env python
 
-##  seq2seq_with_transformerPreLN.py
+##  seq2seq_with_transformerFG.py
 
 """
-    This script is for experimenting with TransformerPreLN.
+    This script is for experimenting with TransformerFG.
 
-    For an introduction to TransformerPreLN, read the large comment block associated
+    For an introduction to TransformerFG, read the large comment block associated
     with the definition of this class in the Transformers co-class of DLStudio.
-    That introduction explains the difference between TransformerPreLN and 
-    TransformerFG.
-    
-    To run this example, you will need to have installed at least one of the following 
+
+    Also read the doc block associated with the other transformer class, TransformerPreLN,
+    for the difference between TransformerFG and TransformerPreLN.
+
+    To run this example, you will need to have installed at least one of the following
     two English-to-Spanish translation dataset archives:
 
           en_es_xformer_8_10000.tar.gz
 
           en_es_xformer_8_90000.tar.gz
-         
-    The first consists of 10,000 pairs of English-Spanish sentences and the second of
-    90,0000.  
+
+    The first consists of 10,000 pairs of English-Spanish sentences and the second
+    90,0000 such pairs.
 
     The maximum number of words in any sentence, English or Spanish, is 8.  When you
     include the sentence delimiter tokens SOS and EOS, that makes for a max length of
     10 for the sentences.
+
+
+    RECOMMENDATION:
+
+       I recommend that you first try to run this script with exactly the settings
+       that are currently in the script:
+
+              1.  Use the smaller debugging dataset for a faster turn-around from
+                  the code:
+
+                         en_es_xformer_8_10000.tar.gz
+
+              2.  Use the option
+
+                         masking = True      
+
+              3.  epochs =  40
+
+       Note that with the smaller dataset, you will only get one training iteration 
+       per epoch, assuming you are using a batch-size of 50.
+
+       Subsequently, try running the script for the larger dataset.
+
 """
 
 import random
 import numpy
 import torch
 import os, sys
 
@@ -41,89 +65,94 @@
 
 
 ##  watch -d -n 0.5 nvidia-smi
 
 from DLStudio import *
 from Transformers import *
 
-
-dataroot = "./data/"
-#dataroot = "/home/kak/TextDatasets/en_es_corpus_xformer/"
+#dataroot = "./data/"
+dataroot = "/home/kak/TextDatasets/en_es_corpus_xformer/"
 #dataroot = "/mnt/cloudNAS3/Avi/TextDatasets/en_es_corpus_xformer/"
 
-#data_archive =  "en_es_xformer_8_10000.tar.gz"
-data_archive =  "en_es_xformer_8_90000.tar.gz"
+data_archive =  "en_es_xformer_8_10000.tar.gz"                     ## for debugging only
+#data_archive =  "en_es_xformer_8_90000.tar.gz"
+
 
 max_seq_length = 10
 
-embedding_size = 256               
+embedding_size = 256        
 #embedding_size = 128
-#embedding_size = 64               
+#embedding_size = 64        
 
-num_basic_encoders = num_basic_decoders = num_atten_heads = 4   
-#num_basic_encoders = num_basic_decoders = num_atten_heads = 2  
+num_basic_encoders = num_basic_decoders = num_atten_heads = 4     
+#num_basic_encoders = num_basic_decoders = num_atten_heads = 2    
 
-masking = True
+#optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-9}
+optimizer_params = {'beta1' : 0.9,  'beta2': 0.98,  'epsilon' : 1e-6}
+
+num_warmup_steps = 4000
+
+masking = True                     ## for better results
 #masking = False
 
 dls = DLStudio(
                 dataroot = dataroot,
-                path_saved_model = {"encoder" : "./saved_encoder", 
-                                    "decoder" : "./saved_decoder", 
-                                    "embeddings_generator_en" : "./saved_embeddings_generator_en",
-                                    "embeddings_generator_es" : "./saved_embeddings_generator_es",
+                path_saved_model = {"encoder_FG" : "./saved_encoder_FG", 
+                                    "decoder_FG" : "./saved_decoder_FG", 
+                                    "embeddings_generator_en_FG" : "./saved_embeddings_generator_en_FG",
+                                    "embeddings_generator_es_FG" : "./saved_embeddings_generator_es_FG",
                                    },
-                learning_rate =  1e-5, 
                 batch_size = 50,
                 use_gpu = True,
-                epochs = 60,
-      )
+                epochs = 40,
+              )
 
-xformer = TransformerPreLN( 
-                            dl_studio = dls,
-                            dataroot = dataroot,
-                            save_checkpoints = True,
-                            data_archive = data_archive,
-                            max_seq_length = max_seq_length,
-                            embedding_size = embedding_size,
+xformer = TransformerFG( 
+                        dl_studio = dls,
+                        dataroot = dataroot,
+                        data_archive = data_archive,
+                        max_seq_length = max_seq_length,
+                        embedding_size = embedding_size,
+                        save_checkpoints = True,
+                        num_warmup_steps = num_warmup_steps,
+                        optimizer_params = optimizer_params,
           )
 
-master_encoder = TransformerPreLN.MasterEncoder(
+master_encoder = TransformerFG.MasterEncoder(
                                   dls,
                                   xformer,
                                   num_basic_encoders = num_basic_encoders,
                                   num_atten_heads = num_atten_heads,
                  )    
 
 
-master_decoder = TransformerPreLN.MasterDecoderWithMasking(
+master_decoder = TransformerFG.MasterDecoderWithMasking(
                                   dls,
                                   xformer, 
                                   num_basic_decoders = num_basic_decoders,
                                   num_atten_heads = num_atten_heads,
-                                  masking = masking,
+                                  masking = masking
                  )
 
 
 number_of_learnable_params_in_encoder = sum(p.numel() for p in master_encoder.parameters() if p.requires_grad)
 print("\n\nThe number of learnable parameters in the Master Encoder: %d" % number_of_learnable_params_in_encoder)
 num_layers_encoder = len(list(master_encoder.parameters()))
 print("\nThe number of layers in the Master Encoder: %d\n\n" % num_layers_encoder)
 
 number_of_learnable_params_in_decoder = sum(p.numel() for p in master_decoder.parameters() if p.requires_grad)
 print("\n\nThe number of learnable parameters in the Master Decoder: %d" % number_of_learnable_params_in_decoder)
 num_layers_decoder = len(list(master_decoder.parameters()))
 print("\nThe number of layers in the Master Decoder: %d\n\n" % num_layers_decoder)
 
 if masking:
-    xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
-                                                                        checkpoints_dir="checkpoints_with_masking_PreLN")
+    xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
+                                                                                     checkpoints_dir="checkpoints_with_masking_FG")
 else:
-    xformer.run_code_for_training_TransformerPreLN(dls,master_encoder,master_decoder,display_train_loss=True,
-                                                                        checkpoints_dir="checkpoints_no_masking_PreLN")
+    xformer.run_code_for_training_TransformerFG(dls,master_encoder,master_decoder,display_train_loss=True,
+                                                                                        checkpoints_dir="checkpoints_no_masking_FG")
 
 #import pymsgbox
 #response = pymsgbox.confirm("Finished training.  Start evaluation?")
-#if response == "OK": 
-
-xformer.run_code_for_evaluating_TransformerPreLN(master_encoder, master_decoder)
 
+#if response == "OK": 
+xformer.run_code_for_evaluating_TransformerFG(master_encoder, master_decoder, 'myoutput.txt')
```

### Comparing `DLStudio-2.4.8/ExamplesTransformers/test_checkpoint_for_visTransformer.py` & `DLStudio-2.4.9/ExamplesTransformers/test_checkpoint_for_visTransformer.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/ExamplesTransformers/upgrade_model.py` & `DLStudio-2.4.9/ExamplesTransformers/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/GenerativeDiffusion/GenerativeDiffusion.py` & `DLStudio-2.4.9/GenerativeDiffusion/GenerativeDiffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__  =  '''
 
-You are looking at the GenerativeDiffusion co-class file in the DLStudio platform.
+You are looking at the GenerativeDiffusion module file in the DLStudio platform.
 For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
                          ************************
```

### Comparing `DLStudio-2.4.8/GenerativeDiffusion/__init__.py` & `DLStudio-2.4.9/GenerativeDiffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/MANIFEST.in` & `DLStudio-2.4.9/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 include MetricLearning/MetricLearning.py
 include MetricLearning/__init__.py
 GenerativeDiffusion/GenerativeDiffusion.py
 GenerativeDiffusion/__init__.py
 include setup.py
 include Makefile
 include README
-include DLStudio-2.4.8.html
+include DLStudio-2.4.9.html
 include TestDLStudio/DLStudio.py
 include TestDLStudio/TestInstanceCreation.py
 include TestDLStudio/Test.py
 include Examples/README
 include Examples/playing_with_reconfig.py
 include Examples/playing_with_sequential.py
 include Examples/playing_with_cifar10.py
```

### Comparing `DLStudio-2.4.8/Makefile` & `DLStudio-2.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/MetricLearning/MetricLearning.py` & `DLStudio-2.4.9/MetricLearning/MetricLearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
   You are looking at the MetricLearning module file in the DLStudio platform.
```

### Comparing `DLStudio-2.4.8/MetricLearning/__init__.py` & `DLStudio-2.4.9/MetricLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/PKG-INFO` & `DLStudio-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DLStudio
-Version: 2.4.8
+Version: 2.4.9
 Summary: A PyTorch based software platform for teaching the Deep Learning class at Purdue University
-Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
+Home-page: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
 Maintainer: Avinash Kak
 Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz
+Download-URL: https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.tar.gz
 Keywords: PyTorch programming
 Platform: All platforms
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.10
 
 
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

### Comparing `DLStudio-2.4.8/README` & `DLStudio-2.4.9/README`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Seq2SeqLearning/Seq2SeqLearning.py` & `DLStudio-2.4.9/Seq2SeqLearning/Seq2SeqLearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 
-  You are looking at the Seq2SeqLearning co-class file in the DLStudio platform.
+  You are looking at the Seq2SeqLearning module file in the DLStudio platform.
   For the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
 
 SEQUENCE-TO-SEQUENCE LEARNING WITH ATTENTION:
```

### Comparing `DLStudio-2.4.8/Seq2SeqLearning/__init__.py` & `DLStudio-2.4.9/Seq2SeqLearning/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/TestDLStudio/DLStudio.py` & `DLStudio-2.4.9/TestDLStudio/DLStudio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
-
 __doc__ = '''
 
 DLStudio.py
 
 Version: ''' + __version__ + '''
    
 Author: Avinash Kak (kak@purdue.edu)
 
 Date: ''' + __date__ + '''
 
 
 @tag_changes
 CHANGE LOG:
 
+  Version 2.4.9:
+
+    This version contains fixes for the pathname errors in the Transformers module
+    of DLStudio. The errors were related to where the models and the checkpoints
+    were supposed to be stored during training.
+
   Version 2.4.8:
 
     In this version, I have made two important changes to the Transformers module
     in DLStudio: (1) The Transformers module now includes a new class that I have
     named visTransformer that works like the famous Vision Transformer (ViT)
     proposed by Dosovitskiy et al. And (2) I have made changes to the QKV code for
     the calculation of self and cross attention in all of the Transformer classes
@@ -45,17 +50,17 @@
     GenerateNewImageSamples.py.  Other changes include minor clean-up of the main
     doc page for GenerativeDiffusion module and of a couple of the functions in
     the module.
 
   Version 2.4.2:
 
     DLStudio now includes a new module devoted to data modeling with diffusion.
-    This module, named GenerativeDiffusion, is a co-class of DLStudio.  That is,
-    GenerativeDiffusion resides at the same level of software abstraction as the
-    main DLStudio class in the platform.  See the README in the new
+    This module, named GenerativeDiffusion, is a module in the overall DLStudio 
+    platform.  The GenerativeDiffusion class resides at the same level of software 
+    abstraction as the main DLStudio class in the platform.  See the README in the
     ExamplesDiffusion directory of the distribution for how to experiment with the
     diffusion based code in DLStudio.
 
   Version 2.3.6:
 
     Gets rid of the inadvertently hardcoded value for the batch size in the
     testing part of the code for Semantic Segmentation.
@@ -159,16 +164,16 @@
     these loss functions is the script object_detection_and_localization_iou.py in
     the Examples directory of DLStudio.
 
   Version 2.2.2:
 
     This version of DLStudio presents my implementation of transformers in deep
     learning. You will find two transformer implementations in the Transformers
-    co-class of DLStudio in the distribution directory: TransformerFG and
-    TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
+    module of the DLStudio platform in the distribution directory: TransformerFG 
+    and TransformerPreLN.  "FG" in TransformerFG stands for "Transformer First
     Generation"; it is my implementation of the architecture presented originally
     in the seminal paper "Attention is All You Need" by Vaswani et el.  And the
     second, TransformerPreLN ("PreLN" stands for "Pre Layer Norm") is a small but
     important modification of the original idea that is based on the paper "On
     Layer Normalization in the Transformer Architecture" by Xiong et al.  I could
     have easily combined the two implementations with a small number of
     conditional statements to account for the differences, however I have chosen
@@ -182,22 +187,22 @@
     components of a transformer for educational purposes.  As things stand, these
     versions contain features that did not make into the public release version
     2.2.2 on account of inadequate testing.  I may include those features in
     versions of DLStudio after 2.2.2.
 
   Version 2.1.6:
 
-    All the changes are confined to the DataPrediction co-class of the DLStudio
-    module.  After posting the previous version, I noticed that the quality of the
-    code in DataPrediction was not up to par.  The new version presents a
+    All the changes are confined to the DataPrediction module in the DLStudio
+    platform.  After posting the previous version, I noticed that the quality of 
+    the code in DataPrediction was not up to par.  The new version presents a
     cleaned-up version of the DataPrediction class.
 
   Version 2.1.5:
 
-    DLStudio has now been equipped with a new co-class named DataPrediction whose
+    DLStudio has now been equipped with a new module named DataPrediction whose
     focus is solely on solving data prediction problems for time-series data.  A
     time-series consists of a sequence of observations recorded at regular
     intervals.  These could, for example, be the price of a stock share recorded
     every hour; the hourly recordings of electrical load at your local power
     utility company; the mean average temperature recorded on an annual basis; and
     so on.  We want to use the past observations to predict the value of the next
     one.  While data prediction has much in common with other forms of sequence
@@ -235,16 +240,16 @@
     classes AdversarialNetworks and Seq2SeqNetworks to AdversarialLearning and
     Seq2SeqLearning, respectively.
 
   Version 2.1.0:
 
     I have reorganized the code base a bit to make it easier for DLStudio to grow
     in the future.  This I did by moving the sequence-to-sequence learning
-    (seq2seq) code to a separate co-class of the main DLStudio class.  The name of
-    the new class is Seq2SeqLearning and it resides at the top level of the
+    (seq2seq) code to a separate module of the DLStudio platform.  The name of
+    the new module is Seq2SeqLearning and it resides at the top level of the
     distribution.
 
   Version 2.0.9:
 
     With this version, DLStudio comes with educational material on
     sequence-to-sequence learning (seq2seq). To that end, I have included the
     following two new classes in DLStudio: (1) Seq2SeqWithLearnableEmbeddings for
@@ -434,32 +439,33 @@
     key features of neural network architectures.  These implementations, along
     with their explanations through detailed slide presentations at our Deep
     Learning class website at Purdue, result in an educational framework that is
     much more efficient in what it can deliver within the time constraints of a
     single semester.
 
     DLStudio facilitates learning through a combination of inner classes of the
-    main module class --- called DLStudio naturally --- and several co-classes of
-    the main class that deal with adversarial learning, sequence-to-sequence
-    learning, data prediction, text analysis, and transformers.
+    main module class --- called DLStudio naturally --- and several modules of
+    the overall platform.  These modules deal with Adversarial Learning, 
+    Sequence-to-Sequence Learning, Diffusion, Data Prediction, Text Analysis, 
+    and Transformers.
 
     For the most part, the common code that you'd need in different scenarios for
     using neural networks has been placed inside the definition of the main
     DLStudio class in a file named DLStudio.py in the distribution.  That makes
     more compact the definition of the other inner classes within DLStudio. And,
     to a certain extent, that also results in a bit more compact code in the
-    co-classes of DLStudio.
+    different modules in the DLStudio platform.
 
 @tag2_skip
     SKIP CONNECTIONS:
 
     You can use DLStudio's inner class BMEnet to experiment with connection
     skipping in a deep network. Connection skipping means to provide shortcuts in
     a computational graph around the commonly used network components like
-    convolutional and other types of layers.  In the absence of such shortcuits,
+    convolutional and other types of layers.  In the absence of such shortcuts,
     deep networks suffer from the problem of vanishing gradients that degrades
     their performance.  Vanishing gradients means that the gradients of the loss
     calculated in the early layers of a network become increasingly muted as the
     network becomes deeper.  An important mitigation strategy for addressing this
     problem consists of creating a CNN using blocks with skip connections.
 
     As shown in the script playing_with_skip_connections.py in the Examples
@@ -669,15 +675,15 @@
     The pre-trained word2vec embeddings used in these scripts are accessed
     through the popular gensim library.
 
 
 @tag2_adversarial
     DATA MODELING WITH ADVERSARIAL LEARNING:
 
-    Starting with version 2.0.3, DLStudio includes a separate co-class named
+    Starting with version 2.0.3, DLStudio includes a separate module named
     AdversarialLearning for experimenting with different adversarial learning
     approaches for data modeling.  Adversarial Learning consists of simultaneously
     training a Generator and a Discriminator (or, a Generator and a Critic) with
     the goal of getting the Generator to produce from pure noise images that look
     like those in the training dataset.  When Generator-Discriminator pairs are
     used, the Discriminator's job is to become an expert at recognizing the
     training images so it can let us know when the generator produces an image
@@ -770,15 +776,15 @@
     options shown in the scripts) are included in a subdirectory named
     RVLCloud_based_results.
 
 
 @tag2_diffusion
     DATA MODELING WITH DIFFUSION:
 
-    Starting with Version 2.4.2, DLStudio includes a co-class named
+    Starting with Version 2.4.2, DLStudio includes a new module named
     GenerativeDiffusion for experimenting with what's known as "Denoising
     Diffusion".  The Denoising Diffusion approach to data modeling is based on the
     interaction between two Markov Chains: A forward chain called the q-chain and
     a reverse chain called the p-chain.  Both chains operate concurrently as
     follows and involved T timesteps where the value of T is a user-specified
     parameter.
 
@@ -873,17 +879,16 @@
 
     Sequence-to-sequence learning (seq2seq) is about predicting an outcome
     sequence from a causation sequence, or, said another way, a target sequence
     from a source sequence.  Automatic machine translation is probably one of the
     most popular applications of seq2seq.  DLStudio uses English-to-Spanish
     translation to illustrate the programming idioms and the PyTorch structures
     you need for seq2seq.  To that end, Version 2.1.0 of DLStudio includes a
-    co-class (meaning a class that resides at the top level in the distribution)
-    named Seq2SeqLearning that consists of the following two demonstration
-    classes:
+    new module named Seq2SeqLearning that consists of the following two 
+    demonstration classes:
 
         1.  Seq2SeqWithLearnableEmbeddings
 
         2.  Seq2SeqWithPretrainedEmbeddings
 
     As their names imply, the first is for seq2seq with learnable embeddings and
     the second for seq2seq with pre-trained embeddings like word2vec or fasttext.
@@ -929,16 +934,16 @@
     DATA PREDICTION
 
     Let's say you have a sequence of observations recorded at regular intervals.
     These could, for example, be the price of a stock share recorded every hour;
     the hourly recordings of electrical load at your local power utility company;
     the mean average temperature recorded on an annual basis; and so on.  We want
     to use the past observations to predict the value of the next one.  Solving
-    these types of problems is the focus of the DataPrediction co-class of
-    DLStudio.
+    these types of problems is the focus of the DataPrediction module in the
+    DLStudio platform.
 
     As a problem, data prediction has much in common with text analytics and
     seq2seq processing, in the sense that the prediction at the next time instant
     must be based on the previous observations in a manner similar to what we do
     in text analytics where the next word is understood taking into account all
     the previous words in a sentence.  However, there are three significant
     differences between purely numerical data prediction problems and text-based
@@ -998,15 +1003,15 @@
     the Reset gates of a regular GRU into a single gate called the Forget Gate.
     You could say that pmGRU is a lightweight version of a regular GRU and its use
     may therefore lead to a slight loss of accuracy in the predictions.  You will
     find it educational to compare the performance you get with my pmGRU-based
     implementation with an implementation that uses PyTorch's GRU for the same
     dataset.
 
-    Your main entry point for experimenting with the DataPrediction co-class is
+    Your main entry point for experimenting with the DataPrediction module is
     the following script in the ExamplesDataPrediction directory of the DLStudio
     distribution:
 
         power_load_prediction_with_pmGRU.py
 
     Before you can run this script, you would need to download the training
     dataset used in this example.  See the "For Data Prediction" part of the "The
@@ -1046,15 +1051,15 @@
     part of the logic in a visTransformer is identical to what it is in a
     transformer class for Seq2SeqLearning learning.  That logic kicks in after you
     have divided an image into patches and you represent each patch by an
     embedding vector --- in exactly the same as when you represent a word or a
     token in a sentence by an embedding vector.
 
     You will see three different implementations of the transformer architecture in
-    the Transformers co-class of DLStudio:
+    the Transformers module of the DLStudio platform:
 
           TransformerFG
 
           TransformerPreLN
 
           visTransformer
 
@@ -1066,15 +1071,15 @@
     the famous paper by Vaswani et al.  and TransformerPreLN my implementation of
     the same architecture but with the modification suggested by Xiong et al. for
     more stable learning.  Since, the modification is small from an architectural
     standpoint, I could have combined both transformer types in the same
     implementation with some conditional logic to account for the differences.
     However, I have chosen to keep them separate mostly for educational purposes.
     Further details on these implementations are in the documentation blocks in
-    the Transformers co-class.  
+    the Transformers module.
 
     The visTransformer implementation is based on the paper "An Image is Worth
     16x16 Words: Transformers for Image Recognition at Scale'' by Dosovitskiy et
     al.
  
     If you want to use my code for learning the main ideas related to how to
     create purely attention based networks, your starting point for that should be
@@ -1393,17 +1398,16 @@
 
 
 @tag_inner_classes
 THE MAIN INNER CLASSES OF THE DLStudio CLASS:
 
     By "inner classes" I mean the classes that are defined within the class file
     DLStudio.py in the DLStudio directory of the distribution.  The DLStudio
-    platform also includes what I have referred to as the Co-Classes in the next
-    section.  A Co-Class resides at the same level of abstraction as the main
-    DLStudio class defined in the DLStudio.py file.
+    platform also includes several modules that reside at the same level of 
+    software abstraction as the main DLStudio class defined in the DLStudio.py file.
 
     The purpose of the following two inner classes is to demonstrate how you can
     create a custom class for your own network and test it within the framework
     provided by DLStudio.
 
     (1)  class ExperimentsWithSequential
 
@@ -1498,24 +1502,25 @@
          this inner class uses the pre-trained 300-element word2vec embeddings as
          made available by Google for 3 million words and phrases drawn from the
          Google News dataset. In DLStudio, we access these embeddings through the
          popular gensim library.
 
 
 @tag_coclasses
-CO-CLASSES IN THE DLStudio PLATFORM:
+MODULES IN THE DLStudio PLATFORM:
 
-    As stated at the beginning of the previous section, a Co-Class resides at the
-    same level of abstraction in the distribution directory as the main DLStudio
-    platform. Each Co-Class is defined in a separate subdirectory at the top level
-    of the distribution directory.  While the main DLStudio class is defined in a
-    subdirectory of the same name, the other subdirectories that contain
-    definitions for the co-classes are named AdversarialLearning, Seq2SeqLearning,
-    DataPrediction, Transformers, and MetricLearning.  What follows in this
-    section are additional details regarding these co-classes:
+    As stated at the beginning of the previous section, a module resides at the
+    same level of software abstraction in the distribution directory as the main
+    DLStudio class in the platform. Each module is defined in a separate
+    subdirectory at the top level of the distribution directory.  While the main
+    DLStudio class is defined in a subdirectory of the same name, the other
+    subdirectories that contain the definitions for the modules are named
+    AdversarialLearning, Seq2SeqLearning, DataPrediction, Transformers,
+    GenerativeDiffusion, and MetricLearning.  What follows in this section are
+    additional details regarding these co-classes:
 
 
 @tag_coclass1
     ===================
     AdversarialLearning:
     ===================
 
@@ -1571,15 +1576,15 @@
     The former is called the q-chain and the latter the p-chain.  The incremental
     diffusion in the q-chain is with known amount of Gaussian isotropic noise.  In
     the p-chain, on the other hand, the goal is for a neural network to learn from
     the diffusion carried out in the q-chain how to carry out a denoising
     operation that would amount to a reversal of that diffusion.
 
     All of the key elements of the code that I have presented in the
-    GenerativeDiffusion co-class are extracted from OpenAI's "Improved Diffusion"
+    GenerativeDiffusion module are extracted from OpenAI's "Improved Diffusion"
     project at GitHub that presents a PyTorch implementation of the work authored
     by Nichol and Dhariwal in their very famous paper "Improved Denoising
     Diffusion Probabilistic Models". See the beginning part of the doc page for
     the GenerativeDiffusion module for URLs to the GitHub code and their
     publication.
 
     If you want to play with the code in GenerativeDiffusion, your starting point
@@ -1611,15 +1616,15 @@
     your overall network learn on its own what are known as vector embeddings for
     the words; or (2) Use pre-trained embeddings as provided by word2vec or
     Fasttext.
 
     After you have resolved the issue of word representation, your next challenge
     is how to implement the attention mechanism that you're going to need for
     aligning the similar grammatical units in the two languages. The seq2seq code
-    demonstrated in this co-class uses the attention model proposed by Bahdanau,
+    demonstrated in this module uses the attention model proposed by Bahdanau,
     Cho, and Bengio in the form of a separate Attention class.  The name of this
     attention class is Attention_BCB.  In a separate attention class named
     Attention_SR, I have also included the attention mechanism used by Sean
     Robertson in his very popular NLP tutorial at the main PyTorch website.
 
     Seq2SeqLearning contains the following two inner classes for illustrating
     seq2seq:
@@ -1707,15 +1712,15 @@
     TransformerPreLN is my implementation of the original idea along with the
     modifications suggested by Xiong et al. in their paper "On Layer Normalization
     in the Transformer Architecture" for more stable learning.  The two versions
     of transformers differ in only one respect: The placement of the LayerNorm in
     relation to the architectural components related to attention and the
     feedforward network.  Literally, the difference is small, yet its consequences
     are significant regarding the stability of learning.  Finally, visTransformer
-    is my implementation of the Vision Transformer as presented in the famou paper
+    is my implementation of the Vision Transformer as presented in the famous paper
     "An Image is Worth 16x16$ Words: Transformers for Image Recognition at Scale''
     by Dosovitskiy et al.
 
     The fundamentals of how the attention works in all three transformer based
     implementations in the Transformers module are exactly the same.  For
     self-attention, you associate a Query Vector Q_i and a Key Vector K_i with
     each word w_i in a sentence.  For a given w_i, the dot product of its Q_i with
@@ -1830,15 +1835,15 @@
     triplets (i,j,k) in which two indices are the same.  If B is the batch size,
     this is easily done by first forming a BxB array that is the logical negation
     of a Boolean array of the same size whose True values are only on the
     diagonal.  We can reshape this BxB Boolean array into three BxBxB shaped
     Boolean arrays, the first in which the True values exist only where i and j
     values are not the same, the second in which the True values occur only when i
     and k index values are not the same, and the third that has True values only
-    when the j and k index values are not the same.  By taking a logial AND of all
+    when the j and k index values are not the same.  By taking a logical AND of all
     three BxBxB Boolean arrays, we get the result we want.  Next, we construct a
     BxBxB Boolean tensor in which the True values occur only where the first two
     index values imply that their corresponding labels are identical and where the
     last index corresponds to a label that does not agree with that for the first
     two index values.
 
     Even after you have formed the triplets, your next mini-challenge is to
@@ -1868,15 +1873,15 @@
 Examples DIRECTORY:
 
     The Examples subdirectory in the distribution contains the following scripts:
 
     (1)  playing_with_reconfig.py
 
          Shows how you can specify a convolution network with a configuration
-         string.  The DLStudio module parses the string constructs the network.
+         string.  The main DLStudio class parses the string constructs the network.
 
     (2)  playing_with_sequential.py
 
          Shows you how you can call on a custom inner class of the 'DLStudio'
          module that is meant to experiment with your own network.  The name of
          the inner class in this example script is ExperimentsWithSequential
 
@@ -1895,22 +1900,22 @@
          directly illustrate in a classroom setting the improvement you can get
          with skip connections.  And by giving an appropriate value to the "depth"
          option, you can show results for networks of different depths.
 
     (6)  custom_data_loading.py
 
          This script shows how to use the custom dataloader in the inner class
-         CustomDataLoading of the DLStudio module.  That custom dataloader is
+         CustomDataLoading of the main DLStudio class.  That custom dataloader is
          meant specifically for the PurdueShapes5 dataset that is used in object
          detection and localization experiments in DLStudio.
 
     (7)  object_detection_and_localization.py
 
          This script shows how you can use the functionality provided by the inner
-         class DetectAndLocalize of the DLStudio module for experimenting with
+         class DetectAndLocalize of the main DLStudio class for experimenting with
          object detection and localization.  Detecting and localizing (D&L)
          objects in images is a more difficult problem than just classifying the
          objects.  D&L requires that your CNN make two different types of
          inferences simultaneously, one for classification and the other for
          localization.  For the localization part, the CNN must carry out what is
          known as regression. What that means is that the CNN must output the
          numerical values for the bounding box that encloses the object that was
@@ -2075,23 +2080,23 @@
          is explained in the main comment doc associated with the class
          Seq2SeqWithPretrainedEmbeddings.
 
 
 @tag_examples_predict
 ExamplesDataPrediction DIRECTORY:
 
-    The ExampsleDataPrediction directory of the distribution contains the
+    The ExamplesDataPrediction directory of the distribution contains the
     following script for demonstrating data prediction for time-series data:
 
         power_load_prediction_with_pmGRU.py
 
     This script uses a subset of the dataset provided by Kaggle for one of their
     machine learning competitions.  The dataset consists of over 10-years worth of
     hourly electric load recordings made available by several utilities in the
-    east and the midwest of the United States.  You can download this dataset from
+    east and the Midwest of the United States.  You can download this dataset from
     a link at the top of the main DLStudio doc page.
 
 
 @tag_examples_xform
 ExamplesTransformers DIRECTORY:
 
     The ExamplesTransformers directory of the distribution contains the following
@@ -2101,16 +2106,16 @@
         seq2seq_with_transformerPreLN.py         
 
         image_recog_with_visTransformer.py
         test_checkpoint_for_visTransformer.py 
 
 
     The first two scripts deal with English-to-Spanish translation in a manner
-    similar to what's demonstrated by the code in the Seq2SeqLearning co-class and
-    the example scripts associated with that co-class. The last two relate to my
+    similar to what's demonstrated by the code in the Seq2SeqLearning module and
+    the example scripts associated with that module. The last two relate to my
     demonstration of image recognition with a transformer based implementation.  I
     have used the CFAR10 dataset for image recognition.
 
 
 @tag_examples_metric
 ExamplesMetricLearning DIRECTORY:
 
@@ -2130,15 +2135,15 @@
 
 @tag_datasets
 THE DATASETS INCLUDED: 
 
     [must be downloaded separately]
 
 @tag2_main_dlstudio
-    FOR THE MAIN DLStudio MODULE:
+    FOR THE MAIN DLStudio CLASS and its INNER CLASSES:
 
         Download the dataset archive 'datasets_for_DLStudio.tar.gz' through the
         link "Download the image datasets for the main DLStudio Class" provided at
         the top of this documentation page and store it in the 'Example' directory
         of the distribution.  Subsequently, execute the following command in the
         'Examples' directory:
     
@@ -2364,15 +2369,15 @@
         That will create a 'data' subdirectory in the ExamplesTransformers
         directory and deposit in that subdirectory the following archives
 
             en_es_xformer_8_10000.tar.gz
             en_es_xformer_8_90000.tar.gz
 
         These are both derived from the same data source as in the dataset for the
-        examples associated with the Seq2SeqLearning co-class.  The first has only
+        examples associated with the Seq2SeqLearning module.  The first has only
         10,000 pars of English-Spanish sentences and meant primarily for debugging
         purposes.  The second contains 90000 pairs of such sentences.  The number
         '8' in the dataset names means that no sentence contains more than 8 real
         words.  With the "SOS" and "EOS" tokens used as sentence delimiters, the
         maximum number of words in each sentence in either language is 10.
 
 
@@ -2407,15 +2412,15 @@
     Version 2.2.2: My laboratory's (RVL) journey into the world of transformers
     began with a series of lab seminars by Constantine Roros and Rahul Deshmukh.
     Several subsequent conversations with them were instrumental in helping me
     improve the understanding I had gained from the seminars.  Additional
     conversations with Rahul about the issue of masking were important to how I
     eventually implemented those ideas in my code.
 
-    Rahul Deshmukh discovered the reason as to why my implmentation of the skip
+    Rahul Deshmukh discovered the reason as to why my implementation of the skip
     connection code was not working with the more recent versions of PyTorch.  My
     problem was using in-place operations in the forward() of the networks that
     called for connection skipping. This led to the release of Version 2.3.3 of
     DLStudio.
 
     The main reason for Version 2.3.4 was my new design for the SkipBlock class
     and also my easier-to-understand code for the BMEnet class that showcases the
@@ -2424,15 +2429,15 @@
     Cheng-Hao Chen reported that when a SkipBlock was asked to change the channels
     from its input to its output but without downsampling the input, that elicited
     an error from the system.  Cheng-Hao also provided a correction for the error.
     Thanks, Cheng-Hao!
 
     Aditya Chauhan proved to be a great sounding board in my journey into the land
     of diffusion that led to Version 2.4.2.  I particularly appreciated Aditya's
-    help in understanding how the attention mechanism worked in the OpanAI code
+    help in understanding how the attention mechanism worked in the OpenAI code
     library at GitHub.  Aditya is working for his PhD in RVL.  Thanks, Aditya!
 
 
 @tag_about_the_author
 ABOUT THE AUTHOR:
 
     The author, Avinash Kak, is a professor of Electrical and Computer Engineering
@@ -3261,16 +3266,16 @@
         designing a custom data loader.  Ordinarily, if the basic format of how the dataset
         is stored is similar to one of the datasets that the Torchvision module knows about,
         you can go ahead and use that for your own dataset.  At worst, you may need to carry
         out some light customizations depending on the number of classes involved, etc.
 
         However, if the underlying dataset is stored in a manner that does not look like
         anything in Torchvision, you have no choice but to supply yourself all of the data
-        loading infrastructure.  That is what this inner class of the DLStudio module is all
-        about.
+        loading infrastructure.  That is what this inner class of the main DLStudio class 
+        is all about.
 
         The custom data loading exercise here is related to a dataset called PurdueShapes5
         that contains 32x32 images of binary shapes belonging to the following five classes:
 
                        1.  rectangle
                        2.  triangle
                        3.  disk
@@ -4484,15 +4489,15 @@
 
     ###%%%
     ########################################################################################
     ##################  Start Definition of Inner Class SemanticSegmentation  ##############
 
     class SemanticSegmentation(nn.Module):             
         """
-        The purpose of this inner class is to be able to use the DLStudio module for
+        The purpose of this inner class is to be able to use the DLStudio platform for
         experiments with semantic segmentation.  At its simplest level, the purpose of
         semantic segmentation is to assign correct labels to the different objects in a
         scene, while localizing them at the same time.  At a more sophisticated level, a
         system that carries out semantic segmentation should also output a symbolic
         expression based on the objects found in the image and their spatial relationships
         with one another.
 
@@ -5054,15 +5059,15 @@
 
     ###%%%
     ########################################################################################
     ##################  Start Definition of Inner Class TextClassification  ################
 
     class TextClassification(nn.Module):             
         """
-        The purpose of this inner class is to be able to use the DLStudio module for simple 
+        The purpose of this inner class is to be able to use the DLStudio platform for simple 
         experiments in text classification.  Consider, for example, the problem of automatic 
         classification of variable-length user feedback: you want to create a neural network
         that can label an uploaded product review of arbitrary length as positive or negative.  
         One way to solve this problem is with a recurrent neural network in which you use a 
         hidden state for characterizing a variable-length product review with a fixed-length 
         state vector.  This inner class allows you to carry out such experiments.
```

### Comparing `DLStudio-2.4.8/TestDLStudio/Test.py` & `DLStudio-2.4.9/TestDLStudio/Test.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/TestDLStudio/TestInstanceCreation.py` & `DLStudio-2.4.9/TestDLStudio/TestInstanceCreation.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/Transformers/Transformers.py` & `DLStudio-2.4.9/Transformers/Transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-__version__   = '2.4.8'
+__version__   = '2.4.9'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2024-April-27'                   
-__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html'
+__date__      = '2024-May-1'                   
+__url__       = 'https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html'
 __copyright__ = "(C) 2024 Avinash Kak. Python Software Foundation."
 
 
 
 __doc__ = '''
 
 
-  You are looking at the Transformers co-class file in the DLStudio platform.  For
+  You are looking at the Transformers module file in the DLStudio platform.  For
   the overall documentation on DLStudio, visit:
 
            https://engineering.purdue.edu/kak/distDLS/
 
 
 
 TRANSFORMERS:
@@ -247,16 +247,16 @@
         self.training_corpus  = list(dataset.values())
         self.vocab_en = vocab_en
         self.vocab_es = vocab_es
         self.vocab_en_size = len(vocab_en)          #  includes the SOS and EOS tokens
         self.vocab_es_size = len(vocab_es)          #  includes the SOS and EOS tokens
         print("\n\nSize of the English vocab in the dataset: ", self.vocab_en_size)
         print("\nSize of the Spanish vocab in the dataset: ", self.vocab_es_size)
-        self.debug = False
-        if self.debug:
+        debug = False
+        if debug:
             print("\n\nFirst 100 elements of English vocab: ", vocab_en[:100])
             print("\n\nFirst 100 elements of Spanish vocab: ", vocab_es[:100])
         # The first two elements of both vocab_en and vocab_es are the SOS and EOS tokens
         # So the index position for SOS is 0 and for EOS is 1.
         self.en_vocab_dict = { vocab_en[i] : i  for i in range(self.vocab_en_size) }  
         self.es_vocab_dict = { vocab_es[i] : i  for i in range(self.vocab_es_size) }
         self.es_index_2_word =   { i : vocab_es[i] for i in range(self.vocab_es_size) }
@@ -846,39 +846,41 @@
 
 
     ###%%%
     ##############################  Training and Evaluation for TransformerFG  ########################################
 
     def save_encoder(self, encoder):
         "Save the trained encoder to a disk file"       
-        torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder"])
+        torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder_FG"])
 
     def save_decoder(self, decoder):
         "Save the trained decoder to a disk file"       
-        torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder"])
+        torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder_FG"])
 
     def save_embeddings_generator_en(self, embeddings_generator_en):
-        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en"])
+        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en_FG"])
 
     def save_embeddings_generator_es(self, embeddings_generator_es):
-        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es"])
+        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es_FG"])
 
     def save_checkpoint_encoder(self, encoder, dir_name, epoch_index):
         "Save the encoder checkpoint"       
-        # if os.path.exists(dir_name + "/encoder_" + str(epoch_index - 1)):              
-        #    os.remove(dir_name + "/encoder_" + str(epoch_index - 1))
-        torch.save(encoder.state_dict(), dir_name + "/encoder_" + str(epoch_index))
+        torch.save(encoder.state_dict(), dir_name + "/encoder_FG_" + str(epoch_index))
 
     def save_checkpoint_decoder(self, decoder, dir_name, epoch_index):
         "Save the decoder checkpoint"       
-        # if os.path.exists(dir_name + "/decoder_" + str(epoch_index - 1)):              
-        #    os.remove(dir_name + "/decoder_" + str(epoch_index - 1))
-        torch.save(decoder.state_dict(), dir_name + "/decoder_" + str(epoch_index))
-
+        torch.save(decoder.state_dict(), dir_name + "/decoder_FG_" + str(epoch_index))
 
+    def save_checkpoint_embeddings_generator_en(self, embeddings_generator_en, dir_name, epoch_index):
+        "save checkpoint for the embeddings_generator_en"
+        torch.save(embeddings_generator_en.state_dict(), dir_name + "/embeddings_generator_en_FG_" + str(epoch_index))        
+
+    def save_checkpoint_embeddings_generator_es(self, embeddings_generator_es, dir_name, epoch_index):
+        "save checkpoint for the embeddings_generator_es"
+        torch.save(embeddings_generator_es.state_dict(), dir_name + "/embeddings_generator_es_FG_" + str(epoch_index))        
 
 
     def run_code_for_training_TransformerFG(self, dls, master_encoder, master_decoder, display_train_loss=False, 
                                                                                                 checkpoints_dir='checkpoints'):
         """
         A particular feature of TransformerFG is how it is trained. Training a transformer as 
         conceptualized in the paper by Vaswani et al. requires a carefully designed warm-up stage 
@@ -928,14 +930,18 @@
                 if os.path.isfile(file): 
                     os.remove(file) 
                 else: 
                     files = glob.glob(file + "/*") 
                     list(map(lambda x: os.remove(x), files)) 
         else: 
             os.mkdir(checkpoints_dir)   
+        saved_files = glob.glob("saved*")
+        for file in saved_files:                                                                                                 
+            if os.path.isfile(file):                                                                                       
+                os.remove(file)  
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
         beta1,beta2,epsilon = self.optimizer_params['beta1'], self.optimizer_params['beta2'], \
                                                                                        self.optimizer_params['epsilon']     
         master_encoder_optimizer = self.ScheduledOptim(optim.Adam(master_encoder.parameters(), betas=(beta1,beta2), eps=epsilon),  
@@ -943,43 +949,43 @@
         master_decoder_optimizer = self.ScheduledOptim(optim.Adam(master_decoder.parameters(), betas=(beta1,beta2), eps=epsilon),
                                             lr_mul=2, d_model=self.embedding_size, n_warmup_steps=self.num_warmup_steps)     ## (B)
         ##  Note that by default, nn.NLLLoss averages over the instances in a batch
         criterion = nn.NLLLoss()                                                                                             ## (C)
         accum_times = []
         start_time = time.perf_counter()
         training_loss_tally = []
-        self.debug = False
         print("")
         num_sentence_pairs = len(self.training_corpus)
         print("\n\nNumber of sentence pairs in the dataset: ", num_sentence_pairs)
         print("\nNo sentence is longer than %d words (including the SOS and EOS tokens)\n\n" % self.max_seq_length)
         batch_size = self.dl_studio.batch_size
         max_iters = len(self.training_corpus) // batch_size                                                                  ## (D)
         max_iters = max_iters if len(self.training_corpus) % batch_size == 0 else max_iters + 1                   
         print("\n\nMaximum number of training iterations in each epoch: %d\n\n" % max_iters)
+        debug = False
         for epoch in range(self.dl_studio.epochs):                                                                           ## (E)
             print("")
             random.shuffle(self.training_corpus)                                                                             ## (F)
             running_loss = 0.0
             for iter in range(max_iters):
-                if self.debug:
+                if debug:
                     print("\n\n\n========================== starting batch indexed: %d ================================\n\n\n" % iter)
                 if (iter+1)*batch_size <= num_sentence_pairs:                                                                ## (G)
                     batched_pairs = self.training_corpus[iter*batch_size : (iter+1)*batch_size]                              ## (H)
                 else:
                     batched_pairs = self.training_corpus[iter*batch_size : ]                                                 ## (I)
-                if self.debug:                 ##  MUST use a batch size of 5 in your script for this to work
+                if debug:                 ##  MUST use a batch size of 5 in your script for this to work
                     batched_pairs =  [['SOS i will kill him EOS', 'SOS le mataré EOS'], 
                                       ['SOS what was that EOS', 'SOS qué era eso EOS'], 
                                       ['SOS he soon left the new job EOS', 'SOS él dejó pronto el nuevo empleo EOS'], 
                                       ['SOS i go into the city every day EOS', 'SOS yo voy a la ciudad todos los días EOS'], 
                                       ['SOS she might come tomorrow EOS', 'SOS puede que ella venga mañana EOS']]
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
-                if self.debug:
+                if debug:
                     print("\n\nfirst source sentence in batch: ", source_sentences[0])
                     print("\nfirst target sentence in batch: ", target_sentences[0])
                     print("\nlast source sentence in batch: ", source_sentences[-1])
                     print("\nlast target sentence in batch: ", target_sentences[-1])
                 en_tensor =  self.sentence_with_words_to_ints(source_sentences, 'en')                                        ## (J)
                 es_tensor =  self.sentence_with_words_to_ints(target_sentences, 'es')                                        ## (K)
                 en_tensor = en_tensor.to(self.dl_studio.device)
@@ -1004,33 +1010,33 @@
                     training_loss_tally.append(avg_loss)
                     running_loss = 0.0
                     current_time = time.perf_counter()
                     time_elapsed = current_time-start_time
                     print("[epoch:%2d/%d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch+1,self.dl_studio.epochs,iter+1,time_elapsed,avg_loss)) 
                     accum_times.append(current_time-start_time)
             ##  At the beginning of the training session, the designated checkpoint_dir has already been flushed
-            if self.save_checkpoints and  (epoch + 1) % 5 == 0:
-                self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch)
-                self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch)
-                self.save_embeddings_generator_en(embeddings_generator_en, checkpoints_dir, epoch)
-                self.save_embeddings_generator_es(embeddings_generator_es, checkpoints_dir, epoch)
-                print("Checkpoint saved at the end of epoch %d" % (epoch))
+            if self.save_checkpoints and  (epoch + 1) % 20 == 0:
+                self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch+1)
+                self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch+1)
+                self.save_checkpoint_embeddings_generator_en(embeddings_generator_en, checkpoints_dir, epoch+1)
+                self.save_checkpoint_embeddings_generator_es(embeddings_generator_es, checkpoints_dir, epoch+1)
+                print("Checkpoint saved at the end of epoch %d" % (epoch+1))
         print("\nFinished Training\n")
         self.save_encoder(master_encoder)       
         self.save_decoder(master_decoder)       
         self.save_embeddings_generator_en(embeddings_generator_en)       
         self.save_embeddings_generator_es(embeddings_generator_es)       
         if display_train_loss:
             plt.figure(figsize=(10,5))
             plt.title("FG Training Loss vs. Iterations")
             plt.plot(training_loss_tally)
             plt.xlabel("iterations")
             plt.ylabel("training loss")
             plt.legend(["Plot of loss versus iterations"], fontsize="x-large")
-            plt.savefig("training_loss_FG.png")
+            plt.savefig("training_loss_FG_" +  str(self.dl_studio.epochs) + ".png")
 #            plt.show()
 
 
 
     def run_code_for_evaluating_TransformerFG(self, master_encoder, master_decoder, result_file=None):
         """
         The main difference between the training code shown in the previous function and the
@@ -1050,37 +1056,38 @@
         predicted log probabilities (logprob) over the target vocabulary for every word 
         position in the target language; and (2) for each target-language word position, 
         the word_vocab_index at which the logprob is maximum.  The loss calculation in
         the training code was based on the former.  ON the other hand, as shown in line (H)
         below, it is the latter that lets us do the the translations in the target words
         in line (I).
         """
-        master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder']))
-        master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder']))
+        master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder_FG']))
+        master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder_FG']))
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size)
-        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en']))
-        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es']))
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_FG']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_FG']))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en.to(self.dl_studio.device)
         embeddings_generator_es.to(self.dl_studio.device)        
-        self.debug = False
+        debug = False
         FILE = open("translations_with_FG_" + str(self.dl_studio.epochs) + ".txt", 'w')
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']      ## (A)
                 batched_pairs = random.sample(self.training_corpus, 1)                                                     ## (B)
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
-                if self.debug:
+                if debug:
                     print("\n\nsource sentences: ", source_sentences)
                     print("\ntarget sentences: ", target_sentences)
                 en_sent_ints =  self.sentence_with_words_to_ints(source_sentences, 'en').to(self.dl_studio.device)         ## (C)
-                if self.debug:
+                if debug:
+                    es_sent_ints =  self.sentence_with_words_to_ints(target_sentences, 'es')
                     print("\n\nsource sentence tensor: ", en_sent_ints)
                     print("\n\ntarget sentence tensor: ", es_sent_ints)
                 en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()
                 master_encoder_output = master_encoder( en_sentence_tensor )                                               ## (E)
                 starter_stub_as_ints = self.sentence_with_words_to_ints(
                                       [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device)            ## (F)
                 starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()                                ## (G)
@@ -1088,15 +1095,15 @@
                 predicted_word_index_values = predicted_word_index_values[0].unsqueeze(1)
                 decoded_words = [self.es_index_2_word[predicted_word_index_values[di].item()] 
                                                                         for di in range(self.max_seq_length)]              ## (I)
                 output_sentence = " ".join(decoded_words)                                                                 
                 print("\n\n\nThe input sentence pair: ", source_sentences, target_sentences)                             
                 print("\nThe translation produced by TransformerFG: ", output_sentence)
                 FILE.write("\n\n\nThe input sentence pair: %s    %s" % (source_sentences, target_sentences))
-                FILE.write("\nThe translation produced by TransformerPreLN:  %s" % output_sentence)
+                FILE.write("\nThe translation produced by TransformerFG:  %s" % output_sentence)
 
 
 
     def run_code_for_evaluating_checkpoint(self, master_encoder, master_decoder, checkpoints_dir, checkpoint_index, result_file=None):
         """
         Training transformer networks has always been difficulty and that's the case even with 
         learning-rate warm-up and other mitigating strategies.  DLStudio provides you with 
@@ -1122,32 +1129,34 @@
 
         where the argument "checkpoints_with_masking" is the subdiretory that has the checkpoints in
         it. The last argument "4" means that we are testing the checkpoint models "encoder_4"  and
         "decoder_4".
         """
         if result_file is not None:
             FILE = open(result_file, 'w')
-        master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_" + str(checkpoint_index) ))
-        master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_" + str(checkpoint_index) ))
+        master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_FG_" + str(checkpoint_index) ))
+        master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_FG_" + str(checkpoint_index) ))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
-        self.debug = False
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_FG_' + str(checkpoint_index)]))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_FG_' + str(checkpoint_index)]))
+        debug = False
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']      ## (A)
                 batched_pairs = random.sample(self.training_corpus, 1)                                                     ## (B)
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
-                if self.debug:
+                if debug:
                     print("\n\nsource sentences: ", source_sentences)
                     print("\ntarget sentences: ", target_sentences)
                 en_sent_ints =  self.sentence_with_words_to_ints(source_sentences, 'en').to(self.dl_studio.device)         ## (C)
-                if self.debug:
+                if debug:
                     print("\n\nsource sentence tensor: ", en_sent_ints)
                     print("\n\ntarget sentence tensor: ", es_sent_ints)
                 en_sentence_tensor = embeddings_generator_en(en_sent_ints)
                 master_encoder_output = master_encoder( en_sentence_tensor )                                               ## (E)
                 starter_stub_as_ints = self.sentence_with_words_to_ints(
                                               [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device)    ## (F)
                 starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()                                ## (G)
@@ -1194,21 +1203,23 @@
         source_sentence = [sentence]
         master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_" + str(checkpoint_index) ))
         master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_" + str(checkpoint_index) ))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
-        self.debug = False
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_FG']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_FG']))
+        debug = False
         starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']     
-        if self.debug:
+        if debug:
             print("\n\nsource sentences: ", source_sentences)
         ##  Since the user-supplied source sentence originated in CPU, we need to move the following to GPU:
         en_sent_ints =  self.sentence_with_words_to_ints(source_sentence, 'en').to(self.dl_studio.device)
-        if self.debug:
+        if debug:
             print("\n\nsource sentence tensor: ", en_sent_ints)
         en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()
         master_encoder_output = master_encoder( en_sentence_tensor )                                              
         starter_stub_as_ints = self.sentence_with_words_to_ints(
                                       [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device)   
         starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()                               
         _, predicted_word_index_values = master_decoder(starter_stub_tensor, master_encoder_output)               
@@ -1384,16 +1395,16 @@
         self.training_corpus  = list(dataset.values())
         self.vocab_en = vocab_en
         self.vocab_es = vocab_es
         self.vocab_en_size = len(vocab_en)          #  includes the SOS and EOS tokens
         self.vocab_es_size = len(vocab_es)          #  includes the SOS and EOS tokens
         print("\n\nSize of the English vocab in the dataset: ", self.vocab_en_size)
         print("\nSize of the Spanish vocab in the dataset: ", self.vocab_es_size)
-        self.debug = False
-        if self.debug:
+        debug = False
+        if debug:
             print("\n\nFirst 100 elements of English vocab: ", vocab_en[:100])
             print("\n\nFirst 100 elements of Spanish vocab: ", vocab_es[:100])
         # The first two elements of both vocab_en and vocab_es are the SOS and EOS tokens
         # So the index position for SOS is 0 and for EOS is 1.
         self.en_vocab_dict = { vocab_en[i] : i  for i in range(self.vocab_en_size) }  
         self.es_vocab_dict = { vocab_es[i] : i  for i in range(self.vocab_es_size) }
         self.es_index_2_word =   { i : vocab_es[i] for i in range(self.vocab_es_size) }
@@ -1998,37 +2009,42 @@
             return out    
 
     ###%%%
     ##############################  Training and Evaluation for TransformerPreLN  ########################################
 
     def save_encoder(self, encoder):
         "Save the trained encoder to a disk file"       
-        torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder"])
+        torch.save(encoder.state_dict(), self.dl_studio.path_saved_model["encoder_PreLN"])
 
     def save_decoder(self, decoder):
         "Save the trained decoder to a disk file"       
-        torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder"])
+        torch.save(decoder.state_dict(), self.dl_studio.path_saved_model["decoder_PreLN"])
 
     def save_embeddings_generator_en(self, embeddings_generator_en):
-        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en"])
+        torch.save(embeddings_generator_en.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_en_PreLN"])
 
     def save_embeddings_generator_es(self, embeddings_generator_es):
-        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es"])
+        torch.save(embeddings_generator_es.state_dict(), self.dl_studio.path_saved_model["embeddings_generator_es_PreLN"])
 
     def save_checkpoint_encoder(self, encoder, dir_name, epoch_index):
         "Save the encoder checkpoint"       
-        # if os.path.exists(dir_name + "/encoder_" + str(epoch_index - 1)):              
-        #    os.remove(dir_name + "/encoder_" + str(epoch_index - 1))
-        torch.save(encoder.state_dict(), dir_name + "/encoder_" + str(epoch_index))
+        torch.save(encoder.state_dict(), dir_name + "/encoder_PreLN_" + str(epoch_index))
 
     def save_checkpoint_decoder(self, decoder, dir_name, epoch_index):
         "Save the decoder checkpoint"       
-        # if os.path.exists(dir_name + "/decoder_" + str(epoch_index - 1)):              
-        #    os.remove(dir_name + "/decoder_" + str(epoch_index - 1))
-        torch.save(decoder.state_dict(), dir_name + "/decoder_" + str(epoch_index))
+        torch.save(decoder.state_dict(), dir_name + "/decoder_PreLN_" + str(epoch_index))
+
+    def save_checkpoint_embeddings_generator_en(self, embeddings_generator_en, dir_name, epoch_index):
+        "save checkpoint for the embeddings_generator_en"
+        torch.save(embeddings_generator_en.state_dict(), dir_name + "/embeddings_generator_en_PreLN_" + str(epoch_index))        
+
+    def save_checkpoint_embeddings_generator_es(self, embeddings_generator_es, dir_name, epoch_index):
+        "save checkpoint for the embeddings_generator_es"
+        torch.save(embeddings_generator_es.state_dict(), dir_name + "/embeddings_generator_es_PreLN_" + str(epoch_index))        
+
 
 
     def run_code_for_training_TransformerPreLN(self, dls, master_encoder, master_decoder, display_train_loss=False, 
                                                                                                 checkpoints_dir='checkpoints'):
         """
         Since we did not construct a dataloader by subclassing from torch.utils.data.DataLoader, we
         need the statements in Lines (A) through (G) to deal with the cases when the size of the
@@ -2065,50 +2081,54 @@
                 if os.path.isfile(file): 
                     os.remove(file) 
                 else: 
                     files = glob.glob(file + "/*") 
                     list(map(lambda x: os.remove(x), files)) 
         else: 
             os.mkdir(checkpoints_dir)   
+        saved_files = glob.glob("saved*")
+        for file in saved_files:                                                                                                 
+            if os.path.isfile(file):                                                                                       
+                os.remove(file)  
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
         master_encoder_optimizer = optim.Adam(master_encoder.parameters(), lr=self.dl_studio.learning_rate)
         master_decoder_optimizer = optim.Adam(master_decoder.parameters(), lr=self.dl_studio.learning_rate)
         ##  Note that by default, nn.NLLLoss averages over the instances in a batch
         criterion = nn.NLLLoss()                                                                                           
         accum_times = []
         start_time = time.perf_counter()
         training_loss_tally = []
-        self.debug = False
+        debug = False
         print("")
         num_sentence_pairs = len(self.training_corpus)
         print("\n\nNumber of sentence pairs in the dataset: ", num_sentence_pairs)
         print("\nNo sentence is longer than %d words (including the SOS and EOS tokens)\n\n" % self.max_seq_length)
         batch_size = self.dl_studio.batch_size
         max_iters = len(self.training_corpus) // batch_size                                                                  ## (A)
         max_iters = max_iters if len(self.training_corpus) % batch_size == 0 else max_iters + 1                              ## (B)
         print("\n\nMaximum number of training iterations in each epoch: %d\n\n" % max_iters)
         for epoch in range(self.dl_studio.epochs):                                                                           ## (C)
             print("")
             random.shuffle(self.training_corpus)                                                                             ## (D)
             running_loss = 0.0
             for iter in range(max_iters):
-                if self.debug:
+                if debug:
                     print("\n\n\n========================== starting batch indexed: %d ================================\n\n\n" % iter)
                 if (iter+1)*batch_size <= num_sentence_pairs:                                                                ## (E)
                     batched_pairs = self.training_corpus[iter*batch_size : (iter+1)*batch_size]                              ## (F)
                 else:
                     batched_pairs = self.training_corpus[iter*batch_size : ]                                                 ## (G)
-                if self.debug:                 ##  MUST use a batch size of 5 in your script for this to work
+                if debug:                 ##  MUST use a batch size of 5 in your script for this to work
                     batched_pairs =  [['SOS i will kill him EOS', 'SOS le mataré EOS'], ['SOS what was that EOS', 'SOS qué era eso EOS'], ['SOS he soon left the new job EOS', 'SOS él dejó pronto el nuevo empleo EOS'], ['SOS i go into the city every day EOS', 'SOS yo voy a la ciudad todos los días EOS'], ['SOS she might come tomorrow EOS', 'SOS puede que ella venga mañana EOS']]
                 source_sentences = [pair[0] for pair in batched_pairs]                                                       ## (H)
                 target_sentences = [pair[1] for pair in batched_pairs]                                                       ## (I)
-                if self.debug:
+                if debug:
                     print("\n\nfirst source sentence in batch: ", source_sentences[0])
                     print("\nfirst target sentence in batch: ", target_sentences[0])
                     print("\nlast source sentence in batch: ", source_sentences[-1])
                     print("\nlast target sentence in batch: ", target_sentences[-1])
                 en_sent_ints =  self.sentence_with_words_to_ints(source_sentences, 'en')                                     ## (J)
                 es_sent_ints =  self.sentence_with_words_to_ints(target_sentences, 'es')                                     ## (K)
                 en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()                                           ## (L)
@@ -2131,33 +2151,36 @@
                     training_loss_tally.append(avg_loss)
                     running_loss = 0.0
                     current_time = time.perf_counter()
                     time_elapsed = current_time-start_time
                     print("[epoch:%2d/%d  iter:%4d  elapsed_time: %4d secs]     loss: %.4f" % (epoch+1,self.dl_studio.epochs,iter+1, time_elapsed,avg_loss))
                     accum_times.append(current_time-start_time)
             ##  At the beginning of the training session, the designated checkpoint_dir has already been flushed
-            if self.save_checkpoints and  (epoch + 1) % 5 == 0:                      
+            if self.save_checkpoints and  (epoch + 1) % 20 == 0:                      
                 self.save_checkpoint_encoder(master_encoder, checkpoints_dir, epoch+1)
                 self.save_checkpoint_decoder(master_decoder, checkpoints_dir, epoch+1)
-                print("Checkpoint saved at the end of epoch %d" % (epoch))
+                self.save_checkpoint_embeddings_generator_en(embeddings_generator_en, checkpoints_dir, epoch+1)       
+                self.save_checkpoint_embeddings_generator_es(embeddings_generator_es, checkpoints_dir, epoch+1)       
+                print("Checkpoint saved at the end of epoch %d" % (epoch+1))
         print("\nFinished Training\n")
         self.save_encoder(master_encoder)       
         self.save_decoder(master_decoder)       
         self.save_embeddings_generator_en(embeddings_generator_en)       
         self.save_embeddings_generator_es(embeddings_generator_es)       
         if display_train_loss:
             plt.figure(figsize=(10,5))
             plt.title("PreLN Training Loss vs. Iterations")
             plt.plot(training_loss_tally)
             plt.xlabel("iterations")
             plt.ylabel("training loss")
 #            plt.legend()
             plt.legend(["Plot of loss versus iterations"], fontsize="x-large")
-            plt.savefig("training_loss_PreLN.png")
-            plt.show()
+            plt.savefig("training_loss_PreLN_" +  str(self.dl_studio.epochs) + ".png")
+#            plt.show()
+
 
     def run_code_for_evaluating_TransformerPreLN(self, master_encoder, master_decoder):
         """
         The main difference between the training code shown in the previous function and the
         evaluation code shown here is with regard to the input to MasterDecoder and how we process 
         its output. As shown in the previous function, for the training loop, the input to 
         MasterDecoder consists of the both the target sentence and the output of the MasterEncoder 
@@ -2172,37 +2195,38 @@
         associated with MasterDecoder, it returns two things: (1) the predicted log probabilities 
         (logprob) over the target vocabulary for every word position in the target language; and 
         (2) for each target-language word position, the word_vocab_index at which the logprob is 
         maximum.  The loss calculation in the training code was based on the former.  ON the other 
         hand, as shown in line (H) below, it is the latter that lets us do the the translations in 
         the target words in line (I).
         """
-        master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder']))
-        master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder']))
+        master_encoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['encoder_PreLN']))
+        master_decoder.load_state_dict(torch.load(self.dl_studio.path_saved_model['decoder_PreLN']))
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size)
-        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en']))
-        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es']))
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_PreLN']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_PreLN']))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en.to(self.dl_studio.device)
         embeddings_generator_es.to(self.dl_studio.device)        
-        self.debug = False
+        debug = False
         FILE = open("translations_with_PreLN_" + str(self.dl_studio.epochs) + ".txt", 'w')
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']      ## (A)
                 batched_pairs = random.sample(self.training_corpus, 1)                                                     ## (B)
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
-                if self.debug:
+                if debug:
                     print("\n\nsource sentences: ", source_sentences)
                     print("\ntarget sentences: ", target_sentences)
                 en_sent_ints =  self.sentence_with_words_to_ints(source_sentences, 'en')                                   ## (C)
-                if self.debug:
+                if debug:
+                    es_sent_ints =  self.sentence_with_words_to_ints(target_sentences, 'es')
                     print("\n\nsource sentence tensor: ", en_sent_ints)
                     print("\n\ntarget sentence tensor: ", es_sent_ints)
                 en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()
                 master_encoder_output = master_encoder( en_sentence_tensor )                                               ## (E)
                 starter_stub_as_ints = self.sentence_with_words_to_ints(
                                               [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device)    ## (F)
                 starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()                                ## (G)
@@ -2243,32 +2267,34 @@
 
         where the argument "checkpoints_no_masking" is the subdiretory that has the checkpoints in it.
         The last argument "4" means that we are testing the checkpoint models "encoder_4"  and
         "decoder_4".
         """
         if result_file is not None:
             FILE = open(result_file, 'w')
-        master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_" + str(checkpoint_index) ))
-        master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_" + str(checkpoint_index) ))
+        master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_PreLN_" + str(checkpoint_index) ))
+        master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_PreLN_" + str(checkpoint_index) ))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
-        self.debug = False
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_PreLN_' + str(checkpoint_index)]))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_PreLN_' + str(checkpoint_index)]))
+        debug = False
         with torch.no_grad():
             for iter in range(20):
                 starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']    
                 batched_pairs = random.sample(self.training_corpus, 1)                                                   
                 source_sentences = [pair[0] for pair in batched_pairs]
                 target_sentences = [pair[1] for pair in batched_pairs]
-                if self.debug:
+                if debug:
                     print("\n\nsource sentences: ", source_sentences)
                     print("\ntarget sentences: ", target_sentences)
                 en_sent_ints =  self.sentence_with_words_to_ints(source_sentences, 'en').to(self.dl_studio.device)       
-                if self.debug:
+                if debug:
                     print("\n\nsource sentence tensor: ", en_sent_ints)
                     print("\n\ntarget sentence tensor: ", es_sent_ints)
                 en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()
                 master_encoder_output = master_encoder( en_sentence_tensor )                                             
                 starter_stub_as_ints = self.sentence_with_words_to_ints(
                                               [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device)  
                 starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()                                      
@@ -2303,21 +2329,23 @@
         source_sentence = [sentence]
         master_encoder.load_state_dict(torch.load(checkpoints_dir + "/encoder_" + str(checkpoint_index) ))
         master_decoder.load_state_dict(torch.load(checkpoints_dir + "/decoder_" + str(checkpoint_index) ))
         master_encoder.to(self.dl_studio.device)
         master_decoder.to(self.dl_studio.device)     
         embeddings_generator_en = self.EmbeddingsGenerator(self, 'en', self.embedding_size).to(self.dl_studio.device)
         embeddings_generator_es = self.EmbeddingsGenerator(self, 'es', self.embedding_size).to(self.dl_studio.device)
-        self.debug = False
+        embeddings_generator_en.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_en_PreLN']))
+        embeddings_generator_es.load_state_dict(torch.load(self.dl_studio.path_saved_model['embeddings_generator_es_PreLN']))
+        debug = False
         starter_stub_for_translation = ['SOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS', 'EOS']  
-        if self.debug:
+        if debug:
             print("\n\nsource sentences: ", source_sentences)
         ##  Since the user-supplied source sentence originated in CPU, we need to move the following to GPU:
         en_sent_ints =  self.sentence_with_words_to_ints(source_sentence, 'en').to(self.dl_studio.device)      
-        if self.debug:
+        if debug:
             print("\n\nsource sentence tensor: ", en_sent_ints)
         en_sentence_tensor = embeddings_generator_en(en_sent_ints).float()
         master_encoder_output = master_encoder( en_sentence_tensor )                                           
         starter_stub_as_ints = self.sentence_with_words_to_ints(
                                               [" ".join(starter_stub_for_translation)], 'es').to(self.dl_studio.device) 
         starter_stub_tensor = embeddings_generator_es(starter_stub_as_ints).float()
         _, predicted_word_index_values = master_decoder(starter_stub_tensor, master_encoder_output)              
@@ -2345,16 +2373,16 @@
     ClassPath:  visTransformer
     """
     def __init__(self, dl_studio, patch_size, embedding_size, num_basic_encoders, num_atten_heads, save_checkpoints=True, checkpoint_freq=10):
         super(visTransformer, self).__init__()
         self.dl_studio = dl_studio
         self.batch_size = dl_studio.batch_size
         self.learning_rate = dl_studio.learning_rate
-        self.train_data_loader =  None                       ## will be set when you call vlt.load_cifar_10_dataset()
-        self.test_data_loader = None                         ## will be set when you call vlt.load_cifar_10_dataset()
+        self.train_data_loader =  None                       ## will be set when you call vlt.load_cifar_10_dataset() in the example script
+        self.test_data_loader = None                         ## will be set when you call vlt.load_cifar_10_dataset() in the example script
         self.num_patches_in_image =  (dl_studio.image_size[0] // patch_size[0] ) * (dl_studio.image_size[1] // patch_size[1] )
         self.checkpoint_freq = checkpoint_freq
         self.patch_size  =  patch_size
         self.patch_dimen = (patch_size[0] * patch_size[1]) * 3
         self.embedding_size = embedding_size
         self.num_basic_encoders = num_basic_encoders
         self.num_atten_heads = num_atten_heads
@@ -2565,15 +2593,15 @@
         optimizer = torch.optim.Adam(vis_encoder_network.parameters(), lr = self.learning_rate, betas = (0.9, 0.99))
         patch_embedding_generator = self.PatchEmbeddingGenerator( self )
         patch_embedding_generator.to(self.dl_studio.device)
         criterion = nn.CrossEntropyLoss()                                                                                       
         accum_times = []
         start_time = time.perf_counter()
         training_loss_tally = []
-        self.debug = False
+        debug = False
         print("")
         batch_size = self.dl_studio.batch_size
         print("\n\n batch_size: ", batch_size)
         print("\n\n number of batches in the dataset: ", len(self.train_data_loader))
 
         for epoch in range(self.dl_studio.epochs):                                                              
             print("")
```

### Comparing `DLStudio-2.4.8/Transformers/__init__.py` & `DLStudio-2.4.9/Transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `DLStudio-2.4.8/setup.py` & `DLStudio-2.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 ### setup.py
 
 from setuptools import setup, find_packages
 import sys, os
 
 setup(name='DLStudio',
-      version='2.4.8',
+      version='2.4.9',
       author='Avinash Kak',
       author_email='kak@purdue.edu',
       maintainer='Avinash Kak',
       maintainer_email='kak@purdue.edu',
-      url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html',
-      download_url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.tar.gz',
+      url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html',
+      download_url='https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.tar.gz',
       description='A PyTorch based software platform for teaching the Deep Learning class at Purdue University',
       long_description='''
 
 Consult the module API page at
 
-      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.8.html
+      https://engineering.purdue.edu/kak/distDLS/DLStudio-2.4.9.html
 
 for all information related to this module, including the information about
 the latest changes to the code.  
 
 ::
 
       convo_layers_config = "1x[128,3,3,1]-MaxPool(2) 1x[16,5,5,1]-MaxPool(2)"
```

