# Comparing `tmp/snakestream-0.2.3.tar.gz` & `tmp/snakestream-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakestream-0.2.3.tar", last modified: Sun Sep  3 17:10:02 2023, max compression
+gzip compressed data, was "snakestream-0.3.0.tar", last modified: Wed May  1 10:19:22 2024, max compression
```

## Comparing `snakestream-0.2.3.tar` & `snakestream-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.790576 snakestream-0.2.3/
--rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2022-11-14 20:54:45.000000 snakestream-0.2.3/.coveragerc
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.766576 snakestream-0.2.3/.github/
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.774576 snakestream-0.2.3/.github/workflows/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1120 2023-01-22 22:20:19.000000 snakestream-0.2.3/.github/workflows/check.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      909 2023-01-22 22:20:19.000000 snakestream-0.2.3/.github/workflows/deliver.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      572 2022-11-14 20:54:45.000000 snakestream-0.2.3/.gitignore
--rw-r--r--   0 tommy     (1000) tommy     (1000)      490 2022-11-14 20:54:45.000000 snakestream-0.2.3/.readthedocs.yml
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1081 2022-11-14 20:54:45.000000 snakestream-0.2.3/LICENSE.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2488 2023-09-03 17:10:02.790576 snakestream-0.2.3/PKG-INFO
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1991 2023-09-03 16:56:10.000000 snakestream-0.2.3/README.md
--rw-r--r--   0 tommy     (1000) tommy     (1000)      346 2022-11-14 20:54:45.000000 snakestream-0.2.3/pyproject.toml
--rw-r--r--   0 tommy     (1000) tommy     (1000)      263 2023-01-15 20:46:44.000000 snakestream-0.2.3/requirements-dev.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)       52 2023-01-15 20:46:44.000000 snakestream-0.2.3/requirements.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1127 2023-09-03 17:10:02.790576 snakestream-0.2.3/setup.cfg
--rw-r--r--   0 tommy     (1000) tommy     (1000)      964 2023-02-05 22:06:05.000000 snakestream-0.2.3/setup.py
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.766576 snakestream-0.2.3/src/
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.778576 snakestream-0.2.3/src/snakestream/
--rw-r--r--   0 tommy     (1000) tommy     (1000)      693 2023-02-05 22:06:05.000000 snakestream-0.2.3/src/snakestream/__init__.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      484 2023-01-29 23:14:42.000000 snakestream-0.2.3/src/snakestream/collector.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     8341 2023-09-03 17:08:29.000000 snakestream-0.2.3/src/snakestream/core.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)       48 2022-12-18 20:26:15.000000 snakestream-0.2.3/src/snakestream/exception.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      644 2023-01-22 22:20:19.000000 snakestream-0.2.3/src/snakestream/sort.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      439 2023-09-03 17:08:29.000000 snakestream-0.2.3/src/snakestream/stream_builder.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     3538 2023-09-03 17:08:29.000000 snakestream-0.2.3/src/snakestream/type.py
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.782576 snakestream-0.2.3/src/snakestream.egg-info/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2488 2023-09-03 17:10:02.000000 snakestream-0.2.3/src/snakestream.egg-info/PKG-INFO
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1088 2023-09-03 17:10:02.000000 snakestream-0.2.3/src/snakestream.egg-info/SOURCES.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2023-09-03 17:10:02.000000 snakestream-0.2.3/src/snakestream.egg-info/dependency_links.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2022-12-18 20:51:22.000000 snakestream-0.2.3/src/snakestream.egg-info/not-zip-safe
--rw-r--r--   0 tommy     (1000) tommy     (1000)      101 2023-09-03 17:10:02.000000 snakestream-0.2.3/src/snakestream.egg-info/requires.txt
--rw-r--r--   0 tommy     (1000) tommy     (1000)       12 2023-09-03 17:10:02.000000 snakestream-0.2.3/src/snakestream.egg-info/top_level.txt
-drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2023-09-03 17:10:02.790576 snakestream-0.2.3/tests/
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1103 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/conftest.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1004 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_all_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1015 2023-02-12 23:06:16.000000 snakestream-0.2.3/tests/test_any_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2023-09-03 17:08:29.000000 snakestream-0.2.3/tests/test_builder.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1666 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_collect.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1346 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_concat.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      651 2023-02-12 23:06:16.000000 snakestream-0.2.3/tests/test_count.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1166 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_distinct.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      306 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_empty.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1365 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_filter.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      834 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_find_first.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1447 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_flat_map.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      713 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_for_each.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2219 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_inputs.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)      536 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_integration.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1421 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_map.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2052 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_max.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2050 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_min.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1008 2023-02-12 23:06:16.000000 snakestream-0.2.3/tests/test_none_match.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     2492 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_peek.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1097 2023-09-03 16:56:10.000000 snakestream-0.2.3/tests/test_reduce.py
--rw-r--r--   0 tommy     (1000) tommy     (1000)     1674 2023-02-05 22:06:05.000000 snakestream-0.2.3/tests/test_sorted.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2022-11-14 20:54:45.000000 snakestream-0.3.0/.coveragerc
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.805450 snakestream-0.3.0/.github/
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.809450 snakestream-0.3.0/.github/workflows/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1128 2024-05-01 10:17:01.000000 snakestream-0.3.0/.github/workflows/check.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      917 2024-05-01 10:17:01.000000 snakestream-0.3.0/.github/workflows/deliver.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      572 2022-11-14 20:54:45.000000 snakestream-0.3.0/.gitignore
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      490 2022-11-14 20:54:45.000000 snakestream-0.3.0/.readthedocs.yml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1081 2022-11-14 20:54:45.000000 snakestream-0.3.0/LICENSE.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     3704 2024-05-01 10:19:22.813450 snakestream-0.3.0/PKG-INFO
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2965 2024-05-01 10:17:01.000000 snakestream-0.3.0/README.md
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      346 2022-11-14 20:54:45.000000 snakestream-0.3.0/pyproject.toml
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      149 2024-04-28 17:38:11.000000 snakestream-0.3.0/requirements-dev.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       52 2023-01-15 20:46:44.000000 snakestream-0.3.0/requirements.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-01 10:19:22.813450 snakestream-0.3.0/setup.cfg
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      964 2023-02-05 22:06:05.000000 snakestream-0.3.0/setup.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.805450 snakestream-0.3.0/src/
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.809450 snakestream-0.3.0/src/snakestream/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      614 2024-05-01 10:17:01.000000 snakestream-0.3.0/src/snakestream/__init__.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      484 2023-01-29 23:14:42.000000 snakestream-0.3.0/src/snakestream/collector.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)    10270 2024-05-01 10:17:01.000000 snakestream-0.3.0/src/snakestream/core.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       48 2022-12-18 20:26:15.000000 snakestream-0.3.0/src/snakestream/exception.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      644 2023-01-22 22:20:19.000000 snakestream-0.3.0/src/snakestream/sort.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      439 2023-09-03 17:08:29.000000 snakestream-0.3.0/src/snakestream/stream_builder.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     3555 2024-04-28 17:38:11.000000 snakestream-0.3.0/src/snakestream/type.py
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/src/snakestream.egg-info/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     3704 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/PKG-INFO
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1109 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/SOURCES.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/dependency_links.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)        1 2022-12-18 20:51:22.000000 snakestream-0.3.0/src/snakestream.egg-info/not-zip-safe
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      101 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/requires.txt
+-rw-r--r--   0 tommy     (1000) tommy     (1000)       12 2024-05-01 10:19:22.000000 snakestream-0.3.0/src/snakestream.egg-info/top_level.txt
+drwxr-xr-x   0 tommy     (1000) tommy     (1000)        0 2024-05-01 10:19:22.813450 snakestream-0.3.0/tests/
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1103 2023-02-05 22:06:05.000000 snakestream-0.3.0/tests/conftest.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1001 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_all_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1012 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_any_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      594 2023-09-03 17:08:29.000000 snakestream-0.3.0/tests/test_builder.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1663 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_collect.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1312 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_concat.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      648 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_count.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1163 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_distinct.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      295 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_empty.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1362 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_filter.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      823 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_find_any.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1444 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_flat_map.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      710 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_for_each.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2216 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_inputs.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)      533 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_integration.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1418 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_map.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2049 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_max.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2047 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_min.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1005 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_none_match.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1246 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_parallel.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     2489 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_peek.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1094 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_reduce.py
+-rw-r--r--   0 tommy     (1000) tommy     (1000)     1671 2024-05-01 10:17:01.000000 snakestream-0.3.0/tests/test_sorted.py
```

### Comparing `snakestream-0.2.3/.coveragerc` & `snakestream-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/.github/workflows/check.yml` & `snakestream-0.3.0/.github/workflows/check.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 jobs:
   code_check:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3.3.0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `snakestream-0.2.3/.github/workflows/deliver.yml` & `snakestream-0.3.0/.github/workflows/deliver.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3.3.0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `snakestream-0.2.3/.gitignore` & `snakestream-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/LICENSE.txt` & `snakestream-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/PKG-INFO` & `snakestream-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: snakestream
