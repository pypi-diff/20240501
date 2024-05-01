# Comparing `tmp/sembansurga-1.0.4.tar.gz` & `tmp/sembansurga-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.4.tar", last modified: Sun Feb 18 17:42:26 2024, max compression
+gzip compressed data, was "sembansurga-1.1.3.tar", last modified: Wed May  1 02:49:17 2024, max compression
```

## Comparing `sembansurga-1.0.4.tar` & `sembansurga-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      405 2024-02-18 17:42:26.174029 sembansurga-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-25 08:55:36.000000 sembansurga-1.0.4/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-01-25 08:55:16.000000 sembansurga-1.0.4/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 17:42:26.174029 sembansurga-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      730 2024-02-18 17:42:08.000000 sembansurga-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 02:49:17.254040 sembansurga-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-01 02:49:17.254040 sembansurga-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 02:49:17.254040 sembansurga-1.1.3/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      143 2024-04-18 10:30:17.000000 sembansurga-1.1.3/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-04-18 10:30:07.000000 sembansurga-1.1.3/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 02:49:17.254040 sembansurga-1.1.3/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-01 02:49:17.000000 sembansurga-1.1.3/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-01 02:49:17.000000 sembansurga-1.1.3/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 02:49:17.000000 sembansurga-1.1.3/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-01 02:49:17.000000 sembansurga-1.1.3/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-01 02:49:17.000000 sembansurga-1.1.3/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 02:49:17.254040 sembansurga-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-01 02:48:41.000000 sembansurga-1.1.3/setup.py
```

### Comparing `sembansurga-1.0.4/setup.py` & `sembansurga-1.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.4',
+    version='1.1.3',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'libtorrent',
+        'usellm',
+
+    
 
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

