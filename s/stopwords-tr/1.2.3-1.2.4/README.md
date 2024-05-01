# Comparing `tmp/stopwords_tr-1.2.3.tar.gz` & `tmp/stopwords_tr-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.2.3.tar", last modified: Wed May  1 07:31:41 2024, max compression
+gzip compressed data, was "stopwords_tr-1.2.4.tar", last modified: Wed May  1 07:34:45 2024, max compression
```

## Comparing `stopwords_tr-1.2.3.tar` & `stopwords_tr-1.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.229762 stopwords_tr-1.2.3/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-05-01 07:31:41.228763 stopwords_tr-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 07:31:41.229762 stopwords_tr-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1296 2024-05-01 07:31:29.000000 stopwords_tr-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.220762 stopwords_tr-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.223763 stopwords_tr-1.2.3/src/stopwords_tr/
--rw-rw-rw-   0        0        0     2822 2024-05-01 07:29:45.000000 stopwords_tr-1.2.3/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 07:31:41.227763 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-01 07:31:41.000000 stopwords_tr-1.2.3/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:34:45.871157 stopwords_tr-1.2.4/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-05-01 07:34:45.870157 stopwords_tr-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:34:45.871157 stopwords_tr-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2024-05-01 07:34:22.000000 stopwords_tr-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:34:45.861157 stopwords_tr-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:34:45.864157 stopwords_tr-1.2.4/src/stopwords_tr/
+-rw-rw-rw-   0        0        0     2749 2024-05-01 07:34:10.000000 stopwords_tr-1.2.4/src/stopwords_tr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:34:45.869157 stopwords_tr-1.2.4/src/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-05-01 07:34:45.000000 stopwords_tr-1.2.4/src/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-01 07:34:45.000000 stopwords_tr-1.2.4/src/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:34:45.000000 stopwords_tr-1.2.4/src/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 07:34:45.000000 stopwords_tr-1.2.4/src/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.2.3/LICENSE` & `stopwords_tr-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.2.3/PKG-INFO` & `stopwords_tr-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.3
+Version: 1.2.4
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.2.3/setup.py` & `stopwords_tr-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.2.3',
+    version='1.2.4',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
```

### Comparing `stopwords_tr-1.2.3/src/stopwords_tr/__init__.py` & `stopwords_tr-1.2.4/src/stopwords_tr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,4 @@
 def stopwords():
     stopwordsarr=["edilecek", "onlari", "bile", "nın", "dahi", "çoğunu", "kimi", "birşey", "edilmesi", "birşeyi", "herkesin", "ta", "etmesi", "şeyden", "kendine", "olmadı", "benden", "diğeri", "onlardan", "hangi", "daha", "hala", "itibaren", "bazen", "kendini", "nasıl", "senden", "onlara", "hiçbiri", "zira", "dört", "bizim", "ve", "hiç", "olan", "önce", "şunları", "olup", "bazıları", "gereği", "tüm", "beri", "ben", "olsun", "ün", "şayet", "bizden", "buna", "beş", "az", "artık", "bunun", "olması", "bunların", "size", "ise", "ü", "defa", "şeye", "diğerleri", "hepsi", "itibariyle", "ancak", "herkese", "dolayısıyla", "nün", "katrilyon", "çok", "elbette", "üç", "şuna", "ediliyor", "yaptıkları", "burada", "onların", "hani", "iki", "oluyor", "değil", "yaptı", "sanki", "nerde", "onlar", "o", "bu", "olmak", "neden", "veya", "ilgili", "şöyle", "öbür", "bizi", "un", "biz", "benim", "seni", "sekiz", "yi", "sizin", "ederek", "u", "bunda", "madem", "filan", "bin", "otuz", "öyle", "gerek", "kaç", "yapılan", "olur", "dan", "ile", "nedenle", "halde", "mü", "birçoğu", "yetmiş", "içinde", "ya", "mu", "birçok", "tamam", "eden", "ayrıca", "ettiğini", "kırk", "bunu", "yüz", "üzere", "bana", "oysa", "mı", "ki", "böyle", "yapacak", "yedi", "bütün", "yapmak", "her", "siz", "bize", "olmaz", "yaptığı", "acaba", "herhangi", "olduklarını", "edecek", "bazı", "tabii", "sizden", "doksan", "beyden", "tamamen", "herkes", "kendilerine", "kendisine", "olursa", "yaptığını", "kime", "hangisi", "elli", "ön", "birkez", "de", "bundan", "senin", "onu", "kendisi", "yapılması", "olduğu", "kez", "mi", "ediyor", "yine", "milyar", "birisi", "pek", "kendisini", "olmayan", "milyon", "yu", "ötürü", "tümü", "ı", "çünkü", "kim", "sizi", "şekilde", "onları", "kendi", "falan", "bey", "altı", "nun", "hatta", "fakat", "ye", "seksen", "yerine", "göre", "dolayı", "neyse", "ne", "şey", "a", "vardı", "için", "hiçbir", "trilyon", "şeyler", "arada", "kimden", "en", "bunlar", "belki", "gibi", "hem", "on", "onun", "kimisi", "nereye", "i", "biraz", "şeyi", "niye", "etti", "olduğunu", "tam", "henüz", "asla", "niçin", "öte", "kadar", "kimin", "rağmen", "zaten", "beni", "ettiği", "şimdi", "yani", "bilhassa", "dokuz", "sen", "bir", "böylece", "eğer", "hep", "lakin", "nerede", "nin", "tarafından", "sonra", "yı", "beyler", "gene", "var", "oldu", "ona", "olarak", "birkaç", "yapıyor", "diye", "biri", "çoğu", "da", "işte", "olmadığı", "karşın", "altmış", "yoksa", "aslında", "halen", "şunu", "e", "kimse", "sana", "şu", "orada", "ama", "ondan", "olsa", "yirmi", "diğer", "herkesi", "bunları"]
-    stopwords=[]
-    for i in stopwordsarr:
-        i=i[0:-1]
-        stopwords.append(i)
-    return stopwords
+    return stopwordsarr
+print(stopwords())
```

### Comparing `stopwords_tr-1.2.3/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.2.4/src/stopwords_tr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.3
+Version: 1.2.4
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

