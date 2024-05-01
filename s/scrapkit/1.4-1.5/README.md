# Comparing `tmp/scrapkit-1.4.tar.gz` & `tmp/scrapkit-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.4.tar", last modified: Wed May  1 14:47:46 2024, max compression
+gzip compressed data, was "scrapkit-1.5.tar", last modified: Wed May  1 15:01:19 2024, max compression
```

## Comparing `scrapkit-1.4.tar` & `scrapkit-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.646178 scrapkit-1.4/
--rw-rw-rw-   0        0        0     1457 2024-05-01 14:47:46.637196 scrapkit-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.612197 scrapkit-1.4/scrapkit/
--rw-rw-rw-   0        0        0      136 2024-05-01 14:39:50.000000 scrapkit-1.4/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     1984 2024-05-01 14:47:14.000000 scrapkit-1.4/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:47:46.625190 scrapkit-1.4/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1457 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 14:47:45.000000 scrapkit-1.4/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:47:46.646178 scrapkit-1.4/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 14:42:44.000000 scrapkit-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.601565 scrapkit-1.5/
+-rw-rw-rw-   0        0        0     1606 2024-05-01 15:01:19.597569 scrapkit-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.573581 scrapkit-1.5/scrapkit/
+-rw-rw-rw-   0        0        0      168 2024-05-01 14:57:24.000000 scrapkit-1.5/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     1966 2024-05-01 14:52:50.000000 scrapkit-1.5/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.595570 scrapkit-1.5/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1606 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 15:01:19.602564 scrapkit-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-01 14:56:52.000000 scrapkit-1.5/setup.py
```

### Comparing `scrapkit-1.4/PKG-INFO` & `scrapkit-1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.4
+Version: 1.5
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
-# ScrapKit 1.4 - WebScrapping is now easy
+# ScrapKit 1.5 - WebScrapping is now easy
 
 ## Usage
 
 ScrapKit is a very useful Python Package that allows you to get the HTML of any website in just one line of code. You don't need to manually import `requests` and `beautifulsoup` type of module from now
 
 ## Syntax
 
-ScrapKit can fetch HTML, Title, Text of the website and can save the Fetched HTML in a file. But After this update you can now also get the Links on any webpage with a very easy syntax
+ScrapKit can fetch HTML, Title, Text of the website, you can save the Fetched HTML in a file and fetch the links on the webpage. But After this update you can now also get URLs of the images on any webpage with a very easy syntax
 
 ```python
 import scrapkit as sk
 
-url = 'https://www.youtube.com'
+url = 'https://en.wikipedia.org/wiki/Adolf_Hitler'
 
-# Now you can fetch the Links on the webpage
-st.getLinks (url)
+# Now you can fetch the URLs of the images on the webpage
+st.getImageUrls (url)
 ```
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
-- ScrapKit 1.4 - Now You can also fetch the links given in any website
+- ScrapKit 1.4 - You can fetch the links given in any website
+- ScrapKit 1.5 - Now you can also fetch the URL of the image on the webpage
```

### Comparing `scrapkit-1.4/scrapkit/main.py` & `scrapkit-1.5/scrapkit/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         soup = BeautifulSoup(response.text, 'html.parser')
         links = [link.get('href') for link in soup.find_all('a')]
         return links
     else:
         print("Failed to fetch links. Status code:", response.status_code)
         return None
 
-# def getImageUrls(url):
-#     response = requests.get(url)
-#     if response.status_code == 200:
-#         soup = BeautifulSoup(response.text, 'html.parser')
-#         img_urls = [img.get('src') for img in soup.find_all('img')]
-#         return img_urls
-#     else:
-#         print("Failed to fetch image URLs. Status code:", response.status_code)
-#         return None
+def getImageUrls(url):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        img_urls = [img.get('src') for img in soup.find_all('img')]
+        return img_urls
+    else:
+        print("Failed to fetch image URLs. Status code:", response.status_code)
+        return None
```

### Comparing `scrapkit-1.4/scrapkit.egg-info/PKG-INFO` & `scrapkit-1.5/scrapkit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.4
+Version: 1.5
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
-# ScrapKit 1.4 - WebScrapping is now easy
+# ScrapKit 1.5 - WebScrapping is now easy
 
 ## Usage
 
 ScrapKit is a very useful Python Package that allows you to get the HTML of any website in just one line of code. You don't need to manually import `requests` and `beautifulsoup` type of module from now
 
 ## Syntax
 
-ScrapKit can fetch HTML, Title, Text of the website and can save the Fetched HTML in a file. But After this update you can now also get the Links on any webpage with a very easy syntax
+ScrapKit can fetch HTML, Title, Text of the website, you can save the Fetched HTML in a file and fetch the links on the webpage. But After this update you can now also get URLs of the images on any webpage with a very easy syntax
 
 ```python
 import scrapkit as sk
 
-url = 'https://www.youtube.com'
+url = 'https://en.wikipedia.org/wiki/Adolf_Hitler'
 
-# Now you can fetch the Links on the webpage
-st.getLinks (url)
+# Now you can fetch the URLs of the images on the webpage
+st.getImageUrls (url)
 ```
 
 # Founder
 
 ScrapKit is a very useful python package that is made by the one and only "Ali Lodhi". Ali Lodhi is from Pakistan, He loves to write code in python and try to easy people's work. Recently Ali Lodhi is working on the next update of this package
 
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
-- ScrapKit 1.4 - Now You can also fetch the links given in any website
+- ScrapKit 1.4 - You can fetch the links given in any website
+- ScrapKit 1.5 - Now you can also fetch the URL of the image on the webpage
```

