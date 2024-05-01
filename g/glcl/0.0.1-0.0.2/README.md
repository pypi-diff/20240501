# Comparing `tmp/glcl-0.0.1.tar.gz` & `tmp/glcl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\glcl-0.0.1.tar", last modified: Tue Apr 30 22:54:11 2024, max compression
+gzip compressed data, was "dist\glcl-0.0.2.tar", last modified: Tue Apr 30 23:15:31 2024, max compression
```

## Comparing `glcl-0.0.1.tar` & `glcl-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 22:54:11.132396 glcl-0.0.1/
--rw-rw-rw-   0        0        0     1039 2024-04-30 22:54:11.116796 glcl-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 22:54:11.116796 glcl-0.0.1/glcl/
--rw-rw-rw-   0        0        0        0 2024-04-30 22:53:53.000000 glcl-0.0.1/glcl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 22:54:11.116796 glcl-0.0.1/glcl.egg-info/
--rw-rw-rw-   0        0        0     1039 2024-04-30 22:54:11.000000 glcl-0.0.1/glcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      137 2024-04-30 22:54:11.000000 glcl-0.0.1/glcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 22:54:11.000000 glcl-0.0.1/glcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-30 22:54:11.000000 glcl-0.0.1/glcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 22:54:11.132396 glcl-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1332 2024-04-30 22:53:53.000000 glcl-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:15:31.958667 glcl-0.0.2/
+-rw-rw-rw-   0        0        0      840 2024-04-30 23:15:31.958667 glcl-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 23:15:31.958667 glcl-0.0.2/glcl/
+-rw-rw-rw-   0        0        0     1793 2024-04-30 23:06:42.000000 glcl-0.0.2/glcl/__init__.py
+-rw-rw-rw-   0        0        0      282 2024-04-30 23:08:15.000000 glcl-0.0.2/glcl/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:15:31.958667 glcl-0.0.2/glcl.egg-info/
+-rw-rw-rw-   0        0        0      840 2024-04-30 23:15:31.000000 glcl-0.0.2/glcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2024-04-30 23:15:31.000000 glcl-0.0.2/glcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 23:15:31.000000 glcl-0.0.2/glcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 23:15:31.000000 glcl-0.0.2/glcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 23:15:31.958667 glcl-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2024-04-30 23:03:50.000000 glcl-0.0.2/setup.py
```

### Comparing `glcl-0.0.1/PKG-INFO` & `glcl-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: glcl
-Version: 0.0.1
+Version: 0.0.2
 Summary: glcl for python studio
 Home-page: UNKNOWN
 Author: glsite.com
 Author-email: admin@glsite.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries
 
 # glcl
 glcl for python studio.
```

### Comparing `glcl-0.0.1/glcl.egg-info/PKG-INFO` & `glcl-0.0.2/glcl.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: glcl
-Version: 0.0.1
+Version: 0.0.2
 Summary: glcl for python studio
 Home-page: UNKNOWN
 Author: glsite.com
 Author-email: admin@glsite.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries
 
 # glcl
 glcl for python studio.
```

### Comparing `glcl-0.0.1/setup.py` & `glcl-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.MD", "r") as f:
   long_description = f.read()
 
 setup(name='glcl',
-      version='0.0.1',
+      version='0.0.2',
       description='glcl for python studio',
       long_description=long_description,
       author='glsite.com',
       author_email='admin@glsite.com',
       url='',
       install_requires=[],
       license='MIT License',
       packages=["glcl"],
       platforms=["all"],
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: 3.12',
+          'Programming Language :: Python :: 3.13',
           'Topic :: Software Development :: Libraries'
       ],
       )
```

