# Comparing `tmp/colony-print-0.3.0.tar.gz` & `tmp/colony-print-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colony-print-0.3.0.tar", last modified: Tue Apr 30 14:28:37 2024, max compression
+gzip compressed data, was "dist/colony-print-0.3.1.tar", last modified: Wed May  1 11:28:07 2024, max compression
```

## Comparing `colony-print-0.3.0.tar` & `colony-print-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1979 2024-04-30 14:28:07.000000 colony-print-0.3.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     2971 2024-04-30 14:28:07.000000 colony-print-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 14:28:37.000000 colony-print-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4677 2024-04-30 14:28:37.000000 colony-print-0.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4677 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:28:33.000000 colony-print-0.3.0/src/colony_print.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/binie/
--rw-r--r--   0 root         (0) root         (0)      875 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/system.py
--rw-r--r--   0 root         (0) root         (0)      263 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20906 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/visitor.py
--rw-r--r--   0 root         (0) root         (0)      870 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/manager/
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/system.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/ast.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/parser.py
--rw-r--r--   0 root         (0) root         (0)     2787 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/visitor.py
--rw-r--r--   0 root         (0) root         (0)      874 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      222 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/common/
--rw-r--r--   0 root         (0) root         (0)     2712 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/common/base.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/pdf/
--rw-r--r--   0 root         (0) root         (0)      969 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/system.py
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33965 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/visitor.py
--rw-r--r--   0 root         (0) root         (0)     1462 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/js/
--rw-r--r--   0 root         (0) root         (0)     3555 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/js/main.js
--rw-r--r--   0 root         (0) root         (0)      594 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/print.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/xml/
--rw-r--r--   0 root         (0) root         (0)      251 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/xml/hello.xml
--rw-r--r--   0 root         (0) root         (0)    26876 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/xml/money_sale_slip.xml
--rw-r--r--   0 root         (0) root         (0)     3210 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/node.py
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/__init__.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/controllers/
--rw-r--r--   0 root         (0) root         (0)      117 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/base.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/printer.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/node.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2790 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1979 2024-05-01 11:27:36.000000 colony-print-0.3.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-05-01 11:27:36.000000 colony-print-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-01 11:28:07.000000 colony-print-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-05-01 11:28:07.000000 colony-print-0.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 11:28:03.000000 colony-print-0.3.1/src/colony_print.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/printing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/printing/binie/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/binie/system.py
+-rw-r--r--   0 root         (0) root         (0)      263 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/binie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20906 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/binie/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      870 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/binie/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/printing/manager/
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/system.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/ast.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/printing/common/
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/common/base.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/printing/pdf/
+-rw-r--r--   0 root         (0) root         (0)      969 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/pdf/system.py
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/pdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33965 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/pdf/visitor.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/printing/pdf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/static/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/static/example/js/
+-rw-r--r--   0 root         (0) root         (0)     3555 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/static/example/js/main.js
+-rw-r--r--   0 root         (0) root         (0)      594 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/static/example/print.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/static/example/xml/
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/static/example/xml/hello.xml
+-rw-r--r--   0 root         (0) root         (0)    26876 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/static/example/xml/money_sale_slip.xml
+-rw-r--r--   0 root         (0) root         (0)     5972 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/node.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:28:07.000000 colony-print-0.3.1/src/colony_print/controllers/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/controllers/base.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/controllers/printer.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/controllers/node.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-01 11:27:36.000000 colony-print-0.3.1/src/colony_print/controllers/document.py
```

### Comparing `colony-print-0.3.0/setup.py` & `colony-print-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
     name="colony-print",
-    version="0.3.0",
+    version="0.3.1",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Colony Print Infra-structure",
     license="Apache License, Version 2.0",
     keywords="colony print native",
     url="http://colony-print.hive.pt",
     zip_safe=False,
```

### Comparing `colony-print-0.3.0/README.md` & `colony-print-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/PKG-INFO` & `colony-print-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colony-print
-Version: 0.3.0
+Version: 0.3.1
 Summary: Colony Print Infra-structure
 Home-page: http://colony-print.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Print Infra-structure](http://colony-print.hive.pt)
