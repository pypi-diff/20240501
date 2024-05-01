# Comparing `tmp/texase-0.1.0.tar.gz` & `tmp/texase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texase-0.1.0.tar", max compression
+gzip compressed data, was "texase-0.2.0.tar", max compression
```

## Comparing `texase-0.1.0.tar` & `texase-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0    16725 2023-01-24 14:04:39.612429 texase-0.1.0/LICENSE
--rw-r--r--   0        0        0     2937 2024-05-01 09:47:24.672289 texase-0.1.0/README.md
--rw-r--r--   0        0        0      742 2024-04-18 10:43:32.047117 texase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-20 09:56:04.735642 texase-0.1.0/src/texase/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-15 13:19:52.017845 texase-0.1.0/src/texase/addcolumn.py
--rw-r--r--   0        0        0    21660 2024-05-01 12:19:03.886302 texase-0.1.0/src/texase/app.py
--rw-r--r--   0        0        0    30660 2024-05-01 09:32:20.082288 texase-0.1.0/src/texase/data.py
--rw-r--r--   0        0        0    11362 2024-04-15 13:07:22.831432 texase-0.1.0/src/texase/details.py
--rw-r--r--   0        0        0     1951 2024-04-19 11:50:01.149990 texase-0.1.0/src/texase/edit.py
--rw-r--r--   0        0        0     4681 2024-05-01 10:40:14.618565 texase-0.1.0/src/texase/files_io.py
--rw-r--r--   0        0        0     8166 2024-04-15 13:19:52.024512 texase-0.1.0/src/texase/filter.py
--rw-r--r--   0        0        0     6056 2024-04-30 08:08:52.985278 texase-0.1.0/src/texase/formatting.py
--rw-r--r--   0        0        0     2982 2024-04-19 11:50:01.149990 texase-0.1.0/src/texase/help.py
--rw-r--r--   0        0        0     4629 2024-04-19 11:50:01.149990 texase-0.1.0/src/texase/input_screens.py
--rw-r--r--   0        0        0     1515 2024-04-15 13:19:52.017845 texase-0.1.0/src/texase/keys.py
--rw-r--r--   0        0        0     1153 2024-01-12 13:42:58.119376 texase-0.1.0/src/texase/saved_columns.py
--rw-r--r--   0        0        0     2950 2024-04-15 13:19:52.024512 texase-0.1.0/src/texase/search.py
--rw-r--r--   0        0        0    15826 2024-04-30 08:53:17.043266 texase-0.1.0/src/texase/table.py
--rw-r--r--   0        0        0     1554 2024-04-15 13:19:52.017845 texase-0.1.0/src/texase/table_add_column.py
--rw-r--r--   0        0        0     1493 2024-04-22 13:00:08.811859 texase-0.1.0/src/texase/table_update_from_thread.py
--rw-r--r--   0        0        0     2062 2024-04-19 11:50:01.149990 texase-0.1.0/src/texase/texase.tcss
--rw-r--r--   0        0        0     1243 2024-04-10 12:28:41.943822 texase-0.1.0/src/texase/validators.py
--rw-r--r--   0        0        0     1122 2024-04-15 13:19:52.024512 texase-0.1.0/src/texase/yesno.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 texase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-01 19:37:53.728919 texase-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2937 2024-05-01 19:37:53.728919 texase-0.2.0/README.md
+-rw-r--r--   0        0        0      742 2024-05-01 19:37:53.740919 texase-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/addcolumn.py
+-rw-r--r--   0        0        0    21660 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/app.py
+-rw-r--r--   0        0        0    30660 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/data.py
+-rw-r--r--   0        0        0    11362 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/details.py
+-rw-r--r--   0        0        0     1951 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/edit.py
+-rw-r--r--   0        0        0     4681 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/files_io.py
+-rw-r--r--   0        0        0     8166 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/filter.py
+-rw-r--r--   0        0        0     6056 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/formatting.py
+-rw-r--r--   0        0        0     2982 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/help.py
+-rw-r--r--   0        0        0     4629 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/input_screens.py
+-rw-r--r--   0        0        0     1515 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/keys.py
+-rw-r--r--   0        0        0     1153 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/saved_columns.py
+-rw-r--r--   0        0        0     2950 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/search.py
+-rw-r--r--   0        0        0    15826 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/table.py
+-rw-r--r--   0        0        0     2062 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/texase.tcss
+-rw-r--r--   0        0        0     1243 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/validators.py
+-rw-r--r--   0        0        0     1122 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/yesno.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 texase-0.2.0/PKG-INFO
```

### Comparing `texase-0.1.0/LICENSE` & `texase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/README.md` & `texase-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/pyproject.toml` & `texase-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "texase"
-version = "0.1.0"
+version = "0.2.0"
 description = "Textual user interface for ASE db."
 authors = ["Steen Lysgaard <stly@dtu.dk>"]
 license = "MPL"
 readme = "README.md"
 packages = [{include = "texase", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `texase-0.1.0/src/texase/addcolumn.py` & `texase-0.2.0/src/texase/addcolumn.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/app.py` & `texase-0.2.0/src/texase/app.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/data.py` & `texase-0.2.0/src/texase/data.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/details.py` & `texase-0.2.0/src/texase/details.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/edit.py` & `texase-0.2.0/src/texase/edit.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/files_io.py` & `texase-0.2.0/src/texase/files_io.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/filter.py` & `texase-0.2.0/src/texase/filter.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/formatting.py` & `texase-0.2.0/src/texase/formatting.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/help.py` & `texase-0.2.0/src/texase/help.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/input_screens.py` & `texase-0.2.0/src/texase/input_screens.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/keys.py` & `texase-0.2.0/src/texase/keys.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/saved_columns.py` & `texase-0.2.0/src/texase/saved_columns.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/search.py` & `texase-0.2.0/src/texase/search.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/table.py` & `texase-0.2.0/src/texase/table.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/texase.tcss` & `texase-0.2.0/src/texase/texase.tcss`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/validators.py` & `texase-0.2.0/src/texase/validators.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/src/texase/yesno.py` & `texase-0.2.0/src/texase/yesno.py`

 * *Files identical despite different names*

### Comparing `texase-0.1.0/PKG-INFO` & `texase-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: texase
-Version: 0.1.0
+Version: 0.2.0
 Summary: Textual user interface for ASE db.
 License: MPL
 Author: Steen Lysgaard
 Author-email: stly@dtu.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ase (>=3.19.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pytest-xvfb (>=3.0.0,<4.0.0)
 Requires-Dist: textual (==0.52.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

