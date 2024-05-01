# Comparing `tmp/idplib-0.0.2.tar.gz` & `tmp/idplib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idplib-0.0.2.tar", max compression
+gzip compressed data, was "idplib-0.0.3.tar", max compression
```

## Comparing `idplib-0.0.2.tar` & `idplib-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2024-03-12 22:46:06.590059 idplib-0.0.2/LICENSE
--rw-r--r--   0        0        0     6024 2024-03-19 21:54:17.249055 idplib-0.0.2/README.md
--rw-r--r--   0        0        0      280 2024-03-18 21:34:48.659905 idplib-0.0.2/idplib/Exceptions.py
--rw-r--r--   0        0        0     6948 2024-03-18 21:34:48.660351 idplib-0.0.2/idplib/HS/DocumentUtils.py
--rw-r--r--   0        0        0      577 2024-03-18 21:34:48.660695 idplib-0.0.2/idplib/HS/SubmissionUtils.py
--rw-r--r--   0        0        0        0 2024-03-18 21:34:48.660752 idplib-0.0.2/idplib/HS/__init__.py
--rw-r--r--   0        0        0     6776 2024-03-25 21:15:44.186568 idplib-0.0.2/idplib/Utilities/FuzzyFinder.py
--rw-r--r--   0        0        0        0 2024-03-19 21:54:17.249623 idplib-0.0.2/idplib/Utilities/__init__.py
--rw-r--r--   0        0        0     9070 2024-03-25 21:29:17.739889 idplib-0.0.2/idplib/ValueUtils.py
--rw-r--r--   0        0        0      205 2024-03-18 21:34:48.661600 idplib-0.0.2/idplib/__init__.py
--rw-r--r--   0        0        0     2598 2024-03-25 21:12:09.001716 idplib-0.0.2/idplib/algorithms.py
--rw-r--r--   0        0        0      811 2024-03-25 21:23:37.641874 idplib-0.0.2/idplib/defaults.py
--rw-r--r--   0        0        0      366 2024-03-19 21:54:17.250163 idplib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6738 1970-01-01 00:00:00.000000 idplib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-12 22:46:06.590059 idplib-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5943 2024-04-04 06:47:37.918008 idplib-0.0.3/README.md
+-rw-r--r--   0        0        0      280 2024-03-18 21:34:48.659905 idplib-0.0.3/idplib/Exceptions.py
+-rw-r--r--   0        0        0     6948 2024-03-18 21:34:48.660351 idplib-0.0.3/idplib/HS/DocumentUtils.py
+-rw-r--r--   0        0        0      577 2024-03-18 21:34:48.660695 idplib-0.0.3/idplib/HS/SubmissionUtils.py
+-rw-r--r--   0        0        0        0 2024-03-18 21:34:48.660752 idplib-0.0.3/idplib/HS/__init__.py
+-rw-r--r--   0        0        0     6776 2024-04-04 06:31:45.539030 idplib-0.0.3/idplib/Utilities/FuzzyFinder.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:31:45.539095 idplib-0.0.3/idplib/Utilities/__init__.py
+-rw-r--r--   0        0        0     9072 2024-05-01 08:24:12.895172 idplib-0.0.3/idplib/ValueUtils.py
+-rw-r--r--   0        0        0      114 2024-05-01 09:13:09.274722 idplib-0.0.3/idplib/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-04 06:31:45.540077 idplib-0.0.3/idplib/algorithms.py
+-rw-r--r--   0        0        0      811 2024-04-04 06:31:45.540528 idplib-0.0.3/idplib/defaults.py
+-rw-r--r--   0        0        0      366 2024-05-01 08:30:26.597337 idplib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6657 1970-01-01 00:00:00.000000 idplib-0.0.3/PKG-INFO
```

### Comparing `idplib-0.0.2/LICENSE` & `idplib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/README.md` & `idplib-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 The purpose of this library is to provide useful tools to support IDP based processes
 
 
 ## Install
 
 ```
-pip install dist/idplib-0.0.1-py3-none-any.whl
+pip install idplib
 ```
 
-Lib is not currently on pypi until it is more stable
 
 ## Usage
 
 Usege will be broken down into a few concepts. General and tool specific.
 
 ### General
```

### Comparing `idplib-0.0.2/idplib/HS/DocumentUtils.py` & `idplib-0.0.3/idplib/HS/DocumentUtils.py`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/idplib/HS/SubmissionUtils.py` & `idplib-0.0.3/idplib/HS/SubmissionUtils.py`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/idplib/Utilities/FuzzyFinder.py` & `idplib-0.0.3/idplib/Utilities/FuzzyFinder.py`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/idplib/ValueUtils.py` & `idplib-0.0.3/idplib/ValueUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import functools
 import re
 import operator
 from decimal import ROUND_HALF_UP, Decimal
-from defaults import DateFormat, Cleaner
-from algorithms import CreditCard, AusGov
+from .defaults import DateFormat, Cleaner
+from .algorithms import CreditCard, AusGov
 from fuzzywuzzy import fuzz # type: ignore
 
 
 def replace_newline(func):
     def wrapper(*args, **kwargs):
         # first convert any None type args or kwargs to empty strings
         args = ["" if isinstance(arg, type(None)) else arg for arg in args]
```

### Comparing `idplib-0.0.2/idplib/algorithms.py` & `idplib-0.0.3/idplib/algorithms.py`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/idplib/defaults.py` & `idplib-0.0.3/idplib/defaults.py`

 * *Files identical despite different names*

### Comparing `idplib-0.0.2/PKG-INFO` & `idplib-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idplib
-Version: 0.0.2
+Version: 0.0.3
 Summary: IDP Project utility tools
 License: MIT
 Author: Jack Jorgensen
 Author-email: jorgensen.jack@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,18 +22,17 @@
 
 The purpose of this library is to provide useful tools to support IDP based processes
 
 
 ## Install
 
 ```
-pip install dist/idplib-0.0.1-py3-none-any.whl
+pip install idplib
 ```
 
-Lib is not currently on pypi until it is more stable
 
 ## Usage
 
 Usege will be broken down into a few concepts. General and tool specific.
 
 ### General
```

