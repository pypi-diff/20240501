# Comparing `tmp/strax-1.6.2.tar.gz` & `tmp/strax-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.6.2.tar", last modified: Fri Apr  5 01:14:17 2024, max compression
+gzip compressed data, was "strax-1.6.3.tar", last modified: Tue Apr 30 23:08:24 2024, max compression
```

## Comparing `strax-1.6.2.tar` & `strax-1.6.3.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.137385 strax-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-05 01:14:12.000000 strax-1.6.2/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-05 01:14:12.000000 strax-1.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    25061 2024-04-05 01:14:12.000000 strax-1.6.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-05 01:14:12.000000 strax-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 01:14:12.000000 strax-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-05 01:14:17.137385 strax-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-05 01:14:12.000000 strax-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-05 01:14:12.000000 strax-1.6.2/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 01:14:12.000000 strax-1.6.2/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 01:14:12.000000 strax-1.6.2/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 01:14:12.000000 strax-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-05 01:14:17.137385 strax-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-05 01:14:12.000000 strax-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/strax/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-05 01:14:12.000000 strax-1.6.2/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 01:14:12.000000 strax-1.6.2/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-05 01:14:12.000000 strax-1.6.2/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-05 01:14:12.000000 strax-1.6.2/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    99037 2024-04-05 01:14:12.000000 strax-1.6.2/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-04-05 01:14:12.000000 strax-1.6.2/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-05 01:14:12.000000 strax-1.6.2/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 01:14:12.000000 strax-1.6.2/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-05 01:14:12.000000 strax-1.6.2/strax/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/down_chunking_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-04-05 01:14:12.000000 strax-1.6.2/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-05 01:14:12.000000 strax-1.6.2/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-04-05 01:14:12.000000 strax-1.6.2/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.133385 strax-1.6.2/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-05 01:14:12.000000 strax-1.6.2/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-05 01:14:12.000000 strax-1.6.2/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-04-05 01:14:12.000000 strax-1.6.2/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.129385 strax-1.6.2/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 01:14:17.000000 strax-1.6.2/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:17.137385 strax-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 01:14:12.000000 strax-1.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_down_chunk_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-05 01:14:12.000000 strax-1.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.442614 strax-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-30 23:08:22.000000 strax-1.6.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-30 23:08:22.000000 strax-1.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    26918 2024-04-30 23:08:22.000000 strax-1.6.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 23:08:22.000000 strax-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:08:22.000000 strax-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-30 23:08:24.442614 strax-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 23:08:22.000000 strax-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.430614 strax-1.6.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-30 23:08:22.000000 strax-1.6.3/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.430614 strax-1.6.3/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 23:08:22.000000 strax-1.6.3/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 23:08:22.000000 strax-1.6.3/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 23:08:22.000000 strax-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-30 23:08:24.442614 strax-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-30 23:08:22.000000 strax-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 23:08:22.000000 strax-1.6.3/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 23:08:22.000000 strax-1.6.3/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-30 23:08:22.000000 strax-1.6.3/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-30 23:08:22.000000 strax-1.6.3/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100198 2024-04-30 23:08:22.000000 strax-1.6.3/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-04-30 23:08:22.000000 strax-1.6.3/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-30 23:08:22.000000 strax-1.6.3/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-30 23:08:22.000000 strax-1.6.3/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-30 23:08:22.000000 strax-1.6.3/strax/mailbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/down_chunking_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.438614 strax-1.6.3/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20586 2024-04-30 23:08:22.000000 strax-1.6.3/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.438614 strax-1.6.3/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-30 23:08:22.000000 strax-1.6.3/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27398 2024-04-30 23:08:22.000000 strax-1.6.3/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.442614 strax-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_down_chunk_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_utils.py
```

### Comparing `strax-1.6.2/CODE-OF-CONDUCT.md` & `strax-1.6.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/CONTRIBUTING.md` & `strax-1.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/HISTORY.md` & `strax-1.6.3/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+1.6.3 / 2024-04-30
+---------------------
+* Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
+* Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
+* Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
+* Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
+* Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
+* Check the consistency of number of items in metadata and data in `dry_load_files` function by @dachengx in https://github.com/AxFoundation/strax/pull/824
+* Remove `strax.plugin` by @dachengx in https://github.com/AxFoundation/strax/pull/825
+* Pick out selection applying function by @dachengx in https://github.com/AxFoundation/strax/pull/826
+* Add `CutList` by @dachengx in https://github.com/AxFoundation/strax/pull/827
+* Update tags handling, added comment field. Allows to define superuns … by @WenzDaniel in https://github.com/AxFoundation/strax/pull/798
+* Prevent start being negative by @dachengx in https://github.com/AxFoundation/strax/pull/828
+* Tiny change on the trailing space by @dachengx in https://github.com/AxFoundation/strax/pull/830
+* Add `register_cut_list` by @dachengx in https://github.com/AxFoundation/strax/pull/831
+* Record all base classes when multiple inheritance by @dachengx in https://github.com/AxFoundation/strax/pull/832
+* Multiple output `DownChunkingPlugin` by @dachengx in https://github.com/AxFoundation/strax/pull/833
+* Add `ExhaustPlugin` that exhausts all chunks when fetching data by @dachengx in https://github.com/AxFoundation/strax/pull/835
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.2...v1.6.3
+
+
 1.6.2 / 2024-04-04
 ---------------------
 * Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
 * Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
 * Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
 * Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `strax-1.6.2/LICENSE` & `strax-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/PKG-INFO` & `strax-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.2
+Version: 1.6.3
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,36 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.3 / 2024-04-30
+---------------------
+* Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
+* Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
+* Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
+* Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
+* Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
+* Check the consistency of number of items in metadata and data in `dry_load_files` function by @dachengx in https://github.com/AxFoundation/strax/pull/824
+* Remove `strax.plugin` by @dachengx in https://github.com/AxFoundation/strax/pull/825
+* Pick out selection applying function by @dachengx in https://github.com/AxFoundation/strax/pull/826
+* Add `CutList` by @dachengx in https://github.com/AxFoundation/strax/pull/827
+* Update tags handling, added comment field. Allows to define superuns … by @WenzDaniel in https://github.com/AxFoundation/strax/pull/798
+* Prevent start being negative by @dachengx in https://github.com/AxFoundation/strax/pull/828
+* Tiny change on the trailing space by @dachengx in https://github.com/AxFoundation/strax/pull/830
+* Add `register_cut_list` by @dachengx in https://github.com/AxFoundation/strax/pull/831
+* Record all base classes when multiple inheritance by @dachengx in https://github.com/AxFoundation/strax/pull/832
+* Multiple output `DownChunkingPlugin` by @dachengx in https://github.com/AxFoundation/strax/pull/833
+* Add `ExhaustPlugin` that exhausts all chunks when fetching data by @dachengx in https://github.com/AxFoundation/strax/pull/835
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.2...v1.6.3
+
+
 1.6.2 / 2024-04-04
 ---------------------
 * Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
 * Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
 * Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
 * Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `strax-1.6.2/README.md` & `strax-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/bin/rechunker` & `strax-1.6.3/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/setup.cfg` & `strax-1.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/setup.py` & `strax-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="strax",
