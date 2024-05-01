# Comparing `tmp/cudf_cu12-24.4.0.tar.gz` & `tmp/cudf_cu12-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudf_cu12-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "cudf_cu12-24.4.1.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cudf_cu12-24.4.0.tar` & `cudf_cu12-24.4.1.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     6022 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     6000 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf-cu12
-Version: 24.4.0
+Version: 24.4.1
 Summary: cuDF - GPU Dataframe
 Author: NVIDIA Corporation
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Requires-Dist: cupy-cuda12x>=12.0.0
 Requires-Dist: fsspec>=0.6.0
 Requires-Dist: numba>=0.57
 Requires-Dist: numpy<2.0a0,>=1.23
 Requires-Dist: nvtx>=0.2.1
 Requires-Dist: packaging
 Requires-Dist: pandas<2.2.2dev0,>=2.0
-Requires-Dist: protobuf<5,>=4.21
+Requires-Dist: protobuf<5,>=3.20
 Requires-Dist: pynvjitlink-cu12
 Requires-Dist: pyarrow<15.0.0a0,>=14.0.1
 Requires-Dist: rich
 Requires-Dist: rmm-cu12==24.4.*
 Requires-Dist: typing_extensions>=4.0.0
 Requires-Dist: cramjam; extra == "test"
 Requires-Dist: fastavro>=0.22.9; extra == "test"
@@ -47,15 +47,14 @@
 Requires-Dist: pytest-reportlog; extra == "pandas-tests"
 Requires-Dist: ipython; extra == "cudf-pandas-tests"
 Requires-Dist: openpyxl; extra == "cudf-pandas-tests"
 Provides-Extra: test
 Provides-Extra: pandas-tests
 Provides-Extra: cudf-pandas-tests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # <div align="left"><img src="img/rapids_logo.png" width="90px"/>&nbsp;cuDF - GPU DataFrames</div>
 
 ## 📢 cuDF can now be used as a no-code-change accelerator for pandas! To learn more, see [here](https://rapids.ai/cudf-pandas/)!
 
 cuDF (pronounced "KOO-dee-eff") is a GPU DataFrame library
 for loading, joining, aggregating, filtering, and otherwise
```

