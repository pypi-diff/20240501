# Comparing `tmp/cellprofiler_library_nightly-5.0.0.dev65.tar.gz` & `tmp/cellprofiler_library_nightly-5.0.0.dev69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellprofiler_library_nightly-5.0.0.dev65.tar", last modified: Tue Apr 30 22:04:33 2024, max compression
+gzip compressed data, was "cellprofiler_library_nightly-5.0.0.dev69.tar", last modified: Wed May  1 00:10:04 2024, max compression
```

## Comparing `cellprofiler_library_nightly-5.0.0.dev65.tar` & `cellprofiler_library_nightly-5.0.0.dev69.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.922478 cellprofiler_library_nightly-5.0.0.dev65/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-30 22:04:33.922478 cellprofiler_library_nightly-5.0.0.dev65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.914478 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 22:04:32.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.918478 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/file_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19520 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16410 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/object_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25257 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.918478 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_closing.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_combineobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_enhanceedges.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_expandorshrinkobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_fillobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_measureimageoverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_medialaxis.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_medianfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_morphologicalskeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_opening.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_overlayobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_reducenoise.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_savecroppedobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_watershed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.918478 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/opts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/opts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/opts/measureimageoverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:33.922478 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-30 22:04:33.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-30 22:04:33.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:04:33.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 22:04:33.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 22:04:33.000000 cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 22:04:19.000000 cellprofiler_library_nightly-5.0.0.dev65/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-30 22:04:29.000000 cellprofiler_library_nightly-5.0.0.dev65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:04:33.922478 cellprofiler_library_nightly-5.0.0.dev65/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.648831 cellprofiler_library_nightly-5.0.0.dev69/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-01 00:10:04.648831 cellprofiler_library_nightly-5.0.0.dev69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.640831 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 00:10:03.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.644831 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/file_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19520 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16410 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/object_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25257 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.644831 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_closing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_combineobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_enhanceedges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_expandorshrinkobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_fillobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_measureimageoverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_medialaxis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_medianfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_morphologicalskeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_opening.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_overlayobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_reducenoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_savecroppedobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_watershed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.644831 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/opts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/opts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/opts/measureimageoverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:04.648831 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-01 00:10:03.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 00:10:04.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:10:03.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 00:10:03.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 00:10:03.000000 cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 00:09:42.000000 cellprofiler_library_nightly-5.0.0.dev69/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-01 00:09:58.000000 cellprofiler_library_nightly-5.0.0.dev69/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:10:04.648831 cellprofiler_library_nightly-5.0.0.dev69/setup.cfg
```

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/LICENSE` & `cellprofiler_library_nightly-5.0.0.dev69/LICENSE`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/PKG-INFO` & `cellprofiler_library_nightly-5.0.0.dev69/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cellprofiler-library-nightly
-Version: 5.0.0.dev65
-Summary: cellprofiler-lirary implements CellProfiler's image processing and mathematical code, and is usable as a standalone library
+Version: 5.0.0.dev69
+Summary: cellprofiler-library implements CellProfiler's image processing and mathematical code, and is usable as a standalone library
 Author: Anne Carpenter, Thouis (Ray) Jones, Lee Kamentsky, Vebjorn Ljosa, David Logan, Mark Bray, Madison Swain-Bowden, Allen Goodman, Claire McQuinn, Alice Lucas, Callum Tromans-Coia
 Author-email: Beth Cimini <bcimini@broadinstitute.org>, David Stirling <dstirling@glencoesoftware.com>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 Maintainer-email: Beth Cimini <bcimini@broadinstitute.org>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 License: The BSD 3-Clause License
         
         Copyright © 2003 - 2021 Broad Institute, Inc. All rights reserved.
         
@@ -78,10 +78,10 @@
 Requires-Dist: pyinstaller; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest~=7.4.1; extra == "test"
 
 # library
 
