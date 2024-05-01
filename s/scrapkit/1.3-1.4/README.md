# Comparing `tmp/scrapkit-1.3.tar.gz` & `tmp/scrapkit-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.3.tar", last modified: Wed May  1 14:36:34 2024, max compression
+gzip compressed data, was "scrapkit-1.4.tar", last modified: Wed May  1 14:47:46 2024, max compression
```

## Comparing `scrapkit-1.3.tar` & `scrapkit-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.257233 scrapkit-1.3/
--rw-rw-rw-   0        0        0     1592 2024-05-01 14:36:34.253235 scrapkit-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.210260 scrapkit-1.3/scrapkit/
--rw-rw-rw-   0        0        0      108 2024-05-01 14:35:21.000000 scrapkit-1.3/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     1233 2024-05-01 14:22:01.000000 scrapkit-1.3/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:36:34.251236 scrapkit-1.3/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1592 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 14:36:34.000000 scrapkit-1.3/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:36:34.257233 scrapkit-1.3/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 14:29:43.000000 scrapkit-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.646178 scrapkit-1.4/
+-rw-rw-rw-   0        0        0     1457 2024-05-01 14:47:46.637196 scrapkit-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.612197 scrapkit-1.4/scrapkit/
+-rw-rw-rw-   0        0        0      136 2024-05-01 14:39:50.000000 scrapkit-1.4/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-05-01 14:47:14.000000 scrapkit-1.4/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.625190 scrapkit-1.4/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1457 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:47:46.646178 scrapkit-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-01 14:42:44.000000 scrapkit-1.4/setup.py
```

### Comparing `scrapkit-1.3/PKG-INFO` & `scrapkit-1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.3
+Version: 1.4
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
-# ScrapKit 1.2 - WebScrapping is now easy
+# ScrapKit 1.4 - WebScrapping is now easy
 
 ## Usage
 
 ScrapKit is a very useful Python Package that allows you to get the HTML of any website in just one line of code. You don't need to manually import `requests` and `beautifulsoup` type of module from now
 
 ## Syntax
 
-ScrapKit can fetch HTML, Title, Text of the website. But After this update you can now also save the html file with a very easy Syntax
+ScrapKit can fetch HTML, Title, Text of the website and can save the Fetched HTML in a file. But After this update you can now also get the Links on any webpage with a very easy syntax
 
 ```python
 import scrapkit as sk
 
 url = 'https://www.youtube.com'
 
-# Now you can save the fetched HTML in a File
-st.saveHTML (url, filename='youtube.html')
-
-# Fetch the Title of the website
-title = st.getTitle (url)
-print (title)
-
-# Fetch the HTML of the website
-html = st.getHTML (url)
-print (html)
-
-# Fetch the Text of the website
-text = st.getText (url)
-print (text)
+# Now you can fetch the Links on the webpage
+st.getLinks (url)
 ```
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
-- ScrapKit 1.2 - Now you also save the Fetched HTML in a `.html` file
+- ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
+- ScrapKit 1.4 - Now You can also fetch the links given in any website
```

### Comparing `scrapkit-1.3/scrapkit.egg-info/PKG-INFO` & `scrapkit-1.4/scrapkit.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.3
+Version: 1.4
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
-# ScrapKit 1.2 - WebScrapping is now easy
+# ScrapKit 1.4 - WebScrapping is now easy
 
 ## Usage
 
 ScrapKit is a very useful Python Package that allows you to get the HTML of any website in just one line of code. You don't need to manually import `requests` and `beautifulsoup` type of module from now
 
 ## Syntax
 
-ScrapKit can fetch HTML, Title, Text of the website. But After this update you can now also save the html file with a very easy Syntax
+ScrapKit can fetch HTML, Title, Text of the website and can save the Fetched HTML in a file. But After this update you can now also get the Links on any webpage with a very easy syntax
 
 ```python
 import scrapkit as sk
 
 url = 'https://www.youtube.com'
 
-# Now you can save the fetched HTML in a File
-st.saveHTML (url, filename='youtube.html')
-
-# Fetch the Title of the website
-title = st.getTitle (url)
-print (title)
-
-# Fetch the HTML of the website
-html = st.getHTML (url)
-print (html)
-
-# Fetch the Text of the website
-text = st.getText (url)
-print (text)
+# Now you can fetch the Links on the webpage
+st.getLinks (url)
 ```
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
-- ScrapKit 1.2 - Now you also save the Fetched HTML in a `.html` file
+- ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
+- ScrapKit 1.4 - Now You can also fetch the links given in any website
```