-Version: 0.2.3
-Summary: Java like streams for snakes
-Home-page: https://github.com/carby/snakestream
-Author: Tommy Derngren
-Author-email: tommy.derngren@hiq.se
-License: MIT
-Project-URL: Documentation, https://github.com/carby/snakestream/wiki
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 # Snakestream
 **Java like streams for snakes**
 
 This is a python streaming api with witch you can get a similar experience as with the Java streams api from Java 8. There is no feature parity, what has been done so far is a beginning, and we will see where the road takes us.
 
 ### Features
 - Create a stream from a List, Generator or AsyncGenerator.
@@ -60,15 +43,15 @@
 
 async def async_int_to_letter(x: int) -> str:
     await asyncio.sleep(0.01)
     return int_2_letter[x]
 
 
 async def main():
-    it = stream_of([1, 3, 4, 5, 6]) \
+    it = Stream.of([1, 3, 4, 5, 6]) \
         .filter(lambda n: 3 < n < 6) \
         .map(async_int_to_letter) \
         .collect(to_generator)
 
     async for x in it:
         print(x)
 
@@ -80,9 +63,40 @@
 ~/t/test> python test.py
 d
 e
 ```
 
 ### Migration
 These are a list of the known breaking changes. Until release 1.0.0 focus will be on implementing features and changing things that does not align with how streams work in java.
-- **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
+- **0.2.4 -> 0.2.5:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
 - **0.1.0 -> 0.2.0:** The `unique()` function has been renamed `distinct()`. So rename all imports of that function, and it should be OK
+- **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
+
+### Left to do:
+
+BaseStream:
+close()
+isParallel()
+iterator()
+onClose(Runnable closeHandler)
+spliterator()
+unordered()
+
+Stream:
+collect(Supplier<R> supplier, BiConsumer<R,? super T> accumulator, BiConsumer<R,R> combiner)
+flatMapToDouble(Function<? super T,? extends DoubleStream> mapper)
+flatMapToInt(Function<? super T,? extends IntStream> mapper)
+flatMapToLong(Function<? super T,? extends LongStream> mapper)
+forEachOrdered(Consumer<? super T> action)
+generate(Supplier<T> s)
+iterate(T seed, UnaryOperator<T> f)
+limit(long maxSize)
+mapToDouble(ToDoubleFunction<? super T> mapper)
+mapToInt(ToIntFunction<? super T> mapper)
+mapToLong(ToLongFunction<? super T> mapper)
+of(T t)
+
+reduce(BinaryOperator<T> accumulator) // have done the one with the identity
+skip(long n)
+sorted() // have done the one with a comparator
+toArray()
+toArray(IntFunction<A[]> generator)
```

### Comparing `snakestream-0.2.3/setup.cfg` & `snakestream-0.3.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 [devpi:upload]
 no_vcs = 1
 formats = bdist_wheel
 
 [flake8]
 max_line_length = 88
 extend_ignore = E203, W503
+per-file-ignores = __init__.py:F401
 exclude = 
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 	.virtualenv
```

### Comparing `snakestream-0.2.3/setup.py` & `snakestream-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/src/snakestream/core.py` & `snakestream-0.3.0/src/snakestream/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,115 @@
 from __future__ import annotations
 
+import asyncio
 from functools import cmp_to_key
 from inspect import iscoroutinefunction
 from typing import Callable, Optional, AsyncIterable, List, \
     Union, AsyncGenerator, Any
 
 from snakestream.collector import to_generator
 from snakestream.exception import StreamBuildException
 from snakestream.sort import merge_sort
 from snakestream.type import R, T, AbstractStream, AbstractStreamBuilder, Accumulator, Comparator, Consumer, \
     FlatMapper, Mapper, Predicate, Streamable
 
 
+PROCESSES: int = 4
+
+
 async def _normalize(iterable: Streamable) -> AsyncGenerator:
-    if isinstance(iterable, AsyncGenerator) or isinstance(iterable, AsyncIterable):
-        async for i in iterable:
-            yield i
-    else:
-        for i in iterable:
-            yield i
+    for i in iterable:
+        yield i
 
 
 async def _concat(a: 'Stream', b: 'Stream') -> AsyncGenerator:
-    async for i in a._compose(a._chain, a._stream):
+    async for i in a._compose():
         yield i
-    async for j in b._compose(b._chain, b._stream):
+    async for j in b._compose():
         yield j
 
 
