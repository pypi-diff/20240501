# Comparing `tmp/research_framework-0.2.2.tar.gz` & `tmp/research_framework-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_framework-0.2.2.tar", last modified: Mon Apr 29 19:47:11 2024, max compression
+gzip compressed data, was "research_framework-0.2.3.tar", last modified: Wed May  1 17:36:41 2024, max compression
```

## Comparing `research_framework-0.2.2.tar` & `research_framework-0.2.3.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research_framework-0.2.2/LICENSE
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research_framework-0.2.2/MANIFEST.in
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-04-29 19:47:11.947612 research_framework-0.2.2/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      393 2024-04-10 15:04:36.000000 research_framework-0.2.2/requirements.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.939612 research_framework-0.2.2/research_framework/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       91 2023-11-07 13:43:38.000000 research_framework-0.2.2/research_framework/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1990 2023-11-09 16:51:42.000000 research_framework-0.2.2/research_framework/base/container/base_container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/container/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.2/research_framework/base/container/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      722 2023-09-19 17:54:13.000000 research_framework-0.2.2/research_framework/base/container/model/bind_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/flyweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.2/research_framework/base/flyweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1074 2023-11-08 13:26:10.000000 research_framework-0.2.2/research_framework/base/flyweight/base_flyweight.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      800 2024-04-25 16:51:06.000000 research_framework-0.2.2/research_framework/base/flyweight/base_flyweight_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2550 2024-03-02 14:06:30.000000 research_framework-0.2.2/research_framework/base/model/base_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/model/base_utils.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/pipeline/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-06 20:33:03.000000 research_framework-0.2.2/research_framework/base/pipeline/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      227 2023-12-29 14:25:32.000000 research_framework-0.2.2/research_framework/base/pipeline/base_pipeline.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/plugin/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/plugin/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1029 2023-10-15 10:47:16.000000 research_framework-0.2.2/research_framework/base/plugin/base_plugin.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      337 2024-04-25 10:02:49.000000 research_framework-0.2.2/research_framework/base/plugin/base_wrapper.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/singleton/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:03:32.000000 research_framework-0.2.2/research_framework/base/singleton/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      262 2024-04-25 16:34:16.000000 research_framework-0.2.2/research_framework/base/singleton/base_singleton.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/storage/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/base/storage/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      545 2024-04-25 16:34:46.000000 research_framework-0.2.2/research_framework/base/storage/base_storage.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/base/utils/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-21 13:26:13.000000 research_framework-0.2.2/research_framework/base/utils/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1503 2023-11-08 11:20:29.000000 research_framework-0.2.2/research_framework/base/utils/grid_seach.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      308 2023-09-19 18:09:27.000000 research_framework-0.2.2/research_framework/base/utils/method_overload.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.2/research_framework/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5051 2024-04-25 18:49:10.000000 research_framework-0.2.2/research_framework/container/container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/container/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-17 21:22:31.000000 research_framework-0.2.2/research_framework/container/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      472 2023-12-29 13:57:37.000000 research_framework-0.2.2/research_framework/container/model/global_config.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/dataset/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:07:36.000000 research_framework-0.2.2/research_framework/dataset/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      872 2023-09-20 22:03:33.000000 research_framework-0.2.2/research_framework/dataset/basic_dataset.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1071 2023-11-07 10:26:41.000000 research_framework-0.2.2/research_framework/dataset/standard_dataset.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/flyweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/flyweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8026 2024-04-24 16:58:20.000000 research_framework-0.2.2/research_framework/flyweight/flyweight.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    14387 2024-04-25 17:28:03.000000 research_framework-0.2.2/research_framework/flyweight/flyweight_manager.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2024-04-29 11:35:05.000000 research_framework-0.2.2/research_framework/flyweight/mem_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/flyweight/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/flyweight/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research_framework-0.2.2/research_framework/flyweight/model/item_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      659 2023-11-08 13:27:58.000000 research_framework-0.2.2/research_framework/flyweight/model/item_model.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      497 2024-04-10 01:30:54.000000 research_framework-0.2.2/research_framework/flyweight/model/item_simple_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/neural_models/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:13:05.000000 research_framework-0.2.2/research_framework/neural_models/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      379 2023-09-13 12:58:06.000000 research_framework-0.2.2/research_framework/neural_models/doomy_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/pipeline/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-11-07 13:43:32.000000 research_framework-0.2.2/research_framework/pipeline/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research_framework-0.2.2/research_framework/pipeline/inputs.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.943612 research_framework-0.2.2/research_framework/pipeline/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/research_framework/pipeline/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3233 2024-04-25 16:57:27.000000 research_framework-0.2.2/research_framework/pipeline/model/pipeline_model.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     9541 2024-04-29 11:56:38.000000 research_framework-0.2.2/research_framework/pipeline/pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2657 2024-04-29 19:46:51.000000 research_framework-0.2.2/research_framework/pipeline/pipeline_manager.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/research_framework/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      416 2023-09-17 16:58:56.000000 research_framework-0.2.2/research_framework/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5755 2024-04-29 17:32:18.000000 research_framework-0.2.2/research_framework/plugins/cv_strategies_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1626 2024-04-10 02:28:58.000000 research_framework-0.2.2/research_framework/plugins/data_ingestion_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4391 2023-09-21 10:17:00.000000 research_framework-0.2.2/research_framework/plugins/doomy_predictor.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    11586 2024-04-10 00:55:18.000000 research_framework-0.2.2/research_framework/plugins/grid_search_cross_val.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2911 2024-04-29 12:02:49.000000 research_framework-0.2.2/research_framework/plugins/metrics_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1526 2023-09-20 20:59:39.000000 research_framework-0.2.2/research_framework/plugins/text_mod_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4267 2023-09-20 22:03:53.000000 research_framework-0.2.2/research_framework/plugins/text_rep_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6845 2024-04-29 12:14:04.000000 research_framework-0.2.2/research_framework/plugins/unsupervised_predictor.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1096 2023-09-19 18:12:57.000000 research_framework-0.2.2/research_framework/plugins/vector_red_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2764 2024-04-29 17:26:12.000000 research_framework-0.2.2/research_framework/plugins/wandb_sweep_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4460 2024-04-24 20:06:57.000000 research_framework-0.2.2/research_framework/plugins/wrappers.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/research_framework/storage/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-02 20:07:06.000000 research_framework-0.2.2/research_framework/storage/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4770 2024-04-25 16:30:23.000000 research_framework-0.2.2/research_framework/storage/google_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1732 2024-04-25 16:33:38.000000 research_framework-0.2.2/research_framework/storage/local_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2893 2024-04-25 16:30:12.000000 research_framework-0.2.2/research_framework/storage/s3_storage.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/research_framework.egg-info/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-04-29 19:47:11.000000 research_framework-0.2.2/research_framework.egg-info/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3817 2024-04-29 19:47:11.000000 research_framework-0.2.2/research_framework.egg-info/SOURCES.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2024-04-29 19:47:11.000000 research_framework-0.2.2/research_framework.egg-info/dependency_links.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      386 2024-04-29 19:47:11.000000 research_framework-0.2.2/research_framework.egg-info/requires.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2024-04-29 19:47:11.000000 research_framework-0.2.2/research_framework.egg-info/top_level.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/scripts/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.2/scripts/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      507 2023-09-19 19:10:14.000000 research_framework-0.2.2/scripts/clean.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research_framework-0.2.2/scripts/clean_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2024-04-29 19:47:11.947612 research_framework-0.2.2/setup.cfg
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1059 2024-04-29 19:47:01.000000 research_framework-0.2.2/setup.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/test/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.2/test/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/test/metrics/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:39:11.000000 research_framework-0.2.2/test/metrics/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      757 2024-04-25 18:51:45.000000 research_framework-0.2.2/test/metrics/test_metrics.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 19:47:11.947612 research_framework-0.2.2/test/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.2/test/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      644 2024-04-25 18:08:47.000000 research_framework-0.2.2/test/plugins/test_mem_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1796 2023-09-20 12:11:32.000000 research_framework-0.2.2/test/plugins/test_plugin.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      956 2023-11-07 13:40:25.000000 research_framework-0.2.2/test/test_container_bindings.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3554 2023-11-07 12:38:53.000000 research_framework-0.2.2/test/test_flyweight_with_google_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2023-11-06 20:17:48.000000 research_framework-0.2.2/test/test_flyweight_with_local_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3555 2024-01-14 01:08:22.000000 research_framework-0.2.2/test/test_flyweight_with_s3_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6278 2024-04-26 12:01:06.000000 research_framework-0.2.2/test/test_mem_module.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     7174 2023-12-29 14:28:04.000000 research_framework-0.2.2/test/test_pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6881 2023-12-29 14:27:46.000000 research_framework-0.2.2/test/test_pipeline_grid_search.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6934 2024-04-25 16:54:39.000000 research_framework-0.2.2/test/test_simple_pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6510 2024-04-10 01:52:30.000000 research_framework-0.2.2/test/test_simple_pipeline_manager.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8532 2024-04-29 17:18:12.000000 research_framework-0.2.2/test/test_simple_pipeline_with_sweep_supervised.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8449 2024-04-29 12:25:07.000000 research_framework-0.2.2/test/test_simple_pipeline_with_sweep_unsupervised.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4580 2023-09-20 12:16:43.000000 research_framework-0.2.2/test/test_wrappers_type_validation.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research_framework-0.2.3/LICENSE
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research_framework-0.2.3/MANIFEST.in
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-01 17:36:41.277938 research_framework-0.2.3/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      393 2024-05-01 13:22:11.000000 research_framework-0.2.3/requirements.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.269938 research_framework-0.2.3/research_framework/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       91 2023-11-07 13:43:38.000000 research_framework-0.2.3/research_framework/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.269938 research_framework-0.2.3/research_framework/base/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.269938 research_framework-0.2.3/research_framework/base/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1990 2023-11-09 16:51:42.000000 research_framework-0.2.3/research_framework/base/container/base_container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.269938 research_framework-0.2.3/research_framework/base/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.3/research_framework/base/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      722 2023-09-19 17:54:13.000000 research_framework-0.2.3/research_framework/base/container/model/bind_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.269938 research_framework-0.2.3/research_framework/base/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.3/research_framework/base/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1074 2023-11-08 13:26:10.000000 research_framework-0.2.3/research_framework/base/flyweight/base_flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      800 2024-04-25 16:51:06.000000 research_framework-0.2.3/research_framework/base/flyweight/base_flyweight_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2550 2024-03-02 14:06:30.000000 research_framework-0.2.3/research_framework/base/model/base_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/model/base_utils.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-06 20:33:03.000000 research_framework-0.2.3/research_framework/base/pipeline/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      227 2023-12-29 14:25:32.000000 research_framework-0.2.3/research_framework/base/pipeline/base_pipeline.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/plugin/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/plugin/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1029 2023-10-15 10:47:16.000000 research_framework-0.2.3/research_framework/base/plugin/base_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      337 2024-04-25 10:02:49.000000 research_framework-0.2.3/research_framework/base/plugin/base_wrapper.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/singleton/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:03:32.000000 research_framework-0.2.3/research_framework/base/singleton/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      262 2024-04-25 16:34:16.000000 research_framework-0.2.3/research_framework/base/singleton/base_singleton.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/base/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      545 2024-04-25 16:34:46.000000 research_framework-0.2.3/research_framework/base/storage/base_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/base/utils/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-21 13:26:13.000000 research_framework-0.2.3/research_framework/base/utils/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1503 2024-05-01 17:24:30.000000 research_framework-0.2.3/research_framework/base/utils/grid_seach.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      308 2023-09-19 18:09:27.000000 research_framework-0.2.3/research_framework/base/utils/method_overload.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.3/research_framework/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5265 2024-05-01 16:40:16.000000 research_framework-0.2.3/research_framework/container/container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-17 21:22:31.000000 research_framework-0.2.3/research_framework/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      505 2024-05-01 12:33:48.000000 research_framework-0.2.3/research_framework/container/model/global_config.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/dataset/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:07:36.000000 research_framework-0.2.3/research_framework/dataset/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      872 2023-09-20 22:03:33.000000 research_framework-0.2.3/research_framework/dataset/basic_dataset.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1071 2023-11-07 10:26:41.000000 research_framework-0.2.3/research_framework/dataset/standard_dataset.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8026 2024-04-24 16:58:20.000000 research_framework-0.2.3/research_framework/flyweight/flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    14387 2024-04-25 17:28:03.000000 research_framework-0.2.3/research_framework/flyweight/flyweight_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2024-04-29 11:35:05.000000 research_framework-0.2.3/research_framework/flyweight/mem_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/flyweight/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/flyweight/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research_framework-0.2.3/research_framework/flyweight/model/item_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      659 2023-11-08 13:27:58.000000 research_framework-0.2.3/research_framework/flyweight/model/item_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      497 2024-04-10 01:30:54.000000 research_framework-0.2.3/research_framework/flyweight/model/item_simple_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/neural_models/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:13:05.000000 research_framework-0.2.3/research_framework/neural_models/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      379 2023-09-13 12:58:06.000000 research_framework-0.2.3/research_framework/neural_models/doomy_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-11-07 13:43:32.000000 research_framework-0.2.3/research_framework/pipeline/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/pipeline/exceptions/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 13:09:29.000000 research_framework-0.2.3/research_framework/pipeline/exceptions/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       54 2024-05-01 13:11:12.000000 research_framework-0.2.3/research_framework/pipeline/exceptions/pipeline_exceptions.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       49 2024-05-01 13:11:19.000000 research_framework-0.2.3/research_framework/pipeline/exceptions/run_exceptions.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research_framework-0.2.3/research_framework/pipeline/inputs.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.273939 research_framework-0.2.3/research_framework/pipeline/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/research_framework/pipeline/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3233 2024-04-25 16:57:27.000000 research_framework-0.2.3/research_framework/pipeline/model/pipeline_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    10259 2024-05-01 15:55:12.000000 research_framework-0.2.3/research_framework/pipeline/pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2707 2024-05-01 15:18:20.000000 research_framework-0.2.3/research_framework/pipeline/pipeline_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/research_framework/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      416 2023-09-17 16:58:56.000000 research_framework-0.2.3/research_framework/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6238 2024-05-01 17:22:28.000000 research_framework-0.2.3/research_framework/plugins/cv_strategies_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1626 2024-04-10 02:28:58.000000 research_framework-0.2.3/research_framework/plugins/data_ingestion_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4391 2023-09-21 10:17:00.000000 research_framework-0.2.3/research_framework/plugins/doomy_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    11566 2024-05-01 12:28:48.000000 research_framework-0.2.3/research_framework/plugins/grid_search_cross_val.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2968 2024-05-01 12:49:35.000000 research_framework-0.2.3/research_framework/plugins/metrics_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1526 2023-09-20 20:59:39.000000 research_framework-0.2.3/research_framework/plugins/text_mod_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4267 2023-09-20 22:03:53.000000 research_framework-0.2.3/research_framework/plugins/text_rep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6845 2024-04-29 12:14:04.000000 research_framework-0.2.3/research_framework/plugins/unsupervised_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1096 2023-09-19 18:12:57.000000 research_framework-0.2.3/research_framework/plugins/vector_red_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3425 2024-05-01 17:31:50.000000 research_framework-0.2.3/research_framework/plugins/wandb_sweep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5324 2024-05-01 17:06:24.000000 research_framework-0.2.3/research_framework/plugins/wrappers.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/research_framework/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-02 20:07:06.000000 research_framework-0.2.3/research_framework/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4770 2024-04-25 16:30:23.000000 research_framework-0.2.3/research_framework/storage/google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1732 2024-04-25 16:33:38.000000 research_framework-0.2.3/research_framework/storage/local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2893 2024-04-25 16:30:12.000000 research_framework-0.2.3/research_framework/storage/s3_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/research_framework.egg-info/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-05-01 17:36:41.000000 research_framework-0.2.3/research_framework.egg-info/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3987 2024-05-01 17:36:41.000000 research_framework-0.2.3/research_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2024-05-01 17:36:41.000000 research_framework-0.2.3/research_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      386 2024-05-01 17:36:41.000000 research_framework-0.2.3/research_framework.egg-info/requires.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2024-05-01 17:36:41.000000 research_framework-0.2.3/research_framework.egg-info/top_level.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/scripts/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.3/scripts/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      507 2023-09-19 19:10:14.000000 research_framework-0.2.3/scripts/clean.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research_framework-0.2.3/scripts/clean_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2024-05-01 17:36:41.277938 research_framework-0.2.3/setup.cfg
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1059 2024-05-01 17:36:35.000000 research_framework-0.2.3/setup.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/test/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.3/test/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/test/metrics/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:39:11.000000 research_framework-0.2.3/test/metrics/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      757 2024-04-25 18:51:45.000000 research_framework-0.2.3/test/metrics/test_metrics.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-05-01 17:36:41.277938 research_framework-0.2.3/test/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.3/test/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      644 2024-04-25 18:08:47.000000 research_framework-0.2.3/test/plugins/test_mem_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1796 2023-09-20 12:11:32.000000 research_framework-0.2.3/test/plugins/test_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      956 2023-11-07 13:40:25.000000 research_framework-0.2.3/test/test_container_bindings.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3554 2023-11-07 12:38:53.000000 research_framework-0.2.3/test/test_flyweight_with_google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2023-11-06 20:17:48.000000 research_framework-0.2.3/test/test_flyweight_with_local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3555 2024-01-14 01:08:22.000000 research_framework-0.2.3/test/test_flyweight_with_s3_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6278 2024-04-26 12:01:06.000000 research_framework-0.2.3/test/test_mem_module.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     7174 2023-12-29 14:28:04.000000 research_framework-0.2.3/test/test_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6881 2023-12-29 14:27:46.000000 research_framework-0.2.3/test/test_pipeline_grid_search.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6934 2024-04-25 16:54:39.000000 research_framework-0.2.3/test/test_simple_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6510 2024-04-10 01:52:30.000000 research_framework-0.2.3/test/test_simple_pipeline_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8901 2024-05-01 15:56:37.000000 research_framework-0.2.3/test/test_simple_pipeline_with_sweep_supervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8441 2024-05-01 17:21:42.000000 research_framework-0.2.3/test/test_simple_pipeline_with_sweep_unsupervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4580 2023-09-20 12:16:43.000000 research_framework-0.2.3/test/test_wrappers_type_validation.py
```

### Comparing `research_framework-0.2.2/LICENSE` & `research_framework-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/PKG-INFO` & `research_framework-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-framework
-Version: 0.2.2
+Version: 0.2.3
 Summary: framework base para investigación
 Home-page: https://github.com/manucouto1/research_framework
 Author: Manuel Couto Pintos
 Author-email: manuel.couto.pintos@usc.es
 License: Apache License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -23,14 +23,14 @@
 Requires-Dist: pytest==7.4.0
 Requires-Dist: pandas==2.1.0
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: scikit-fuzzy==0.4.2
 Requires-Dist: torch==2.0.1
 Requires-Dist: transformers[torch]==4.33.0
 Requires-Dist: sentence-transformers[torch]==2.2.2
