# Comparing `tmp/oscb-1.7.9.tar.gz` & `tmp/oscb-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.7.9.tar", last modified: Tue Apr 30 01:36:11 2024, max compression
+gzip compressed data, was "oscb-1.8.9.tar", last modified: Wed May  1 01:48:10 2024, max compression
```

## Comparing `oscb-1.7.9.tar` & `oscb-1.8.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 01:36:11.434860 oscb-1.7.9/
--rw-rw-rw-   0        0        0       48 2024-04-28 06:24:03.000000 oscb-1.7.9/MANIFEST.in
--rw-rw-rw-   0        0        0      658 2024-04-30 01:36:11.434860 oscb-1.7.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 01:36:11.410861 oscb-1.7.9/oscb/
--rw-rw-rw-   0        0        0       57 2024-04-29 02:09:08.000000 oscb-1.7.9/oscb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:36:11.432860 oscb-1.7.9/oscb/download_dataset/
--rw-rw-rw-   0        0        0       99 2024-04-30 00:21:20.000000 oscb-1.7.9/oscb/download_dataset/__init__.py
--rw-rw-rw-   0        0        0      193 2024-04-23 23:03:07.000000 oscb-1.7.9/oscb/download_dataset/download_file.py
--rw-rw-rw-   0        0        0     2529 2024-04-23 23:06:51.000000 oscb-1.7.9/oscb/download_dataset/download_utils.py
--rw-rw-rw-   0        0        0      650 2024-04-30 01:35:45.000000 oscb-1.7.9/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:36:11.429861 oscb-1.7.9/oscb.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-30 01:36:11.000000 oscb-1.7.9/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-30 01:36:11.000000 oscb-1.7.9/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 01:36:11.000000 oscb-1.7.9/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-30 01:36:11.000000 oscb-1.7.9/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-30 01:36:11.000000 oscb-1.7.9/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 01:36:11.434860 oscb-1.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1670 2024-04-30 01:36:03.000000 oscb-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.602944 oscb-1.8.9/
+-rw-rw-rw-   0        0        0       26 2024-05-01 01:43:58.000000 oscb-1.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      658 2024-05-01 01:48:10.601946 oscb-1.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.542994 oscb-1.8.9/oscb/
+-rw-rw-rw-   0        0        0       57 2024-04-29 02:09:08.000000 oscb-1.8.9/oscb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.600946 oscb-1.8.9/oscb/download_dataset/
+-rw-rw-rw-   0        0        0       99 2024-04-30 00:21:20.000000 oscb-1.8.9/oscb/download_dataset/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-04-23 23:03:07.000000 oscb-1.8.9/oscb/download_dataset/download_file.py
+-rw-rw-rw-   0        0        0     2529 2024-04-23 23:06:51.000000 oscb-1.8.9/oscb/download_dataset/download_utils.py
+-rw-rw-rw-   0        0        0      650 2024-05-01 01:47:35.000000 oscb-1.8.9/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:48:10.574046 oscb-1.8.9/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 01:48:10.000000 oscb-1.8.9/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 01:48:10.602944 oscb-1.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1801 2024-05-01 01:47:21.000000 oscb-1.8.9/setup.py
```

### Comparing `oscb-1.7.9/PKG-INFO` & `oscb-1.8.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.7.9
+Version: 1.8.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
-Author: Your Name
+Author: OSCB TEAM
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `oscb-1.7.9/oscb/download_dataset/download_utils.py` & `oscb-1.8.9/oscb/download_dataset/download_utils.py`

 * *Files identical despite different names*

### Comparing `oscb-1.7.9/oscb/version.py` & `oscb-1.8.9/oscb/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.7.9'
+__version__ = '1.8.9'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.7.9/oscb.egg-info/PKG-INFO` & `oscb-1.8.9/oscb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.7.9
+Version: 1.8.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
-Author: Your Name
+Author: OSCB TEAM
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `oscb-1.7.9/setup.py` & `oscb-1.8.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,43 +3,46 @@
 
 # Get the current directory
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Function to collect all files under oscb folder
 def find_oscb_files():
     oscb_files = []
-    for root, _, files in os.walk(os.path.join(here, 'oscb')):
+    oscb_dir = os.path.join(here, 'oscb')
+    for root, _, files in os.walk(oscb_dir):
         for file in files:
-            oscb_files.append(os.path.relpath(os.path.join(root, file), here))
+            # Get the relative path of the file
+            rel_path = os.path.relpath(os.path.join(root, file), oscb_dir)
+            oscb_files.append(rel_path)
     return oscb_files
 
-# Include the oscb/download_dataset directory as well
+# Include the parent oscb directory and its contents
 oscb_files = find_oscb_files()
 
 setup(
     name='oscb',
-    version='1.7.9',
+    version='1.8.9',
     description='Description of your package',
     long_description='Long description of your package',
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/oscb',
-    author='Your Name',
+    author='OSCB TEAM',
     author_email='your.email@example.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords='sample setuptools development',
     packages=find_packages(),
-    package_data={'oscb': oscb_files},  # Specify package data directly
+    package_data={'oscb': oscb_files},  # Include all files and folders under oscb directory
     include_package_data=True,
     install_requires=[
         'torch>=1.6.0',
         'numpy>=1.16.0',
         'tqdm>=4.29.0',
         'scikit-learn>=0.20.0',
         'pandas>=0.24.0',
```

