# Comparing `tmp/json_schema_filter-0.2.0.tar.gz` & `tmp/json_schema_filter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_filter-0.2.0.tar", max compression
+gzip compressed data, was "json_schema_filter-0.3.0.tar", max compression
```

## Comparing `json_schema_filter-0.2.0.tar` & `json_schema_filter-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-12-25 22:03:17.193575 json_schema_filter-0.2.0/LICENSE
--rw-r--r--   0        0        0     1036 2023-12-30 05:50:46.703231 json_schema_filter-0.2.0/README.md
--rw-r--r--   0        0        0       69 2023-12-30 04:00:39.896921 json_schema_filter-0.2.0/json_schema_filter/__init__.py
--rw-r--r--   0        0        0     2051 2023-12-31 04:42:41.204359 json_schema_filter-0.2.0/json_schema_filter/filter.py
--rw-r--r--   0        0        0      602 2023-12-30 04:05:13.025776 json_schema_filter-0.2.0/json_schema_filter/filter_validator/__init__.py
--rw-r--r--   0        0        0      464 2023-12-30 04:05:13.027310 json_schema_filter-0.2.0/json_schema_filter/filter_validator/equals_validator.py
--rw-r--r--   0        0        0      786 2023-12-30 05:07:20.251938 json_schema_filter-0.2.0/json_schema_filter/filter_validator/iequal_validator.py
--rw-r--r--   0        0        0      360 2023-12-30 04:05:13.024016 json_schema_filter-0.2.0/json_schema_filter/filter_validator/registry.py
--rw-r--r--   0        0        0      880 2023-12-30 04:14:24.724700 json_schema_filter-0.2.0/json_schema_filter/logging.py
--rw-r--r--   0        0        0       55 2023-12-30 04:18:24.448224 json_schema_filter-0.2.0/json_schema_filter/struct/__init__.py
--rw-r--r--   0        0        0      952 2023-12-31 04:51:46.054663 json_schema_filter-0.2.0/json_schema_filter/struct/filtered.py
--rw-r--r--   0        0        0      590 2023-12-31 05:28:21.518595 json_schema_filter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 json_schema_filter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-25 22:03:17.193575 json_schema_filter-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1164 2024-05-01 17:32:16.595352 json_schema_filter-0.3.0/README.md
+-rw-r--r--   0        0        0       69 2023-12-30 04:00:39.896921 json_schema_filter-0.3.0/json_schema_filter/__init__.py
+-rw-r--r--   0        0        0     2051 2023-12-31 04:42:41.204359 json_schema_filter-0.3.0/json_schema_filter/filter.py
+-rw-r--r--   0        0        0      602 2023-12-30 04:05:13.025776 json_schema_filter-0.3.0/json_schema_filter/filter_validator/__init__.py
+-rw-r--r--   0        0        0      464 2023-12-30 04:05:13.027310 json_schema_filter-0.3.0/json_schema_filter/filter_validator/equals_validator.py
+-rw-r--r--   0        0        0      786 2023-12-30 05:07:20.251938 json_schema_filter-0.3.0/json_schema_filter/filter_validator/iequal_validator.py
+-rw-r--r--   0        0        0      494 2024-05-01 17:39:22.676628 json_schema_filter-0.3.0/json_schema_filter/filter_validator/nequals_validator.py
+-rw-r--r--   0        0        0      360 2023-12-30 04:05:13.024016 json_schema_filter-0.3.0/json_schema_filter/filter_validator/registry.py
+-rw-r--r--   0        0        0      880 2023-12-30 04:14:24.724700 json_schema_filter-0.3.0/json_schema_filter/logging.py
+-rw-r--r--   0        0        0       55 2023-12-30 04:18:24.448224 json_schema_filter-0.3.0/json_schema_filter/struct/__init__.py
+-rw-r--r--   0        0        0      952 2023-12-31 04:51:46.054663 json_schema_filter-0.3.0/json_schema_filter/struct/filtered.py
+-rw-r--r--   0        0        0      590 2024-05-01 17:32:50.546873 json_schema_filter-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 json_schema_filter-0.3.0/PKG-INFO
```

### Comparing `json_schema_filter-0.2.0/LICENSE` & `json_schema_filter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/README.md` & `json_schema_filter-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -33,11 +33,12 @@
         1. name: Values not equal. Expected: Shakespeare, Found: what is in the name
 Filtered Item: [2]
         1. name: Values not equal. Expected: Shakespeare, Found: hamlet
 """
 ```
 
 ### Supported additional properties
-|Property|Supported type|
-|--------|--------------|
-|equals|*|
-|iequals|string|
+|Property|Supported type|Description|
+|--------|--------------|-----------|
+|equals|*|Check if value matches
+|iequals|string|Check if value matches (case insensitive)
+|nequals|*|Check if value does not match
```

### Comparing `json_schema_filter-0.2.0/json_schema_filter/filter.py` & `json_schema_filter-0.3.0/json_schema_filter/filter.py`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/json_schema_filter/filter_validator/__init__.py` & `json_schema_filter-0.3.0/json_schema_filter/filter_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/json_schema_filter/filter_validator/iequal_validator.py` & `json_schema_filter-0.3.0/json_schema_filter/filter_validator/iequal_validator.py`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/json_schema_filter/logging.py` & `json_schema_filter-0.3.0/json_schema_filter/logging.py`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/json_schema_filter/struct/filtered.py` & `json_schema_filter-0.3.0/json_schema_filter/struct/filtered.py`

 * *Files identical despite different names*

### Comparing `json_schema_filter-0.2.0/pyproject.toml` & `json_schema_filter-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-schema-filter"
-version = "0.2.0"
+version = "0.3.0"
 description = "A library that uses json schema to filter the objects"
 authors = ["Bharat Sinha <bharat.sinha.2307@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Bharat23/json-schema-filter"
 
 [tool.poetry.dependencies]
```

### Comparing `json_schema_filter-0.2.0/PKG-INFO` & `json_schema_filter-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-filter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library that uses json schema to filter the objects
 Home-page: https://github.com/Bharat23/json-schema-filter
 License: MIT
 Author: Bharat Sinha
 Author-email: bharat.sinha.2307@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,12 +52,13 @@
         1. name: Values not equal. Expected: Shakespeare, Found: what is in the name
 Filtered Item: [2]
         1. name: Values not equal. Expected: Shakespeare, Found: hamlet
 """
 ```
 
 ### Supported additional properties
-|Property|Supported type|
-|--------|--------------|
-|equals|*|
-|iequals|string|
+|Property|Supported type|Description|
+|--------|--------------|-----------|
+|equals|*|Check if value matches
+|iequals|string|Check if value matches (case insensitive)
+|nequals|*|Check if value does not match
```

