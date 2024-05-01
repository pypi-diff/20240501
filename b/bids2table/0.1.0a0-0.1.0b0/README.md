# Comparing `tmp/bids2table-0.1.0a0.tar.gz` & `tmp/bids2table-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bids2table-0.1.0a0.tar", last modified: Wed Aug  9 18:30:58 2023, max compression
+gzip compressed data, was "bids2table-0.1.0b0.tar", last modified: Fri Feb 23 16:37:07 2024, max compression
```

## Comparing `bids2table-0.1.0a0.tar` & `bids2table-0.1.0b0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.384979 bids2table-0.1.0a0/
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.374656 bids2table-0.1.0a0/.github/
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.377135 bids2table-0.1.0a0/.github/workflows/
--rw-r--r--   0 clane      (503) staff       (20)      835 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/.github/workflows/ci.yaml
--rw-r--r--   0 clane      (503) staff       (20)     1148 2023-08-09 16:52:28.000000 bids2table-0.1.0a0/.github/workflows/docs.yaml
--rw-r--r--   0 clane      (503) staff       (20)      509 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/.gitignore
--rw-r--r--   0 clane      (503) staff       (20)      108 2023-08-07 14:35:31.000000 bids2table-0.1.0a0/.gitmodules
--rw-r--r--   0 clane      (503) staff       (20)      875 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/.pre-commit-config.yaml
--rw-r--r--   0 clane      (503) staff       (20)    14287 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/.pylintrc
--rw-r--r--   0 clane      (503) staff       (20)     1068 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/LICENSE
--rw-r--r--   0 clane      (503) staff       (20)     3945 2023-08-09 18:30:58.385073 bids2table-0.1.0a0/PKG-INFO
--rw-r--r--   0 clane      (503) staff       (20)     3074 2023-08-09 18:28:04.000000 bids2table-0.1.0a0/README.md
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.374887 bids2table-0.1.0a0/benchmark/
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.378968 bids2table-0.1.0a0/benchmark/indexing/
--rw-r--r--   0 clane      (503) staff       (20)     1771 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/README.md
--rw-r--r--   0 clane      (503) staff       (20)    46028 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/analysis.ipynb
--rw-r--r--   0 clane      (503) staff       (20)     3952 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/benchmark_indexing.py
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.379127 bids2table-0.1.0a0/benchmark/indexing/figures/
--rw-r--r--   0 clane      (503) staff       (20)   108048 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/figures/indexing_performance.png
--rw-r--r--   0 clane      (503) staff       (20)      694 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/nki_ancpbids_batch_array.sh
--rw-r--r--   0 clane      (503) staff       (20)      669 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/nki_bids2table_batch_array.sh
--rw-r--r--   0 clane      (503) staff       (20)      692 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/nki_pybids_batch_array.sh
--rw-r--r--   0 clane      (503) staff       (20)      691 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/indexing/setup_environments.sh
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.379850 bids2table-0.1.0a0/benchmark/query/
--rw-r--r--   0 clane      (503) staff       (20)     2053 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/query/README.md
--rw-r--r--   0 clane      (503) staff       (20)    13995 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/query/query_benchmark.ipynb
--rw-r--r--   0 clane      (503) staff       (20)      157 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/query/requirements.txt
--rw-r--r--   0 clane      (503) staff       (20)      252 2023-08-09 07:48:16.000000 bids2table-0.1.0a0/benchmark/query/setup_environment.sh
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.380982 bids2table-0.1.0a0/bids2table/
--rw-r--r--   0 clane      (503) staff       (20)     4959 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/bids2table/__init__.py
--rw-r--r--   0 clane      (503) staff       (20)     1810 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/__main__.py
--rw-r--r--   0 clane      (503) staff       (20)     3478 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/bids2table/_b2t.py
--rw-r--r--   0 clane      (503) staff       (20)      162 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table/_version.py
--rw-r--r--   0 clane      (503) staff       (20)    10829 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/entities.py
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.382839 bids2table-0.1.0a0/bids2table/extractors/
--rw-r--r--   0 clane      (503) staff       (20)       88 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/extractors/__init__.py
--rw-r--r--   0 clane      (503) staff       (20)     1721 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/extractors/bids.py
--rw-r--r--   0 clane      (503) staff       (20)     2589 2023-08-09 07:41:06.000000 bids2table-0.1.0a0/bids2table/extractors/dataset.py
--rw-r--r--   0 clane      (503) staff       (20)     2400 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/extractors/image.py
--rw-r--r--   0 clane      (503) staff       (20)     2610 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/extractors/inheritance.py
--rw-r--r--   0 clane      (503) staff       (20)     1996 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/bids2table/extractors/metadata.py
--rw-r--r--   0 clane      (503) staff       (20)    12554 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/bids2table/table.py
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.381763 bids2table-0.1.0a0/bids2table.egg-info/
--rw-r--r--   0 clane      (503) staff       (20)     3945 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/PKG-INFO
--rw-r--r--   0 clane      (503) staff       (20)     1435 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/SOURCES.txt
--rw-r--r--   0 clane      (503) staff       (20)        1 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/dependency_links.txt
--rw-r--r--   0 clane      (503) staff       (20)       87 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/entry_points.txt
--rw-r--r--   0 clane      (503) staff       (20)      161 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/requires.txt
--rw-r--r--   0 clane      (503) staff       (20)       11 2023-08-09 18:30:58.000000 bids2table-0.1.0a0/bids2table.egg-info/top_level.txt
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.382992 bids2table-0.1.0a0/example/
--rw-r--r--   0 clane      (503) staff       (20)   131274 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/example/example.ipynb
--rw-r--r--   0 clane      (503) staff       (20)     1666 2023-08-09 16:47:05.000000 bids2table-0.1.0a0/pyproject.toml
--rw-r--r--   0 clane      (503) staff       (20)      103 2023-08-09 18:30:58.385294 bids2table-0.1.0a0/setup.cfg
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.384171 bids2table-0.1.0a0/tests/
--rw-r--r--   0 clane      (503) staff       (20)        0 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/tests/__init__.py
--rw-r--r--   0 clane      (503) staff       (20)     1414 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/tests/test_bids2table.py
--rw-r--r--   0 clane      (503) staff       (20)     2914 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/tests/test_entities.py
-drwxr-xr-x   0 clane      (503) staff       (20)        0 2023-08-09 18:30:58.384842 bids2table-0.1.0a0/tests/test_extractors/
--rw-r--r--   0 clane      (503) staff       (20)        0 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/tests/test_extractors/__init__.py
--rw-r--r--   0 clane      (503) staff       (20)      857 2023-08-09 07:41:06.000000 bids2table-0.1.0a0/tests/test_extractors/test_dataset.py
--rw-r--r--   0 clane      (503) staff       (20)      827 2023-08-07 14:19:45.000000 bids2table-0.1.0a0/tests/test_extractors/test_image.py
--rw-r--r--   0 clane      (503) staff       (20)     2158 2023-08-09 07:41:06.000000 bids2table-0.1.0a0/tests/test_extractors/test_metadata.py
--rw-r--r--   0 clane      (503) staff       (20)      859 2023-08-09 07:41:06.000000 bids2table-0.1.0a0/tests/test_main.py
--rw-r--r--   0 clane      (503) staff       (20)     5607 2023-08-09 10:30:56.000000 bids2table-0.1.0a0/tests/test_table.py
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.952486 bids2table-0.1.0b0/
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.938887 bids2table-0.1.0b0/.github/
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.942405 bids2table-0.1.0b0/.github/workflows/
+-rw-r--r--   0 clane      (503) staff       (20)      835 2023-08-09 16:47:05.000000 bids2table-0.1.0b0/.github/workflows/ci.yaml
+-rw-r--r--   0 clane      (503) staff       (20)     1148 2023-08-09 16:52:28.000000 bids2table-0.1.0b0/.github/workflows/docs.yaml
+-rw-r--r--   0 clane      (503) staff       (20)      509 2023-08-09 16:47:05.000000 bids2table-0.1.0b0/.gitignore
+-rw-r--r--   0 clane      (503) staff       (20)      108 2023-08-07 14:35:31.000000 bids2table-0.1.0b0/.gitmodules
+-rw-r--r--   0 clane      (503) staff       (20)      875 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 clane      (503) staff       (20)    14287 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/.pylintrc
+-rw-r--r--   0 clane      (503) staff       (20)     1068 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/LICENSE
+-rw-r--r--   0 clane      (503) staff       (20)     4529 2024-02-23 16:37:07.952415 bids2table-0.1.0b0/PKG-INFO
+-rw-r--r--   0 clane      (503) staff       (20)     3146 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/README.md
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.939230 bids2table-0.1.0b0/benchmark/
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.944446 bids2table-0.1.0b0/benchmark/indexing/
+-rw-r--r--   0 clane      (503) staff       (20)     1780 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/benchmark/indexing/README.md
+-rw-r--r--   0 clane      (503) staff       (20)    46028 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/analysis.ipynb
+-rw-r--r--   0 clane      (503) staff       (20)     3952 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/benchmark_indexing.py
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.944691 bids2table-0.1.0b0/benchmark/indexing/figures/
+-rw-r--r--   0 clane      (503) staff       (20)   108048 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/figures/indexing_performance.png
+-rw-r--r--   0 clane      (503) staff       (20)      694 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/nki_ancpbids_batch_array.sh
+-rw-r--r--   0 clane      (503) staff       (20)      669 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/nki_bids2table_batch_array.sh
+-rw-r--r--   0 clane      (503) staff       (20)      692 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/indexing/nki_pybids_batch_array.sh
+-rw-r--r--   0 clane      (503) staff       (20)      709 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/benchmark/indexing/setup_environments.sh
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.945592 bids2table-0.1.0b0/benchmark/query/
+-rw-r--r--   0 clane      (503) staff       (20)     2062 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/benchmark/query/README.md
+-rw-r--r--   0 clane      (503) staff       (20)    14004 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/benchmark/query/query_benchmark.ipynb
+-rw-r--r--   0 clane      (503) staff       (20)      175 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/benchmark/query/requirements.txt
+-rw-r--r--   0 clane      (503) staff       (20)      252 2023-08-09 07:48:16.000000 bids2table-0.1.0b0/benchmark/query/setup_environment.sh
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.947003 bids2table-0.1.0b0/bids2table/
+-rw-r--r--   0 clane      (503) staff       (20)     4977 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/bids2table/__init__.py
+-rw-r--r--   0 clane      (503) staff       (20)     1824 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/__main__.py
+-rw-r--r--   0 clane      (503) staff       (20)     3461 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/_b2t.py
+-rw-r--r--   0 clane      (503) staff       (20)      413 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table/_version.py
+-rw-r--r--   0 clane      (503) staff       (20)    10829 2023-08-09 10:30:56.000000 bids2table-0.1.0b0/bids2table/entities.py
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.948978 bids2table-0.1.0b0/bids2table/extractors/
+-rw-r--r--   0 clane      (503) staff       (20)       97 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/bids2table/extractors/__init__.py
+-rw-r--r--   0 clane      (503) staff       (20)     1758 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/extractors/bids.py
+-rw-r--r--   0 clane      (503) staff       (20)     2626 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/extractors/dataset.py
+-rw-r--r--   0 clane      (503) staff       (20)     2437 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/extractors/image.py
+-rw-r--r--   0 clane      (503) staff       (20)     2610 2023-08-09 10:30:56.000000 bids2table-0.1.0b0/bids2table/extractors/inheritance.py
+-rw-r--r--   0 clane      (503) staff       (20)     2033 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/extractors/metadata.py
+-rw-r--r--   0 clane      (503) staff       (20)     2050 2024-02-23 16:36:05.000000 bids2table-0.1.0b0/bids2table/logging.py
+-rw-r--r--   0 clane      (503) staff       (20)    12554 2023-08-09 16:47:05.000000 bids2table-0.1.0b0/bids2table/table.py
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.951500 bids2table-0.1.0b0/bids2table.egg-info/
+-rw-r--r--   0 clane      (503) staff       (20)     4529 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/PKG-INFO
+-rw-r--r--   0 clane      (503) staff       (20)     1457 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/SOURCES.txt
+-rw-r--r--   0 clane      (503) staff       (20)        1 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/dependency_links.txt
+-rw-r--r--   0 clane      (503) staff       (20)       87 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/entry_points.txt
+-rw-r--r--   0 clane      (503) staff       (20)      161 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/requires.txt
+-rw-r--r--   0 clane      (503) staff       (20)       11 2024-02-23 16:37:07.000000 bids2table-0.1.0b0/bids2table.egg-info/top_level.txt
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.949142 bids2table-0.1.0b0/example/
+-rw-r--r--   0 clane      (503) staff       (20)   131274 2024-02-23 16:02:10.000000 bids2table-0.1.0b0/example/example.ipynb
+-rw-r--r--   0 clane      (503) staff       (20)     1675 2024-02-23 16:08:13.000000 bids2table-0.1.0b0/pyproject.toml
+-rw-r--r--   0 clane      (503) staff       (20)      103 2024-02-23 16:37:07.952709 bids2table-0.1.0b0/setup.cfg
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.950567 bids2table-0.1.0b0/tests/
+-rw-r--r--   0 clane      (503) staff       (20)        0 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/tests/__init__.py
+-rw-r--r--   0 clane      (503) staff       (20)     1414 2023-08-09 10:30:56.000000 bids2table-0.1.0b0/tests/test_bids2table.py
+-rw-r--r--   0 clane      (503) staff       (20)     2914 2023-08-09 10:30:56.000000 bids2table-0.1.0b0/tests/test_entities.py
+drwxr-xr-x   0 clane      (503) staff       (20)        0 2024-02-23 16:37:07.951297 bids2table-0.1.0b0/tests/test_extractors/
+-rw-r--r--   0 clane      (503) staff       (20)        0 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/tests/test_extractors/__init__.py
+-rw-r--r--   0 clane      (503) staff       (20)      857 2023-08-09 07:41:06.000000 bids2table-0.1.0b0/tests/test_extractors/test_dataset.py
+-rw-r--r--   0 clane      (503) staff       (20)      827 2023-08-07 14:19:45.000000 bids2table-0.1.0b0/tests/test_extractors/test_image.py
+-rw-r--r--   0 clane      (503) staff       (20)     2158 2023-08-09 07:41:06.000000 bids2table-0.1.0b0/tests/test_extractors/test_metadata.py
+-rw-r--r--   0 clane      (503) staff       (20)      859 2023-08-09 07:41:06.000000 bids2table-0.1.0b0/tests/test_main.py
+-rw-r--r--   0 clane      (503) staff       (20)     5607 2023-08-09 10:30:56.000000 bids2table-0.1.0b0/tests/test_table.py
```

### Comparing `bids2table-0.1.0a0/.github/workflows/ci.yaml` & `bids2table-0.1.0b0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/.github/workflows/docs.yaml` & `bids2table-0.1.0b0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/.pre-commit-config.yaml` & `bids2table-0.1.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/.pylintrc` & `bids2table-0.1.0b0/.pylintrc`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/LICENSE` & `bids2table-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/PKG-INFO` & `bids2table-0.1.0b0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 Metadata-Version: 2.1
 Name: bids2table
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: Efficiently index large-scale BIDS datasets and derivatives
 Author-email: Connor Lane <connor.lane858@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/cmi-dair/bids2table
+Project-URL: Homepage, https://github.com/childmindresearch/bids2table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: elbow
+Requires-Dist: nibabel
+Requires-Dist: pandas
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: pdoc==14.0.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: flake8==5.0.4; extra == "dev"
+Requires-Dist: isort==5.11.5; extra == "dev"
+Requires-Dist: mypy==1.2.0; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint>=2.5.0; extra == "dev"
+Requires-Dist: setuptools-scm; extra == "dev"
 
 # bids2table
-[![Build](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
-[![Docs](https://github.com/cmi-dair/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://cmi-dair.github.io/bids2table/bids2table)
-[![codecov](https://codecov.io/gh/cmi-dair/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/cmi-dair/bids2table)
+[![Build](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
+[![Docs](https://github.com/childmindresearch/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://childmindresearch.github.io/bids2table/bids2table)
+[![codecov](https://codecov.io/gh/childmindresearch/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/bids2table)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 
 bids2table is a library for efficiently indexing and querying large-scale BIDS neuroimaging datasets and derivatives. It aims to improve upon the efficiency of [PyBIDS](https://github.com/bids-standard/pybids) by leveraging modern data science tools.
 
 bids2table represents a BIDS dataset index as a single table with columns for BIDS entities and file metadata. The index is constructed using [Arrow](https://arrow.apache.org/) and stored in [Parquet](https://parquet.apache.org/) format, a binary tabular file format optimized for efficient storage and retrieval.
 
@@ -39,20 +52,20 @@
 ```sh
 pip install bids2table
 ```
 
 The latest development version can be installed with
 
 ```sh
