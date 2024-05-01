# Comparing `tmp/raven-cycode-1.0.8.tar.gz` & `tmp/raven_cycode-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raven-cycode-1.0.8.tar", last modified: Sun Mar 24 10:51:26 2024, max compression
+gzip compressed data, was "raven_cycode-1.0.9.tar", last modified: Wed May  1 14:13:38 2024, max compression
```

## Comparing `raven-cycode-1.0.8.tar` & `raven_cycode-1.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.715506 raven-cycode-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28896 2024-03-24 10:51:26.715506 raven-cycode-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27324 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/raven_cycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28896 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-24 10:51:26.000000 raven-cycode-1.0.8/raven_cycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 10:51:26.715506 raven-cycode-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/common/ignore_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/downloader/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/downloader/gh_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/indexer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/indexer/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/logger/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.707506 raven-cycode-1.0.8/src/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/src/reporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/reporter/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/reporter/slack_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/src/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/storage/neo4j_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/storage/neo4j_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/storage/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/storage/redis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/src/workflow_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/workflow_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/workflow_components/composite_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/workflow_components/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/workflow_components/parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/src/workflow_components/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/integration/integration_consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/integration/test_graph_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/tests_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:26.711506 raven-cycode-1.0.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_composite_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/unit/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-24 10:51:22.000000 raven-cycode-1.0.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.779138 raven_cycode-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28929 2024-05-01 14:13:38.779138 raven_cycode-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27357 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.779138 raven_cycode-1.0.9/raven_cycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28929 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-01 14:13:38.000000 raven_cycode-1.0.9/raven_cycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:13:38.779138 raven_cycode-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.771138 raven_cycode-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.771138 raven_cycode-1.0.9/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/common/ignore_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.771138 raven_cycode-1.0.9/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.771138 raven_cycode-1.0.9/src/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/downloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/downloader/gh_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/indexer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/indexer/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/logger/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/reporter/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/reporter/slack_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/storage/neo4j_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/storage/neo4j_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/storage/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/storage/redis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/src/workflow_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/workflow_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/workflow_components/composite_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/workflow_components/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/workflow_components/parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/src/workflow_components/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.775138 raven_cycode-1.0.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/integration/integration_consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/integration/test_graph_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/tests_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:38.779138 raven_cycode-1.0.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_composite_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/unit/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-01 14:13:34.000000 raven_cycode-1.0.9/tests/utils.py
```

### Comparing `raven-cycode-1.0.8/LICENSE.md` & `raven_cycode-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/PKG-INFO` & `raven_cycode-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-cycode
-Version: 1.0.8
+Version: 1.0.9
 Summary: RAVEN (Risk Analysis and Vulnerability Enumeration for CI/CD)
 Home-page: https://github.com/CycodeLabs/raven
 Author: ['Cycode <research@cycode.com>']
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CycodeLabs/raven
 Keywords: cycode,raven,security,ci/cd
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
-Requires-Dist: idna==3.6
+Requires-Dist: idna==3.7
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: interchange==2021.0.4
 Requires-Dist: loguru==0.7.2
 Requires-Dist: monotonic==1.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pansi==2020.7.3
 Requires-Dist: pluggy==1.4.0
@@ -169,30 +169,28 @@
 The tool contains three main functionalities, `download` and `index` and `report`.
 
 ### Download
 
 #### Download Account Repositories
 
 ```bash
-usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST]
-                                [--redis-port REDIS_PORT] [--clean-redis] --account-name
-                                ACCOUNT_NAME
+usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] (--account-name ACCOUNT_NAME | --personal)
 
 options:
   -h, --help            show this help message and exit
-  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective
-                        rate-limiting)
+  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective rate-limiting)
   --debug               Whether to print debug statements, default: False
   --redis-host REDIS_HOST
                         Redis host, default: localhost
   --redis-port REDIS_PORT
                         Redis port, default: 6379
   --clean-redis, -cr    Whether to clean cache in the redis, default: False
   --account-name ACCOUNT_NAME
-                        Account name for downloading the workflows
+                        Account name for downloading the workflows, can be used multiple times
+  --personal            Download repositories owned by the authenticated user
 ```
 
 #### Download Public Repositories
 
 ```bash
 usage: raven download crawl [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] [--max-stars MAX_STARS] [--min-stars MIN_STARS]
```

