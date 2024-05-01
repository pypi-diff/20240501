# Comparing `tmp/princo-1.0.5.tar.gz` & `tmp/princo-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "princo-1.0.5.tar", last modified: Wed May  1 09:55:52 2024, max compression
+gzip compressed data, was "princo-4.0.5.tar", last modified: Wed May  1 10:37:16 2024, max compression
```

## Comparing `princo-1.0.5.tar` & `princo-4.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 09:55:52.856073 princo-1.0.5/
--rw-rw-rw-   0        0        0     1088 2024-05-01 09:20:39.000000 princo-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      261 2024-05-01 09:55:52.855074 princo-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-01 09:28:20.000000 princo-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 09:55:52.820542 princo-1.0.5/princo/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:40:17.000000 princo-1.0.5/princo/__init__.py
--rw-rw-rw-   0        0        0      215 2024-05-01 09:50:45.000000 princo-1.0.5/princo/princo.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:55:52.853067 princo-1.0.5/princo.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-01 09:55:52.000000 princo-1.0.5/princo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-01 09:55:52.000000 princo-1.0.5/princo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 09:55:52.000000 princo-1.0.5/princo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-01 09:55:52.000000 princo-1.0.5/princo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 09:55:52.857073 princo-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      593 2024-05-01 09:39:16.000000 princo-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.349031 princo-4.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-01 09:20:39.000000 princo-4.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      261 2024-05-01 10:37:16.346505 princo-4.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-01 09:28:20.000000 princo-4.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.321778 princo-4.0.5/princo/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:40:17.000000 princo-4.0.5/princo/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-05-01 09:50:45.000000 princo-4.0.5/princo/princo.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:37:16.345504 princo-4.0.5/princo.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 10:37:16.000000 princo-4.0.5/princo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:37:16.349031 princo-4.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-01 10:35:47.000000 princo-4.0.5/setup.py
```

### Comparing `princo-1.0.5/LICENSE.txt` & `princo-4.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `princo-1.0.5/setup.py` & `princo-4.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='princo',
-    version='1.0.5',
+    version='4.0.5',
     author='The Urban Penguin',
     author_email="mahdisahnoun31@gmail.com",  # Replace with your email address
     description='princo package',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    packages=find_packages(), 
+    packages=find_packages(),
     install_requires=[],
 )
```

