# Comparing `tmp/sufi-1.0.tar.gz` & `tmp/sufi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufi-1.0.tar", last modified: Tue Apr 30 20:41:28 2024, max compression
+gzip compressed data, was "sufi-1.0.1.tar", last modified: Tue Apr 30 23:24:22 2024, max compression
```

## Comparing `sufi-1.0.tar` & `sufi-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 20:41:28.284288 sufi-1.0/
--rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-04-30 20:35:03.000000 sufi-1.0/LICENCE
--rw-r--r--   0 sunny      (501) staff       (20)      475 2024-04-30 20:41:28.284088 sufi-1.0/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      170 2024-04-30 20:31:50.000000 sufi-1.0/README.md
--rw-r--r--   0 sunny      (501) staff       (20)       38 2024-04-30 20:41:28.284348 sufi-1.0/setup.cfg
--rw-r--r--   0 sunny      (501) staff       (20)      518 2024-04-30 20:39:11.000000 sufi-1.0/setup.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 20:41:28.282811 sufi-1.0/sufi/
--rw-r--r--   0 sunny      (501) staff       (20)        2 2024-04-30 20:26:41.000000 sufi-1.0/sufi/__init__.py
--rw-r--r--   0 sunny      (501) staff       (20)     1926 2024-04-30 17:37:04.000000 sufi-1.0/sufi/filters.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 20:41:28.283869 sufi-1.0/sufi.egg-info/
--rw-r--r--   0 sunny      (501) staff       (20)      475 2024-04-30 20:41:28.000000 sufi-1.0/sufi.egg-info/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      198 2024-04-30 20:41:28.000000 sufi-1.0/sufi.egg-info/SOURCES.txt
--rw-r--r--   0 sunny      (501) staff       (20)        1 2024-04-30 20:41:28.000000 sufi-1.0/sufi.egg-info/dependency_links.txt
--rw-r--r--   0 sunny      (501) staff       (20)       28 2024-04-30 20:41:28.000000 sufi-1.0/sufi.egg-info/requires.txt
--rw-r--r--   0 sunny      (501) staff       (20)        5 2024-04-30 20:41:28.000000 sufi-1.0/sufi.egg-info/top_level.txt
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 23:24:22.606910 sufi-1.0.1/
+-rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-04-30 20:35:03.000000 sufi-1.0.1/LICENCE
+-rw-r--r--   0 sunny      (501) staff       (20)      477 2024-04-30 23:24:22.606727 sufi-1.0.1/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      170 2024-04-30 20:31:50.000000 sufi-1.0.1/README.md
+-rw-r--r--   0 sunny      (501) staff       (20)       38 2024-04-30 23:24:22.606969 sufi-1.0.1/setup.cfg
+-rw-r--r--   0 sunny      (501) staff       (20)      520 2024-04-30 23:20:59.000000 sufi-1.0.1/setup.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 23:24:22.605494 sufi-1.0.1/sufi/
+-rw-r--r--   0 sunny      (501) staff       (20)        2 2024-04-30 20:26:41.000000 sufi-1.0.1/sufi/__init__.py
+-rw-r--r--   0 sunny      (501) staff       (20)     1926 2024-04-30 17:37:04.000000 sufi-1.0.1/sufi/filters.py
+-rw-r--r--   0 sunny      (501) staff       (20)     2532 2024-04-30 23:07:19.000000 sufi-1.0.1/sufi/utility.py
+-rw-r--r--   0 sunny      (501) staff       (20)     1771 2024-04-30 23:20:36.000000 sufi-1.0.1/sufi/videoProcessing.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-04-30 23:24:22.606504 sufi-1.0.1/sufi.egg-info/
+-rw-r--r--   0 sunny      (501) staff       (20)      477 2024-04-30 23:24:22.000000 sufi-1.0.1/sufi.egg-info/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      238 2024-04-30 23:24:22.000000 sufi-1.0.1/sufi.egg-info/SOURCES.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        1 2024-04-30 23:24:22.000000 sufi-1.0.1/sufi.egg-info/dependency_links.txt
+-rw-r--r--   0 sunny      (501) staff       (20)       28 2024-04-30 23:24:22.000000 sufi-1.0.1/sufi.egg-info/requires.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        5 2024-04-30 23:24:22.000000 sufi-1.0.1/sufi.egg-info/top_level.txt
```

### Comparing `sufi-1.0/LICENCE` & `sufi-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `sufi-1.0/setup.py` & `sufi-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	description = fh.read()
 
 setuptools.setup(
 	name="sufi",
-	version="1.0",
+	version="1.0.1",
 	author="sunny kumar",
 	author_email="sunnykumar1516@gmail.com",
 	packages=["sufi"],
 	description="apply different types of filters on image",
 	long_description=description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/sunnykumar1516/sufi",
```

### Comparing `sufi-1.0/sufi/filters.py` & `sufi-1.0.1/sufi/filters.py`

 * *Files identical despite different names*

