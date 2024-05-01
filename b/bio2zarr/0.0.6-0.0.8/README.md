# Comparing `tmp/bio2zarr-0.0.6.tar.gz` & `tmp/bio2zarr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio2zarr-0.0.6.tar", last modified: Wed Apr 24 11:49:53 2024, max compression
+gzip compressed data, was "bio2zarr-0.0.8.tar", last modified: Wed May  1 07:42:27 2024, max compression
```

## Comparing `bio2zarr-0.0.6.tar` & `bio2zarr-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,47 @@
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.381729 bio2zarr-0.0.6/.github/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.385730 bio2zarr-0.0.6/.github/workflows/
--rw-r--r--   0 jk        (1000) jk        (1000)     1181 2024-04-24 11:39:12.000000 bio2zarr-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0 jk        (1000) jk        (1000)      299 2024-04-19 14:35:26.000000 bio2zarr-0.0.6/.github/workflows/lint.yml
--rw-r--r--   0 jk        (1000) jk        (1000)     3078 2024-02-14 18:08:29.000000 bio2zarr-0.0.6/.gitignore
--rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 jk        (1000) jk        (1000)     1089 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/CHANGELOG.md
--rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.6/LICENSE
--rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.6/MANIFEST.in
--rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)     2916 2024-03-28 11:53:55.000000 bio2zarr-0.0.6/README.md
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/bio2zarr/
--rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/__init__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/__main__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr/_version.py
--rw-r--r--   0 jk        (1000) jk        (1000)    14397 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/cli.py
--rw-r--r--   0 jk        (1000) jk        (1000)     8516 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/core.py
--rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/plink.py
--rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.6/bio2zarr/provenance.py
--rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/bio2zarr/typing.py
--rw-r--r--   0 jk        (1000) jk        (1000)    83330 2024-04-24 11:39:37.000000 bio2zarr-0.0.6/bio2zarr/vcf.py
--rw-r--r--   0 jk        (1000) jk        (1000)    17307 2024-04-17 13:14:09.000000 bio2zarr-0.0.6/bio2zarr/vcf_utils.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/bio2zarr.egg-info/
--rw-r--r--   0 jk        (1000) jk        (1000)     1076 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)      835 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/SOURCES.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/dependency_links.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/entry_points.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-03-06 15:57:50.000000 bio2zarr-0.0.6/bio2zarr.egg-info/not-zip-safe
--rw-r--r--   0 jk        (1000) jk        (1000)       69 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/requires.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-24 11:49:53.000000 bio2zarr-0.0.6/bio2zarr.egg-info/top_level.txt
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/docs/
--rw-r--r--   0 jk        (1000) jk        (1000)      489 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/Makefile
--rw-r--r--   0 jk        (1000) jk        (1000)     1041 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/_config.yml
--rw-r--r--   0 jk        (1000) jk        (1000)       50 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/_toc.yml
--rwxr-xr-x   0 jk        (1000) jk        (1000)      505 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/build.sh
--rw-r--r--   0 jk        (1000) jk        (1000)      182 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/cli.md
--rw-r--r--   0 jk        (1000) jk        (1000)     1947 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/intro.md
--rw-r--r--   0 jk        (1000) jk        (1000)   107441 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/logo.png
--rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-19 14:33:24.000000 bio2zarr-0.0.6/docs/references.bib
--rw-r--r--   0 jk        (1000) jk        (1000)       94 2024-04-19 14:51:51.000000 bio2zarr-0.0.6/docs/requirements.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      305 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/pyproject.toml
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/requirements/
--rw-r--r--   0 jk        (1000) jk        (1000)      105 2024-04-08 12:31:57.000000 bio2zarr-0.0.6/requirements/development.txt
--rw-r--r--   0 jk        (1000) jk        (1000)     1674 2024-04-24 11:49:53.393730 bio2zarr-0.0.6/setup.cfg
--rw-r--r--   0 jk        (1000) jk        (1000)      311 2024-02-26 14:12:59.000000 bio2zarr-0.0.6/setup.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-04-24 11:49:53.389730 bio2zarr-0.0.6/validation-data/
--rw-r--r--   0 jk        (1000) jk        (1000)     2985 2024-02-29 11:43:51.000000 bio2zarr-0.0.6/validation-data/Makefile
--rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.6/validation-data/split.sh
--rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.6/validation.py
--rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.6/vcf_generator.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.179027 bio2zarr-0.0.8/.github/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.183027 bio2zarr-0.0.8/.github/workflows/
+-rw-r--r--   0 jk        (1000) jk        (1000)      789 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)     1181 2024-04-24 11:39:12.000000 bio2zarr-0.0.8/.github/workflows/docs.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)     2827 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.gitignore
+-rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 jk        (1000) jk        (1000)     1280 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/CHANGELOG.md
+-rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.8/LICENSE
+-rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.8/MANIFEST.in
+-rw-r--r--   0 jk        (1000) jk        (1000)    17401 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)     3075 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/README.md
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.187027 bio2zarr-0.0.8/bio2zarr/
+-rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/__init__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/__main__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr/_version.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    14397 2024-04-24 11:39:37.000000 bio2zarr-0.0.8/bio2zarr/cli.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     9006 2024-04-24 22:27:00.000000 bio2zarr-0.0.8/bio2zarr/core.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/plink.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.8/bio2zarr/provenance.py
+-rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/typing.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    83878 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/bio2zarr/vcf.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    17328 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/bio2zarr/vcf_utils.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/bio2zarr.egg-info/
+-rw-r--r--   0 jk        (1000) jk        (1000)    17401 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)      754 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/entry_points.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      137 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/requires.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/top_level.txt
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/docs/
+-rw-r--r--   0 jk        (1000) jk        (1000)      489 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/Makefile
+-rw-r--r--   0 jk        (1000) jk        (1000)     1041 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/_config.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)       50 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/_toc.yml
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      505 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/build.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)      182 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/cli.md
+-rw-r--r--   0 jk        (1000) jk        (1000)     1947 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/intro.md
+-rw-r--r--   0 jk        (1000) jk        (1000)   107441 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/logo.png
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/references.bib
+-rw-r--r--   0 jk        (1000) jk        (1000)       94 2024-04-19 14:51:51.000000 bio2zarr-0.0.8/docs/requirements.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)     2098 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/pyproject.toml
+-rw-r--r--   0 jk        (1000) jk        (1000)       38 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/setup.cfg
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/validation-data/
+-rw-r--r--   0 jk        (1000) jk        (1000)     2985 2024-02-29 11:43:51.000000 bio2zarr-0.0.8/validation-data/Makefile
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.8/validation-data/split.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/validation.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.8/vcf_generator.py
```

### Comparing `bio2zarr-0.0.6/.github/workflows/docs.yml` & `bio2zarr-0.0.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/.gitignore` & `bio2zarr-0.0.8/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# auto generated by setuptools_scm and configured in pyproject.toml
+bio2zarr/_version.py
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -148,13 +151,13 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# IDE
+.vscode
+.idea
+
+# Mac
+.DS_Store
```

### Comparing `bio2zarr-0.0.6/CHANGELOG.md` & `bio2zarr-0.0.8/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.0.7 2024-04-30
+- Change on-disk format of distributed encode and simplify
+- Check for all partitions nominally completed encoding before doing
+  anything destructive in dencode-finalise
+
 # 0.0.6 2024-04-24
 
 - Only use NOSHUFFLE by default on ``call_genotype`` and bool arrays.
 - Add initial implementation of distributed encode
 
 # 0.0.5 2024-04-17