+class BaseStream():
+    def __init__(self, streamable: Streamable) -> None:
+        if isinstance(streamable, AsyncGenerator) or isinstance(streamable, AsyncIterable):
+            self._stream = streamable
+        else:
+            self._stream: AsyncGenerator = _normalize(streamable)
+        self._chain: List[Callable] = []
+        self.is_parallel = False
+
+    def _sequential(self, intermediaries: List[Callable], iterable: AsyncGenerator) -> AsyncGenerator:
+        if len(intermediaries) == 0:
+            return iterable
+        if len(intermediaries) == 1:
+            fn = intermediaries.pop(0)
+            return fn(iterable)
+        fn = intermediaries.pop(0)
+        return self._sequential(intermediaries, fn(iterable))
+
+    async def _parallel(
+        self,
+        intermediaries: List[Callable],
+        iterable: AsyncGenerator,
+        processes: int = PROCESSES
+    ) -> AsyncGenerator:
+        async_iterators = [self._sequential(intermediaries[:], iterable) for n in range(processes)]
+        tasks = [asyncio.ensure_future(n.__anext__()) for n in async_iterators]
+
+        while any([n is not None for n in tasks]):
+
+            waitlist = filter(lambda n: n is not None, tasks)
+            done, _ = await asyncio.wait(waitlist, return_when=asyncio.FIRST_COMPLETED)
+
+            for task in done:
+                task_idx = tasks.index(task)
+                try:
+                    result = tasks[task_idx].result()
+                    tasks[task_idx] = asyncio.ensure_future(async_iterators[task_idx].__anext__())
+                    yield result
+                except StopAsyncIteration:
+                    tasks[task_idx] = None
+
+    def _compose(self) -> AsyncGenerator:
+        if self.is_parallel:
+            return self._parallel(self._chain, self._stream)
+        else:
+            return self._sequential(self._chain, self._stream)
+
+    def sequential(self) -> 'Stream':
+        self.stream = self._compose()
+        self.is_parallel = False
+
+        async def fn(iterable: AsyncGenerator) -> AsyncGenerator:
+            async for i in iterable:
+                yield i
+        self._chain = [fn]
+        return self
+
+    def parallel(self) -> 'Stream':
+        self.stream = self._compose()
+        self.is_parallel = True
+
+        async def fn(iterable: AsyncGenerator) -> AsyncGenerator:
+            async for i in iterable:
+                yield i
+        self._chain = [fn]
+        return self
+
+
 #
 # If you add a method here, also add it to AbstractStream
 #
-class Stream(AbstractStream):
+class Stream(BaseStream, AbstractStream):
     def __init__(self, streamable: Streamable) -> None:
-        self._stream: AsyncGenerator = _normalize(streamable)
-        self._chain: List[Callable] = []
+        super().__init__(streamable)
+
+    @staticmethod
+    def of(iterable: Streamable) -> 'Stream':
+        return Stream(iterable)
 
     @staticmethod
     def empty() -> 'Stream':
         return Stream([])
 
     @staticmethod
     async def concat(a: 'Stream', b: 'Stream') -> 'Stream':
@@ -136,44 +207,42 @@
                     consumer(i)
                 yield i
 
         self._chain.append(fn)
         return self
 
     # Terminals
-    def _compose(self, intermediaries: List[Callable], iterable: AsyncGenerator) -> AsyncGenerator:
-        if len(intermediaries) == 0:
-            return iterable
-        if len(intermediaries) == 1:
-            fn = intermediaries.pop(0)
-            return fn(iterable)
-        fn = intermediaries.pop(0)
-        return self._compose(intermediaries, fn(iterable))
-
-    def collect(self, collector: Callable) -> AsyncGenerator:
-        return collector(self._compose(self._chain, self._stream))
+    def collect(self, collector: Callable) -> Union[List, AsyncGenerator]:
+        return collector(self._compose())
 
     async def reduce(self, identity: Union[T, R], accumulator: Accumulator) -> Union[T, R]:
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if iscoroutinefunction(accumulator):
                 identity = await accumulator(identity, n)
             else:
                 identity = accumulator(identity, n)
         return identity
 
     async def for_each(self, consumer: Callable[[T], Any]) -> None:
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if iscoroutinefunction(consumer):
                 await consumer(n)
             else:
                 consumer(n)
         return None
 
+    '''
     async def find_first(self) -> Optional[Any]:
-        async for n in self._compose(self._chain, self._stream):
+        # until we have ordered parallel stream then we
+        # cant do this one
+        return await self.find_any()
+    '''
+
+    async def find_any(self) -> Optional[Any]:
+        async for n in self._compose():
             return n
 
     async def max(self, comparator: Comparator) -> Optional[T]:
         return await self._min_max(comparator)
 
     async def min(self, comparator: Comparator) -> Optional[T]:
         if iscoroutinefunction(comparator):
@@ -183,67 +252,67 @@
         else:
             def negative_comparator(x, y):
                 return not comparator(x, y)
             return await self._min_max(negative_comparator)
 
     async def _min_max(self, comparator: Comparator) -> Optional[T]:
         found = None
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if found is None:
                 found = n
                 continue
 
             if iscoroutinefunction(comparator):
                 if n and await comparator(n, found):
                     found = n
             else:
                 if n and comparator(n, found):
                     found = n
         return found
 
     async def all_match(self, predicate: Predicate) -> bool:
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if iscoroutinefunction(predicate):
                 if await predicate(n):
                     continue
                 else:
                     return False
             else:
                 if predicate(n):
                     continue
                 else:
                     return False
         return True
 
     async def none_match(self, predicate: Predicate) -> bool:
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if iscoroutinefunction(predicate):
                 if await predicate(n):
                     return False
                 else:
                     continue
             else:
                 if predicate(n):
                     return False
                 else:
                     continue
         return True
 
     async def any_match(self, predicate: Predicate) -> bool:
-        async for n in self._compose(self._chain, self._stream):
+        async for n in self._compose():
             if iscoroutinefunction(predicate):
                 if await predicate(n):
                     return True
                 else:
                     continue
             else:
                 if predicate(n):
                     return True
                 else:
                     continue
         return False
 
     async def count(self) -> int:
         c = 0
-        async for _ in self._compose(self._chain, self._stream):
+        async for _ in self._compose():
             c += 1
         return c
```

### Comparing `snakestream-0.2.3/src/snakestream/sort.py` & `snakestream-0.3.0/src/snakestream/sort.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/src/snakestream/type.py` & `snakestream-0.3.0/src/snakestream/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Any, AsyncGenerator, AsyncIterable, Awaitable, Callable, Generator, Iterable, Optional, TypeVar, Union
+from typing import Any, AsyncGenerator, AsyncIterable, Awaitable, Callable, Generator, Iterable, Optional, TypeVar, Union, List
 
 
 #
 # Generic types
 #
 T = TypeVar('T')
 R = TypeVar('R')
@@ -66,27 +66,27 @@
 
     @abc.abstractclassmethod
     def peek(self, consumer: Consumer) -> 'AbstractStream':
         raise NotImplementedError
 
     # Terminals
     @abc.abstractclassmethod
-    def collect(self, collector: Callable) -> AsyncGenerator:
+    def collect(self, collector: Callable) -> Union[AsyncGenerator, List]:
         raise NotImplementedError
 
     @abc.abstractclassmethod
     async def reduce(self, identity: Union[T, R], accumulator: Accumulator) -> Union[T, R]:
         raise NotImplementedError
 
     @abc.abstractclassmethod
     async def for_each(self, consumer: Callable[[T], Any]) -> None:
         raise NotImplementedError
 
     @abc.abstractclassmethod
