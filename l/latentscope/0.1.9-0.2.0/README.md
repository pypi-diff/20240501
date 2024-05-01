# Comparing `tmp/latentscope-0.1.9.tar.gz` & `tmp/latentscope-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentscope-0.1.9.tar", last modified: Fri Mar 29 13:49:14 2024, max compression
+gzip compressed data, was "latentscope-0.2.0.tar", last modified: Wed May  1 21:55:19 2024, max compression
```

## Comparing `latentscope-0.1.9.tar` & `latentscope-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.280872 latentscope-0.1.9/
--rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.1.9/LICENSE
--rw-r--r--   0 enjalot    (501) staff       (20)    19886 2024-03-29 13:49:14.280647 latentscope-0.1.9/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)    13982 2024-02-28 15:27:45.000000 latentscope-0.1.9/README.md
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.272616 latentscope-0.1.9/latentscope/
--rw-r--r--   0 enjalot    (501) staff       (20)     1995 2024-03-19 19:16:01.000000 latentscope-0.1.9/latentscope/__init__.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.273662 latentscope-0.1.9/latentscope/models/
--rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.1.9/latentscope/models/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.1.9/latentscope/models/chat_models.json
--rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.1.9/latentscope/models/embedding_models.json
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.274732 latentscope-0.1.9/latentscope/models/providers/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.1.9/latentscope/models/providers/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.1.9/latentscope/models/providers/base.py
--rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.1.9/latentscope/models/providers/cohereai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.1.9/latentscope/models/providers/mistralai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.1.9/latentscope/models/providers/nltk.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.1.9/latentscope/models/providers/openai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.1.9/latentscope/models/providers/togetherai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.1.9/latentscope/models/providers/transformers.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.1.9/latentscope/models/providers/voyageai.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.275727 latentscope-0.1.9/latentscope/scripts/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.1.9/latentscope/scripts/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.1.9/latentscope/scripts/cluster-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.1.9/latentscope/scripts/cluster.py
--rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.1.9/latentscope/scripts/embed.py
--rw-r--r--   0 enjalot    (501) staff       (20)     5445 2024-03-20 19:01:04.000000 latentscope-0.1.9/latentscope/scripts/ingest.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.1.9/latentscope/scripts/label_clusters.py
--rw-r--r--   0 enjalot    (501) staff       (20)     4370 2024-03-19 19:15:07.000000 latentscope-0.1.9/latentscope/scripts/scope.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.1.9/latentscope/scripts/umapper-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.1.9/latentscope/scripts/umapper.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.276430 latentscope-0.1.9/latentscope/server/
--rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.1.9/latentscope/server/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7299 2024-03-23 01:39:57.000000 latentscope-0.1.9/latentscope/server/app.py
--rw-r--r--   0 enjalot    (501) staff       (20)     9249 2024-03-20 19:09:45.000000 latentscope-0.1.9/latentscope/server/datasets.py
--rw-r--r--   0 enjalot    (501) staff       (20)    12640 2024-03-20 19:31:26.000000 latentscope-0.1.9/latentscope/server/jobs.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.1.9/latentscope/server/search.py
--rw-r--r--   0 enjalot    (501) staff       (20)     4405 2024-02-09 20:02:07.000000 latentscope-0.1.9/latentscope/server/tags.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.276762 latentscope-0.1.9/latentscope/util/
--rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.1.9/latentscope/util/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.1.9/latentscope/util/configuration.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-03-29 13:49:14.273314 latentscope-0.1.9/latentscope.egg-info/
--rw-r--r--   0 enjalot    (501) staff       (20)    19886 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)     1258 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/SOURCES.txt
--rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/dependency_links.txt
--rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/entry_points.txt
--rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/requires.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-03-29 13:49:14.000000 latentscope-0.1.9/latentscope.egg-info/top_level.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-03-29 13:49:14.280926 latentscope-0.1.9/setup.cfg
--rw-r--r--   0 enjalot    (501) staff       (20)     3282 2024-03-29 13:49:01.000000 latentscope-0.1.9/setup.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.358158 latentscope-0.2.0/
+-rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.0/LICENSE
+-rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-01 21:55:19.357919 latentscope-0.2.0/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)    12893 2024-05-01 21:43:52.000000 latentscope-0.2.0/README.md
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.349647 latentscope-0.2.0/latentscope/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/__version__.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.350807 latentscope-0.2.0/latentscope/models/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.0/latentscope/models/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.0/latentscope/models/chat_models.json
+-rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.0/latentscope/models/embedding_models.json
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.351907 latentscope-0.2.0/latentscope/models/providers/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.0/latentscope/models/providers/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.0/latentscope/models/providers/base.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.0/latentscope/models/providers/cohereai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.0/latentscope/models/providers/mistralai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.0/latentscope/models/providers/nltk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.0/latentscope/models/providers/openai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.0/latentscope/models/providers/togetherai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.0/latentscope/models/providers/transformers.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.0/latentscope/models/providers/voyageai.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.352945 latentscope-0.2.0/latentscope/scripts/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.0/latentscope/scripts/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.0/latentscope/scripts/cluster-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.0/latentscope/scripts/cluster.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.0/latentscope/scripts/embed.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/scripts/ingest.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.0/latentscope/scripts/label_clusters.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     5930 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/scripts/scope.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.0/latentscope/scripts/umapper-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.0/latentscope/scripts/umapper.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.353780 latentscope-0.2.0/latentscope/server/
+-rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.0/latentscope/server/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.0/latentscope/server/app.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     5099 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/bulk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/datasets.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    13747 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/jobs.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.0/latentscope/server/search.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/tags.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.354036 latentscope-0.2.0/latentscope/util/
+-rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.0/latentscope/util/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.0/latentscope/util/configuration.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.350399 latentscope-0.2.0/latentscope.egg-info/
+-rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/entry_points.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/requires.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/top_level.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-01 21:55:19.358234 latentscope-0.2.0/setup.cfg
+-rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.0/setup.py
```

### Comparing `latentscope-0.1.9/LICENSE` & `latentscope-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/PKG-INFO` & `latentscope-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
@@ -178,48 +178,51 @@
 Requires-Dist: zipp==3.17.0
 
 # Latent Scope
 [![](https://dcbadge.vercel.app/api/server/x7NvpnM4pY?style=flat)](https://discord.gg/x7NvpnM4pY)
 [![PyPI version](https://img.shields.io/pypi/v/latentscope.svg)](https://pypi.org/project/latentscope/)
 
 Quickly embed, project, cluster and explore a dataset. This project is a new kind of workflow + tool for visualizing and exploring datasets through the lens of latent spaces. 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-explore.png?raw=true" height="480px"  alt="Example exploration">](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-007)
+
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/end.png?raw=true" width="45%"  alt="Setup your scope"><img src="https://github.com/enjalot/latent-scope/blob/main/documentation/curate-combined-cluster.png?raw=true" width="45%"  alt="Explore and Curate your data">
 
 The power of machine learning models to encode unstructured data into high-dimensional embeddings is relatively under-explored. Retrieval Augmented Generation has taken off as a popular usecase for embeddings, but do you feel confident in your understanding of why certain data is being retrieved? Do you have a clear picture of what all is in your dataset? Latentscope is like a microscope that allows you to get a new perspective on what's happening to your data when it's embedded. You can try similarity search with different embeddings, peruse automatically labeled clusters and zoom in on individual data points all while keeping the context of your entire dataset. 
 
-### Demo
-This tool is meant to be run locally or on a trusted server to process data for viewing in the latent scope. You can see the result of the process in a read-only [live demo](https://enjalot.github.io/latent-scope):
-* [datavis survey responses](https://enjalot.github.io/latent-scope/#/datasets/datavis-misunderstood/explore/scopes-001) - 700 survey responses
-* [Dolly 15k](https://enjalot.github.io/latent-scope/#/datasets/dolly15k/explore/scopes-001) - 15k instructions
-* [r/DadJokes](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) - 50k dad jokes
-* [emotion](https://enjalot.github.io/latent-scope/#/datasets/emotion/explore/scopes-001) - 400k emotion statements from Twitter
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/process-crop.png?raw=true"  alt="Setup your scope">
 
-The source of each demo dataset is documented in the notebooks linked below. Each demo was chosen to represent different scales of data as well as some common usecases.
+Latent Scope is a tool that encodes a process, taking your input data and running it through the steps of Embedding, Projecting, Clustering and Labeling resulting in a nicely structured annotation useful as input to further analysis. You can also explore the annotated data within the web UI to get a better understanding of your dataset and curate it to get a better quality dataset.
 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-scopes.png?raw=true" width="100%"  alt="Dadabase demo scopes">](https://enjalot.github.io/latent-scope)
+## Getting started
+Follow the documentation guides to get started:
+1. [Install and Configure](https://enjalot.github.io/latent-scope/install-and-config)
+2. [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope)
+3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
+4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
+
+## Example Analysis
+What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
+* Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
+* Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
+* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install latentscope
 ls-init ~/local-scope-data --openai_key=XXX --mistral_key=YYY # optional api keys to enable API models 
 ls-serve 
 ```
 
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
-<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/home.png?raw=true" width="320px"  alt="Ingest">  <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/0-ingest.png?raw=true" width="320px"  alt="Ingest">
-
-Once ingested, you will go through the following 6 steps: Embed, UMAP, Cluster, Label, Scope and Explore 
- <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/1-embed.png?raw=true" width="320px"  alt="Embed"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/2-umap.png?raw=true" width="320px"  alt="UMAP"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/3-cluster.png?raw=true" width="320px"  alt="Cluster"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/4-label.png?raw=true" width="320px"  alt="Label"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/5-scope.png?raw=true" width="320px"  alt="Scope"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/6-explore.png?raw=true" width="320px"  alt="Scope">
 
-Each step focuses on the relevant choices to move you to the next step. For example choosing which embedding model you want to use to embed with, or the parameters for UMAP. It's very likely you may want to try several choices at each step, which is why the final step before "Explore" is to make a "scope". You can make multiple scopes, as seen in the [dadabase example](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) to explore your data through different lenses (i.e. OpenAI embeddings vs. Jina v2).
+See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
 from latentscope import ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
```

### Comparing `latentscope-0.1.9/README.md` & `latentscope-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # Latent Scope
 [![](https://dcbadge.vercel.app/api/server/x7NvpnM4pY?style=flat)](https://discord.gg/x7NvpnM4pY)
 [![PyPI version](https://img.shields.io/pypi/v/latentscope.svg)](https://pypi.org/project/latentscope/)
 
 Quickly embed, project, cluster and explore a dataset. This project is a new kind of workflow + tool for visualizing and exploring datasets through the lens of latent spaces. 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-explore.png?raw=true" height="480px"  alt="Example exploration">](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-007)
+
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/end.png?raw=true" width="45%"  alt="Setup your scope"><img src="https://github.com/enjalot/latent-scope/blob/main/documentation/curate-combined-cluster.png?raw=true" width="45%"  alt="Explore and Curate your data">
 
 The power of machine learning models to encode unstructured data into high-dimensional embeddings is relatively under-explored. Retrieval Augmented Generation has taken off as a popular usecase for embeddings, but do you feel confident in your understanding of why certain data is being retrieved? Do you have a clear picture of what all is in your dataset? Latentscope is like a microscope that allows you to get a new perspective on what's happening to your data when it's embedded. You can try similarity search with different embeddings, peruse automatically labeled clusters and zoom in on individual data points all while keeping the context of your entire dataset. 
 
-### Demo
-This tool is meant to be run locally or on a trusted server to process data for viewing in the latent scope. You can see the result of the process in a read-only [live demo](https://enjalot.github.io/latent-scope):
-* [datavis survey responses](https://enjalot.github.io/latent-scope/#/datasets/datavis-misunderstood/explore/scopes-001) - 700 survey responses
-* [Dolly 15k](https://enjalot.github.io/latent-scope/#/datasets/dolly15k/explore/scopes-001) - 15k instructions
-* [r/DadJokes](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) - 50k dad jokes
-* [emotion](https://enjalot.github.io/latent-scope/#/datasets/emotion/explore/scopes-001) - 400k emotion statements from Twitter
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/process-crop.png?raw=true"  alt="Setup your scope">
 
-The source of each demo dataset is documented in the notebooks linked below. Each demo was chosen to represent different scales of data as well as some common usecases.
+Latent Scope is a tool that encodes a process, taking your input data and running it through the steps of Embedding, Projecting, Clustering and Labeling resulting in a nicely structured annotation useful as input to further analysis. You can also explore the annotated data within the web UI to get a better understanding of your dataset and curate it to get a better quality dataset.
 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-scopes.png?raw=true" width="100%"  alt="Dadabase demo scopes">](https://enjalot.github.io/latent-scope)
+## Getting started
+Follow the documentation guides to get started:
+1. [Install and Configure](https://enjalot.github.io/latent-scope/install-and-config)
+2. [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope)
+3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
+4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
+
+## Example Analysis
+What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
+* Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
+* Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
+* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install latentscope
 ls-init ~/local-scope-data --openai_key=XXX --mistral_key=YYY # optional api keys to enable API models 
 ls-serve 
 ```
 
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
-<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/home.png?raw=true" width="320px"  alt="Ingest">  <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/0-ingest.png?raw=true" width="320px"  alt="Ingest">
-
-Once ingested, you will go through the following 6 steps: Embed, UMAP, Cluster, Label, Scope and Explore 
- <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/1-embed.png?raw=true" width="320px"  alt="Embed"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/2-umap.png?raw=true" width="320px"  alt="UMAP"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/3-cluster.png?raw=true" width="320px"  alt="Cluster"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/4-label.png?raw=true" width="320px"  alt="Label"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/5-scope.png?raw=true" width="320px"  alt="Scope"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/6-explore.png?raw=true" width="320px"  alt="Scope">
 
-Each step focuses on the relevant choices to move you to the next step. For example choosing which embedding model you want to use to embed with, or the parameters for UMAP. It's very likely you may want to try several choices at each step, which is why the final step before "Explore" is to make a "scope". You can make multiple scopes, as seen in the [dadabase example](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) to explore your data through different lenses (i.e. OpenAI embeddings vs. Jina v2).
+See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
 from latentscope import ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
```

### Comparing `latentscope-0.1.9/latentscope/__init__.py` & `latentscope-0.2.0/latentscope/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .__version__ import __version__
 from . import models
 from .scripts.ingest import ingest
 from .scripts.embed import embed
 from .scripts.embed import import_embeddings
 from .scripts.umapper import umapper as umap
 from .scripts.cluster import clusterer as cluster
 from .scripts.label_clusters import labeler as label
```

### Comparing `latentscope-0.1.9/latentscope/models/__init__.py` & `latentscope-0.2.0/latentscope/models/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/chat_models.json` & `latentscope-0.2.0/latentscope/models/chat_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/embedding_models.json` & `latentscope-0.2.0/latentscope/models/embedding_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/base.py` & `latentscope-0.2.0/latentscope/models/providers/base.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/cohereai.py` & `latentscope-0.2.0/latentscope/models/providers/cohereai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/mistralai.py` & `latentscope-0.2.0/latentscope/models/providers/mistralai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/nltk.py` & `latentscope-0.2.0/latentscope/models/providers/nltk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/openai.py` & `latentscope-0.2.0/latentscope/models/providers/openai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/togetherai.py` & `latentscope-0.2.0/latentscope/models/providers/togetherai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/transformers.py` & `latentscope-0.2.0/latentscope/models/providers/transformers.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/models/providers/voyageai.py` & `latentscope-0.2.0/latentscope/models/providers/voyageai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/cluster-1d.py` & `latentscope-0.2.0/latentscope/scripts/cluster-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/cluster.py` & `latentscope-0.2.0/latentscope/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/embed.py` & `latentscope-0.2.0/latentscope/scripts/embed.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/ingest.py` & `latentscope-0.2.0/latentscope/scripts/ingest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Usage: ls-ingest <dataset_id>
 import os
 import json
 import argparse
 
 from latentscope.util import get_data_dir
+from latentscope import __version__
 
 # TODO make a parquet version of these
 def main():
     parser = argparse.ArgumentParser(description='Ingest a dataset')
     parser.add_argument('id', type=str, help='Dataset id (directory name in data folder)')
     parser.add_argument('--path', type=str, help='Path to csv or parquet file, otherwise assumes input.csv in dataset directory')
+    parser.add_argument('--text_column', type=str, help='Column to use as text for the scope')
     args = parser.parse_args()
-    ingest_file(args.id, args.path)
+    ingest_file(args.id, args.path, args.text_column)
 
-def ingest_file(dataset_id, file_path):
+def ingest_file(dataset_id, file_path, text_column = None):
     import pandas as pd
     DATA_DIR = get_data_dir()
     directory = os.path.join(DATA_DIR, dataset_id)
     # check if dataset exists, if it does we want to increment a postfix on the dataset_id
     # if os.path.exists(directory):
     #     postfix = 1
     #     while os.path.exists(f"{directory}-{postfix:03d}"):
@@ -40,15 +42,15 @@
     elif file_type == "jsonl":
         with open(file, 'r') as f:
             lines = f.readlines()
             df = pd.DataFrame([json.loads(line) for line in lines])
     else:
         raise ValueError(f"Unsupported file type: {file_type}")
 
-    ingest(dataset_id, df)
+    ingest(dataset_id, df, text_column)
 
 
 def ingest(dataset_id, df, text_column = None):
 
 
     DATA_DIR = get_data_dir()
     print("DATA DIR", DATA_DIR)
@@ -87,27 +89,41 @@
         elif isinstance(non_null_series.iloc[0], np.ndarray):
             print("np array", column)
             column_type = "array"
         else:
             column_type = "unknown"
 
         # Count unique values, excluding NaN
-        if isinstance(df[column].iloc[0], np.ndarray):
-            unique_values_count = len(set([tuple(x) for x in df[column].dropna()]))
-        else:
-            unique_values_count = df[column].nunique(dropna=True)
+        try:
+            if isinstance(df[column].iloc[0], np.ndarray):
+                unique_values_count = len(set([tuple(x) for x in df[column].dropna()]))
+            elif isinstance(df[column].iloc[0], bytes):
+                unique_values_count = len(set(df[column].dropna().apply(lambda x: x.decode('utf-8'))))
+            elif isinstance(df[column].iloc[0], dict):
+                unique_values_count = len(set(df[column].dropna().apply(json.dumps)))
+            else:
+                unique_values_count = df[column].nunique(dropna=True)
+        except:
+            unique_values_count = -1
 
         # Store the metadata
         column_metadata[column] = {
             "type": column_type,
             "unique_values_count": unique_values_count
         }
         if column_type == "string" and unique_values_count <= 20:
             categories = df[column].value_counts().index.tolist()
             column_metadata[column]["categories"] = categories
+            column_metadata[column]["counts"] = df[column].value_counts().to_dict()
+        if column_type == "string":
+            if df[column].str.startswith("http").all():
+                column_metadata[column]["url"] = True
+                # check if endings of string are common image formats like png, jpg, jpeg, webp
+                if df[column].str.lower().str.endswith(("png", "jpg", "jpeg", "webp", "svg", "gif")).all():
+                    column_metadata[column]["image"] = True
         if column_type == "number":
             extent = df[column].agg(['min', 'max'])
             column_metadata[column]["extent"] = extent.tolist()
         if column_type == "date":
             extent = df[column].agg(['min', 'max'])
             column_metadata[column]["extent"] = extent.tolist()
 
@@ -122,20 +138,29 @@
     with open(os.path.join(directory,'meta.json'), 'w') as f:
         json.dump({
             "id": dataset_id,
             "length": df.shape[0],
             "columns": df.columns.tolist(),
             "text_column": text_column,
             "column_metadata": column_metadata,
-            "potential_embeddings": potential_embeddings
+            "potential_embeddings": potential_embeddings,
+            "ls_version": __version__
             }, f, indent=2)
 
     # create all the directories we will use
-    os.makedirs(os.path.join(DATA_DIR, dataset_id, "tags"), exist_ok=True)
     os.makedirs(os.path.join(DATA_DIR, dataset_id, "embeddings"), exist_ok=True)
     os.makedirs(os.path.join(DATA_DIR, dataset_id, "umaps"), exist_ok=True)
     os.makedirs(os.path.join(DATA_DIR, dataset_id, "clusters"), exist_ok=True)
     os.makedirs(os.path.join(DATA_DIR, dataset_id, "scopes"), exist_ok=True)
+    tags_dir = os.path.join(DATA_DIR, dataset_id, "tags")
+    os.makedirs(tags_dir, exist_ok=True)
+    # Create default tags if they don't exist
+    new_files = ['👍.indices', '👎.indices']
+    for file_name in new_files:
+        file_path = os.path.join(tags_dir, file_name)
+        if not os.path.exists(file_path):
+            with open(file_path, 'w') as file:
+                file.write('')  # Initialize with an empty JSON object
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `latentscope-0.1.9/latentscope/scripts/label_clusters.py` & `latentscope-0.2.0/latentscope/scripts/label_clusters.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/scope.py` & `latentscope-0.2.0/latentscope/scripts/scope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import re
 import json
 import argparse
+from datetime import datetime
 from latentscope.util import get_data_dir
+from latentscope import __version__
 
 
 def main():
     parser = argparse.ArgumentParser(description='Setup a scope')
     parser.add_argument('dataset_id', type=str, help='Dataset id (directory name in data folder)')
     parser.add_argument('embedding_id', type=str, help='Embedding id')
     parser.add_argument('umap_id', type=str, help='UMAP id')
@@ -43,24 +45,30 @@
         id = scope_id
 
     print("RUNNING:", id)
 
     import pandas as pd
 
     scope = {
+        "ls_version": __version__,
         "id": id,
         "embedding_id": embedding_id,
         "umap_id": umap_id,
         "cluster_id": cluster_id,
         "cluster_labels_id": cluster_labels_id,
         "label": label,
         "description": description
     }
 
     # read each json file and add its contents to the scope file
+    dataset_file = os.path.join(DATA_DIR, dataset_id, "meta.json")
+    with open(dataset_file) as f:
+        dataset = json.load(f)
+        scope["dataset"] = dataset
+
     embedding_file = os.path.join(DATA_DIR, dataset_id, "embeddings", embedding_id + ".json")
     with open(embedding_file) as f:
         embedding = json.load(f)
         scope["embedding"] = embedding
     
     umap_file = os.path.join(DATA_DIR, dataset_id, "umaps", umap_id + ".json")
     with open(umap_file) as f:
@@ -76,26 +84,49 @@
         cluster_labels_id = cluster_id + "-labels-default"
         scope["cluster_labels"] = {"id": cluster_labels_id, "cluster_id": cluster_id}
     else:
         cluster_labels_file = os.path.join(DATA_DIR, dataset_id, "clusters", cluster_labels_id + ".json")
         with open(cluster_labels_file) as f:
             cluster_labels = json.load(f)
             scope["cluster_labels"] = cluster_labels
+
+    # load the actual labels and save everything but the indices in a dict
+    cluster_labels_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "clusters", cluster_labels_id + ".parquet"))
+    # remove the indices column
+
+    cluster_labels_df = cluster_labels_df.drop(columns=[col for col in ["indices", "labeled", "label_raw"] if col in cluster_labels_df.columns])
+    # cluster_labels_df = cluster_labels_df.drop(columns=["indices", "labeled", "label_raw"])
+    # change hulls to a list of lists
+    cluster_labels_df["hull"] = cluster_labels_df["hull"].apply(lambda x: x.tolist())
+    cluster_labels_df["cluster"] = cluster_labels_df.index
+    scope["cluster_labels_lookup"] = cluster_labels_df.to_dict(orient="records")
     
     # create a scope parquet by combining the parquets from umap and cluster, as well as getting the labels from cluster_labels
     # then write the parquet to the scopes directory
     umap_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "umaps", umap_id + ".parquet"))
+    print("umap columns", umap_df.columns)
     cluster_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "clusters", cluster_id + ".parquet"))
     cluster_labels_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "clusters", cluster_labels_id + ".parquet"))
     # create a column where we lookup the label from cluster_labels_df for the index found in the cluster_df
     cluster_df["label"] = cluster_df["cluster"].apply(lambda x: cluster_labels_df.loc[x]["label"])
+    print("cluster columns", cluster_df.columns)
     scope_parquet = pd.concat([umap_df, cluster_df], axis=1)
+    # Add an ls_index column that is the index of each row in the dataframe
+    scope_parquet['ls_index'] = scope_parquet.index
+    print("scope columns", scope_parquet.columns)
     scope_parquet.to_parquet(os.path.join(directory, id + ".parquet"))
 
     scope["rows"] = len(scope_parquet)
     scope["columns"] = scope_parquet.columns.tolist()
     scope["size"] = os.path.getsize(os.path.join(directory, id + ".parquet"))
+    scope["timestamp"] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     
     file_path = os.path.join(directory, id + ".json")
     with open(file_path, 'w') as f:
         json.dump(scope, f, indent=2)
+    
+    transactions_file_path = os.path.join(directory, id + "-transactions.json")
+    if not os.path.exists(transactions_file_path):
+        with open(transactions_file_path, 'w') as f:
+            json.dump([], f)
+
     print("wrote scope", id)
```

### Comparing `latentscope-0.1.9/latentscope/scripts/umapper-1d.py` & `latentscope-0.2.0/latentscope/scripts/umapper-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/scripts/umapper.py` & `latentscope-0.2.0/latentscope/scripts/umapper.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/server/__init__.py` & `latentscope-0.2.0/latentscope/server/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/server/app.py` & `latentscope-0.2.0/latentscope/server/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import os
 import sys
 import json
+import math
 import logging
 import argparse
 import pandas as pd
 import pkg_resources
 from dotenv import dotenv_values, set_key
 from flask import Flask, request, jsonify, send_from_directory
 from flask_cors import CORS
@@ -52,14 +53,18 @@
     app.register_blueprint(tags_write_bp, url_prefix='/api/tags') 
 
 from .datasets import datasets_bp, datasets_write_bp
 app.register_blueprint(datasets_bp, url_prefix='/api/datasets')
 if(not READ_ONLY):
     app.register_blueprint(datasets_write_bp, url_prefix='/api/datasets')
 
+from .bulk import bulk_bp, bulk_write_bp
+app.register_blueprint(bulk_bp, url_prefix='/api/bulk') 
+if(not READ_ONLY):
+    app.register_blueprint(bulk_write_bp, url_prefix='/api/bulk') 
 
 
 # ===========================================================
 # File based routes for reading data and metadata from disk
 # ===========================================================
 @app.route('/api/embedding_models', methods=['GET'])
 def get_embedding_models():
@@ -100,32 +105,29 @@
     
     # get the indexed rows
     rows = df.iloc[indices]
 
     # send back the rows as json
     return rows.to_json(orient="records")
 
-@app.route('/api/query', methods=['POST'])
-def query():
-    per_page = 100
+@app.route('/api/column-filter', methods=['POST'])
+def column_filter():
     data = request.get_json()
     dataset = data['dataset']
-    page = data['page'] if 'page' in data else 0
-    indices = data['indices'] if 'indices' in data else []
-    filters = data['filters'] if 'filters' in data else None
-    sort = data['sort'] if 'sort' in data else None
+    filters = data['filters']
+
     if dataset not in DATAFRAMES:
         df = pd.read_parquet(os.path.join(DATA_DIR, dataset, "input.parquet"))
         DATAFRAMES[dataset] = df
     else:
         df = DATAFRAMES[dataset]
     
     # apply filters
     rows = df.copy()
-    rows['ls_index'] = rows.index
+
     print("FILTERS", filters)
     if filters:
         for f in filters:
             if f["type"] == "eq":
                 rows = rows[rows[f['column']] == f['value']]
             elif f["type"] == "gt":
                 rows = rows[rows[f['column']] > f['value']]
@@ -136,35 +138,57 @@
             elif f["type"] == "lte":
                 rows = rows[rows[f['column']] <= f['value']]
             elif f["type"] == "in":
                 rows = rows[rows[f['column']].isin(f['value'])]
             elif f["type"] == "contains":
                 rows = rows[rows[f['column']].str.contains(f['value'])]
 
+    return jsonify(indices=rows.index.to_list())
+
+@app.route('/api/query', methods=['POST'])
+def query():
+    per_page = 100
+    data = request.get_json()
+    dataset = data['dataset']
+    page = data['page'] if 'page' in data else 0
+    indices = data['indices'] if 'indices' in data else []
+    # filters = data['filters'] if 'filters' in data else None
+    sort = data['sort'] if 'sort' in data else None
+    if dataset not in DATAFRAMES:
+        df = pd.read_parquet(os.path.join(DATA_DIR, dataset, "input.parquet"))
+        DATAFRAMES[dataset] = df
+    else:
+        df = DATAFRAMES[dataset]
+    
+    # apply filters
+    rows = df.copy()
+    rows['ls_index'] = rows.index
+    
+
     # get the indexed rows
     print("INDICES", indices)
     if len(indices):
         rows = rows.loc[indices]
 
     print("ROWS", rows.head())
     # apply sort
     if sort:
         rows = rows.sort_values(by=sort['column'], ascending=sort['ascending'])
 
     # Convert DataFrame to a list of dictionaries
     rows_json = json.loads(rows[page*per_page:page*per_page+per_page].to_json(orient="records"))
-    print("ROWS JSON", rows_json)
+    # print("ROWS JSON", rows_json)
 
     # send back the rows as json
     return jsonify({
         "rows": rows_json,
         "page": page,
         "per_page": per_page,
         "total": len(rows),
-        "totalPages": len(rows) // per_page
+        "totalPages": math.ceil(len(rows) / per_page)
     })
 
 if not READ_ONLY:
     @app.route('/api/settings', methods=['POST'])
     def update_settings():
         data = request.get_json()
         print("update settings", data)
```

### Comparing `latentscope-0.1.9/latentscope/server/datasets.py` & `latentscope-0.2.0/latentscope/server/datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -134,36 +134,37 @@
     #     return get_dataset_cluster_labels_default(dataset, cluster)
     file_name = cluster + "-labels-" + id + ".parquet"
     file_path = os.path.join(DATA_DIR, dataset, "clusters", file_name)
     df = pd.read_parquet(file_path)
     df.reset_index(inplace=True)
     return df.to_json(orient="records")
 
-@datasets_write_bp.route('/<dataset>/clusters/<cluster>/labels/<id>/label/<index>', methods=['GET'])
-def overwrite_dataset_cluster_label(dataset, cluster, id, index):
-    index = int(index)
-    new_label = request.args.get('label')
-    print("write label", index, new_label)
-    if new_label is None:
-        return jsonify({"error": "Missing 'label' in request data"}), 400
-
-    file_name = cluster + "-labels-" + id + ".parquet"
-    file_path = os.path.join(DATA_DIR, dataset, "clusters", file_name)
-    try:
-        df = pd.read_parquet(file_path)
-    except FileNotFoundError:
-        return jsonify({"error": "File not found"}), 404
+# This was rewritten in bulk.py to only affect a scope
+# @datasets_write_bp.route('/<dataset>/clusters/<cluster>/labels/<id>/label/<index>', methods=['GET'])
+# def overwrite_dataset_cluster_label(dataset, cluster, id, index):
+#     index = int(index)
+#     new_label = request.args.get('label')
+#     print("write label", index, new_label)
+#     if new_label is None:
+#         return jsonify({"error": "Missing 'label' in request data"}), 400
+
+#     file_name = cluster + "-labels-" + id + ".parquet"
+#     file_path = os.path.join(DATA_DIR, dataset, "clusters", file_name)
+#     try:
+#         df = pd.read_parquet(file_path)
+#     except FileNotFoundError:
+#         return jsonify({"error": "File not found"}), 404
 
-    if index >= len(df):
-        return jsonify({"error": "Index out of range"}), 400
+#     if index >= len(df):
+#         return jsonify({"error": "Index out of range"}), 400
 
-    df.at[index, 'label'] = new_label
-    df.to_parquet(file_path)
+#     df.at[index, 'label'] = new_label
+#     df.to_parquet(file_path)
 
-    return jsonify({"success": True, "message": "Label updated successfully"})
+#     return jsonify({"success": True, "message": "Label updated successfully"})
 
 
 @datasets_bp.route('/<dataset>/clusters/<cluster>/labels_available', methods=['GET'])
 def get_dataset_cluster_labels_available(dataset, cluster):
     directory_path = os.path.join(DATA_DIR, dataset, "clusters")
     return scan_for_json_files(directory_path, match_pattern=rf"{cluster}-labels-.*\.json")
     # try:
@@ -188,24 +189,74 @@
         next_scopes_number = 1
     return next_scopes_number
 
 @datasets_bp.route('/<dataset>/scopes', methods=['GET'])
 def get_dataset_scopes(dataset):
     directory_path = os.path.join(DATA_DIR, dataset, "scopes")
     print("dataset", dataset, directory_path)
-    return scan_for_json_files(directory_path)
+    return scan_for_json_files(directory_path, match_pattern=r".*[0-9]+\.json$")
 
 @datasets_bp.route('/<dataset>/scopes/<scope>', methods=['GET'])
 def get_dataset_scope(dataset, scope):
     directory_path = os.path.join(DATA_DIR, dataset, "scopes")
     file_path = os.path.join(directory_path, scope + ".json")
     with open(file_path, 'r', encoding='utf-8') as json_file:
         json_contents = json.load(json_file)
     return jsonify(json_contents)
 
+@datasets_bp.route('/<dataset>/scopes/<scope>/parquet', methods=['GET'])
+def get_dataset_scope_parquet(dataset, scope):
+    directory_path = os.path.join(DATA_DIR, dataset, "scopes")
+    file_path = os.path.join(directory_path, scope + ".parquet")
+    df = pd.read_parquet(file_path)
+    return df.to_json(orient="records")
+
+@datasets_write_bp.route('/<dataset>/scopes/<scope>/description', methods=['GET'])
+def overwrite_scope_description(dataset, scope):
+    new_label = request.args.get('label')
+    new_description = request.args.get('description')
+
+    file_name = scope + ".json"
+    file_path = os.path.join(DATA_DIR, dataset, "scopes", file_name)
+    with open(file_path, 'r', encoding='utf-8') as json_file:
+        json_contents = json.load(json_file)
+
+    json_contents['label'] = new_label
+    json_contents['description'] = new_description
+
+    with open(file_path, 'w', encoding='utf-8') as json_file:
+        json.dump(json_contents, json_file)
+    
+    return jsonify({"success": True, "message": "Description updated successfully"})
+
+@datasets_write_bp.route('/<dataset>/scopes/<scope>/new-cluster', methods=['GET'])
+def new_scope_cluster(dataset, scope):
+    new_label = request.args.get('label')
+
+    file_name = scope + ".json"
+    file_path = os.path.join(DATA_DIR, dataset, "scopes", file_name)
+    with open(file_path, 'r', encoding='utf-8') as json_file:
+        json_contents = json.load(json_file)
+
+    clusters = json_contents.get('cluster_labels_lookup', [])
+    clusterIndex = len(clusters)
+    clusters.append({
+        "cluster": clusterIndex, 
+        "label": new_label,
+        "hull": [],
+        "description": ""
+    })
+    json_contents['cluster_labels_lookup'] = clusters
+
+    with open(file_path, 'w', encoding='utf-8') as json_file:
+        json.dump(json_contents, json_file)
+    
+    return jsonify({"success": True, "message": "Description updated successfully"})
+
+
 @datasets_bp.route('/<dataset>/export/list', methods=['GET'])
 def get_dataset_export_list(dataset):
     directory_path = os.path.join(DATA_DIR, dataset)
     print("dataset", dataset, directory_path)
     # scan the directory for files and directories
     # then walk the directories to find all the files
     # then return the list of files
```

### Comparing `latentscope-0.1.9/latentscope/server/jobs.py` & `latentscope-0.2.0/latentscope/server/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,62 +113,80 @@
                 jobs.append(job)
     return jsonify(jobs)
 
 @jobs_write_bp.route('/ingest', methods=['POST'])
 def run_ingest():
     dataset = request.form.get('dataset')
     file = request.files.get('file')
+    text_column = request.form.get('text_column')
     dataset_dir = os.path.join(DATA_DIR, dataset)
     if not os.path.exists(dataset_dir):
         os.makedirs(dataset_dir)
     file_path = os.path.join(dataset_dir, file.filename)
     file.save(file_path)
 
     job_id = str(uuid.uuid4())
-    command = f'ls-ingest {dataset} --path="{file_path}"'
+    command = f'ls-ingest "{dataset}" --path="{file_path}"'
+    if text_column:
+        command += f' --text_column="{text_column}"'
+    threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
+    return jsonify({"job_id": job_id})
+
+@jobs_write_bp.route('/reingest', methods=['GET'])
+def run_reingest():
+    dataset = request.args.get('dataset')
+    text_column = request.args.get('text_column')
+    dataset_dir = os.path.join(DATA_DIR, dataset)
+    file_path = os.path.join(dataset_dir, "input.parquet")
+
+    job_id = str(uuid.uuid4())
+    command = f'ls-ingest "{dataset}" --path="{file_path}"'
+    if text_column:
+        command += f' --text_column="{text_column}"'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 
+
 @jobs_write_bp.route('/embed')
 def run_embed():
     dataset = request.args.get('dataset')
     text_column = request.args.get('text_column')
     model_id = request.args.get('model_id') # model id
     prefix = request.args.get('prefix')
     dimensions = request.args.get('dimensions')
     batch_size = request.args.get('batch_size')
 
     job_id = str(uuid.uuid4())
-    command = f'ls-embed {dataset} "{text_column}" {model_id} --prefix="{prefix}" --batch_size={batch_size}'
+    command = f'ls-embed "{dataset}" "{text_column}" "{model_id}" --prefix="{prefix}" --batch_size={batch_size}'
     if dimensions is not None:
         command += f" --dimensions={dimensions}"
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/embed_truncate')
 def run_embed_truncate():
     dataset = request.args.get('dataset')
     embedding_id = request.args.get('embedding_id') # model id
     dimensions = request.args.get('dimensions')
 
     job_id = str(uuid.uuid4())
-    command = f'ls-embed-truncate {dataset} {embedding_id} {dimensions}'
+    command = f'ls-embed-truncate "{dataset}" "{embedding_id}" {dimensions}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/embed_importer')
 def run_embed_importer():
     dataset = request.args.get('dataset')
     model_id = request.args.get('model_id')
     embedding_column = request.args.get('embedding_column')
     text_column = request.args.get('text_column')
 
     job_id = str(uuid.uuid4())
-    command = f'ls-embed-importer {dataset} {embedding_column} "{model_id}" {text_column}'
+    command = f'ls-embed-importer "{dataset}" "{embedding_column}" "{model_id}" "{text_column}"'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/rerun')
 def rerun_job():
     dataset = request.args.get('dataset')
     job_id = request.args.get('job_id')
@@ -217,15 +235,15 @@
             with open(os.path.join(umap_dir, file), 'r') as f:
                 umap_data = json.load(f)
             if umap_data.get('embedding_id') == embedding_id:
                 umaps_to_delete.append(file.replace('.json', ''))
     
 
     job_id = str(uuid.uuid4())
-    command = f'rm -rf {os.path.join(DATA_DIR, dataset, "embeddings", f"{embedding_id}*")}'
+    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "embeddings", f"{embedding_id}*")}"'
     for umap in umaps_to_delete:
         delete_umap(dataset, umap)
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/umap')
 def run_umap():
@@ -234,15 +252,15 @@
     neighbors = request.args.get('neighbors')
     min_dist = request.args.get('min_dist')
     init = request.args.get('init')
     align = request.args.get('align')
     print("run umap", dataset, embedding_id, neighbors, min_dist, init, align)
 
     job_id = str(uuid.uuid4())
-    command = f'ls-umap {dataset} {embedding_id} {neighbors} {min_dist}'
+    command = f'ls-umap "{dataset}" "{embedding_id}" {neighbors} {min_dist}'
     if init:
         command += f' --init={init}'
     if align:
         command += f' --align={align}'
 
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
@@ -262,56 +280,56 @@
             with open(os.path.join(cluster_dir, file), 'r') as f:
                 cluster_data = json.load(f)
             if cluster_data.get('umap_id') == umap_id:
                 clusters_to_delete.append(file.replace('.json', ''))
     
 
     job_id = str(uuid.uuid4())
-    command = f'rm -rf {os.path.join(DATA_DIR, dataset, "umaps", f"{umap_id}*")}'
+    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "umaps", f"{umap_id}*")}"'
     # Create the rm -rf commands from the clusters_to_delete list
     for cluster in clusters_to_delete:
-        command += f'; rm {os.path.join(DATA_DIR, dataset, "clusters", f"{cluster}*")}'
+        command += f'; rm "{os.path.join(DATA_DIR, dataset, "clusters", f"{cluster}*")}"'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/cluster')
 def run_cluster():
     dataset = request.args.get('dataset')
     umap_id = request.args.get('umap_id')
     samples = request.args.get('samples')
     min_samples = request.args.get('min_samples')
     cluster_selection_epsilon = request.args.get('cluster_selection_epsilon')
     print("run cluster", dataset, umap_id, samples, min_samples, cluster_selection_epsilon)
 
     job_id = str(uuid.uuid4())
-    command = f'ls-cluster {dataset} {umap_id} {samples} {min_samples} {cluster_selection_epsilon}'
+    command = f'ls-cluster "{dataset}" "{umap_id}" {samples} {min_samples} {cluster_selection_epsilon}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/delete/cluster')
 def delete_cluster():
     dataset = request.args.get('dataset')
     cluster_id = request.args.get('cluster_id')
     job_id = str(uuid.uuid4())
-    command = f'rm -rf {os.path.join(DATA_DIR, dataset, "clusters", f"{cluster_id}*")}'
+    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "clusters", f"{cluster_id}*")}"'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/cluster_label')
 def run_cluster_label():
     dataset = request.args.get('dataset')
     chat_id = request.args.get('chat_id')
     text_column = request.args.get('text_column')
     cluster_id = request.args.get('cluster_id')
     context = request.args.get('context')
     print("run cluster label", dataset, chat_id, text_column, cluster_id)
     print("context", context)
 
     job_id = str(uuid.uuid4())
-    command = f'ls-label {dataset} "{text_column}" {cluster_id} {chat_id} "{context}"'
+    command = f'ls-label "{dataset}" "{text_column}" "{cluster_id}" "{chat_id}" "{context}"'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/scope')
 def run_scope():
     dataset = request.args.get('dataset')
     embedding_id = request.args.get('embedding_id')
@@ -320,13 +338,23 @@
     cluster_labels_id = request.args.get('cluster_labels_id')
     label = request.args.get('label')
     description = request.args.get('description')
     scope_id = request.args.get('scope_id')
     print("run scope", dataset, embedding_id, umap_id, cluster_id, cluster_labels_id, label, description, scope_id)
 
     job_id = str(uuid.uuid4())
-    command = f'ls-scope {dataset} {embedding_id} {umap_id} {cluster_id} {cluster_labels_id} "{label}" "{description}"'
+    command = f'ls-scope "{dataset}" "{embedding_id}" "{umap_id}" "{cluster_id}" "{cluster_labels_id}" "{label}" "{description}"'
     if scope_id:
         command += f' --scope_id={scope_id}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
+@jobs_write_bp.route('/delete/scope')
+def delete_scope():
+    dataset = request.args.get('dataset')
+    scope_id = request.args.get('scope_id')
+
+    job_id = str(uuid.uuid4())
+    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "scopes", f"{scope_id}*")}"'
+    threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
+    return jsonify({"job_id": job_id})
+
```

### Comparing `latentscope-0.1.9/latentscope/server/search.py` & `latentscope-0.2.0/latentscope/server/search.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope/server/tags.py` & `latentscope-0.2.0/latentscope/server/tags.py`

 * *Files 27% similar despite different names*

```diff
@@ -98,33 +98,140 @@
         ts[tag] = indices
         # save the indices to a file
         np.savetxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), indices, fmt='%d')
     # return an object with the tags for a given dataset
     return jsonify(tagsets[dataset])
 
 """
+Add data indices to a tag
+"""
+@tags_write_bp.route("/add", methods=['POST'])
+def add_tags():
+    data = request.get_json()
+    dataset = data.get('dataset')
+    tag = data.get('tag')
+    new_indices = data.get('indices')
+    # print("DATASET", dataset)
+    # print("tag", tag)
+    # print("indices", new_indices)
+
+    if dataset not in tagsets:
+        ts = tagsets[dataset] = {}
+    else:
+        ts = tagsets[dataset]
+    if tag not in ts:
+        # read a tag file, which is just a csv with a single column into an array of integers
+        indices = np.loadtxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), dtype=int).tolist()
+        if type(indices) == int:
+            indices = [indices]
+        ts[tag] = indices
+    else:
+        indices = ts[tag]
+
+    if not indices:
+        indices = []
+
+    # new_indices_list = [int(idx) for idx in new_indices.split(',')]
+    new_indices_list = [int(idx) for idx in new_indices]
+    for idx in new_indices_list:
+        if idx not in indices:
+            indices.append(idx)
+    ts[tag] = indices
+    # save the indices to a file
+    np.savetxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), indices, fmt='%d')
+    # return an object with the tags for a given dataset
+    return jsonify(tagsets[dataset])
+
+
+"""
 Remove a data index from a tag
 """
 @tags_write_bp.route("/remove", methods=['GET'])
 def remove_tag():
     dataset = request.args.get('dataset')
     tag = request.args.get('tag')
-    index = request.args.get('index')
+    index = int(request.args.get('index'))
+    # print("dataset", dataset)
+    # print("tag", tag)
+    # print("index", index)
     if dataset not in tagsets:
-        tagsets[dataset] = {}
+        ts = tagsets[dataset] = {}
     else:
         ts = tagsets[dataset]
     if tag not in ts:
         # read a tag file, which is just a csv with a single column into an array of integers
         indices = np.loadtxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), dtype=int).tolist()
         if type(indices) == int:
             indices = [indices]
         ts[tag] = indices
     else:
         indices = ts[tag]
