# Comparing `tmp/imsciences-0.5.4.9.tar.gz` & `tmp/imsciences-0.5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.4.9.tar", last modified: Wed May  1 10:05:52 2024, max compression
+gzip compressed data, was "imsciences-0.5.5.0.tar", last modified: Wed May  1 10:23:53 2024, max compression
```

## Comparing `imsciences-0.5.4.9.tar` & `imsciences-0.5.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 10:05:52.459662 imsciences-0.5.4.9/
--rw-rw-rw-   0        0        0     5465 2024-05-01 10:05:52.455662 imsciences-0.5.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     4962 2024-03-14 19:13:12.000000 imsciences-0.5.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 10:05:52.430225 imsciences-0.5.4.9/imsciences/
--rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.4.9/imsciences/__init__.py
--rw-rw-rw-   0        0        0    33182 2024-05-01 09:40:46.000000 imsciences-0.5.4.9/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 10:05:52.452566 imsciences-0.5.4.9/imsciences.egg-info/
--rw-rw-rw-   0        0        0     5465 2024-05-01 10:05:52.000000 imsciences-0.5.4.9/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-01 10:05:52.000000 imsciences-0.5.4.9/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 10:05:52.000000 imsciences-0.5.4.9/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-01 10:05:52.000000 imsciences-0.5.4.9/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 10:05:52.000000 imsciences-0.5.4.9/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 10:05:52.460528 imsciences-0.5.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-01 09:47:34.000000 imsciences-0.5.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.674617 imsciences-0.5.5.0/
+-rw-rw-rw-   0        0        0     5465 2024-05-01 10:23:53.671407 imsciences-0.5.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4962 2024-03-14 19:13:12.000000 imsciences-0.5.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.637571 imsciences-0.5.5.0/imsciences/
+-rw-rw-rw-   0        0        0       41 2024-03-14 19:23:10.000000 imsciences-0.5.5.0/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    33182 2024-05-01 09:40:46.000000 imsciences-0.5.5.0/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:23:53.666425 imsciences-0.5.5.0/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     5465 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 10:23:53.000000 imsciences-0.5.5.0/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:23:53.674617 imsciences-0.5.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-01 10:23:21.000000 imsciences-0.5.5.0/setup.py
```

### Comparing `imsciences-0.5.4.9/PKG-INFO` & `imsciences-0.5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.4.9
+Version: 0.5.5.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.4.9/README.md` & `imsciences-0.5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.4.9/imsciences/datafunctions.py` & `imsciences-0.5.5.0/imsciences/datafunctions.py`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.4.9/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.5.0/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.4.9
+Version: 0.5.5.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.4.9/setup.py` & `imsciences-0.5.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.4.9'
+VERSION = '0.5.5.0'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