-Requires-Dist: wandb==0.16.0
+Requires-Dist: wandb==0.16.6
 Requires-Dist: atpbar==1.1.4
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: rich==13.5.2
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: boto3==1.34.16
 Requires-Dist: randomname
```

### Comparing `research_framework-0.2.2/research_framework/base/container/base_container.py` & `research_framework-0.2.3/research_framework/base/container/base_container.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/container/model/bind_model.py` & `research_framework-0.2.3/research_framework/base/container/model/bind_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/flyweight/base_flyweight.py` & `research_framework-0.2.3/research_framework/base/flyweight/base_flyweight.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/flyweight/base_flyweight_manager.py` & `research_framework-0.2.3/research_framework/base/flyweight/base_flyweight_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/model/base_dao.py` & `research_framework-0.2.3/research_framework/base/model/base_dao.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/model/base_utils.py` & `research_framework-0.2.3/research_framework/base/model/base_utils.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/plugin/base_plugin.py` & `research_framework-0.2.3/research_framework/base/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/storage/base_storage.py` & `research_framework-0.2.3/research_framework/base/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/base/utils/grid_seach.py` & `research_framework-0.2.3/research_framework/base/utils/grid_seach.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/container/container.py` & `research_framework-0.2.3/research_framework/container/container.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,28 +42,30 @@
             if wandb.run is None:
                 Container.logger = wandb.init(project=project, name=name, settings=wandb.Settings(start_method="fork"), config=config)
     
     @staticmethod
     def freeze_wandb_logger():
         if Container.logger is not None:
             Container.freeze_id = Container.logger.id