-    async def find_first(self) -> Optional[Any]:
+    async def find_any(self) -> Optional[Any]:
         raise NotImplementedError
 
     @abc.abstractclassmethod
     async def max(self, comparator: Comparator) -> Optional[T]:
         raise NotImplementedError
 
     @abc.abstractclassmethod
```

### Comparing `snakestream-0.2.3/src/snakestream.egg-info/PKG-INFO` & `snakestream-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: snakestream
-Version: 0.2.3
+Version: 0.3.0
 Summary: Java like streams for snakes
 Home-page: https://github.com/carby/snakestream
 Author: Tommy Derngren
 Author-email: tommy.derngren@hiq.se
 License: MIT
 Project-URL: Documentation, https://github.com/carby/snakestream/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-asyncio; extra == "testing"
 
 # Snakestream
 **Java like streams for snakes**
 
 This is a python streaming api with witch you can get a similar experience as with the Java streams api from Java 8. There is no feature parity, what has been done so far is a beginning, and we will see where the road takes us.
 
 ### Features
@@ -60,15 +65,15 @@
 
 async def async_int_to_letter(x: int) -> str:
     await asyncio.sleep(0.01)
     return int_2_letter[x]
 
 
 async def main():
-    it = stream_of([1, 3, 4, 5, 6]) \
+    it = Stream.of([1, 3, 4, 5, 6]) \
         .filter(lambda n: 3 < n < 6) \
         .map(async_int_to_letter) \
         .collect(to_generator)
 
     async for x in it:
         print(x)
 
@@ -80,9 +85,40 @@
 ~/t/test> python test.py
 d
 e
 ```
 
 ### Migration
 These are a list of the known breaking changes. Until release 1.0.0 focus will be on implementing features and changing things that does not align with how streams work in java.
-- **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
+- **0.2.4 -> 0.2.5:** stream_of() has been removed in favour of Stream.of() for getting closer to the java api.
 - **0.1.0 -> 0.2.0:** The `unique()` function has been renamed `distinct()`. So rename all imports of that function, and it should be OK
+- **0.0.5 -> 0.0.6:** The `stream()` function has been renamed `stream_of()`. So rename all imports of that function, and it should be OK
+
+### Left to do:
+
+BaseStream:
+close()
+isParallel()
+iterator()
+onClose(Runnable closeHandler)
+spliterator()
+unordered()
+
+Stream:
+collect(Supplier<R> supplier, BiConsumer<R,? super T> accumulator, BiConsumer<R,R> combiner)
+flatMapToDouble(Function<? super T,? extends DoubleStream> mapper)
+flatMapToInt(Function<? super T,? extends IntStream> mapper)
+flatMapToLong(Function<? super T,? extends LongStream> mapper)
+forEachOrdered(Consumer<? super T> action)
+generate(Supplier<T> s)
+iterate(T seed, UnaryOperator<T> f)
+limit(long maxSize)
+mapToDouble(ToDoubleFunction<? super T> mapper)
+mapToInt(ToIntFunction<? super T> mapper)
+mapToLong(ToLongFunction<? super T> mapper)
+of(T t)
+
+reduce(BinaryOperator<T> accumulator) // have done the one with the identity
+skip(long n)
+sorted() // have done the one with a comparator
+toArray()
+toArray(IntFunction<A[]> generator)
```

### Comparing `snakestream-0.2.3/src/snakestream.egg-info/SOURCES.txt` & `snakestream-0.3.0/src/snakestream.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 tests/test_builder.py
 tests/test_collect.py
 tests/test_concat.py
 tests/test_count.py
 tests/test_distinct.py
 tests/test_empty.py
 tests/test_filter.py
-tests/test_find_first.py
+tests/test_find_any.py
 tests/test_flat_map.py
 tests/test_for_each.py
 tests/test_inputs.py
 tests/test_integration.py
 tests/test_map.py
 tests/test_max.py
 tests/test_min.py
 tests/test_none_match.py
+tests/test_parallel.py
 tests/test_peek.py
 tests/test_reduce.py
 tests/test_sorted.py
```

### Comparing `snakestream-0.2.3/tests/conftest.py` & `snakestream-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/tests/test_all_match.py` & `snakestream-0.3.0/tests/test_none_match.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import asyncio
 
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 
 
 @pytest.mark.asyncio
 async def test_empty_stream() -> None:
-    it = await stream_of([]) \
-        .all_match(lambda x: x > 5)
+    it = await Stream.of([]) \
+        .none_match(lambda x: x > 5)
     assert it is True
 
 
 @pytest.mark.asyncio
-async def test_none_matches() -> None:
-    it = await stream_of([1, 2, 3, 2, 3, 1, 2]) \
-        .all_match(lambda x: x > 5)
-    assert it is False
+async def test_simple() -> None:
+    it = await Stream.of([1, 2, 3, 2, 3, 1, 2]) \
+        .none_match(lambda x: x > 5)
+    assert it is True
 
 
 @pytest.mark.asyncio
 async def test_some_matches() -> None:
-    it = await stream_of([1, 2, 3, 2, 3, 1, 2, 5, 6, 7]) \
-        .all_match(lambda x: x < 5)
+    it = await Stream.of([1, 2, 3, 2, 3, 1, 2, 5, 6, 7]) \
+        .none_match(lambda x: x < 5)
     assert it is False
 
 
 @pytest.mark.asyncio
-async def test_simple() -> None:
-    it = await stream_of([1, 2, 3, 2, 3, 1, 2]) \
-        .all_match(lambda x: x < 5)
-    assert it is True
-
-
-@pytest.mark.asyncio
 async def test_simple_async() -> None:
     async def async_predicate(x: int) -> bool:
         await asyncio.sleep(0.01)
-        return x < 5
+        return x > 5
 
-    it = await stream_of([1, 2, 3, 2, 3, 1, 2]) \
-        .all_match(async_predicate)
+    it = await Stream.of([1, 2, 3, 2, 3, 1, 2]) \
+        .none_match(async_predicate)
     assert it is True
