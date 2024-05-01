# Comparing `tmp/stopwords_tr-1.2.5.tar.gz` & `tmp/stopwords_tr-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.2.5.tar", last modified: Wed May  1 07:36:17 2024, max compression
+gzip compressed data, was "stopwords_tr-2.0.0.tar", last modified: Wed May  1 10:22:01 2024, max compression
```

## Comparing `stopwords_tr-1.2.5.tar` & `stopwords_tr-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 07:36:17.394950 stopwords_tr-1.2.5/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-05-01 07:36:17.394950 stopwords_tr-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 07:36:17.394950 stopwords_tr-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1296 2024-05-01 07:35:50.000000 stopwords_tr-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 07:36:17.385948 stopwords_tr-1.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 07:36:17.388949 stopwords_tr-1.2.5/src/stopwords_tr/
--rw-rw-rw-   0        0        0     2729 2024-05-01 07:35:47.000000 stopwords_tr-1.2.5/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 07:36:17.393950 stopwords_tr-1.2.5/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-05-01 07:36:17.000000 stopwords_tr-1.2.5/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-01 07:36:17.000000 stopwords_tr-1.2.5/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 07:36:17.000000 stopwords_tr-1.2.5/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-01 07:36:17.000000 stopwords_tr-1.2.5/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 10:22:01.223811 stopwords_tr-2.0.0/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1175 2024-05-01 10:22:01.222809 stopwords_tr-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-01 07:50:48.000000 stopwords_tr-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:22:01.223811 stopwords_tr-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2024-05-01 10:18:50.000000 stopwords_tr-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:22:01.213810 stopwords_tr-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 10:22:01.217809 stopwords_tr-2.0.0/src/stopwords_tr/
+-rw-rw-rw-   0        0        0    23960 2024-05-01 10:20:50.000000 stopwords_tr-2.0.0/src/stopwords_tr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:22:01.221810 stopwords_tr-2.0.0/src/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1175 2024-05-01 10:22:01.000000 stopwords_tr-2.0.0/src/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-01 10:22:01.000000 stopwords_tr-2.0.0/src/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:22:01.000000 stopwords_tr-2.0.0/src/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 10:22:01.000000 stopwords_tr-2.0.0/src/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.2.5/LICENSE` & `stopwords_tr-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.2.5/PKG-INFO` & `stopwords_tr-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.5
+Version: 2.0.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
@@ -15,10 +15,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>STOPWORDS FOR TURKISH LANGUAGE</h1>
-<h3>import stopwordstr</h3></h3>
-<h3>stopwordstr.stopwords()</h3>
+# STOPWORDS-TR
+
+Stop words for Turkish.
+
+
+## Installation / Kurulum
+
+```bash
+pip install stopwords_tr
+```
+
+## Usage / Kullanım
+
+```bash
+>>> import stopwords_tr as stp
+>>> stp.stopwords() #Stopwords Array List
+
+```
```

### Comparing `stopwords_tr-1.2.5/setup.py` & `stopwords_tr-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.2.5',
+    version='2.0.0',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
```

### Comparing `stopwords_tr-1.2.5/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-2.0.0/src/stopwords_tr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.5
+Version: 2.0.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
@@ -15,10 +15,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>STOPWORDS FOR TURKISH LANGUAGE</h1>
-<h3>import stopwordstr</h3></h3>
-<h3>stopwordstr.stopwords()</h3>
+# STOPWORDS-TR
+
+Stop words for Turkish.
+
+
+## Installation / Kurulum
+
+```bash
+pip install stopwords_tr
+```
+
+## Usage / Kullanım
+
+```bash
+>>> import stopwords_tr as stp
+>>> stp.stopwords() #Stopwords Array List
+
+```
```