+            print(f"* Frizzing run_id > {Container.freeze_id}")
             Container.logger.finish()    
     
     @staticmethod
     def update_freezed_run(project:str, run_id:str, update_dict:Dict[str, Any]):
         api = wandb.Api()
         run = api.run(f'citius-irlab/{project}/{run_id}')
         run.config.update(update_dict)
         run.update()
 
         
     @staticmethod
     def un_freeze_wandb_logger():
         if Container.freeze_id is not None:
-            Container.logger = wandb.init(id=Container.freeze_id, resume='allow', reinit=True)
+            print(f"* Unfrizzing run_id > {Container.freeze_id}")
+            Container.logger = wandb.init(id=Container.freeze_id, project=Container.global_config.project_name, name=Container.global_config.run_name, resume="must", reinit=True)
     
     
     @staticmethod
     def send_to_logger(message:Dict[str, Any], step:Optional[int] = None):
         if Container.global_config.log:
             if step is None:
                 wandb.log(message)
```

### Comparing `research_framework-0.2.2/research_framework/dataset/basic_dataset.py` & `research_framework-0.2.3/research_framework/dataset/basic_dataset.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/dataset/standard_dataset.py` & `research_framework-0.2.3/research_framework/dataset/standard_dataset.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/flyweight/flyweight.py` & `research_framework-0.2.3/research_framework/flyweight/flyweight.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/flyweight/flyweight_manager.py` & `research_framework-0.2.3/research_framework/flyweight/flyweight_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/flyweight/mem_manager.py` & `research_framework-0.2.3/research_framework/flyweight/mem_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/flyweight/model/item_dao.py` & `research_framework-0.2.3/research_framework/flyweight/model/item_dao.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/flyweight/model/item_model.py` & `research_framework-0.2.3/research_framework/flyweight/model/item_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/pipeline/model/pipeline_model.py` & `research_framework-0.2.3/research_framework/pipeline/model/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/pipeline/pipeline.py` & `research_framework-0.2.3/research_framework/pipeline/pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from research_framework.base.flyweight.base_flyweight_manager import BaseFlyManager
 from research_framework.base.pipeline.base_pipeline import BasePipeline
 from research_framework.base.plugin.base_wrapper import BaseWrapper
 from research_framework.container.container import Container
 from research_framework.flyweight.mem_manager import FILTER_VARS
