# Comparing `tmp/glcl-0.0.6.tar.gz` & `tmp/glcl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\glcl-0.0.6.tar", last modified: Wed May  1 03:45:40 2024, max compression
+gzip compressed data, was "dist\glcl-0.0.7.tar", last modified: Wed May  1 03:56:17 2024, max compression
```

## Comparing `glcl-0.0.6.tar` & `glcl-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.366156 glcl-0.0.6/
--rw-rw-rw-   0        0        0       24 2024-05-01 01:31:02.000000 glcl-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1088 2024-05-01 01:12:19.000000 glcl-0.0.6/MIT License
--rw-rw-rw-   0        0        0      837 2024-05-01 03:45:40.366156 glcl-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-01 01:12:19.000000 glcl-0.0.6/README.MD
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.334956 glcl-0.0.6/glcl/
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.334956 glcl-0.0.6/glcl/Win32/
--rw-rw-rw-   0        0        0  6138880 2024-05-01 00:46:18.000000 glcl-0.0.6/glcl/Win32/glcl.pyd
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.350556 glcl-0.0.6/glcl/Win64/
--rw-rw-rw-   0        0        0  9771520 2024-05-01 00:46:18.000000 glcl-0.0.6/glcl/Win64/glcl.pyd
--rw-rw-rw-   0        0        0     1793 2024-05-01 00:46:18.000000 glcl-0.0.6/glcl/__init__.py
--rw-rw-rw-   0        0        0  2034267 2024-04-24 15:59:06.000000 glcl-0.0.6/glcl/__init__.pyi
--rw-rw-rw-   0        0        0      282 2024-05-01 01:26:04.000000 glcl-0.0.6/glcl/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.366156 glcl-0.0.6/glcl/doc/
--rw-rw-rw-   0        0        0  1465315 2024-05-01 00:46:18.000000 glcl-0.0.6/glcl/doc/docs.xml
-drwxrwxrwx   0        0        0        0 2024-05-01 03:45:40.334956 glcl-0.0.6/glcl.egg-info/
--rw-rw-rw-   0        0        0      837 2024-05-01 03:45:40.000000 glcl-0.0.6/glcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-01 03:45:40.000000 glcl-0.0.6/glcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:45:40.000000 glcl-0.0.6/glcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-01 03:45:40.000000 glcl-0.0.6/glcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 03:45:40.366156 glcl-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1170 2024-05-01 03:45:29.000000 glcl-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.443280 glcl-0.0.7/
+-rw-rw-rw-   0        0        0       35 2024-05-01 03:54:33.000000 glcl-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1088 2024-05-01 01:12:19.000000 glcl-0.0.7/MIT License
+-rw-rw-rw-   0        0        0      837 2024-05-01 03:56:17.443280 glcl-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-01 01:12:19.000000 glcl-0.0.7/README.MD
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.412080 glcl-0.0.7/glcl/
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.412080 glcl-0.0.7/glcl/Win32/
+-rw-rw-rw-   0        0        0  6138880 2024-05-01 00:46:18.000000 glcl-0.0.7/glcl/Win32/glcl.pyd
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.412080 glcl-0.0.7/glcl/Win64/
+-rw-rw-rw-   0        0        0  9771520 2024-05-01 00:46:18.000000 glcl-0.0.7/glcl/Win64/glcl.pyd
+-rw-rw-rw-   0        0        0     1793 2024-05-01 00:46:18.000000 glcl-0.0.7/glcl/__init__.py
+-rw-rw-rw-   0        0        0  2034267 2024-04-24 15:59:06.000000 glcl-0.0.7/glcl/__init__.pyi
+-rw-rw-rw-   0        0        0      282 2024-05-01 01:26:04.000000 glcl-0.0.7/glcl/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.427680 glcl-0.0.7/glcl/doc/
+-rw-rw-rw-   0        0        0  1465315 2024-05-01 00:46:18.000000 glcl-0.0.7/glcl/doc/docs.xml
+drwxrwxrwx   0        0        0        0 2024-05-01 03:56:17.412080 glcl-0.0.7/glcl.egg-info/
+-rw-rw-rw-   0        0        0      837 2024-05-01 03:56:17.000000 glcl-0.0.7/glcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-01 03:56:17.000000 glcl-0.0.7/glcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:56:17.000000 glcl-0.0.7/glcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 03:56:17.000000 glcl-0.0.7/glcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:56:17.443280 glcl-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2024-05-01 03:56:10.000000 glcl-0.0.7/setup.py
```

### Comparing `glcl-0.0.6/MIT License` & `glcl-0.0.7/MIT License`

 * *Files identical despite different names*

### Comparing `glcl-0.0.6/PKG-INFO` & `glcl-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glcl
-Version: 0.0.6
+Version: 0.0.7
 Summary: glcl for python studio
 Home-page: UNKNOWN
 Author: glsite.com
 Author-email: admin@glsite.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `glcl-0.0.6/glcl/__init__.py` & `glcl-0.0.7/glcl/__init__.py`

 * *Files identical despite different names*

### Comparing `glcl-0.0.6/glcl/__init__.pyi` & `glcl-0.0.7/glcl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `glcl-0.0.6/glcl/doc/docs.xml` & `glcl-0.0.7/glcl/doc/docs.xml`

 * *Files identical despite different names*

### Comparing `glcl-0.0.6/glcl.egg-info/PKG-INFO` & `glcl-0.0.7/glcl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glcl
-Version: 0.0.6
+Version: 0.0.7
 Summary: glcl for python studio
 Home-page: UNKNOWN
 Author: glsite.com
 Author-email: admin@glsite.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `glcl-0.0.6/setup.py` & `glcl-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.MD", "r") as f:
   long_description = f.read()
 
 setup(name='glcl',
-      version='0.0.6',
+      version='0.0.7',
       description='glcl for python studio',
       long_description=long_description,
       author='glsite.com',
       author_email='admin@glsite.com',
       url='',
       install_requires=[],
       license='MIT License',
       platforms=["all"],
-      packages=find_packages(),
+      packages=['glcl'],
       include_package_data=True,
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
           'Programming Language :: Python',
           'Programming Language :: Python :: 3.7',
```

