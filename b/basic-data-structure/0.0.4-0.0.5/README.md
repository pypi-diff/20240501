# Comparing `tmp/basic_data_structure-0.0.4.tar.gz` & `tmp/basic_data_structure-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_data_structure-0.0.4.tar", max compression
+gzip compressed data, was "basic_data_structure-0.0.5.tar", max compression
```

## Comparing `basic_data_structure-0.0.4.tar` & `basic_data_structure-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-04-28 08:59:59.054530 basic_data_structure-0.0.4/LICENSE
--rw-r--r--   0        0        0      200 2024-04-28 12:46:15.312904 basic_data_structure-0.0.4/README.md
--rw-r--r--   0        0        0      171 2024-04-28 12:26:39.411611 basic_data_structure-0.0.4/basic_data_structure/__init__.py
--rw-r--r--   0        0        0       63 2024-04-28 12:08:02.577734 basic_data_structure-0.0.4/basic_data_structure/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055304 basic_data_structure-0.0.4/basic_data_structure/lists/__init__.py
--rw-r--r--   0        0        0      462 2024-04-28 12:07:08.784934 basic_data_structure-0.0.4/basic_data_structure/lists/linked_list.py
--rw-r--r--   0        0        0        0 2024-04-28 10:54:44.865814 basic_data_structure-0.0.4/basic_data_structure/stack/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-28 12:23:43.893829 basic_data_structure-0.0.4/basic_data_structure/stack/stack.py
--rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055652 basic_data_structure-0.0.4/basic_data_structure/trees/__init__.py
--rw-r--r--   0        0        0      611 2024-04-28 11:41:56.300001 basic_data_structure-0.0.4/basic_data_structure/trees/binary_tree.py
--rw-r--r--   0        0        0     1546 2024-04-28 11:00:27.880165 basic_data_structure-0.0.4/examples/binary_tree.py
--rw-r--r--   0        0        0      614 2024-04-28 11:00:27.880508 basic_data_structure-0.0.4/examples/linked_list.py
--rw-r--r--   0        0        0      669 2024-04-28 12:09:03.807986 basic_data_structure-0.0.4/examples/stack.py
--rw-r--r--   0        0        0     3052 2024-04-28 13:03:00.823024 basic_data_structure-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1009 1970-01-01 00:00:00.000000 basic_data_structure-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-28 08:59:59.054530 basic_data_structure-0.0.5/LICENSE
+-rw-r--r--   0        0        0    10047 2024-04-30 22:14:31.641597 basic_data_structure-0.0.5/README.md
+-rw-r--r--   0        0        0      226 2024-04-29 21:00:00.031231 basic_data_structure-0.0.5/basic_data_structure/__init__.py
+-rw-r--r--   0        0        0      264 2024-04-30 13:24:11.669087 basic_data_structure-0.0.5/basic_data_structure/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055304 basic_data_structure-0.0.5/basic_data_structure/list/__init__.py
+-rw-r--r--   0        0        0     1810 2024-04-29 21:02:08.921475 basic_data_structure-0.0.5/basic_data_structure/list/iterators.py
+-rw-r--r--   0        0        0     7537 2024-04-30 21:25:30.858355 basic_data_structure-0.0.5/basic_data_structure/list/linked_list.py
+-rw-r--r--   0        0        0      462 2024-04-28 12:07:08.784934 basic_data_structure-0.0.5/basic_data_structure/list/list_node.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:54:44.865814 basic_data_structure-0.0.5/basic_data_structure/stack/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-30 20:57:16.139682 basic_data_structure-0.0.5/basic_data_structure/stack/stack.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055652 basic_data_structure-0.0.5/basic_data_structure/tree/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-28 11:41:56.300001 basic_data_structure-0.0.5/basic_data_structure/tree/tree_node.py
+-rw-r--r--   0        0        0     3080 2024-04-30 22:05:08.355073 basic_data_structure-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 basic_data_structure-0.0.5/PKG-INFO
```

### Comparing `basic_data_structure-0.0.4/LICENSE` & `basic_data_structure-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.4/basic_data_structure/trees/binary_tree.py` & `basic_data_structure-0.0.5/basic_data_structure/tree/tree_node.py`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.4/pyproject.toml` & `basic_data_structure-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "basic-data-structure"
-version = "0.0.4"
+version = "0.0.5"
 description = "Implementation of basic sata structures in Python"
 authors = ["Mikhail Shagov <mishaga@me.com>"]
 readme = "README.md"
 license = "MIT"
-homepage = "https://github.com/mishaga/basic_data_structure"
 repository = "https://github.com/mishaga/basic_data_structure"
-keywords = ["data structure", "data structures"]
-include = ["examples", "tests"]
+keywords = ["data structure", "data structures", "python data structures", "basic data structures"]
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/mishaga/basic_data_structure/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 wemake-python-styleguide = "^0.19.2"
 flake8-pyproject = "^1.2.3"
+pytest = "^8.2.0"
+isort = "^5.13.2"
+
+
+[tool.isort]
+profile = "wemake"
 
 
 [tool.flake8]
 format = "wemake"
 max-complexity = "10"
 import-order-style = "pycharm"
 min-coverage-percents = "80"
```

