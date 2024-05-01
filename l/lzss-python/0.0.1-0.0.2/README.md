# Comparing `tmp/lzss-python-0.0.1.tar.gz` & `tmp/lzss-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzss-python-0.0.1.tar", last modified: Wed May  1 13:28:32 2024, max compression
+gzip compressed data, was "lzss-python-0.0.2.tar", last modified: Wed May  1 14:31:43 2024, max compression
```

## Comparing `lzss-python-0.0.1.tar` & `lzss-python-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2024-05-01 12:37:47.433589 lzss-python-0.0.1/LICENSE
--rw-r--r--   0        0        0      193 2022-05-22 02:35:32.308390 lzss-python-0.0.1/README.md
--rw-r--r--   0        0        0      141 2024-05-01 12:38:19.606495 lzss-python-0.0.1/lzss/__init__.py
--rw-r--r--   0        0        0     2854 2024-05-01 13:02:49.836853 lzss-python-0.0.1/lzss/lzss.py
--rw-r--r--   0        0        0      122 2024-05-01 13:18:00.977194 lzss-python-0.0.1/lzss/version.py
--rw-r--r--   0        0        0     1170 2024-05-01 13:25:42.979697 lzss-python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      990 2022-05-21 22:39:44.962298 lzss-python-0.0.1/tests/test_lzss.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 lzss-python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-01 14:27:34.324744 lzss-python-0.0.2/LICENSE
+-rw-r--r--   0        0        0      494 2024-05-01 14:31:36.556872 lzss-python-0.0.2/README.md
+-rw-r--r--   0        0        0      141 2024-05-01 14:27:34.324744 lzss-python-0.0.2/lzss/__init__.py
+-rw-r--r--   0        0        0     2854 2024-05-01 14:27:34.324744 lzss-python-0.0.2/lzss/lzss.py
+-rw-r--r--   0        0        0      122 2024-05-01 14:31:36.556872 lzss-python-0.0.2/lzss/version.py
+-rw-r--r--   0        0        0     1170 2024-05-01 14:27:34.324744 lzss-python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      990 2022-05-21 22:39:44.962298 lzss-python-0.0.2/tests/test_lzss.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 lzss-python-0.0.2/PKG-INFO
```

### Comparing `lzss-python-0.0.1/LICENSE` & `lzss-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lzss-python-0.0.1/lzss/lzss.py` & `lzss-python-0.0.2/lzss/lzss.py`

 * *Files identical despite different names*

### Comparing `lzss-python-0.0.1/pyproject.toml` & `lzss-python-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     { name = "Tim Cogan" },
 ]
 dependencies = [
     "bitarray",
 ]
 readme = "README.md"
 dynamic = []
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "MIT"
 
 [tool.autoflake]
 remove-all-unused-imports = true
 remove-unused-variables = true
```

### Comparing `lzss-python-0.0.1/tests/test_lzss.py` & `lzss-python-0.0.2/tests/test_lzss.py`

 * *Files identical despite different names*