+
+
+@pytest.mark.asyncio
+async def test_all_matches() -> None:
+    it = await Stream.of([1, 2, 3, 2, 3, 1, 2]) \
+        .none_match(lambda x: x < 5)
+    assert it is False
```

### Comparing `snakestream-0.2.3/tests/test_builder.py` & `snakestream-0.3.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `snakestream-0.2.3/tests/test_collect.py` & `snakestream-0.3.0/tests/test_collect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_list, to_generator
 
 
 @pytest.mark.asyncio
 async def test_to_generator() -> None:
     # when
-    it = stream_of([1, 2, 3, 4]) \
+    it = Stream.of([1, 2, 3, 4]) \
         .collect(to_generator)
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     assert await it.__anext__() == 3
     assert await it.__anext__() == 4
 
     with pytest.raises(StopAsyncIteration):
         await it.__anext__()
 
 
 @pytest.mark.asyncio
 async def test_to_generator_with_null_in_stream() -> None:
     # when
-    it = stream_of([1, 2, None, 4]) \
+    it = Stream.of([1, 2, None, 4]) \
         .collect(to_generator)
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     assert await it.__anext__() is None
     assert await it.__anext__() == 4
 
     with pytest.raises(StopAsyncIteration):
         await it.__anext__()
 
 
 @pytest.mark.asyncio
 async def test_to_generator_with_empty_list_input() -> None:
     # when
-    it = stream_of([]) \
+    it = Stream.of([]) \
         .collect(to_generator)
     # then
     with pytest.raises(StopAsyncIteration):
         await it.__anext__()
 
 
 @pytest.mark.asyncio
 async def test_to_list() -> None:
     # when
-    it = await stream_of([1, 2, 3, 4]) \
+    it = await Stream.of([1, 2, 3, 4]) \
         .collect(to_list)
     # then
     assert it == [1, 2, 3, 4]
 
 
 @pytest.mark.asyncio
 async def test_to_list_with_none_in_stream() -> None:
     # when
-    it = await stream_of([1, None, 3, 4]) \
+    it = await Stream.of([1, None, 3, 4]) \
         .collect(to_list)
     # then
     assert it == [1, None, 3, 4]
 
 
 @pytest.mark.asyncio
 async def test_to_list_with_empty_list_input() -> None:
     # when
-    it = await stream_of([]) \
+    it = await Stream.of([]) \
         .collect(to_list)
     # then
     assert it == []
```

### Comparing `snakestream-0.2.3/tests/test_concat.py` & `snakestream-0.3.0/tests/test_concat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 
 import pytest
 
-from snakestream import stream_of
 from snakestream.collector import to_generator
 from snakestream.core import Stream
 
 
 @pytest.mark.asyncio
 async def test_concat_simple() -> None:
     # when
-    a = stream_of([1, 2, 3, 4])
-    b = stream_of([5, 6, 7])
+    a = Stream.of([1, 2, 3, 4])
+    b = Stream.of([5, 6, 7])
 
     generator = (await Stream.concat(a, b)) \
         .collect(to_generator)
 
     # then
     assert await generator.__anext__() == 1
     assert await generator.__anext__() == 2
@@ -27,17 +26,17 @@
     with pytest.raises(StopAsyncIteration):
         await generator.__anext__()
 
 
 @pytest.mark.asyncio
 async def test_concat_with_intermediaries() -> None:
     # when
-    a = stream_of([1, 2, 3, 4]) \
+    a = Stream.of([1, 2, 3, 4]) \
         .filter(lambda x: x < 3)
-    b = stream_of([5, 6, 7, 7]) \
+    b = Stream.of([5, 6, 7, 7]) \
         .distinct()
 
     generator = (await Stream.concat(a, b)) \
         .collect(to_generator)
 
     # then
     assert await generator.__anext__() == 1
```

### Comparing `snakestream-0.2.3/tests/test_count.py` & `snakestream-0.3.0/tests/test_count.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 
 
 @pytest.mark.asyncio
 async def test_empty_stream() -> None:
-    it = await stream_of([]) \
+    it = await Stream.of([]) \
         .count()
     assert it == 0
 
 
 @pytest.mark.asyncio
 async def test_base_test() -> None:
-    it = await stream_of([1, 2, 3, 4, 5, 6]) \
+    it = await Stream.of([1, 2, 3, 4, 5, 6]) \
         .count()
     assert it == 6
 
 
 @pytest.mark.asyncio
 async def test_case_insensitive() -> None:
-    it = await stream_of(['test', 'Test', 'test', 'foo', 'bar']) \
+    it = await Stream.of(['test', 'Test', 'test', 'foo', 'bar']) \
         .count()
     assert it == 5
 
 
 @pytest.mark.asyncio
 async def test_null_count() -> None:
-    it = await stream_of(['test', 'Test', 'test', None, 'bar']) \
+    it = await Stream.of(['test', 'Test', 'test', None, 'bar']) \
         .count()
     assert it == 5
```

### Comparing `snakestream-0.2.3/tests/test_distinct.py` & `snakestream-0.3.0/tests/test_distinct.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_list
 from conftest import MyObject
 
 
 @pytest.mark.asyncio
 async def test_unique() -> None:
     # when
-    it = await stream_of([1, 7, 3, 7, 5, 6, 0, 6, 6]) \
+    it = await Stream.of([1, 7, 3, 7, 5, 6, 0, 6, 6]) \
         .distinct() \
         .collect(to_list)
     # then
     assert it == [1, 7, 3, 5, 6, 0]
 
 
 @pytest.mark.asyncio
 async def test_unique_empty_list() -> None:
     # when
-    it = await stream_of([]) \
+    it = await Stream.of([]) \
         .distinct() \
         .collect(to_list)
     # then
     assert it == []
 
 
 @pytest.mark.asyncio
 async def test_unique_list_with_no_dupes() -> None:
     # when
-    it = await stream_of([1, 2, 3, 4]) \
+    it = await Stream.of([1, 2, 3, 4]) \
         .distinct() \
         .collect(to_list)
     # then
     assert it == [1, 2, 3, 4]
 
 
 @pytest.mark.asyncio
 async def test_unique_object_list() -> None:
     # when
     input_list = [MyObject(1, "object1"), MyObject(2, "object2"), MyObject(3, "object3"), MyObject(2, "object2"),
                   MyObject(3, "object3")]
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .distinct() \
         .collect(to_list)
     # then
     assert it == [MyObject(1, "object1"), MyObject(2, "object2"), MyObject(3, "object3")]
```

### Comparing `snakestream-0.2.3/tests/test_filter.py` & `snakestream-0.3.0/tests/test_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 import asyncio
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_generator, to_list
 
 
 @pytest.mark.asyncio
 async def test_filter_multiple() -> None:
     # when
-    it = stream_of([1, 2, 3, 4, 5, 6]) \
+    it = Stream.of([1, 2, 3, 4, 5, 6]) \
         .filter(lambda x: x > 3) \
         .filter(lambda x: x < 6) \
         .collect(to_generator)
 
     # then
     assert await it.__anext__() == 4
     assert await it.__anext__() == 5
@@ -25,15 +25,15 @@
 
 
 @pytest.mark.asyncio
 async def test_filter_does_not_mutate_source() -> None:
     source = [1, 2, 3, 4, 5, 6]
 
     # when
-    it = await stream_of(source) \
+    it = await Stream.of(source) \
         .filter(lambda x: x > 3) \
         .filter(lambda x: x < 6) \
         .collect(to_list)
 
     # then
     assert source != it
     assert len(source) == 6
@@ -44,15 +44,15 @@
 async def test_filter_async_function() -> None:
 
     async def async_predicate(x: int) -> bool:
         await asyncio.sleep(0.01)
         return x < 3
 
     # when
-    it = stream_of([1, 2, 3, 4]) \
+    it = Stream.of([1, 2, 3, 4]) \
         .filter(async_predicate) \
         .collect(to_generator)
 
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     try:
```

### Comparing `snakestream-0.2.3/tests/test_find_first.py` & `snakestream-0.3.0/tests/test_find_any.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 
 
 @pytest.mark.asyncio
