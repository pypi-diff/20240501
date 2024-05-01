# Comparing `tmp/aiinitiate-0.1.0.tar.gz` & `tmp/aiinitiate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiinitiate-0.1.0.tar", max compression
+gzip compressed data, was "aiinitiate-0.1.1.tar", max compression
```

## Comparing `aiinitiate-0.1.0.tar` & `aiinitiate-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-05-01 08:06:39.740273 aiinitiate-0.1.0/aiinitiate/__init__.py
--rw-r--r--   0        0        0     1159 2024-05-01 08:48:43.743703 aiinitiate-0.1.0/aiinitiate/cli.py
--rw-r--r--   0        0        0     2607 2024-05-01 08:05:05.053797 aiinitiate-0.1.0/aiinitiate/sysinfo.py
--rw-r--r--   0        0        0      284 2024-05-01 08:49:32.423215 aiinitiate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 aiinitiate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-01 09:31:17.094915 aiinitiate-0.1.1/aiinitiate/__init__.py
+-rw-r--r--   0        0        0     1159 2024-05-01 08:48:43.743703 aiinitiate-0.1.1/aiinitiate/cli.py
+-rw-r--r--   0        0        0     2607 2024-05-01 08:05:05.053797 aiinitiate-0.1.1/aiinitiate/sysinfo.py
+-rw-r--r--   0        0        0      282 2024-05-01 09:31:17.098914 aiinitiate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 aiinitiate-0.1.1/PKG-INFO
```

### Comparing `aiinitiate-0.1.0/aiinitiate/cli.py` & `aiinitiate-0.1.1/aiinitiate/cli.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.0/aiinitiate/sysinfo.py` & `aiinitiate-0.1.1/aiinitiate/sysinfo.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.0/PKG-INFO` & `aiinitiate-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aiinitiate
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: CachCheng
 Author-email: tkggpdc2007@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: typer (==0.9.4)
 Description-Content-Type: text/markdown
```