+from research_framework.pipeline.exceptions.pipeline_exceptions import PipelineExecutionException
 from research_framework.pipeline.model.pipeline_model import FilterModel, InputFilterModel, PipelineModel, WandbRunPipelineModel
 from research_framework.base.utils.grid_seach import generate_combis
 from research_framework.flyweight.flyweight import SimpleFlyWeight
 from rich import print
 
 from research_framework.pipeline.pipeline_manager import PipelineManager
 from research_framework.storage.local_storage import LocalStorage
 
+import wandb
 
 @Container.register_pipeline
 class WandbRunPipeline(BasePipeline):
     def __init__(self, doc:WandbRunPipelineModel):
         self.pipeline:WandbRunPipelineModel = doc
         self.pipeline_wrappers = []
 
-
+    def init(self):
+        Container.un_freeze_wandb_logger()
+        
     def start(self):
         train_input = self.pipeline.train_input
         test_input = self.pipeline.test_input
         
-        train_f = self.fit(train_input)
-        
-        if test_input is not None:
-            test_f = self.predict(test_input)
-        else:
-            test_f = train_f
+        try:
+            train_f = self.fit(train_input)
             
-        for idx, metric in enumerate(self.pipeline.metrics):
-                m_wrapper = Container.get_metric(metric.clazz, metric.params)
-                metric.value = m_wrapper.predict(test_f)
-                self.pipeline.metrics[idx] = metric
+            if test_input is not None:
+                test_f = self.predict(test_input)
+            else:
+                test_f = train_f
+                
+            for idx, metric in enumerate(self.pipeline.metrics):
+                    m_wrapper = Container.get_metric(metric.clazz, metric.params)
+                    metric.value = m_wrapper.predict(test_f)
+                    self.pipeline.metrics[idx] = metric
 
+        except Exception as ex:
+            raise PipelineExecutionException(ex)
 
     def fit(self, train_input:InputFilterModel):
         train_w = Container.get_wrapper(train_input.clazz, train_input.params)
         train_f = train_w.predict(None)
         
         for _, filter_model in enumerate(self.pipeline.filters):
             # Container.MEM.insert(FILTER_VARS("TEMP", LocalStorage('data/cache')))
@@ -63,58 +70,64 @@
         
     def log_metrics(self) -> None:
         print(self.pipeline.metrics)
         for metric in self.pipeline.metrics:
             Container.send_to_logger(message={metric.clazz: metric.value})
 
     def finish(self) -> None:
-        if not Container.logger is None:
+        if Container.logger is not None:
             Container.logger.finish()
 
 @Container.register_pipeline
 class SimpleFitPredictPipeline(BasePipeline):
     def __init__(self, doc:PipelineModel, project:str):
         Container.fly = SimpleFlyWeight()
-        
         self.pipeline: PipelineModel = doc
-        
-        config = {'dataset': self.pipeline.train_input.name}
+        self.config = {'dataset': self.pipeline.train_input.name}
         
         for f in self.pipeline.filters:
-            config[f.clazz] = f.params
+            self.config[f.clazz] = f.params
             
-        project_hash = Container.fly.hashcode_from_name("->".join(list(map(lambda x: f'({x.clazz}:{x.params})', self.pipeline.filters))))
+        self.project_hash = Container.fly.hashcode_from_name("->".join(list(map(lambda x: f'({x.clazz}:{x.params})', self.pipeline.filters))))
         
+        Container.global_config.dataset = self.pipeline.train_input.name
         Container.global_config.project_name = project
-        Container.global_config.run_name = self.pipeline.train_input.name+"->("+project_hash+")"
-        Container.init_wandb_logger(
-            project=project, 
-            name=self.pipeline.train_input.name+"->("+project_hash+")",
-            config=config
-        )
+        Container.global_config.run_name = self.pipeline.train_input.name+"->("+self.project_hash+")"
         
         self.pipeline_filters = []
         
-        Container.send_to_logger(message={"dataset": self.pipeline.train_input.name})
     
+    def init(self):
+        Container.init_wandb_logger(
+            project=Container.global_config.project_name, 
+            name=Container.global_config.run_name,
+            config=self.config
+        )
+        Container.send_to_logger(message={"dataset": Container.global_config.dataset})
+        
+        
     def start(self):
         train_input = self.pipeline.train_input
         test_input = self.pipeline.test_input
         
-        train_f = self.fit(train_input)
-        
-        if test_input is not None:
-            test_f = self.predict(test_input)
-        else:
-            test_f = train_f
+        try:
+            train_f = self.fit(train_input)
             
-        for idx, metric in enumerate(self.pipeline.metrics):
-                m_wrapper = Container.get_metric(metric.clazz, metric.params)
-                metric.value = m_wrapper.predict(test_f)
-                self.pipeline.metrics[idx] = metric
+            if test_input is not None:
+                test_f = self.predict(test_input)
+            else:
+                test_f = train_f
+                
+            for idx, metric in enumerate(self.pipeline.metrics):
+                    m_wrapper = Container.get_metric(metric.clazz, metric.params)
+                    metric.value = m_wrapper.predict(test_f)
+                    self.pipeline.metrics[idx] = metric
+        
+        except Exception as ex:
+            raise PipelineExecutionException(ex)
         
     def fit(self, train_input:InputFilterModel):
         train_m = Container.get_filter_manager(train_input.clazz, train_input.params)
         
         train_item = train_m.next_data_item(train_input, train_input, None)
         train_f = train_m.predict(data_item=train_item)
         
@@ -164,30 +177,33 @@
             
 @Container.register_pipeline
 class FitPredictPipeline(BasePipeline):
     def __init__(self, doc:PipelineModel, project:str):
         print("\n* Pipeline: ")
         self.pipeline:PipelineModel = PipelineManager.fill_pipline_items(doc) 
         print(self.pipeline)
-        
-        config = {'dataset': self.pipeline.train_input.name}
+        self.project = project
+        self.config = {'dataset': self.pipeline.train_input.name}
         for f in self.pipeline.filters:
-            config[f.clazz] = f.params
+            self.config[f.clazz] = f.params
             
-        project_hash = Container.fly.hashcode_from_name("->".join(list(map(lambda x: f'({x.clazz}:{x.params})', self.pipeline.filters))))
-        Container.global_config.project_name = project
-        Container.global_config.run_name = self.pipeline.train_input.name+"->("+project_hash+")"
-        Container.init_wandb_logger(
-            project=project, 
-            name=self.pipeline.train_input.name+"->("+project_hash+")",
-            config=config
-        )
+        self.project_hash = Container.fly.hashcode_from_name("->".join(list(map(lambda x: f'({x.clazz}:{x.params})', self.pipeline.filters))))
         
         self.pipeline_filters = []
         
