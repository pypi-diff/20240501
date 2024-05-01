# Comparing `tmp/cleanlab_studio-2.0.2.tar.gz` & `tmp/cleanlab_studio-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab_studio-2.0.2.tar", last modified: Fri Apr 19 18:53:16 2024, max compression
+gzip compressed data, was "cleanlab_studio-2.0.3.tar", last modified: Wed May  1 19:25:00 2024, max compression
```

## Comparing `cleanlab_studio-2.0.2.tar` & `cleanlab_studio-2.0.3.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.113166 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.117166 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    30234 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 18:53:16.000000 cleanlab_studio-2.0.2/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:53:16.121166 cleanlab_studio-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-19 18:53:06.000000 cleanlab_studio-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.069349 cleanlab_studio-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.057349 cleanlab_studio-2.0.3/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.057349 cleanlab_studio-2.0.3/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.061349 cleanlab_studio-2.0.3/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24287 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30234 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio/utils/data_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/utils/data_enrichment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/utils/data_enrichment/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/utils/data_enrichment/enrichment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:25:00.065349 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 19:25:00.000000 cleanlab_studio-2.0.3/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:25:00.069349 cleanlab_studio-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-01 19:24:49.000000 cleanlab_studio-2.0.3/setup.py
```

### Comparing `cleanlab_studio-2.0.2/LICENSE` & `cleanlab_studio-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/PKG-INFO` & `cleanlab_studio-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.2
+Version: 2.0.3
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab_studio-2.0.2/README.md` & `cleanlab_studio-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/api_service.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/dataset.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/click_helpers.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/dataset/upload.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/login/login.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/main.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/types.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/cli/util.py` & `cleanlab_studio-2.0.3/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/errors.py` & `cleanlab_studio-2.0.3/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/api/api.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import aiohttp
 import aiohttp.client_exceptions
 import requests
 from tqdm import tqdm
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
+from io import StringIO
 
 try:
     import snowflake
 
     snowflake_exists = True
 except ImportError:
     snowflake_exists = False
@@ -35,16 +36,17 @@
     pyspark_exists = True
 except ImportError:
     pyspark_exists = False
 
 from cleanlab_studio.internal.types import JSONDict, SchemaOverride
 from cleanlab_studio.version import __version__
 from cleanlab_studio.errors import NotInstalledError
-from cleanlab_studio.internal.api.api_helper import check_uuid_well_formed
-
+from cleanlab_studio.internal.api.api_helper import (
+    check_uuid_well_formed,
+)
 
 base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
 cli_base_url = f"{base_url}/cli/v0"
 upload_base_url = f"{base_url}/upload/v1"
 dataset_base_url = f"{base_url}/datasets"
 project_base_url = f"{base_url}/projects"
 cleanset_base_url = f"{base_url}/cleansets"
@@ -304,15 +306,15 @@
     )
     handle_api_error(res)
     res_json: JSONDict = res.json()
     if res_json["success"]:
         if res_json["array_type"] == "numpy":
             np_data: npt.NDArray[np.float_] = np.array(res_json[name])
             return np_data
-        pd_data: pd.DataFrame = pd.read_json(res_json[name], orient="records")
+        pd_data: pd.DataFrame = pd.read_json(StringIO(res_json[name]), orient="records")
         return pd_data
     raise APIError(f"{name} for cleanset {cleanset_id} not found")
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     check_uuid_well_formed(cleanset_id, "cleanset ID")
     res = requests.get(
```

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/clean_helpers.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/constants.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/settings.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/concurrency.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/concurrency.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/tlm/validation.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/tlm/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/upload_helpers.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/internal/util.py` & `cleanlab_studio-2.0.3/cleanlab_studio/internal/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import math
 import functools
 import sys
 import traceback
 import contextlib
 import subprocess
 import platform
-import requests
 import re
 
 
-import numpy as np
 import pandas as pd
 
 from cleanlab_studio.internal.api import api
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.errors import InvalidDatasetError, HandledError
 
 try:
```

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/studio/inference.py` & `cleanlab_studio-2.0.3/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/studio/studio.py` & `cleanlab_studio-2.0.3/cleanlab_studio/studio/studio.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab_studio-2.0.3/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio/utils/synthetic.py` & `cleanlab_studio-2.0.3/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab_studio-2.0.3/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.2
+Version: 2.0.3
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab_studio-2.0.2/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab_studio-2.0.3/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,8 +56,11 @@
 cleanlab_studio/internal/tlm/concurrency.py
 cleanlab_studio/internal/tlm/validation.py
 cleanlab_studio/studio/__init__.py
 cleanlab_studio/studio/inference.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/trustworthy_language_model.py
 cleanlab_studio/utils/__init__.py
-cleanlab_studio/utils/synthetic.py
+cleanlab_studio/utils/synthetic.py
+cleanlab_studio/utils/data_enrichment/__init__.py
+cleanlab_studio/utils/data_enrichment/enrich.py
+cleanlab_studio/utils/data_enrichment/enrichment_utils.py
```

### Comparing `cleanlab_studio-2.0.2/setup.py` & `cleanlab_studio-2.0.3/setup.py`

 * *Files identical despite different names*

