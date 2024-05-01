# Comparing `tmp/pybangla-0.0.3.tar.gz` & `tmp/pybangla-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-0.0.3.tar", last modified: Wed May  1 18:16:33 2024, max compression
+gzip compressed data, was "pybangla-0.0.4.tar", last modified: Wed May  1 18:21:50 2024, max compression
```

## Comparing `pybangla-0.0.3.tar` & `pybangla-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:26.000000 pybangla-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:16:33.281125 pybangla-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-05-01 18:16:26.000000 pybangla-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.277125 pybangla-0.0.3/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:16:33.281125 pybangla-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 18:16:26.000000 pybangla-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-01 18:16:26.000000 pybangla-0.0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:42.000000 pybangla-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:21:50.770495 pybangla-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-05-01 18:21:42.000000 pybangla-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.766495 pybangla-0.0.4/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-01 18:21:42.000000 pybangla-0.0.4/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:21:50.000000 pybangla-0.0.4/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:21:50.770495 pybangla-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 18:21:42.000000 pybangla-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:21:50.770495 pybangla-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-01 18:21:42.000000 pybangla-0.0.4/tests/test.py
```

### Comparing `pybangla-0.0.3/PKG-INFO` & `pybangla-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.3
+Version: 0.0.4
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-0.0.3/README.md` & `pybangla-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/config.py` & `pybangla-0.0.4/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/date_extractor.py` & `pybangla-0.0.4/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/main.py` & `pybangla-0.0.4/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/number_parser.py` & `pybangla-0.0.4/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/parser.py` & `pybangla-0.0.4/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/module/word_to_number.py` & `pybangla-0.0.4/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla/test.py` & `pybangla-0.0.4/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.3/pybangla.egg-info/PKG-INFO` & `pybangla-0.0.4/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.3
+Version: 0.0.4
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-0.0.3/setup.py` & `pybangla-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-0.0.3/tests/test.py` & `pybangla-0.0.4/tests/test.py`

 * *Files identical despite different names*