+        
+    
+    def init(self):
+        Container.global_config.project_name = self.project
+        Container.global_config.run_name = self.pipeline.train_input.name+"->("+self.project_hash+")"
+        Container.init_wandb_logger(
+            project=self.project, 
+            name=self.pipeline.train_input.name+"->("+self.project_hash+")",
+            config=self.config
+        )
         Container.send_to_logger(message={"dataset": self.pipeline.train_input.name})
         
     def start(self) -> None:
         try:
             train_input = self.pipeline.train_input
             test_input = self.pipeline.test_input
             
@@ -216,15 +232,15 @@
 
             for idx, metric in enumerate(self.pipeline.metrics):
                 m_wrapper = Container.get_metric(metric.clazz, metric.params)
                 metric.value = m_wrapper.predict(test_f)
                 self.pipeline.metrics[idx] = metric
                 
         except Exception as ex:
-            raise ex
+            raise PipelineExecutionException(ex)
          
         
     def log_metrics(self) -> None:
         print(self.pipeline.metrics)
         for metric in self.pipeline.metrics:
             Container.send_to_logger(message={metric.clazz: metric.value})
```

### Comparing `research_framework-0.2.2/research_framework/pipeline/pipeline_manager.py` & `research_framework-0.2.3/research_framework/pipeline/pipeline_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,18 @@
         Container.global_config = GlobalConfig(
             log=log,
             overwrite=overwrite,
             store=store
         )
         
         pipeline:BasePipeline = Container.PIPELINES[pl_conf._clazz](pl_conf, project)
+        pipeline.init()
         pipeline.start()
         pipeline.log_metrics()
+        pipeline.finish()
         return pipeline
     
     @staticmethod
     def fill_pipline_items(config:PipelineModel):
         PipelineManager.init_fly(SimpleFlyWeight)
         print("___________________ FILLING PIPELINE WITH ITEMS ____________________\n")
         print("* Train input")
```

### Comparing `research_framework-0.2.2/research_framework/plugins/cv_strategies_plugins.py` & `research_framework-0.2.3/research_framework/plugins/cv_strategies_plugins.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,172 +5,185 @@
 import wandb
 import wandb.sdk
 import numpy as np
 
 from research_framework.base.plugin.base_wrapper import BaseWrapper
 from research_framework.container.container import Container
 from research_framework.dataset.standard_dataset import StandardDataset
-from research_framework.pipeline.model.pipeline_model import FilterModel, InputFilterModel, SimplePipelineModel, WandbRunPipelineModel
+from research_framework.pipeline.exceptions.run_exceptions import RunExecutionException
+from research_framework.pipeline.model.pipeline_model import FilterModel, WandbRunPipelineModel
 
 
 class UnsupervisedRun:
-    def __init__(self, data, scorer, metrics):
+    def __init__(self, data, scorer, metrics, dataset):
         self.data = data
         self.scorer = scorer
         self.metrics = metrics
+        self.dataset = dataset
         self.out_metrics = {}
-        
-    def exec(self):
+    
+    def init(self):
         run = wandb.init(reinit=True)
-        config = wandb.config
-        
         assert run is not None
         assert type(run) is wandb.sdk.wandb_run.Run
         
-        x_train:StandardDataset = self.data
+    def exec(self):
+        config = wandb.config
         
-        for clazz in config.order:
-            wrapper:BaseWrapper = Container.get_wrapper(clazz, config[clazz])
-            wrapper.fit(x_train)
+        try:
+            x_train:StandardDataset = self.data
             
-            x_train = wrapper.predict(x_train)
+            for clazz in config.order:
+                wrapper:BaseWrapper = Container.get_wrapper(clazz, config[clazz])
+                wrapper.fit(x_train)
+                
+                x_train = wrapper.predict(x_train)
 
-        m_wrapper = Container.get_metric(self.scorer)
-        
-        self.out_metrics[self.scorer] = m_wrapper.predict(x_train)
-        
-        for metric in self.metrics:
-            m_wrapper = Container.get_metric(metric)
-            try:
+            m_wrapper = Container.get_metric(self.scorer)
+            
+            self.out_metrics[self.scorer] = m_wrapper.predict(x_train)
+            
+            for metric in self.metrics:
+                m_wrapper = Container.get_metric(metric)
+                
                 self.out_metrics[metric] = m_wrapper.predict(x_train)
-            except Exception as ex:
-                print(traceback.print_exc())
+        except Exception as ex:
+                raise RunExecutionException(ex)
         
     def log_metrics(self):
         wandb.log(self.out_metrics)
     
     def get_pipeline(self, name, config, train_dm):
         
         pl_conf = WandbRunPipelineModel(
             name=f'CrossValPipeline_{name}',
             train_input=train_dm,
             filters=[FilterModel(clazz=clazz, params=config[clazz]) for clazz in config["order"]],
             metrics=self.metrics
         )
 
         pipeline = Container.PIPELINES[pl_conf._clazz](pl_conf)
-        pipeline.fit(train_dm)
 
         return pipeline
+    
+    def finish(self):
+        wandb.finish()
 
 
 """
 TODO Todavía no se cómo tengo que hacer
 """   
 class SupervisedRun:
-    def __init__(self, train_data, test_data, scorer, metrics, group_name=None, run_name=None):
+    def __init__(self, train_data, test_data, scorer, metrics, dataset, group_name=None, run_name=None):
         self.train_data = train_data
         self.test_data = test_data
         self.scorer = scorer
         self.metrics = metrics
+        self.dataset = dataset
         self.group_name = group_name
         self.run_name = run_name
         self.out_metrics = {}
-        
-    def exec(self):
-        config = wandb.config
-        print(f'Config > {config}')
+    
+    def init(self):
         run = wandb.init(group=self.group_name, name=self.run_name, reinit=True)
         assert run is not None
         assert type(run) is wandb.sdk.wandb_run.Run
         
-        train_data = self.train_data
-        test_data = self.test_data
-        
-        for clazz in config.order:
-            wrapper:BaseWrapper = Container.get_wrapper(clazz, config[clazz])
-            wrapper.fit(self.train_data)
+    def exec(self):
+        try:
+            config = wandb.config
+            print(f'Config > {config}')
+            
+            train_data = self.train_data
+            test_data = self.test_data
             
-            train_data = wrapper.predict(train_data)
-            test_data = wrapper.predict(test_data)
+            for clazz in config.order:
+                wrapper:BaseWrapper = Container.get_wrapper(clazz, config[clazz])
+                wrapper.fit(self.train_data)
+                
+                train_data = wrapper.predict(train_data)
+                test_data = wrapper.predict(test_data)
 
-        m_wrapper = Container.get_metric(self.scorer)
-        
-        self.out_metrics[self.scorer] = m_wrapper.predict(test_data)
-        
-        for metric in self.metrics:
-            m_wrapper = Container.get_metric(metric)
-            self.out_metrics[metric] = m_wrapper.predict(test_data)
+            m_wrapper = Container.get_metric(self.scorer)
+            
+            self.out_metrics[self.scorer] = m_wrapper.predict(test_data)
+            
+            for metric in self.metrics:
+                m_wrapper = Container.get_metric(metric)
+                self.out_metrics[metric] = m_wrapper.predict(test_data)
+            
+        except Exception as ex:
+            raise RunExecutionException(ex)
         
     def get_pipeline(self, name, config):
         pipeline = []
         for clazz in config["order"]:
             wrapper:BaseWrapper = Container.get_wrapper(clazz, config[clazz])
             wrapper.fit(self.data)
             pipeline.append(wrapper)
         return pipeline
     
     def log_metrics(self):
