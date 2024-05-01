# Comparing `tmp/librelingo_fakes-3.2.0.tar.gz` & `tmp/librelingo_fakes-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librelingo_fakes-3.2.0.tar", max compression
+gzip compressed data, was "librelingo_fakes-3.2.1.tar", last modified: Wed May  1 16:17:09 2024, max compression
```

## Comparing `librelingo_fakes-3.2.0.tar` & `librelingo_fakes-3.2.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1138 2022-11-15 21:28:53.264930 librelingo_fakes-3.2.0/README.md
--rw-r--r--   0        0        0       98 2022-11-15 21:28:53.264930 librelingo_fakes-3.2.0/librelingo_fakes/__init__.py
--rw-r--r--   0        0        0     7592 2023-06-10 11:57:31.714229 librelingo_fakes-3.2.0/librelingo_fakes/fakes.py
--rw-r--r--   0        0        0      477 2023-06-10 12:54:59.251359 librelingo_fakes-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 librelingo_fakes-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1138 2023-12-27 12:41:42.079019 librelingo_fakes-3.2.1/README.md
+-rw-r--r--   0        0        0      445 2024-05-01 16:17:09.811411 librelingo_fakes-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-04-30 08:02:28.240291 librelingo_fakes-3.2.1/src/librelingo_fakes/__init__.py
+-rw-r--r--   0        0        0     7592 2024-04-30 08:02:43.005452 librelingo_fakes-3.2.1/src/librelingo_fakes/fakes.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:55:30.107705 librelingo_fakes-3.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 librelingo_fakes-3.2.1/PKG-INFO
```

### Comparing `librelingo_fakes-3.2.0/README.md` & `librelingo_fakes-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `librelingo_fakes-3.2.0/librelingo_fakes/fakes.py` & `librelingo_fakes-3.2.1/src/librelingo_fakes/fakes.py`

 * *Files identical despite different names*