-async def test_find_first() -> None:
+async def test_find_any() -> None:
     counter = 0
 
     def incr_counter(c):
         nonlocal counter
         counter += 1
         return c
 
     # when
-    it = await stream_of([1, 2, 3, 4, 5, 6, 1, 2, 3, 4, 5, 6]) \
+    it = await Stream.of([1, 2, 3, 4, 5, 6, 1, 2, 3, 4, 5, 6]) \
         .map(incr_counter) \
         .filter(lambda x: x == 6) \
-        .find_first()
+        .find_any()
 
     # then
     assert it == 6
     assert counter == 6
 
 
 @pytest.mark.asyncio
-async def test_find_first_found_none() -> None:
+async def test_find_any_found_none() -> None:
     counter = 0
 
     def incr_counter(c):
         nonlocal counter
         counter += 1
         return c
 
     # when
-    it = await stream_of([1, 2, 3, 4, 5, 6, 1, 2, 3, 4, 5, 6]) \
+    it = await Stream.of([1, 2, 3, 4, 5, 6, 1, 2, 3, 4, 5, 6]) \
         .map(incr_counter) \
         .filter(lambda x: x == 100) \
-        .find_first()
+        .find_any()
 
     # then
     assert it is None
     assert counter == 12
```

### Comparing `snakestream-0.2.3/tests/test_flat_map.py` & `snakestream-0.3.0/tests/test_inputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,96 @@
+# pylint: disable=missing-module-docstring
+# pylint: disable=missing-class-docstring
+# pylint: disable=missing-function-docstring
+# pylint: disable=invalid-name
+
+from typing import AsyncGenerator
 import pytest
-import asyncio
 
-from snakestream import stream_of
-from snakestream.collector import to_generator
-from snakestream.exception import StreamBuildException
+from snakestream import Stream
+from snakestream.collector import to_generator, to_list
+
+
+async def async_generator() -> AsyncGenerator:
+    for i in range(1, 6):
+        yield i
 
 
-async def async_flat_map(x: int) -> int:
-    await asyncio.sleep(0.01)
-    return x
+class AsyncIteratorImpl:
+    def __init__(self, end_range):
+        self.end = end_range
+        self.start = -1
+
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self):
+        if self.start < self.end - 1:
+            self.start += 1
+            return self.start
+        raise StopAsyncIteration
 
 
 @pytest.mark.asyncio
-async def test_flat_map() -> None:
+async def test_input_list() -> None:
     # when
-    it = stream_of([[1, 2], [3, 4]]) \
-        .flat_map(lambda x: stream_of(x)) \
+    it = Stream.of([1, 2, 3, 4]) \
         .collect(to_generator)
-
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     assert await it.__anext__() == 3
     assert await it.__anext__() == 4
     try:
         await it.__anext__()
     except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_flat_map_no_mixed_list() -> None:
-    it = stream_of([[1, 2], [3, 4], 5]) \
-        .flat_map(lambda x: stream_of(x)) \
+async def test_input_async_generator() -> None:
+    # when
+    it = Stream.of(async_generator()) \
         .collect(to_generator)
 
     # then
     assert await it.__anext__() == 1
     assert await it.__anext__() == 2
     assert await it.__anext__() == 3
     assert await it.__anext__() == 4
+    assert await it.__anext__() == 5
     try:
         await it.__anext__()
-    except TypeError:
+    except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_flat_map_async_function() -> None:
+async def test_input_async_iterator() -> None:
     # when
+    it = Stream.of(AsyncIteratorImpl(5)) \
+        .collect(to_generator)
+
+    # then
+    assert await it.__anext__() == 0
+    assert await it.__anext__() == 1
+    assert await it.__anext__() == 2
+    assert await it.__anext__() == 3
+    assert await it.__anext__() == 4
     try:
-        stream_of([[1, 2], [3, 4], 5]) \
-            .flat_map(async_flat_map) \
-            .collect(to_generator)
-    except StreamBuildException:
+        await it.__anext__()
+    except StopAsyncIteration:
         pass
     else:
         assert False
+
+
+@pytest.mark.asyncio
+async def test_null_input() -> None:
+    # when
+    with pytest.raises(TypeError):
+        await Stream.of(None) \
+            .collect(to_list)
```

### Comparing `snakestream-0.2.3/tests/test_for_each.py` & `snakestream-0.3.0/tests/test_for_each.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import pytest
 import asyncio
 
-from snakestream import stream_of
+from snakestream import Stream
 
 
 coords = [
     {'x': 1, 'y': 5},
     {'x': 2, 'y': 6},
     {'x': 3, 'y': 7},
 ]
 
 
 @pytest.mark.asyncio
 async def test_for_each() -> None:
     def incr_y(c) -> None:
         c['y'] = 1
 
-    await stream_of(coords) \
+    await Stream.of(coords) \
         .for_each(incr_y)
 
     assert coords[0]['y'] == 1
     assert coords[1]['y'] == 1
     assert coords[2]['y'] == 1
 
 
 @pytest.mark.asyncio
 async def test_for_each_async() -> None:
     async def async_incr_y(c) -> None:
         await asyncio.sleep(0.01)
         c['y'] = 1
 
-    await stream_of(coords) \
+    await Stream.of(coords) \
         .for_each(async_incr_y)
 
     assert coords[0]['y'] == 1
     assert coords[1]['y'] == 1
     assert coords[2]['y'] == 1
```

### Comparing `snakestream-0.2.3/tests/test_inputs.py` & `snakestream-0.3.0/tests/test_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,61 @@
-# pylint: disable=missing-module-docstring
-# pylint: disable=missing-class-docstring
-# pylint: disable=missing-function-docstring
-# pylint: disable=invalid-name
-
-from typing import AsyncGenerator
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_generator, to_list
 
 
-async def async_generator() -> AsyncGenerator:
-    for i in range(1, 6):
-        yield i
-
-
-class AsyncIteratorImpl:
-    def __init__(self, end_range):
-        self.end = end_range
-        self.start = -1
-
-    def __aiter__(self):
-        return self
-
-    async def __anext__(self):
-        if self.start < self.end - 1:
-            self.start += 1
-            return self.start
-        raise StopAsyncIteration
-
-
 @pytest.mark.asyncio
-async def test_input_list() -> None:
+async def test_map(int_2_letter) -> None:
     # when
-    it = stream_of([1, 2, 3, 4]) \
+    it = Stream.of([1, 2, 3, 4]) \
+        .map(lambda x: int_2_letter[x]) \
         .collect(to_generator)
+
     # then
-    assert await it.__anext__() == 1
-    assert await it.__anext__() == 2
-    assert await it.__anext__() == 3
-    assert await it.__anext__() == 4
+    assert await it.__anext__() == 'a'
+    assert await it.__anext__() == 'b'
+    assert await it.__anext__() == 'c'
+    assert await it.__anext__() == 'd'
     try:
         await it.__anext__()
     except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_input_async_generator() -> None:
+async def test_map_async_function(async_int_to_letter) -> None:
+    async_int_to_letter = await async_int_to_letter
+
     # when
