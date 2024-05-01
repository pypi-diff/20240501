# Comparing `tmp/scrapkit-1.2.tar.gz` & `tmp/scrapkit-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.2.tar", last modified: Wed May  1 14:27:48 2024, max compression
+gzip compressed data, was "scrapkit-1.3.tar", last modified: Wed May  1 14:36:34 2024, max compression
```

## Comparing `scrapkit-1.2.tar` & `scrapkit-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:27:48.594411 scrapkit-1.2/
--rw-rw-rw-   0        0        0     1563 2024-05-01 14:27:48.577420 scrapkit-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 14:27:48.490472 scrapkit-1.2/scrapkit/
--rw-rw-rw-   0        0        0      110 2024-05-01 14:20:39.000000 scrapkit-1.2/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     1233 2024-05-01 14:22:01.000000 scrapkit-1.2/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:27:48.574422 scrapkit-1.2/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1563 2024-05-01 14:27:48.000000 scrapkit-1.2/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 14:27:48.000000 scrapkit-1.2/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:27:48.000000 scrapkit-1.2/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 14:27:48.000000 scrapkit-1.2/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 14:27:48.000000 scrapkit-1.2/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:27:48.612413 scrapkit-1.2/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 14:25:52.000000 scrapkit-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.257233 scrapkit-1.3/
+-rw-rw-rw-   0        0        0     1592 2024-05-01 14:36:34.253235 scrapkit-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.210260 scrapkit-1.3/scrapkit/
+-rw-rw-rw-   0        0        0      108 2024-05-01 14:35:21.000000 scrapkit-1.3/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-05-01 14:22:01.000000 scrapkit-1.3/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.251236 scrapkit-1.3/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1592 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:36:34.257233 scrapkit-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-01 14:29:43.000000 scrapkit-1.3/setup.py
```

### Comparing `scrapkit-1.2/PKG-INFO` & `scrapkit-1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.2
+Version: 1.3
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
@@ -41,10 +41,11 @@
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
-- ScrapKit 1.0 - It provide you to fetch only HTML of the website
+- ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - Now you also save the Fetched HTML in a `.html` file
+- ScrapKit 1.3 - Bug Fixes
```

### Comparing `scrapkit-1.2/scrapkit/main.py` & `scrapkit-1.3/scrapkit/main.py`

 * *Files identical despite different names*

### Comparing `scrapkit-1.2/scrapkit.egg-info/PKG-INFO` & `scrapkit-1.3/scrapkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.2
+Version: 1.3
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
@@ -41,10 +41,11 @@
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
-- ScrapKit 1.0 - It provide you to fetch only HTML of the website
+- ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - Now you also save the Fetched HTML in a `.html` file
+- ScrapKit 1.3 - Bug Fixes
```

