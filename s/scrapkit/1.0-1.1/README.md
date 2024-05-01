# Comparing `tmp/scrapkit-1.0.tar.gz` & `tmp/scrapkit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.0.tar", last modified: Wed May  1 14:07:53 2024, max compression
+gzip compressed data, was "scrapkit-1.1.tar", last modified: Wed May  1 14:20:19 2024, max compression
```

## Comparing `scrapkit-1.0.tar` & `scrapkit-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:07:53.903328 scrapkit-1.0/
--rw-rw-rw-   0        0        0     1015 2024-05-01 14:07:53.901329 scrapkit-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 14:07:53.841364 scrapkit-1.0/scrapkit/
--rw-rw-rw-   0        0        0      115 2024-05-01 13:57:44.000000 scrapkit-1.0/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-05-01 13:57:37.000000 scrapkit-1.0/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:07:53.897331 scrapkit-1.0/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1015 2024-05-01 14:07:53.000000 scrapkit-1.0/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 14:07:53.000000 scrapkit-1.0/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:07:53.000000 scrapkit-1.0/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 14:07:53.000000 scrapkit-1.0/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 14:07:53.000000 scrapkit-1.0/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:07:53.908335 scrapkit-1.0/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 13:59:14.000000 scrapkit-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:20:19.445815 scrapkit-1.1/
+-rw-rw-rw-   0        0        0     1365 2024-05-01 14:20:19.442816 scrapkit-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 14:20:19.399841 scrapkit-1.1/scrapkit/
+-rw-rw-rw-   0        0        0      110 2024-05-01 14:20:00.000000 scrapkit-1.1/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     1249 2024-05-01 14:13:11.000000 scrapkit-1.1/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:20:19.439818 scrapkit-1.1/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1365 2024-05-01 14:20:19.000000 scrapkit-1.1/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-01 14:20:19.000000 scrapkit-1.1/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:20:19.000000 scrapkit-1.1/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-01 14:20:19.000000 scrapkit-1.1/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 14:20:19.000000 scrapkit-1.1/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:20:19.445815 scrapkit-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-01 14:12:50.000000 scrapkit-1.1/setup.py
```

### Comparing `scrapkit-1.0/scrapkit/main.py` & `scrapkit-1.1/scrapkit/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import requests
 from bs4 import BeautifulSoup
 
-# def getTitle(url):
-#     response = requests.get(url)
-#     if response.status_code == 200:
-#         soup = BeautifulSoup(response.text, 'html.parser')
-#         title = soup.title.string
-#         return title
-#     else:
-#         print("Failed to fetch title. Status code:", response.status_code)
-#         return None
+def getTitle(url):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        title = soup.title.string
+        return title
+    else:
+        print("Failed to fetch title. Status code:", response.status_code)
+        return None
 
 def getHTML(url):
     response = requests.get(url)
     if response.status_code == 200:
         return response.text
     else:
         print("Failed to fetch HTML content. Status code:", response.status_code)
         return None
 
-# def getText(url):
-#     response = requests.get(url)
-#     if response.status_code == 200:
-#         soup = BeautifulSoup(response.text, 'html.parser')
-#         text = soup.get_text()
-#         return text
-#     else:
-#         print("Failed to fetch text content. Status code:", response.status_code)
-#         return None
+def getText(url):
+    response = requests.get(url)
+    if response.status_code == 200:
+        soup = BeautifulSoup(response.text, 'html.parser')
+        text = soup.get_text()
+        return text
+    else:
+        print("Failed to fetch text content. Status code:", response.status_code)
+        return None
 
 # def saveHTML(url, filename="output.html"):
 #     html_content = getHTML(url)
 #     if html_content:
 #         with open(filename, "w", encoding="utf-8") as file:
 #             file.write(html_content)
 #         print(f"HTML content saved to {filename}")
```