```

### Comparing `bio2zarr-0.0.6/LICENSE` & `bio2zarr-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/README.md` & `bio2zarr-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![CI](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml)
+
 # bio2zarr
 Convert bioinformatics file formats to Zarr
 
 Initially supports converting VCF to the
 [sgkit vcf-zarr specification](https://github.com/pystatgen/vcf-zarr-spec/)
 
 **This is early alpha-status code: everything is subject to change,
```

### Comparing `bio2zarr-0.0.6/bio2zarr/__main__.py` & `bio2zarr-0.0.8/bio2zarr/__main__.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/bio2zarr/cli.py` & `bio2zarr-0.0.8/bio2zarr/cli.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/bio2zarr/core.py` & `bio2zarr-0.0.8/bio2zarr/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import concurrent.futures as cf
 import contextlib
 import dataclasses
 import logging
 import multiprocessing
+import os
+import os.path
 import threading
 import time
 
 import numcodecs
 import numpy as np
 import tqdm
 import zarr
@@ -41,14 +43,30 @@
         start = split[0] * chunk_size
         stop = (split[-1] + 1) * chunk_size
         stop = min(stop, z.shape[0])
         slices.append((start, stop))
     return slices
 
 
+def du(path):
+    """
+    Return the total bytes stored at this path.
+    """
+    total = os.path.getsize(path)
+    # pathlib walk method doesn't exist until 3.12 :(
+    for root, dirs, files in os.walk(path):
+        for lst in [dirs, files]:
+            for name in lst:
+                fullname = os.path.join(root, name)
+                size = os.path.getsize(fullname)
+                total += size
+    logger.debug(f"du({path}) = {total}")
+    return total
+
+
 class SynchronousExecutor(cf.Executor):
     def submit(self, fn, /, *args, **kwargs):
         future = cf.Future()
         future.set_result(fn(*args, **kwargs))
         return future
```

### Comparing `bio2zarr-0.0.6/bio2zarr/plink.py` & `bio2zarr-0.0.8/bio2zarr/plink.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/bio2zarr/vcf.py` & `bio2zarr-0.0.8/bio2zarr/vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import contextlib
 import dataclasses
 import functools
 import json
 import logging
 import math
 import os
+import os.path
 import pathlib
 import pickle
 import shutil
 import sys
 import tempfile
-from typing import Any, List
+from typing import Any
 
 import cyvcf2
 import humanfriendly
 import numcodecs
 import numpy as np
 import numpy.testing as nt
 import tqdm
@@ -289,25 +290,26 @@
             )
         core.update_progress(1)
         return metadata, vcf.raw_header
 
 
 def check_overlap(partitions):
     for i in range(1, len(partitions)):
