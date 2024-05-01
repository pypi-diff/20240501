# Comparing `tmp/snowfakery-3.6.2.tar.gz` & `tmp/snowfakery-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowfakery-3.6.2.tar", last modified: Thu Mar 28 00:01:15 2024, max compression
+gzip compressed data, was "snowfakery-3.6.3.tar", last modified: Wed May  1 19:56:27 2024, max compression
```

## Comparing `snowfakery-3.6.2.tar` & `snowfakery-3.6.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.103139 snowfakery-3.6.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1499 2024-03-28 00:01:01.000000 snowfakery-3.6.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-03-28 00:01:01.000000 snowfakery-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     2166 2024-03-28 00:01:15.103139 snowfakery-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1340 2024-03-28 00:01:01.000000 snowfakery-3.6.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-03-28 00:01:01.000000 snowfakery-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.095139 snowfakery-3.6.2/requirements/
--rw-r--r--   0 runner    (1000) runner    (1000)     4864 2024-03-28 00:01:01.000000 snowfakery-3.6.2/requirements/dev.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1163 2024-03-28 00:01:01.000000 snowfakery-3.6.2/requirements/prod.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-03-28 00:01:01.000000 snowfakery-3.6.2/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-03-28 00:01:01.000000 snowfakery-3.6.2/requirements_dev.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-28 00:01:15.103139 snowfakery-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2189 2024-03-28 00:01:01.000000 snowfakery-3.6.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.099139 snowfakery-3.6.2/snowfakery/
--rw-r--r--   0 runner    (1000) runner    (1000)      579 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       74 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12213 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/api.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.099139 snowfakery-3.6.2/snowfakery/backports/
--rw-r--r--   0 runner    (1000) runner    (1000)      842 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/backports/typeguard_context_manager_hack.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.099139 snowfakery-3.6.2/snowfakery/cci_mapping_files/
--rw-r--r--   0 runner    (1000) runner    (1000)     5716 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/cci_mapping_files/declaration_parser.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/cci_mapping_files/post_processes.py
--rwxr-xr-x   0 runner    (1000) runner    (1000)     9202 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/cli.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2149 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/data_gen_exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9468 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/data_generator.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26461 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/data_generator_runtime.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16482 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/data_generator_runtime_object_model.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.099139 snowfakery-3.6.2/snowfakery/fakedata/
--rw-r--r--   0 runner    (1000) runner    (1000)     8442 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/fakedata/fake_data_generator.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7700 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/generate_mapping_from_recipe.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/object_rows.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21856 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/output_streams.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27740 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/parse_recipe_yaml.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11381 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/plugins.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8676 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/row_history.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2452 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/salesforce.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.103139 snowfakery-3.6.2/snowfakery/standard_plugins/
--rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/Counters.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14928 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/Salesforce.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14341 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/Schedule.py
--rw-r--r--   0 runner    (1000) runner    (1000)      311 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/SnowfakeryVersion.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/UniqueId.py
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/_math.py
--rw-r--r--   0 runner    (1000) runner    (1000)      237 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/base64.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8255 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/datasets.py
--rw-r--r--   0 runner    (1000) runner    (1000)      437 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/file.py
--rw-r--r--   0 runner    (1000) runner    (1000)      764 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/standard_plugins/statistical_distributions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14206 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/template_funcs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.103139 snowfakery-3.6.2/snowfakery/tools/
--rw-r--r--   0 runner    (1000) runner    (1000)      256 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/bench_overhead.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2063 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/benchmark_1.yml
--rw-r--r--   0 runner    (1000) runner    (1000)     1119 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/mkdocs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5757 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/snowbench.py
--rw-r--r--   0 runner    (1000) runner    (1000)      877 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/snowcheck.py
--rw-r--r--   0 runner    (1000) runner    (1000)      168 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/tools/storage_bench.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.103139 snowfakery-3.6.2/snowfakery/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2783 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/collections.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1266 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/files.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1955 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/pickle.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4135 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/randomized_range.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2257 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/scrambled_numbers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2235 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/template_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2380 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      170 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/utils/yaml_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-28 00:01:01.000000 snowfakery-3.6.2/snowfakery/version.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-28 00:01:15.099139 snowfakery-3.6.2/snowfakery.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2166 2024-03-28 00:01:14.000000 snowfakery-3.6.2/snowfakery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1955 2024-03-28 00:01:15.000000 snowfakery-3.6.2/snowfakery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-28 00:01:14.000000 snowfakery-3.6.2/snowfakery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      164 2024-03-28 00:01:14.000000 snowfakery-3.6.2/snowfakery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-28 00:01:14.000000 snowfakery-3.6.2/snowfakery.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-28 00:01:14.000000 snowfakery-3.6.2/snowfakery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.229928 snowfakery-3.6.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1499 2024-05-01 19:56:04.000000 snowfakery-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-05-01 19:56:04.000000 snowfakery-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     2166 2024-05-01 19:56:27.229928 snowfakery-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1340 2024-05-01 19:56:04.000000 snowfakery-3.6.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-05-01 19:56:04.000000 snowfakery-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/requirements/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5066 2024-05-01 19:56:04.000000 snowfakery-3.6.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1183 2024-05-01 19:56:04.000000 snowfakery-3.6.3/requirements/prod.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-05-01 19:56:04.000000 snowfakery-3.6.3/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-05-01 19:56:04.000000 snowfakery-3.6.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-01 19:56:27.229928 snowfakery-3.6.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2189 2024-05-01 19:56:04.000000 snowfakery-3.6.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/snowfakery/
+-rw-r--r--   0 runner    (1000) runner    (1000)      579 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       74 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12213 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/api.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/snowfakery/backports/
+-rw-r--r--   0 runner    (1000) runner    (1000)      842 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/backports/typeguard_context_manager_hack.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/snowfakery/cci_mapping_files/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5716 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/cci_mapping_files/declaration_parser.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/cci_mapping_files/post_processes.py
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     9202 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/cli.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2149 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/data_gen_exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9468 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/data_generator.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26467 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/data_generator_runtime.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16482 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/data_generator_runtime_object_model.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/snowfakery/fakedata/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8442 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/fakedata/fake_data_generator.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7700 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/generate_mapping_from_recipe.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/object_rows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21975 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/output_streams.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27740 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/parse_recipe_yaml.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11441 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/plugins.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8676 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/row_history.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2461 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/salesforce.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.229928 snowfakery-3.6.3/snowfakery/standard_plugins/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/Counters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14635 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/Salesforce.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14379 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/Schedule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      311 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/SnowfakeryVersion.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/UniqueId.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/_math.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      237 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/base64.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8563 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/datasets.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      437 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/file.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      764 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/standard_plugins/statistical_distributions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14206 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/template_funcs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.229928 snowfakery-3.6.3/snowfakery/tools/
+-rw-r--r--   0 runner    (1000) runner    (1000)      256 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/bench_overhead.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2063 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/benchmark_1.yml
+-rw-r--r--   0 runner    (1000) runner    (1000)     1102 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/mkdocs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5798 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/snowbench.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      877 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/snowcheck.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      168 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/tools/storage_bench.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.229928 snowfakery-3.6.3/snowfakery/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2783 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/collections.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1266 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1955 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/pickle.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4135 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/randomized_range.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2257 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/scrambled_numbers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2235 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/template_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2380 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      170 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/utils/yaml_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-05-01 19:56:04.000000 snowfakery-3.6.3/snowfakery/version.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 19:56:27.225928 snowfakery-3.6.3/snowfakery.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2166 2024-05-01 19:56:26.000000 snowfakery-3.6.3/snowfakery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1955 2024-05-01 19:56:27.000000 snowfakery-3.6.3/snowfakery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-01 19:56:26.000000 snowfakery-3.6.3/snowfakery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      164 2024-05-01 19:56:26.000000 snowfakery-3.6.3/snowfakery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-05-01 19:56:26.000000 snowfakery-3.6.3/snowfakery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-01 19:56:26.000000 snowfakery-3.6.3/snowfakery.egg-info/top_level.txt
```

### Comparing `snowfakery-3.6.2/LICENSE` & `snowfakery-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/PKG-INFO` & `snowfakery-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowfakery
-Version: 3.6.2
+Version: 3.6.3
 Summary: Snowfakery is a tool for generating fake data that has relations between tables. Every row is faked data, but also unique and random, like a snowflake.
 Home-page: https://github.com/SFDO-Tooling/Snowfakery
 Author: Paul Prescod
 Author-email: pprescod@salesforce.com
 License: UNKNOWN
 Description: [![Coverage Status](https://coveralls.io/repos/github/SFDO-Tooling/Snowfakery/badge.svg?branch=main)](https://coveralls.io/github/SFDO-Tooling/Snowfakery?branch=main)
```

### Comparing `snowfakery-3.6.2/README.md` & `snowfakery-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/requirements/dev.txt` & `snowfakery-3.6.3/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --allow-unsafe requirements/dev.in
 #
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-black==24.3.0
+black==24.4.2
     # via -r requirements/dev.in
 cachetools==5.3.3
     # via tox
 certifi==2024.2.2
     # via
     #   -r requirements/prod.txt
     #   requests
@@ -36,57 +36,58 @@
 coverage[toml]==6.5.0
     # via
     #   -r requirements/dev.in
     #   coveralls
     #   pytest-cov
 coveralls==3.3.1
     # via -r requirements/dev.in
-diff-cover==8.0.3
+diff-cover==9.0.0
     # via -r requirements/dev.in
 distlib==0.3.8
     # via virtualenv
 docopt==0.6.2
     # via coveralls
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
-faker==24.4.0
+faker==24.14.0
     # via
     #   -r requirements/prod.txt
     #   faker-edu
     #   faker-microservice
     #   faker-nonprofit
 faker-edu==1.1.0
     # via -r requirements/prod.txt
 faker-microservice==2.0.0
     # via -r requirements/dev.in
 faker-nonprofit==1.0.0
     # via -r requirements/prod.txt
-filelock==3.13.3
+filelock==3.13.4
     # via
     #   tox
     #   virtualenv
 ghp-import==2.1.0
     # via mkdocs
 greenlet==3.0.3
     # via
     #   -r requirements/prod.txt
     #   sqlalchemy
 gvgen==1.0
     # via -r requirements/prod.txt
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   -r requirements/prod.txt
     #   requests
     #   yarl
 importlib-metadata==7.1.0
     # via
     #   markdown
     #   mkdocs
+    #   mkdocs-get-deps
 importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.3
@@ -100,22 +101,27 @@
     # via jsonschema
 markdown==3.6
     # via mkdocs
 markupsafe==2.1.5
     # via
     #   -r requirements/prod.txt
     #   jinja2
+    #   mkdocs
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.2.4
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   -r requirements/dev.in
     #   mkdocs-exclude-search
 mkdocs-exclude-search==0.6.6
     # via -r requirements/dev.in
+mkdocs-get-deps==0.2.0
+    # via mkdocs
 multidict==6.0.5
     # via yarl
 mypy-extensions==1.0.0
     # via black
 nodeenv==1.8.0
     # via
     #   pre-commit
@@ -124,36 +130,39 @@
     # via
     #   black
     #   mkdocs
     #   pyproject-api
     #   pytest
     #   tox
 pathspec==0.12.1
-    # via black
+    # via
+    #   black
+    #   mkdocs
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   black
+    #   mkdocs-get-deps
     #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   diff-cover
     #   pytest
     #   tox
 pre-commit==3.5.0
     # via -r requirements/dev.in
-pydantic==1.10.14
+pydantic==1.10.15
     # via -r requirements/prod.txt
 pygments==2.17.2
     # via diff-cover
 pyproject-api==1.6.1
     # via tox
-pyright==1.1.356
+pyright==1.1.360
     # via -r requirements/dev.in
 pytest==8.1.1
     # via
     #   -r requirements/dev.in
     #   pytest-cov
     #   pytest-vcr
 pytest-cov==5.0.0
@@ -167,21 +176,22 @@
     #   -r requirements/prod.txt
     #   faker
     #   ghp-import
 pyyaml==6.0.1
     # via
     #   -r requirements/prod.txt
     #   mkdocs
+    #   mkdocs-get-deps
     #   pre-commit
     #   pyyaml-env-tag
     #   responses
     #   vcrpy
 pyyaml-env-tag==0.1
     # via mkdocs
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.29.0
     # via
     #   -r requirements/prod.txt
     #   coveralls
@@ -192,15 +202,15 @@
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via
     #   -r requirements/prod.txt
     #   python-dateutil
-sqlalchemy==1.4.52
+sqlalchemy==2.0.29
     # via -r requirements/prod.txt
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pyproject-api
     #   pytest
@@ -209,31 +219,32 @@
     # via
     #   -r requirements/dev.in
     #   tox-gh-actions
 tox-gh-actions==3.2.0
     # via -r requirements/dev.in
 types-pyyaml==6.0.12.20240311
     # via responses
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   -r requirements/prod.txt
     #   black
     #   faker
     #   pydantic
+    #   sqlalchemy
 urllib3==1.26.18
     # via
     #   -r requirements/prod.txt
     #   requests
     #   responses
     #   vcrpy
 vcrpy==6.0.1
     # via
     #   -r requirements/dev.in
     #   pytest-vcr
-virtualenv==20.25.1
+virtualenv==20.26.0
     # via
     #   pre-commit
     #   tox
 watchdog==4.0.0
     # via mkdocs
 wrapt==1.16.0
     # via vcrpy
@@ -241,9 +252,9 @@
     # via vcrpy
 zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==69.2.0
+setuptools==69.5.1
     # via nodeenv
```

### Comparing `snowfakery-3.6.2/requirements/prod.txt` & `snowfakery-3.6.3/requirements/prod.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,48 +6,49 @@
 #
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via -r requirements/prod.in
-faker==24.4.0
+faker==24.14.0
     # via
     #   -r requirements/prod.in
     #   faker-edu
     #   faker-nonprofit
 faker-edu==1.1.0
     # via -r requirements/prod.in
 faker-nonprofit==1.0.0
     # via -r requirements/prod.in
 greenlet==3.0.3
     # via sqlalchemy
 gvgen==1.0
     # via -r requirements/prod.in
-idna==3.6
+idna==3.7
     # via requests
 jinja2==3.1.3
     # via -r requirements/prod.in
 markupsafe==2.1.5
     # via jinja2
-pydantic==1.10.14
+pydantic==1.10.15
     # via -r requirements/prod.in
 python-baseconv==1.2.2
     # via -r requirements/prod.in
 python-dateutil==2.9.0.post0
     # via
     #   -r requirements/prod.in
     #   faker
 pyyaml==6.0.1
     # via -r requirements/prod.in
 requests==2.29.0
     # via -r requirements/prod.in
 six==1.16.0
     # via python-dateutil
-sqlalchemy==1.4.52
+sqlalchemy==2.0.29
     # via -r requirements/prod.in
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   faker
     #   pydantic
+    #   sqlalchemy
 urllib3==1.26.18
     # via requests
```

### Comparing `snowfakery-3.6.2/setup.py` & `snowfakery-3.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/__init__.py` & `snowfakery-3.6.3/snowfakery/__init__.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/api.py` & `snowfakery-3.6.3/snowfakery/api.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/backports/typeguard_context_manager_hack.py` & `snowfakery-3.6.3/snowfakery/backports/typeguard_context_manager_hack.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/cci_mapping_files/declaration_parser.py` & `snowfakery-3.6.3/snowfakery/cci_mapping_files/declaration_parser.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/cci_mapping_files/post_processes.py` & `snowfakery-3.6.3/snowfakery/cci_mapping_files/post_processes.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/cli.py` & `snowfakery-3.6.3/snowfakery/cli.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/data_gen_exceptions.py` & `snowfakery-3.6.3/snowfakery/data_gen_exceptions.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/data_generator.py` & `snowfakery-3.6.3/snowfakery/data_generator.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/data_generator_runtime.py` & `snowfakery-3.6.3/snowfakery/data_generator_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
         return self
 
     def __exit__(self, *args):
         for plugin in self.plugin_instances.values():
             try:
                 plugin.close()
             except Exception as e:
-                warn(f"Could not close {plugin} because {e}")
+                warn(f"Could not close {plugin} because {repr(e)}")
         self.current_context = None
         self.plugin_instances = None
         self.plugin_function_libraries = None
         self.instance_states = None
 
     def get_contextual_state(
         self,
```

### Comparing `snowfakery-3.6.2/snowfakery/data_generator_runtime_object_model.py` & `snowfakery-3.6.3/snowfakery/data_generator_runtime_object_model.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/fakedata/fake_data_generator.py` & `snowfakery-3.6.3/snowfakery/fakedata/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/generate_mapping_from_recipe.py` & `snowfakery-3.6.3/snowfakery/generate_mapping_from_recipe.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/object_rows.py` & `snowfakery-3.6.3/snowfakery/object_rows.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/output_streams.py` & `snowfakery-3.6.3/snowfakery/output_streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,19 @@
         return self
 
     def write_single_row(self, tablename: str, row: Dict) -> None:
         # cache the value for later insert
         self.buffered_rows[tablename].append(row)
 
     def flush(self):
+        with self.session.begin():
+            self._flush_rows()
+            self.session.flush()
+
+    def _flush_rows(self):
         for tablename, (insert_statement, fallback_dict) in self.table_info.items():
             # Make sure every row has the same records per SQLAlchemy's rules
 
             # According to the SQL Alchemy docs, every dictionary in a set must
             # have the same keys.
 
             # This means that the INSERT statement will be more bloated but it
@@ -346,24 +351,23 @@
                     for key in fallback_dict.keys()
                 }
                 for row in self.buffered_rows[tablename]
             ]
             if values:
                 self.session.execute(insert_statement, values)
             self.buffered_rows[tablename] = []
-        self.session.flush()
 
     def commit(self):
         if any(self.buffered_rows):
             self.flush()
-        self.session.commit()
 
     def close(self, **kwargs) -> Optional[Sequence[str]]:
         self.commit()
         self.session.close()
+        self.engine.dispose()
 
     def create_or_validate_tables(self, inferred_tables: Dict[str, TableInfo]) -> None:
         try:
             create_tables_from_inferred_fields(
                 inferred_tables, self.engine, self.metadata
             )
         except Exception as e:
@@ -433,14 +437,16 @@
         con = self.sql_db.engine.raw_connection()
 
         # https://docs.python.org/3/library/sqlite3.html#sqlite3.Connection.iterdump
         for line in con.iterdump():  # type: ignore
             assert self.text_output.stream
             self.text_output.stream.write("%s\n" % line)
 
+        con.close()
+
     def close(self, *args, **kwargs):
         self._dump_db()
         self.sql_db.close(*args, **kwargs)
         self.text_output.close(*args, **kwargs)
         self.tempdir.cleanup()
```

### Comparing `snowfakery-3.6.2/snowfakery/parse_recipe_yaml.py` & `snowfakery-3.6.3/snowfakery/parse_recipe_yaml.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/plugins.py` & `snowfakery-3.6.3/snowfakery/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     def __init__(self, interpreter):
         self.interpreter = interpreter
         self.context = PluginContext(self)
 
     def custom_functions(self, *args, **kwargs):
         """Instantiate, contextualize and return a function library
 
-        Default behaviour is to return self.Function()."""
-        functions = self.Functions()
+        Default behaviour is to return self.Functions()."""
+        functions = self.Functions() # type: ignore
         functions.context = self.context
         return functions
 
     def close(self, *args, **kwargs):
         pass
 
 
@@ -196,15 +196,15 @@
 def resolve_plugins(
     plugin_specs: List[Tuple[str, object]], search_paths: List[Union[str, Path]]
 ):
     "Resolve a list of plugins and lineinfos"
     with plugin_path(search_paths):
         plugins = []
         for plugin_spec in plugin_specs:
-            plugins.extend(resolve_plugin(*plugin_spec))
+            plugins.extend(resolve_plugin(*plugin_spec)) # type: ignore
         return plugins
 
 
 def plugin_path(search_paths):
     cwd_plugins = "./plugins"
     user_plugins = Path.home() / ".snowfakery/plugins"
     new_sys_path = [
@@ -308,30 +308,30 @@
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         _register_for_continuation(cls)
 
 
 def _register_for_continuation(cls):
-    SnowfakeryDumper.add_representer(cls, Representer.represent_object)
+    SnowfakeryDumper.add_representer(cls, Representer.represent_object) # type: ignore
     yaml.SafeLoader.add_constructor(
         f"tag:yaml.org,2002:python/object/apply:{cls.__module__}.{cls.__name__}",
         lambda loader, node: cls._from_continuation(
             loader.construct_mapping(node.value[0])
         ),
     )
 
 
 class PluginResultIterator(PluginResult):
     closed = False
 
     def __init__(self, repeat):
         self.repeat = repeat
 
-    def __iter__(self):
+    def __iter__(self) -> T.Iterator:
         return self
 
     def __next__(self):
         return self.next()
 
     def next(self):
         try:
```

### Comparing `snowfakery-3.6.2/snowfakery/row_history.py` & `snowfakery-3.6.3/snowfakery/row_history.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/salesforce.py` & `snowfakery-3.6.3/snowfakery/salesforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             )
             if record_type_column:
                 rt_table = _create_record_type_table(tablename, metadata)
                 rt_table.create(bind=connection)
                 _populate_rt_table(connection, table, record_type_column, rt_table)
 
 
-def _create_record_type_table(tablename: str, metadata: MetaData):
+def _create_record_type_table(tablename: str, metadata: MetaData) -> Table:
     """Create a table to store mapping between Record Type Ids and Developer Names."""
     rt_map_fields = [
         Column("record_type_id", Unicode(18), primary_key=True),
         Column("developer_name", Unicode(255)),
     ]
     rt_map_table = Table(tablename + "_rt_mapping", metadata, *rt_map_fields)
     return rt_map_table
```

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/Counters.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/Counters.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/Salesforce.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/Salesforce.py`

 * *Files 3% similar despite different names*

```diff
@@ -326,34 +326,22 @@
             raise DataGenError(f"Unable to query records for {query}: {e}") from e
 
         if qs.job_result.status is not self.DataOperationStatus.SUCCESS:
             raise DataGenError(
                 f"Unable to query records for {query}: {','.join(qs.job_result.job_errors)}"
             )
 
-        self.tempdir, self.iterator = create_tempfile_sql_db_iterator(
+        tempdir, iterator = create_tempfile_sql_db_iterator(
             iteration_mode, fieldnames, qs.get_results()
         )
-        return self.iterator
+        iterator.cleanup.push(tempdir)
+        return iterator
 
     def close(self):
-        if self.iterator:
-            self.iterator.close()
-            self.iterator = None
-
-        if self.tempdir:
-            self.tempdir.cleanup()
-            self.tempdir = None
-
-    def __del__(self):
-        # in case close was not called
-        # properly, try to do an orderly
-        # cleanup
-        self.close()
-
+        pass
 
 def create_tempfile_sql_db_iterator(mode, fieldnames, results):
     tempdir, db_url = _create_db(fieldnames, results)
     rc = sql_dataset(db_url, "data", mode)
     return tempdir, rc
```

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/Schedule.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/Schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         elif action == "include":
             # https://dateutil.readthedocs.io/en/stable/rrule.html#dateutil.rrule.rruleset.rrule
             add_rule = self.ruleset.rrule
             # https://dateutil.readthedocs.io/en/stable/rrule.html#dateutil.rrule.rruleset.rdate
             add_date = self.ruleset.rdate
         else:  # pragma: no cover   -   Should be unreachable
             assert action in ("include", "exclude"), "Bad action!"
-            raise NotImplementedError()
+            raise NotImplementedError("Bad action!")
 
         if isinstance(case, (list, tuple)):
             for case in case:
                 self._process_special_cases(case, action)
         elif isinstance(case, CalendarRule):
             add_rule(T.cast(T.Any, case.ruleset))
 
@@ -334,15 +334,15 @@
     def __iter__(self) -> T.Union[T.Iterator[datetime], T.Iterator[date]]:
         return iter(self.ruleset)
 
     def next(self) -> None:  # pragma: no cover
         """This method is never called.
 
         It is replaced at runtime by _next_datetime or _next_date"""
-        raise NotImplementedError()
+        raise NotImplementedError("next is not implemented")
 
     def _next_datetime(self) -> datetime:
         return next(self.iterator)
 
     def _next_date(self) -> date:
         val: datetime = next(self.iterator)
         return val.date()
```

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/UniqueId.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/UniqueId.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/datasets.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,25 @@
 
 class DatasetIteratorBase(PluginResultIterator):
     """Base class for Dataset Iterators
 
     Subclasses should implement 'self.restart' which puts an iterator into 'self.results'
     """
 
+    def __init__(self, repeat):
+        # subclasses can register stuff to be cleaned up here.
+        self.cleanup = ExitStack()
+        super().__init__(repeat)
+
     def next_result(self):
         return next(self.results)
 
+    def close(self):
+        self.cleanup.close()
+
 
 class SQLDatasetIterator(DatasetIteratorBase):
     def __init__(self, engine, table, repeat):
         self.connection = engine.connect()
         self.table = table
         super().__init__(repeat)
         self.start()
@@ -82,14 +90,15 @@
             DatasetPluginResult(dict(row._mapping))
             for row in self.connection.execute(self.query())
         )
 
     def close(self):
         self.results = None
         self.connection.close()
+        super().close()
 
     def query(self):
         "Return a SQL Alchemy SELECT statement"
         raise NotImplementedError(f"query method on {self.__class__.__name__}")
 
 
 class SQLDatasetLinearIterator(SQLDatasetIterator):
@@ -104,34 +113,33 @@
 
     def query(self):
         return select(self.table).order_by(func.random())
 
 
 class CSVDatasetLinearIterator(DatasetIteratorBase):
     def __init__(self, datasource: FileLike, repeat: bool):
-        self.cleanup = ExitStack()
+        super().__init__(repeat)
         # utf-8-sig and newline="" are for Windows
         self.path, self.file = self.cleanup.enter_context(
             open_file_like(datasource, "r", newline="", encoding="utf-8-sig")
         )
 
         self.start()
-        super().__init__(repeat)
 
     def start(self):
         assert self.file
         self.file.seek(0)
         d = DictReader(self.file)  # type: ignore
 
         plugin_result = self.plugin_result
         self.results = (plugin_result(row) for row in d)
 
     def close(self):
         self.results = None
-        self.cleanup.close()
+        super().close()
 
     def plugin_result(self, row):
         if None in row:
             raise DataGenError(
                 f"Your CSV row has more columns than the CSV header:  {row[None]}, {self.path} {self.file}"
             )
 
@@ -186,21 +194,25 @@
         filename = plugin_context.field_vars()["template"].filename
         assert filename
         rootpath = Path(filename).parent
         dataset_instance = self._load_dataset(iteration_mode, rootpath, kwargs)
         return dataset_instance
 
     def _load_dataset(self, iteration_mode, rootpath, kwargs):
-        raise NotImplementedError()
+        raise NotImplementedError("_load_dataset not implemented")
 
     def close(self):
-        raise NotImplementedError()
+        raise NotImplementedError("close not implemented: " + repr(self))
 
 
 class FileDataset(DatasetBase):
+
+    def close(self):
+        pass
+    
     def _load_dataset(self, iteration_mode, rootpath, kwargs):
         dataset = kwargs.get("dataset")
         tablename = kwargs.get("table")
         repeat = kwargs.get("repeat", True)
 
         with chdir(rootpath):
             if "://" in dataset:
```

### Comparing `snowfakery-3.6.2/snowfakery/standard_plugins/statistical_distributions.py` & `snowfakery-3.6.3/snowfakery/standard_plugins/statistical_distributions.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/template_funcs.py` & `snowfakery-3.6.3/snowfakery/template_funcs.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/tools/benchmark_1.yml` & `snowfakery-3.6.3/snowfakery/tools/benchmark_1.yml`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/tools/mkdocs.py` & `snowfakery-3.6.3/snowfakery/tools/mkdocs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import sys
 from pathlib import Path
 from importlib import import_module
 from unittest.mock import patch
 
 from mkdocs.plugins import BasePlugin
-import mkdocs
+from mkdocs.config import config_options
 
 
 class Plugin(BasePlugin):
-    config_scheme = (
-        ("build_locales", mkdocs.config.config_options.Type(bool, default=False)),  # type: ignore
-    )
+    config_scheme = (("build_locales", config_options.Type(bool, default=False)),)
 
     def on_config(self, config):
         """Look for and load main_mkdocs_plugin in tools/faker_docs_utils/mkdocs_plugins.py
         This bootstrap plugin is needed because that other one is never "installed"
         It is just present in the repo. So it can't have an official entry point
         in setup.py.
         """
```

### Comparing `snowfakery-3.6.2/snowfakery/tools/snowbench.py` & `snowfakery-3.6.3/snowfakery/tools/snowbench.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from tempfile import TemporaryDirectory
 from pathlib import Path
 from collections import defaultdict
 import locale
 
 import click
-from sqlalchemy import create_engine, inspect
+from sqlalchemy import create_engine, inspect, text
 
 from snowfakery import generate_data
 
 benchmark_1 = Path(__file__).parent / "benchmark_1.yml"
 try:
     locale.setlocale(locale.LC_ALL, "")
 except locale.Error as e:
@@ -46,15 +46,14 @@
     differently than the default behaviour, because the single
     execution process is spawned off into a sub-process instead
     of being executed inline.
     """
     with TemporaryDirectory() as tempdir, click.progressbar(
         label="Benchmarking", length=num_records, show_eta=False
     ) as progress_bar:
-
         start = time()
         Thread(
             daemon=True,
             target=status,
             args=[
                 tempdir,
                 num_records,
@@ -159,22 +158,23 @@
     return counts[relevant_table_name]
 
 
 def count_database(filename, counts):
     dburl = f"sqlite:///{filename}?mode=ro"
     engine = create_engine(dburl)
     insp = inspect(engine)
-    tables = insp.get_table_names()  # type: ignore
+    tables = insp.get_table_names() # type: ignore
     for table in tables:
         counts[table] += count_table(engine, table)
     return counts
 
 
 def count_table(engine, tablename):
-    return engine.execute(f"select count(Id) from '{tablename}'").first()[0]
+    with engine.connect() as c:
+        return c.execute(text(f"select count(Id) from '{tablename}'")).first()[0]
 
 
 def snowfakery(recipe, num_records, tablename, outputfile):
     assert Path(recipe).exists(), recipe
     output = f"sqlite:///{outputfile}"
     print(output)
     generate_data(
```

### Comparing `snowfakery-3.6.2/snowfakery/tools/snowcheck.py` & `snowfakery-3.6.3/snowfakery/tools/snowcheck.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/collections.py` & `snowfakery-3.6.3/snowfakery/utils/collections.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/files.py` & `snowfakery-3.6.3/snowfakery/utils/files.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/pickle.py` & `snowfakery-3.6.3/snowfakery/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/randomized_range.py` & `snowfakery-3.6.3/snowfakery/utils/randomized_range.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/scrambled_numbers.py` & `snowfakery-3.6.3/snowfakery/utils/scrambled_numbers.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/template_utils.py` & `snowfakery-3.6.3/snowfakery/utils/template_utils.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery/utils/versions.py` & `snowfakery-3.6.3/snowfakery/utils/versions.py`

 * *Files identical despite different names*

### Comparing `snowfakery-3.6.2/snowfakery.egg-info/PKG-INFO` & `snowfakery-3.6.3/snowfakery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowfakery
-Version: 3.6.2
+Version: 3.6.3
 Summary: Snowfakery is a tool for generating fake data that has relations between tables. Every row is faked data, but also unique and random, like a snowflake.
 Home-page: https://github.com/SFDO-Tooling/Snowfakery
 Author: Paul Prescod
 Author-email: pprescod@salesforce.com
 License: UNKNOWN
 Description: [![Coverage Status](https://coveralls.io/repos/github/SFDO-Tooling/Snowfakery/badge.svg?branch=main)](https://coveralls.io/github/SFDO-Tooling/Snowfakery?branch=main)
```

### Comparing `snowfakery-3.6.2/snowfakery.egg-info/SOURCES.txt` & `snowfakery-3.6.3/snowfakery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

