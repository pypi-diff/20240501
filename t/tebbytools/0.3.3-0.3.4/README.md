# Comparing `tmp/tebbytools-0.3.3.tar.gz` & `tmp/tebbytools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tebbytools-0.3.3.tar", last modified: Wed May  1 12:46:57 2024, max compression
+gzip compressed data, was "tebbytools-0.3.4.tar", last modified: Wed May  1 16:08:24 2024, max compression
```

## Comparing `tebbytools-0.3.3.tar` & `tebbytools-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.032612 tebbytools-0.3.3/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 12:46:57.032436 tebbytools-0.3.3/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2074 2024-05-01 12:39:54.000000 tebbytools-0.3.3/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-05-01 12:46:57.032660 tebbytools-0.3.3/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-05-01 12:46:26.000000 tebbytools-0.3.3/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.030480 tebbytools-0.3.3/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.031520 tebbytools-0.3.3/src/tebbytools/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-05-01 12:39:54.000000 tebbytools-0.3.3/src/tebbytools/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.3/src/tebbytools/reviewlist.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     5366 2024-05-01 12:39:54.000000 tebbytools-0.3.3/src/tebbytools/wordbank.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 12:46:57.032254 tebbytools-0.3.3/src/tebbytools.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      253 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-05-01 12:46:57.000000 tebbytools-0.3.3/src/tebbytools.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 16:08:24.819679 tebbytools-0.3.4/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 16:08:24.819518 tebbytools-0.3.4/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2053 2024-05-01 16:06:30.000000 tebbytools-0.3.4/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-05-01 16:08:24.819714 tebbytools-0.3.4/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-05-01 16:07:43.000000 tebbytools-0.3.4/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 16:08:24.817815 tebbytools-0.3.4/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 16:08:24.818734 tebbytools-0.3.4/src/tebbytools/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-05-01 12:39:54.000000 tebbytools-0.3.4/src/tebbytools/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.4/src/tebbytools/reviewlist.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     4931 2024-05-01 16:06:30.000000 tebbytools-0.3.4/src/tebbytools/wordbank.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-05-01 16:08:24.819372 tebbytools-0.3.4/src/tebbytools.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-05-01 16:08:24.000000 tebbytools-0.3.4/src/tebbytools.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      253 2024-05-01 16:08:24.000000 tebbytools-0.3.4/src/tebbytools.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-05-01 16:08:24.000000 tebbytools-0.3.4/src/tebbytools.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-05-01 16:08:24.000000 tebbytools-0.3.4/src/tebbytools.egg-info/top_level.txt
```

### Comparing `tebbytools-0.3.3/README.md` & `tebbytools-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,21 +30,20 @@
 
 # Get all words in the bank
 words = wb.get_all_words()
 
 # Get all unique words in the bank
 unique_words = wb.get_all_unique_words()
 
-# Get words added in the past n days
-recent_words = wb.get_words_from_past_n_days(7)
-
 # Get words added today
-# Same as get_words_from_past_n_days(0)
 todays_words = wb.get_todays_words()
 
+# Get today's words that were added for the first time
+todays_new_words = wb.get_todays_new_words(self)
+
 # Get words by a specific tag
 greeting_words = wb.get_words_by_tag("greeting")
 
 # Get words added on a specific date
 from datetime import date
 words_on_date = wb.get_words_by_date(date(2021, 12, 31))
```

### Comparing `tebbytools-0.3.3/src/tebbytools/reviewlist.py` & `tebbytools-0.3.4/src/tebbytools/reviewlist.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.3.3/src/tebbytools/wordbank.py` & `tebbytools-0.3.4/src/tebbytools/wordbank.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,16 +64,17 @@
         conn.commit()
         conn.close()
 
     def add_word(self, word, date_time=datetime.now(), tags=None):
         """
         Add a new word to the wordbank
         Args:
-            word: the word to add
-            tags: a list of string tags
+            word (string): the word to add
+            date_time (datetime.datetime): the date and time the word was added
+            tags (string[]): a list of string tags
         """
         tags_str = json.dumps(tags) if tags else None
         date_time_str = date_time.strftime(DATETIME_FORMAT)
         conn = self.create_connection()
         c = conn.cursor()
         # Insert the word into the database
         c.execute(
@@ -104,36 +105,19 @@
         conn = self.create_connection()
         c = conn.cursor()
         c.execute("SELECT DISTINCT word FROM wordbank")
         words = [row[0] for row in c.fetchall()]
         conn.close()
         return words
 
-    def get_words_from_past_n_days(self, n=0):
-        """
-        Get a list of all the words added in the past n days, where n=0 will return the words added today
-        """
-        conn = self.create_connection()
-        c = conn.cursor()
-        c.execute(
-            """
-            SELECT word FROM wordbank
-            WHERE datetime >= ?
-            """,
-            ((datetime.now() - timedelta(days=n)).strftime(DATETIME_FORMAT),),
-        )
-        words = [row[0] for row in c.fetchall()]
-        conn.close()
-        return words
-
     def get_todays_words(self):
         """
         Get the list of words added today
         """
-        return self.get_words_from_past_n_days(0)
+        return self.get_words_by_date(datetime.now().date())
 
     def get_todays_new_words(self):
         """
         Get a list of the words added today that only appear once in the bank
         """
         todays_words = self.get_todays_words()
         new_words = [word for word in todays_words if self.occurences(word) == 1]
```

