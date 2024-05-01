# Comparing `tmp/aocstat-0.2.1.tar.gz` & `tmp/aocstat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aocstat-0.2.1.tar", max compression
+gzip compressed data, was "aocstat-0.2.2.tar", max compression
```

## Comparing `aocstat-0.2.1.tar` & `aocstat-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.1/LICENSE
--rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.1/aocstat/__init__.py
--rw-r--r--   0        0        0    13236 2024-04-30 23:58:10.851359 aocstat-0.2.1/aocstat/api.py
--rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.1/aocstat/config.py
--rw-r--r--   0        0        0     7054 2024-05-01 00:06:55.741258 aocstat-0.2.1/aocstat/format.py
--rw-r--r--   0        0        0     7248 2024-05-01 00:06:30.927924 aocstat-0.2.1/aocstat/main.py
--rw-r--r--   0        0        0      538 2024-05-01 00:07:20.121259 aocstat-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.2/LICENSE
+-rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.2/aocstat/__init__.py
+-rw-r--r--   0        0        0    13236 2024-04-30 23:58:10.851359 aocstat-0.2.2/aocstat/api.py
+-rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.2/aocstat/config.py
+-rw-r--r--   0        0        0     7054 2024-05-01 00:06:55.741258 aocstat-0.2.2/aocstat/format.py
+-rw-r--r--   0        0        0     7421 2024-05-01 00:13:49.321301 aocstat-0.2.2/aocstat/main.py
+-rw-r--r--   0        0        0      538 2024-05-01 00:14:09.701305 aocstat-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.2/PKG-INFO
```

### Comparing `aocstat-0.2.1/LICENSE` & `aocstat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.1/aocstat/api.py` & `aocstat-0.2.2/aocstat/api.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.1/aocstat/config.py` & `aocstat-0.2.2/aocstat/config.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.1/aocstat/format.py` & `aocstat-0.2.2/aocstat/format.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.1/aocstat/main.py` & `aocstat-0.2.2/aocstat/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import importlib.metadata
 import os
 import os.path as op
 import re
 import sys
 
 import aocstat.api as api
 import aocstat.config as config
@@ -22,14 +23,20 @@
         description="Interact with Advent of Code from your terminal."
     )
     parser.add_argument(
         "subcommand",
         choices=["lb", "purge", "config"],
         help="Subcommand to use. Available options are 'lb' (leaderboard), 'purge' (purge cache), or 'config' (view and edit config values).",
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version=importlib.metadata.version("aocstat"),
+    )
     parser.add_argument("subcommand args", nargs=argparse.REMAINDER)
     args = vars(parser.parse_args(args))
     if args["subcommand"] == "lb":
         _lb(args=args["subcommand args"])
     elif args["subcommand"] == "purge":
         _purge(args=args["subcommand args"])
     elif args["subcommand"] == "config":
```

### Comparing `aocstat-0.2.1/pyproject.toml` & `aocstat-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aocstat"
-version = "0.2.1"
+version = "0.2.2"
 description = "Command line tool for interacting with Advent of Code."
 authors = ["Hector Brown <hectorjbrown@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 selenium = "^4.7.2"
```

### Comparing `aocstat-0.2.1/PKG-INFO` & `aocstat-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aocstat
-Version: 0.2.1
+Version: 0.2.2
 Summary: Command line tool for interacting with Advent of Code.
 Author: Hector Brown
 Author-email: hectorjbrown@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