+    print("indices", indices)
     if index in indices:
-        indices = indices.remove(int(index))
+        print("Removing", index)
+        indices.remove(index)
+        print("removed", indices)
         ts[tag] = indices
         # save the indices to a file
         np.savetxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), indices, fmt='%d')
+    print("returning", tagsets[dataset])
     # return an object with the tags for a given dataset
     return jsonify(tagsets[dataset])
+
+
+"""
+Add data indices to a tag
+"""
+@tags_write_bp.route("/remove", methods=['POST'])
+def remove_tags():
+    data = request.get_json()
+    dataset = data.get('dataset')
+    tag = data.get('tag')
+    remove_indices = data.get('indices')
+    print("dataset", dataset)
+    print("tag", tag)
+    print("indices", remove_indices)
+
+    if dataset not in tagsets:
+        ts = tagsets[dataset] = {}
+    else:
+        ts = tagsets[dataset]
+    if tag not in ts:
+        # read a tag file, which is just a csv with a single column into an array of integers
+        indices = np.loadtxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), dtype=int).tolist()
+        if type(indices) == int:
+            indices = [indices]
+        ts[tag] = indices
+    else:
+        indices = ts[tag]
+
+    if not indices:
+        indices = []
+
+    # new_indices_list = [int(idx) for idx in new_indices.split(',')]
+    new_indices_list = [int(idx) for idx in remove_indices]
+    for idx in new_indices_list:
+        if idx in indices:
+            indices.remove(idx)
+    ts[tag] = indices
+    # save the indices to a file
+    np.savetxt(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"), indices, fmt='%d')
+    # return an object with the tags for a given dataset
+    return jsonify(tagsets[dataset])
+
+
+@tags_write_bp.route("/delete", methods=['GET'])
+def delete_tag():
+    dataset = request.args.get('dataset')
+    tag = request.args.get('tag')
+    if dataset not in tagsets:
+        ts = tagsets[dataset] = {}
+    else:
+        ts = tagsets[dataset]
+    if tag in ts:
+        del ts[tag]
+    try:
+        os.remove(os.path.join(DATA_DIR, dataset, "tags", tag + ".indices"))
+    except FileNotFoundError:
+        pass
+    return jsonify(tagsets[dataset])
+
```

### Comparing `latentscope-0.1.9/latentscope/util/configuration.py` & `latentscope-0.2.0/latentscope/util/configuration.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope.egg-info/PKG-INFO` & `latentscope-0.2.0/latentscope.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
@@ -178,48 +178,51 @@
 Requires-Dist: zipp==3.17.0
 
 # Latent Scope
 [![](https://dcbadge.vercel.app/api/server/x7NvpnM4pY?style=flat)](https://discord.gg/x7NvpnM4pY)
 [![PyPI version](https://img.shields.io/pypi/v/latentscope.svg)](https://pypi.org/project/latentscope/)
 
 Quickly embed, project, cluster and explore a dataset. This project is a new kind of workflow + tool for visualizing and exploring datasets through the lens of latent spaces. 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-explore.png?raw=true" height="480px"  alt="Example exploration">](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-007)
+
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/end.png?raw=true" width="45%"  alt="Setup your scope"><img src="https://github.com/enjalot/latent-scope/blob/main/documentation/curate-combined-cluster.png?raw=true" width="45%"  alt="Explore and Curate your data">
 
 The power of machine learning models to encode unstructured data into high-dimensional embeddings is relatively under-explored. Retrieval Augmented Generation has taken off as a popular usecase for embeddings, but do you feel confident in your understanding of why certain data is being retrieved? Do you have a clear picture of what all is in your dataset? Latentscope is like a microscope that allows you to get a new perspective on what's happening to your data when it's embedded. You can try similarity search with different embeddings, peruse automatically labeled clusters and zoom in on individual data points all while keeping the context of your entire dataset. 
 
-### Demo
-This tool is meant to be run locally or on a trusted server to process data for viewing in the latent scope. You can see the result of the process in a read-only [live demo](https://enjalot.github.io/latent-scope):
-* [datavis survey responses](https://enjalot.github.io/latent-scope/#/datasets/datavis-misunderstood/explore/scopes-001) - 700 survey responses
-* [Dolly 15k](https://enjalot.github.io/latent-scope/#/datasets/dolly15k/explore/scopes-001) - 15k instructions
-* [r/DadJokes](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) - 50k dad jokes
-* [emotion](https://enjalot.github.io/latent-scope/#/datasets/emotion/explore/scopes-001) - 400k emotion statements from Twitter
+<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/process-crop.png?raw=true"  alt="Setup your scope">
 
-The source of each demo dataset is documented in the notebooks linked below. Each demo was chosen to represent different scales of data as well as some common usecases.
+Latent Scope is a tool that encodes a process, taking your input data and running it through the steps of Embedding, Projecting, Clustering and Labeling resulting in a nicely structured annotation useful as input to further analysis. You can also explore the annotated data within the web UI to get a better understanding of your dataset and curate it to get a better quality dataset.
 
-[<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/dadabase-scopes.png?raw=true" width="100%"  alt="Dadabase demo scopes">](https://enjalot.github.io/latent-scope)
+## Getting started
+Follow the documentation guides to get started:
+1. [Install and Configure](https://enjalot.github.io/latent-scope/install-and-config)
+2. [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope)
+3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
+4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
+
+## Example Analysis
+What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
+* Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
+* Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
+* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
 source venv/bin/activate
 pip install latentscope
 ls-init ~/local-scope-data --openai_key=XXX --mistral_key=YYY # optional api keys to enable API models 
 ls-serve 
 ```
 
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
-<img src="https://github.com/enjalot/latent-scope/blob/main/documentation/home.png?raw=true" width="320px"  alt="Ingest">  <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/0-ingest.png?raw=true" width="320px"  alt="Ingest">
-
-Once ingested, you will go through the following 6 steps: Embed, UMAP, Cluster, Label, Scope and Explore 
- <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/1-embed.png?raw=true" width="320px"  alt="Embed"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/2-umap.png?raw=true" width="320px"  alt="UMAP"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/3-cluster.png?raw=true" width="320px"  alt="Cluster"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/4-label.png?raw=true" width="320px"  alt="Label"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/5-scope.png?raw=true" width="320px"  alt="Scope"> <img src="https://github.com/enjalot/latent-scope/blob/main/documentation/6-explore.png?raw=true" width="320px"  alt="Scope">
 
-Each step focuses on the relevant choices to move you to the next step. For example choosing which embedding model you want to use to embed with, or the parameters for UMAP. It's very likely you may want to try several choices at each step, which is why the final step before "Explore" is to make a "scope". You can make multiple scopes, as seen in the [dadabase example](https://enjalot.github.io/latent-scope/#/datasets/dadabase/explore/scopes-004) to explore your data through different lenses (i.e. OpenAI embeddings vs. Jina v2).
+See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
 from latentscope import ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
```

### Comparing `latentscope-0.1.9/latentscope.egg-info/SOURCES.txt` & `latentscope-0.2.0/latentscope.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 latentscope/__init__.py
+latentscope/__version__.py
 latentscope.egg-info/PKG-INFO
 latentscope.egg-info/SOURCES.txt
 latentscope.egg-info/dependency_links.txt
 latentscope.egg-info/entry_points.txt
 latentscope.egg-info/requires.txt
 latentscope.egg-info/top_level.txt
 latentscope/models/__init__.py
@@ -27,13 +28,14 @@
 latentscope/scripts/ingest.py
 latentscope/scripts/label_clusters.py
 latentscope/scripts/scope.py
 latentscope/scripts/umapper-1d.py
 latentscope/scripts/umapper.py
 latentscope/server/__init__.py
 latentscope/server/app.py
+latentscope/server/bulk.py
 latentscope/server/datasets.py
 latentscope/server/jobs.py
 latentscope/server/search.py
 latentscope/server/tags.py
 latentscope/util/__init__.py
 latentscope/util/configuration.py
```

### Comparing `latentscope-0.1.9/latentscope.egg-info/entry_points.txt` & `latentscope-0.2.0/latentscope.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.1.9/latentscope.egg-info/requires.txt` & `latentscope-0.2.0/latentscope.egg-info/requires.txt`

 * *Files identical despite different names*

