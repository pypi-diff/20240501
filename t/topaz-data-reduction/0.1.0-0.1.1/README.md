# Comparing `tmp/topaz_data_reduction-0.1.0.tar.gz` & `tmp/topaz_data_reduction-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topaz_data_reduction-0.1.0.tar", last modified: Wed May  1 15:00:42 2024, max compression
+gzip compressed data, was "topaz_data_reduction-0.1.1.tar", last modified: Wed May  1 15:15:16 2024, max compression
```

## Comparing `topaz_data_reduction-0.1.0.tar` & `topaz_data_reduction-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:00:42.888175 topaz_data_reduction-0.1.0/
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      226 2024-05-01 15:00:42.888050 topaz_data_reduction-0.1.0/PKG-INFO
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)     6232 2024-04-29 19:00:54.000000 topaz_data_reduction-0.1.0/README.md
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       38 2024-05-01 15:00:42.888220 topaz_data_reduction-0.1.0/setup.cfg
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      455 2024-05-01 15:00:14.000000 topaz_data_reduction-0.1.0/setup.py
-drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:00:42.887153 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      226 2024-05-01 15:00:42.000000 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/PKG-INFO
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      316 2024-05-01 15:00:42.000000 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/SOURCES.txt
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)        1 2024-05-01 15:00:42.000000 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/dependency_links.txt
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       44 2024-05-01 15:00:42.000000 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/requires.txt
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       10 2024-05-01 15:00:42.000000 topaz_data_reduction-0.1.0/topaz_data_reduction.egg-info/top_level.txt
-drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:00:42.887781 topaz_data_reduction-0.1.0/utilities/
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       83 2024-05-01 14:56:48.000000 topaz_data_reduction-0.1.0/utilities/__init__.py
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      149 2024-05-01 14:58:04.000000 topaz_data_reduction-0.1.0/utilities/data_processing.py
--rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      321 2024-05-01 14:57:15.000000 topaz_data_reduction-0.1.0/utilities/job_management.py
+drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:15:16.040530 topaz_data_reduction-0.1.1/
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      226 2024-05-01 15:15:16.040403 topaz_data_reduction-0.1.1/PKG-INFO
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)     6232 2024-04-29 19:00:54.000000 topaz_data_reduction-0.1.1/README.md
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       38 2024-05-01 15:15:16.040573 topaz_data_reduction-0.1.1/setup.cfg
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      396 2024-05-01 15:14:58.000000 topaz_data_reduction-0.1.1/setup.py
+drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:15:16.039543 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      226 2024-05-01 15:15:15.000000 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/PKG-INFO
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      316 2024-05-01 15:15:16.000000 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/SOURCES.txt
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)        1 2024-05-01 15:15:15.000000 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/dependency_links.txt
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       18 2024-05-01 15:15:15.000000 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/requires.txt
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       10 2024-05-01 15:15:15.000000 topaz_data_reduction-0.1.1/topaz_data_reduction.egg-info/top_level.txt
+drwxr-xr-x   0 owd      (598642127) ORNL\Domain Users (1551083765)        0 2024-05-01 15:15:16.040132 topaz_data_reduction-0.1.1/utilities/
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)       83 2024-05-01 14:56:48.000000 topaz_data_reduction-0.1.1/utilities/__init__.py
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      149 2024-05-01 14:58:04.000000 topaz_data_reduction-0.1.1/utilities/data_processing.py
+-rw-r--r--   0 owd      (598642127) ORNL\Domain Users (1551083765)      321 2024-05-01 14:57:15.000000 topaz_data_reduction-0.1.1/utilities/job_management.py
```

### Comparing `topaz_data_reduction-0.1.0/README.md` & `topaz_data_reduction-0.1.1/README.md`

 * *Files identical despite different names*