-        wandb.log(self.metrics)   
+        wandb.log(self.metrics)
+        
+    def finish(self):
+        wandb.finish()
 
 class ShuffleCVRun:
-    def __init__(self, data, scorer, metrics=[], n_splits=2, test_size=0.2, random_state=7):
+    def __init__(self, data, scorer, dataset, metrics=[], n_splits=2, test_size=0.2, random_state=7):
         self.data = data
         self.metrics = metrics
         self.scorer = scorer
+        self.dataset = dataset
         self.n_splits = n_splits
         self.test_size = test_size
         self.random_state = random_state
         self.out_metrics = {}
     
-    def exec(self):
+    def init(self):
         run = wandb.init(reinit=True)
-        
         assert run is not None
         assert type(run) is wandb.sdk.wandb_run.Run
         
+    def exec(self):
         cv = ShuffleSplit(
             n_splits=self.n_splits, 
             test_size=self.test_size, 
             random_state=self.random_state
         )
         
         splits = cv.split(self.data)
-        cv_name = randomname.get_name()
-        
+    
         for split,(train_idx, test_idx) in enumerate(splits):
-        
-            run_name = f"{cv_name}-{split:02}"
-            group_name = f"cv_{cv_name}"
+            print(f'* Split {split} ->')
             
-            train_data = self.data[train_idx]
-            test_data = self.data[test_idx]
-        
-            s_run = SupervisedRun(train_data, test_data, group_name, run_name)
+            train_data = StandardDataset(*self.data[train_idx])
+            test_data = StandardDataset(*self.data[test_idx])
+
+            s_run = SupervisedRun(train_data, test_data, dataset=self.dataset, scorer=self.scorer, metrics=self.metrics)
             s_run.exec()
-            
-            for k,v in s_run.metrics.items():
-                m_acum = self.out_metrics.get(k, []) 
-                m_acum.append(v)
-                self.out_metrics[k] = m_acum
         
+        for k,v in s_run.out_metrics.items():
+            m_acum = self.out_metrics.get(k, []) 
+            m_acum.append(v)
+            self.out_metrics[k] = m_acum
+            
     def log_metrics(self):
         wandb.log(dict(map(lambda kv: (kv[0],np.mean(kv[1])), self.out_metrics.items())))
     
     def get_pipeline(self, name, config, train_dm):
-        
         pl_conf = WandbRunPipelineModel(
             name=f'CrossValPipeline_{name}',
             train_input=train_dm,
             filters=[FilterModel(clazz=clazz, params=config[clazz]) for clazz in config["order"]],
             metrics=self.metrics
         )
-        
         pipeline = Container.PIPELINES[pl_conf._clazz](pl_conf)
-        pipeline.fit(train_dm)
-        
         return pipeline
+    
+    def finish(self):
+        wandb.finish()
 
 class RunEnum(Enum):
     unsupervised = UnsupervisedRun
     superised = SupervisedRun
     shuffle_cv = ShuffleCVRun
```

### Comparing `research_framework-0.2.2/research_framework/plugins/data_ingestion_plugins.py` & `research_framework-0.2.3/research_framework/plugins/data_ingestion_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/doomy_predictor.py` & `research_framework-0.2.3/research_framework/plugins/doomy_predictor.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/grid_search_cross_val.py` & `research_framework-0.2.3/research_framework/plugins/grid_search_cross_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             x = x()
         
         for wrapper in self.best_pipeline:
             x = wrapper.predict(x)
         
         return x
 
-@Container.bind(WandbSeepsFlyManager)
+@Container.bind()
 class WandbSeepsAgent(BaseFilterPlugin):
     
     def __init__(self, scorer=MetricModel(clazz='F1'), refit=True, sweep_id=None, metrics=[], filters=[]):
         self.filters = filters
         self.scorer = scorer
         self.metrics = metrics
         self.refit = refit
```

### Comparing `research_framework-0.2.2/research_framework/plugins/metrics_plugins.py` & `research_framework-0.2.3/research_framework/plugins/metrics_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,21 +72,21 @@
     def predict(self, y, predicted ):
         return  homogeneity_completeness_v_measure(y, predicted)
     
 @Container.bind(OutputFlyManager, MetricWrapper)
 class F1(BasePlugin): 
     def fit(self, *args, **kwargs): ...
     def predict(self, y, predicted):
-        return f1_score(y, predicted)
+        return f1_score(y, predicted, zero_division=0.0)
 
 @Container.bind(OutputFlyManager, MetricWrapper)
 class Precision(BasePlugin):
     def fit(self, *args, **kwargs): ...
     def predict(self, y, predicted):
-        return precision_score(y, predicted)
+        return precision_score(y, predicted, zero_division=0.0)
 
 
 @Container.bind(OutputFlyManager, MetricWrapper)
 class Recall(BasePlugin):
     def fit(self, *args, **kwargs): ...
     def predict(self, y, predicted):
-        return recall_score(y, predicted)
+        return recall_score(y, predicted, zero_division=0.0)
```

### Comparing `research_framework-0.2.2/research_framework/plugins/text_mod_plugins.py` & `research_framework-0.2.3/research_framework/plugins/text_mod_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/text_rep_plugins.py` & `research_framework-0.2.3/research_framework/plugins/text_rep_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/unsupervised_predictor.py` & `research_framework-0.2.3/research_framework/plugins/unsupervised_predictor.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/vector_red_plugins.py` & `research_framework-0.2.3/research_framework/plugins/vector_red_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/plugins/wandb_sweep_plugins.py` & `research_framework-0.2.3/research_framework/plugins/wandb_sweep_plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,55 +8,77 @@
 from research_framework.pipeline.model.pipeline_model import InputFilterModel, MetricModel
 
 import json
 import wandb
 
 from research_framework.plugins.cv_strategies_plugins import RunEnum
 from research_framework.plugins.grid_search_cross_val import WandbSeepsRun
+from research_framework.plugins.wrappers import PullWrapper
 
 
-@Container.bind() #TODO Revisar esto porque parece más un parche que otra cosa
+@Container.bind(DummyFlyManager, PullWrapper) #TODO Revisar esto porque parece más un parche que otra cosa
 class SimpleWandbSeepsAgent(BaseFilterPlugin):
     
     def __init__(self, scorer=MetricModel(clazz='F1'), run_type=RunEnum.unsupervised.name, metrics=[], run_params={}, sweep_id=None, refit=True, filters=[]):
         self.filters = filters
         self.scorer = scorer
         self.refit = refit
         self.run_type = run_type
         self.run_params = run_params
         self.metrics = metrics
         
         sweep_config = generate_sweep_config(self.filters)
         sweep_config['method'] = 'grid'
+        sweep_config['parameters']['dataset'] = {'value':Container.global_config.dataset}
         sweep_config['metric'] = {
             'name': self.scorer.clazz,
             'goal': 'maximize' if self.scorer.higher_better else 'minimize'
         }
         
+        print(sweep_config)
+        
         if sweep_id is None:
             self.sweep_id = wandb.sweep(sweep_config, project=Container.global_config.project_name)
         else:
             self.sweep_id = sweep_id
             
+        Container.send_to_logger({"Sweep": self.sweep_id})
+            
         self.best_config:str = None
         self.best_pipeline:WandbSeepsRun = None
     
     def get_params(self, _: bool = True) -> dict:
         return json.loads(self.best_config)
     
     def fit(self, x):