-        prev_partition = partitions[i - 1]
-        current_partition = partitions[i]
-        if (
-            prev_partition.region.contig == current_partition.region.contig
-            and prev_partition.region.end > current_partition.region.start
-        ):
-            raise ValueError(
-                f"Multiple VCFs have the region "
-                f"{prev_partition.region.contig}:{prev_partition.region.start}-"
-                f"{current_partition.region.end}"
-            )
+        prev_region = partitions[i - 1].region
+        current_region = partitions[i].region
+        if prev_region.contig == current_region.contig:
+            if prev_region.end is None:
+                logger.warning("Cannot check overlaps; issue #146")
+                continue
+            if prev_region.end > current_region.start:
+                raise ValueError(
+                    f"Multiple VCFs have the region "
+                    f"{prev_region.contig}:{prev_region.start}-"
+                    f"{current_region.end}"
+                )
 
 
 def scan_vcfs(paths, show_progress, target_num_partitions, worker_processes=1):
     logger.info(
         f"Scanning {len(paths)} VCFs attempting to split into {target_num_partitions}"
         f" partitions."
     )
@@ -448,15 +450,15 @@
         value = np.array(value, ndmin=2, dtype=buff.dtype, copy=False)
         buff[j] = FLOAT32_FILL
         buff[j, :, : value.shape[1]] = value
 
 
 def sanitise_int_array(value, ndmin, dtype):
     if isinstance(value, tuple):
