# Comparing `tmp/sailing_log-0.4.2.tar.gz` & `tmp/sailing_log-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sailing_log-0.4.2.tar", last modified: Mon Feb 26 14:20:03 2024, max compression
+gzip compressed data, was "sailing_log-0.4.3.tar", last modified: Wed May  1 16:11:14 2024, max compression
```

## Comparing `sailing_log-0.4.2.tar` & `sailing_log-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-02-26 14:20:03.946337 sailing_log-0.4.2/
--rw-r--r--   0 julian    (1000) julian    (1000)    34596 2024-02-26 10:59:06.000000 sailing_log-0.4.2/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)      791 2024-02-26 14:20:03.946337 sailing_log-0.4.2/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      103 2024-02-26 10:59:06.000000 sailing_log-0.4.2/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)      829 2024-02-26 12:16:38.000000 sailing_log-0.4.2/pyproject.toml
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-02-26 14:20:03.942337 sailing_log-0.4.2/sailing_log/
--rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-02-26 12:09:04.000000 sailing_log-0.4.2/sailing_log/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2774 2024-02-26 12:09:53.000000 sailing_log-0.4.2/sailing_log/logger.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-02-26 14:20:03.942337 sailing_log-0.4.2/sailing_log.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)      791 2024-02-26 14:20:03.000000 sailing_log-0.4.2/sailing_log.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      252 2024-02-26 14:20:03.000000 sailing_log-0.4.2/sailing_log.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-02-26 14:20:03.000000 sailing_log-0.4.2/sailing_log.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        8 2024-02-26 14:20:03.000000 sailing_log-0.4.2/sailing_log.egg-info/requires.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       12 2024-02-26 14:20:03.000000 sailing_log-0.4.2/sailing_log.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-02-26 14:20:03.946337 sailing_log-0.4.2/setup.cfg
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-05-01 16:11:14.905884 sailing_log-0.4.3/
+-rw-r--r--   0 julian    (1000) julian    (1000)    34596 2024-05-01 15:47:07.000000 sailing_log-0.4.3/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)     1823 2024-05-01 16:11:14.905884 sailing_log-0.4.3/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1136 2024-05-01 15:47:07.000000 sailing_log-0.4.3/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)      829 2024-05-01 16:11:12.000000 sailing_log-0.4.3/pyproject.toml
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-05-01 16:11:14.905884 sailing_log-0.4.3/sailing_log/
+-rw-r--r--   0 julian    (1000) julian    (1000)       32 2024-05-01 15:49:13.000000 sailing_log-0.4.3/sailing_log/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2774 2024-05-01 15:47:07.000000 sailing_log-0.4.3/sailing_log/logger.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-05-01 16:11:14.905884 sailing_log-0.4.3/sailing_log.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1823 2024-05-01 16:11:14.000000 sailing_log-0.4.3/sailing_log.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      252 2024-05-01 16:11:14.000000 sailing_log-0.4.3/sailing_log.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-05-01 16:11:14.000000 sailing_log-0.4.3/sailing_log.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        8 2024-05-01 16:11:14.000000 sailing_log-0.4.3/sailing_log.egg-info/requires.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       12 2024-05-01 16:11:14.000000 sailing_log-0.4.3/sailing_log.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-05-01 16:11:14.905884 sailing_log-0.4.3/setup.cfg
```

### Comparing `sailing_log-0.4.2/LICENSE` & `sailing_log-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sailing_log-0.4.2/pyproject.toml` & `sailing_log-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sailing_log"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Simple logger class for usage in data streams related to deep learning, reinforcement learning, and high performance computing"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sailing_log-0.4.2/sailing_log/logger.py` & `sailing_log-0.4.3/sailing_log/logger.py`

 * *Files identical despite different names*

