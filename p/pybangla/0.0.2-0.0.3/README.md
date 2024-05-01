# Comparing `tmp/pybangla-0.0.2.tar.gz` & `tmp/pybangla-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-0.0.2.tar", last modified: Tue Apr 30 17:37:02 2024, max compression
+gzip compressed data, was "pybangla-0.0.3.tar", last modified: Wed May  1 18:16:33 2024, max compression
```

## Comparing `pybangla-0.0.2.tar` & `pybangla-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/
--rw-rw-r--   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:27:19.000000 pybangla-0.0.2/MANIFEST.in
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    13705 2024-04-30 17:37:02.321241 pybangla-0.0.2/PKG-INFO
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    13196 2024-04-30 17:31:39.000000 pybangla-0.0.2/README.md
-drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla/
--rw-rw-r--   0 sayan     (1000) sayan     (1000)       66 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/__init__.py
-drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla/module/
--rw-rw-r--   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/__init__.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    16979 2024-04-30 17:31:06.000000 pybangla-0.0.2/pybangla/module/config.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)     9002 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/main.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    16398 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/number_parser.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    15187 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/parser.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    22922 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/word_to_number.py
--rw-rw-r--   0 sayan     (1000) sayan     (1000)     8917 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/test.py
-drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla.egg-info/
--rw-rw-r--   0 sayan     (1000) sayan     (1000)    13705 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/PKG-INFO
--rw-rw-r--   0 sayan     (1000) sayan     (1000)      422 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/SOURCES.txt
--rw-rw-r--   0 sayan     (1000) sayan     (1000)        1 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/dependency_links.txt
--rw-rw-r--   0 sayan     (1000) sayan     (1000)       19 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/requires.txt
--rw-rw-r--   0 sayan     (1000) sayan     (1000)        9 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/top_level.txt
--rw-rw-r--   0 sayan     (1000) sayan     (1000)       38 2024-04-30 17:37:02.321241 pybangla-0.0.2/setup.cfg
--rw-rw-r--   0 sayan     (1000) sayan     (1000)      940 2024-04-30 17:35:35.000000 pybangla-0.0.2/setup.py
-drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/tests/
--rw-rw-r--   0 sayan     (1000) sayan     (1000)     2751 2024-04-30 17:27:19.000000 pybangla-0.0.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:26.000000 pybangla-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:16:33.281125 pybangla-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-05-01 18:16:26.000000 pybangla-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.277125 pybangla-0.0.3/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-01 18:16:26.000000 pybangla-0.0.3/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:16:33.000000 pybangla-0.0.3/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:16:33.281125 pybangla-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 18:16:26.000000 pybangla-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:33.281125 pybangla-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-01 18:16:26.000000 pybangla-0.0.3/tests/test.py
```

### Comparing `pybangla-0.0.2/PKG-INFO` & `pybangla-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pybangla
-Version: 0.0.2
-Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
-Home-page: https://github.com/saiful9379/pybangla
-Author: saiful
-Author-email: saifulbrur79@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
@@ -34,14 +20,15 @@
 
 
 
 
 # Usage
 
 ## 1. Text Normalization
+### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 text = "রাহিম ক্লাস ওয়ান এ ১ম, এন্ড বাসার ক্লাস এ ৩৩ তম, সে জন্য ২০৩০ শতাব্দীতে ¥২০৩০.১২৩৪ দিতে হয়েছে"
 text = nrml.text_normalizer(text)
 
@@ -106,15 +93,15 @@
 ("₽", "রুবেল"), 
 ("₺", "লিরা")
 
 ```
 
 
 ## 2. Number Conversion
-
+### It supports converting Bangla text numbers to numeric numbers.
 ```py
 text = "আপনার ফোন নম্বর হলো জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন"
 text = nrml.word2number(text)
 
 #output:
 
 'আপনার ফোন নম্বর হলো 01773559379 '
@@ -195,14 +182,17 @@
 number = "2013"
 number = nrml.number_convert(number, language="bn")
 #output
 {'digit': '২০১৩', 'digit_word': 'দুই শূন্য এক তিন', 'number_string': 'দুই হাজার তেরো'}
 ```
 
 ## 3. Date Format
+
+### It supports converting different formats of Bangla date to English date.
+
 ```py
 
 import pybangla
 nrml = pybangla.Normalizer()
 date = "০১-এপ্রিল/২০২৩"
 date = nrml.date_format(date, language="en")
 print(date)