-        value = [VCF_INT_MISSING if x is None else x for x in value]  #  NEEDS TEST
+        value = [VCF_INT_MISSING if x is None else x for x in value]  # NEEDS TEST
     value = np.array(value, ndmin=ndmin, copy=False)
     value[value == VCF_INT_MISSING] = -1
     value[value == VCF_INT_FILL] = -2
     # TODO watch out for clipping here!
     return value.astype(dtype)
 
 
@@ -741,17 +743,17 @@
 @dataclasses.dataclass
 class IcfFieldWriter:
     vcf_field: VcfField
     path: pathlib.Path
     transformer: VcfValueTransformer
     compressor: Any
     max_buffered_bytes: int
-    buff: List[Any] = dataclasses.field(default_factory=list)
+    buff: list[Any] = dataclasses.field(default_factory=list)
     buffered_bytes: int = 0
-    chunk_index: List[int] = dataclasses.field(default_factory=lambda: [0])
+    chunk_index: list[int] = dataclasses.field(default_factory=lambda: [0])
     num_records: int = 0
 
     def append(self, val):
         val = self.transformer.transform_and_update_bounds(val)
         assert val is None or isinstance(val, np.ndarray)
         self.buff.append(val)
         val_bytes = sys.getsizeof(val)
@@ -1505,22 +1507,20 @@
         )
 
 
 class VcfZarr:
     def __init__(self, path):
         if not (path / ".zmetadata").exists():
             raise ValueError("Not in VcfZarr format")  # NEEDS TEST
+        self.path = path
         self.root = zarr.open(path, mode="r")
 
-    def __repr__(self):
-        return repr(self.root)  # NEEDS TEST
-
     def summary_table(self):
         data = []
