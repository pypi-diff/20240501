# Comparing `tmp/zyx-0.0.1.tar.gz` & `tmp/zyx-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.1.tar", last modified: Sat Apr 27 07:01:11 2024, max compression
+gzip compressed data, was "zyx-0.0.10.tar", last modified: Wed May  1 02:19:43 2024, max compression
```

## Comparing `zyx-0.0.1.tar` & `zyx-0.0.10.tar`

### file list

```diff
@@ -1,11 +1,37 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-04-27 07:01:11.772577 zyx-0.0.1/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       47 2024-04-27 07:01:11.771577 zyx-0.0.1/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-04-27 07:01:11.772577 zyx-0.0.1/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-04-27 07:00:55.000000 zyx-0.0.1/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-04-27 07:01:11.770577 zyx-0.0.1/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-04-27 06:53:47.000000 zyx-0.0.1/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-04-27 07:01:11.771577 zyx-0.0.1/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       47 2024-04-27 07:01:11.000000 zyx-0.0.1/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      132 2024-04-27 07:01:11.000000 zyx-0.0.1/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-04-27 07:01:11.000000 zyx-0.0.1/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-04-27 07:01:11.000000 zyx-0.0.1/zyx.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.368854 zyx-0.0.10/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:19:43.368854 zyx-0.0.10/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       58 2024-04-30 22:57:31.000000 zyx-0.0.10/README.md
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 02:19:43.368854 zyx-0.0.10/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      918 2024-05-01 01:52:47.000000 zyx-0.0.10/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.363854 zyx-0.0.10/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.364854 zyx-0.0.10/src/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.10/src/zyx/__cli__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      145 2024-05-01 02:17:07.000000 zyx-0.0.10/src/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.366854 zyx-0.0.10/src/zyx/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.10/src/zyx/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.10/src/zyx/core/chat.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.10/src/zyx/core/input.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.10/src/zyx/core/lightning.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.10/src/zyx/core/loaders.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2173 2024-05-01 01:31:23.000000 zyx-0.0.10/src/zyx/core/print.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.10/src/zyx/core/validate_path.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.10/src/zyx/core/validate_type.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.366854 zyx-0.0.10/src/zyx/functions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:12:32.000000 zyx-0.0.10/src/zyx/functions/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.10/src/zyx/functions/create_id.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.10/src/zyx/functions/generate_name.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.10/src/zyx/functions/get_system_info.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx/jupyter/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.10/src/zyx/jupyter/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.10/src/zyx/jupyter/tailwind.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx/text/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.10/src/zyx/text/__chunker__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.10/src/zyx/text/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.10/src/zyx/text/__read_doc__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       96 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/top_level.txt
```

