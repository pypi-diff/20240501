# Comparing `tmp/princo-4.0.5.tar.gz` & `tmp/princo-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "princo-4.0.5.tar", last modified: Wed May  1 10:37:16 2024, max compression
+gzip compressed data, was "princo-5.0.5.tar", last modified: Wed May  1 11:01:24 2024, max compression
```

## Comparing `princo-4.0.5.tar` & `princo-5.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.349031 princo-4.0.5/
--rw-rw-rw-   0        0        0     1088 2024-05-01 09:20:39.000000 princo-4.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      261 2024-05-01 10:37:16.346505 princo-4.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-01 09:28:20.000000 princo-4.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.321778 princo-4.0.5/princo/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:40:17.000000 princo-4.0.5/princo/__init__.py
--rw-rw-rw-   0        0        0      215 2024-05-01 09:50:45.000000 princo-4.0.5/princo/princo.py
-drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.345504 princo-4.0.5/princo.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 10:37:16.349031 princo-4.0.5/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-05-01 10:35:47.000000 princo-4.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:24.414583 princo-5.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-01 09:20:39.000000 princo-5.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      261 2024-05-01 11:01:24.412619 princo-5.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:24.411100 princo-5.0.5/Princo.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-05-01 11:01:24.000000 princo-5.0.5/Princo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-01 11:01:24.000000 princo-5.0.5/Princo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:01:24.000000 princo-5.0.5/Princo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 11:01:24.000000 princo-5.0.5/Princo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-01 09:28:20.000000 princo-5.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 11:01:24.398281 princo-5.0.5/princo/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:40:17.000000 princo-5.0.5/princo/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-05-01 09:50:45.000000 princo-5.0.5/princo/princo.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:01:24.414583 princo-5.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-01 11:01:19.000000 princo-5.0.5/setup.py
```

### Comparing `princo-4.0.5/LICENSE.txt` & `princo-5.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `princo-4.0.5/setup.py` & `princo-5.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='princo',
-    version='4.0.5',
+    name='Princo',
+    version='5.0.5',
     author='The Urban Penguin',
     author_email="mahdisahnoun31@gmail.com",  # Replace with your email address
     description='princo package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[],
```