-    it = stream_of(async_generator()) \
+    it = Stream.of([1, 2, 3, 4]) \
+        .map(async_int_to_letter) \
         .collect(to_generator)
 
     # then
-    assert await it.__anext__() == 1
-    assert await it.__anext__() == 2
-    assert await it.__anext__() == 3
-    assert await it.__anext__() == 4
-    assert await it.__anext__() == 5
+    assert await it.__anext__() == 'a'
+    assert await it.__anext__() == 'b'
+    assert await it.__anext__() == 'c'
+    assert await it.__anext__() == 'd'
     try:
         await it.__anext__()
     except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_input_async_iterator() -> None:
+async def test_map_does_not_mutate_source(int_2_letter) -> None:
+    source = [1, 2, 3, 4]
+
     # when
-    it = stream_of(AsyncIteratorImpl(5)) \
-        .collect(to_generator)
+    it = await Stream.of(source) \
+        .map(lambda x: int_2_letter[x]) \
+        .collect(to_list)
 
     # then
-    assert await it.__anext__() == 0
-    assert await it.__anext__() == 1
-    assert await it.__anext__() == 2
-    assert await it.__anext__() == 3
-    assert await it.__anext__() == 4
-    try:
-        await it.__anext__()
-    except StopAsyncIteration:
-        pass
-    else:
-        assert False
-
-
-@pytest.mark.asyncio
-async def test_null_input() -> None:
-    # when
-    with pytest.raises(TypeError):
-        await stream_of(None) \
-            .collect(to_list)
+    assert source != it
+    assert len(source) == 4
+    assert len(it) == 4
```

### Comparing `snakestream-0.2.3/tests/test_integration.py` & `snakestream-0.3.0/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_generator
 
 
 @pytest.mark.asyncio
 async def test_mixed_chain(int_2_letter) -> None:
     # when
-    it = stream_of([1, 2, 3, 4, 5, 6]) \
+    it = Stream.of([1, 2, 3, 4, 5, 6]) \
         .filter(lambda x: 3 < x < 6) \
         .map(lambda x: int_2_letter[x]) \
         .collect(to_generator)
 
     # then
     assert await it.__anext__() == 'd'
     assert await it.__anext__() == 'e'
```

### Comparing `snakestream-0.2.3/tests/test_map.py` & `snakestream-0.3.0/tests/test_flat_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 import pytest
+import asyncio
 
-from snakestream import stream_of
-from snakestream.collector import to_generator, to_list
+from snakestream import Stream
+from snakestream.collector import to_generator
+from snakestream.exception import StreamBuildException
+
+
+async def async_flat_map(x: int) -> int:
+    await asyncio.sleep(0.01)
+    return x
 
 
 @pytest.mark.asyncio
-async def test_map(int_2_letter) -> None:
+async def test_flat_map() -> None:
     # when
-    it = stream_of([1, 2, 3, 4]) \
-        .map(lambda x: int_2_letter[x]) \
+    it = Stream.of([[1, 2], [3, 4]]) \
+        .flat_map(lambda x: Stream.of(x)) \
         .collect(to_generator)
 
     # then
-    assert await it.__anext__() == 'a'
-    assert await it.__anext__() == 'b'
-    assert await it.__anext__() == 'c'
-    assert await it.__anext__() == 'd'
+    assert await it.__anext__() == 1
+    assert await it.__anext__() == 2
+    assert await it.__anext__() == 3
+    assert await it.__anext__() == 4
     try:
         await it.__anext__()
     except StopAsyncIteration:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_map_async_function(async_int_to_letter) -> None:
-    async_int_to_letter = await async_int_to_letter
-
-    # when
-    it = stream_of([1, 2, 3, 4]) \
-        .map(async_int_to_letter) \
+async def test_flat_map_no_mixed_list() -> None:
+    it = Stream.of([[1, 2], [3, 4], 5]) \
+        .flat_map(lambda x: Stream.of(x)) \
         .collect(to_generator)
 
     # then
-    assert await it.__anext__() == 'a'
-    assert await it.__anext__() == 'b'
-    assert await it.__anext__() == 'c'
-    assert await it.__anext__() == 'd'
+    assert await it.__anext__() == 1
+    assert await it.__anext__() == 2
+    assert await it.__anext__() == 3
+    assert await it.__anext__() == 4
     try:
         await it.__anext__()
-    except StopAsyncIteration:
+    except TypeError:
         pass
     else:
         assert False
 
 
 @pytest.mark.asyncio
-async def test_map_does_not_mutate_source(int_2_letter) -> None:
-    source = [1, 2, 3, 4]
-
+async def test_flat_map_async_function() -> None:
     # when
-    it = await stream_of(source) \
-        .map(lambda x: int_2_letter[x]) \
-        .collect(to_list)
-
-    # then
-    assert source != it
-    assert len(source) == 4
-    assert len(it) == 4
+    try:
+        Stream.of([[1, 2], [3, 4], 5]) \
+            .flat_map(async_flat_map) \
+            .collect(to_generator)
+    except StreamBuildException:
+        pass
+    else:
+        assert False
```

### Comparing `snakestream-0.2.3/tests/test_max.py` & `snakestream-0.3.0/tests/test_max.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 import pytest
 import asyncio
 
-from snakestream import stream_of
+from snakestream import Stream
 from conftest import MyObject
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_normal_input():
     input_list = [1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x > y)
     # then
     assert it == 5
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_async_input():
     async def async_comparator(x: int, y: int) -> bool:
         await asyncio.sleep(0.01)
         return x > y
 
     input_list = [1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(async_comparator)
     # then
     assert it == 5
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_empty_input():
     input_list = []
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x > y)
     # then
     assert it is None
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_list_with_dupe_items():
     input_list = [1, 1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x > y)
     # then
     assert it == 5
 
     input_list = [1, 2, 3, 4, 5, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x > y)
     # then
     assert it == 5
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_negative_values():
     input_list = [-1, -2, -3, -4, -5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x > y)
     # then
     assert it == -1
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_custom_comparator():
     input_list = ['a', 'bb', 'ccc']
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: len(x) > len(y))
     # then
     assert it == 'ccc'
 
 
 @pytest.mark.asyncio
 async def test_find_max_value_object_comparator() -> None:
     # when
     input_list = [MyObject(1, "object1"), MyObject(2, "object2"), MyObject(3, "object3"), MyObject(2, "object2"),
                   MyObject(3, "object3")]
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .max(lambda x, y: x.id > y.id)
     # then
     assert it == MyObject(3, "object3")
```

### Comparing `snakestream-0.2.3/tests/test_min.py` & `snakestream-0.3.0/tests/test_min.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 import pytest
 import asyncio
 
