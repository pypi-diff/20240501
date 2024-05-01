# Comparing `tmp/sciterra-0.0.1.tar.gz` & `tmp/sciterra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciterra-0.0.1.tar", last modified: Tue Dec 26 05:59:18 2023, max compression
+gzip compressed data, was "sciterra-0.0.2.tar", last modified: Wed May  1 01:17:42 2024, max compression
```

## Comparing `sciterra-0.0.1.tar` & `sciterra-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.604426 sciterra-0.0.1/
--rw-r--r--   0 nathanielimel   (501) staff       (20)     7651 2023-12-26 05:59:18.604104 sciterra-0.0.1/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)     6930 2023-11-13 08:11:42.000000 sciterra-0.0.1/README.md
--rw-r--r--   0 nathanielimel   (501) staff       (20)       84 2023-06-05 00:40:34.000000 sciterra-0.0.1/pyproject.toml
--rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2023-12-26 05:59:18.604534 sciterra-0.0.1/setup.cfg
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1207 2023-11-12 02:03:20.000000 sciterra-0.0.1/setup.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.592954 sciterra-0.0.1/src/
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.593548 sciterra-0.0.1/src/examples/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:29.000000 sciterra-0.0.1/src/examples/__init__.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.594489 sciterra-0.0.1/src/examples/scratch/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:36.000000 sciterra-0.0.1/src/examples/scratch/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1786 2023-11-13 05:59:18.000000 sciterra-0.0.1/src/examples/scratch/main.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1421 2023-11-10 06:06:25.000000 sciterra-0.0.1/src/examples/scratch/run_topography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     3472 2023-12-26 05:26:00.000000 sciterra-0.0.1/src/examples/scratch/util.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.594786 sciterra-0.0.1/src/sciterra/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      253 2023-07-25 05:25:07.000000 sciterra-0.0.1/src/sciterra/__init__.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.598071 sciterra-0.0.1/src/sciterra/librarians/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2023-11-12 17:04:39.000000 sciterra-0.0.1/src/sciterra/librarians/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     6912 2023-11-13 05:42:27.000000 sciterra-0.0.1/src/sciterra/librarians/adslibrarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2115 2023-07-22 05:34:01.000000 sciterra-0.0.1/src/sciterra/librarians/librarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     9618 2023-11-13 05:42:27.000000 sciterra-0.0.1/src/sciterra/librarians/s2librarian.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.599689 sciterra-0.0.1/src/sciterra/mapping/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      246 2023-07-12 00:09:56.000000 sciterra-0.0.1/src/sciterra/mapping/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5323 2023-11-12 18:25:31.000000 sciterra-0.0.1/src/sciterra/mapping/atlas.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    31788 2023-11-13 08:25:37.000000 sciterra-0.0.1/src/sciterra/mapping/cartography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5121 2023-07-20 19:30:28.000000 sciterra-0.0.1/src/sciterra/mapping/publication.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     6125 2023-11-11 02:44:01.000000 sciterra-0.0.1/src/sciterra/mapping/topography.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.600037 sciterra-0.0.1/src/sciterra/misc/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-19 02:27:46.000000 sciterra-0.0.1/src/sciterra/misc/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4084 2023-11-10 06:06:25.000000 sciterra-0.0.1/src/sciterra/misc/utils.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.601897 sciterra-0.0.1/src/sciterra/vectorization/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      291 2023-12-26 05:25:07.000000 sciterra-0.0.1/src/sciterra/vectorization/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2367 2023-12-26 05:58:40.000000 sciterra-0.0.1/src/sciterra/vectorization/bow.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1763 2023-11-13 01:52:29.000000 sciterra-0.0.1/src/sciterra/vectorization/preprocessing.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     3806 2023-11-11 09:57:21.000000 sciterra-0.0.1/src/sciterra/vectorization/projection.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2752 2023-12-26 05:09:45.000000 sciterra-0.0.1/src/sciterra/vectorization/sbert.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4057 2023-12-26 05:58:40.000000 sciterra-0.0.1/src/sciterra/vectorization/scibert.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1009 2023-11-12 17:49:39.000000 sciterra-0.0.1/src/sciterra/vectorization/vectorizer.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4440 2023-12-26 03:43:29.000000 sciterra-0.0.1/src/sciterra/vectorization/word2vec.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.603790 sciterra-0.0.1/src/sciterra.egg-info/
--rw-r--r--   0 nathanielimel   (501) staff       (20)     7651 2023-12-26 05:59:18.000000 sciterra-0.0.1/src/sciterra.egg-info/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1249 2023-12-26 05:59:18.000000 sciterra-0.0.1/src/sciterra.egg-info/SOURCES.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2023-12-26 05:59:18.000000 sciterra-0.0.1/src/sciterra.egg-info/dependency_links.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)      122 2023-12-26 05:59:18.000000 sciterra-0.0.1/src/sciterra.egg-info/requires.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)       24 2023-12-26 05:59:18.000000 sciterra-0.0.1/src/sciterra.egg-info/top_level.txt
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2023-12-26 05:59:18.603514 sciterra-0.0.1/src/tests/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-04 08:04:46.000000 sciterra-0.0.1/src/tests/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2943 2023-11-11 09:57:14.000000 sciterra-0.0.1/src/tests/test_atlas.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    20791 2023-11-12 17:49:39.000000 sciterra-0.0.1/src/tests/test_cartography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5050 2023-11-11 09:57:13.000000 sciterra-0.0.1/src/tests/test_librarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1110 2023-11-11 09:57:10.000000 sciterra-0.0.1/src/tests/test_publication.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    10871 2023-12-26 05:58:40.000000 sciterra-0.0.1/src/tests/test_vectorization.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.011403 sciterra-0.0.2/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     9365 2024-05-01 01:17:42.011084 sciterra-0.0.2/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     8609 2024-03-22 03:23:54.000000 sciterra-0.0.2/README.md
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       84 2023-06-05 00:40:34.000000 sciterra-0.0.2/pyproject.toml
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2024-05-01 01:17:42.011442 sciterra-0.0.2/setup.cfg
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1329 2024-05-01 01:13:10.000000 sciterra-0.0.2/setup.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.001912 sciterra-0.0.2/src/
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.002503 sciterra-0.0.2/src/examples/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:29.000000 sciterra-0.0.2/src/examples/__init__.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.002964 sciterra-0.0.2/src/examples/scratch/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:36.000000 sciterra-0.0.2/src/examples/scratch/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2024-02-06 02:15:00.000000 sciterra-0.0.2/src/examples/scratch/main.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1490 2023-12-26 23:42:31.000000 sciterra-0.0.2/src/examples/scratch/run_topography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     3472 2023-12-26 05:26:00.000000 sciterra-0.0.2/src/examples/scratch/util.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.003077 sciterra-0.0.2/src/sciterra/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      253 2023-07-25 05:25:07.000000 sciterra-0.0.2/src/sciterra/__init__.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.004320 sciterra-0.0.2/src/sciterra/librarians/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2023-11-12 17:04:39.000000 sciterra-0.0.2/src/sciterra/librarians/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     7908 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/librarians/adslibrarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2332 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/librarians/librarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    10475 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/librarians/s2librarian.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.006291 sciterra-0.0.2/src/sciterra/mapping/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      246 2023-07-12 00:09:56.000000 sciterra-0.0.2/src/sciterra/mapping/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5837 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/mapping/atlas.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    32018 2024-05-01 00:58:38.000000 sciterra-0.0.2/src/sciterra/mapping/cartography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5450 2023-12-27 22:43:43.000000 sciterra-0.0.2/src/sciterra/mapping/publication.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     6257 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/mapping/topography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    12388 2024-03-22 03:23:54.000000 sciterra-0.0.2/src/sciterra/mapping/tracing.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.007115 sciterra-0.0.2/src/sciterra/misc/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-19 02:27:46.000000 sciterra-0.0.2/src/sciterra/misc/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4197 2024-03-15 05:07:12.000000 sciterra-0.0.2/src/sciterra/misc/analysis.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4084 2023-11-10 06:06:25.000000 sciterra-0.0.2/src/sciterra/misc/utils.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.009369 sciterra-0.0.2/src/sciterra/vectorization/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      352 2024-02-05 00:13:40.000000 sciterra-0.0.2/src/sciterra/vectorization/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2377 2024-02-06 02:20:47.000000 sciterra-0.0.2/src/sciterra/vectorization/bow.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4725 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/gpt2.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1763 2023-11-13 01:52:29.000000 sciterra-0.0.2/src/sciterra/vectorization/preprocessing.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     3806 2023-11-11 09:57:21.000000 sciterra-0.0.2/src/sciterra/vectorization/projection.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2858 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/sbert.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4145 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/scibert.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1108 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/vectorization/vectorizer.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4570 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/vectorization/word2vec.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.010807 sciterra-0.0.2/src/sciterra.egg-info/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     9365 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1372 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/SOURCES.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/dependency_links.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      143 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/requires.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       24 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/top_level.txt
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.010614 sciterra-0.0.2/src/tests/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-04 08:04:46.000000 sciterra-0.0.2/src/tests/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2943 2023-11-11 09:57:14.000000 sciterra-0.0.2/src/tests/test_atlas.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    21972 2024-05-01 01:00:57.000000 sciterra-0.0.2/src/tests/test_cartography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5050 2023-11-11 09:57:13.000000 sciterra-0.0.2/src/tests/test_librarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1110 2023-11-11 09:57:10.000000 sciterra-0.0.2/src/tests/test_publication.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     8145 2024-03-22 03:23:54.000000 sciterra-0.0.2/src/tests/test_tracing.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    15974 2024-02-06 00:04:07.000000 sciterra-0.0.2/src/tests/test_vectorization.py
```

### Comparing `sciterra-0.0.1/PKG-INFO` & `sciterra-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,16 @@
-Metadata-Version: 2.1
-Name: sciterra
-Version: 0.0.1
-Summary: Scientific literature data exploration analysis
-Home-page: https://github.com/nathimel/sciterra
-Author: Nathaniel Imel
-Author-email: nimel@uci.edu
-Project-URL: Bug Tracker, https://github.com/nathimel/sciterra/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-Requires-Dist: ads
-Requires-Dist: bibtexparser
-Requires-Dist: gensim
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: plotnine
-Requires-Dist: scikit-learn
-Requires-Dist: sentence-transformers
-Requires-Dist: semanticscholar
-Requires-Dist: spacy
-Requires-Dist: torch
-Requires-Dist: transformers
-
 # sciterra: a python library for similarity-based scientometrics
 
 [![build](https://github.com/nathimel/sciterra/actions/workflows/build.yml/badge.svg)](https://github.com/nathimel/sciterra/actions/workflows/build.yml)
 
 Sciterra is a software libary to support data-driven analyses of scientific literature, with a focus on unifying different bibliographic database APIs and document-embedding methods for systematic scientometrics research.
 
 ## Overview
 
-The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services/existing software that makes this simple, this software library exists to
+The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services that can make the individual steps of this simple, this software library exists to
 
 1. Unify the different APIs and vector-based retrieval methods
 
 2. Support scientometrics analyses of citation dynamics, especially with respect to a vectorized 'landscape' of literature.
 
 ## Installing sciterra
 
@@ -44,25 +20,48 @@
 
     `python -m pip install 'sciterra @ git+https://github.com/nathimel/sciterra.git'`
 
 2. Alternatively, download or clone this repository and navigate to the root folder, and install locally:
 
     `pip install -e .`
 
+3. It is not yet recommended because sciterra is still in development, but you can also install via pip from pypi:
+
+    `pip install sciterra`
+
+You will also need to download a trained pipeline for [spacy](https://spacy.io/usage):
+
+`python -m spacy download en_core_web_sm`    
+
+Optional: If you plan on querying the NASA Astrophysical Data System (ADS), you must have an ADS API key saved at `~/.ads/dev_key`.
+To generate an ADS API key navigate to [the ADS web interface](https://ui.adsabs.harvard.edu/), create and sign in to an ADS account, and navigate to [Settings > API Token](https://ui.adsabs.harvard.edu/user/settings/token).
+
+## Tests
+
+To run all the unit tests for sciterra, found at [src/tests](https://github.com/nathimel/sciterra/tree/main/src/tests), run the following command at the root of the repository:
+
+`pytest`
+
+This may take up to several hours in total, due to slow api calls in `test_cartography` and `test_tracing`.
+
+Note: If you opted not to set up authentication for ADS during the set up, the tests in `test_librarian.TestADSLibrarian` and the test `test_tracing.TestExpansion.test_atlas_tracer_ads` will fail.
+<!-- TODO: Add an `--ads` flag to the pytests that is turned off by default. Turn it on if the user is using ADS. -->
+
+
 ## Usage
 
 ### Atlas
 
 The central object in sciterra is the [`Atlas`](src/sciterra/mapping/atlas.py). This is a basic data structure for containing scientific publications that are returned from calls to various bibliographic database APIs.
 
 An Atlas minimally requires a list of [`Publications`](src/sciterra/mapping/publication.py).
 
 #### Publication
 
-A publication object is a minimal wrapper of the publication data, and minimally should have a string identifier. It is designed to encompass the basic metadata contained in the results from some bibliographic database API.
+A publication object is a minimal wrapper around publication data, and should have a string identifier. It is designed to standardize the basic metadata contained in the results from some bibliographic database API.
 
 ```python
 from sciterra import Atlas, Publication
 
 atl = Atlas([Publication({"identifier": "id"})])
 ```
 
@@ -79,27 +78,27 @@
 The Cartographer class is named because interfaces with an Atlas to build out a library of publications. Since it does so via similarity-based retrieval, the resulting Atlas can be considered a 'region' of publications.
 
 To do this, a Cartographer needs two things: an API with which to interface, and a way of getting document embeddings. Both are encapsulated, respectively, by the [`Librarian`](src/sciterra/librarians/librarian.py) and the [`Vectorizer`](src/sciterra/vectorization/vectorizer.py) classes.
 
 ```python
 from sciterra import Cartographer
 from sciterra.librarians import SemanticScholarLibrarian # or ADSLibrarian
-from sciterra.vectorization import SciBERTVectorizer # or Word2VecVectorizer
+from sciterra.vectorization import SciBERTVectorizer # among others
 
 crt = Cartographer(
     librarian=SemanticScholarLibrarian(),
     vectorizer=SciBERTVectorizer(),
 )
 ```
 
 #### Librarian
 
 Each Librarian subclass is designed to be a wrapper for an existing python API service, such as the [ads](https://ads.readthedocs.io/en/latest/) package or the [semanticscholar](https://github.com/danielnsilva/semanticscholar#) client library.
 
-A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keywords arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call is converted to a sciterra Publication object.
+A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keyword arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call should be converted to a sciterra Publication object.
 
 Contributions to sciterra in the form of new Librarian subclasses are encouraged and appreciated.
 
 ### Vectorizer
 
 Vectorizer subclasses override one function, `embed_documents`, which takes a list of strings, representing the text of a publication (currently, just its abstract), and returns an `np.ndarray` of embeddings.
 
@@ -114,44 +113,46 @@
 embeddings = result["embeddings"]
 
 # depending on the vectorizer, sometimes not all embeddings can be obtained due to out-of-vocab issues
 success_indices = result["success_indices"] # shape `(len(embeddings),)`
 fail_indices = result["fail_indices"] # shape `(len(docs) - len(embeddings))``
 ```
 
-Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), and [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#). Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
+Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), [GPT-2](https://huggingface.co/docs/transformers/en/model_doc/gpt2), [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#), and a simple bag-of-words (BOW) vectorizer that uses the same vocabulary as the Word2Vec vectorizer. Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
 
 ### Putting it all together
 
 The main use case for all of these ingredients is to iteratively build out a region of publications. This is done using `iterate_expand`:
 
 ```python
-from sciterra.mapping.cartography import iterate_expand
+from sciterra.mapping.tracing import iterate_expand
 
 # Assuming the initial atlas contains just one publication
-(atl.center, ) = atl.publications.values()
+(atl.center, ) = atl.publications.keys()
 # build out an atlas to contain 10,000 publications, with increasing dissimilarity to the initial publication, saving progress in binary files to the directory named "atlas".
 iterate_expand(
     atl=atl,
     crt=crt,
     atlas_dir="atlas",
     target_size=10000,
     center=atl.center,
 )
 ```
 
-This method has a number of useful keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+This method has a number of keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+
+In practice, it may be helpful to use the [`sciterra.mapping.tracing.AtlasTracer`](src/sciterra/mapping/tracing.py) data structure to reduce most of the loading/initialization boilerplate described above. For an example, see [main.py](src/examples/scratch/main.py).
 
 ## Additional features
 
 - The [topography](src/sciterra/mapping/topography.py) submodule contains similarity-based metrics for publications, to support scientometrics analyses.
 
 ## Acknowledgments
 
-This software is an reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
+This software is a reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
 
 To cite sciterra, please use the following workshop paper,
 
 ```
 @inproceedings{Imel2023,
  author = {Imel, Nathaniel, and Hafen, Zachary},
  title = {Citation-similarity relationships in astrophysics},
```

### Comparing `sciterra-0.0.1/README.md` & `sciterra-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,41 @@
+Metadata-Version: 2.1
+Name: sciterra
+Version: 0.0.2
+Summary: Scientific literature data exploration analysis
+Home-page: https://github.com/nathimel/sciterra
+Author: Nathaniel Imel
+Author-email: nimel@uci.edu
+Project-URL: Bug Tracker, https://github.com/nathimel/sciterra/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+Requires-Dist: ads
+Requires-Dist: bibtexparser
+Requires-Dist: gensim
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: plotnine
+Requires-Dist: scikit-learn
+Requires-Dist: scipy==1.10.1
+Requires-Dist: sentence-transformers
+Requires-Dist: semanticscholar==0.5.0
+Requires-Dist: spacy
+Requires-Dist: torch
+Requires-Dist: transformers
+
 # sciterra: a python library for similarity-based scientometrics
 
 [![build](https://github.com/nathimel/sciterra/actions/workflows/build.yml/badge.svg)](https://github.com/nathimel/sciterra/actions/workflows/build.yml)
 
 Sciterra is a software libary to support data-driven analyses of scientific literature, with a focus on unifying different bibliographic database APIs and document-embedding methods for systematic scientometrics research.
 
 ## Overview
 
-The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services/existing software that makes this simple, this software library exists to
+The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services that can make the individual steps of this simple, this software library exists to
 
 1. Unify the different APIs and vector-based retrieval methods
 
 2. Support scientometrics analyses of citation dynamics, especially with respect to a vectorized 'landscape' of literature.
 
 ## Installing sciterra
 
@@ -20,25 +45,48 @@
 
     `python -m pip install 'sciterra @ git+https://github.com/nathimel/sciterra.git'`
 
 2. Alternatively, download or clone this repository and navigate to the root folder, and install locally:
 
     `pip install -e .`
 
+3. It is not yet recommended because sciterra is still in development, but you can also install via pip from pypi:
+
+    `pip install sciterra`
+
+You will also need to download a trained pipeline for [spacy](https://spacy.io/usage):
+
+`python -m spacy download en_core_web_sm`    
+
+Optional: If you plan on querying the NASA Astrophysical Data System (ADS), you must have an ADS API key saved at `~/.ads/dev_key`.
+To generate an ADS API key navigate to [the ADS web interface](https://ui.adsabs.harvard.edu/), create and sign in to an ADS account, and navigate to [Settings > API Token](https://ui.adsabs.harvard.edu/user/settings/token).
+
+## Tests
+
+To run all the unit tests for sciterra, found at [src/tests](https://github.com/nathimel/sciterra/tree/main/src/tests), run the following command at the root of the repository:
+
+`pytest`
+
+This may take up to several hours in total, due to slow api calls in `test_cartography` and `test_tracing`.
+
+Note: If you opted not to set up authentication for ADS during the set up, the tests in `test_librarian.TestADSLibrarian` and the test `test_tracing.TestExpansion.test_atlas_tracer_ads` will fail.
+<!-- TODO: Add an `--ads` flag to the pytests that is turned off by default. Turn it on if the user is using ADS. -->
+
+
 ## Usage
 
 ### Atlas
 
 The central object in sciterra is the [`Atlas`](src/sciterra/mapping/atlas.py). This is a basic data structure for containing scientific publications that are returned from calls to various bibliographic database APIs.
 
 An Atlas minimally requires a list of [`Publications`](src/sciterra/mapping/publication.py).
 
 #### Publication
 
-A publication object is a minimal wrapper of the publication data, and minimally should have a string identifier. It is designed to encompass the basic metadata contained in the results from some bibliographic database API.
+A publication object is a minimal wrapper around publication data, and should have a string identifier. It is designed to standardize the basic metadata contained in the results from some bibliographic database API.
 
 ```python
 from sciterra import Atlas, Publication
 
 atl = Atlas([Publication({"identifier": "id"})])
 ```
 
@@ -55,27 +103,27 @@
 The Cartographer class is named because interfaces with an Atlas to build out a library of publications. Since it does so via similarity-based retrieval, the resulting Atlas can be considered a 'region' of publications.
 
 To do this, a Cartographer needs two things: an API with which to interface, and a way of getting document embeddings. Both are encapsulated, respectively, by the [`Librarian`](src/sciterra/librarians/librarian.py) and the [`Vectorizer`](src/sciterra/vectorization/vectorizer.py) classes.
 
 ```python
 from sciterra import Cartographer
 from sciterra.librarians import SemanticScholarLibrarian # or ADSLibrarian
-from sciterra.vectorization import SciBERTVectorizer # or Word2VecVectorizer
+from sciterra.vectorization import SciBERTVectorizer # among others
 
 crt = Cartographer(
     librarian=SemanticScholarLibrarian(),
     vectorizer=SciBERTVectorizer(),
 )
 ```
 
 #### Librarian
 
 Each Librarian subclass is designed to be a wrapper for an existing python API service, such as the [ads](https://ads.readthedocs.io/en/latest/) package or the [semanticscholar](https://github.com/danielnsilva/semanticscholar#) client library.
 
-A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keywords arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call is converted to a sciterra Publication object.
+A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keyword arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call should be converted to a sciterra Publication object.
 
 Contributions to sciterra in the form of new Librarian subclasses are encouraged and appreciated.
 
 ### Vectorizer
 
 Vectorizer subclasses override one function, `embed_documents`, which takes a list of strings, representing the text of a publication (currently, just its abstract), and returns an `np.ndarray` of embeddings.
 
@@ -90,49 +138,51 @@
 embeddings = result["embeddings"]
 
 # depending on the vectorizer, sometimes not all embeddings can be obtained due to out-of-vocab issues
 success_indices = result["success_indices"] # shape `(len(embeddings),)`
 fail_indices = result["fail_indices"] # shape `(len(docs) - len(embeddings))``
 ```
 
-Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), and [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#). Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
+Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), [GPT-2](https://huggingface.co/docs/transformers/en/model_doc/gpt2), [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#), and a simple bag-of-words (BOW) vectorizer that uses the same vocabulary as the Word2Vec vectorizer. Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
 
 ### Putting it all together
 
 The main use case for all of these ingredients is to iteratively build out a region of publications. This is done using `iterate_expand`:
 
 ```python
-from sciterra.mapping.cartography import iterate_expand
+from sciterra.mapping.tracing import iterate_expand
 
 # Assuming the initial atlas contains just one publication
-(atl.center, ) = atl.publications.values()
+(atl.center, ) = atl.publications.keys()
 # build out an atlas to contain 10,000 publications, with increasing dissimilarity to the initial publication, saving progress in binary files to the directory named "atlas".
 iterate_expand(
     atl=atl,
     crt=crt,
     atlas_dir="atlas",
     target_size=10000,
     center=atl.center,
 )
 ```
 
-This method has a number of useful keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+This method has a number of keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+
+In practice, it may be helpful to use the [`sciterra.mapping.tracing.AtlasTracer`](src/sciterra/mapping/tracing.py) data structure to reduce most of the loading/initialization boilerplate described above. For an example, see [main.py](src/examples/scratch/main.py).
 
 ## Additional features
 
 - The [topography](src/sciterra/mapping/topography.py) submodule contains similarity-based metrics for publications, to support scientometrics analyses.
 
 ## Acknowledgments
 
-This software is an reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
+This software is a reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
 
 To cite sciterra, please use the following workshop paper,
 
 ```
 @inproceedings{Imel2023,
  author = {Imel, Nathaniel, and Hafen, Zachary},
  title = {Citation-similarity relationships in astrophysics},
  booktitle = {AI for Scientific Discovery: From Theory to Practice Workshop (AI4Science @ NeurIPS)},
  year = {2023},
  url = {https://openreview.net/pdf?id=mISayy7DPI},
 }
-```
+```
```

### Comparing `sciterra-0.0.1/setup.py` & `sciterra-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requirements = [
     "ads",
     "bibtexparser",
-    "gensim",
+    "gensim", # N.B.: requires scipy <= 1.10.1
     "numpy",
     "pandas",
     "plotnine",
     "scikit-learn",
+    "scipy==1.10.1",
     "sentence-transformers",
-    "semanticscholar",
+    "semanticscholar==0.5.0",  # 0.6.0 has AsyncSemanticScholar which creates difficulties
     "spacy",
     "torch",
     "transformers",
 ]
 
 test_requirements = [
     "black",
     "coverage",
     "pytest",
 ]
 
 setuptools.setup(
     name="sciterra",
-    version="0.0.1",
+    version="0.0.2",
     author="Nathaniel Imel",
     author_email="nimel@uci.edu",
     description="Scientific literature data exploration analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathimel/sciterra",
     project_urls={"Bug Tracker": "https://github.com/nathimel/sciterra/issues"},
```

### Comparing `sciterra-0.0.1/src/examples/scratch/run_topography.py` & `sciterra-0.0.2/src/examples/scratch/run_topography.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 from sciterra.mapping.atlas import Atlas
 from sciterra.mapping.cartography import Cartographer
 from sciterra.vectorization.scibert import SciBERTVectorizer
 
 
 def main():
-    atlas_dir = "outputs/atlas_from_cc_region_8/"
+    # atlas_dir = "outputs/atlas_from_cc_region_8/"
     # atlas_dir = "outputs/atlas_s2-7-29-23_centered_imeletal"
+    atlas_dir = "outputs/atlas_s2-11-11-23_bow-centered_hafenetal"
 
     atl = Atlas.load(atlas_dir)
 
     print(len(atl))
 
     vectorizer = SciBERTVectorizer(device="mps")
     crt = Cartographer(vectorizer=vectorizer)
```

### Comparing `sciterra-0.0.1/src/examples/scratch/util.py` & `sciterra-0.0.2/src/examples/scratch/util.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/sciterra/librarians/__init__.py` & `sciterra-0.0.2/src/sciterra/librarians/__init__.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/sciterra/librarians/adslibrarian.py` & `sciterra-0.0.2/src/sciterra/librarians/adslibrarian.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "entry_date",  # datetime (earliest possible)
     "pubdate",  # a datetime
     "year",  # int
     "citation_count",
     "citation",  # list
     "reference",  # list
     "identifier",  # list of external ids
+    "arxiv_class",  # list of arxiv classifiers; interestingly, returned even for DOIs that aren't arxiv
 ]
 
 ALLOWED_EXCEPTIONS = (ads.exceptions.APIResponseError,)
 
 EXTERNAL_IDS = [
     "DOI",  # returns a list
     "arXiv",  # returns a str
@@ -188,22 +189,37 @@
                 f"The length of the citations list ({len(citations)}) is different from citation_count ({citation_count})"
             )
             if "infer_citation_count" in kwargs and kwargs["infer_citation_count"]:
                 if verbose:
                     warnings.warn("Setting citation_count = {len(citations)}.")
                 citation_count = len(citations)
 
+        # N.B.: for fields_of_study, manually annotate, and add arxiv classes.
+        fields_of_study = [
+            "ads_dummy_field"
+        ]  # n.b. there is actually some diversity of fields beyond physics in ADS, e.g. theoretical biology.
+        arxiv_classes = article.arxiv_class if article.arxiv_class is not None else []
+        fields_of_study = fields_of_study + arxiv_classes
+        fields_of_study = list(set(fields_of_study))
+
         data = {
             # primary fields
             "identifier": identifier,
             "abstract": article.abstract,
             "publication_date": publication_date,
             "citations": citations,
             "references": references,
             "citation_count": citation_count,
+            "fields_of_study": fields_of_study,
             # additional fields
             "doi": doi,
             "title": article.title,
         }
         data = {k: v for k, v in data.items() if v is not None}
 
         return Publication(data)
+
+
+# TODO: consider implementing `random_publications`
+# We are interested in determining whether the distribution of density is normal, even when not doing the iterative similarity-based expansion loop. To do this, we need a sample of publications that aren't necessarily similar to each other.
+
+# This has already been implemented by Zach in his `background_distribution` step, using cc and ADS.
```

### Comparing `sciterra-0.0.1/src/sciterra/librarians/librarian.py` & `sciterra-0.0.2/src/sciterra/librarians/librarian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from ..mapping.publication import Publication
 
+from abc import ABC, abstractmethod
+from functools import partial
 from typing import Any
 from multiprocessing import Pool
 from tqdm import tqdm
 
 
-class Librarian:
-    def __init__(self) -> None:
-        pass
-
+class Librarian(ABC):
+    @abstractmethod
     def bibtex_entry_identifier(self, bibtex_entry: dict) -> str:
         """Parse a bibtex entry for a usable unique identifier appropriate to the API."""
         raise NotImplementedError
 
+    @abstractmethod
     def get_publications(
         self,
         identifiers: list[str],
         *args,
         call_size: int = None,
         n_attempts_per_query: int = None,
         convert: bool = True,
@@ -27,14 +28,15 @@
         Args:
             n_attempts_per_query: Number of attempts to access the API per query. Useful when experiencing connection issues.
 
             call_size: (int): maximum number of papers to call API for in one query; if less than `len(paper_ids)`, chunking will be performed.
         """
         raise NotImplementedError
 
+    @abstractmethod
     def convert_publication(self, pub: Any, *args, **kwargs):
         """Convert an API-specific resulting publication data structure into a sciterra Publication object."""
         raise NotImplementedError
 
     def convert_publications(
         self,
         papers: list,
@@ -42,27 +44,29 @@
         multiprocess: bool = True,
         num_processes=6,
         **kwargs,
     ) -> list[Publication]:
         """Convet a list of API-specific results to sciterra Publications, possibly using multiprocessing."""
 
         # TODO: you need to pass args and kwargs into these
-
         if not multiprocess:
             return [
                 self.convert_publication(
                     paper,
                     *args,
                     **kwargs,
                 )
                 for paper in papers
             ]
-
         with Pool(processes=num_processes) as p:
             publications = list(
                 tqdm(
-                    p.imap(self.convert_publication, papers),
+                    p.map(
+                        partial(self.convert_publication, *args, **kwargs),
+                        papers,
+                        chunksize=10,
+                    ),
                     total=len(papers),
                 )
             )
 
         return publications
```

### Comparing `sciterra-0.0.1/src/sciterra/librarians/s2librarian.py` & `sciterra-0.0.2/src/sciterra/librarians/s2librarian.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 # NOTE: semantic scholar will truncate total number of references, citations each at 10,000 for the entire batch.
 QUERY_FIELDS = [
     "year",
     "abstract",
     "title",  # useful for inspection
     "externalIds",  # supports ArXiv, MAG, ACL, PubMed, Medline, PubMedCentral, DBLP, DOI
     "citationCount",
+    "fieldsOfStudy",  # useful for scoping to a particular field
+    "s2FieldsOfStudy",  # if above (annotated) is none we can still extract predicted field
     "url",  # as a possible external id
     "citations.externalIds",
     "citations.url",
     "references.externalIds",
     "references.url",
     "citationStyles",  # supports a very basic bibtex that we will augment
     "publicationDate",  # if available, type datetime.datetime (YYYY-MM-DD)
@@ -48,40 +50,14 @@
     "PubMed",
     "Medline",
     "PubMedCentral",
     "DBLP",
     "URL",
 ]
 
-# for storing the results from above, we avoid dot operator to avoid attribute error, but note that everything above will be included.
-# n.b.: no idea what i meant above here
-STORE_FIELDS = [
-    "abstract",
-    "externalIds",
-    "url",
-    "citations",
-    "references",
-    "citationStyles",
-    "publicationDate",
-]
-
-# Attributes to save via save_data
-ATTRS_TO_SAVE = [
-    "paper",
-    "abstract",
-    "citations",
-    "references",
-    "bibcode",
-    "entry_date",
-    "notes",
-    "unofficial_flag",
-    "citation",
-    "stemmed_content_words",
-]
-
 ALLOWED_EXCEPTIONS = (
     Exception,  # "Internal Service Error"
     ReadTimeout,
     ConnectionError,
     ObjectNotFoundException,
 )
 CALL_SIZE = 10
@@ -89,23 +65,35 @@
 
 ##############################################################################
 # Main librarian class
 ##############################################################################
 
 
 class SemanticScholarLibrarian(Librarian):
-    def __init__(self) -> None:
-        self.sch = SemanticScholar()
+    def __init__(
+        self,
+        api_key: str = None,
+        api_key_fn: str = None,
+    ) -> None:
+        if api_key_fn is not None:
+            print(f"Reading private api key from {api_key_fn}.")
+            # Parse api_key_fn for 40-ch private key
+            with open(api_key_fn, "r") as f:
+                api_key = f.read()
+
+        self.sch = SemanticScholar(api_key=api_key)
         super().__init__()
 
     def bibtex_entry_identifier(self, bibtex_entry: dict) -> str:
         """Parse a bibtex entry for a usable identifier for querying SemanticScholar (see EXTERNAL_IDS)."""
         identifier = None
         if "paper_id" in bibtex_entry:
             identifier = bibtex_entry["paper_id"]
+        elif "corpus_id" in bibtex_entry:
+            identifier = f"CorpusID:{bibtex_entry['corpus_id']}"
         elif "doi" in bibtex_entry:
             identifier = f"DOI:{bibtex_entry['doi']}"
         return identifier
 
     def get_publications(
         self,
         paper_ids: list[str],
@@ -200,50 +188,69 @@
         if paper.publicationDate is not None:
             publication_date = paper.publicationDate.date()
         elif paper.year is not None:
             publication_date = date(paper.year, 1, 1)
         else:
             publication_date = None
 
-        # get doi from externalids
-        doi = None
-        if "DOI" in paper.externalIds:
-            doi = paper.externalIds["DOI"]
-
-        # convert citations/references from lists of Papers to identifiers
-        citations = [
-            paper.paperId for paper in paper.citations if paper.paperId is not None
-        ]  # no point using recursion assuming identifier=paperId
+        # Parse citations
+        citations = None
+        if paper.citations is not None:
+            # convert citations/references from lists of Papers to identifiers
+            citations = [
+                paper.paperId for paper in paper.citations if paper.paperId is not None
+            ]  # no point using recursion assuming identifier=paperId
+
         references = [
             paper.paperId for paper in paper.references if paper.paperId is not None
         ]
 
+        # TODO: same with citationCount
         citation_count = paper.citationCount
         if citation_count != len(citations) and verbose:
             warnings.warn(
                 f"The length of the citations list ({len(citations)}) is different from citation_count ({citation_count})"
             )
+
+        # TODO: What if citations = []?
         if (
             "infer_citation_count" in kwargs
             and kwargs["infer_citation_count"]
             and verbose
         ):
             warnings.warn("Setting citation_count = {len(citations)}.")
             citation_count = len(citations)
 
+        # Clobber together a field of study from the validated annoatation or s2's model-predicted fields
+        primary_fields = (
+            paper.fieldsOfStudy
+            if hasattr(paper, "fieldsOfStudy") and paper.fieldsOfStudy is not None
+            else []
+        )
+        addl_fields = (
+            [entry["category"] for entry in paper.s2FieldsOfStudy]
+            if hasattr(paper, "s2FieldsOfStudy") and paper.s2FieldsOfStudy is not None
+            else []
+        )
+        fields_of_study = primary_fields + addl_fields
+        fields_of_study = list(set(fields_of_study))
+        if not fields_of_study:
+            fields_of_study = None
+
         data = {
             # primary fields
             "identifier": identifier,
             "abstract": paper.abstract,
             "publication_date": publication_date,
             "citations": citations,
             "references": references,
             "citation_count": citation_count,
+            "fields_of_study": fields_of_study,
             # additional fields
-            "doi": doi,
+            "doi": paper.externalIds["DOI"] if "DOI" in paper.externalIds else None,
             "url": paper.url if hasattr(paper, "url") else None,
             "title": paper.title if hasattr(paper, "title") else None,
             "issn": paper.issn if hasattr(paper, "issn") else None,
         }
         data = {k: v for k, v in data.items() if v is not None}
 
         return Publication(data)
```

### Comparing `sciterra-0.0.1/src/sciterra/mapping/atlas.py` & `sciterra-0.0.2/src/sciterra/mapping/atlas.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
     `self.projection`: the Projection object containing the embeddings of all publications and their mapping to str identifiers.
 
     `self.bad_ids`: a list of identifiers that have failed for some reason or other during an expansion, and will be excluded from subsequent expansions.
 
     `self.history`: dict of the form {'pubs_per_update': list[list[str]], 'kernel_size': np.ndarray of ints of shape `(num_pubs, last_update)` where last_update <= the total number of expansions performed.}
 
-    `self.center`: the core, central Publication repeatedly passed to `cartography.Cartographer.expand`. Default is None, which means the Atlas has no internal record of the central publication.
+    `self.center`: the core, central Publication identifier repeatedly passed to `cartography.Cartographer.expand`. Default is None, which means the Atlas has no internal record of the central publication.
     """
 
     def __init__(
         self,
         publications: list[Publication],
         projection: Projection = None,
         bad_ids: set[str] = set(),
-        history: dict[str, Any] = dict(),
-        center: Publication = None,
+        history: dict[str, Any] = None,
+        center: str = None,
     ) -> None:
         if not isinstance(publications, list):
             raise ValueError
 
         self.publications: dict[str, Publication] = {
             str(pub): pub for pub in publications
         }
@@ -56,14 +56,15 @@
         Raises:
             ValueError: the identifier is not in the Atlas.
         """
         if identifier in self.publications:
             return self.publications[identifier]
         raise ValueError(f"Identifier {identifier} not in Atlas.")
 
+    @property
     def ids(self) -> list[str]:
         """Get a list of all the publication identifiers in the Atlas."""
         return list(self.publications.keys())
 
     ######################################################################
     # File I/O
     ######################################################################
@@ -76,16 +77,27 @@
         """Write the Atlas to a directory containing a .pkl binary for each attribute.
 
         Warnings cannot be silenced.
 
         Args:
             atlas_dirpath: path of directory to save files to.
         """
-        if not overwrite:
-            return
+
+        # Create directory as needed, or overwrite existing files
+        if os.path.isdir(atlas_dirpath):
+            if not overwrite:
+                warnings.warn(
+                    f"Skipping overwrite of atlas data found at {atlas_dirpath}."
+                )
+                return
+        else:
+            warnings.warn(
+                f"Recursively creating atlas data directory at {atlas_dirpath}."
+            )
+            os.makedirs(atlas_dirpath)
 
         attributes = {
             k: getattr(self, k)
             for k in [
                 "publications",
                 "projection",
                 "bad_ids",
@@ -100,14 +112,16 @@
                 if attribute == "publications":
                     attributes[attribute] = list(self.publications.values())
 
                 fn = f"{attribute}.pkl"
                 fp = os.path.join(atlas_dirpath, fn)
                 if os.path.isfile(fp):
                     warnings.warn(f"Overwriting existing file at {fp}.")
+                else:
+                    warnings.warn(f"Writing to {fp}.")
                 write_pickle(fp, attributes[attribute])
             else:
                 warnings.warn(f"No {attribute} to save, skipping.")
 
     @classmethod
     def load(
         cls,
```

### Comparing `sciterra-0.0.1/src/sciterra/mapping/cartography.py` & `sciterra-0.0.2/src/sciterra/mapping/cartography.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import inspect
 import warnings
 
 import numpy as np
 
 from . import topography
 from .atlas import Atlas
+from .publication import Publication
 from ..librarians.librarian import Librarian
 from ..vectorization.vectorizer import Vectorizer
 from ..vectorization.projection import Projection, merge, get_empty_projection
 from ..misc.utils import get_verbose, custom_formatwarning
 
-from functools import partial
+from typing import Callable, Tuple
 from tqdm import tqdm
 from sklearn.metrics.pairwise import cosine_similarity
 
 warnings.formatwarning = custom_formatwarning
 
 ##############################################################################
 # Helper function
@@ -26,18 +27,18 @@
 
 def batch_cospsi_matrix(embeddings: np.ndarray) -> np.ndarray:
     """Batch-process a pairwise cosine similarity matrix between embeddings.
 
     In order to avoid memory errors (e.g. bus error, segfaults) resulting from too large arrays, we batch process the construction of the cospsi_matrix.
 
     Args:
-        embeddings: a 1D numpy array of embeddings
+        embeddings: a numpy array of embeddings of shape `(num_pubs, embedding_dim)`
 
     Returns:
-        cosine_similarities: a 2D numpy array representing the pairwise cosine similarity between each embedding
+        cosine_similarities: a 2D numpy array of shape `(num_pubs, num_pubs)` representing the pairwise cosine similarity between each embedding
     """
     batch_size = min(1000, len(embeddings))  # Define a batch size
 
     cosine_similarities = None
     print(
         f"computing cosine similarity for {len(embeddings)} embeddings with batch size {batch_size}."
     )
@@ -50,14 +51,39 @@
             cosine_similarities = np.vstack(
                 (cosine_similarities, cosine_similarity(batch, embeddings))
             )
 
     return cosine_similarities
 
 
+# Helper function for filtering
+def pub_has_attributes(
+    pub: Publication,
+    attributes: list[str],
+) -> bool:
+    """Return True if a publication has all `attributes`.
+
+    Args:
+        attributes: the list of attributes to check are not `None` for each publication from the atlas.
+    """
+    return pub is not None and all(
+        [getattr(pub, attr) is not None for attr in attributes]
+    )
+
+
+def pub_has_fields_of_study(
+    pub: Publication,
+    fields_of_study: list[str],
+) -> bool:
+    """Return true if any of `pub.fields_of_study` are in passed `fields_of_study`."""
+    return pub is not None and any(
+        [field in fields_of_study for field in pub.fields_of_study]
+    )
+
+
 ##############################################################################
 # Cartographer
 ##############################################################################
 
 
 class Cartographer:
     """A basic wrapper for obtaining and updating atlas projections.
@@ -137,25 +163,27 @@
 
     def project(self, atl: Atlas, **kwargs) -> Atlas:
         """Update an atlas with its projection, i.e. the document embeddings for all publications using `self.vectorizer`, removing publications with no abstracts.
 
         Args:
             atl: the Atlas containing publications to project to document embeddings
 
+            kwargs: keyword arguments propagated to `filter_by_func`
+
         Returns:
             the updated atlas containing all nonempty-abstract-containing publications and their projection
         """
         verbose = get_verbose(kwargs)
 
         # Only project publications that have abstracts and publication dates
-        atl_filtered = self.filter_by_attributes(atl, **kwargs)
+        atl_filtered = self.filter_by_func(atl, **kwargs)
         num_empty = len(atl) - len(atl_filtered)
         if num_empty and verbose:
             warnings.warn(
-                f"{num_empty} publications were filtered due to missing crucial data. There are now {len(atl_filtered.bad_ids)} total ids that will be excluded in the future."
+                f"{num_empty} publications were filtered due to missing crucial data or incorrect field of study. There are now {len(atl_filtered.bad_ids)} total ids that will be excluded in the future."
             )
 
         # Project
         embeddings = None
         # get only embeddings for publications not already projected in atlas
         previously_embedded_ids = []
         if atl_filtered.projection is not None:
@@ -171,15 +199,16 @@
                     warnings.warn(
                         f"Found {len(atl_filtered.publications) - len(atl_filtered.projection)} publications not contained in Atlas projection."
                     )
                 warnings.warn(f"Embedding {len(embed_ids)} total documents.")
 
             # Embed documents
             result = self.vectorizer.embed_documents(
-                [atl_filtered[id].abstract for id in embed_ids]
+                [atl_filtered[id].abstract for id in embed_ids],
+                batch_size=kwargs["batch_size"] if "batch_size" in kwargs else None,
             )
             embeddings = result["embeddings"]
             success_indices = result["success_indices"]
             fail_indices = result["fail_indices"]
 
             # get new set of bad ids
             atl_filtered.bad_ids = atl_filtered.bad_ids.union(fail_ids)
@@ -218,14 +247,59 @@
 
         # Overwrite atlas data
         atl_filtered.publications = embedded_publications
         atl_filtered.projection = merged_projection
         return atl_filtered
 
     ######################################################################
+    # Sort Atlas
+    ######################################################################
+
+    def sort(
+        self,
+        atl: Atlas,
+        center: str,
+    ) -> Tuple[list[str], list[str]]:
+        """Sort an atlas according to cosine similarity to a center publication.
+        Like numpy argsort, this returns identifiers that can be used to
+        index the original atlas.
+
+        Args:
+            atl: the atlas to sort
+
+            center: center the search on this publication
+
+        Returns:
+            sorted_keys: keys in descending order of similarity to the center publication
+            sorted_values: values in descending order of similarity to the center publication
+        """
+
+        # If atlas is initial
+        if atl.projection is None:
+            atl = self.project(atl)
+            if atl.projection is None:
+                raise Exception(
+                    f"Initial projection of atlas failed; make sure the initial publication has all the required attributes."
+                )
+
+        if len(atl.projection):
+            # build cosine similarity matrix, of shape (1, num_pubs)
+            cospsi_matrix = cosine_similarity(
+                atl.projection.identifiers_to_embeddings([center]),
+                atl.projection.embeddings,
+            )
+            # get most similar keys from center, including center itself
+            sort_inds = np.argsort(cospsi_matrix)[-1][::-1]
+            # argsort orders from least to greatest similarity, so reverse
+            sorted_keys = atl.projection.indices_to_identifiers(sort_inds)
+            sorted_values = cospsi_matrix[0][sort_inds]
+
+            return sorted_keys, sorted_values
+
+    ######################################################################
     # Expand Atlas
     ######################################################################
 
     def expand(
         self,
         atl: Atlas,
         *args,
@@ -247,32 +321,24 @@
             n_sources_max: maximum number of publications (already in the atlas) to draw references and citations from.
 
             record_pubs_per_update: whether to track all the publications that exist in the resulting atlas to `self.pubs_per_update`. This should only be set to `True` when you need to later filter by degree of convergence of the atlas.
 
         Returns:
             atl_expanded: the expanded atlas
         """
-        existing_keys = set(atl.ids())
-        expand_keys = existing_keys
+
+        # Get the keys to expand
+        expand_keys = None
         if center is not None:
-            # If atlas is initial
-            if atl.projection is None:
-                atl = self.project(atl)
+            expand_keys = self.sort(atl, center)[0]
 
-            if len(atl.projection):
-                # build cosine similarity matrix, of shape (1, num_pubs)
-                cospsi_matrix = cosine_similarity(
-                    atl.projection.identifiers_to_embeddings([center]),
-                    atl.projection.embeddings,
-                )
-                # get most similar keys from center, including center itself
-                sort_inds = np.argsort(cospsi_matrix)[::-1][
-                    0
-                ]  # argsort orders from least to greatest similarity, so reverse
-                expand_keys = atl.projection.indices_to_identifiers(sort_inds)
+        # If that didn't work, just use all the keys
+        existing_keys = set(atl.ids)
+        if expand_keys is None:
+            expand_keys = existing_keys
 
         if n_sources_max is not None:
             expand_keys = expand_keys[:n_sources_max]
 
         # Get identifiers for the expansion
         # For each publication corresponding to an id in `expand_keys`, collect the ids corresponding to the publication's references and citations.
         ids = set()
@@ -306,59 +372,62 @@
         atl_exp.projection = (
             atl.projection
         )  # new projection will be updated in `project`
         atl_exp.center = atl.center
 
         # Record the new list of publications
         if record_pubs_per_update:
-            self.pubs_per_update.append(list(atl_exp.ids()))
+            self.pubs_per_update.append(list(atl_exp.ids))
 
         return atl_exp
 
     ######################################################################
     # Filter Atlas
     ######################################################################
 
-    def filter_by_attributes(
+    def filter_by_func(
         self,
         atl: Atlas,
-        attributes: list = [
-            "abstract",
-            "publication_date",
-        ],
+        require_func: Callable[[Publication], bool] = lambda pub: pub_has_attributes(
+            pub,
+            attributes=[
+                "abstract",
+                "publication_date",
+                "fields_of_study",
+            ],
+        ),
         record_pubs_per_update=False,
         **kwargs,
     ) -> Atlas:
         """Update an atlas by dropping publications (and corresponding data in projection) when certain fields are empty.
 
         Args:
             atl: the Atlas containing publications to filter
 
-            attributes: the list of attributes to filter publications from the atlas IF any of items are None for a publication. For example, if attributes = ["abstract"], then all publications `pub` such that `pub.abstract is None` is True will be removed from the atlas, along with the corresponding data in the projection.
+            require_func: a function that takes a publication and returns True if it should be kept in the atlas. For example, if `func = lambda pub: pub_has_attributes(pub, ["abstract"])`, then all publications that have `None` for the attribute `abstract` will be removed from the atlas, along with the corresponding data in the projection.
 
             record_pubs_per_update: whether to track all the publications that exist in the resulting atlas to `self.pubs_per_update`. This should only be set to `True` when you need to later filter by degree of convergence of the atlas. This is an important parameter because `self.filter` is called in `self.project`, which typically is called after `self.expand`, where we pass in the same parameter.
 
         Returns:
             the filtered atlas
         """
         # Filter publications
         invalid_pubs = {
-            id: pub
-            for id, pub in atl.publications.items()
-            if (pub is None or any([getattr(pub, attr) is None for attr in attributes]))
+            id: pub for id, pub in atl.publications.items() if not require_func(pub)
         }
+
         # Do not update if unnecessary
         if not len(invalid_pubs):
             return atl
 
         atl_filtered = self.filter_by_ids(atl, drop_ids=invalid_pubs.keys())
 
         # Record only the publications in the history that weren't filtered out
         if record_pubs_per_update:
-            self.pubs_per_update[-1] = atl_filtered.ids()
+            self.pubs_per_update[-1] = atl_filtered.ids
 
         return atl_filtered
 
     def filter_by_ids(
         self,
         atl: Atlas,
         keep_ids: list[str] = None,
@@ -375,15 +444,15 @@
         """
 
         if all(x is not None for x in [keep_ids, drop_ids]):
             raise ValueError(
                 "You must pass exactly one of `keep_ids` or `drop_ids`, but both had a value that was not `None`."
             )
         if keep_ids is not None:
-            filter_ids = set([id for id in atl.ids() if id not in keep_ids])
+            filter_ids = set([id for id in atl.ids if id not in keep_ids])
         elif drop_ids is not None:
             filter_ids = set(drop_ids)
         else:
             raise ValueError(
                 "You must pass exactly one of `keep_ids` or `drop_ids`, but both had value `None`."
             )
 
@@ -438,24 +507,36 @@
     ########################################################################
     # Record Atlas history
     ########################################################################
 
     def track(
         self,
         atl: Atlas,
+        calculate_convergence: bool = False,
         pubs: list[str] = None,
         pubs_per_update: list[list[str]] = None,
     ) -> Atlas:
-        """Overwrite the data associated with tracking degree of convergence of publications in an atlas over multiple expansions. N.B.: the atlas must be fully projected, or else `converged_kernel_size` will raise a KeyError.
+        """Overwrite the data associated with tracking degree of convergence of publications in an atlas over multiple expansions. N.B.: the atlas must be fully projected, or else `converged_kernel_size` will raise a KeyError. By default, this function will overwrite the `atl.history` with updated `self.pubs_per_update`, but not `kernel_size`, which requires computing the converged kernel size for every publication in the atlas.
 
         Args:
             atl: the Atlas that will be updated by overwriting `Atlas.history`
+
+            calculate_convergence: whether to call `self.converged_kernel_size`, and store the results in the `atl.history`.
+
+            pubs: the list of publications to pass to `self.record_update_history`. By default `None`, and the most recent list of publications in the `self.update_history` list will be used.
+
+            pubs_per_update: the list of lists of publications to pass to `self.record_update_history`. By default `None`, adn the full history in `self.update_history` will be used.
+
+        Returns:
+            atl the updated Atlas
         """
+        print("Tracking atlas...")
         self.record_update_history(pubs, pubs_per_update)
-        kernel_size = self.converged_kernel_size(atl)
+        # Skip expensive convergence calculation if possible
+        kernel_size = self.converged_kernel_size(atl) if calculate_convergence else None
         atl.history = {
             "pubs_per_update": self.pubs_per_update
             if pubs_per_update is None
             else pubs_per_update,
             "kernel_size": kernel_size,
         }
         return atl
@@ -510,53 +591,54 @@
 
         Returns:
             kernel_size: an array of ints of shape `(num_pubs, max_update)` representing the kernel size for converged kernels.
                 - The first column indicates the largest kernel size that hasn't changed since the beginning,
                 - The second column indicates the largest kernel size that hasn't changed since the first update,
                 - etc. for the nth column.
         """
-
+        print("Calculating degree of convergence for all publications.")
         if self.update_history is None:
             raise ValueError(
                 "update_history is None; make sure you have called record_update_history()!"
             )
 
         if -2 in self.update_history:
             raise ValueError(
                 "Incomplete update history as indicated by entries with values of -2."
             )
 
-        publications = np.array(atl.ids())
+        publications = np.array(atl.ids)
 
-        # 1. Loop over each publication
-        cospsi_kernel = []
-        for pub in tqdm(publications):
-            # 2. Identify the similarity with the other publications relative to this publication, and sort accordingly.
-            cospsi = cosine_similarity(
-                atl.projection.identifiers_to_embeddings([pub]),
-                atl.projection.embeddings,
-            ).flatten()  # shape `(num_pubs,)`
+        # Compute pairwise cosine similarity, shape `(num_pubs,num_pubs)`
+        cospsi_matrix = batch_cospsi_matrix(atl.projection.embeddings)
+
+        # 0. Loop over each publication
+        cospsi_kernel: list[list[int]] = []
+        for pub in tqdm(publications, desc="calculating converged kernel size"):
+            # 1. Identify the similarity with the other publications relative to this publication, and sort accordingly.
+            cospsi = cospsi_matrix[publications == pub].flatten()  # shape `(num_pubs,)`
             sort_inds = np.argsort(cospsi)[::-1]  # shape `(num_pubs,)`
 
-            # 3. Identify the expansion iteration at which those publications were added to the atlas (`sorted_history`).
+            # 2. Identify the expansion iteration at which those publications were added to the atlas (`sorted_history`).
             sorted_history = self.update_history[sort_inds]  # shape `(num_pubs,)`
 
-            # 4. Identify the latest iteration at which any publication was added to the atlas; this can be less than the total iterations.
+            # 3. Identify the latest iteration at which any publication was added to the atlas; this can be less than the total iterations.
             last_update = self.update_history.max()
 
-            # 5. Loop through each iteration until `last_update`, and identify which publications were added at or before that iteration.
-            result_2 = [
-                # 6. Compute how many publications out we can go and still only contain publications added at or before that iteration.
+            # 4. Loop through each iteration until `last_update`, and identify which publications were added at or before that iteration.
+            result = [
+                # 5. Compute how many publications out we can go and still only contain publications added at or before that iteration.
                 # Use `argmin` to get the first instance of False
                 # Finally, subtract 1: we want the first index before False.
-                np.argmin(sorted_history <= update) - 1
-                for update in range(last_update)
-            ]  # shape `(num_pubs, last_update)`
+                # See tests.test_cartography.TestConvergence.test_converged_kernel_size for a concrete example.
+                np.argmin(sorted_history <= update_idx) - 1
+                for update_idx in range(last_update)
+            ]  # shape `(last_update, )`
 
-            cospsi_kernel.append(result_2)
+            cospsi_kernel.append(result)
 
         return np.array(cospsi_kernel)
 
     ########################################################################
     # Measure Atlas topography
     ########################################################################
 
@@ -594,19 +676,19 @@
             min_prior_pubs: The minimum number of publications prior to the target publication for which to calculate the metric.
 
             kernel_size: the number of publications surrounding the publication for which to compute the topography metric, i.e. k nearest neighbors for k=kernel_size.
 
         Returns:
             estimates: an np.ndarray of shape `(len(publication_indices), len(metrics))` representing the estimated topography metric values for each publication.
         """
-        verbose = get_verbose(kwargs)
+        _ = get_verbose(kwargs)
 
         # By default calculate for all publications
         if ids is None:
-            ids = atl.ids()
+            ids = atl.ids
         else:
             ids = list(ids)
 
         if not ids:
             raise Exception("No publications to measure topography of.")
 
         # Get publication dates, for filtering
@@ -615,22 +697,19 @@
         # Get pairwise cosine similarities for ids
         embeddings = atl.projection.identifiers_to_embeddings(ids)
         cospsi_matrix = batch_cospsi_matrix(embeddings)
 
         # From here on, use embedding indices instead of identifiers
         # our embeddings are already in the correct order, so just use them
         publication_indices = np.arange(len(embeddings))
-        # publication_indices = atl.projection.identifiers_to_indices(ids)
 
         print(f"Computing {metrics} for {len(ids)} publications.")
         estimates = []
-        # for idx in tqdm(publication_indices):
-        for idx, identifier in enumerate(ids):
+        for idx, identifier in tqdm(enumerate(ids), total=len(ids)):
             # Get the date of publication
-            # identifier = atl.projection.index_to_identifier[idx]
             date = atl[identifier].publication_date
 
             # Identify prior publications
             is_prior = dates < date
             if is_prior.sum() < min_prior_pubs:
                 estimates.append([np.nan for _ in metrics])
                 continue
@@ -664,101 +743,11 @@
                     if key in fn_args.args:
                         used_kwargs[key] = value
                 # Call
                 estimate = fn(**used_kwargs)
                 return estimate
 
             estimates.append([call_metric(metric, **kwargs) for metric in metrics])
+
         estimates = np.array(estimates)
 
         return estimates
-
-
-##############################################################################
-# Iterative expansion helper function
-##############################################################################
-
-
-def iterate_expand(
-    atl: Atlas,
-    crt: Cartographer,
-    atlas_dir: str,
-    target_size: int,
-    max_failed_expansions: int = 2,
-    center: str = None,
-    n_pubs_max: int = None,
-    call_size: int = None,
-    n_sources_max: int = None,
-    record_pubs_per_update: bool = False,
-) -> Atlas:
-    """Build out an Atlas of publications, i.e. search for similar publications. This is done by iterating a sequence of [expand, save, project, save, track, save].
-
-    Args:
-        atl: the Atlas to expand
-
-        crt: the Cartographer to use
-
-        atlas_dir: the directory where Atlas binaries will be saved/loaded from
-
-        target_size: stop iterating when we reach this number of publications in the Atlas
-
-        max_failed_expansions: stop iterating when we fail to add new publications after this many successive iterations. Default is 2.
-
-        center: (if given) center the search on this publication, preferentially searching related publications.
-
-        n_pubs_max: maximum number of publications allowed in the expansion.
-
-        call_size: maximum number of papers to call API for in one query; if less than `len(paper_ids)`, chunking will be performed.
-
-        n_sources_max: maximum number of publications (already in the atlas) to draw references and citations from.
-
-        record_pubs_per_update: whether to track all the publications that exist in the resulting atlas to `self.pubs_per_update`. This should only be set to `True` when you need to later filter by degree of convergence of the atlas.
-
-    Returns:
-        atl: the expanded Atlas
-    """
-    converged = False
-    print_progress = lambda atl: print(  # view incremental progress
-        f"Atlas has {len(atl)} publications and {len(atl.projection) if atl.projection is not None else 'None'} embeddings."
-    )
-
-    # Expansion loop
-    failures = 0
-    its = 0
-    while not converged:
-        its += 1
-        len_prev = len(atl)
-
-        # Retrieve up to n_pubs_max citations and references.
-        atl = crt.expand(
-            atl,
-            center=center,
-            n_pubs_max=n_pubs_max,
-            call_size=call_size,
-            n_sources_max=n_sources_max,
-            record_pubs_per_update=record_pubs_per_update,
-        )
-        print_progress(atl)
-        atl.save(atlas_dir)
-
-        # Obtain document embeddings for all new abstracts.
-        atl = crt.project(
-            atl,
-            verbose=True,
-            record_pubs_per_update=record_pubs_per_update,
-        )
-        print_progress(atl)
-        atl.save(atlas_dir)
-
-        atl = crt.track(atl)
-        atl.save(atlas_dir)
-
-        if len_prev == len(atl):
-            failures += 0
-        else:
-            failures = 0
-
-        converged = len(atl) >= target_size or failures >= max_failed_expansions
-        print()
-
-    print(f"Expansion loop exited with atlas size {len(atl)} after {its} iterations.")
-    return atl
```

### Comparing `sciterra-0.0.1/src/sciterra/mapping/publication.py` & `sciterra-0.0.2/src/sciterra/mapping/publication.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             data: to initialize attributes
         """
         # Below are the attributes we expect every publication to have. If a publication is missing these, it will be removed from analysis.
         self._identifier = None
         self._abstract = None
         self._publication_date = None
         self._citation_count = None
+        self._fields_of_study = None
 
         # Regularize and store data, including but not limited to above attrs.
         self.init_attributes(data, **kwargs)
 
     @property
     def identifier(self) -> str:
         return self._identifier
@@ -95,14 +96,18 @@
         return self._references
 
     @property
     def citation_count(self) -> int:
         """The citation_count can be different from the length of `citations`, since the number of citations listed for a paper might be different from the number of (valid) citing papers indexed on the relevant API."""
         return self._citation_count
 
+    @property
+    def fields_of_study(self) -> list[str]:
+        return self._fields_of_study
+
     def __repr__(self) -> str:
         return "sciterra.publication.Publication:{}".format(self.identifier)
 
     def __str__(self) -> str:
         return self.identifier
 
     def __hash__(self) -> int:
@@ -161,13 +166,19 @@
             # we can use citations, but this is unexpected, so raise a warning.
             if self.citations and verbose:
                 warnings.warn(
                     "Found an entry for 'citations' but no entry for citation_count; this is unexpected. Inferring value from citation_count."
                 )
                 self._citation_count = len(self.citations)
 
+        if "fields_of_study" in data:
+            val = data["fields_of_study"]
+            if not isinstance(val, list):
+                raise ValueError
+            self._fields_of_study = val
+
         ######################################################################
         # Other attributes
         ######################################################################
 
         data_copy = {k: v for k, v in data.items() if k in ADDITIONAL_FIELDS}
         self.__dict__.update(data_copy)
```

### Comparing `sciterra-0.0.1/src/sciterra/mapping/topography.py` & `sciterra-0.0.2/src/sciterra/mapping/topography.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Functions for measuring topographic properties of (the semantic feature space of publications inside) an Atlas."""
 
-import inspect
 import numpy as np
 
 
 ########################################################################
 # Density metrics
 ########################################################################
 
@@ -32,18 +31,15 @@
     """
 
     # We can't have the kernel larger than the number of valid publications
     if kernel_size > len(valid_indices):
         return np.nan
 
     # Get 1D array of similarity scores to idx vector
-    try:
-        cospsi = cospsi_matrix[idx][valid_indices]
-    except IndexError:
-        breakpoint()
+    cospsi = cospsi_matrix[idx][valid_indices]
 
     # Get cosine distance to the least similar vector
     # np.sort orders from least to greatest similarity, so reverse after
     cospsi_max = np.sort(cospsi)[::-1][kernel_size - 1]
 
     # Compute arclength to furthest vector
     return np.arccos(cospsi_max)
@@ -70,14 +66,18 @@
     Returns:
         density: a float representing `kernel_size` divided by arc length containing `kernel_size` other publications.
     """
 
     h = smoothing_length_metric(idx, cospsi_matrix, valid_indices, kernel_size)
     density = kernel_size / h
 
+    # # TODO: there is serious numerical instability for BOW methods. Not sure what the most principled way to deal with them are.
+    # if density > 1e7 and np.isfinite(density):
+    #     breakpoint()
+
     return density
 
 
 ########################################################################
 # Asymmetry metrics
 ########################################################################
```

### Comparing `sciterra-0.0.1/src/sciterra/misc/utils.py` & `sciterra-0.0.2/src/sciterra/misc/utils.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/bow.py` & `sciterra-0.0.2/src/sciterra/vectorization/bow.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """Construct a bag-of-words document vectorizer."""
         # this part is slow because involves training the word2vec model
         self.word2vec_vectorizer = Word2VecVectorizer(*args, **kwargs)
         self.vocabulary = self.word2vec_vectorizer.model.wv.key_to_index
         self.embedding_dim = len(self.vocabulary)
         self.count_vectorizer = CountVectorizer(vocabulary=self.vocabulary)
 
-    def embed_documents(self, docs: list[str]) -> dict[str, ndarray]:
+    def embed_documents(self, docs: list[str], **kwargs) -> dict[str, ndarray]:
         """Embed a list of documents (raw text) into bow document vectors using scikit-learn's CountVectorizer.
 
         Args:
             docs: the documents to embed.
 
         Returns:
             a numpy array of shape `(num_documents, len(self.vocabulary))`
```

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/preprocessing.py` & `sciterra-0.0.2/src/sciterra/vectorization/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/projection.py` & `sciterra-0.0.2/src/sciterra/vectorization/projection.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/sbert.py` & `sciterra-0.0.2/src/sciterra/vectorization/sbert.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 MPS_DEVICE = torch.device("mps")
 
 # MODEL_PATH = "bert-base-nli-mean-tokens" # NOTE: while Liu and Xu (2020) use this model in a metascience context, huggingface recommends a more recent sentence transformer.
 MODEL_PATH = "all-MiniLM-L6-v2"  # All-round model tuned for many use-cases. Trained on a large and diverse dataset of over 1 billion training pairs. Listed as rank 50 on https://huggingface.co/spaces/mteb/leaderboard on 10/11/2023 with an average of 56; rank 1 achieved 64, bert-base-uncased achieved 34; GPT embedding ada-002 achieved 60.
 EMBEDDING_DIM = 384
 MAX_SEQ_LENGTH = 256
 
+BATCH_SIZE = 64
+
 
 class SBERTVectorizer(Vectorizer):
     def __init__(self, device="cuda", **kwargs) -> None:
         # Get the model
         self.model = SentenceTransformer(MODEL_PATH)
 
         # set device to GPU
@@ -34,23 +36,27 @@
         print(f"Using device: {self.device}.")
         self.model.to(self.device)
 
         # Put the model in "evaluation" mode
         self.model.eval()
         super().__init__()
 
-    def embed_documents(self, docs: list[str], batch_size: int = 64) -> np.ndarray:
+    def embed_documents(
+        self, docs: list[str], batch_size: int = BATCH_SIZE
+    ) -> np.ndarray:
         """Embed a list of documents (raw text) into SBERT vectors, by batching.
 
         Args:
             docs: the documents to embed.
 
         Returns:
             a numpy array of shape `(num_documents, 384)`
         """
+        if batch_size is None:
+            batch_size = BATCH_SIZE
 
         embeddings = []
 
         pbar = tqdm(
             total=len(docs),
             desc="embedding documents",
             leave=True,
```

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/scibert.py` & `sciterra-0.0.2/src/sciterra/vectorization/scibert.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 MPS_DEVICE = torch.device("mps")
 
 # the SciBERT pretrained model path from Allen AI repo
 MODEL_PATH = "allenai/scibert_scivocab_uncased"
 EMBEDDING_DIM = 768
 
+BATCH_SIZE = 64
+
 
 class SciBERTVectorizer(Vectorizer):
     def __init__(self, device="cuda", **kwargs) -> None:
         # Get tokenizer
         # TODO: does this include the SCIVOCAB or BASEVOCAB?
         self.tokenizer = BertTokenizerFast.from_pretrained(
             MODEL_PATH,
@@ -49,25 +51,27 @@
         self.model.to(self.device)
 
         # Put the model in "evaluation" mode
         self.model.eval()
         super().__init__()
 
     def embed_documents(
-        self, docs: list[str], batch_size: int = 64
+        self, docs: list[str], batch_size: int = BATCH_SIZE
     ) -> dict[str, np.ndarray]:
         """Embed a list of documents (raw text) into SciBERT vectors, by batching.
 
         Args:
             docs: the documents to embed.
 
         Returns:
             a numpy array of shape `(num_documents, 768)`
 
         """
+        if batch_size is None:
+            batch_size = BATCH_SIZE
 
         embeddings = []
 
         pbar = tqdm(
             total=len(docs),
             desc="embedding documents",
             leave=True,
@@ -97,26 +101,26 @@
                 _, encoded_layers = self.model(  # discard logits
                     **encoded,
                     return_dict=False,
                 )
 
             # Extract the embeddings
             # index last (13th) BERT layer before the classifier
-            final_hidden_state = encoded_layers[12]  # [batch_size, 256, 768]
+            final_hidden_state = encoded_layers[12]  # [batch_size, seq_len, 768]
             # index first token of sequence, [CLS], for our document embeddings
             batched_embeddings = final_hidden_state[:, 0, :]  # [batch_size, 768]
 
             # Move to the CPU and convert to numpy ndarray
             batched_embeddings = batched_embeddings.detach().cpu().numpy()
 
             # Collect batched embeddings
             embeddings.extend(batched_embeddings)
 
             pbar.update(batch_size)
         pbar.close()
 
-        # We don't have to deal with OOV, so we always return full list of ids
+        # We don't deal with OOV, so we always return full list of ids
         return {
             "embeddings": np.array(embeddings),
             "success_indices": np.arange(len(embeddings), dtype=int),
             "fail_indices": np.array([], dtype=int),
         }
```

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/vectorizer.py` & `sciterra-0.0.2/src/sciterra/vectorization/vectorizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Base class for vectorizing abstracts."""
 
 import numpy as np
+from abc import ABC, abstractmethod
 
 
-class Vectorizer:
-    def __init__(self) -> None:
-        pass
-
-    def embed_documents(self, docs: list[str]) -> dict[str, np.ndarray]:
+class Vectorizer(ABC):
+    @abstractmethod
+    def embed_documents(
+        self, docs: list[str], batch_size: int = 64
+    ) -> dict[str, np.ndarray]:
         """Embed a list of documents into document vectors.
 
         Args:
             docs: the documents to embed.
 
+            batch_size: the batch size to use.
+
         Returns:
             a dict of the form
             {
                 "embeddings": a numpy array of shape `(num_successful, embedding_dim)`, containing the document embeddingss
 
                 "success_indices": a numpy array of shape `(num_successful,)`, containing the indices of all the documents for which document embeddings were successfully obtained.
```

### Comparing `sciterra-0.0.1/src/sciterra/vectorization/word2vec.py` & `sciterra-0.0.2/src/sciterra/vectorization/word2vec.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ASTROPHYSICS_CORPUS = "astro_small.txt"
 DEFAULT_CORPUS = os.path.join(corpora_path, ASTROPHYSICS_CORPUS)
 
 
 class Word2VecVectorizer(Vectorizer):
     def __init__(
         self,
-        corpus_path: str = DEFAULT_CORPUS,
+        corpus_path: str,
         model_path: str = None,
         vector_size: int = EMBEDDING_DIM,
         window: int = 5,
         min_count: int = 2,
         workers: int = cpu_count(),
         epochs: int = 10,
         tokenizer: Callable[[str], list[str]] = None,
@@ -55,15 +55,18 @@
 
         if (model_path is None) or (not os.path.exists(model_path)):
             start = time.time()
             # Assume the file is line-based, and one document per line
             print(
                 f"Loading and tokenizing data from {corpus_path} for vocabulary and training..."
             )
-            sentences = [self.tokenizer(line) for line in tqdm(open(corpus_path))]
+            sentences = [
+                self.tokenizer(line)
+                for line in tqdm(open(corpus_path), desc="tokenizing lines")
+            ]
 
             print(f"Training Word2Vec model...")
             model = Word2Vec(
                 sentences=sentences,
                 vector_size=vector_size,
                 window=window,
                 min_count=min_count,
@@ -91,15 +94,20 @@
         """Embed a list of documents (raw text) into word2vec document vectors by averaging the word vectors in each of the documents.
 
         Since there's no speedup via batching like there is in pytorch models, we iterate one document at a time.
         """
         means = []
         success_indices = []
         failed_indices = []
-        for i, doc in tqdm(enumerate(docs), desc="embedding documents", leave=True):
+        for i, doc in tqdm(
+            enumerate(docs),
+            desc="embedding documents",
+            leave=True,
+            total=len(docs),
+        ):
             mean = np.mean(
                 [
                     self.model.wv[word]
                     for word in self.tokenizer(doc)
                     if word in self.model.wv
                 ],  # shape `(300,)`
                 axis=0,
```

### Comparing `sciterra-0.0.1/src/sciterra.egg-info/PKG-INFO` & `sciterra-0.0.2/src/sciterra.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciterra
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scientific literature data exploration analysis
 Home-page: https://github.com/nathimel/sciterra
 Author: Nathaniel Imel
 Author-email: nimel@uci.edu
 Project-URL: Bug Tracker, https://github.com/nathimel/sciterra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,29 +12,30 @@
 Requires-Dist: ads
 Requires-Dist: bibtexparser
 Requires-Dist: gensim
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotnine
 Requires-Dist: scikit-learn
+Requires-Dist: scipy==1.10.1
 Requires-Dist: sentence-transformers
-Requires-Dist: semanticscholar
+Requires-Dist: semanticscholar==0.5.0
 Requires-Dist: spacy
 Requires-Dist: torch
 Requires-Dist: transformers
 
 # sciterra: a python library for similarity-based scientometrics
 
 [![build](https://github.com/nathimel/sciterra/actions/workflows/build.yml/badge.svg)](https://github.com/nathimel/sciterra/actions/workflows/build.yml)
 
 Sciterra is a software libary to support data-driven analyses of scientific literature, with a focus on unifying different bibliographic database APIs and document-embedding methods for systematic scientometrics research.
 
 ## Overview
 
-The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services/existing software that makes this simple, this software library exists to
+The main purpose of sciterra is to perform similarity-based retrieval of scientific publications for metascience/scientometrics research. While there are many services that can make the individual steps of this simple, this software library exists to
 
 1. Unify the different APIs and vector-based retrieval methods
 
 2. Support scientometrics analyses of citation dynamics, especially with respect to a vectorized 'landscape' of literature.
 
 ## Installing sciterra
 
@@ -44,25 +45,48 @@
 
     `python -m pip install 'sciterra @ git+https://github.com/nathimel/sciterra.git'`
 
 2. Alternatively, download or clone this repository and navigate to the root folder, and install locally:
 
     `pip install -e .`
 
+3. It is not yet recommended because sciterra is still in development, but you can also install via pip from pypi:
+
+    `pip install sciterra`
+
+You will also need to download a trained pipeline for [spacy](https://spacy.io/usage):
+
+`python -m spacy download en_core_web_sm`    
+
+Optional: If you plan on querying the NASA Astrophysical Data System (ADS), you must have an ADS API key saved at `~/.ads/dev_key`.
+To generate an ADS API key navigate to [the ADS web interface](https://ui.adsabs.harvard.edu/), create and sign in to an ADS account, and navigate to [Settings > API Token](https://ui.adsabs.harvard.edu/user/settings/token).
+
+## Tests
+
+To run all the unit tests for sciterra, found at [src/tests](https://github.com/nathimel/sciterra/tree/main/src/tests), run the following command at the root of the repository:
+
+`pytest`
+
+This may take up to several hours in total, due to slow api calls in `test_cartography` and `test_tracing`.
+
+Note: If you opted not to set up authentication for ADS during the set up, the tests in `test_librarian.TestADSLibrarian` and the test `test_tracing.TestExpansion.test_atlas_tracer_ads` will fail.
+<!-- TODO: Add an `--ads` flag to the pytests that is turned off by default. Turn it on if the user is using ADS. -->
+
+
 ## Usage
 
 ### Atlas
 
 The central object in sciterra is the [`Atlas`](src/sciterra/mapping/atlas.py). This is a basic data structure for containing scientific publications that are returned from calls to various bibliographic database APIs.
 
 An Atlas minimally requires a list of [`Publications`](src/sciterra/mapping/publication.py).
 
 #### Publication
 
-A publication object is a minimal wrapper of the publication data, and minimally should have a string identifier. It is designed to encompass the basic metadata contained in the results from some bibliographic database API.
+A publication object is a minimal wrapper around publication data, and should have a string identifier. It is designed to standardize the basic metadata contained in the results from some bibliographic database API.
 
 ```python
 from sciterra import Atlas, Publication
 
 atl = Atlas([Publication({"identifier": "id"})])
 ```
 
@@ -79,27 +103,27 @@
 The Cartographer class is named because interfaces with an Atlas to build out a library of publications. Since it does so via similarity-based retrieval, the resulting Atlas can be considered a 'region' of publications.
 
 To do this, a Cartographer needs two things: an API with which to interface, and a way of getting document embeddings. Both are encapsulated, respectively, by the [`Librarian`](src/sciterra/librarians/librarian.py) and the [`Vectorizer`](src/sciterra/vectorization/vectorizer.py) classes.
 
 ```python
 from sciterra import Cartographer
 from sciterra.librarians import SemanticScholarLibrarian # or ADSLibrarian
-from sciterra.vectorization import SciBERTVectorizer # or Word2VecVectorizer
+from sciterra.vectorization import SciBERTVectorizer # among others
 
 crt = Cartographer(
     librarian=SemanticScholarLibrarian(),
     vectorizer=SciBERTVectorizer(),
 )
 ```
 
 #### Librarian
 
 Each Librarian subclass is designed to be a wrapper for an existing python API service, such as the [ads](https://ads.readthedocs.io/en/latest/) package or the [semanticscholar](https://github.com/danielnsilva/semanticscholar#) client library.
 
-A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keywords arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call is converted to a sciterra Publication object.
+A Librarian subclass also overrides two methods. The first is `get_publications`, which takes a list of identifiers, should query the specific API for that Librarian, and returns a list of Publications. Keyword arguments can be passed to specify the metadata that is kept for each publication (e.g. date, title, journal, authors, etc.) The second method is `convert_publication`, which defines how the result of an API call should be converted to a sciterra Publication object.
 
 Contributions to sciterra in the form of new Librarian subclasses are encouraged and appreciated.
 
 ### Vectorizer
 
 Vectorizer subclasses override one function, `embed_documents`, which takes a list of strings, representing the text of a publication (currently, just its abstract), and returns an `np.ndarray` of embeddings.
 
@@ -114,44 +138,46 @@
 embeddings = result["embeddings"]
 
 # depending on the vectorizer, sometimes not all embeddings can be obtained due to out-of-vocab issues
 success_indices = result["success_indices"] # shape `(len(embeddings),)`
 fail_indices = result["fail_indices"] # shape `(len(docs) - len(embeddings))``
 ```
 
-Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), and [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#). Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
+Currently, sciterra has vectorizers using [SciBERT](https://aclanthology.org/D19-1371/), [SBERT](https://www.sbert.net/docs/pretrained_models.html#sentence-embedding-models), [GPT-2](https://huggingface.co/docs/transformers/en/model_doc/gpt2), [Word2Vec](https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#), and a simple bag-of-words (BOW) vectorizer that uses the same vocabulary as the Word2Vec vectorizer. Contributions to sciterra in the form of new Vectorizer subclasses are also encouraged and appreciated.
 
 ### Putting it all together
 
 The main use case for all of these ingredients is to iteratively build out a region of publications. This is done using `iterate_expand`:
 
 ```python
-from sciterra.mapping.cartography import iterate_expand
+from sciterra.mapping.tracing import iterate_expand
 
 # Assuming the initial atlas contains just one publication
-(atl.center, ) = atl.publications.values()
+(atl.center, ) = atl.publications.keys()
 # build out an atlas to contain 10,000 publications, with increasing dissimilarity to the initial publication, saving progress in binary files to the directory named "atlas".
 iterate_expand(
     atl=atl,
     crt=crt,
     atlas_dir="atlas",
     target_size=10000,
     center=atl.center,
 )
 ```
 
-This method has a number of useful keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+This method has a number of keyword arguments that enable tracking the Atlas expansion, limiting the number of publications per expansion, how many times to try to get a response if there are connection issues, etc.
+
+In practice, it may be helpful to use the [`sciterra.mapping.tracing.AtlasTracer`](src/sciterra/mapping/tracing.py) data structure to reduce most of the loading/initialization boilerplate described above. For an example, see [main.py](src/examples/scratch/main.py).
 
 ## Additional features
 
 - The [topography](src/sciterra/mapping/topography.py) submodule contains similarity-based metrics for publications, to support scientometrics analyses.
 
 ## Acknowledgments
 
-This software is an reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
+This software is a reimplimentation of Zachary Hafen-Saavedra's library, [cc](https://github.com/zhafen/cc).
 
 To cite sciterra, please use the following workshop paper,
 
 ```
 @inproceedings{Imel2023,
  author = {Imel, Nathaniel, and Hafen, Zachary},
  title = {Citation-similarity relationships in astrophysics},
```

### Comparing `sciterra-0.0.1/src/sciterra.egg-info/SOURCES.txt` & `sciterra-0.0.2/src/sciterra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,27 @@
 src/sciterra/librarians/librarian.py
 src/sciterra/librarians/s2librarian.py
 src/sciterra/mapping/__init__.py
 src/sciterra/mapping/atlas.py
 src/sciterra/mapping/cartography.py
 src/sciterra/mapping/publication.py
 src/sciterra/mapping/topography.py
+src/sciterra/mapping/tracing.py
 src/sciterra/misc/__init__.py
+src/sciterra/misc/analysis.py
 src/sciterra/misc/utils.py
 src/sciterra/vectorization/__init__.py
 src/sciterra/vectorization/bow.py
+src/sciterra/vectorization/gpt2.py
 src/sciterra/vectorization/preprocessing.py
 src/sciterra/vectorization/projection.py
 src/sciterra/vectorization/sbert.py
 src/sciterra/vectorization/scibert.py
 src/sciterra/vectorization/vectorizer.py
 src/sciterra/vectorization/word2vec.py
 src/tests/__init__.py
 src/tests/test_atlas.py
 src/tests/test_cartography.py
 src/tests/test_librarian.py
 src/tests/test_publication.py
+src/tests/test_tracing.py
 src/tests/test_vectorization.py
```

### Comparing `sciterra-0.0.1/src/tests/test_atlas.py` & `sciterra-0.0.2/src/tests/test_atlas.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/tests/test_cartography.py` & `sciterra-0.0.2/src/tests/test_cartography.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 import bibtexparser
 
 import numpy as np
 
 from datetime import datetime
 
 from sciterra.mapping.atlas import Atlas
-from sciterra.mapping.cartography import Cartographer, iterate_expand
+from sciterra.mapping.cartography import (
+    Cartographer,
+    pub_has_attributes,
+)
 from sciterra.librarians.s2librarian import SemanticScholarLibrarian
 from sciterra.mapping.publication import Publication
 from sciterra.vectorization import SciBERTVectorizer, Word2VecVectorizer
 
 bib_dir = "src/tests/data/bib"
 single_pub_bibtex_fp = f"{bib_dir}/single_publication.bib"
 ten_pub_bibtex_fp = f"{bib_dir}/ten_publications.bib"
 realistic_bibtex_fp = f"{bib_dir}/rdsg.bib"
+corpus_path = "src/tests/data/corpora/astro_1.txt"
 
 ##############################################################################
 # SemanticScholar x SciBERT
 ##############################################################################
 
 atlas_dir = "atlas_tmpdir"
 
@@ -153,14 +157,15 @@
     def test_dummy_projection(self):
         pubs = [
             Publication(
                 {
                     "identifier": f"id_{i}",
                     "abstract": "blah blah blah",
                     "publication_date": datetime(2023, 1, 1),
+                    "fields_of_study": ["dummy_field"],
                 }
             )
             for i in range(10)
         ]
         atl = Atlas(pubs)
 
         atl_proj = TestS2SBProjection.crt.project(atl)
@@ -168,36 +173,38 @@
         projection = atl_proj.projection
 
         vector0 = projection.identifiers_to_embeddings(["id_0"])
         vector1 = projection.identifiers_to_embeddings(["id_9"])
         assert np.array_equal(vector0, vector1)
 
     def test_dummy_projection_partial(self):
-        crt = Cartographer(vectorizer=Word2VecVectorizer())
+        crt = Cartographer(vectorizer=Word2VecVectorizer(corpus_path=corpus_path))
 
         pubs = [
             Publication(
                 {
                     "identifier": f"id_{0}",
                     "abstract": "We use cosmological hydrodynamic simulations with stellar feedback from the FIRE (Feedback In Realistic Environments) project to study the physical nature of Lyman limit systems (LLSs) at z ≤ 1.",  # everything here should be in the Word2Vec default vocab, since it trains on this abstract.
                     "publication_date": datetime(2023, 1, 1),
+                    "fields_of_study": ["dummy_field"],
                 }
             ),
             Publication(
                 {
                     "identifier": f"id_{1}",
                     "abstract": "outofvocabularyitem",  # this should not
                     "publication_date": datetime(2023, 1, 1),
                 }
             ),
             Publication(
                 {
                     "identifier": f"id_{2}",
                     "abstract": "We use cosmological hydrodynamic simulations with stellar feedback from the FIRE (Feedback In Realistic Environments) project to study the physical nature of Lyman limit systems (LLSs) at z ≤ 1.",
                     "publication_date": datetime(2023, 1, 1),
+                    "fields_of_study": ["dummy_field"],
                 }
             ),
         ]
         atl = Atlas(pubs)
 
         atl_proj = crt.project(atl)
 
@@ -208,15 +215,15 @@
         path.mkdir()
         # Construct Atlas
         atl = TestS2SBProjection.crt.bibtex_to_atlas(single_pub_bibtex_fp)
 
         atl_proj = TestS2SBProjection.crt.project(atl)
         projection = atl_proj.projection
 
-        identifier = atl.ids()[0]
+        identifier = atl.ids[0]
         assert projection.identifier_to_index == {identifier: 0}
         assert projection.index_to_identifier == (identifier,)
         assert projection.embeddings.shape == (1, 768)  # (num_pubs, embedding_dim)
 
     def test_project_correct_number(self, tmp_path):
         # Load single file from bibtex
         # Load expected values
@@ -242,31 +249,63 @@
         )
         after = len(atl_exp_double)
 
         # Check that the second projection does not need to pull more docs than necessary
 
         # 1. Simulate first part of project
         # 'only project publications that have abstracts'
-        atl_filtered = TestS2SBProjection.crt.filter_by_attributes(
+        atl_filtered = TestS2SBProjection.crt.filter_by_func(
             atl_exp_double,
-            attributes=["abstract"],
+            require_func=lambda pub: pub_has_attributes(
+                pub,
+                attributes=["abstract"],
+            ),
         )
 
         # 'get only embeddings for publications not already projected in atlas'
         previously_embedded_ids = []
         if atl_filtered.projection is not None:
             previously_embedded_ids = atl_filtered.projection.identifier_to_index
         embed_ids = [
             id for id in atl_filtered.publications if id not in previously_embedded_ids
         ]
 
         # 2. Check that the number of abstracts to be embedded does not exceed the size of the previous expansion
         assert len(embed_ids) <= after - before
 
 
+class TestS2SBSort:
+    librarian = SemanticScholarLibrarian()
+    vectorizer = SciBERTVectorizer()
+    crt = Cartographer(librarian, vectorizer)
+
+    def test_argsort(self, tmp_path):
+        # TODO: This takes a while, and we can probably reduce the time
+
+        # Load single file from bibtex
+        # Load expected values
+        bibtex_fp = ten_pub_bibtex_fp
+        with open(bibtex_fp, "r") as f:
+            bib_database = bibtexparser.load(f)
+
+        path = tmp_path / atlas_dir
+        path.mkdir()
+        # Construct Atlas
+        atl = TestS2SBExpand.crt.bibtex_to_atlas(bibtex_fp)
+
+        pub = list(atl.publications.values())[0]
+        center = pub.identifier
+
+        sorted_keys, sorted_values = TestS2SBSort.crt.sort(atl, center=center)
+        assert len(sorted_keys) == 10
+        assert sorted_keys[0] == center
+        assert sorted_values[0] > sorted_values[1]
+        assert sorted_values[1] > sorted_values[-1]
+
+
 class TestS2SBExpand:
     librarian = SemanticScholarLibrarian()
     vectorizer = SciBERTVectorizer()
     crt = Cartographer(librarian, vectorizer)
 
     def test_expand_single(self, tmp_path):
         # Load single file from bibtex
@@ -383,15 +422,15 @@
         )
         assert measurements.shape == tuple((len(atl), len(metrics)))
 
     def test_measure_topography_subset(self):
         bibtex_fp = ten_pub_bibtex_fp
         atl = TestTopography.crt.bibtex_to_atlas(bibtex_fp)
         atl = TestTopography.crt.project(atl)
-        ids = atl.ids()[:-5]
+        ids = atl.ids[:-5]
         metrics = [
             "density",
             "edginess",
         ]
         measurements = TestTopography.crt.measure_topography(
             atl,
             ids=ids,
@@ -415,15 +454,15 @@
             atl,
             center=center,
             n_pubs_max=200,
         )
 
         # Project, necessary for metrics!
         atl_exp_single = TestTopography.crt.project(atl_exp_single)
-        ids = atl_exp_single.ids()
+        ids = atl_exp_single.ids
 
         metrics = [
             "density",
             "edginess",
         ]
         measurements = TestTopography.crt.measure_topography(
             atl_exp_single,
@@ -441,15 +480,15 @@
     def test_record_update_history(self):
         # Construct Atlas
         bibtex_fp = ten_pub_bibtex_fp
 
         atl = TestConvergence.crt.bibtex_to_atlas(bibtex_fp)
 
         # Mock expansion/update history data
-        input = [
+        history = [
             ["f2c251056dee4c6f9130b31e5e3e4b3296051c49"],  # it=0
             [
                 "4364af31229f7e9a3d83a289a928b2f2a43d30cb",  # it=1
                 "f2c251056dee4c6f9130b31e5e3e4b3296051c49",
                 "287fa946f30eaa78ea86f9c5bd61d67238202356",
             ],
             [
@@ -460,16 +499,16 @@
                 "287fa946f30eaa78ea86f9c5bd61d67238202356",
                 "2e6438be4901cb9b42ff23dcc3d433789b37d032",
                 "04da6471743468b6bb1d26dd9a6eac4c03ca73ee",
             ],
         ]
 
         TestConvergence.crt.record_update_history(
-            atl.ids(),
-            pubs_per_update=input,
+            atl.ids,
+            pubs_per_update=history,
         )
 
         expected = np.array(
             [
                 -2,
                 -2,
                 2,
@@ -505,19 +544,33 @@
                 "54a83cd1d94814b0f37ee48084260a2d1882648d",
                 "4364af31229f7e9a3d83a289a928b2f2a43d30cb",
                 "f2c251056dee4c6f9130b31e5e3e4b3296051c49",
                 "287fa946f30eaa78ea86f9c5bd61d67238202356",
                 "2e6438be4901cb9b42ff23dcc3d433789b37d032",
                 "04da6471743468b6bb1d26dd9a6eac4c03ca73ee",
             ],
-            atl.ids(),  # it=3
+            # it=3, len=10. This is equiv to atl.ids
+            [
+                "9d1a233164f27342d316662821e9a6bb855c25b4",
+                "af6a1c9da102e29fee5d309ec33831207e9f23e5",
+                # ----- it 2 ----
+                "50dea78a96f03ba7fc3398c5deea5174630ef186",
+                "54a83cd1d94814b0f37ee48084260a2d1882648d",
+                "4364af31229f7e9a3d83a289a928b2f2a43d30cb",
+                "f2c251056dee4c6f9130b31e5e3e4b3296051c49",
+                "287fa946f30eaa78ea86f9c5bd61d67238202356",
+                "2e6438be4901cb9b42ff23dcc3d433789b37d032",
+                "04da6471743468b6bb1d26dd9a6eac4c03ca73ee",
+                # ----- end it 2 ----
+                "0def4f553107451204b34470890d019b373798b5",
+            ],
         ]
 
         TestConvergence.crt.record_update_history(
-            atl.ids(),
+            atl.ids,
             input,
         )
 
         expected = np.array(
             [
                 3,
                 3,
@@ -584,39 +637,7 @@
         TestConvergence.crt.record_update_history()
 
         # need to project all pubs before kernel calculations!
         atl = TestConvergence.crt.project(atl)
 
         # test convergence calculations
         result = TestConvergence.crt.converged_kernel_size(atl)
-
-
-class TestIterateExpand:
-    def test_iterate_expand(self, tmp_path):
-        librarian = SemanticScholarLibrarian()
-        vectorizer = SciBERTVectorizer()
-        crt = Cartographer(librarian, vectorizer)
-
-        # Load single file from bibtex
-        bibtex_fp = single_pub_bibtex_fp
-
-        path = tmp_path / atlas_dir
-        path.mkdir()
-
-        # Construct Atlas
-        atl = crt.bibtex_to_atlas(bibtex_fp)
-
-        pub = list(atl.publications.values())[0]
-        center = pub.identifier
-
-        iterate_expand(
-            atl=atl,
-            crt=crt,
-            atlas_dir=path,
-            target_size=100,
-            max_failed_expansions=2,
-            center=center,
-            n_pubs_max=10,
-            call_size=None,
-            n_sources_max=None,
-            record_pubs_per_update=True,
-        )
```

### Comparing `sciterra-0.0.1/src/tests/test_librarian.py` & `sciterra-0.0.2/src/tests/test_librarian.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.1/src/tests/test_publication.py` & `sciterra-0.0.2/src/tests/test_publication.py`

 * *Files identical despite different names*

