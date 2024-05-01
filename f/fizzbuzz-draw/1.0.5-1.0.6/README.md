# Comparing `tmp/fizzbuzz_draw-1.0.5.tar.gz` & `tmp/fizzbuzz_draw-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fizzbuzz_draw-1.0.5.tar", last modified: Wed May  1 12:17:06 2024, max compression
+gzip compressed data, was "fizzbuzz_draw-1.0.6.tar", last modified: Wed May  1 12:39:36 2024, max compression
```

## Comparing `fizzbuzz_draw-1.0.5.tar` & `fizzbuzz_draw-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:17:06.291185 fizzbuzz_draw-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:17:06.291185 fizzbuzz_draw-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:17:06.291185 fizzbuzz_draw-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:17:06.287186 fizzbuzz_draw-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:17:06.287186 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/nested_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/setup_mg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:17:06.287186 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:17:06.000000 fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:17:06.287186 fizzbuzz_draw-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-01 12:15:59.000000 fizzbuzz_draw-1.0.5/tests/test_flask_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:36.871672 fizzbuzz_draw-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/nested_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/setup_mg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:39:36.000000 fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:39:36.875673 fizzbuzz_draw-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-01 12:39:03.000000 fizzbuzz_draw-1.0.6/tests/test_flask_webapp.py
```

### Comparing `fizzbuzz_draw-1.0.5/LICENSE` & `fizzbuzz_draw-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.5/PKG-INFO` & `fizzbuzz_draw-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzbuzz-draw
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fizzbuzz draw lolz
 Author-email: Dhiyaa Al Jorf <da2863@nyu.edu>, Firas Darwish <fbd2014@nyu.edu>, Shubhi Upadhyay <su2132@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fizzbuzz_draw-1.0.5/pyproject.toml` & `fizzbuzz_draw-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fizzbuzz-draw"
 description = "Fizzbuzz draw lolz"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Dhiyaa Al Jorf", email= "da2863@nyu.edu" },
   { name= "Firas Darwish", email= "fbd2014@nyu.edu" },
   { name= "Shubhi Upadhyay", email= "su2132@nyu.edu"}
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/app.py` & `fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/app.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/nested_collections.py` & `fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/nested_collections.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.5/src/fizzbuzz_draw/setup_mg.py` & `fizzbuzz_draw-1.0.6/src/fizzbuzz_draw/setup_mg.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.5/src/fizzbuzz_draw.egg-info/PKG-INFO` & `fizzbuzz_draw-1.0.6/src/fizzbuzz_draw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzbuzz-draw
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fizzbuzz draw lolz
 Author-email: Dhiyaa Al Jorf <da2863@nyu.edu>, Firas Darwish <fbd2014@nyu.edu>, Shubhi Upadhyay <su2132@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fizzbuzz_draw-1.0.5/tests/test_flask_webapp.py` & `fizzbuzz_draw-1.0.6/tests/test_flask_webapp.py`

 * *Files identical despite different names*