-from snakestream import stream_of
+from snakestream import Stream
 from conftest import MyObject
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_normal_input():
     input_list = [1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x > y)
     # then
     assert it == 1
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_async_input():
     async def async_comparator(x: int, y: int) -> bool:
         await asyncio.sleep(0.01)
         return x > y
 
     input_list = [1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(async_comparator)
     # then
     assert it == 1
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_empty_input():
     input_list = []
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x > y)
     # then
     assert it is None
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_list_with_dupe_items():
     input_list = [1, 1, 2, 3, 4, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x > y)
     # then
     assert it == 1
 
     input_list = [1, 2, 3, 4, 5, 5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x > y)
     # then
     assert it == 1
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_negative_values():
     input_list = [-1, -2, -3, -4, -5]
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x > y)
     # then
     assert it == -5
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_custom_comparator():
     input_list = ['a', 'bb', 'ccc']
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: len(x) > len(y))
     # then
     assert it == 'a'
 
 
 @pytest.mark.asyncio
 async def test_find_min_value_object_comparator() -> None:
     # when
     input_list = [MyObject(1, "object1"), MyObject(2, "object2"), MyObject(3, "object3"), MyObject(2, "object2"),
                   MyObject(3, "object3")]
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .min(lambda x, y: x.id > y.id)
     # then
     assert it == MyObject(1, "object1")
```

### Comparing `snakestream-0.2.3/tests/test_peek.py` & `snakestream-0.3.0/tests/test_peek.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
 import pytest
 
 from conftest import MyObject
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_list
 
 obj1 = MyObject(1, "Object1")
 obj2 = MyObject(2, "Object2")
 obj3 = MyObject(3, "Object3")
 
 
@@ -19,15 +19,15 @@
     obj3,
 ]
 
 
 @pytest.mark.asyncio
 async def test_ok() -> None:
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .peek(lambda x: x) \
         .collect(to_list)
     # then
     assert it == input_list
     assert it[0] is input_list[0]
     assert it[1] is input_list[1]
     assert it[2] is input_list[2]
@@ -41,15 +41,15 @@
 
     async def some_func(x: MyObject) -> None:
         await asyncio.sleep(0.01)
         names.append(x.name)
         return
 
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .peek(some_func) \
         .collect(to_list)
     # then
     assert it == input_list
     assert it[0] is input_list[0]
     assert it[1] is input_list[1]
     assert it[2] is input_list[2]
@@ -58,25 +58,25 @@
 
     assert names == ['Object1', 'Object2', 'Object3', 'Object2', 'Object3',]
 
 
 @pytest.mark.asyncio
 async def test_empty_stream() -> None:
     # when
-    it = await stream_of([]) \
+    it = await Stream.of([]) \
         .peek(lambda x: x) \
         .collect(to_list)
     # then
     assert it == []
 
 
 @pytest.mark.asyncio
 async def test_multiple_calls() -> None:
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .peek(lambda x: x) \
         .peek(lambda x: x) \
         .collect(to_list)
     # then
     assert it == input_list
     assert it[0] is input_list[0]
     assert it[1] is input_list[1]
@@ -87,15 +87,15 @@
 
 @pytest.mark.asyncio
 async def test_mutate_internal_state() -> None:
     def lower_name(x: MyObject) -> None:
         x.name = x.name.lower()
 
     # when
-    it = await stream_of(input_list) \
+    it = await Stream.of(input_list) \
         .peek(lower_name) \
         .collect(to_list)
     # then
     assert it == input_list
     assert it[0] is input_list[0]
     assert it[1] is input_list[1]
     assert it[2] is input_list[2]
```

### Comparing `snakestream-0.2.3/tests/test_reduce.py` & `snakestream-0.3.0/tests/test_reduce.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import asyncio
 
 import pytest
 
-from snakestream import stream_of
+from snakestream import Stream
 
 
 @pytest.mark.asyncio
 async def test_reducer() -> None:
     # when
-    it = stream_of([1, 2, 3, 4, 5, 6]) \
+    it = Stream.of([1, 2, 3, 4, 5, 6]) \
         .reduce(0, lambda x, y: x + y)
     # then
     assert await it == 21
 
 
 @pytest.mark.asyncio
 async def test_reducer_associative() -> None:
     # when
-    it = stream_of([1, 2, 3, 4, 5, 6]) \
+    it = Stream.of([1, 2, 3, 4, 5, 6]) \
         .reduce(0, lambda x, y: x + y)
 
-    it2 = stream_of([1, 2, 3, 4, 5, 6]) \
+    it2 = Stream.of([1, 2, 3, 4, 5, 6]) \
         .reduce(0, lambda x, y: y + x)
     # then
     assert await it == 21
     assert await it2 == 21
 
 
 @pytest.mark.asyncio
 async def test_async_reducer() -> None:
     async def async_reducer(x: int, y: int):
         await asyncio.sleep(0.01)
         return x + y
 
     # when
-    it = stream_of([1, 2, 3, 4, 5, 6]) \
+    it = Stream.of([1, 2, 3, 4, 5, 6]) \
         .reduce(0, async_reducer)
 
     # then
     assert await it == 21
 
 
 @pytest.mark.asyncio
 async def test_reducer_mixed_chain(letter_2_int) -> None:
     # when
-    it = stream_of(['a', 'b', 'c', 'd']) \
+    it = Stream.of(['a', 'b', 'c', 'd']) \
         .map(lambda x: letter_2_int[x]) \
         .reduce(0, lambda x, y: x + y)
     # then
     assert await it == 10
```

### Comparing `snakestream-0.2.3/tests/test_sorted.py` & `snakestream-0.3.0/tests/test_sorted.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pytest
 import asyncio
 
-from snakestream import stream_of
+from snakestream import Stream
 from snakestream.collector import to_list
 
 
 @pytest.mark.asyncio
 async def test_sorted() -> None:
     outset = [1, 5, 3, 4, 5, 2]
 
-    actual = await stream_of(outset) \
+    actual = await Stream.of(outset) \
         .sorted() \
         .collect(to_list)
 
     assert sorted(outset) == actual
 
 
 @pytest.mark.asyncio
 async def test_sorted_reverse() -> None:
     outset = [1, 5, 3, 4, 5, 2]
 
-    actual = await stream_of(outset) \
+    actual = await Stream.of(outset) \
         .sorted(reverse=True) \
         .collect(to_list)
 
     assert sorted(outset, reverse=True) == actual
 
 
 @pytest.mark.asyncio
@@ -39,15 +39,15 @@
         if a['x'] > b['x']:
             return 1
         elif a['x'] < b['x']:
             return -1
         else:
             return 0
 
-    actual = await stream_of(outset) \
+    actual = await Stream.of(outset) \
         .sorted(comparator=compare) \
         .collect(to_list)
 
     assert sorted(outset, key=lambda x: x['x']) == actual
 
 
 @pytest.mark.asyncio
@@ -63,15 +63,15 @@
         if a['x'] == b['x']:
             return 0
         elif a['x'] > b['x']:
             return 1
         else:
             return -1
 
-    actual = await stream_of(outset) \
+    actual = await Stream.of(outset) \
         .sorted(comparator=compare_async, reverse=True) \
         .collect(to_list)
 
     assert actual == [
         {'x': 3, 'y': 7},
         {'x': 2, 'y': 6},
         {'x': 1, 'y': 5},
```

