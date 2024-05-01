# Comparing `tmp/nmrpype-0.8.0.tar.gz` & `tmp/nmrpype-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmrpype-0.8.0.tar", last modified: Wed May  1 17:47:46 2024, max compression
+gzip compressed data, was "nmrpype-0.8.1.tar", last modified: Wed May  1 19:04:53 2024, max compression
```

## Comparing `nmrpype-0.8.0.tar` & `nmrpype-0.8.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     3113 2024-05-01 17:43:04.000000 nmrpype-0.8.0/LICENSE
--rw-r--r--   0 mykah     (1000) mykah     (1000)      710 2024-05-01 17:47:46.991933 nmrpype-0.8.0/PKG-INFO
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      107 2024-05-01 17:29:48.000000 nmrpype-0.8.0/README.md
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.987933 nmrpype-0.8.0/nmrPype/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      169 2024-02-15 13:54:00.000000 nmrpype-0.8.0/nmrPype/__init__.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.987933 nmrpype-0.8.0/nmrPype/fn/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     6035 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/fn/DI.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    11112 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/fn/FT.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     7895 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/fn/PS.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    12366 2024-04-26 13:34:20.000000 nmrpype-0.8.0/nmrPype/fn/SP.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    21458 2024-04-26 13:34:20.000000 nmrpype-0.8.0/nmrPype/fn/TP.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    14491 2024-04-26 13:34:20.000000 nmrpype-0.8.0/nmrPype/fn/ZF.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      683 2024-05-01 17:07:34.000000 nmrpype-0.8.0/nmrPype/fn/__init__.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     7295 2024-04-26 13:34:20.000000 nmrpype-0.8.0/nmrPype/fn/function.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/nmrPype/nmrio/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     7761 2024-05-01 17:07:34.000000 nmrpype-0.8.0/nmrPype/nmrio/__init__.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    23256 2024-02-15 13:54:00.000000 nmrpype-0.8.0/nmrPype/nmrio/fileiobase.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     9687 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/nmrio/read.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    10240 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/nmrio/write.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/nmrPype/parse/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)       48 2024-02-15 13:54:00.000000 nmrpype-0.8.0/nmrPype/parse/__init__.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     3112 2024-04-26 13:35:04.000000 nmrpype-0.8.0/nmrPype/parse/parser.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     5941 2024-05-01 17:07:34.000000 nmrpype-0.8.0/nmrPype/pype.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/nmrPype/utils/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     7985 2024-05-01 17:07:34.000000 nmrpype-0.8.0/nmrPype/utils/DataFrame.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      244 2024-02-15 13:54:00.000000 nmrpype-0.8.0/nmrPype/utils/__init__.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)     2283 2024-03-26 12:56:30.000000 nmrpype-0.8.0/nmrPype/utils/errorHandler.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/nmrPype/utils/fdata/
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      622 2024-02-15 13:54:00.000000 nmrpype-0.8.0/nmrPype/utils/fdata/__init__.py
--rw-rw-r--   0 mykah     (1000) mykah     (1000)    38480 2024-04-22 18:17:53.000000 nmrpype-0.8.0/nmrPype/utils/fdata/datamanip.py
-drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 17:47:46.991933 nmrpype-0.8.0/nmrPype.egg-info/
--rw-r--r--   0 mykah     (1000) mykah     (1000)      710 2024-05-01 17:47:46.000000 nmrpype-0.8.0/nmrPype.egg-info/PKG-INFO
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      646 2024-05-01 17:47:46.000000 nmrpype-0.8.0/nmrPype.egg-info/SOURCES.txt
--rw-rw-r--   0 mykah     (1000) mykah     (1000)        1 2024-05-01 17:47:46.000000 nmrpype-0.8.0/nmrPype.egg-info/dependency_links.txt
--rw-rw-r--   0 mykah     (1000) mykah     (1000)        8 2024-05-01 17:47:46.000000 nmrpype-0.8.0/nmrPype.egg-info/top_level.txt
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      657 2024-05-01 17:43:43.000000 nmrpype-0.8.0/pyproject.toml
--rw-rw-r--   0 mykah     (1000) mykah     (1000)       38 2024-05-01 17:47:46.991933 nmrpype-0.8.0/setup.cfg
--rw-rw-r--   0 mykah     (1000) mykah     (1000)      489 2024-05-01 17:07:34.000000 nmrpype-0.8.0/setup.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     3113 2024-05-01 17:43:04.000000 nmrpype-0.8.1/LICENSE
+-rw-r--r--   0 mykah     (1000) mykah     (1000)      776 2024-05-01 19:04:53.574836 nmrpype-0.8.1/PKG-INFO
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      107 2024-05-01 17:29:48.000000 nmrpype-0.8.1/README.md
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.570836 nmrpype-0.8.1/nmrPype/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      169 2024-02-15 13:54:00.000000 nmrpype-0.8.1/nmrPype/__init__.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype/fn/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     6035 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/fn/DI.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    11112 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/fn/FT.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     7895 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/fn/PS.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    12366 2024-04-26 13:34:20.000000 nmrpype-0.8.1/nmrPype/fn/SP.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    21458 2024-04-26 13:34:20.000000 nmrpype-0.8.1/nmrPype/fn/TP.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    14491 2024-04-26 13:34:20.000000 nmrpype-0.8.1/nmrPype/fn/ZF.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      683 2024-05-01 17:07:34.000000 nmrpype-0.8.1/nmrPype/fn/__init__.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     7295 2024-04-26 13:34:20.000000 nmrpype-0.8.1/nmrPype/fn/function.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype/nmrio/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     7761 2024-05-01 17:07:34.000000 nmrpype-0.8.1/nmrPype/nmrio/__init__.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    23256 2024-02-15 13:54:00.000000 nmrpype-0.8.1/nmrPype/nmrio/fileiobase.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     9687 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/nmrio/read.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    10240 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/nmrio/write.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype/parse/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)       48 2024-02-15 13:54:00.000000 nmrpype-0.8.1/nmrPype/parse/__init__.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     3112 2024-04-26 13:35:04.000000 nmrpype-0.8.1/nmrPype/parse/parser.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     5941 2024-05-01 17:07:34.000000 nmrpype-0.8.1/nmrPype/pype.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype/utils/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     7985 2024-05-01 17:07:34.000000 nmrpype-0.8.1/nmrPype/utils/DataFrame.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      244 2024-02-15 13:54:00.000000 nmrpype-0.8.1/nmrPype/utils/__init__.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)     2283 2024-03-26 12:56:30.000000 nmrpype-0.8.1/nmrPype/utils/errorHandler.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype/utils/fdata/
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      622 2024-02-15 13:54:00.000000 nmrpype-0.8.1/nmrPype/utils/fdata/__init__.py
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)    38480 2024-04-22 18:17:53.000000 nmrpype-0.8.1/nmrPype/utils/fdata/datamanip.py
+drwxrwxr-x   0 mykah     (1000) mykah     (1000)        0 2024-05-01 19:04:53.574836 nmrpype-0.8.1/nmrPype.egg-info/
+-rw-r--r--   0 mykah     (1000) mykah     (1000)      776 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/PKG-INFO
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      710 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/SOURCES.txt
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)        1 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/dependency_links.txt
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)       46 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/entry_points.txt
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)       12 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/requires.txt
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)        8 2024-05-01 19:04:53.000000 nmrpype-0.8.1/nmrPype.egg-info/top_level.txt
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      779 2024-05-01 19:04:44.000000 nmrpype-0.8.1/pyproject.toml
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)       38 2024-05-01 19:04:53.574836 nmrpype-0.8.1/setup.cfg
+-rw-rw-r--   0 mykah     (1000) mykah     (1000)      490 2024-05-01 19:02:58.000000 nmrpype-0.8.1/setup.py
```

### Comparing `nmrpype-0.8.0/LICENSE` & `nmrpype-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/DI.py` & `nmrpype-0.8.1/nmrPype/fn/DI.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/FT.py` & `nmrpype-0.8.1/nmrPype/fn/FT.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/PS.py` & `nmrpype-0.8.1/nmrPype/fn/PS.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/SP.py` & `nmrpype-0.8.1/nmrPype/fn/SP.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/TP.py` & `nmrpype-0.8.1/nmrPype/fn/TP.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/ZF.py` & `nmrpype-0.8.1/nmrPype/fn/ZF.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/__init__.py` & `nmrpype-0.8.1/nmrPype/fn/__init__.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/fn/function.py` & `nmrpype-0.8.1/nmrPype/fn/function.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/nmrio/__init__.py` & `nmrpype-0.8.1/nmrPype/nmrio/__init__.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/nmrio/fileiobase.py` & `nmrpype-0.8.1/nmrPype/nmrio/fileiobase.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/nmrio/read.py` & `nmrpype-0.8.1/nmrPype/nmrio/read.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/nmrio/write.py` & `nmrpype-0.8.1/nmrPype/nmrio/write.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/parse/parser.py` & `nmrpype-0.8.1/nmrPype/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/pype.py` & `nmrpype-0.8.1/nmrPype/pype.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/utils/DataFrame.py` & `nmrpype-0.8.1/nmrPype/utils/DataFrame.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/utils/errorHandler.py` & `nmrpype-0.8.1/nmrPype/utils/errorHandler.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/utils/fdata/__init__.py` & `nmrpype-0.8.1/nmrPype/utils/fdata/__init__.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype/utils/fdata/datamanip.py` & `nmrpype-0.8.1/nmrPype/utils/fdata/datamanip.py`

 * *Files identical despite different names*

### Comparing `nmrpype-0.8.0/nmrPype.egg-info/SOURCES.txt` & `nmrpype-0.8.1/nmrPype.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 pyproject.toml
 setup.py
 nmrPype/__init__.py
 nmrPype/pype.py
 nmrPype.egg-info/PKG-INFO
 nmrPype.egg-info/SOURCES.txt
 nmrPype.egg-info/dependency_links.txt
+nmrPype.egg-info/entry_points.txt
+nmrPype.egg-info/requires.txt
 nmrPype.egg-info/top_level.txt
 nmrPype/fn/DI.py
 nmrPype/fn/FT.py
 nmrPype/fn/PS.py
 nmrPype/fn/SP.py
 nmrPype/fn/TP.py
 nmrPype/fn/ZF.py
```

