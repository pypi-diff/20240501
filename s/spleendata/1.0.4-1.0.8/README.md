# Comparing `tmp/spleendata-1.0.4.tar.gz` & `tmp/spleendata-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleendata-1.0.4.tar", last modified: Mon Apr 22 18:11:53 2024, max compression
+gzip compressed data, was "spleendata-1.0.8.tar", last modified: Mon Apr 22 18:29:25 2024, max compression
```

## Comparing `spleendata-1.0.4.tar` & `spleendata-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 18:11:53.159369 spleendata-1.0.4/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-22 17:46:01.000000 spleendata-1.0.4/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      521 2024-04-22 18:11:53.159369 spleendata-1.0.4/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4308 2024-04-22 17:46:01.000000 spleendata-1.0.4/README.md
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-04-22 18:11:53.159369 spleendata-1.0.4/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1437 2024-04-22 17:46:01.000000 spleendata-1.0.4/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 18:11:53.159369 spleendata-1.0.4/spleendata.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      521 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      246 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       47 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       40 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       11 2024-04-22 18:11:53.000000 spleendata-1.0.4/spleendata.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3941 2024-04-22 18:10:41.000000 spleendata-1.0.4/spleendata.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 18:29:25.324593 spleendata-1.0.8/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-22 17:46:01.000000 spleendata-1.0.8/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5197 2024-04-22 18:29:25.324593 spleendata-1.0.8/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4308 2024-04-22 17:46:01.000000 spleendata-1.0.8/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4675 2024-04-22 18:29:23.000000 spleendata-1.0.8/README.rst
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-04-22 18:29:25.324593 spleendata-1.0.8/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1465 2024-04-22 18:24:52.000000 spleendata-1.0.8/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-22 18:29:25.324593 spleendata-1.0.8/spleendata.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5197 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      257 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       47 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       40 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       11 2024-04-22 18:29:25.000000 spleendata-1.0.8/spleendata.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3941 2024-04-22 18:28:17.000000 spleendata-1.0.8/spleendata.py
```

### Comparing `spleendata-1.0.4/LICENSE` & `spleendata-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spleendata-1.0.4/README.md` & `spleendata-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spleendata-1.0.4/spleendata.py` & `spleendata-1.0.8/spleendata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 from argparse import ArgumentParser, Namespace, ArgumentDefaultsHelpFormatter
 
 from chris_plugin import chris_plugin, PathMapper
 
 from monai.apps.utils import download_and_extract
 
-__version__ = "1.0.4"
+__version__ = "1.0.8"
 
 DISPLAY_TITLE = r"""
        _                  _                     _       _
       | |                | |                   | |     | |
  _ __ | |______ ___ _ __ | | ___  ___ _ __   __| | __ _| |_ __ _
 | '_ \| |______/ __| '_ \| |/ _ \/ _ \ '_ \ / _` |/ _` | __/ _` |
 | |_) | |      \__ \ |_) | |  __/  __/ | | | (_| | (_| | || (_| |
```

