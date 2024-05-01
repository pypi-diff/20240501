# Comparing `tmp/scrapkit-1.5.tar.gz` & `tmp/scrapkit-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.5.tar", last modified: Wed May  1 15:01:19 2024, max compression
+gzip compressed data, was "scrapkit-1.6.tar", last modified: Wed May  1 15:41:42 2024, max compression
```

## Comparing `scrapkit-1.5.tar` & `scrapkit-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.601565 scrapkit-1.5/
--rw-rw-rw-   0        0        0     1606 2024-05-01 15:01:19.597569 scrapkit-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.573581 scrapkit-1.5/scrapkit/
--rw-rw-rw-   0        0        0      168 2024-05-01 14:57:24.000000 scrapkit-1.5/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     1966 2024-05-01 14:52:50.000000 scrapkit-1.5/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:01:19.595570 scrapkit-1.5/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1606 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 15:01:19.000000 scrapkit-1.5/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 15:01:19.602564 scrapkit-1.5/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 14:56:52.000000 scrapkit-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:41:42.864848 scrapkit-1.6/
+-rw-rw-rw-   0        0        0     1681 2024-05-01 15:41:42.859851 scrapkit-1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 15:41:42.812877 scrapkit-1.6/scrapkit/
+-rw-rw-rw-   0        0        0      300 2024-05-01 15:40:58.000000 scrapkit-1.6/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     3710 2024-05-01 15:41:04.000000 scrapkit-1.6/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:41:42.852855 scrapkit-1.6/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1681 2024-05-01 15:41:42.000000 scrapkit-1.6/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-01 15:41:42.000000 scrapkit-1.6/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 15:41:42.000000 scrapkit-1.6/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-01 15:41:42.000000 scrapkit-1.6/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 15:41:42.000000 scrapkit-1.6/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 15:41:42.865847 scrapkit-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-01 15:39:37.000000 scrapkit-1.6/setup.py
```

### Comparing `scrapkit-1.5/PKG-INFO` & `scrapkit-1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.5
+Version: 1.6
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
@@ -34,8 +34,9 @@
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
 - ScrapKit 1.4 - You can fetch the links given in any website
-- ScrapKit 1.5 - Now you can also fetch the URL of the image on the webpage
+- ScrapKit 1.5 - You can also fetch the URL of the image on the webpage
+- ScrapKit 1.6 - Now you can get Elements data by using their IDs and Classes
```

### Comparing `scrapkit-1.5/scrapkit/main.py` & `scrapkit-1.6/scrapkit/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,7 +55,53 @@
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, 'html.parser')
         img_urls = [img.get('src') for img in soup.find_all('img')]
         return img_urls
     else:
         print("Failed to fetch image URLs. Status code:", response.status_code)
         return None
+
+def getElementByClass(url, class_name):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        elements = soup.find_all(class_=class_name)
+        return elements
+    else:
+        print(f"Failed to fetch elements with class '{class_name}'. Status code:", response.status_code)
+        return None
+
+def getElementById(url, id_name):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        element = soup.find(id=id_name)
+        return element
+    else:
+        print(f"Failed to fetch element with id '{id_name}'. Status code:", response.status_code)
+        return None
+
+def submitForm(url, form_data):
+    response = requests.post(url, data=form_data)
+    if response.status_code == 200:
+        return response.text
+    else:
+        print("Failed to submit form. Status code:", response.status_code)
+        return None
+
+def clickButton(url, button_id):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        form = soup.find('form')
+        button = form.find('button', id=button_id)
+        action_url = form.get('action')
+        button_data = {button.get('name'): button.get('value')}
+        response = requests.post(action_url, data=button_data)
+        if response.status_code == 200:
+            return response.text
+        else:
+            print("Failed to click button. Status code:", response.status_code)
+            return None
+    else:
+        print("Failed to fetch webpage. Status code:", response.status_code)
+        return None
```

### Comparing `scrapkit-1.5/scrapkit.egg-info/PKG-INFO` & `scrapkit-1.6/scrapkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapkit
-Version: 1.5
+Version: 1.6
 Summary: WebScrapping in 3 lines of code
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
 
@@ -34,8 +34,9 @@
 # Versions
 
 - ScrapKit 1.0 - It provide you to fetch whole HTML of the website
 - ScrapKit 1.1 - It provides you to fetch HTML, Title and the Text of the website
 - ScrapKit 1.2 - You can save the Fetched HTML in a `.html` file
 - ScrapKit 1.3 - Bug Fixes
 - ScrapKit 1.4 - You can fetch the links given in any website
-- ScrapKit 1.5 - Now you can also fetch the URL of the image on the webpage
+- ScrapKit 1.5 - You can also fetch the URL of the image on the webpage
+- ScrapKit 1.6 - Now you can get Elements data by using their IDs and Classes
```

