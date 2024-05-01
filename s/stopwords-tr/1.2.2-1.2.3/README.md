# Comparing `tmp/stopwords_tr-1.2.2.tar.gz` & `tmp/stopwords_tr-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.2.2.tar", last modified: Tue Apr 30 09:14:41 2024, max compression
+gzip compressed data, was "stopwords_tr-1.2.3.tar", last modified: Wed May  1 07:31:41 2024, max compression
```

## Comparing `stopwords_tr-1.2.2.tar` & `stopwords_tr-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 09:14:41.869525 stopwords_tr-1.2.2/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 09:14:41.868524 stopwords_tr-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 09:14:41.869525 stopwords_tr-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1296 2024-04-30 09:14:31.000000 stopwords_tr-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:14:41.859524 stopwords_tr-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 09:14:41.862524 stopwords_tr-1.2.2/src/stopwords_tr/
--rw-rw-rw-   0        0        0      157 2024-04-30 09:11:56.000000 stopwords_tr-1.2.2/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:14:41.868524 stopwords_tr-1.2.2/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 09:14:41.000000 stopwords_tr-1.2.2/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-30 09:14:41.000000 stopwords_tr-1.2.2/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 09:14:41.000000 stopwords_tr-1.2.2/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 09:14:41.000000 stopwords_tr-1.2.2/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.229762 stopwords_tr-1.2.3/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-05-01 07:31:41.228763 stopwords_tr-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:31:41.229762 stopwords_tr-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2024-05-01 07:31:29.000000 stopwords_tr-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.220762 stopwords_tr-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.223763 stopwords_tr-1.2.3/src/stopwords_tr/
+-rw-rw-rw-   0        0        0     2822 2024-05-01 07:29:45.000000 stopwords_tr-1.2.3/src/stopwords_tr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.227763 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.2.2/LICENSE` & `stopwords_tr-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.2.2/PKG-INFO` & `stopwords_tr-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.2.2/setup.py` & `stopwords_tr-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.2.2',
+    version='1.2.3',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
```

### Comparing `stopwords_tr-1.2.2/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.2.3/src/stopwords_tr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

