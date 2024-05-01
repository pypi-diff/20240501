# Comparing `tmp/NewareNDA-2024.4.1.tar.gz` & `tmp/newarenda-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewareNDA-2024.4.1.tar", last modified: Mon Apr  1 13:51:41 2024, max compression
+gzip compressed data, was "newarenda-2024.5.1.tar", last modified: Wed May  1 18:20:30 2024, max compression
```

## Comparing `NewareNDA-2024.4.1.tar` & `newarenda-2024.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 NewareNDA-2024.4.1/LICENSE
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.051063 NewareNDA-2024.4.1/NewareNDA/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    11344 2024-03-26 18:47:09.000000 NewareNDA-2024.4.1/NewareNDA/NewareNDA.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    14809 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/NewareNDA/NewareNDAx.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      101 2023-10-03 15:33:50.000000 NewareNDA-2024.4.1/NewareNDA/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1677 2024-04-01 13:48:28.000000 NewareNDA-2024.4.1/NewareNDA/dicts.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2024-04-01 13:48:28.000000 NewareNDA-2024.4.1/NewareNDA/version.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/NewareNDA.egg-info/
--rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      344 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/SOURCES.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/dependency_links.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       40 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/requires.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2024-04-01 13:51:41.000000 NewareNDA-2024.4.1/NewareNDA.egg-info/top_level.txt
--rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1734 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/README.md
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.051063 NewareNDA-2024.4.1/bin/
--rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-10-03 15:33:50.000000 NewareNDA-2024.4.1/bin/NewareNDA-cli.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/setup.cfg
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      968 2024-04-01 13:41:36.000000 NewareNDA-2024.4.1/setup.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-01 13:51:41.055063 NewareNDA-2024.4.1/tests/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      209 2024-03-08 19:10:17.000000 NewareNDA-2024.4.1/tests/test_NewareNDA.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-05-01 18:20:30.724565 newarenda-2024.5.1/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 newarenda-2024.5.1/LICENSE
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-05-01 18:20:30.720565 newarenda-2024.5.1/NewareNDA/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    11065 2024-05-01 18:16:37.000000 newarenda-2024.5.1/NewareNDA/NewareNDA.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    14809 2024-05-01 18:10:41.000000 newarenda-2024.5.1/NewareNDA/NewareNDAx.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      101 2023-10-03 15:33:50.000000 newarenda-2024.5.1/NewareNDA/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1677 2024-04-03 15:07:49.000000 newarenda-2024.5.1/NewareNDA/dicts.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2024-05-01 18:16:37.000000 newarenda-2024.5.1/NewareNDA/version.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-05-01 18:20:30.724565 newarenda-2024.5.1/NewareNDA.egg-info/
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-05-01 18:20:30.000000 newarenda-2024.5.1/NewareNDA.egg-info/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      344 2024-05-01 18:20:30.000000 newarenda-2024.5.1/NewareNDA.egg-info/SOURCES.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2024-05-01 18:20:30.000000 newarenda-2024.5.1/NewareNDA.egg-info/dependency_links.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       40 2024-05-01 18:20:30.000000 newarenda-2024.5.1/NewareNDA.egg-info/requires.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2024-05-01 18:20:30.000000 newarenda-2024.5.1/NewareNDA.egg-info/top_level.txt
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     2271 2024-05-01 18:20:30.724565 newarenda-2024.5.1/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1734 2024-04-03 15:07:49.000000 newarenda-2024.5.1/README.md
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-05-01 18:20:30.720565 newarenda-2024.5.1/bin/
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-10-03 15:33:50.000000 newarenda-2024.5.1/bin/NewareNDA-cli.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2024-05-01 18:20:30.724565 newarenda-2024.5.1/setup.cfg
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      968 2024-04-03 15:07:49.000000 newarenda-2024.5.1/setup.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-05-01 18:20:30.720565 newarenda-2024.5.1/tests/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      209 2024-04-23 15:09:47.000000 newarenda-2024.5.1/tests/test_NewareNDA.py
```

### Comparing `NewareNDA-2024.4.1/LICENSE` & `newarenda-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.4.1/NewareNDA/NewareNDA.py` & `newarenda-2024.5.1/NewareNDA/NewareNDA.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,17 @@
             mm.seek(50, 1)
             client = mm.read(50).strip(b'\x00').decode()
             logging.info(f"Client: {client}")
         else:
             logging.info("BTS version not found!")
 
         # version specific settings
-        if nda_version < 130:
+        if nda_version == 8:
+            raise NotImplementedError("nda version 8 is not supported!")
+        elif nda_version < 130:
             output, aux = _read_nda(mm)
         else:
             output, aux = _read_nda_130(mm)
 
     # Create DataFrame and sort by Index
     df = pd.DataFrame(output, columns=rec_columns)
     df.drop_duplicates(subset='Index', inplace=True)
@@ -148,24 +150,16 @@
 
 def _read_nda_130(mm):
     """Helper function for nda version 130"""
     mm_size = mm.size()
 
     # Identify the beginning of the data section
     record_len = 88
-    identifier = b'\x1d\xf0\x00\x06\x55\x81'
-    header = mm.find(identifier)
-    if header == -1:
-        raise EOFError("File does not contain any valid records.")
-    while (((mm[header + 4 + record_len] != 85)
-            | (not _valid_record(mm[header+4:header+4+record_len])))
-            if header + 4 + record_len < mm_size
-            else False):
-        header = mm.find(identifier, header + 4)
-    mm.seek(header)
+    identifier = mm[1024:1030]
+    mm.seek(1024)
 
     # Read data records
     output = []
     aux = []
     while mm.tell() < mm_size:
         bytes = mm.read(record_len)
         if len(bytes) == record_len:
```

### Comparing `NewareNDA-2024.4.1/NewareNDA/NewareNDAx.py` & `newarenda-2024.5.1/NewareNDA/NewareNDAx.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.4.1/NewareNDA/dicts.py` & `newarenda-2024.5.1/NewareNDA/dicts.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.4.1/NewareNDA.egg-info/PKG-INFO` & `newarenda-2024.5.1/NewareNDA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `NewareNDA-2024.4.1/PKG-INFO` & `newarenda-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `NewareNDA-2024.4.1/README.md` & `newarenda-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.4.1/bin/NewareNDA-cli.py` & `newarenda-2024.5.1/bin/NewareNDA-cli.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2024.4.1/setup.py` & `newarenda-2024.5.1/setup.py`

 * *Files identical despite different names*