-    version="1.6.2",
+    version="1.6.3",
     description="Streaming analysis for xenon TPCs",
     author="strax developers",
     url="https://github.com/AxFoundation/strax",
     setup_requires=["pytest-runner"],
     install_requires=requires,
     tests_require=requires + tests_requires,
     long_description=readme + "\n\n" + history,
```

### Comparing `strax-1.6.2/strax/__init__.py` & `strax-1.6.3/strax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.6.2/strax/chunk.py` & `strax-1.6.3/strax/chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             raise ValueError(f"Attempt to create chunk {self} with data that isn't a numpy array")
         expected_dtype = strax.remove_titles_from_dtype(dtype)
         got_dtype = strax.remove_titles_from_dtype(dtype)
         if expected_dtype != got_dtype:
             raise ValueError(
                 f"Attempt to create chunk {self} with data of {dtype}, should be {expected_dtype}"
             )
+        if self.start < 0:
+            raise ValueError(f"Attempt to create chunk {self} with negative start time")
         if self.start > self.end:
             raise ValueError(f"Attempt to create chunk {self} with negative length")
 
         if len(self.data):
             data_starts_at = self.data[0]["time"]
             # Check the last 500 samples (arbitrary number) as sanity check
             data_ends_at = strax.endtime(self.data[-500:]).max()
```

### Comparing `strax-1.6.2/strax/config.py` & `strax-1.6.3/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/context.py` & `strax-1.6.3/strax/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import strax
 import inspect
 import types
 from collections import defaultdict
 from immutabledict import immutabledict
 from enum import IntEnum
 
+from strax import CutList
+
 
 export, __all__ = strax.exporter()
 __all__.extend(["RUN_DEFAULTS_KEY"])
 
 RUN_DEFAULTS_KEY = "strax_defaults"
 
 # use tqdm as loaded in utils (from tqdm.notebook when in a juypyter env)
@@ -315,14 +317,17 @@
         """
         if isinstance(plugin_class, (tuple, list)):
             # Shortcut for multiple registration
             for x in plugin_class:
                 self.register(x)
             return
 
+        if not issubclass(plugin_class, strax.Plugin):
+            raise ValueError(f"Can only register subclasses of strax.Plugin, not {plugin_class}!")
+
         if not hasattr(plugin_class, "provides"):
             # No output name specified: construct one from the class name
             snake_name = strax.camel_to_snake(plugin_class.__name__)
             plugin_class.provides = (snake_name,)
 
         # Ensure plugin_class.provides is a tuple
         if isinstance(plugin_class.provides, str):
@@ -409,15 +414,15 @@
             all_provides = set()
             plugins_to_deregister = []
 
             for p in self._plugin_class_registry.values():
                 all_provides |= set(p.provides)
 
             for p_key, p in self._plugin_class_registry.items():
-                requires = set(strax.to_str_tuple(p.depends_on))
+                requires = set(strax.to_str_tuple(p().depends_on))
                 if not requires.issubset(all_provides):
                     plugins_to_deregister.append(p_key)
 
             for p_key in plugins_to_deregister:
                 self.log.info(f"Deregister {p_key}")
                 del self._plugin_class_registry[p_key]
 
@@ -497,15 +502,15 @@
                             if plug.__class__.__name__ == "type":
                                 # Make sure we have the instance, not the class:
                                 # >>> class A: pass
                                 # >>> A.__class__.__name__
                                 # 'type'
                                 # >>> A().__class__.__name__
                                 # 'A'
-                                plug = plug()
+                                plug = plug()  # type: ignore
                             result += [f"{plug.__class__.__name__}.{attribute_name}"]
                             # Likely to be used several other times
                             break
         return result
 
     def show_config(self, data_type=None, pattern="*", run_id="9" * 20):
         """Return configuration options that affect data_type.