-        arrays = [(a.nbytes_stored, a) for _, a in self.root.arrays()]
+        arrays = [(core.du(self.path / a.basename), a) for _, a in self.root.arrays()]
         arrays.sort(key=lambda x: x[0])
         for stored, array in reversed(arrays):
             d = {
                 "name": array.name,
                 "dtype": str(array.dtype),
                 "stored": display_size(stored),
                 "size": display_size(array.nbytes),
@@ -1545,34 +1545,30 @@
         max_memory = humanfriendly.parse_size(max_memory)
     logger.info(f"Set memory budget to {display_size(max_memory)}")
     return max_memory
 
 
 @dataclasses.dataclass
 class VcfZarrPartition:
-    start_index: int
-    stop_index: int
-    start_chunk: int
-    stop_chunk: int
+    start: int
+    stop: int
 
     @staticmethod
     def generate_partitions(num_records, chunk_size, num_partitions, max_chunks=None):
         num_chunks = int(np.ceil(num_records / chunk_size))
         if max_chunks is not None:
             num_chunks = min(num_chunks, max_chunks)
         partitions = []
         splits = np.array_split(np.arange(num_chunks), min(num_partitions, num_chunks))
         for chunk_slice in splits:
             start_chunk = int(chunk_slice[0])
             stop_chunk = int(chunk_slice[-1]) + 1
             start_index = start_chunk * chunk_size
             stop_index = min(stop_chunk * chunk_size, num_records)
-            partitions.append(
-                VcfZarrPartition(start_index, stop_index, start_chunk, stop_chunk)
-            )
+            partitions.append(VcfZarrPartition(start_index, stop_index))
         return partitions
 
 
 VZW_METADATA_FORMAT_VERSION = "0.1"
 
 
 @dataclasses.dataclass
@@ -1587,15 +1583,15 @@
     def asdict(self):
         return dataclasses.asdict(self)
 
     @staticmethod
     def fromdict(d):
         if d["format_version"] != VZW_METADATA_FORMAT_VERSION:
             raise ValueError(
-                "VcfZarrWriter  format version mismatch: "
+                "VcfZarrWriter format version mismatch: "
                 f"{d['format_version']} != {VZW_METADATA_FORMAT_VERSION}"
             )
         ret = VcfZarrWriterMetadata(**d)
         ret.schema = VcfZarrSchema.fromdict(ret.schema)
         ret.partitions = [VcfZarrPartition(**p) for p in ret.partitions]
         return ret
 
@@ -1672,15 +1668,15 @@
         self.wip_path.mkdir()
         self.arrays_path.mkdir()
         self.partitions_path.mkdir()
         store = zarr.DirectoryStore(self.arrays_path)
         root = zarr.group(store=store)
 
         for column in self.schema.columns.values():
-            self.init_array(root, column, partitions[-1].stop_index)
+            self.init_array(root, column, partitions[-1].stop)
 
         logger.info("Writing WIP metadata")
         with open(self.wip_path / "metadata.json", "w") as f:
             json.dump(self.metadata.asdict(), f, indent=4)
         return len(partitions)
 
     def encode_samples(self, root):
@@ -1759,68 +1755,72 @@
             with open(self.wip_path / "metadata.json") as f:
                 self.metadata = VcfZarrWriterMetadata.fromdict(json.load(f))
             self.icf = IntermediateColumnarFormat(self.metadata.icf_path)
 
     def partition_path(self, partition_index):
         return self.partitions_path / f"p{partition_index}"
 
+    def wip_partition_path(self, partition_index):
+        return self.partitions_path / f"wip_p{partition_index}"
+
     def wip_partition_array_path(self, partition_index, name):
-        return self.partition_path(partition_index) / f"wip_{name}"
+        return self.wip_partition_path(partition_index) / name
 
     def partition_array_path(self, partition_index, name):
         return self.partition_path(partition_index) / name
 
     def encode_partition(self, partition_index):
         self.load_metadata()
-        partition_path = self.partition_path(partition_index)
+        if partition_index < 0 or partition_index >= self.num_partitions:
+            raise ValueError(
+                "Partition index must be in the range 0 <= index < num_partitions"
+            )
+        partition_path = self.wip_partition_path(partition_index)
         partition_path.mkdir(exist_ok=True)
         logger.info(f"Encoding partition {partition_index} to {partition_path}")
 
-        self.encode_alleles_partition(partition_index)
         self.encode_id_partition(partition_index)
         self.encode_filters_partition(partition_index)
         self.encode_contig_partition(partition_index)
+        self.encode_alleles_partition(partition_index)
         for col in self.schema.columns.values():
             if col.vcf_field is not None:
                 self.encode_array_partition(col, partition_index)
         if "call_genotype" in self.schema.columns:
             self.encode_genotypes_partition(partition_index)
 
+        final_path = self.partition_path(partition_index)
+        logger.info(f"Finalising {partition_index} at {final_path}")
+        if final_path.exists():
+            logger.warning("Removing existing partition at {final_path}")
+            shutil.rmtree(final_path)
+        os.rename(partition_path, final_path)
+
     def init_partition_array(self, partition_index, name):
         wip_path = self.wip_partition_array_path(partition_index, name)
         # Create an empty array like the definition
         src = self.arrays_path / name
         # Overwrite any existing WIP files
         shutil.copytree(src, wip_path, dirs_exist_ok=True)
         array = zarr.open(wip_path)
         logger.debug(f"Opened empty array {array} @ {wip_path}")
         return array
 
     def finalise_partition_array(self, partition_index, name):
-        wip_path = self.wip_partition_array_path(partition_index, name)
-        final_path = self.partition_array_path(partition_index, name)
-        if final_path.exists():
-            # NEEDS TEST
-            logger.warning(f"Removing existing {final_path}")
-            shutil.rmtree(final_path)
-        # Atomic swap
-        os.rename(wip_path, final_path)
         logger.debug(f"Encoded {name} partition {partition_index}")
 
     def encode_array_partition(self, column, partition_index):
         array = self.init_partition_array(partition_index, column.name)
 
         partition = self.metadata.partitions[partition_index]
-        ba = core.BufferedArray(array, partition.start_index)
+        ba = core.BufferedArray(array, partition.start)
         source_col = self.icf.columns[column.vcf_field]
         sanitiser = source_col.sanitiser_factory(ba.buff.shape)
 
-        for value in source_col.iter_values(
-            partition.start_index, partition.stop_index
-        ):
+        for value in source_col.iter_values(partition.start, partition.stop):
             # We write directly into the buffer in the sanitiser function
             # to make it easier to reason about dimension padding
             j = ba.next_buffer_row()
             sanitiser(ba.buff, j, value)
         ba.flush()
         self.finalise_partition_array(partition_index, column.name)
 
@@ -1828,22 +1828,20 @@
         gt_array = self.init_partition_array(partition_index, "call_genotype")
         gt_mask_array = self.init_partition_array(partition_index, "call_genotype_mask")
         gt_phased_array = self.init_partition_array(
             partition_index, "call_genotype_phased"
         )
 
         partition = self.metadata.partitions[partition_index]
-        gt = core.BufferedArray(gt_array, partition.start_index)
-        gt_mask = core.BufferedArray(gt_mask_array, partition.start_index)
-        gt_phased = core.BufferedArray(gt_phased_array, partition.start_index)
+        gt = core.BufferedArray(gt_array, partition.start)
+        gt_mask = core.BufferedArray(gt_mask_array, partition.start)
+        gt_phased = core.BufferedArray(gt_phased_array, partition.start)
 
         source_col = self.icf.columns["FORMAT/GT"]
-        for value in source_col.iter_values(
-            partition.start_index, partition.stop_index
-        ):
+        for value in source_col.iter_values(partition.start, partition.stop):
             j = gt.next_buffer_row()
             sanitise_value_int_2d(gt.buff, j, value[:, :-1])
             j = gt_phased.next_buffer_row()
             sanitise_value_int_1d(gt_phased.buff, j, value[:, -1])
             # TODO check is this the correct semantics when we are padding
             # with mixed ploidies?
             j = gt_mask.next_buffer_row()
@@ -1856,39 +1854,39 @@
         self.finalise_partition_array(partition_index, "call_genotype_mask")
         self.finalise_partition_array(partition_index, "call_genotype_phased")
 
     def encode_alleles_partition(self, partition_index):
         array_name = "variant_allele"
         alleles_array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
-        alleles = core.BufferedArray(alleles_array, partition.start_index)
+        alleles = core.BufferedArray(alleles_array, partition.start)
         ref_col = self.icf.columns["REF"]
         alt_col = self.icf.columns["ALT"]
 
         for ref, alt in zip(
-            ref_col.iter_values(partition.start_index, partition.stop_index),
-            alt_col.iter_values(partition.start_index, partition.stop_index),
+            ref_col.iter_values(partition.start, partition.stop),
+            alt_col.iter_values(partition.start, partition.stop),
         ):
             j = alleles.next_buffer_row()
             alleles.buff[j, :] = STR_FILL
             alleles.buff[j, 0] = ref[0]
             alleles.buff[j, 1 : 1 + len(alt)] = alt
         alleles.flush()
 
         self.finalise_partition_array(partition_index, array_name)
 
     def encode_id_partition(self, partition_index):
         vid_array = self.init_partition_array(partition_index, "variant_id")
         vid_mask_array = self.init_partition_array(partition_index, "variant_id_mask")
         partition = self.metadata.partitions[partition_index]
-        vid = core.BufferedArray(vid_array, partition.start_index)
-        vid_mask = core.BufferedArray(vid_mask_array, partition.start_index)
+        vid = core.BufferedArray(vid_array, partition.start)
+        vid_mask = core.BufferedArray(vid_mask_array, partition.start)
         col = self.icf.columns["ID"]
 
-        for value in col.iter_values(partition.start_index, partition.stop_index):
+        for value in col.iter_values(partition.start, partition.stop):
             j = vid.next_buffer_row()
             k = vid_mask.next_buffer_row()
             assert j == k
             if value is not None:
                 vid.buff[j] = value[0]
                 vid_mask.buff[j] = False
             else:
@@ -1901,18 +1899,18 @@
         self.finalise_partition_array(partition_index, "variant_id_mask")
 
     def encode_filters_partition(self, partition_index):
         lookup = {filt: index for index, filt in enumerate(self.schema.filter_id)}
         array_name = "variant_filter"
         array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
-        var_filter = core.BufferedArray(array, partition.start_index)
+        var_filter = core.BufferedArray(array, partition.start)
 
         col = self.icf.columns["FILTERS"]
-        for value in col.iter_values(partition.start_index, partition.stop_index):
+        for value in col.iter_values(partition.start, partition.stop):
             j = var_filter.next_buffer_row()
             var_filter.buff[j] = False
             for f in value:
                 try:
                     var_filter.buff[j, lookup[f]] = True
                 except KeyError:
                     raise ValueError(
@@ -1923,18 +1921,18 @@
         self.finalise_partition_array(partition_index, array_name)
 
     def encode_contig_partition(self, partition_index):
         lookup = {contig: index for index, contig in enumerate(self.schema.contig_id)}
         array_name = "variant_contig"
         array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
-        contig = core.BufferedArray(array, partition.start_index)
+        contig = core.BufferedArray(array, partition.start)
         col = self.icf.columns["CHROM"]
 
-        for value in col.iter_values(partition.start_index, partition.stop_index):
+        for value in col.iter_values(partition.start, partition.stop):
             j = contig.next_buffer_row()
             # Note: because we are using the indexes to define the lookups
             # and we always have an index, it seems that we the contig lookup
             # will always succeed. However, if anyone ever does hit a KeyError
             # here, please do open an issue with a reproducible example!
             contig.buff[j] = lookup[value[0]]
         contig.flush()
@@ -1947,15 +1945,15 @@
 
     def finalise_array(self, name):
         logger.info(f"Finalising {name}")
         final_path = self.path / name
         if final_path.exists():
             # NEEDS TEST
             raise ValueError(f"Array {name} already exists")
-        for partition in range(len(self.metadata.partitions)):
+        for partition in range(self.num_partitions):
             # Move all the files in partition dir to dest dir
             src = self.partition_array_path(partition, name)
             if not src.exists():
                 # Needs test
                 raise ValueError(f"Partition {partition} of {name} does not exist")
             dest = self.arrays_path / name
             # This is Zarr v2 specific. Chunks in v3 with start with "c" prefix.
@@ -1974,14 +1972,23 @@
         # we move it out of wip
         os.rename(self.arrays_path / name, self.path / name)
         core.update_progress(1)
 
     def finalise(self, show_progress=False):
         self.load_metadata()
 
+        logger.info("Scanning {self.num_partitions} partitions")
+        missing = []
+        # TODO may need a progress bar here
+        for partition_id in range(self.num_partitions):
+            if not self.partition_path(partition_id).exists():
+                missing.append(partition_id)
+        if len(missing) > 0:
+            raise FileNotFoundError(f"Partitions not encoded: {missing}")
+
         progress_config = core.ProgressConfig(
             total=len(self.schema.columns),
             title="Finalise",
             units="array",
             show=show_progress,
         )
         # NOTE: it's not clear that adding more workers will make this quicker,
@@ -1991,14 +1998,17 @@
         # SynchronousExecutor which is intended for testing purposes so
         # that we get test coverage. Should fix this either by allowing
         # for multiple workers, or making a standard wrapper for tqdm
         # that allows us to have a consistent look and feel.
         with core.ParallelWorkManager(0, progress_config) as pwm:
             for name in self.schema.columns:
                 pwm.submit(self.finalise_array, name)
+        logger.debug(f"Removing {self.wip_path}")
+        shutil.rmtree(self.wip_path)
+        logger.info("Consolidating Zarr metadata")
         zarr.consolidate_metadata(self.path)
 
     ######################
     # encode_all_partitions
     ######################
 
     def get_max_encoding_memory(self):
```

### Comparing `bio2zarr-0.0.6/bio2zarr/vcf_utils.py` & `bio2zarr-0.0.8/bio2zarr/vcf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import contextlib
 import gzip
 import os
 import pathlib
 import struct
+from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import IO, Any, Dict, Optional, Sequence, Union
+from typing import IO, Any, Optional, Union
 
 import cyvcf2
 import humanfriendly
 import numpy as np
 
 from bio2zarr.typing import PathType
 
@@ -179,15 +180,15 @@
     first_bin_on_level = get_first_bin_in_level(level)
     level_size = get_level_size(level)
     max_span = 1 << (csi.min_shift + 3 * csi.depth)
     return (bin - first_bin_on_level) * (max_span // level_size) + 1
 
 
 def read_csi(
-    file: PathType, storage_options: Optional[Dict[str, str]] = None
+    file: PathType, storage_options: Optional[dict[str, str]] = None
 ) -> CSIIndex:
     """Parse a CSI file into a `CSIIndex` object.
 
     Parameters
     ----------
     file : PathType
         The path to the CSI file.
@@ -293,15 +294,15 @@
         assert len(file_offsets) == len(contig_indexes)
         assert len(file_offsets) == len(positions)
 
         return file_offsets, contig_indexes, positions
 
 
 def read_tabix(
-    file: PathType, storage_options: Optional[Dict[str, str]] = None
+    file: PathType, storage_options: Optional[dict[str, str]] = None
 ) -> TabixIndex:
     """Parse a tabix file into a `TabixIndex` object.
 
     Parameters
     ----------
     file : PathType
         The path to the tabix file.
```

### Comparing `bio2zarr-0.0.6/bio2zarr.egg-info/SOURCES.txt` & `bio2zarr-0.0.8/bio2zarr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 validation.py
 vcf_generator.py
+.github/workflows/ci.yml
 .github/workflows/docs.yml
-.github/workflows/lint.yml
 bio2zarr/__init__.py
 bio2zarr/__main__.py
 bio2zarr/_version.py
 bio2zarr/cli.py
 bio2zarr/core.py
 bio2zarr/plink.py
 bio2zarr/provenance.py
 bio2zarr/typing.py
 bio2zarr/vcf.py
 bio2zarr/vcf_utils.py
 bio2zarr.egg-info/PKG-INFO
 bio2zarr.egg-info/SOURCES.txt
 bio2zarr.egg-info/dependency_links.txt
 bio2zarr.egg-info/entry_points.txt
-bio2zarr.egg-info/not-zip-safe
 bio2zarr.egg-info/requires.txt
 bio2zarr.egg-info/top_level.txt
 docs/Makefile
 docs/_config.yml
 docs/_toc.yml
 docs/build.sh
 docs/cli.md
 docs/intro.md
 docs/logo.png
 docs/references.bib
 docs/requirements.txt
-requirements/development.txt
 validation-data/Makefile
 validation-data/split.sh
```

### Comparing `bio2zarr-0.0.6/docs/_config.yml` & `bio2zarr-0.0.8/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/docs/intro.md` & `bio2zarr-0.0.8/docs/intro.md`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/docs/logo.png` & `bio2zarr-0.0.8/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/validation-data/Makefile` & `bio2zarr-0.0.8/validation-data/Makefile`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/validation.py` & `bio2zarr-0.0.8/validation.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.6/vcf_generator.py` & `bio2zarr-0.0.8/vcf_generator.py`

 * *Files identical despite different names*