-pip install git+https://github.com/cmi-dair/bids2table.git
+pip install git+https://github.com/childmindresearch/bids2table.git
 ```
 
 ## Documentation
 
-Our documentation is [here](https://cmi-dair.github.io/bids2table/).
+Our documentation is [here](https://childmindresearch.github.io/bids2table/).
 
 ## Example
 
 ```python
 import pandas as pd
 
 from bids2table import bids2table
```

### Comparing `bids2table-0.1.0a0/README.md` & `bids2table-0.1.0b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # bids2table
-[![Build](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
-[![Docs](https://github.com/cmi-dair/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://cmi-dair.github.io/bids2table/bids2table)
-[![codecov](https://codecov.io/gh/cmi-dair/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/cmi-dair/bids2table)
+[![Build](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
+[![Docs](https://github.com/childmindresearch/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://childmindresearch.github.io/bids2table/bids2table)
+[![codecov](https://codecov.io/gh/childmindresearch/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/bids2table)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 
 bids2table is a library for efficiently indexing and querying large-scale BIDS neuroimaging datasets and derivatives. It aims to improve upon the efficiency of [PyBIDS](https://github.com/bids-standard/pybids) by leveraging modern data science tools.
 
 bids2table represents a BIDS dataset index as a single table with columns for BIDS entities and file metadata. The index is constructed using [Arrow](https://arrow.apache.org/) and stored in [Parquet](https://parquet.apache.org/) format, a binary tabular file format optimized for efficient storage and retrieval.
 
@@ -16,20 +16,20 @@
 ```sh
 pip install bids2table
 ```
 
 The latest development version can be installed with
 
 ```sh
-pip install git+https://github.com/cmi-dair/bids2table.git
+pip install git+https://github.com/childmindresearch/bids2table.git
 ```
 
 ## Documentation
 
-Our documentation is [here](https://cmi-dair.github.io/bids2table/).
+Our documentation is [here](https://childmindresearch.github.io/bids2table/).
 
 ## Example
 
 ```python
 import pandas as pd
 
 from bids2table import bids2table
```

### Comparing `bids2table-0.1.0a0/benchmark/indexing/README.md` & `bids2table-0.1.0b0/benchmark/indexing/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Indexing benchmark
 
-In this benchmark we compare the indexing performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/cmi-dair/bids2table) using the raw data from the [NKI Rockland Sample](https://fcon_1000.projects.nitrc.org/indi/pro/nki.html) (1334 subjects, 1.5TB).
+In this benchmark we compare the indexing performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/childmindresearch/bids2table) using the raw data from the [NKI Rockland Sample](https://fcon_1000.projects.nitrc.org/indi/pro/nki.html) (1334 subjects, 1.5TB).
 
 ## Setup environment
 
 First install each library in a separate environment using the [setup_environments.sh](setup_environments.sh) script. The main libraries are pinned to the following versions.
 
 - PyBIDS: 0.16.0
 - ancpBIDS: 0.2.2
```

### Comparing `bids2table-0.1.0a0/benchmark/indexing/analysis.ipynb` & `bids2table-0.1.0b0/benchmark/indexing/analysis.ipynb`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/indexing/benchmark_indexing.py` & `bids2table-0.1.0b0/benchmark/indexing/benchmark_indexing.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/indexing/figures/indexing_performance.png` & `bids2table-0.1.0b0/benchmark/indexing/figures/indexing_performance.png`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/indexing/nki_ancpbids_batch_array.sh` & `bids2table-0.1.0b0/benchmark/indexing/nki_ancpbids_batch_array.sh`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/indexing/nki_bids2table_batch_array.sh` & `bids2table-0.1.0b0/benchmark/indexing/nki_bids2table_batch_array.sh`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/indexing/nki_pybids_batch_array.sh` & `bids2table-0.1.0b0/benchmark/indexing/nki_pybids_batch_array.sh`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/benchmark/query/README.md` & `bids2table-0.1.0b0/benchmark/query/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Query benchmark
 
-In this benchmark we compare the query performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/cmi-dair/bids2table). The queries are modeled after the [PyBIDS `BIDSLayout` tutorial](https://bids-standard.github.io/pybids/examples/pybids_tutorial.html#querying-the-bidslayout).
+In this benchmark we compare the query performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/childmindresearch/bids2table). The queries are modeled after the [PyBIDS `BIDSLayout` tutorial](https://bids-standard.github.io/pybids/examples/pybids_tutorial.html#querying-the-bidslayout).
 
 For this benchmark, we use raw data from the [Chinese Color Nest Project](http://deepneuro.bnu.edu.cn/?p=163) (195 subjects, 2 resting state sessions per subject).
 
 ## Setup environment
 
 We create a single environment that includes all three main libraries using the [setup_environments.sh](setup_environments.sh) script. The main libraries are pinned to the following versions.
```

### Comparing `bids2table-0.1.0a0/benchmark/query/query_benchmark.ipynb` & `bids2table-0.1.0b0/benchmark/query/query_benchmark.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999732905982906%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'In this benchmark we compare the query performance for "*

 * *            '[PyBIDS](https://github.com/bids-standard/pybids), '*

 * *            '[ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and '*

 * *            '[bids2table](https://github.com/childmindresearch/bids2table). The queries are '*

 * *            'modeled after the [PyBIDS `BIDSLayout` '*

 * *            "tutorial](https://bids-standard.github.io/pybids/examples/pybids_tutorial.html#querying-the-bidslayout).\\n […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Query benchmark\n",
                 "\n",
-                "In this benchmark we compare the query performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/cmi-dair/bids2table). The queries are modeled after the [PyBIDS `BIDSLayout` tutorial](https://bids-standard.github.io/pybids/examples/pybids_tutorial.html#querying-the-bidslayout).\n",
+                "In this benchmark we compare the query performance for [PyBIDS](https://github.com/bids-standard/pybids), [ancpBIDS](https://github.com/ANCPLabOldenburg/ancp-bids), and [bids2table](https://github.com/childmindresearch/bids2table). The queries are modeled after the [PyBIDS `BIDSLayout` tutorial](https://bids-standard.github.io/pybids/examples/pybids_tutorial.html#querying-the-bidslayout).\n",
                 "\n",
                 "For this benchmark, we use raw data from the [Chinese Color Nest Project](http://deepneuro.bnu.edu.cn/?p=163) (195 subjects, 2 resting state sessions per subject)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
```

### Comparing `bids2table-0.1.0a0/bids2table/__init__.py` & `bids2table-0.1.0b0/bids2table/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 r"""
-[bids2table](https://github.com/cmi-dair/bids2table) is a library for efficiently
+[bids2table](https://github.com/childmindresearch/bids2table) is a library for efficiently
 indexing and querying large-scale BIDS neuroimaging datasets and derivatives. It aims to
 improve upon the efficiency of [PyBIDS](https://github.com/bids-standard/pybids) by
 leveraging modern data science tools.
 
 bids2table represents a BIDS dataset index as a single table with columns for BIDS
 entities and file metadata. The index is constructed using
 [Arrow](https://arrow.apache.org/) and stored in [Parquet](https://parquet.apache.org/)
@@ -16,15 +16,15 @@
 ```sh
 pip install bids2table
 ```
 
 The latest development version can be installed with
 
 ```sh
-pip install git+https://github.com/cmi-dair/bids2table.git
+pip install git+https://github.com/childmindresearch/bids2table.git
 ```
 
 ## Quickstart
 
 The main entrypoint to the library is the `bids2table.bids2table` function, which builds
 the index.
```

### Comparing `bids2table-0.1.0a0/bids2table/__main__.py` & `bids2table-0.1.0b0/bids2table/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import sys
 from pathlib import Path
 
-from elbow.utils import setup_logging
-
 from bids2table import bids2table
+from bids2table.logging import setup_logging
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument("root", metavar="ROOT", type=Path, help="Path to BIDS dataset")
     parser.add_argument(
@@ -48,15 +47,15 @@
         "Incompatible with --overwrite. (default: None)",
         default=None,
     )
     parser.add_argument("--verbose", "-v", help="Verbose logging.", action="store_true")
 
     args = parser.parse_args()
 
-    setup_logging("INFO" if args.verbose else "ERROR")
+    setup_logging(level="INFO" if args.verbose else "WARNING")
 
     bids2table(
         root=args.root,
         persistent=True,
         index_path=args.output,
         incremental=args.incremental,
         overwrite=args.overwrite,
```

### Comparing `bids2table-0.1.0a0/bids2table/_b2t.py` & `bids2table-0.1.0b0/bids2table/_b2t.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from pathlib import Path
 from typing import Optional
 
 from elbow.builders import build_parquet, build_table
 from elbow.sources.filesystem import Crawler
 from elbow.typing import StrOrPath
-from elbow.utils import setup_logging
 
 from bids2table.extractors.bids import extract_bids_subdir
 from bids2table.table import BIDSTable
 
-setup_logging()
+logger = logging.getLogger("bids2table")
 
 
 def bids2table(
     root: StrOrPath,
     *,
     persistent: bool = False,
     index_path: Optional[StrOrPath] = None,
@@ -66,33 +65,33 @@
         index_path = root / "index.b2t"
     else:
         index_path = Path(index_path).resolve()
 
     stale = overwrite or incremental or worker_id is not None
     if index_path.exists() and not stale:
         if return_table:
-            logging.info("Loading cached index %s", index_path)
+            logger.info("Loading cached index %s", index_path)
             tab = BIDSTable.from_parquet(index_path)
         else:
-            logging.info("Found cached index %s; nothing to do", index_path)
+            logger.info("Found cached index %s; nothing to do", index_path)
             tab = None
         return tab
 
     if not persistent:
-        logging.info("Building index in memory")
+        logger.info("Building index in memory")
         df = build_table(
             source=source,
             extract=extract_bids_subdir,
             workers=workers,
             worker_id=worker_id,
         )
         tab = BIDSTable.from_df(df)
         return tab
 
-    logging.info("Building persistent Parquet index")
+    logger.info("Building persistent Parquet index")
     build_parquet(
         source=source,
         extract=extract_bids_subdir,
         output=index_path,
         incremental=incremental,
         overwrite=overwrite,
         workers=workers,
```

### Comparing `bids2table-0.1.0a0/bids2table/entities.py` & `bids2table-0.1.0b0/bids2table/entities.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/bids2table/extractors/bids.py` & `bids2table-0.1.0b0/bids2table/extractors/bids.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 from elbow.typing import StrOrPath
 
 from bids2table.entities import BIDSEntities
 
 from .dataset import extract_dataset
 from .metadata import extract_metadata, is_associated_sidecar
 
+logger = logging.getLogger(__name__)
+
 
 def extract_bids_file(path: StrOrPath) -> Optional[Record]:
     """
     Extract BIDS entities and metadata from a data file in a BIDS dataset.
     """
     if not is_bids_file(path):
         return None
 
     try:
         entities = BIDSEntities.from_path(path)
     except (TypeError, ValueError) as exc:
-        logging.warning(
+        logger.warning(
             "Incomplete and/or invalid entities in file %s", path, exc_info=exc
         )
         return None
 
     dset_rec = extract_dataset(path)
     meta_rec = extract_metadata(path)
     file_rec = extract_file_meta(path)
```

### Comparing `bids2table-0.1.0a0/bids2table/extractors/dataset.py` & `bids2table-0.1.0b0/bids2table/extractors/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 from elbow.record import Record
 from elbow.typing import StrOrPath
 
+logger = logging.getLogger(__name__)
+
 
 def extract_dataset(path: StrOrPath) -> Record:
     """
     Get info about the BIDS dataset that ``path`` belongs to.
     """
     name, root = identify_bids_dataset(path)
     desc = get_dataset_description(root) if root is not None else None
@@ -51,15 +53,15 @@
 
         if scanning:
             parts.append(parent.name)
 
         parent = parent.parent
 
     if len(parts) == 0:
-        logging.warning("File %s is not part of any valid BIDS dataset.", path)
+        logger.warning("File %s is not part of any valid BIDS dataset.", path)
         return None, None
 
     parts = parts[: top_idx + 1]
     dataset = "/".join(reversed(parts))
     return dataset, root
```

### Comparing `bids2table-0.1.0a0/bids2table/extractors/image.py` & `bids2table-0.1.0b0/bids2table/extractors/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 try:
     import nifti
 
     has_nifti = True
 except ModuleNotFoundError:
     has_nifti = False
 
+logger = logging.getLogger(__name__)
+
 # TODO: add more
 IMAGE_EXTENSIONS = {".nii", ".nii.gz"}
 
 
 def extract_image_meta(path: StrOrPath, *, backend: str = "nibabel") -> Record:
     entities = parse_bids_entities(path)
     ext = entities.get("ext")
 
     header = affine = None
     if ext in IMAGE_EXTENSIONS:
         try:
             header, affine = _read_image_meta(str(path), backend=backend)
         except (ImageFileError, SystemError) as exc:
-            logging.warning("Failed to load image %s", path, exc_info=exc)
+            logger.warning("Failed to load image %s", path, exc_info=exc)
 
     rec = Record(
         {"image_header": header, "image_affine": affine},
         types={"image_header": "json", "image_affine": "ndarray<float64>"},
     )
     return rec
```

### Comparing `bids2table-0.1.0a0/bids2table/extractors/inheritance.py` & `bids2table-0.1.0b0/bids2table/extractors/inheritance.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/bids2table/extractors/metadata.py` & `bids2table-0.1.0b0/bids2table/extractors/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from elbow.record import Record
 from elbow.typing import StrOrPath
 
 from bids2table.entities import parse_bids_entities
 
 from .inheritance import _glob, find_bids_parents
 
+logger = logging.getLogger(__name__)
+
 
 def extract_metadata(path: StrOrPath) -> Record:
     """
     Load the JSON sidecar metadata associated with ``path``. Supports metadata
     inheritance by searching up the directory tree for matching JSON files.
     """
     entities = parse_bids_entities(path)
@@ -22,15 +24,15 @@
     metadata = {}
     sidecars = reversed(list(find_bids_parents(query, start=Path(path).parent)))
     for path in sidecars:
         with open(path) as f:
             try:
                 metadata.update(json.load(f))
             except (json.JSONDecodeError, TypeError):
-                logging.warning(
+                logger.warning(
                     f"Bad JSON sidecar data {path}\n\n" + traceback.format_exc()
                 )
 
     # TODO: type aliases for json, pickle, etc so we can use a dataclass here.
     rec = Record({"json": metadata or None}, types={"json": "json"})
     return rec
```

### Comparing `bids2table-0.1.0a0/bids2table/table.py` & `bids2table-0.1.0b0/bids2table/table.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/bids2table.egg-info/PKG-INFO` & `bids2table-0.1.0b0/bids2table.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 Metadata-Version: 2.1
 Name: bids2table
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: Efficiently index large-scale BIDS datasets and derivatives
 Author-email: Connor Lane <connor.lane858@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/cmi-dair/bids2table
+Project-URL: Homepage, https://github.com/childmindresearch/bids2table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: elbow
+Requires-Dist: nibabel
+Requires-Dist: pandas
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: pdoc==14.0.0; extra == "dev"
+Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: flake8==5.0.4; extra == "dev"
+Requires-Dist: isort==5.11.5; extra == "dev"
+Requires-Dist: mypy==1.2.0; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint>=2.5.0; extra == "dev"
+Requires-Dist: setuptools-scm; extra == "dev"
 
 # bids2table
-[![Build](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/cmi-dair/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
-[![Docs](https://github.com/cmi-dair/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://cmi-dair.github.io/bids2table/bids2table)
-[![codecov](https://codecov.io/gh/cmi-dair/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/cmi-dair/bids2table)
+[![Build](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/bids2table/actions/workflows/ci.yaml?query=branch%3Amain)
+[![Docs](https://github.com/childmindresearch/bids2table/actions/workflows/docs.yaml/badge.svg?branch=main)](https://childmindresearch.github.io/bids2table/bids2table)
+[![codecov](https://codecov.io/gh/childmindresearch/bids2table/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/bids2table)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
 
 bids2table is a library for efficiently indexing and querying large-scale BIDS neuroimaging datasets and derivatives. It aims to improve upon the efficiency of [PyBIDS](https://github.com/bids-standard/pybids) by leveraging modern data science tools.
 
 bids2table represents a BIDS dataset index as a single table with columns for BIDS entities and file metadata. The index is constructed using [Arrow](https://arrow.apache.org/) and stored in [Parquet](https://parquet.apache.org/) format, a binary tabular file format optimized for efficient storage and retrieval.
 
@@ -39,20 +52,20 @@
 ```sh
 pip install bids2table
 ```
 
 The latest development version can be installed with
 
 ```sh
-pip install git+https://github.com/cmi-dair/bids2table.git
+pip install git+https://github.com/childmindresearch/bids2table.git
 ```
 
 ## Documentation
 
-Our documentation is [here](https://cmi-dair.github.io/bids2table/).
+Our documentation is [here](https://childmindresearch.github.io/bids2table/).
 
 ## Example
 
 ```python
 import pandas as pd
 
 from bids2table import bids2table
```

### Comparing `bids2table-0.1.0a0/bids2table.egg-info/SOURCES.txt` & `bids2table-0.1.0b0/bids2table.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 benchmark/query/requirements.txt
 benchmark/query/setup_environment.sh
 bids2table/__init__.py
 bids2table/__main__.py
 bids2table/_b2t.py
 bids2table/_version.py
 bids2table/entities.py
+bids2table/logging.py
 bids2table/table.py
 bids2table.egg-info/PKG-INFO
 bids2table.egg-info/SOURCES.txt
 bids2table.egg-info/dependency_links.txt
 bids2table.egg-info/entry_points.txt
 bids2table.egg-info/requires.txt
 bids2table.egg-info/top_level.txt
```

### Comparing `bids2table-0.1.0a0/example/example.ipynb` & `bids2table-0.1.0b0/example/example.ipynb`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/pyproject.toml` & `bids2table-0.1.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "mypy==1.2.0",
     "pre-commit",
     "pylint>=2.5.0",
     "setuptools-scm",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/cmi-dair/bids2table"
+"Homepage" = "https://github.com/childmindresearch/bids2table"
 
 [project.scripts]
 bids2table = "bids2table.__main__:main"
 b2t = "bids2table.__main__:main"
 
 [tool.setuptools.packages.find]
 include = ["bids2table*"]
```

### Comparing `bids2table-0.1.0a0/tests/test_bids2table.py` & `bids2table-0.1.0b0/tests/test_bids2table.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_entities.py` & `bids2table-0.1.0b0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_extractors/test_dataset.py` & `bids2table-0.1.0b0/tests/test_extractors/test_dataset.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_extractors/test_image.py` & `bids2table-0.1.0b0/tests/test_extractors/test_image.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_extractors/test_metadata.py` & `bids2table-0.1.0b0/tests/test_extractors/test_metadata.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_main.py` & `bids2table-0.1.0b0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bids2table-0.1.0a0/tests/test_table.py` & `bids2table-0.1.0b0/tests/test_table.py`

 * *Files identical despite different names*

