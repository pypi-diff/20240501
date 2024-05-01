# Comparing `tmp/monisha-0.0.62.tar.gz` & `tmp/monisha-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.62.tar", last modified: Tue Apr 30 19:32:08 2024, max compression
+gzip compressed data, was "monisha-0.0.63.tar", last modified: Tue Apr 30 20:49:29 2024, max compression
```

## Comparing `monisha-0.0.62.tar` & `monisha-0.0.63.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 19:32:03.000000 monisha-0.0.62/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.001797 monisha-0.0.62/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function18.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 19:32:08.005797 monisha-0.0.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 19:32:03.000000 monisha-0.0.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:32:08.005797 monisha-0.0.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 19:32:03.000000 monisha-0.0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:49:29.782544 monisha-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 20:49:25.000000 monisha-0.0.63/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:49:29.778545 monisha-0.0.63/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:49:29.782544 monisha-0.0.63/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/functions/function18.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:49:29.782544 monisha-0.0.63/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 20:49:25.000000 monisha-0.0.63/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 20:49:29.782544 monisha-0.0.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 20:49:25.000000 monisha-0.0.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:49:29.782544 monisha-0.0.63/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 20:49:29.000000 monisha-0.0.63/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 20:49:29.000000 monisha-0.0.63/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:49:29.000000 monisha-0.0.63/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 20:49:29.000000 monisha-0.0.63/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 20:49:29.000000 monisha-0.0.63/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:49:29.782544 monisha-0.0.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 20:49:25.000000 monisha-0.0.63/setup.py
```

### Comparing `monisha-0.0.62/LICENSE` & `monisha-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/__init__.py` & `monisha-0.0.63/Monisha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.62"
+version = "0.0.63"
 
 install = ["hachoir"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `monisha-0.0.62/Monisha/functions/__init__.py` & `monisha-0.0.63/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function01.py` & `monisha-0.0.63/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function02.py` & `monisha-0.0.63/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function03.py` & `monisha-0.0.63/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function04.py` & `monisha-0.0.63/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function06.py` & `monisha-0.0.63/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function07.py` & `monisha-0.0.63/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function10.py` & `monisha-0.0.63/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function14.py` & `monisha-0.0.63/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function15.py` & `monisha-0.0.63/Monisha/functions/function15.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from .function09 import Storage
 #=================================================================================================
 
 class Messages:
     def __init__(self, **kwargs):
         self.numfiles = kwargs.get('numfiles', 0)
         self.filesize = kwargs.get('filesize', 0)
-        self.allfiles = kwargs.get('allfiles', [])
+        self.allfiles = kwargs.get('allfiles', None)
         self.location = kwargs.get('location', None)
 
 #=================================================================================================
 
 class Location:
 
-    async def get00(dlocation, skip=Eimes.DATA00, files=[]):
+    async def get00(files, dlocation, skip=Eimes.DATA00):
         for patho in sorted(os.listdir(dlocation)):
             filez = os.path.join(dlocation, patho)
             if filez.upper().endswith(skip):
                 continue
             else:
                 files.append(filez)
```

### Comparing `monisha-0.0.62/Monisha/functions/function16.py` & `monisha-0.0.63/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function17.py` & `monisha-0.0.63/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/functions/function18.py` & `monisha-0.0.63/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/Monisha/scripts/es.py` & `monisha-0.0.63/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/PKG-INFO` & `monisha-0.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.62
+Version: 0.0.63
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.62 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.63 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.62/monisha.egg-info/PKG-INFO` & `monisha-0.0.63/monisha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.62
+Version: 0.0.63
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.62 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.63 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.62/monisha.egg-info/SOURCES.txt` & `monisha-0.0.63/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.62/setup.py` & `monisha-0.0.63/setup.py`

 * *Files identical despite different names*