@@ -571,14 +576,36 @@
         for x in dir(module):
             x = getattr(module, x)
             if not isinstance(x, type(type)):
                 continue
             if issubclass(x, strax.Plugin):
                 self.register(x)
 
+    def register_cut_list(self, cut_list):
+        """Register cut lists to strax context.
+
+        :param cut_list: cut lists to be registered. can be cutlist object or list/tuple of cutlist
+            objects
+
+        """
+        assert not isinstance(
+            cut_list, str
+        ), "Please don't put string... use cutlist object or list/tuple of cutlist objects"
+        if hasattr(cut_list, "__len__"):
+            for _cut_list in cut_list:
+                self.register_cut_list(_cut_list)
+        else:
+            for cut in cut_list.cuts:
+                # maybe cutlist within cutlist?
+                if CutList in cut.__bases__:
+                    self.register_cut_list(cut)
+                else:
+                    self.register(cut)
+            self.register(cut_list)
+
     def data_info(self, data_name: str) -> pd.DataFrame:
         """Return pandas DataFrame describing fields in data_name."""
         p = self._get_plugins((data_name,), run_id="0")[data_name]
         display_headers = ["Field name", "Data type", "Comment"]
         result = []
         for name, dtype in strax.utils.unpack_dtype(p.dtype_for(data_name)):
             if isinstance(name, tuple):
@@ -812,16 +839,14 @@
         last_provide = [d_provides for d_provides in plugin.provides][-1]
 
         if plugin.child_plugin:
             # Plugin is a child of another plugin, hence we have to
             # drop the parents config from the lineage
             configs = {}
 
-            # Getting information about the parent:
-            parent_class = plugin.__class__.__bases__[0]
             # Get all parent options which are overwritten by a child:
             parent_options = [
                 option.parent_option_name
                 for option in plugin.takes_config.values()
                 if option.child_option
             ]
 
@@ -833,15 +858,16 @@
                     continue
 
                 if plugin.takes_config[option_name].track:
                     # Add all options which should be tracked:
                     configs[option_name] = v
 
             # Also adding name and version of the parent to the lineage:
-            configs[parent_class.__name__] = parent_class.__version__
+            for parent_class in plugin.__class__.__bases__:
+                configs[parent_class.__name__] = parent_class.__version__
 
             plugin.lineage = {
                 last_provide: (plugin.__class__.__name__, plugin.version(run_id), configs)
             }
         else:
             plugin.lineage = {
                 last_provide: (
@@ -1443,15 +1469,15 @@
         ).iter()
 
         try:
             _p, t_start, t_end = self._make_progress_bar(
                 run_id, targets=targets, progress_bar=progress_bar
             )
             with _p as pbar:
-                pbar.last_print_t = time.time()
+                pbar.strax_print_time = time.perf_counter()
                 pbar.mbs = []
                 for n_chunks, result in enumerate(strax.continuity_check(generator), 1):
                     seen_a_chunk = True
                     if not isinstance(result, strax.Chunk):
                         raise ValueError(
                             f"Got type {type(result)} rather than a strax Chunk from the processor!"
                         )
@@ -1466,14 +1492,15 @@
                         drop_columns=drop_columns,
                         time_range=time_range,
                         time_selection=time_selection,
                     )
                     self._update_progress_bar(
                         pbar, t_start, t_end, n_chunks, result.end, result.nbytes
                     )