### Comparing `raven-cycode-1.0.8/README.md` & `raven_cycode-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -124,30 +124,28 @@
 The tool contains three main functionalities, `download` and `index` and `report`.
 
 ### Download
 
 #### Download Account Repositories
 
 ```bash
-usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST]
-                                [--redis-port REDIS_PORT] [--clean-redis] --account-name
-                                ACCOUNT_NAME
+usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] (--account-name ACCOUNT_NAME | --personal)
 
 options:
   -h, --help            show this help message and exit
-  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective
-                        rate-limiting)
+  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective rate-limiting)
   --debug               Whether to print debug statements, default: False
   --redis-host REDIS_HOST
                         Redis host, default: localhost
   --redis-port REDIS_PORT
                         Redis port, default: 6379
   --clean-redis, -cr    Whether to clean cache in the redis, default: False
   --account-name ACCOUNT_NAME
-                        Account name for downloading the workflows
+                        Account name for downloading the workflows, can be used multiple times
+  --personal            Download repositories owned by the authenticated user
 ```
 
 #### Download Public Repositories
 
 ```bash
 usage: raven download crawl [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] [--max-stars MAX_STARS] [--min-stars MIN_STARS]
```

### Comparing `raven-cycode-1.0.8/raven_cycode.egg-info/PKG-INFO` & `raven_cycode-1.0.9/raven_cycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-cycode
-Version: 1.0.8
+Version: 1.0.9
 Summary: RAVEN (Risk Analysis and Vulnerability Enumeration for CI/CD)
 Home-page: https://github.com/CycodeLabs/raven
 Author: ['Cycode <research@cycode.com>']
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CycodeLabs/raven
 Keywords: cycode,raven,security,ci/cd
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
-Requires-Dist: idna==3.6
+Requires-Dist: idna==3.7
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: interchange==2021.0.4
 Requires-Dist: loguru==0.7.2
 Requires-Dist: monotonic==1.6
 Requires-Dist: packaging==24.0
 Requires-Dist: pansi==2020.7.3
 Requires-Dist: pluggy==1.4.0
@@ -169,30 +169,28 @@
 The tool contains three main functionalities, `download` and `index` and `report`.
 
 ### Download
 
 #### Download Account Repositories
 
 ```bash
-usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST]
-                                [--redis-port REDIS_PORT] [--clean-redis] --account-name
-                                ACCOUNT_NAME
+usage: raven download account [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] (--account-name ACCOUNT_NAME | --personal)
 
 options:
   -h, --help            show this help message and exit
-  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective
-                        rate-limiting)
+  --token TOKEN         GITHUB_TOKEN to download data from Github API (Needed for effective rate-limiting)
   --debug               Whether to print debug statements, default: False
   --redis-host REDIS_HOST
                         Redis host, default: localhost
   --redis-port REDIS_PORT
                         Redis port, default: 6379
   --clean-redis, -cr    Whether to clean cache in the redis, default: False
   --account-name ACCOUNT_NAME
-                        Account name for downloading the workflows
+                        Account name for downloading the workflows, can be used multiple times
+  --personal            Download repositories owned by the authenticated user
 ```
 
 #### Download Public Repositories
 
 ```bash
 usage: raven download crawl [-h] --token TOKEN [--debug] [--redis-host REDIS_HOST] [--redis-port REDIS_PORT] [--clean-redis] [--max-stars MAX_STARS] [--min-stars MIN_STARS]
```

### Comparing `raven-cycode-1.0.8/raven_cycode.egg-info/SOURCES.txt` & `raven_cycode-1.0.9/raven_cycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/setup.py` & `raven_cycode-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/cmdline.py` & `raven_cycode-1.0.9/src/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,32 +141,44 @@
 
     account_download_parser = download_sub_parser.add_parser(
         "account",
         help="Scan a specific GitHub account (user or organization)",
         parents=[download_parser_options, redis_parser],
     )
 