```

### Comparing `colony-print-0.3.0/src/colony_print.egg-info/SOURCES.txt` & `colony-print-0.3.1/src/colony_print.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print.egg-info/PKG-INFO` & `colony-print-0.3.1/src/colony_print.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colony-print
-Version: 0.3.0
+Version: 0.3.1
 Summary: Colony Print Infra-structure
 Home-page: http://colony-print.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Print Infra-structure](http://colony-print.hive.pt)
```

### Comparing `colony-print-0.3.0/src/colony_print/printing/binie/system.py` & `colony-print-0.3.1/src/colony_print/printing/binie/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/binie/visitor.py` & `colony-print-0.3.1/src/colony_print/printing/binie/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/binie/exceptions.py` & `colony-print-0.3.1/src/colony_print/printing/binie/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/manager/system.py` & `colony-print-0.3.1/src/colony_print/printing/manager/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/manager/ast.py` & `colony-print-0.3.1/src/colony_print/printing/manager/ast.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/manager/parser.py` & `colony-print-0.3.1/src/colony_print/printing/manager/parser.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/manager/visitor.py` & `colony-print-0.3.1/src/colony_print/printing/manager/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/manager/exceptions.py` & `colony-print-0.3.1/src/colony_print/printing/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/common/base.py` & `colony-print-0.3.1/src/colony_print/printing/common/base.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/pdf/system.py` & `colony-print-0.3.1/src/colony_print/printing/pdf/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/pdf/visitor.py` & `colony-print-0.3.1/src/colony_print/printing/pdf/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/printing/pdf/exceptions.py` & `colony-print-0.3.1/src/colony_print/printing/pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/static/example/js/main.js` & `colony-print-0.3.1/src/colony_print/static/example/js/main.js`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/static/example/print.html` & `colony-print-0.3.1/src/colony_print/static/example/print.html`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/static/example/xml/money_sale_slip.xml` & `colony-print-0.3.1/src/colony_print/static/example/xml/money_sale_slip.xml`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/controllers/printer.py` & `colony-print-0.3.1/src/colony_print/controllers/printer.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.0/src/colony_print/controllers/node.py` & `colony-print-0.3.1/src/colony_print/controllers/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 AAAAAAAABDYWxpYnJpAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACQAAAAMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAwAAABIZWxsbyBXb3JsZAA="
 
+VALID_OPTIONS = set(["scale", "quality", "email_address"])
+
 
 class NodeController(appier.Controller):
     @appier.route("/nodes", "GET", json=True)
     @appier.ensure(token="admin")
     def list(self):
         return self.owner.nodes
 
@@ -61,15 +63,17 @@
         name = name or str(uuid.uuid4())
         job = dict(data_b64=data_b64)
         if name:
             job["name"] = name
         if type:
             job["type"] = type
         if options:
-            job["options"] = options
+            job["options"] = dict(
+                (k, v) for k, v in options.items() if k in VALID_OPTIONS
+            )
         jobs = self.owner.jobs.get(id, [])
         jobs.append(job)
         self.owner.jobs[id] = jobs
         appier.notify("jobs:%s" % id)
 
     @appier.route("/nodes/<str:id>/print", "OPTIONS")
     def print_default_o(self, id):
@@ -111,15 +115,17 @@
         name = name or str(uuid.uuid4())
         job = dict(data_b64=data_b64, printer=printer)
         if name:
             job["name"] = name
         if type:
             job["type"] = type
         if options:
-            job["options"] = options
+            job["options"] = dict(
+                (k, v) for k, v in options.items() if k in VALID_OPTIONS
+            )
         jobs = self.owner.jobs.get(id, [])
         jobs.append(job)
         self.owner.jobs[id] = jobs
         appier.notify("jobs:%s" % id)
 
     @appier.route("/nodes/<str:id>/printers/<str:printer>/print", "OPTIONS")
     def print_printer_o(self, id, printer):
```

### Comparing `colony-print-0.3.0/src/colony_print/controllers/document.py` & `colony-print-0.3.1/src/colony_print/controllers/document.py`

 * *Files identical despite different names*

