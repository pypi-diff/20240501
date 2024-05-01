# Comparing `tmp/blechpy-2.2.7.tar.gz` & `tmp/blechpy-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blechpy-2.2.7.tar", last modified: Mon Aug 21 17:42:04 2023, max compression
+gzip compressed data, was "dist/blechpy-2.2.8.tar", last modified: Mon Aug 21 17:47:46 2023, max compression
```

## Comparing `blechpy-2.2.7.tar` & `blechpy-2.2.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1055 2021-06-14 16:20:28.000000 blechpy-2.2.7/LICENSE
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      122 2021-06-14 16:20:28.000000 blechpy-2.2.7/MANIFEST.in
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-21 17:42:04.000000 blechpy-2.2.7/PKG-INFO
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    13849 2023-08-01 16:45:44.000000 blechpy-2.2.7/README.md
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      430 2023-06-28 22:29:28.000000 blechpy-2.2.7/blechpy/__init__.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/analysis/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    65368 2021-11-18 18:57:35.000000 blechpy-2.2.7/blechpy/analysis/blech_clustering.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    11522 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/circus_interface.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2734 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/clustering.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/analysis/defaults/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      850 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/defaults/bilateral32.prb
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2797 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/defaults/default_config.params
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    12715 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/held_unit_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    25063 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/palatability_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    68071 2023-08-21 17:38:07.000000 blechpy-2.2.7/blechpy/analysis/poissonHMM.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    55747 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/poissonHMM_deprecated.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     9485 2022-07-14 00:49:50.000000 blechpy-2.2.7/blechpy/analysis/spike_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      516 2021-11-12 15:27:15.000000 blechpy-2.2.7/blechpy/analysis/spike_detection.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10253 2022-08-24 19:14:57.000000 blechpy-2.2.7/blechpy/analysis/spike_sorting.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1220 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/analysis/stat_tests.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/datastructures/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/datastructures/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    63858 2023-06-16 18:07:52.000000 blechpy-2.2.7/blechpy/datastructures/dataset.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    18325 2022-08-09 19:53:31.000000 blechpy-2.2.7/blechpy/datastructures/experiment.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5165 2021-11-12 15:27:15.000000 blechpy-2.2.7/blechpy/datastructures/objects.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8334 2022-12-09 16:30:22.000000 blechpy-2.2.7/blechpy/datastructures/project.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/dio/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      118 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10654 2022-05-23 16:45:59.000000 blechpy-2.2.7/blechpy/dio/blech_params.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/dio/defaults/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1395 2023-02-02 18:51:46.000000 blechpy-2.2.7/blechpy/dio/defaults/CAR_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2053 2022-05-23 18:04:09.000000 blechpy-2.2.7/blechpy/dio/defaults/clustering_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      205 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/defaults/pal_id_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      100 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/defaults/psth_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      124 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/defaults/spike_array_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    49150 2022-10-14 16:51:23.000000 blechpy-2.2.7/blechpy/dio/h5io.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10722 2023-03-09 19:13:34.000000 blechpy-2.2.7/blechpy/dio/hmmIO.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/dio/intanutil/
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/__init__.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     2710 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/data_to_result.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1642 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/get_bytes_per_data_block.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1467 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/notch_filter.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1036 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/qstring.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     6858 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/read_header.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     3649 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/intanutil/read_one_data_block.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)    10224 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/dio/load_intan_rhd_format.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8453 2021-11-12 15:27:15.000000 blechpy-2.2.7/blechpy/dio/rawIO.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3168 2022-02-10 19:18:13.000000 blechpy-2.2.7/blechpy/environment.yml
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/plotting/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      149 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/plotting/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2822 2022-08-11 19:05:52.000000 blechpy-2.2.7/blechpy/plotting/blech_waveforms_datashader.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    29972 2023-03-24 15:16:51.000000 blechpy-2.2.7/blechpy/plotting/data_plot.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    17524 2023-06-28 22:11:05.000000 blechpy-2.2.7/blechpy/plotting/hmm_plot.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    34279 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/plotting/palatability_plot.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy/utils/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      208 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      736 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/cluster_filters.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      970 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/data_reset.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1418 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/decorators.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1311 2021-11-18 19:01:07.000000 blechpy-2.2.7/blechpy/utils/math_tools.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1100 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/memory_monitor.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3547 2021-11-12 15:27:15.000000 blechpy-2.2.7/blechpy/utils/particles.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3752 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/print_tools.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    20821 2023-04-10 17:57:49.000000 blechpy-2.2.7/blechpy/utils/spike_sorting_GUI.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5082 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/tk_widgets.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    19601 2022-08-11 19:06:02.000000 blechpy-2.2.7/blechpy/utils/userIO.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1535 2021-06-14 16:20:28.000000 blechpy-2.2.7/blechpy/utils/write_tools.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/PKG-INFO
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2076 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/SOURCES.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/dependency_links.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      399 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/requires.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        8 2023-08-21 17:42:04.000000 blechpy-2.2.7/blechpy.egg-info/top_level.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-08-21 17:42:04.000000 blechpy-2.2.7/setup.cfg
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1280 2023-08-21 17:39:47.000000 blechpy-2.2.7/setup.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1055 2021-06-14 16:20:28.000000 blechpy-2.2.8/LICENSE
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      122 2021-06-14 16:20:28.000000 blechpy-2.2.8/MANIFEST.in
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-21 17:47:46.000000 blechpy-2.2.8/PKG-INFO
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    13849 2023-08-01 16:45:44.000000 blechpy-2.2.8/README.md
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      430 2023-06-28 22:29:28.000000 blechpy-2.2.8/blechpy/__init__.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/analysis/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    65368 2021-11-18 18:57:35.000000 blechpy-2.2.8/blechpy/analysis/blech_clustering.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    11522 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/circus_interface.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2734 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/clustering.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/analysis/defaults/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      850 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/defaults/bilateral32.prb
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2797 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/defaults/default_config.params
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    12715 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/held_unit_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    25063 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/palatability_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    68031 2023-08-21 17:47:34.000000 blechpy-2.2.8/blechpy/analysis/poissonHMM.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    55747 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/poissonHMM_deprecated.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     9485 2022-07-14 00:49:50.000000 blechpy-2.2.8/blechpy/analysis/spike_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      516 2021-11-12 15:27:15.000000 blechpy-2.2.8/blechpy/analysis/spike_detection.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10253 2022-08-24 19:14:57.000000 blechpy-2.2.8/blechpy/analysis/spike_sorting.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1220 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/analysis/stat_tests.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/datastructures/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/datastructures/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    63858 2023-06-16 18:07:52.000000 blechpy-2.2.8/blechpy/datastructures/dataset.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    18325 2022-08-09 19:53:31.000000 blechpy-2.2.8/blechpy/datastructures/experiment.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5165 2021-11-12 15:27:15.000000 blechpy-2.2.8/blechpy/datastructures/objects.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8334 2022-12-09 16:30:22.000000 blechpy-2.2.8/blechpy/datastructures/project.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/dio/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      118 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10654 2022-05-23 16:45:59.000000 blechpy-2.2.8/blechpy/dio/blech_params.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/dio/defaults/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1395 2023-02-02 18:51:46.000000 blechpy-2.2.8/blechpy/dio/defaults/CAR_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2053 2022-05-23 18:04:09.000000 blechpy-2.2.8/blechpy/dio/defaults/clustering_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      205 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/defaults/pal_id_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      100 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/defaults/psth_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      124 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/defaults/spike_array_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    49150 2022-10-14 16:51:23.000000 blechpy-2.2.8/blechpy/dio/h5io.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10722 2023-03-09 19:13:34.000000 blechpy-2.2.8/blechpy/dio/hmmIO.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/dio/intanutil/
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/__init__.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     2710 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/data_to_result.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1642 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/get_bytes_per_data_block.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1467 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/notch_filter.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1036 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/qstring.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     6858 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/read_header.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     3649 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/intanutil/read_one_data_block.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)    10224 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/dio/load_intan_rhd_format.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8453 2021-11-12 15:27:15.000000 blechpy-2.2.8/blechpy/dio/rawIO.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3168 2022-02-10 19:18:13.000000 blechpy-2.2.8/blechpy/environment.yml
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/plotting/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      149 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/plotting/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2822 2022-08-11 19:05:52.000000 blechpy-2.2.8/blechpy/plotting/blech_waveforms_datashader.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    29972 2023-03-24 15:16:51.000000 blechpy-2.2.8/blechpy/plotting/data_plot.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    17524 2023-06-28 22:11:05.000000 blechpy-2.2.8/blechpy/plotting/hmm_plot.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    34279 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/plotting/palatability_plot.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy/utils/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      208 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      736 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/cluster_filters.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      970 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/data_reset.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1418 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/decorators.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1311 2021-11-18 19:01:07.000000 blechpy-2.2.8/blechpy/utils/math_tools.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1100 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/memory_monitor.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3547 2021-11-12 15:27:15.000000 blechpy-2.2.8/blechpy/utils/particles.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3752 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/print_tools.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    20821 2023-04-10 17:57:49.000000 blechpy-2.2.8/blechpy/utils/spike_sorting_GUI.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5082 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/tk_widgets.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    19601 2022-08-11 19:06:02.000000 blechpy-2.2.8/blechpy/utils/userIO.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1535 2021-06-14 16:20:28.000000 blechpy-2.2.8/blechpy/utils/write_tools.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/PKG-INFO
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2076 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      399 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/requires.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        8 2023-08-21 17:47:46.000000 blechpy-2.2.8/blechpy.egg-info/top_level.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-08-21 17:47:46.000000 blechpy-2.2.8/setup.cfg
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1280 2023-08-21 17:46:39.000000 blechpy-2.2.8/setup.py
```

### Comparing `blechpy-2.2.7/LICENSE` & `blechpy-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/PKG-INFO` & `blechpy-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blechpy
-Version: 2.2.7
+Version: 2.2.8
 Summary: Package for exrtacting, processing and analyzing Intan and OpenEphys data
 Home-page: https://github.com/nubs01/blechpy
 Author: Roshan Nanu, Daniel Svedberg
 Author-email: roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com
 License: UNKNOWN
 Keywords: blech katz_lab Intan electrophysiology neuroscience
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blechpy Version: 2.2.7 Summary: Package for
+Metadata-Version: 2.1 Name: blechpy Version: 2.2.8 Summary: Package for
 exrtacting, processing and analyzing Intan and OpenEphys data Home-page: https:
 //github.com/nubs01/blechpy Author: Roshan Nanu, Daniel Svedberg Author-email:
 roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com License: UNKNOWN Keywords:
 blech katz_lab Intan electrophysiology neuroscience Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `blechpy-2.2.7/README.md` & `blechpy-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/blech_clustering.py` & `blechpy-2.2.8/blechpy/analysis/blech_clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/circus_interface.py` & `blechpy-2.2.8/blechpy/analysis/circus_interface.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/clustering.py` & `blechpy-2.2.8/blechpy/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/defaults/bilateral32.prb` & `blechpy-2.2.8/blechpy/analysis/defaults/bilateral32.prb`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/defaults/default_config.params` & `blechpy-2.2.8/blechpy/analysis/defaults/default_config.params`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/held_unit_analysis.py` & `blechpy-2.2.8/blechpy/analysis/held_unit_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/palatability_analysis.py` & `blechpy-2.2.8/blechpy/analysis/palatability_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/poissonHMM.py` & `blechpy-2.2.8/blechpy/analysis/poissonHMM.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,15 @@
     """Gives probability of each neurons spike count assuming poisson spiking
     """
     tmp = n * np.log(rate * dt) - np.array([np.log(fast_factorial(x)) for x in n])
     tmp = tmp - rate * dt
     tmp = np.exp(tmp)
     tmp[rate > 150] = MIN_PROB  # cap rate at 150, since neurons don't really fire that fast
     tmp[((rate < MIN_PROB) & (n == 0))] = 1.0
-    tmp = np.nan_to_num(tmp, copy=False, nan=MIN_PROB, posinf=MIN_PROB, neginf=MIN_PROB)
-
+    tmp[((rate < MIN_PROB) & (n > 0))] = MIN_PROB
     return tmp
 
 
 @njit
 def log_emission(rate, n, dt):
     return np.sum(np.log(poisson(rate, n, dt)))
```

