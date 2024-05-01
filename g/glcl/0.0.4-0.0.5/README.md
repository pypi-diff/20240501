# Comparing `tmp/glcl-0.0.4.tar.gz` & `tmp/glcl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\glcl-0.0.4.tar", last modified: Wed May  1 01:18:13 2024, max compression
+gzip compressed data, was "dist\glcl-0.0.5.tar", last modified: Wed May  1 01:31:04 2024, max compression
```

## Comparing `glcl-0.0.4.tar` & `glcl-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/
--rw-rw-rw-   0        0        0     1027 2024-05-01 01:18:13.677758 glcl-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/glcl/
--rw-rw-rw-   0        0        0        0 2024-05-01 01:12:19.000000 glcl-0.0.4/glcl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/glcl.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      137 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 01:18:13.677758 glcl-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1332 2024-05-01 01:12:19.000000 glcl-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.338522 glcl-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-01 01:12:19.000000 glcl-0.0.5/MIT License
+-rw-rw-rw-   0        0        0       24 2024-05-01 01:31:02.000000 glcl-0.0.5/Manifest.in
+-rw-rw-rw-   0        0        0      828 2024-05-01 01:31:04.338522 glcl-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-01 01:12:19.000000 glcl-0.0.5/README.MD
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.307322 glcl-0.0.5/glcl/
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.307322 glcl-0.0.5/glcl/Win32/
+-rw-rw-rw-   0        0        0  6138880 2024-05-01 00:46:18.000000 glcl-0.0.5/glcl/Win32/glcl.pyd
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.322922 glcl-0.0.5/glcl/Win64/
+-rw-rw-rw-   0        0        0  9771520 2024-05-01 00:46:18.000000 glcl-0.0.5/glcl/Win64/glcl.pyd
+-rw-rw-rw-   0        0        0     1793 2024-05-01 00:46:18.000000 glcl-0.0.5/glcl/__init__.py
+-rw-rw-rw-   0        0        0  2034267 2024-04-24 15:59:06.000000 glcl-0.0.5/glcl/__init__.pyi
+-rw-rw-rw-   0        0        0      282 2024-05-01 01:26:04.000000 glcl-0.0.5/glcl/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.322922 glcl-0.0.5/glcl/doc/
+-rw-rw-rw-   0        0        0  1465315 2024-05-01 00:46:18.000000 glcl-0.0.5/glcl/doc/docs.xml
+drwxrwxrwx   0        0        0        0 2024-05-01 01:31:04.338522 glcl-0.0.5/glcl.egg-info/
+-rw-rw-rw-   0        0        0      828 2024-05-01 01:31:04.000000 glcl-0.0.5/glcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-01 01:31:04.000000 glcl-0.0.5/glcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 01:31:04.000000 glcl-0.0.5/glcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 01:31:04.000000 glcl-0.0.5/glcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 01:31:04.338522 glcl-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2024-05-01 01:27:16.000000 glcl-0.0.5/setup.py
```

### Comparing `glcl-0.0.4/setup.py` & `glcl-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.MD", "r") as f:
   long_description = f.read()
 
 setup(name='glcl',
-      version='0.0.4',
+      version='0.0.5',
       description='glcl for python studio',
       long_description=long_description,
       author='glsite.com',
       author_email='admin@glsite.com',
       url='',
       install_requires=[],
       license='MIT License',
-      packages=["glcl"],
       platforms=["all"],
+      packages=find_packages(),
+      include_package_data=True,
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

