# Comparing `tmp/ibonds-1.0.3.tar.gz` & `tmp/ibonds-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibonds-1.0.3.tar", last modified: Tue Oct 31 14:58:17 2023, max compression
+gzip compressed data, was "ibonds-1.0.4.tar", last modified: Wed May  1 03:39:46 2024, max compression
```

## Comparing `ibonds-1.0.3.tar` & `ibonds-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-10-31 14:58:17.186040 ibonds-1.0.3/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.3/LICENSE
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.3/MANIFEST.in
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1863 2023-10-31 14:58:17.186040 ibonds-1.0.3/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.3/README.md
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-10-31 14:58:17.186040 ibonds-1.0.3/ibonds/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6901 2023-06-01 03:32:08.000000 ibonds-1.0.3/ibonds/__init__.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1354 2023-10-31 14:55:36.000000 ibonds-1.0.3/ibonds/interest_rates.yaml
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-10-31 14:58:17.186040 ibonds-1.0.3/ibonds.egg-info/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1863 2023-10-31 14:58:17.000000 ibonds-1.0.3/ibonds.egg-info/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2023-10-31 14:58:17.000000 ibonds-1.0.3/ibonds.egg-info/SOURCES.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-10-31 14:58:17.000000 ibonds-1.0.3/ibonds.egg-info/dependency_links.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2023-10-31 14:58:17.000000 ibonds-1.0.3/ibonds.egg-info/requires.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2023-10-31 14:58:17.000000 ibonds-1.0.3/ibonds.egg-info/top_level.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-10-31 14:58:17.186040 ibonds-1.0.3/setup.cfg
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1013 2023-10-31 14:58:00.000000 ibonds-1.0.3/setup.py
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-10-31 14:58:17.186040 ibonds-1.0.3/tests/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5167 2023-06-01 03:10:53.000000 ibonds-1.0.3/tests/test_ibonds.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2024-05-01 03:39:46.462133 ibonds-1.0.4/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.4/LICENSE
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.4/MANIFEST.in
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1920 2024-05-01 03:39:46.462133 ibonds-1.0.4/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.4/README.md
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2024-05-01 03:39:46.462133 ibonds-1.0.4/ibonds/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6901 2023-06-01 03:32:08.000000 ibonds-1.0.4/ibonds/__init__.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1380 2024-05-01 03:21:19.000000 ibonds-1.0.4/ibonds/interest_rates.yaml
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2024-05-01 03:39:46.462133 ibonds-1.0.4/ibonds.egg-info/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1920 2024-05-01 03:39:46.000000 ibonds-1.0.4/ibonds.egg-info/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2024-05-01 03:39:46.000000 ibonds-1.0.4/ibonds.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2024-05-01 03:39:46.000000 ibonds-1.0.4/ibonds.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2024-05-01 03:39:46.000000 ibonds-1.0.4/ibonds.egg-info/requires.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2024-05-01 03:39:46.000000 ibonds-1.0.4/ibonds.egg-info/top_level.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2024-05-01 03:39:46.462133 ibonds-1.0.4/setup.cfg
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1013 2024-05-01 03:25:26.000000 ibonds-1.0.4/setup.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2024-05-01 03:39:46.462133 ibonds-1.0.4/tests/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5167 2023-06-01 03:10:53.000000 ibonds-1.0.4/tests/test_ibonds.py
```

### Comparing `ibonds-1.0.3/LICENSE` & `ibonds-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.3/PKG-INFO` & `ibonds-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to calculate the current value of a Series I Savings bond (I Bond)
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.28
 
 # I Bonds
 
 This is a python library that calculates the current value of a
 [Series I Savings Bond](https://www.treasurydirect.gov/savings-bonds/i-bonds/).
 The historic rates are supplied via a data file which is updated every time
 a new rate is released by [Treasury Direct](https://www.treasurydirect.gov/).
```

### Comparing `ibonds-1.0.3/README.md` & `ibonds-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.3/ibonds/__init__.py` & `ibonds-1.0.4/ibonds/__init__.py`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.3/ibonds/interest_rates.yaml` & `ibonds-1.0.4/ibonds/interest_rates.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -150,7 +150,10 @@
 - 3.24
 2023-05-01:
 - 0.90
 - 1.69
 2023-11-01:
 - 1.30
 - 1.97
+2024-05-01:
+- 1.30
+- 1.48
```

### Comparing `ibonds-1.0.3/ibonds.egg-info/PKG-INFO` & `ibonds-1.0.4/ibonds.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to calculate the current value of a Series I Savings bond (I Bond)
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.28
 
 # I Bonds
 
 This is a python library that calculates the current value of a
 [Series I Savings Bond](https://www.treasurydirect.gov/savings-bonds/i-bonds/).
 The historic rates are supplied via a data file which is updated every time
 a new rate is released by [Treasury Direct](https://www.treasurydirect.gov/).
```

### Comparing `ibonds-1.0.3/setup.py` & `ibonds-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='ibonds',
-    version='1.0.3',
+    version='1.0.4',
     author='Sarvjeet Singh',
     author_email='sarvjeet@gmail.com',
     description=('Library to calculate the current value of a '
                  'Series I Savings bond (I Bond)'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sarvjeets/ibonds',
```

### Comparing `ibonds-1.0.3/tests/test_ibonds.py` & `ibonds-1.0.4/tests/test_ibonds.py`

 * *Files identical despite different names*

