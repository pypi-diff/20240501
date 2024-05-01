# Comparing `tmp/aocstat-0.2.0.tar.gz` & `tmp/aocstat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aocstat-0.2.0.tar", max compression
+gzip compressed data, was "aocstat-0.2.1.tar", max compression
```

## Comparing `aocstat-0.2.0.tar` & `aocstat-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.0/LICENSE
--rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.0/aocstat/__init__.py
--rw-r--r--   0        0        0    13236 2024-04-30 23:58:10.851359 aocstat-0.2.0/aocstat/api.py
--rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.0/aocstat/config.py
--rw-r--r--   0        0        0     7055 2024-04-30 23:58:10.851359 aocstat-0.2.0/aocstat/format.py
--rw-r--r--   0        0        0     7248 2024-04-30 23:58:10.851359 aocstat-0.2.0/aocstat/main.py
--rw-r--r--   0        0        0      538 2024-04-30 23:58:41.238012 aocstat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.1/LICENSE
+-rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.1/aocstat/__init__.py
+-rw-r--r--   0        0        0    13236 2024-04-30 23:58:10.851359 aocstat-0.2.1/aocstat/api.py
+-rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.1/aocstat/config.py
+-rw-r--r--   0        0        0     7054 2024-05-01 00:06:55.741258 aocstat-0.2.1/aocstat/format.py
+-rw-r--r--   0        0        0     7248 2024-05-01 00:06:30.927924 aocstat-0.2.1/aocstat/main.py
+-rw-r--r--   0        0        0      538 2024-05-01 00:07:20.121259 aocstat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.1/PKG-INFO
```

### Comparing `aocstat-0.2.0/LICENSE` & `aocstat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.0/aocstat/api.py` & `aocstat-0.2.1/aocstat/api.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.0/aocstat/config.py` & `aocstat-0.2.1/aocstat/config.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.0/aocstat/format.py` & `aocstat-0.2.1/aocstat/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             elif day <= api.get_most_recent_day(int(lb["event"])):
                 res += _colour("* ", "bright_grey", ansi_on, alt_text=". ")
             else:
                 res += "  "
         res += "  "
         # add names
         res += (
-            +_colour(
+            _colour(
                 lb["members"][member]["name"],
                 "bright_cyan" if user_id == int(member) else "bright_white",
                 ansi_on,
             )
             + "\n"
         )
```

### Comparing `aocstat-0.2.0/aocstat/main.py` & `aocstat-0.2.1/aocstat/main.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.0/pyproject.toml` & `aocstat-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aocstat"
-version = "0.2.0"
+version = "0.2.1"
 description = "Command line tool for interacting with Advent of Code."
 authors = ["Hector Brown <hectorjbrown@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 selenium = "^4.7.2"
```

### Comparing `aocstat-0.2.0/PKG-INFO` & `aocstat-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aocstat
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command line tool for interacting with Advent of Code.
 Author: Hector Brown
 Author-email: hectorjbrown@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

