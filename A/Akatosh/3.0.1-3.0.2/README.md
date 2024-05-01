# Comparing `tmp/akatosh-3.0.1.tar.gz` & `tmp/akatosh-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.1.tar", max compression
+gzip compressed data, was "akatosh-3.0.2.tar", max compression
```

## Comparing `akatosh-3.0.1.tar` & `akatosh-3.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      546 2024-05-01 01:03:37.389203 akatosh-3.0.1/Akatosh/__init__.py
--rw-r--r--   0        0        0     4911 2024-05-01 01:03:37.390209 akatosh-3.0.1/Akatosh/entity.py
--rw-r--r--   0        0        0     6051 2024-05-01 03:23:36.963728 akatosh-3.0.1/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.1/Akatosh/resource.py
--rw-r--r--   0        0        0     7286 2024-05-01 03:19:13.357671 akatosh-3.0.1/Akatosh/universe.py
--rw-r--r--   0        0        0      322 2024-05-01 03:32:45.315243 akatosh-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.1/README.md
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 akatosh-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      546 2024-05-01 01:03:37.389203 akatosh-3.0.2/Akatosh/__init__.py
+-rw-r--r--   0        0        0     4911 2024-05-01 01:03:37.390209 akatosh-3.0.2/Akatosh/entity.py
+-rw-r--r--   0        0        0     6051 2024-05-01 03:23:36.963728 akatosh-3.0.2/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.2/Akatosh/resource.py
+-rw-r--r--   0        0        0     7286 2024-05-01 03:19:13.357671 akatosh-3.0.2/Akatosh/universe.py
+-rw-r--r--   0        0        0      321 2024-05-01 05:15:06.777438 akatosh-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.2/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.2/PKG-INFO
```

### Comparing `akatosh-3.0.1/Akatosh/__init__.py` & `akatosh-3.0.2/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.1/Akatosh/entity.py` & `akatosh-3.0.2/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.1/Akatosh/event.py` & `akatosh-3.0.2/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.1/Akatosh/resource.py` & `akatosh-3.0.2/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.1/Akatosh/universe.py` & `akatosh-3.0.2/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.1/README.md` & `akatosh-3.0.2/README.md`

 * *Files identical despite different names*