+    account_download_group = account_download_parser.add_mutually_exclusive_group(
+        required=True
+    )
+
+    account_download_group.add_argument(
+        "--account-name",
+        required=False,
+        action="append",
+        type=str,
+        help="Account name for downloading the workflows, can be used multiple times",
+    )
+
+    account_download_group.add_argument(
+        "--personal",
+        required=False,
+        action="store_const",
+        const=True,
+        help="Download repositories owned by the authenticated user",
+    )
+
     crawl_download_parser.add_argument(
         "--max-stars", type=int, help="Maximum number of stars for a repository"
     )
     crawl_download_parser.add_argument(
         "--min-stars",
         type=int,
         default=MIN_STARS_DEFAULT,
         help=f"Minimum number of stars for a repository, default: {MIN_STARS_DEFAULT}",
     )
 
-    account_download_parser.add_argument(
-        "--account-name",
-        required=True,
-        action="append",
-        type=str,
-        help="Account name for downloading the workflows",
-    )
-
     # Index action
     index_parser = subparsers.add_parser(
         "index",
         parents=[redis_parser, neo4j_parser],
         help="Index the download workflows into Neo4j database",
     )
     index_parser.add_argument(
```

### Comparing `raven-cycode-1.0.8/src/common/utils.py` & `raven_cycode-1.0.9/src/common/utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/config/config.py` & `raven_cycode-1.0.9/src/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     Includes redis config.
     """
     Config.debug = args.get("debug", DEBUG_DEFAULT)
     Config.github_token = args.get("token")
     Config.min_stars = args.get("min_stars", MIN_STARS_DEFAULT)
     Config.max_stars = args.get("max_stars")
     Config.account_name = args.get("account_name")
+    Config.personal = args.get("personal")
     Config.clean_redis = args.get("clean_redis", REDIS_CLEAN_DEFAULT)
 
     load_redis_config(args)
 
     if Config.clean_redis:
         from src.storage.redis_utils import clean_redis_db
 
@@ -138,14 +139,15 @@
     debug: bool = None
 
     # Downloader Config
     github_token: str = None
     min_stars: int = None
     max_stars: int = None
     account_name: list[str] = []
+    personal: bool = None
 
     # Indexer Configs
     clean_neo4j: bool = None
 
     # Redis Config
     redis_host: str = None
     redis_port: int = None
```

### Comparing `raven-cycode-1.0.8/src/downloader/download.py` & `raven_cycode-1.0.9/src/downloader/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from src.storage.redis_connection import RedisConnection
 from src.downloader.utils import (
     insert_workflow_or_action_to_redis,
     add_ref_pointer_to_redis,
 )
 from src.downloader.gh_api import (
     get_account_generator,
+    get_personal_account_generator,
     get_repository_generator,
     get_repository_workflows,
     get_repository_composite_action,
     get_repository_reusable_workflow,
 )
 from src.common.utils import (
     find_uses_strings,
@@ -34,20 +35,30 @@
     so we download it as well.
 
     For each such workflow we also scan if it uses additional external actions.
     If so, we download these as well.
 
     We are trying to cache the downloads as much as we can to reduce redundant download attempts.
     """
-    for account in Config.account_name:
-        generator = get_account_generator(account)
+    if Config.account_name:
+        for account in Config.account_name:
+            generator = get_account_generator(account)
+
+            for repo in generator:
+                download_workflows_and_actions(repo)
+
+    elif Config.personal:
+        generator = get_personal_account_generator()
 
         for repo in generator:
             download_workflows_and_actions(repo)
 
+    else:
+        raise Exception("Account name or personal flag must be provided.")
+
 
 def download_all_workflows_and_actions() -> None:
     """Iterating all repositories through Github search API.
 
     For each repository we enumerating the .github/workflows directory,
     and downloading all the workflows.
     In addition if the repository contains action.yml file, it means it is a composite action,
```

### Comparing `raven-cycode-1.0.8/src/downloader/gh_api.py` & `raven_cycode-1.0.9/src/downloader/gh_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,54 +19,71 @@
 """
 
 BASE_URL = "https://api.github.com"
 REPOSITORY_SEARCH_URL = (
     BASE_URL
     + "/search/repositories?q={query}&sort=stars&order=desc&per_page=100&page={page}"
 )
+
+
 ACCOUNT_INFO_URL = BASE_URL + "/users/{account_name}"
-USER_REPOSITORY_URL = BASE_URL + "/user/repos?type=owner&per_page=100&page={page}"
+USER_REPOSITORY_URL = BASE_URL + "/users/{user_name}/repos?per_page=100&page={page}"
+
+PERSONAL_USER_REPOSITORY_URL = (
+    BASE_URL + "/user/repos?type=owner&per_page=100&page={page}"
+)
+
 ORGANIZATION_REPOSITORY_URL = (
     BASE_URL + "/orgs/{organization_name}/repos?per_page=100&page={page}"
 )
 CONTENTS_URL = BASE_URL + "/repos/{repo_path}/contents/{file_path}"
 
 REPOSITORY_QUERY_MIN = "stars:>={min_stars}"
 REPOSITORY_QUERY_MIN_MAX = "stars:{min_stars}..{max_stars}"
 
 headers = {
     "Accept": "application/vnd.github+json",
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36 Edg/107.0.1418.42",
 }
 
 
+def get_personal_account_generator() -> Iterator[str]:
+    return get_user_repository_generator(user_name=None, is_personal_account=True)
+
+
 def get_account_generator(account_name: str) -> Iterator[str]:
     account_info = get_account_info(account_name=account_name)
     account_type = account_info.get("type")
 
     if account_type == "User":
         log.info(f"[+] Scanning user: {account_name}")
-        return get_user_repository_generator(account_name)
+        return get_user_repository_generator(
+            user_name=account_name, is_personal_account=False
+        )
 
     elif account_type == "Organization":
         log.info(f"[+] Scanning organization: {account_name}")
         return get_organization_repository_generator(account_name)
 
     else:
         log.error(f"[-] Failed to get account type for {account_name}")
         return None
 
 
-def get_user_repository_generator(user_name: str) -> Iterator[str]:
+def get_user_repository_generator(
+    user_name: str, is_personal_account: bool
+) -> Iterator[str]:
     # Quering user repositories is not limited. We loop over each page,
     # and look for more repos. If there are no more repos, we break
     page = 1
     while True:
         log.info(f"[*] Querying page: {page}")
-        repos = get_user_repository(user_name=user_name, page=page)
+        repos = get_user_repositories(
+            user_name=user_name, page=page, is_personal_account=is_personal_account
+        )
         if repos:
             for repo in repos:
                 repo_star_count = int(repo["stargazers_count"])
                 log.debug(
                     f"[+] About to download repository: {repo['full_name']}, Stars: {repo_star_count}"
                 )
                 yield repo["full_name"]
@@ -78,15 +95,15 @@
 
 def get_organization_repository_generator(organization_name: str) -> Iterator[str]:
     # Quering organization repositories is not limited. We loop over each page,
     # and look for more repos. If there are no more repos, we break
     page = 1
     while True:
         log.info(f"[*] Querying page: {page}")
-        repos = get_organization_repository(
+        repos = get_organization_repositories(
             organization_name=organization_name, page=page
         )
         if repos:
             for repo in repos:
                 repo_star_count = int(repo["stargazers_count"])
                 log.debug(
                     f"[+] About to download repository: {repo['full_name']}, Stars: {repo_star_count}"
@@ -160,41 +177,47 @@
     if r.status_code != HTTPStatus.OK:
         log.error(f"[-] Failed fetching repositories for {account_name}")
         raise Exception(f"status code: {r.status_code}. Response: {r.text}")
 
     return r.json()
 
 
-def get_user_repository(user_name: str, page: int) -> list[dict]:
+def get_user_repositories(
+    user_name: str, page: int, is_personal_account: bool
+) -> list[dict]:
     """
     Returns a list of all repositories for the specified user.
     The objects look like this:
     {
         "id": 000000000,
         "node_id": "R_...",
         "name": "example",
         "full_name": "example/example",
         "private": true,
         ...
     }
     """
     headers["Authorization"] = f"Token {Config.github_token}"
 
+    repo_endpoint = (
+        PERSONAL_USER_REPOSITORY_URL if is_personal_account else USER_REPOSITORY_URL
+    )
     r = get(
-        USER_REPOSITORY_URL.format(page=page),
+        repo_endpoint.format(user_name=user_name, page=page),
         headers=headers,
     )
+
     if r.status_code != HTTPStatus.OK:
-        log.error(f"[-] Failed fetching repositories for {user_name}")
+        log.error(f"[-] Failed fetching repositories")
         raise Exception(f"status code: {r.status_code}. Response: {r.text}")
 
     return r.json()
 
 
-def get_organization_repository(organization_name: str, page: int) -> list[dict]:
+def get_organization_repositories(organization_name: str, page: int) -> list[dict]:
     """
     Returns a list of all repositories for the specified organization.
     The objects look like this:
     {
         "id": 000000000,
         "node_id": "R_...",
         "name": "example",
```

### Comparing `raven-cycode-1.0.8/src/downloader/utils.py` & `raven_cycode-1.0.9/src/downloader/utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/indexer/index.py` & `raven_cycode-1.0.9/src/indexer/index.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/logger/log.py` & `raven_cycode-1.0.9/src/logger/log.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/queries/__init__.py` & `raven_cycode-1.0.9/src/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/reporter/report.py` & `raven_cycode-1.0.9/src/reporter/report.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/reporter/slack_reporter.py` & `raven_cycode-1.0.9/src/reporter/slack_reporter.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/storage/neo4j_graph.py` & `raven_cycode-1.0.9/src/storage/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/storage/redis_connection.py` & `raven_cycode-1.0.9/src/storage/redis_connection.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/storage/redis_utils.py` & `raven_cycode-1.0.9/src/storage/redis_utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/workflow_components/composite_action.py` & `raven_cycode-1.0.9/src/workflow_components/composite_action.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/workflow_components/dependency.py` & `raven_cycode-1.0.9/src/workflow_components/dependency.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/workflow_components/parsing_utils.py` & `raven_cycode-1.0.9/src/workflow_components/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/src/workflow_components/workflow.py` & `raven_cycode-1.0.9/src/workflow_components/workflow.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/integration/integration_consts.py` & `raven_cycode-1.0.9/tests/integration/integration_consts.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/integration/test_graph_structures.py` & `raven_cycode-1.0.9/tests/integration/test_graph_structures.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/tests_init.py` & `raven_cycode-1.0.9/tests/tests_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     load_downloader_config(
         {
             "debug": False,
             "token": getenv("GITHUB_TOKEN"),
             "account_name": ["RavenIntegrationTests"],
             "redis_host": "raven-redis-test",
             "redis_port": 6379,
-            "clean_redis": False,
+            "clean_redis": True,
         }
     )
 
     load_indexer_config(
         {
             "debug": False,
             "redis_host": "raven-redis-test",
             "redis_port": 6379,
-            "clean_redis": False,
+            "clean_redis": True,
             "neo4j_uri": "neo4j://raven-neo4j-test:7687",
             "neo4j_user": "neo4j",
             "neo4j_pass": "123456789",
             "threads": 1,
-            "clean_neo4j": False,
+            "clean_neo4j": True,
         }
     )
```

### Comparing `raven-cycode-1.0.8/tests/unit/test_composite_action.py` & `raven_cycode-1.0.9/tests/unit/test_composite_action.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/unit/test_dependency.py` & `raven_cycode-1.0.9/tests/unit/test_dependency.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/unit/test_parsing_utils.py` & `raven_cycode-1.0.9/tests/unit/test_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/unit/test_report.py` & `raven_cycode-1.0.9/tests/unit/test_report.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/unit/test_utils.py` & `raven_cycode-1.0.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/unit/test_workflow.py` & `raven_cycode-1.0.9/tests/unit/test_workflow.py`

 * *Files identical despite different names*

### Comparing `raven-cycode-1.0.8/tests/utils.py` & `raven_cycode-1.0.9/tests/utils.py`

 * *Files identical despite different names*