-This subpackage contains the code to build the `cellprofiler-library` package. It contains the image processing modules required by the [CellProfiler](cellprofiler.org) software. Both the [core](../core/) subpackage, and the [frontend](../../frontend/) rely on this subpackage. This package can be used in isolation, separate from the `cellprofiler` and `cellprofiler-core` packages to access CellProfiler's image processing functionality as a Python package.
+This subpackage contains the code to build the `cellprofiler-library` package. It contains the image processing modules required by the [CellProfiler](https://cellprofiler.org) software. Both the [core](https://github.com/CellProfiler/CellProfiler/tree/main/src/subpackages/core) subpackage, and the [frontend](https://github.com/CellProfiler/CellProfiler/tree/main/src/frontend) rely on this subpackage. This package can be used in isolation, separate from the `cellprofiler` and `cellprofiler-core` packages to access CellProfiler's image processing functionality as a Python package.
 
 It is currently a work under progress, and does not yet contain all or even most of CellProfiler's image processing capabilities.
```

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/file_processing.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/file_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/image_processing.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/measurement.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/object_processing.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/object_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/functions/segmentation.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/functions/segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/__init__.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_combineobjects.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_combineobjects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_enhanceedges.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_enhanceedges.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_expandorshrinkobjects.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_expandorshrinkobjects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_measureimageoverlap.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_measureimageoverlap.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_savecroppedobjects.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_savecroppedobjects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_threshold.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_threshold.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library/modules/_watershed.py` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library/modules/_watershed.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/PKG-INFO` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cellprofiler-library-nightly
-Version: 5.0.0.dev65
-Summary: cellprofiler-lirary implements CellProfiler's image processing and mathematical code, and is usable as a standalone library
+Version: 5.0.0.dev69
+Summary: cellprofiler-library implements CellProfiler's image processing and mathematical code, and is usable as a standalone library
 Author: Anne Carpenter, Thouis (Ray) Jones, Lee Kamentsky, Vebjorn Ljosa, David Logan, Mark Bray, Madison Swain-Bowden, Allen Goodman, Claire McQuinn, Alice Lucas, Callum Tromans-Coia
 Author-email: Beth Cimini <bcimini@broadinstitute.org>, David Stirling <dstirling@glencoesoftware.com>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 Maintainer-email: Beth Cimini <bcimini@broadinstitute.org>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 License: The BSD 3-Clause License
         
         Copyright © 2003 - 2021 Broad Institute, Inc. All rights reserved.
         
@@ -78,10 +78,10 @@
 Requires-Dist: pyinstaller; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest~=7.4.1; extra == "test"
 
 # library
 
-This subpackage contains the code to build the `cellprofiler-library` package. It contains the image processing modules required by the [CellProfiler](cellprofiler.org) software. Both the [core](../core/) subpackage, and the [frontend](../../frontend/) rely on this subpackage. This package can be used in isolation, separate from the `cellprofiler` and `cellprofiler-core` packages to access CellProfiler's image processing functionality as a Python package.
+This subpackage contains the code to build the `cellprofiler-library` package. It contains the image processing modules required by the [CellProfiler](https://cellprofiler.org) software. Both the [core](https://github.com/CellProfiler/CellProfiler/tree/main/src/subpackages/core) subpackage, and the [frontend](https://github.com/CellProfiler/CellProfiler/tree/main/src/frontend) rely on this subpackage. This package can be used in isolation, separate from the `cellprofiler` and `cellprofiler-core` packages to access CellProfiler's image processing functionality as a Python package.
 
 It is currently a work under progress, and does not yet contain all or even most of CellProfiler's image processing capabilities.
```

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/cellprofiler_library_nightly.egg-info/SOURCES.txt` & `cellprofiler_library_nightly-5.0.0.dev69/cellprofiler_library_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellprofiler_library_nightly-5.0.0.dev65/pyproject.toml` & `cellprofiler_library_nightly-5.0.0.dev69/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=64.0.0", "setuptools-scm>=8.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cellprofiler-library-nightly"
-description = "cellprofiler-lirary implements CellProfiler's image processing and mathematical code, and is usable as a standalone library"
+description = "cellprofiler-library implements CellProfiler's image processing and mathematical code, and is usable as a standalone library"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [ "computer vision", "image analysis", "biology", "cell", "cellprofiler",]
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Science/Research", "License :: OSI Approved :: BSD License", "Operating System :: OS Independent", "Programming Language :: Python :: 3.9", "Topic :: Scientific/Engineering :: Bio-Informatics", "Topic :: Scientific/Engineering :: Image Recognition", "Topic :: Scientific/Engineering :: Image Processing", "Topic :: Scientific/Engineering",]
 dependencies = [ "numpy~=1.24.4", "scikit-image~=0.20.0", "scipy>=1.9.1,<1.11", "mahotas~=1.4.13", "centrosome~=1.2.2", "matplotlib>=3.1.3,<4", "packaging>=20.0",]
 dynamic = [ "version",]
 [[project.authors]]
```

