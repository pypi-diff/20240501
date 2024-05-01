# Comparing `tmp/fizzbuzz_draw-1.0.7.tar.gz` & `tmp/fizzbuzz_draw-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fizzbuzz_draw-1.0.7.tar", last modified: Wed May  1 12:53:12 2024, max compression
+gzip compressed data, was "fizzbuzz_draw-1.0.8.tar", last modified: Wed May  1 13:37:33 2024, max compression
```

## Comparing `fizzbuzz_draw-1.0.7.tar` & `fizzbuzz_draw-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:53:12.939492 fizzbuzz_draw-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/nested_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/setup_mg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:53:12.000000 fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:53:12.943492 fizzbuzz_draw-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-01 12:52:43.000000 fizzbuzz_draw-1.0.7/tests/test_flask_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:37:33.349555 fizzbuzz_draw-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 13:37:33.349555 fizzbuzz_draw-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:37:33.349555 fizzbuzz_draw-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:37:33.345555 fizzbuzz_draw-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:37:33.345555 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/nested_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/setup_mg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:37:33.345555 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41784 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:37:33.000000 fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:37:33.345555 fizzbuzz_draw-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-01 13:36:57.000000 fizzbuzz_draw-1.0.8/tests/test_flask_webapp.py
```

### Comparing `fizzbuzz_draw-1.0.7/LICENSE` & `fizzbuzz_draw-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.7/PKG-INFO` & `fizzbuzz_draw-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzbuzz-draw
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fizzbuzz draw lolz
 Author-email: Dhiyaa Al Jorf <da2863@nyu.edu>, Firas Darwish <fbd2014@nyu.edu>, Shubhi Upadhyay <su2132@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fizzbuzz_draw-1.0.7/pyproject.toml` & `fizzbuzz_draw-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fizzbuzz-draw"
 description = "Fizzbuzz draw lolz"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Dhiyaa Al Jorf", email= "da2863@nyu.edu" },
   { name= "Firas Darwish", email= "fbd2014@nyu.edu" },
   { name= "Shubhi Upadhyay", email= "su2132@nyu.edu"}
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/app.py` & `fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/app.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/nested_collections.py` & `fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/nested_collections.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.7/src/fizzbuzz_draw/setup_mg.py` & `fizzbuzz_draw-1.0.8/src/fizzbuzz_draw/setup_mg.py`

 * *Files identical despite different names*

### Comparing `fizzbuzz_draw-1.0.7/src/fizzbuzz_draw.egg-info/PKG-INFO` & `fizzbuzz_draw-1.0.8/src/fizzbuzz_draw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzbuzz-draw
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fizzbuzz draw lolz
 Author-email: Dhiyaa Al Jorf <da2863@nyu.edu>, Firas Darwish <fbd2014@nyu.edu>, Shubhi Upadhyay <su2132@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fizzbuzz_draw-1.0.7/tests/test_flask_webapp.py` & `fizzbuzz_draw-1.0.8/tests/test_flask_webapp.py`

 * *Files identical despite different names*