### Comparing `blechpy-2.2.7/blechpy/analysis/poissonHMM_deprecated.py` & `blechpy-2.2.8/blechpy/analysis/poissonHMM_deprecated.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/spike_analysis.py` & `blechpy-2.2.8/blechpy/analysis/spike_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/spike_detection.py` & `blechpy-2.2.8/blechpy/analysis/spike_detection.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/spike_sorting.py` & `blechpy-2.2.8/blechpy/analysis/spike_sorting.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/analysis/stat_tests.py` & `blechpy-2.2.8/blechpy/analysis/stat_tests.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/datastructures/dataset.py` & `blechpy-2.2.8/blechpy/datastructures/dataset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/datastructures/experiment.py` & `blechpy-2.2.8/blechpy/datastructures/experiment.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/datastructures/objects.py` & `blechpy-2.2.8/blechpy/datastructures/objects.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/datastructures/project.py` & `blechpy-2.2.8/blechpy/datastructures/project.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/blech_params.py` & `blechpy-2.2.8/blechpy/dio/blech_params.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/defaults/CAR_params.json` & `blechpy-2.2.8/blechpy/dio/defaults/CAR_params.json`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/defaults/clustering_params.json` & `blechpy-2.2.8/blechpy/dio/defaults/clustering_params.json`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/h5io.py` & `blechpy-2.2.8/blechpy/dio/h5io.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/hmmIO.py` & `blechpy-2.2.8/blechpy/dio/hmmIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/data_to_result.py` & `blechpy-2.2.8/blechpy/dio/intanutil/data_to_result.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/get_bytes_per_data_block.py` & `blechpy-2.2.8/blechpy/dio/intanutil/get_bytes_per_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/notch_filter.py` & `blechpy-2.2.8/blechpy/dio/intanutil/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/qstring.py` & `blechpy-2.2.8/blechpy/dio/intanutil/qstring.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/read_header.py` & `blechpy-2.2.8/blechpy/dio/intanutil/read_header.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/intanutil/read_one_data_block.py` & `blechpy-2.2.8/blechpy/dio/intanutil/read_one_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/load_intan_rhd_format.py` & `blechpy-2.2.8/blechpy/dio/load_intan_rhd_format.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/dio/rawIO.py` & `blechpy-2.2.8/blechpy/dio/rawIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/environment.yml` & `blechpy-2.2.8/blechpy/environment.yml`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/plotting/blech_waveforms_datashader.py` & `blechpy-2.2.8/blechpy/plotting/blech_waveforms_datashader.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/plotting/data_plot.py` & `blechpy-2.2.8/blechpy/plotting/data_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/plotting/hmm_plot.py` & `blechpy-2.2.8/blechpy/plotting/hmm_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/plotting/palatability_plot.py` & `blechpy-2.2.8/blechpy/plotting/palatability_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/cluster_filters.py` & `blechpy-2.2.8/blechpy/utils/cluster_filters.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/data_reset.py` & `blechpy-2.2.8/blechpy/utils/data_reset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/decorators.py` & `blechpy-2.2.8/blechpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/math_tools.py` & `blechpy-2.2.8/blechpy/utils/math_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/memory_monitor.py` & `blechpy-2.2.8/blechpy/utils/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/particles.py` & `blechpy-2.2.8/blechpy/utils/particles.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/print_tools.py` & `blechpy-2.2.8/blechpy/utils/print_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/spike_sorting_GUI.py` & `blechpy-2.2.8/blechpy/utils/spike_sorting_GUI.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/tk_widgets.py` & `blechpy-2.2.8/blechpy/utils/tk_widgets.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/userIO.py` & `blechpy-2.2.8/blechpy/utils/userIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy/utils/write_tools.py` & `blechpy-2.2.8/blechpy/utils/write_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/blechpy.egg-info/PKG-INFO` & `blechpy-2.2.8/blechpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blechpy
-Version: 2.2.7
+Version: 2.2.8
 Summary: Package for exrtacting, processing and analyzing Intan and OpenEphys data
 Home-page: https://github.com/nubs01/blechpy
 Author: Roshan Nanu, Daniel Svedberg
 Author-email: roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com
 License: UNKNOWN
 Keywords: blech katz_lab Intan electrophysiology neuroscience
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blechpy Version: 2.2.7 Summary: Package for
+Metadata-Version: 2.1 Name: blechpy Version: 2.2.8 Summary: Package for
 exrtacting, processing and analyzing Intan and OpenEphys data Home-page: https:
 //github.com/nubs01/blechpy Author: Roshan Nanu, Daniel Svedberg Author-email:
 roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com License: UNKNOWN Keywords:
 blech katz_lab Intan electrophysiology neuroscience Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `blechpy-2.2.7/blechpy.egg-info/SOURCES.txt` & `blechpy-2.2.8/blechpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.7/setup.py` & `blechpy-2.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = [] # Examples: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     name='blechpy',
-    version='2.2.7',
+    version='2.2.8',
     author='Roshan Nanu, Daniel Svedberg',
     author_email='roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com',
     description='Package for exrtacting, processing and analyzing Intan and OpenEphys data',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/nubs01/blechpy',
     packages=setuptools.find_packages(),
```

