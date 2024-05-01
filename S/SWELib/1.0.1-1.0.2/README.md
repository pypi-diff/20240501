# Comparing `tmp/SWELib-1.0.1.tar.gz` & `tmp/SWELib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SWELib-1.0.1.tar", last modified: Tue Apr 30 13:51:02 2024, max compression
+gzip compressed data, was "SWELib-1.0.2.tar", last modified: Tue Apr 30 13:58:07 2024, max compression
```

## Comparing `SWELib-1.0.1.tar` & `SWELib-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:51:02.651159 SWELib-1.0.1/
--rw-r--r--   0 felixfernando   (501) staff       (20)      342 2024-04-30 13:51:02.651037 SWELib-1.0.1/PKG-INFO
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:51:02.650154 SWELib-1.0.1/SWELib/
--rw-r--r--   0 felixfernando   (501) staff       (20)       22 2024-04-30 13:33:32.000000 SWELib-1.0.1/SWELib/__init__.py
--rw-r--r--   0 felixfernando   (501) staff       (20)    12384 2024-04-30 13:40:45.000000 SWELib-1.0.1/SWELib/main.py
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:51:02.650874 SWELib-1.0.1/SWELib.egg-info/
--rw-r--r--   0 felixfernando   (501) staff       (20)      342 2024-04-30 13:51:02.000000 SWELib-1.0.1/SWELib.egg-info/PKG-INFO
--rw-r--r--   0 felixfernando   (501) staff       (20)      191 2024-04-30 13:51:02.000000 SWELib-1.0.1/SWELib.egg-info/SOURCES.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)        1 2024-04-30 13:51:02.000000 SWELib-1.0.1/SWELib.egg-info/dependency_links.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)       32 2024-04-30 13:51:02.000000 SWELib-1.0.1/SWELib.egg-info/requires.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)        7 2024-04-30 13:51:02.000000 SWELib-1.0.1/SWELib.egg-info/top_level.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)       38 2024-04-30 13:51:02.651206 SWELib-1.0.1/setup.cfg
--rw-r--r--   0 felixfernando   (501) staff       (20)      353 2024-04-30 13:50:37.000000 SWELib-1.0.1/setup.py
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:58:07.898967 SWELib-1.0.2/
+-rw-r--r--   0 felixfernando   (501) staff       (20)      382 2024-04-30 13:58:07.898839 SWELib-1.0.2/PKG-INFO
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:58:07.897838 SWELib-1.0.2/SWELib/
+-rw-r--r--   0 felixfernando   (501) staff       (20)       22 2024-04-30 13:33:32.000000 SWELib-1.0.2/SWELib/__init__.py
+-rw-r--r--   0 felixfernando   (501) staff       (20)    12384 2024-04-30 13:40:45.000000 SWELib-1.0.2/SWELib/main.py
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-04-30 13:58:07.898678 SWELib-1.0.2/SWELib.egg-info/
+-rw-r--r--   0 felixfernando   (501) staff       (20)      382 2024-04-30 13:58:07.000000 SWELib-1.0.2/SWELib.egg-info/PKG-INFO
+-rw-r--r--   0 felixfernando   (501) staff       (20)      191 2024-04-30 13:58:07.000000 SWELib-1.0.2/SWELib.egg-info/SOURCES.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)        1 2024-04-30 13:58:07.000000 SWELib-1.0.2/SWELib.egg-info/dependency_links.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)       32 2024-04-30 13:58:07.000000 SWELib-1.0.2/SWELib.egg-info/requires.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)        7 2024-04-30 13:58:07.000000 SWELib-1.0.2/SWELib.egg-info/top_level.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)       38 2024-04-30 13:58:07.899011 SWELib-1.0.2/setup.cfg
+-rw-r--r--   0 felixfernando   (501) staff       (20)      354 2024-04-30 13:57:56.000000 SWELib-1.0.2/setup.py
```

### Comparing `SWELib-1.0.1/SWELib/main.py` & `SWELib-1.0.2/SWELib/main.py`

 * *Files identical despite different names*

