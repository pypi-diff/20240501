# Comparing `tmp/tebbytools-0.2.5.tar.gz` & `tmp/tebbytools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tebbytools-0.2.5.tar", last modified: Sat Apr 27 22:54:30 2024, max compression
+gzip compressed data, was "tebbytools-0.3.3.tar", last modified: Wed May  1 12:46:57 2024, max compression
```

## Comparing `tebbytools-0.2.5.tar` & `tebbytools-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:54:30.781155 tebbytools-0.2.5/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:54:30.780975 tebbytools-0.2.5/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1933 2024-04-27 22:54:19.000000 tebbytools-0.2.5/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-27 22:54:30.781198 tebbytools-0.2.5/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-27 22:54:19.000000 tebbytools-0.2.5/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:54:30.779044 tebbytools-0.2.5/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:54:30.779847 tebbytools-0.2.5/src/tebbytools/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       99 2024-04-27 22:29:15.000000 tebbytools-0.2.5/src/tebbytools/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.2.5/src/tebbytools/reviewlist.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.2.5/src/tebbytools/wordbank.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:54:30.780807 tebbytools-0.2.5/src/tebbytools.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:54:30.000000 tebbytools-0.2.5/src/tebbytools.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      253 2024-04-27 22:54:30.000000 tebbytools-0.2.5/src/tebbytools.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-27 22:54:30.000000 tebbytools-0.2.5/src/tebbytools.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-27 22:54:30.000000 tebbytools-0.2.5/src/tebbytools.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.032612 tebbytools-0.3.3/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 12:46:57.032436 tebbytools-0.3.3/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2074 2024-05-01 12:39:54.000000 tebbytools-0.3.3/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-05-01 12:46:57.032660 tebbytools-0.3.3/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-05-01 12:46:26.000000 tebbytools-0.3.3/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.030480 tebbytools-0.3.3/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.031520 tebbytools-0.3.3/src/tebbytools/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-05-01 12:39:54.000000 tebbytools-0.3.3/src/tebbytools/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.3/src/tebbytools/reviewlist.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     5366 2024-05-01 12:39:54.000000 tebbytools-0.3.3/src/tebbytools/wordbank.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.032254 tebbytools-0.3.3/src/tebbytools.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      253 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/top_level.txt
```

### Comparing `tebbytools-0.2.5/README.md` & `tebbytools-0.3.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,41 @@
 pip install tebbytools
 ```
 
 ## Usage
 
 ### Word bank
 
-A `WordBank` manages a json file that contains a list of words you've encountered.
+A `WordBank` manages a database file that contains a list of words you've encountered.
 You can add words to the bank and query them in various ways.
 
 ```python
 from tebbytools import WordBank
 
 # Initialize a WordBank instance
-wb = WordBank(file_path="path/to/your/word_bank.json")
+wb = WordBank(file_path="path/to/your/word_bank.db")
 
 # Set a new file path
-wb.set_file_path("new/path/to/your/word_bank.json")
+wb.set_file_path("new/path/to/your/word_bank.db")
 
-# Add a word to the bank with optional tags
-wb.add_word("hello", tags=["greeting", "basic"])
+# Add a word to the bank with optional date_time and tags
+# If date_time is not specified, datetime.now() will be used
+wb.add_word("hello", date_time=datetime.now(), tags=["greeting", "basic"])
 
 # Get all words in the bank
 words = wb.get_all_words()
 
 # Get all unique words in the bank
 unique_words = wb.get_all_unique_words()
 
 # Get words added in the past n days
 recent_words = wb.get_words_from_past_n_days(7)
 
 # Get words added today
+# Same as get_words_from_past_n_days(0)
 todays_words = wb.get_todays_words()
 
 # Get words by a specific tag
 greeting_words = wb.get_words_by_tag("greeting")
 
 # Get words added on a specific date
 from datetime import date
```

### Comparing `tebbytools-0.2.5/src/tebbytools/reviewlist.py` & `tebbytools-0.3.3/src/tebbytools/reviewlist.py`

 * *Files identical despite different names*

