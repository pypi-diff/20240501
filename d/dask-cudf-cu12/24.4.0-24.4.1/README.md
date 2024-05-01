# Comparing `tmp/dask_cudf_cu12-24.4.0.tar.gz` & `tmp/dask_cudf_cu12-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_cudf_cu12-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "dask_cudf_cu12-24.4.1.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `dask_cudf_cu12-24.4.0.tar` & `dask_cudf_cu12-24.4.1.tar`

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cudf-cu12
-Version: 24.4.0
+Version: 24.4.1
 Summary: Utilities for Dask and cuDF interactions
 Author: NVIDIA Corporation
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/rapidsai/cudf
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
```