-        run = getattr(RunEnum, self.run_type).value(x, scorer=self.scorer.clazz, metrics=list(map(lambda x: x.clazz , self.metrics)),  **self.run_params)
-        wandb.agent(self.sweep_id, lambda: {run.exec(), run.log_metrics()}, project=Container.global_config.project_name)
-
+        RunClazz = getattr(RunEnum, self.run_type).value
+        run = RunClazz(x, scorer=self.scorer.clazz, metrics=list(map(lambda x: x.clazz , self.metrics)), dataset=Container.global_config.dataset, **self.run_params)
+        
+        Container.freeze_wandb_logger()
+        
+        wandb.agent(self.sweep_id, lambda: {
+            run.init(),
+            run.exec(), 
+            run.log_metrics(),
+            run.finish()
+        }, project=Container.global_config.project_name)
+        
+        wandb.teardown()
+        
         api = wandb.Api()
         sweep = api.sweep(f"citius-irlab/{Container.global_config.project_name}/sweeps/{self.sweep_id}")
         best_run = sweep.best_run(order=self.scorer.clazz)
         
         self.best_conf = best_run.config
-        self.best_pipeline = run.get_pipeline(best_run.name, best_run.config, InputFilterModel(name="", clazz='MeMPlugin', params={"obj": x}))
+        
+        input_dm = InputFilterModel(name="", clazz='MeMPlugin', params={"obj": x})
+        
+        self.best_pipeline = run.get_pipeline(best_run.name, best_run.config, input_dm)
+        self.best_pipeline.init()
+        self.best_pipeline.fit(input_dm)
         
     def predict(self, x):
         if self.best_pipeline is None:
             raise Exception("Model not trained")
         
         return self.best_pipeline.predict(InputFilterModel(name="", clazz='MeMPlugin', params={"obj": x}))
```

### Comparing `research_framework-0.2.2/research_framework/plugins/wrappers.py` & `research_framework-0.2.3/research_framework/plugins/wrappers.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,48 @@
     def fit(self, *args, **kwargs):
         return self.plugin.fit(*args, **kwargs)
     
     def predict(self, *args, **kwargs):
         return self.plugin.predict(*args, **kwargs)
 
 
+class PullWrapper(BaseWrapper):
+    @methdispatch
+    def fit(self, x):
+        raise TypeError(f"Wrong input type {type(x)}")
+    
+    @methdispatch
+    def predict(self, x):
+        raise TypeError(f"Wrong input type {type(x)}")
 
+    @fit.register
+    def _(self, x:pd.DataFrame) -> BasePlugin:
+        return self.plugin.fit(x, None)
+    
+    @predict.register
+    def _(self, x:pd.DataFrame) -> pd.DataFrame:
+        return self.plugin.predict(x)
+    
+    @fit.register
+    def _fit(self, x:StandardDataset):
+        return self.plugin.fit(x)
+    
+    @predict.register
+    def _predict(self, x:StandardDataset):
+        return self.plugin.predict(x)
+    
+    @fit.register
+    def _(self, x:type(lambda:0)):
+        x = x()
+        return self.fit(x)
+    
+    @predict.register
+    def _(self, x:type(lambda:0)):
+        x = x()
+        return self.predict(x)
     
 # Este es para los plugins que transforman texto
 class DataFrameInOutWrapper(BaseWrapper):
     @methdispatch
     def fit(self, x):
         raise TypeError(f"Wrong input type {type(x)}")
```

### Comparing `research_framework-0.2.2/research_framework/storage/google_storage.py` & `research_framework-0.2.3/research_framework/storage/google_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/storage/local_storage.py` & `research_framework-0.2.3/research_framework/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework/storage/s3_storage.py` & `research_framework-0.2.3/research_framework/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/research_framework.egg-info/PKG-INFO` & `research_framework-0.2.3/research_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-framework
-Version: 0.2.2
+Version: 0.2.3
 Summary: framework base para investigación
 Home-page: https://github.com/manucouto1/research_framework
 Author: Manuel Couto Pintos
 Author-email: manuel.couto.pintos@usc.es
 License: Apache License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -23,14 +23,14 @@
 Requires-Dist: pytest==7.4.0
 Requires-Dist: pandas==2.1.0
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: scikit-fuzzy==0.4.2
 Requires-Dist: torch==2.0.1
 Requires-Dist: transformers[torch]==4.33.0
 Requires-Dist: sentence-transformers[torch]==2.2.2
-Requires-Dist: wandb==0.16.0
+Requires-Dist: wandb==0.16.6
 Requires-Dist: atpbar==1.1.4
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: rich==13.5.2
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: boto3==1.34.16
 Requires-Dist: randomname
```

### Comparing `research_framework-0.2.2/research_framework.egg-info/SOURCES.txt` & `research_framework-0.2.3/research_framework.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 research_framework/flyweight/model/item_simple_model.py
 research_framework/neural_models/__init__.py
 research_framework/neural_models/doomy_model.py
 research_framework/pipeline/__init__.py
 research_framework/pipeline/inputs.py
 research_framework/pipeline/pipeline.py
 research_framework/pipeline/pipeline_manager.py
+research_framework/pipeline/exceptions/__init__.py
+research_framework/pipeline/exceptions/pipeline_exceptions.py
+research_framework/pipeline/exceptions/run_exceptions.py
 research_framework/pipeline/model/__init__.py
 research_framework/pipeline/model/pipeline_model.py
 research_framework/plugins/__init__.py
 research_framework/plugins/cv_strategies_plugins.py
 research_framework/plugins/data_ingestion_plugins.py
 research_framework/plugins/doomy_predictor.py
 research_framework/plugins/grid_search_cross_val.py