@@ -299,14 +289,15 @@
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
 ## 4. Today, Months, Weekdays, Seasons
+### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 today = nrml.today()
```

### Comparing `pybangla-0.0.2/README.md` & `pybangla-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pybangla
+Version: 0.0.3
+Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
+Home-page: https://github.com/saiful9379/pybangla
+Author: saiful
+Author-email: saifulbrur79@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: DateTime
+Requires-Dist: num2words
+
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
@@ -20,14 +36,15 @@
 
 
 
 
 # Usage
 
 ## 1. Text Normalization
+### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 text = "রাহিম ক্লাস ওয়ান এ ১ম, এন্ড বাসার ক্লাস এ ৩৩ তম, সে জন্য ২০৩০ শতাব্দীতে ¥২০৩০.১২৩৪ দিতে হয়েছে"
 text = nrml.text_normalizer(text)
 
@@ -92,15 +109,15 @@
 ("₽", "রুবেল"), 
 ("₺", "লিরা")
 
 ```
 
 
 ## 2. Number Conversion
-
+### It supports converting Bangla text numbers to numeric numbers.
 ```py
 text = "আপনার ফোন নম্বর হলো জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন"
 text = nrml.word2number(text)
 
 #output:
 
 'আপনার ফোন নম্বর হলো 01773559379 '
@@ -181,14 +198,17 @@
 number = "2013"
 number = nrml.number_convert(number, language="bn")
 #output
 {'digit': '২০১৩', 'digit_word': 'দুই শূন্য এক তিন', 'number_string': 'দুই হাজার তেরো'}
 ```
 
 ## 3. Date Format
+
+### It supports converting different formats of Bangla date to English date.
+
 ```py
 
 import pybangla
 nrml = pybangla.Normalizer()
 date = "০১-এপ্রিল/২০২৩"
 date = nrml.date_format(date, language="en")
 print(date)
@@ -285,14 +305,15 @@
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
 ## 4. Today, Months, Weekdays, Seasons
+### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 today = nrml.today()
```

### Comparing `pybangla-0.0.2/pybangla/module/config.py` & `pybangla-0.0.3/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla/module/main.py` & `pybangla-0.0.3/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla/module/number_parser.py` & `pybangla-0.0.3/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla/module/parser.py` & `pybangla-0.0.3/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla/module/word_to_number.py` & `pybangla-0.0.3/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla/test.py` & `pybangla-0.0.3/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.2/pybangla.egg-info/PKG-INFO` & `pybangla-0.0.3/pybangla.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.2
+Version: 0.0.3
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: DateTime
+Requires-Dist: num2words
 
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
@@ -34,14 +36,15 @@
 
 
 
 
 # Usage
 
 ## 1. Text Normalization
+### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 text = "রাহিম ক্লাস ওয়ান এ ১ম, এন্ড বাসার ক্লাস এ ৩৩ তম, সে জন্য ২০৩০ শতাব্দীতে ¥২০৩০.১২৩৪ দিতে হয়েছে"
 text = nrml.text_normalizer(text)
 
@@ -106,15 +109,15 @@
 ("₽", "রুবেল"), 
 ("₺", "লিরা")
 
 ```
 
 
 ## 2. Number Conversion
-
+### It supports converting Bangla text numbers to numeric numbers.
 ```py
 text = "আপনার ফোন নম্বর হলো জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন"
 text = nrml.word2number(text)
 
 #output:
 
 'আপনার ফোন নম্বর হলো 01773559379 '
@@ -195,14 +198,17 @@
 number = "2013"
 number = nrml.number_convert(number, language="bn")
 #output
 {'digit': '২০১৩', 'digit_word': 'দুই শূন্য এক তিন', 'number_string': 'দুই হাজার তেরো'}
 ```
 
 ## 3. Date Format
+
+### It supports converting different formats of Bangla date to English date.
+
 ```py
 
 import pybangla
 nrml = pybangla.Normalizer()
 date = "০১-এপ্রিল/২০২৩"
 date = nrml.date_format(date, language="en")
 print(date)
@@ -299,14 +305,15 @@
 print(f"{en_date}")
 
 # Output :
 {'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
 ```
 
 ## 4. Today, Months, Weekdays, Seasons
+### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
 ## 1. Today:
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 today = nrml.today()
```

### Comparing `pybangla-0.0.2/setup.py` & `pybangla-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-0.0.2/tests/test.py` & `pybangla-0.0.3/tests/test.py`

 * *Files identical despite different names*

