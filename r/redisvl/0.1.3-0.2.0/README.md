# Comparing `tmp/redisvl-0.1.3.tar.gz` & `tmp/redisvl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redisvl-0.1.3.tar", last modified: Tue Apr  9 16:07:21 2024, max compression
+gzip compressed data, was "redisvl-0.2.0.tar", max compression
```

## Comparing `redisvl-0.1.3.tar` & `redisvl-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 16:07:17.000000 redisvl-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-09 16:07:21.640422 redisvl-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-04-09 16:07:17.000000 redisvl-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 16:07:17.000000 redisvl-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.632422 redisvl-0.1.3/redisvl/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/extensions/llmcache/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/semantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/index/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35935 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/query/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/redis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/token_escaper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/vectorize/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/vectorize/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 16:07:21.640422 redisvl-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 16:07:17.000000 redisvl-0.1.3/setup.py
+-rw-r--r--   0        0        0     1068 2024-05-01 19:02:34.225653 redisvl-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12455 2024-05-01 19:02:34.225653 redisvl-0.2.0/README.md
+-rw-r--r--   0        0        0     2871 2024-05-01 19:02:50.545824 redisvl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/__init__.py
+-rw-r--r--   0        0        0     5695 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/index.py
+-rw-r--r--   0        0        0     1181 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/main.py
+-rw-r--r--   0        0        0      161 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/runner.py
+-rw-r--r--   0        0        0     2779 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/stats.py
+-rw-r--r--   0        0        0     1478 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/utils.py
+-rw-r--r--   0        0        0      740 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/cli/version.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/extensions/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/extensions/llmcache/__init__.py
+-rw-r--r--   0        0        0     1993 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/extensions/llmcache/base.py
+-rw-r--r--   0        0        0    12879 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/extensions/llmcache/semantic.py
+-rw-r--r--   0        0        0      109 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/index/__init__.py
+-rw-r--r--   0        0        0    35935 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/index/index.py
+-rw-r--r--   0        0        0    18469 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/index/storage.py
+-rw-r--r--   0        0        0      151 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/query/__init__.py
+-rw-r--r--   0        0        0    17821 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/query/filter.py
+-rw-r--r--   0        0        0    13740 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/query/query.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/redis/__init__.py
+-rw-r--r--   0        0        0     6498 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/redis/connection.py
+-rw-r--r--   0        0        0      180 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/redis/constants.py
+-rw-r--r--   0        0        0     1177 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/redis/utils.py
+-rw-r--r--   0        0        0      125 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/schema/__init__.py
+-rw-r--r--   0        0        0    10698 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/schema/fields.py
+-rw-r--r--   0        0        0    17186 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/schema/schema.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/log.py
+-rw-r--r--   0        0        0      163 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/rerank/__init__.py
+-rw-r--r--   0        0        0     1506 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/rerank/base.py
+-rw-r--r--   0        0        0     7797 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/rerank/cohere.py
+-rw-r--r--   0        0        0     1028 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/token_escaper.py
+-rw-r--r--   0        0        0      597 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/__init__.py
+-rw-r--r--   0        0        0     1965 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/base.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/__init__.py
+-rw-r--r--   0        0        0    11501 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/azureopenai.py
+-rw-r--r--   0        0        0    10081 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/cohere.py
+-rw-r--r--   0        0        0     6090 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/huggingface.py
+-rw-r--r--   0        0        0     9843 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/openai.py
+-rw-r--r--   0        0        0     7762 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/utils/vectorize/text/vertexai.py
+-rw-r--r--   0        0        0       22 2024-05-01 19:02:34.237653 redisvl-0.2.0/redisvl/version.py
+-rw-r--r--   0        0        0    13954 1970-01-01 00:00:00.000000 redisvl-0.2.0/PKG-INFO
```

### Comparing `redisvl-0.1.3/LICENSE` & `redisvl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/PKG-INFO` & `redisvl-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: redisvl
-Version: 0.1.3
-Summary: Python client library and CLI for using Redis as a vector database
-Home-page: https://github.com/RedisVentures/redisvl
-Author: Redis Inc.
-License: MIT
-Project-URL: Source, https://github.com/RedisVentures/redisvl
-Project-URL: Documentation, https://www.redisvl.com
-Keywords: ai,redis,redis-client,vector-database,vector-search
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1 align="center">🔥 Redis Vector Library</h1>
 
 <div align="center">
         <span style="font-size: smaller;">the AI-native Redis Python client</span>
         <br />
 
 [![Codecov](https://img.shields.io/codecov/c/github/RedisVentures/RedisVL/dev?label=Codecov&logo=codecov&token=E30WxqBeJJ)](https://codecov.io/gh/RedisVentures/RedisVL)
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: redisvl Version: 0.1.3 Summary: Python client
-library and CLI for using Redis as a vector database Home-page: https://
-github.com/RedisVentures/redisvl Author: Redis Inc. License: MIT Project-URL:
-Source, https://github.com/RedisVentures/redisvl Project-URL: Documentation,
-https://www.redisvl.com Keywords: ai,redis,redis-client,vector-database,vector-
-search Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-License :: OSI Approved :: MIT License Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: all Provides-Extra: dev License-
-File: LICENSE
                     ************ ?ð???¥ RReeddiiss VVeeccttoorr LLiibbrraarryy ************
                       the AI-native Redis Python client
   [![Codecov](https://img.shields.io/codecov/c/github/RedisVentures/RedisVL/
    dev?label=Codecov&logo=codecov&token=E30WxqBeJJ)](https://codecov.io/gh/
  RedisVentures/RedisVL) [![License: MIT](https://img.shields.io/badge/License-
   MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![Language](https://
    img.shields.io/github/languages/top/RedisVentures/RedisVL) [![Code style:
```

### Comparing `redisvl-0.1.3/README.md` & `redisvl-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: redisvl
+Version: 0.2.0
+Summary: Python client library and CLI for using Redis as a vector database
+Home-page: https://github.com/RedisVentures/redisvl
+License: MIT
+Keywords: ai,redis,redis-client,vector-database,vector-search
+Author: Redis Inc.
+Author-email: applied.ai@redis.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: cohere
+Provides-Extra: google-cloud-aiplatform
+Provides-Extra: openai
+Provides-Extra: sentence-transformers
+Requires-Dist: cohere (>=4.44) ; extra == "cohere"
+Requires-Dist: coloredlogs
+Requires-Dist: google-cloud-aiplatform (>=1.26) ; extra == "google-cloud-aiplatform"
+Requires-Dist: numpy
+Requires-Dist: openai (>=1.13.0) ; extra == "openai"
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pyyaml
+Requires-Dist: redis (>=5.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2) ; extra == "sentence-transformers"
+Requires-Dist: tabulate (>=0.9.0,<1)
+Requires-Dist: tenacity (>=8.2.2)
+Project-URL: Documentation, https://www.redisvl.com
+Project-URL: Repository, https://github.com/RedisVentures/redisvl
+Description-Content-Type: text/markdown
+
 <h1 align="center">🔥 Redis Vector Library</h1>
 
 <div align="center">
         <span style="font-size: smaller;">the AI-native Redis Python client</span>
         <br />
 
 [![Codecov](https://img.shields.io/codecov/c/github/RedisVentures/RedisVL/dev?label=Codecov&logo=codecov&token=E30WxqBeJJ)](https://codecov.io/gh/RedisVentures/RedisVL)
@@ -285,7 +322,8 @@
 
 ## 🫱🏼‍🫲🏽 Contributing
 
 Please help us by contributing PRs, opening GitHub issues for bugs or new feature ideas, improving documentation, or increasing test coverage. [Read more about how to contribute!](CONTRIBUTING.md)
 
 ## 🚧 Maintenance
 This project is supported by [Redis, Inc](https://redis.com) on a good faith effort basis. To report bugs, request features, or receive assistance, please [file an issue](https://github.com/RedisVentures/redisvl/issues).
+
```

#### html2text {}

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1 Name: redisvl Version: 0.2.0 Summary: Python client
+library and CLI for using Redis as a vector database Home-page: https://
+github.com/RedisVentures/redisvl License: MIT Keywords: ai,redis,redis-
+client,vector-database,vector-search Author: Redis Inc. Author-email:
+applied.ai@redis.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: cohere Provides-Extra: google-cloud-aiplatform Provides-Extra:
+openai Provides-Extra: sentence-transformers Requires-Dist: cohere (>=4.44) ;
+extra == "cohere" Requires-Dist: coloredlogs Requires-Dist: google-cloud-
+aiplatform (>=1.26) ; extra == "google-cloud-aiplatform" Requires-Dist: numpy
+Requires-Dist: openai (>=1.13.0) ; extra == "openai" Requires-Dist: pydantic
+(>=2,<3) Requires-Dist: pyyaml Requires-Dist: redis (>=5.0.0) Requires-Dist:
+sentence-transformers (>=2.2.2) ; extra == "sentence-transformers" Requires-
+Dist: tabulate (>=0.9.0,<1) Requires-Dist: tenacity (>=8.2.2) Project-URL:
+Documentation, https://www.redisvl.com Project-URL: Repository, https://
+github.com/RedisVentures/redisvl Description-Content-Type: text/markdown
                     ************ ?ð???¥ RReeddiiss VVeeccttoorr LLiibbrraarryy ************
                       the AI-native Redis Python client
   [![Codecov](https://img.shields.io/codecov/c/github/RedisVentures/RedisVL/
    dev?label=Codecov&logo=codecov&token=E30WxqBeJJ)](https://codecov.io/gh/
  RedisVentures/RedisVL) [![License: MIT](https://img.shields.io/badge/License-
   MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![Language](https://
    img.shields.io/github/languages/top/RedisVentures/RedisVL) [![Code style:
```

### Comparing `redisvl-0.1.3/redisvl/cli/index.py` & `redisvl-0.2.0/redisvl/cli/index.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/cli/main.py` & `redisvl-0.2.0/redisvl/cli/main.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/cli/stats.py` & `redisvl-0.2.0/redisvl/cli/stats.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/cli/utils.py` & `redisvl-0.2.0/redisvl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/cli/version.py` & `redisvl-0.2.0/redisvl/cli/version.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/extensions/llmcache/base.py` & `redisvl-0.2.0/redisvl/extensions/llmcache/base.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/extensions/llmcache/semantic.py` & `redisvl-0.2.0/redisvl/extensions/llmcache/semantic.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/index/index.py` & `redisvl-0.2.0/redisvl/index/index.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/index/storage.py` & `redisvl-0.2.0/redisvl/index/storage.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/query/filter.py` & `redisvl-0.2.0/redisvl/query/filter.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/query/query.py` & `redisvl-0.2.0/redisvl/query/query.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/redis/connection.py` & `redisvl-0.2.0/redisvl/redis/connection.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/redis/utils.py` & `redisvl-0.2.0/redisvl/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/schema/fields.py` & `redisvl-0.2.0/redisvl/schema/fields.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/schema/schema.py` & `redisvl-0.2.0/redisvl/schema/schema.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/utils/log.py` & `redisvl-0.2.0/redisvl/utils/log.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/utils/token_escaper.py` & `redisvl-0.2.0/redisvl/utils/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.3/redisvl/utils/vectorize/base.py` & `redisvl-0.2.0/redisvl/utils/vectorize/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-from typing import Any, Callable, List, Optional
+from abc import ABC, abstractmethod
+from typing import Callable, List, Optional
 
 from pydantic.v1 import BaseModel, validator
 
 from redisvl.redis.utils import array_to_buffer
 
 
-class BaseVectorizer(BaseModel):
+class BaseVectorizer(BaseModel, ABC):
     model: str
     dims: int
-    client: Any
 
-    @validator("dims", pre=True)
+    @validator("dims")
     @classmethod
-    def check_dims(cls, v):
-        if v <= 0:
-            raise ValueError("Dimension must be a positive integer")
-        return v
+    def check_dims(cls, value):
+        """Ensures the dims are a positive integer."""
+        if value <= 0:
+            raise ValueError("Dims must be a positive integer.")
+        return value
 
+    @abstractmethod
     def embed_many(
         self,
         texts: List[str],
         preprocess: Optional[Callable] = None,
         batch_size: int = 1000,
         as_buffer: bool = False,
         **kwargs,
     ) -> List[List[float]]:
         raise NotImplementedError
 
+    @abstractmethod
     def embed(
         self,
         text: str,
         preprocess: Optional[Callable] = None,
         as_buffer: bool = False,
         **kwargs,
     ) -> List[float]:
         raise NotImplementedError
 
+    @abstractmethod
     async def aembed_many(
         self,
         texts: List[str],
         preprocess: Optional[Callable] = None,
         batch_size: int = 1000,
         as_buffer: bool = False,
         **kwargs,
     ) -> List[List[float]]:
         raise NotImplementedError
 
+    @abstractmethod
     async def aembed(
         self,
         text: str,
         preprocess: Optional[Callable] = None,
         as_buffer: bool = False,
         **kwargs,
     ) -> List[float]:
```

### Comparing `redisvl-0.1.3/redisvl/utils/vectorize/text/cohere.py` & `redisvl-0.2.0/redisvl/utils/vectorize/text/cohere.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
-from typing import Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 
+from pydantic.v1 import PrivateAttr
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from tenacity.retry import retry_if_not_exception_type
 
 from redisvl.utils.vectorize.base import BaseVectorizer
 
 # ignore that cohere isn't imported
 # mypy: disable-error-code="name-defined"
@@ -39,14 +40,16 @@
         doc_embeddings = cohere.embed_many(
             texts=["your document text", "more document text"],
             input_type="search_document"
         )
 
     """
 
+    _client: Any = PrivateAttr()
+
     def __init__(
         self, model: str = "embed-english-v3.0", api_config: Optional[Dict] = None
     ):
         """Initialize the Cohere vectorizer.
 
         Visit https://cohere.ai/embed to learn about embeddings.
 
@@ -56,17 +59,25 @@
                 Defaults to None.
 
         Raises:
             ImportError: If the cohere library is not installed.
             ValueError: If the API key is not provided.
 
         """
+        self._initialize_client(api_config)
+        super().__init__(model=model, dims=self._set_model_dims(model))
+
+    def _initialize_client(self, api_config: Optional[Dict]):
+        """
+        Setup the Cohere clients using the provided API key or an
+        environment variable.
+        """
         # Dynamic import of the cohere module
         try:
-            import cohere
+            from cohere import AsyncClient, Client
         except ImportError:
             raise ImportError(
                 "Cohere vectorizer requires the cohere library. \
                     Please install with `pip install cohere`"
             )
 
         # Fetch the API key from api_config or environment variable
@@ -74,23 +85,19 @@
             api_config.get("api_key") if api_config else os.getenv("COHERE_API_KEY")
         )
         if not api_key:
             raise ValueError(
                 "Cohere API key is required. "
                 "Provide it in api_config or set the COHERE_API_KEY environment variable."
             )
+        self._client = Client(api_key=api_key, client_name="redisvl")
 
-        client = cohere.Client(api_key, client_name="redisvl")
-        dims = self._set_model_dims(client, model)
-        super().__init__(model=model, dims=dims, client=client)
-
-    @staticmethod
-    def _set_model_dims(client, model) -> int:
+    def _set_model_dims(self, model) -> int:
         try:
-            embedding = client.embed(
+            embedding = self._client.embed(
                 texts=["dimension test"],
                 model=model,
                 input_type="search_document",
             ).embeddings[0]
         except (KeyError, IndexError) as ke:
             raise ValueError(f"Unexpected response from the Cohere API: {str(ke)}")
         except Exception as e:  # pylint: disable=broad-except
@@ -146,15 +153,15 @@
         if not isinstance(input_type, str):
             raise TypeError(
                 "Must pass in a str value for cohere embedding input_type. \
                     See https://docs.cohere.com/reference/embed."
             )
         if preprocess:
             text = preprocess(text)
-        embedding = self.client.embed(
+        embedding = self._client.embed(
             texts=[text], model=self.model, input_type=input_type
         ).embeddings[0]
         return self._process_embedding(embedding, as_buffer)
 
     @retry(
         wait=wait_random_exponential(min=1, max=60),
         stop=stop_after_attempt(6),
@@ -215,15 +222,34 @@
             raise TypeError(
                 "Must pass in a str value for cohere embedding input_type.\
                     See https://docs.cohere.com/reference/embed."
             )
 
         embeddings: List = []
         for batch in self.batchify(texts, batch_size, preprocess):
-            response = self.client.embed(
+            response = self._client.embed(
                 texts=batch, model=self.model, input_type=input_type
             )
             embeddings += [
                 self._process_embedding(embedding, as_buffer)
                 for embedding in response.embeddings
             ]
         return embeddings
+
+    async def aembed_many(
+        self,
+        texts: List[str],
+        preprocess: Optional[Callable] = None,
+        batch_size: int = 1000,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[List[float]]:
+        raise NotImplementedError
+
+    async def aembed(
+        self,
+        text: str,
+        preprocess: Optional[Callable] = None,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[float]:
+        raise NotImplementedError
```

### Comparing `redisvl-0.1.3/redisvl/utils/vectorize/text/huggingface.py` & `redisvl-0.2.0/redisvl/utils/vectorize/text/huggingface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Callable, Dict, List, Optional
+from typing import Any, Callable, List, Optional
+
+from pydantic.v1 import PrivateAttr
 
 from redisvl.utils.vectorize.base import BaseVectorizer
 
 
 class HFTextVectorizer(BaseVectorizer):
     """The HFTextVectorizer class is designed to leverage the power of Hugging
     Face's Sentence Transformers for generating text embeddings. This vectorizer
@@ -24,45 +26,49 @@
         embedding = vectorizer.embed("Hello, world!")
 
         # Embedding a batch of texts
         embeddings = vectorizer.embed_many(["Hello, world!", "How are you?"], batch_size=2)
 
     """
 
+    _client: Any = PrivateAttr()
+
     def __init__(
         self, model: str = "sentence-transformers/all-mpnet-base-v2", **kwargs
     ):
         """Initialize the Hugging Face text vectorizer.
 
         Args:
             model (str): The pre-trained model from Hugging Face's Sentence
                 Transformers to be used for embedding. Defaults to
                 'sentence-transformers/all-mpnet-base-v2'.
 
         Raises:
             ImportError: If the sentence-transformers library is not installed.
             ValueError: If there is an error setting the embedding model dimensions.
         """
-        # Load the SentenceTransformer model
+        self._initialize_client(model)
+        super().__init__(model=model, dims=self._set_model_dims())
+
+    def _initialize_client(self, model: str):
+        """Setup the HuggingFace client"""
+        # Dynamic import of the cohere module\
         try:
             from sentence_transformers import SentenceTransformer
         except ImportError:
             raise ImportError(
                 "HFTextVectorizer requires the sentence-transformers library. "
                 "Please install with `pip install sentence-transformers`"
             )
 
-        client = SentenceTransformer(model)
-        dims = self._set_model_dims(client)
-        super().__init__(model=model, dims=dims, client=client)
+        self._client = SentenceTransformer(model)
 
-    @staticmethod
-    def _set_model_dims(client):
+    def _set_model_dims(self):
         try:
-            embedding = client.encode(["dimension check"])[0]
+            embedding = self._client.encode(["dimension check"])[0]
         except (KeyError, IndexError) as ke:
             raise ValueError(f"Empty response from the embedding model: {str(ke)}")
         except Exception as e:  # pylint: disable=broad-except
             # fall back (TODO get more specific)
             raise ValueError(f"Error setting embedding model dimensions: {str(e)}")
         return len(embedding)
 
@@ -89,15 +95,15 @@
             TypeError: If the wrong input type is passed in for the text.
         """
         if not isinstance(text, str):
             raise TypeError("Must pass in a str value to embed.")
 
         if preprocess:
             text = preprocess(text)
-        embedding = self.client.encode([text])[0]
+        embedding = self._client.encode([text])[0]
         return self._process_embedding(embedding.tolist(), as_buffer)
 
     def embed_many(
         self,
         texts: List[str],
         preprocess: Optional[Callable] = None,
         batch_size: int = 1000,
@@ -125,15 +131,34 @@
         if not isinstance(texts, list):
             raise TypeError("Must pass in a list of str values to embed.")
         if len(texts) > 0 and not isinstance(texts[0], str):
             raise TypeError("Must pass in a list of str values to embed.")
 
         embeddings: List = []
         for batch in self.batchify(texts, batch_size, preprocess):
-            batch_embeddings = self.client.encode(batch)
+            batch_embeddings = self._client.encode(batch)
             embeddings.extend(
                 [
                     self._process_embedding(embedding.tolist(), as_buffer)
                     for embedding in batch_embeddings
                 ]
             )
         return embeddings
+
+    async def aembed_many(
+        self,
+        texts: List[str],
+        preprocess: Optional[Callable] = None,
+        batch_size: int = 1000,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[List[float]]:
+        raise NotImplementedError
+
+    async def aembed(
+        self,
+        text: str,
+        preprocess: Optional[Callable] = None,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[float]:
+        raise NotImplementedError
```

### Comparing `redisvl-0.1.3/redisvl/utils/vectorize/text/openai.py` & `redisvl-0.2.0/redisvl/utils/vectorize/text/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from typing import Any, Callable, Dict, List, Optional
 
+from pydantic.v1 import PrivateAttr
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from tenacity.retry import retry_if_not_exception_type
 
 from redisvl.utils.vectorize.base import BaseVectorizer
 
 # ignore that openai isn't imported
 # mypy: disable-error-code="name-defined"
@@ -38,15 +39,16 @@
         embeddings = await vectorizer.aembed_many(
             ["Hello, world!", "How are you?"],
             batch_size=2
         )
 
     """
 
-    aclient: Any  # Since the OpenAI module is loaded dynamically
+    _client: Any = PrivateAttr()
+    _aclient: Any = PrivateAttr()
 
     def __init__(
         self, model: str = "text-embedding-ada-002", api_config: Optional[Dict] = None
     ):
         """Initialize the OpenAI vectorizer.
 
         Args:
@@ -55,14 +57,22 @@
             api_config (Optional[Dict], optional): Dictionary containing the
                 API key. Defaults to None.
 
         Raises:
             ImportError: If the openai library is not installed.
             ValueError: If the OpenAI API key is not provided.
         """
+        self._initialize_clients(api_config)
+        super().__init__(model=model, dims=self._set_model_dims(model))
+
+    def _initialize_clients(self, api_config: Optional[Dict]):
+        """
+        Setup the OpenAI clients using the provided API key or an
+        environment variable.
+        """
         # Dynamic import of the openai module
         try:
             from openai import AsyncOpenAI, OpenAI
         except ImportError:
             raise ImportError(
                 "OpenAI vectorizer requires the openai library. \
                     Please install with `pip install openai`"
@@ -75,24 +85,21 @@
         if not api_key:
             raise ValueError(
                 "OpenAI API key is required. "
                 "Provide it in api_config or set the OPENAI_API_KEY\
                     environment variable."
             )
 
-        client = OpenAI(api_key=api_key)
-        dims = self._set_model_dims(client, model)
-        super().__init__(model=model, dims=dims, client=client)
-        self.aclient = AsyncOpenAI(api_key=api_key)
+        self._client = OpenAI(api_key=api_key)
+        self._aclient = AsyncOpenAI(api_key=api_key)
 
-    @staticmethod
-    def _set_model_dims(client, model) -> int:
+    def _set_model_dims(self, model) -> int:
         try:
             embedding = (
-                client.embeddings.create(input=["dimension test"], model=model)
+                self._client.embeddings.create(input=["dimension test"], model=model)
                 .data[0]
                 .embedding
             )
         except (KeyError, IndexError) as ke:
             raise ValueError(f"Unexpected response from the OpenAI API: {str(ke)}")
         except Exception as e:  # pylint: disable=broad-except
             # fall back (TODO get more specific)
@@ -132,15 +139,15 @@
         if not isinstance(texts, list):
             raise TypeError("Must pass in a list of str values to embed.")
         if len(texts) > 0 and not isinstance(texts[0], str):
             raise TypeError("Must pass in a list of str values to embed.")
 
         embeddings: List = []
         for batch in self.batchify(texts, batch_size, preprocess):
-            response = self.client.embeddings.create(input=batch, model=self.model)
+            response = self._client.embeddings.create(input=batch, model=self.model)
             embeddings += [
                 self._process_embedding(r.embedding, as_buffer) for r in response.data
             ]
         return embeddings
 
     @retry(
         wait=wait_random_exponential(min=1, max=60),
@@ -170,15 +177,15 @@
             TypeError: If the wrong input type is passed in for the test.
         """
         if not isinstance(text, str):
             raise TypeError("Must pass in a str value to embed.")
 
         if preprocess:
             text = preprocess(text)
-        result = self.client.embeddings.create(input=[text], model=self.model)
+        result = self._client.embeddings.create(input=[text], model=self.model)
         return self._process_embedding(result.data[0].embedding, as_buffer)
 
     @retry(
         wait=wait_random_exponential(min=1, max=60),
         stop=stop_after_attempt(6),
         retry=retry_if_not_exception_type(TypeError),
     )
@@ -210,15 +217,15 @@
         if not isinstance(texts, list):
             raise TypeError("Must pass in a list of str values to embed.")
         if len(texts) > 0 and not isinstance(texts[0], str):
             raise TypeError("Must pass in a list of str values to embed.")
 
         embeddings: List = []
         for batch in self.batchify(texts, batch_size, preprocess):
-            response = await self.aclient.embeddings.create(
+            response = await self._aclient.embeddings.create(
                 input=batch, model=self.model
             )
             embeddings += [
                 self._process_embedding(r.embedding, as_buffer) for r in response.data
             ]
         return embeddings
 
@@ -250,9 +257,9 @@
             TypeError: If the wrong input type is passed in for the test.
         """
         if not isinstance(text, str):
             raise TypeError("Must pass in a str value to embed.")
 
         if preprocess:
             text = preprocess(text)
-        result = await self.aclient.embeddings.create(input=[text], model=self.model)
+        result = await self._aclient.embeddings.create(input=[text], model=self.model)
         return self._process_embedding(result.data[0].embedding, as_buffer)
```

### Comparing `redisvl-0.1.3/redisvl/utils/vectorize/text/vertexai.py` & `redisvl-0.2.0/redisvl/utils/vectorize/text/vertexai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
-from typing import Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 
+from pydantic.v1 import PrivateAttr
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from tenacity.retry import retry_if_not_exception_type
 
 from redisvl.utils.vectorize.base import BaseVectorizer
 
 
 class VertexAITextVectorizer(BaseVectorizer):
@@ -36,14 +37,16 @@
         embeddings = await vectorizer.embed_many(
             ["Hello, world!", "Goodbye, world!"],
             batch_size=2
         )
 
     """
 
+    _client: Any = PrivateAttr()
+
     def __init__(
         self, model: str = "textembedding-gecko", api_config: Optional[Dict] = None
     ):
         """Initialize the VertexAI vectorizer.
 
         Args:
             model (str): Model to use for embedding. Defaults to
@@ -51,14 +54,22 @@
             api_config (Optional[Dict], optional): Dictionary containing the
                 API config details. Defaults to None.
 
         Raises:
             ImportError: If the google-cloud-aiplatform library is not installed.
             ValueError: If the API key is not provided.
         """
+        self._initialize_client(model, api_config)
+        super().__init__(model=model, dims=self._set_model_dims())
+
+    def _initialize_client(self, model: str, api_config: Optional[Dict]):
+        """
+        Setup the VertexAI clients using the provided API key or an
+        environment variable.
+        """
         # Fetch the project_id and location from api_config or environment variables
         project_id = (
             api_config.get("project_id") if api_config else os.getenv("GCP_PROJECT_ID")
         )
         location = (
             api_config.get("location") if api_config else os.getenv("GCP_LOCATION")
         )
@@ -89,22 +100,19 @@
             )
         except ImportError:
             raise ImportError(
                 "VertexAI vectorizer requires the google-cloud-aiplatform library. "
                 "Please install with `pip install google-cloud-aiplatform>=1.26`"
             )
 
-        client = TextEmbeddingModel.from_pretrained(model)
-        dims = self._set_model_dims(client)
-        super().__init__(model=model, dims=dims, client=client)
+        self._client = TextEmbeddingModel.from_pretrained(model)
 
-    @staticmethod
-    def _set_model_dims(client) -> int:
+    def _set_model_dims(self) -> int:
         try:
-            embedding = client.get_embeddings(["dimension test"])[0].values
+            embedding = self._client.get_embeddings(["dimension test"])[0].values
         except (KeyError, IndexError) as ke:
             raise ValueError(f"Unexpected response from the VertexAI API: {str(ke)}")
         except Exception as e:  # pylint: disable=broad-except
             # fall back (TODO get more specific)
             raise ValueError(f"Error setting embedding model dimensions: {str(e)}")
         return len(embedding)
 
@@ -141,15 +149,15 @@
         if not isinstance(texts, list):
             raise TypeError("Must pass in a list of str values to embed.")
         if len(texts) > 0 and not isinstance(texts[0], str):
             raise TypeError("Must pass in a list of str values to embed.")
 
         embeddings: List = []
         for batch in self.batchify(texts, batch_size, preprocess):
-            response = self.client.get_embeddings(batch)
+            response = self._client.get_embeddings(batch)
             embeddings += [
                 self._process_embedding(r.values, as_buffer) for r in response
             ]
         return embeddings
 
     @retry(
         wait=wait_random_exponential(min=1, max=60),
@@ -179,9 +187,28 @@
             TypeError: If the wrong input type is passed in for the test.
         """
         if not isinstance(text, str):
             raise TypeError("Must pass in a str value to embed.")
 
         if preprocess:
             text = preprocess(text)
-        result = self.client.get_embeddings([text])
+        result = self._client.get_embeddings([text])
         return self._process_embedding(result[0].values, as_buffer)
+
+    async def aembed_many(
+        self,
+        texts: List[str],
+        preprocess: Optional[Callable] = None,
+        batch_size: int = 1000,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[List[float]]:
+        raise NotImplementedError
+
+    async def aembed(
+        self,
+        text: str,
+        preprocess: Optional[Callable] = None,
+        as_buffer: bool = False,
+        **kwargs,
+    ) -> List[float]:
+        raise NotImplementedError
```