```

### Comparing `research_framework-0.2.2/setup.py` & `research_framework-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         str(requirement)
         for requirement
         in parse_requirements(requirements_txt)
     ]
 
 setup(
     name="research-framework",
-    version='0.2.2',
+    version='0.2.3',
     description="framework base para investigación",
     url="https://github.com/manucouto1/research_framework",
     author="Manuel Couto Pintos",
     author_email="manuel.couto.pintos@usc.es",
     license="Apache License",
     packages=find_packages(),
     install_requires=install_requires,
```

### Comparing `research_framework-0.2.2/test/metrics/test_metrics.py` & `research_framework-0.2.3/test/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/plugins/test_mem_plugins.py` & `research_framework-0.2.3/test/plugins/test_mem_plugins.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/plugins/test_plugin.py` & `research_framework-0.2.3/test/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_container_bindings.py` & `research_framework-0.2.3/test/test_container_bindings.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_flyweight_with_google_storage.py` & `research_framework-0.2.3/test/test_flyweight_with_google_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_flyweight_with_local_storage.py` & `research_framework-0.2.3/test/test_flyweight_with_local_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_flyweight_with_s3_storage.py` & `research_framework-0.2.3/test/test_flyweight_with_s3_storage.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_mem_module.py` & `research_framework-0.2.3/test/test_mem_module.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_pipeline.py` & `research_framework-0.2.3/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_pipeline_grid_search.py` & `research_framework-0.2.3/test/test_pipeline_grid_search.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_simple_pipeline.py` & `research_framework-0.2.3/test/test_simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_simple_pipeline_manager.py` & `research_framework-0.2.3/test/test_simple_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `research_framework-0.2.2/test/test_simple_pipeline_with_sweep_supervised.py` & `research_framework-0.2.3/test/test_simple_pipeline_with_sweep_unsupervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,40 +64,38 @@
                 params={
                     "n_components":5
                 } 
             ),
             FilterModel(
                 clazz="SimpleWandbSeepsAgent",
                 params={
-                    "scorer": MetricModel(clazz='F1'),
+                    "scorer": MetricModel(clazz='NMI'),
                     "metrics": [
                         #MetricModel(clazz='NMI')
                     ],
-                    "run_type": "shuffle_cv",
+                    "run_type":"unsupervised",
                     "run_params": {
-                        "n_splits": 3,
-                        "test_size": 0.2,
-                        "random_state": 47
+                        
                     },
                     "filters": [
                         FilterModel(
-                            clazz="DoomyPredictor",
+                            clazz="Kmeans",
                             params={
-                                "emb_d": 5,
-                                
-                                "hidden_d":[2, 4, 8]
+                                "refit": True,
+                                "n_init": "auto",
+                                "n_clusters": [3, 4],
                             }
                         )
                     ],
                 }
             )
         ],
         metrics = [
             MetricModel(
-                clazz="Precision"
+                clazz="Silhouette"
             )
         ]
     )
 
 
 @pytest.fixture
 def simple_pipeline():
@@ -105,15 +103,15 @@
     print(Container.BINDINGS)
     Container.storage = LocalStorage('data/cache')
     Container.fly = SimpleFlyWeight()
     Container.MEM = MEMManager(overwrite=True)
     
     filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
     
-    return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=True, store=True, storage=LocalStorage('data/cache'))
+    return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=True, overwrite=True, store=True, storage=LocalStorage('data/cache'))
     
 
 def aux_delete_pipeline_generated_items(pipeline:SimpleFitPredictPipeline):
     pipeline:SimplePipelineModel = pipeline.pipeline
     
     print("- Input Data:")
     print("__________________________________________________________________________")
@@ -158,15 +156,15 @@
     print(Container.BINDINGS)
     Container.storage = LocalStorage('data/cache')
     Container.fly = SimpleFlyWeight()
     Container.MEM = MEMManager(overwrite=True)
     
     filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
     
-    return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=False, store=True, storage=LocalStorage('data/cache'))
+    PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=False, store=True, storage=LocalStorage('data/cache'))
     
 
 
 def test_stored_items_types_and_wrappers(delete_pipeline_items: Any):
     pipeline:SimpleFitPredictPipeline = delete_pipeline_items
     print(pipeline.pipeline)
     for item in pipeline.pipeline.train_input.items.values():
```

### Comparing `research_framework-0.2.2/test/test_simple_pipeline_with_sweep_unsupervised.py` & `research_framework-0.2.3/test/test_simple_pipeline_with_sweep_supervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from research_framework.base.plugin.base_plugin import BasePlugin
 from research_framework.base.plugin.base_wrapper import BaseWrapper
 from research_framework.container.container import Container
 from research_framework.dataset.standard_dataset import StandardDataset
 from research_framework.flyweight.flyweight import SimpleFlyWeight
 from research_framework.flyweight.mem_manager import MEMManager
 from research_framework.flyweight.model.item_simple_model import ItemSimpleModel
+from research_framework.pipeline.exceptions.pipeline_exceptions import PipelineExecutionException
 from research_framework.pipeline.model.pipeline_model import FilterModel, InputFilterModel, MetricModel, SimpleInputFilterModel, SimplePipelineModel
 from research_framework.plugins.wandb_sweep_plugins import *
 from research_framework.plugins.unsupervised_predictor import *
 from research_framework.pipeline.pipeline import SimpleFitPredictPipeline
 from research_framework.pipeline.pipeline_manager import PipelineManager
 from research_framework.storage.local_storage import LocalStorage
 
 import pytest
 import pandas as pd
 import copy
 from rich import print
+import traceback
 
 test_pipeline = SimplePipelineModel(
         name='pipeline para tests',
         train_input= 
             SimpleInputFilterModel(
                 clazz='CSVPlugin',
                 name='sample_2000_standard_depression_train_2017.csv',
@@ -64,54 +66,60 @@
                 params={
                     "n_components":5
                 } 
             ),
             FilterModel(
                 clazz="SimpleWandbSeepsAgent",
                 params={
-                    "scorer": MetricModel(clazz='NMI'),
+                    "scorer": MetricModel(clazz='F1'),
                     "metrics": [
                         #MetricModel(clazz='NMI')
                     ],
-                    "run_type":"unsupervised",
+                    "run_type": "shuffle_cv",
                     "run_params": {
-                        
+                        "n_splits": 3,
+                        "test_size": 0.2,
+                        "random_state": 47
                     },
                     "filters": [
                         FilterModel(
-                            clazz="Kmeans",
+                            clazz="DoomyPredictor",
                             params={
-                                "refit": True,
-                                "n_init": "auto",
-                                "n_clusters": [3, 4],
+                                "emb_d": 5,
+                                
+                                "hidden_d":[2, 4, 8]
                             }
                         )
                     ],
                 }
             )
         ],
         metrics = [
             MetricModel(
-                clazz="Silhouette"
+                clazz="Precision"
             )
         ]
     )
 
 
 @pytest.fixture
 def simple_pipeline():
-    print("\n* Container content: ")
-    print(Container.BINDINGS)
-    Container.storage = LocalStorage('data/cache')
-    Container.fly = SimpleFlyWeight()
-    Container.MEM = MEMManager(overwrite=True)
-    
-    filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
-    
-    return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=True, store=True, storage=LocalStorage('data/cache'))
+    try:
+        print("\n* Container content: ")
+        print(Container.BINDINGS)
+        Container.storage = LocalStorage('data/cache')
+        Container.fly = SimpleFlyWeight()
+        Container.MEM = MEMManager(overwrite=True)
+        
+        filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
+        
+        return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=True, overwrite=True, store=True, storage=LocalStorage('data/cache'))
+    except PipelineExecutionException:
+        traceback.print_exc()
+        assert False
     
 
 def aux_delete_pipeline_generated_items(pipeline:SimpleFitPredictPipeline):
     pipeline:SimplePipelineModel = pipeline.pipeline
     
     print("- Input Data:")
     print("__________________________________________________________________________")
@@ -150,21 +158,25 @@
 
 
 def test_pipeline_with_prev_stored_items(delete_pipeline_items: Any):
     pipeline:SimpleFitPredictPipeline = delete_pipeline_items
 
     print("\n* Container content: ")
     print(Container.BINDINGS)
-    Container.storage = LocalStorage('data/cache')
-    Container.fly = SimpleFlyWeight()
-    Container.MEM = MEMManager(overwrite=True)
-    
-    filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
-    
-    return PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=False, store=True, storage=LocalStorage('data/cache'))
+    try:
+        Container.storage = LocalStorage('data/cache')
+        Container.fly = SimpleFlyWeight()
+        Container.MEM = MEMManager(overwrite=True)
+        
+        filled_config = PipelineManager.fill_pipline_items(copy.deepcopy(test_pipeline))
+        
+        PipelineManager.start_pipeline(project='test', pl_conf=filled_config, log=False, overwrite=False, store=True, storage=LocalStorage('data/cache'))
+    except PipelineExecutionException:
+        traceback.print_exc()
+        assert False
     
 
 
 def test_stored_items_types_and_wrappers(delete_pipeline_items: Any):
     pipeline:SimpleFitPredictPipeline = delete_pipeline_items
     print(pipeline.pipeline)
     for item in pipeline.pipeline.train_input.items.values():
```

### Comparing `research_framework-0.2.2/test/test_wrappers_type_validation.py` & `research_framework-0.2.3/test/test_wrappers_type_validation.py`

 * *Files identical despite different names*

