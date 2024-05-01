# Comparing `tmp/icc_utils-0.1.62.tar.gz` & `tmp/icc_utils-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icc_utils-0.1.62.tar", last modified: Wed May  1 16:25:34 2024, max compression
+gzip compressed data, was "icc_utils-0.1.63.tar", last modified: Wed May  1 16:30:24 2024, max compression
```

## Comparing `icc_utils-0.1.62.tar` & `icc_utils-0.1.63.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.110279 icc_utils-0.1.62/
--rw-rw-rw-   0        0        0     1068 2024-05-01 16:10:12.000000 icc_utils-0.1.62/LICENSE
--rw-rw-rw-   0        0        0      883 2024-05-01 16:25:34.094653 icc_utils-0.1.62/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-01 16:10:12.000000 icc_utils-0.1.62/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.000905 icc_utils-0.1.62/icc_utils/
--rw-rw-rw-   0        0        0     5463 2024-03-01 06:14:57.000000 icc_utils-0.1.62/icc_utils/PandasUtils.py
--rw-rw-rw-   0        0        0     7021 2024-03-01 06:14:57.000000 icc_utils-0.1.62/icc_utils/SQLUtils.py
--rw-rw-rw-   0        0        0     2698 2024-05-01 16:25:26.000000 icc_utils-0.1.62/icc_utils/Scheduler.py
--rw-rw-rw-   0        0        0    12141 2024-05-01 16:25:26.000000 icc_utils-0.1.62/icc_utils/SystemUtils.py
--rw-rw-rw-   0        0        0      407 2024-05-01 16:10:18.000000 icc_utils-0.1.62/icc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:25:34.047781 icc_utils-0.1.62/icc_utils.egg-info/
--rw-rw-rw-   0        0        0      883 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 16:25:33.000000 icc_utils-0.1.62/icc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 16:25:34.110279 icc_utils-0.1.62/setup.cfg
--rw-rw-rw-   0        0        0     1178 2024-05-01 16:25:31.000000 icc_utils-0.1.62/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:30:24.514673 icc_utils-0.1.63/
+-rw-rw-rw-   0        0        0     1068 2024-05-01 16:10:12.000000 icc_utils-0.1.63/LICENSE
+-rw-rw-rw-   0        0        0      883 2024-05-01 16:30:24.499048 icc_utils-0.1.63/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-01 16:10:12.000000 icc_utils-0.1.63/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:30:24.405299 icc_utils-0.1.63/icc_utils/
+-rw-rw-rw-   0        0        0     5463 2024-03-01 06:14:57.000000 icc_utils-0.1.63/icc_utils/PandasUtils.py
+-rw-rw-rw-   0        0        0     7021 2024-03-01 06:14:57.000000 icc_utils-0.1.63/icc_utils/SQLUtils.py
+-rw-rw-rw-   0        0        0    12141 2024-05-01 16:25:26.000000 icc_utils-0.1.63/icc_utils/SystemUtils.py
+-rw-rw-rw-   0        0        0      407 2024-05-01 16:10:18.000000 icc_utils-0.1.63/icc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:30:24.452175 icc_utils-0.1.63/icc_utils.egg-info/
+-rw-rw-rw-   0        0        0      883 2024-05-01 16:30:24.000000 icc_utils-0.1.63/icc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-01 16:30:24.000000 icc_utils-0.1.63/icc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:30:24.000000 icc_utils-0.1.63/icc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-01 16:30:24.000000 icc_utils-0.1.63/icc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 16:30:24.000000 icc_utils-0.1.63/icc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:30:24.514673 icc_utils-0.1.63/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2024-05-01 16:30:21.000000 icc_utils-0.1.63/setup.py
```

### Comparing `icc_utils-0.1.62/LICENSE` & `icc_utils-0.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.62/PKG-INFO` & `icc_utils-0.1.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.62
+Version: 0.1.63
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `icc_utils-0.1.62/icc_utils/PandasUtils.py` & `icc_utils-0.1.63/icc_utils/PandasUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.62/icc_utils/SQLUtils.py` & `icc_utils-0.1.63/icc_utils/SQLUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.62/icc_utils/SystemUtils.py` & `icc_utils-0.1.63/icc_utils/SystemUtils.py`

 * *Files identical despite different names*

### Comparing `icc_utils-0.1.62/icc_utils.egg-info/PKG-INFO` & `icc_utils-0.1.63/icc_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icc_utils
-Version: 0.1.62
+Version: 0.1.63
 Summary: Package used to handle common functions at ICC
 Home-page: https://github.com/jbradleyicc/icc_utils
 Author: Jordan Bradley
 Author-email: jbradley@internationalcybernetics.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `icc_utils-0.1.62/setup.py` & `icc_utils-0.1.63/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='icc_utils',
-    version='0.1.62',
+    version='0.1.63',
     packages=find_packages(),
     description='Package used to handle common functions at ICC',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jordan Bradley',
     author_email='jbradley@internationalcybernetics.com',
     url='https://github.com/jbradleyicc/icc_utils',
```