+                    pbar.strax_print_time = time.perf_counter()
                     yield result
             _p.close()
 
         except GeneratorExit:
             generator.throw(
                 OutsideException(
                     "Terminating due to an exception originating from outside "
@@ -1536,19 +1563,19 @@
                 fraction_done = 1
             pbar.n = np.clip(fraction_done, 0, 1)
         else:
             # Strange, start and endtime are the same, probably we don't
             # have data yet e.g. allow_incomplete == True.
             pbar.n = 0
         # Let's add the postfix which is the info behind the tqdm marker
-        seconds_per_chunk = time.time() - pbar.last_print_t
+        seconds_per_chunk = time.perf_counter() - pbar.strax_print_time
         pbar.mbs.append((nbytes / 1e6) / seconds_per_chunk)
         mbs = np.mean(pbar.mbs)
         if mbs < 1:
-            rate = f"{mbs*1000:.1f} kB/s"
+            rate = f"{mbs * 1000:.1f} kB/s"
         else:
             rate = f"{mbs:.1f} MB/s"
         postfix = f"#{n_chunks} ({seconds_per_chunk:.2f} s). {rate}"
         pbar.set_postfix_str(postfix)
         pbar.update(0)
 
     def make(
@@ -2403,14 +2430,16 @@
 :param multi_run_progress_bar: Display a progress bar for loading multiple runs
 """
 
 get_docs = (
     """
 :param run_id: run id to get
 :param targets: list/tuple of strings of data type names to get
+:param ignore_errors: Return the data for the runs that successfully loaded, even if some runs
+        failed executing.
 :param save: extra data types you would like to save
     to cache, if they occur in intermediate computations.
     Many plugins save automatically anyway.
 :param max_workers: Number of worker threads/processes to spawn.
     In practice more CPUs may be used due to strax's multithreading.
 :param allow_multiple: Allow multiple targets to be computed
     simultaneously without merging the results of the target. This can
```

### Comparing `strax-1.6.2/strax/corrections.py` & `strax-1.6.3/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/dtypes.py` & `strax-1.6.3/strax/dtypes.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/io.py` & `strax-1.6.3/strax/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -106,29 +106,37 @@
     md_path = os.path.join(dirname, metadata_json)
 
     with open(md_path, mode="r") as f:
         metadata = json.loads(f.read())
 
     dtype = literal_eval(metadata["dtype"])
 
-    results = []
-    if chunk_number is None:
-        for chunk_info in metadata["chunks"]:
-            if chunk_info["n"] != 0:
-                results.append(
-                    load_file(
-                        os.path.join(dirname, f"{prefix}-{chunk_info['chunk_i']:06d}"),
-                        metadata["compressor"],
-                        dtype,
-                    )
+    def load_chunk(chunk_info):
+        if chunk_info["n"] != 0:
+            data = load_file(
+                os.path.join(dirname, f"{prefix}-{chunk_info['chunk_i']:06d}"),
+                metadata["compressor"],
+                dtype,
+            )
+            if len(data) != chunk_info["n"]:
+                raise ValueError(
+                    f"Chunk {chunk_info['chunk_i']:06d} has {len(data)} "
+                    f"items, but metadata says {chunk_info['n']}."
                 )
-        results = np.hstack(results)
+        return data if len(data) else np.empty(0, dtype)
+
+    # Load all chunks if chunk_number is None, otherwise load the specified chunk
+    if chunk_number is None:
+        chunk_numbers = list(range(len(metadata["chunks"])))
     else:
+        if not isinstance(chunk_number, int):
+            raise ValueError(f"Chunk number must be an integer, not {chunk_number}.")
         if chunk_number >= len(metadata["chunks"]):
             raise ValueError(f"Chunk {chunk_number:06d} does not exist in {dirname}.")
-        if metadata["chunks"][chunk_number]["n"] != 0:
-            results = load_file(
-                os.path.join(dirname, f"{prefix}-{chunk_number:06d}"),
-                metadata["compressor"],
-                dtype,
-            )
+        chunk_numbers = [chunk_number]
+
+    results = []
+    for c in chunk_numbers:
+        chunk_info = metadata["chunks"][c]
+        results.append(load_chunk(chunk_info))
+    results = np.hstack(results)
     return results if len(results) else np.empty(0, dtype)
```

### Comparing `strax-1.6.2/strax/mailbox.py` & `strax-1.6.3/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/plugins/down_chunking_plugin.py` & `strax-1.6.3/strax/plugins/down_chunking_plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Generator
+
 import strax
 from .plugin import Plugin
 
 export, __all__ = strax.exporter()
 
 
 ##
@@ -22,20 +24,33 @@
 
         if self.parallel:
             raise NotImplementedError(
                 f'Plugin "{self.__class__.__name__}" is a DownChunkingPlugin which '
                 "currently does not support parallel processing."
             )
 
-        if self.multi_output:
-            raise NotImplementedError(
-                f'Plugin "{self.__class__.__name__}" is a DownChunkingPlugin which '
-                "currently does not support multiple outputs. Please only provide "
-                "a single data-type."
-            )
-
     def _iter_compute(self, chunk_i, **inputs_merged):
         return self.do_compute(chunk_i=chunk_i, **inputs_merged)
 
     def _fix_output(self, result, start, end, _dtype=None):
         """Wrapper around _fix_output to support the return of iterators."""
-        return result
+        if self.multi_output and not isinstance(result, Generator):
+            raise ValueError(
+                f"Plugin {self.__class__.__name__} should return a generator in compute method."
+            )
+
+        for _result in result:
+            if isinstance(_result, dict):
+                values = _result.values()
+            else:
+                if self.multi_output:
+                    raise ValueError(
+                        f"{self.__class__.__name__} is multi-output and should "
+                        "provide a generator of dict output."
+                    )
+                values = [_result]
+            if not all(isinstance(v, strax.Chunk) for v in values):
+                raise ValueError(
+                    f"Plugin {self.__class__.__name__} should yield (dict of) "
+                    "strax.Chunk in compute method."
+                )
+            yield _result
```

### Comparing `strax-1.6.2/strax/plugins/loop_plugin.py` & `strax-1.6.3/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/plugins/merge_only_plugin.py` & `strax-1.6.3/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/plugins/overlap_window_plugin.py` & `strax-1.6.3/strax/plugins/overlap_window_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
                 _, self.cached_input[data_kind] = chunk.split(t=prev_split, allow_early_split=True)
                 prev_split = self.cached_input[data_kind].start
 
             unique_starts = set([c.start for c in self.cached_input.values()])
             chunk_starts_are_equal = len(unique_starts) == 1
             if chunk_starts_are_equal:
                 self.log.debug(
-                    f"Success after {try_counter}. Extra time = {cache_inputs_beyond-prev_split} ns"
+                    f"Success after {try_counter}. "
+                    f"Extra time = {cache_inputs_beyond - prev_split} ns"
                 )
                 break
             else:
                 self.log.debug(
                     "Inconsistent start times of the cashed chunks after"
                     f" {try_counter}/{max_trials} passes.\nChunks {self.cached_input}"
                 )
```

### Comparing `strax-1.6.2/strax/plugins/parrallel_source_plugin.py` & `strax-1.6.3/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/plugins/plugin.py` & `strax-1.6.3/strax/plugins/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
     __version__: typing.Optional[str] = "0.0.0"
 
     # For multi-output plugins these should be (immutable)dicts
     data_kind: typing.Union[str, immutabledict, dict]
     dtype: typing.Union[tuple, np.dtype, immutabledict, dict]
 
-    depends_on: tuple
-    provides: tuple
+    depends_on: typing.Union[str, tuple, list]
+    provides: typing.Union[str, tuple, list]
     input_buffer: typing.Dict[str, strax.Chunk]
 
     # Needed for plugins which are inherited from an already existing plugins,
     # indicates such an inheritance.
     child_plugin = False
 
     compressor = "blosc"
@@ -200,21 +200,20 @@
         if self.multi_output:
             # Convert to a dict of numpy dtypes
             if not hasattr(self, "data_kind") or not isinstance(
                 self.data_kind, (dict, immutabledict)
             ):
                 raise ValueError(
                     f"{self.__class__.__name__} has multiple outputs and "
-                    "must declare its data kind as a dict: "
-                    "{dtypename: data kind}."
+                    "must declare its data kind as a dict."
                 )
             if not isinstance(self.dtype, dict):
                 raise ValueError(
                     f"{self.__class__.__name__} has multiple outputs, so its "
-                    "dtype must be specified as a dict: {output: dtype}."
+                    "dtype must be specified as a dict."
                 )
             self.dtype = {k: strax.to_numpy_dtype(dt) for k, dt in self.dtype.items()}
         else:
             # Convert to a numpy dtype
             self.dtype = strax.to_numpy_dtype(self.dtype)
 
         # Check required time information is present
@@ -590,18 +589,18 @@
                 # </start>This warning/check will be deleted, see UserWarning
                 if len(set(tranges.values())) != 1:
                     start = min([v.start for v in kwargs.values()])
                     end = max([v.end for v in kwargs.values()])  # Don't delete
                     message = (
                         "New feature, we are ignoring inconsistent the "
                         "possible ValueError in time ranges for "
-                        f"{self.__class__.__name__} of inputs: {tranges}"
+                        f"{self.__class__.__name__} of inputs: {tranges} "
                         "because this occurred in a save_when.NEVER "
                         "plugin. Report any findings in "
-                        "github.com/AxFoundation/strax/issues/247"
+                        "https://github.com/AxFoundation/strax/issues/247"
                     )
                     warn(message, UserWarning)
                 # This block will be deleted </end>
             elif len(set(tranges.values())) != 1:
                 message = (
                     f"{self.__class__.__name__} got inconsistent time ranges of inputs: {tranges}"
                 )
@@ -621,15 +620,15 @@
         return self._fix_output(result, start, end)
 
     def _fix_output(self, result, start, end, _dtype=None):
         if self.multi_output and _dtype is None:
             if not isinstance(result, dict):
                 raise ValueError(
                     f"{self.__class__.__name__} is multi-output and should "
-                    "provide a dict output {dtypename: result}"
+                    "provide a dict output."
                 )
             return {d: self._fix_output(result[d], start, end, _dtype=d) for d in self.provides}
 
         if _dtype is None:
             assert not self.multi_output
             _dtype = self.provides[0]
```

### Comparing `strax-1.6.2/strax/processing/data_reduction.py` & `strax-1.6.3/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/general.py` & `strax-1.6.3/strax/processing/general.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/hitlets.py` & `strax-1.6.3/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/peak_building.py` & `strax-1.6.3/strax/processing/peak_building.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/peak_merging.py` & `strax-1.6.3/strax/processing/peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/peak_properties.py` & `strax-1.6.3/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/peak_splitting.py` & `strax-1.6.3/strax/processing/peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/pulse_processing.py` & `strax-1.6.3/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processing/statistics.py` & `strax-1.6.3/strax/processing/statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/processor.py` & `strax-1.6.3/strax/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
                     m.max_messages = max_m
 
         # Remove defaultdict-like behaviour; all mailboxes should
         # have been made by now. See #444
         self.mailboxes = dict(self.mailboxes)
         self.log.debug(
             f"Created the following mailboxes: {self.mailboxes} with the "
-            f"following threads: {[(d, m._threads) for d,m in self.mailboxes.items()]}"
+            f"following threads: {[(d, m._threads) for d, m in self.mailboxes.items()]}"
         )
 
     def iter(self):
         target = self.components.targets[0]
         final_generator = self.mailboxes[target].subscribe()
 
         self.log.debug("Starting threads")
```

### Comparing `strax-1.6.2/strax/run_selection.py` & `strax-1.6.3/strax/run_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     docs = docs[["name"] + [x for x in docs.columns.tolist() if x != "name"]]  # type: ignore
     self.runs = docs
 
     # Add available data types,
     # this is kept for the case users directly call list_available
     for d in tqdm(
         check_available,
-        desc="Checking data availability scan_runs",
+        desc="Checking data availability",
         disable=not len(check_available),
     ):
         self.runs[d + "_available"] = np.in1d(self.runs.name.values, self.list_available(d))
 
     return self.runs
 
 
@@ -293,15 +293,19 @@
     )
 
     # Check data availability only for selected datasets
     check_available = tuple(
         set(list(strax.to_str_tuple(available)) + list(self.context_config["check_available"]))
     )
 
-    for d in tqdm(check_available, desc="Checking data availability"):
+    for d in tqdm(
+        check_available,
+        desc="Checking data availability",
+        disable=not len(check_available),
+    ):
         dsets[d + "_available"] = np.in1d(
             dsets.name.values, self.list_available(target=d, runs=dsets.name.values)
         )
 
     # This will help users call select_runs multiple times
     # with same run mode and/or name, but different available
     have_available = strax.to_str_tuple(available)
@@ -388,26 +392,34 @@
         livetime=0,
     )
     keys = []
     starts = []
     tags = set()
     modes = set()
     sources = set()
+    comments = set()
     for _subrunid in data:
-        doc = self.run_metadata(_subrunid, ["start", "end", "mode", "tags", "source"])
+        doc = self.run_metadata(_subrunid, ["start", "end", "mode", "tags", "source", "comments"])
         doc.setdefault(
             "tags",
             [
                 {"name": ""},
             ],
         )
         doc.setdefault("mode", "")
         doc.setdefault("source", "")
+        doc.setdefault(
+            "comments",
+            [
+                {"comment": ""},
+            ],
+        )
 
         tags |= set([tag["name"] for tag in doc["tags"]])
+        comments |= set([comment["comment"] for comment in doc["comments"]])
 
         modes |= set(strax.to_str_tuple(doc["mode"]))
         sources |= set(strax.to_str_tuple(doc["source"]))
         if len(sources) > 1:
             warnings.warn(f'You are defining a superrun with more than one source: "{sources}"')
 
         run_doc_start = doc["start"].replace(tzinfo=pytz.utc)
@@ -417,17 +429,18 @@
         run_md["end"] = max(run_md["end"], run_doc_end)
 
         time_delta = run_doc_end - run_doc_start
         run_md["livetime"] += time_delta.total_seconds()
         keys.append(_subrunid)
         starts.append(run_doc_start)
 
-    run_md["tags"] = tuple(tags)
     run_md["mode"] = tuple(modes)
     run_md["source"] = tuple(sources)
+    run_md["tags"] = [{"name": tag} for tag in tags]
+    run_md["comments"] = [{"comment": comment} for comment in comments]
 
     # Make sure subruns are sorted in time
     sort_index = np.argsort(starts)
     data = {keys[i]: data[keys[i]] for i in sort_index}
 
     # Superrun names must start with an underscore
     if not name.startswith("_"):
```

### Comparing `strax-1.6.2/strax/storage/common.py` & `strax-1.6.3/strax/storage/common.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/storage/file_rechunker.py` & `strax-1.6.3/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/storage/files.py` & `strax-1.6.3/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/storage/mongo.py` & `strax-1.6.3/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/storage/zipfiles.py` & `strax-1.6.3/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/strax/testutils.py` & `strax-1.6.3/strax/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,20 +291,22 @@
 
         count = 0
         for count, r in enumerate(records):
             if count == 5:
                 res = records[offset:count]
                 chunk_end = np.max(strax.endtime(res))
                 offset = count
-                chunk = self.chunk(start=last_start, end=chunk_end, data=res)
+                chunk = self.chunk(
+                    start=last_start, end=chunk_end, data=res, data_type=self.provides[0]
+                )
                 last_start = chunk_end
                 yield chunk
 
         res = records[offset : count + 1]
-        chunk = self.chunk(start=last_start, end=end, data=res)
+        chunk = self.chunk(start=last_start, end=end, data=res, data_type=self.provides[0])
         yield chunk
 
 
 # Used in test_core.py
 run_id = "0"
 
 ##
```

### Comparing `strax-1.6.2/strax/utils.py` & `strax-1.6.3/strax/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,15 +586,15 @@
         final_result = []
         while futures:
             futures_done, _ = wait(futures, return_when=FIRST_COMPLETED)
             for f in futures_done:
                 tasks_done += 1
                 _run_id = futures.pop(f)
                 log.debug(
-                    f"Done with run_id: {_run_id} and {len(run_id_numpy)-tasks_done} are left."
+                    f"Done with run_id: {_run_id} and {len(run_id_numpy) - tasks_done} are left."
                 )
                 pbar.update(1)
                 if f.exception() is not None:
                     if ignore_errors:
                         log.warning(f"Ran into {f.exception()}, ignoring that for now!")
                         failures.append(_run_id)
                         continue
@@ -626,15 +626,15 @@
         else:
             # In case we do not have any run_id sort according to time:
             start_of_runs = [np.min(res["time"]) for res in final_result]
             final_result = [final_result[ind] for ind in np.argsort(start_of_runs)]
         pbar.close()
         if ignore_errors and len(failures):
             log.warning(
-                f"Failures for {len(failures)/len(run_ids):.0%} of runs. Failed for: {failures}"
+                f"Failures for {len(failures) / len(run_ids):.0%} of runs. Failed for: {failures}"
             )
         return final_result
 
 
 @export
 def group_by_kind(dtypes, plugins=None, context=None) -> ty.Dict[str, ty.List]:
     """Return dtypes grouped by data kind i.e. {kind1: [d, d, ...], kind2: [d, d, ...], ...}
@@ -667,14 +667,32 @@
         _n_to = _n_from + c["n"]
         c["n_from"] = _n_from
         c["n_to"] = _n_to
         yield c
 
 
 @export
+def parse_selection(x, selection):
+    """Parse a selection string into a mask that can be used to filter data.
+
+    :param selection: Query string, sequence of strings, or simple function to apply.
+    :return: Boolean indicating the selected items.
+
+    """
+    if hasattr(selection, "__call__"):
+        mask = selection(x)
+    else:
+        if isinstance(selection, (list, tuple)):
+            selection = " & ".join(f"({x})" for x in selection)
+
+        mask = numexpr.evaluate(selection, local_dict={fn: x[fn] for fn in x.dtype.names})
+    return mask
+
+
+@export
 def apply_selection(
     x,
     selection=None,
     selection_str=None,
     keep_columns=None,
     drop_columns=None,
     time_range=None,
@@ -718,23 +736,15 @@
         warn(
             'The option "selection_str" is depricated and will be removed in a future release. '
             'Please use "selection" instead.'
         )
         selection = selection_str
 
     if selection:
-        if hasattr(selection, "__call__"):
-            mask = selection(x)
-        else:
-            if isinstance(selection, (list, tuple)):
-                selection = " & ".join(f"({x})" for x in selection)
-
-            mask = numexpr.evaluate(selection, local_dict={fn: x[fn] for fn in x.dtype.names})
-
-        x = x[mask]
+        x = x[parse_selection(x, selection)]
 
     if keep_columns:
         keep_columns = strax.to_str_tuple(keep_columns)
 
     if drop_columns:
         drop_columns = strax.to_str_tuple(drop_columns)
         keep_columns = []
```

### Comparing `strax-1.6.2/strax.egg-info/PKG-INFO` & `strax-1.6.3/strax.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.2
+Version: 1.6.3
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,36 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.3 / 2024-04-30
+---------------------
+* Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
+* Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
+* Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
+* Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
+* Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
+* Check the consistency of number of items in metadata and data in `dry_load_files` function by @dachengx in https://github.com/AxFoundation/strax/pull/824
+* Remove `strax.plugin` by @dachengx in https://github.com/AxFoundation/strax/pull/825
+* Pick out selection applying function by @dachengx in https://github.com/AxFoundation/strax/pull/826
+* Add `CutList` by @dachengx in https://github.com/AxFoundation/strax/pull/827
+* Update tags handling, added comment field. Allows to define superuns … by @WenzDaniel in https://github.com/AxFoundation/strax/pull/798
+* Prevent start being negative by @dachengx in https://github.com/AxFoundation/strax/pull/828
+* Tiny change on the trailing space by @dachengx in https://github.com/AxFoundation/strax/pull/830
+* Add `register_cut_list` by @dachengx in https://github.com/AxFoundation/strax/pull/831
+* Record all base classes when multiple inheritance by @dachengx in https://github.com/AxFoundation/strax/pull/832
+* Multiple output `DownChunkingPlugin` by @dachengx in https://github.com/AxFoundation/strax/pull/833
+* Add `ExhaustPlugin` that exhausts all chunks when fetching data by @dachengx in https://github.com/AxFoundation/strax/pull/835
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.2...v1.6.3
+
+
 1.6.2 / 2024-04-04
 ---------------------
 * Use parentheses to separate the class name and attributes in the representation of StorageFrontend by @dachengx in https://github.com/AxFoundation/strax/pull/809
 * Specifically install `lxml_html_clean` by @dachengx in https://github.com/AxFoundation/strax/pull/812
 * Add a function to purge unused configs by @dachengx in https://github.com/AxFoundation/strax/pull/800
 * Warn if user checks is_stored for plugin not always saved by @cfuselli in https://github.com/AxFoundation/strax/pull/796
 * Bump urllib3 from 2.2.0 to 2.2.1 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/808
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `strax-1.6.2/strax.egg-info/SOURCES.txt` & `strax-1.6.3/strax.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 strax/chunk.py
 strax/config.py
 strax/context.py
 strax/corrections.py
 strax/dtypes.py
 strax/io.py
 strax/mailbox.py
-strax/plugin.py
 strax/processor.py
 strax/run_selection.py
 strax/testutils.py
 strax/utils.py
 strax.egg-info/PKG-INFO
 strax.egg-info/SOURCES.txt
 strax.egg-info/dependency_links.txt
 strax.egg-info/not-zip-safe
 strax.egg-info/requires.txt
 strax.egg-info/top_level.txt
 strax/plugins/__init__.py
 strax/plugins/cut_plugin.py
 strax/plugins/down_chunking_plugin.py
+strax/plugins/exhaust_plugin.py
 strax/plugins/loop_plugin.py
 strax/plugins/merge_only_plugin.py
 strax/plugins/overlap_window_plugin.py
 strax/plugins/parrallel_source_plugin.py
 strax/plugins/plugin.py
 strax/processing/__init__.py
 strax/processing/data_reduction.py
@@ -59,14 +59,15 @@
 tests/test_config.py
 tests/test_context.py
 tests/test_core.py
 tests/test_corrections.py
 tests/test_cut_plugin.py
 tests/test_data_reduction.py
 tests/test_down_chunk_plugin.py
+tests/test_exhaust_plugin.py
 tests/test_fixed_plugin_cache.py
 tests/test_general_processing.py
 tests/test_get_zarr.py
 tests/test_helpers.py
 tests/test_hitlet.py
 tests/test_inline_plugin.py
 tests/test_lone_hit_integration.py
```

### Comparing `strax-1.6.2/tests/test_child_plugins.py` & `strax-1.6.3/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_config.py` & `strax-1.6.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_context.py` & `strax-1.6.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_core.py` & `strax-1.6.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_corrections.py` & `strax-1.6.3/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_cut_plugin.py` & `strax-1.6.3/tests/test_cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_data_reduction.py` & `strax-1.6.3/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_down_chunk_plugin.py` & `strax-1.6.3/tests/test_down_chunk_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from immutabledict import immutabledict
 from strax.testutils import RecordsWithTimeStructure, DownSampleRecords, run_id
 import strax
 import numpy as np
 
 import os
 import tempfile
 import shutil
@@ -54,14 +55,36 @@
         class TestMultiProcessing(DownSampleRecords):
             parallel = True
 
         st.register(TestMultiProcessing)
         with self.assertRaises(NotImplementedError):
             st.make(run_id, "records_down_chunked", max_workers=2)
 
+    def test_down_chunking_multi_output(self):
+        st = self.get_context(allow_multiprocess=True)
+        st.register(RecordsWithTimeStructure)
+        st.register(DownSampleRecords)
+
+        st.make(run_id, "records", max_workers=1)
+
+        class TestMultiOutput(DownSampleRecords):
+            provides = ("records_down_chunked", "records_down_chunked_copy")
+            data_kind = immutabledict(zip(provides, provides))
+
+            def infer_dtype(self):
+                return {p: DownSampleRecords.dtype for p in self.provides}
+
+            def compute(self, records, start, end):
+                for r in super().compute(records, start, end):
+                    yield r
+
+        st.register(TestMultiOutput)
+        with self.assertRaises(ValueError):
+            st.make(run_id, "records_down_chunked", max_workers=2)
+
     def get_context(self, **kwargs):
         """Simple context to run tests."""
         st = strax.Context(storage=self.get_mock_sf(), check_available=("records",), **kwargs)
         return st
 
     def get_mock_sf(self):
         mock_rundb = [{"name": "0", strax.RUN_DEFAULTS_KEY: dict(base_area=43)}]
```

### Comparing `strax-1.6.2/tests/test_fixed_plugin_cache.py` & `strax-1.6.3/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_general_processing.py` & `strax-1.6.3/tests/test_general_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_get_zarr.py` & `strax-1.6.3/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_helpers.py` & `strax-1.6.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_hitlet.py` & `strax-1.6.3/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_inline_plugin.py` & `strax-1.6.3/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_lone_hit_integration.py` & `strax-1.6.3/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_loop_plugins.py` & `strax-1.6.3/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_mailbox.py` & `strax-1.6.3/tests/test_mailbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         mb.add_reader(test_reader)
         mb.start()
         time.sleep(SHORT_TIMEOUT)
         assert hasattr(test_reader, "got")
         assert test_reader.got == list(range(10))
         mb.cleanup()
-        threads = [f"{t.name} is dead: {True^t.is_alive()}" for t in threading.enumerate()]
+        threads = [f"{t.name} is dead: {True ^ t.is_alive()}" for t in threading.enumerate()]
         assert (
             len(threads) == n_threads_start
         ), f"Not all threads died. \n Threads running are:{threads}"
 
 
 def test_result_timeout():
     """Test that our mailbox tester actually times out.
```

### Comparing `strax-1.6.2/tests/test_mongo_frontend.py` & `strax-1.6.3/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_multi_output.py` & `strax-1.6.3/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_overlap_plugin.py` & `strax-1.6.3/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_peak_merging.py` & `strax-1.6.3/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_peak_processing.py` & `strax-1.6.3/tests/test_peak_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     )
     r_buffer = np.tile(r, n_repeat // len(r) + 1)[: len(time_offset)]
     assert len(r_buffer) == len(time_offset)
     r_buffer["time"] = r_buffer["time"] + time_offset
     assert strax.endtime(r_buffer[-1]) - r_buffer["time"].min() > magic_overflow_time
     r = r_buffer.copy()
     del r_buffer
-    print(f"Array is {r.nbytes/1e6} MB, good luck")
+    print(f"Array is {r.nbytes / 1e6} MB, good luck")
 
     # Do peak finding!
     print(f"Find hits")
     hits = strax.find_hits(r, min_amplitude=0)
     assert len(hits)
     hits = strax.sort_by_time(hits)
```

### Comparing `strax-1.6.2/tests/test_peak_properties.py` & `strax-1.6.3/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_peak_splitting.py` & `strax-1.6.3/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_pulse_processing.py` & `strax-1.6.3/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_saving.py` & `strax-1.6.3/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_statistics.py` & `strax-1.6.3/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_storage.py` & `strax-1.6.3/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.2/tests/test_superruns.py` & `strax-1.6.3/tests/test_superruns.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
         rr_superrun = self.context.get_array("_superrun_test_rechunking", "records")
         rr_subruns = self.context.get_array(self.subrun_ids, "records")
 
         chunks = [chunk for chunk in self.context.get_iter("_superrun_test_rechunking", "records")]
         assert len(chunks) > 1, (
             "Number of chunks should be larger 1. "
-            f"{chunks[0].target_size_mb, chunks[0].nbytes/10**6}"
+            f"{chunks[0].target_size_mb, chunks[0].nbytes / 10**6}"
         )
         assert np.all(rr_superrun["time"] == rr_subruns["time"])
 
     def test_superrun_triggers_subrun_processing(self):
         """Tests if superrun processing can trigger subrun processing.
 
         Which it should.
```

### Comparing `strax-1.6.2/tests/test_utils.py` & `strax-1.6.3/tests/test_utils.py`

 * *Files identical despite different names*

