# Comparing `tmp/cim_11_certic-0.5.0.tar.gz` & `tmp/cim_11_certic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim_11_certic-0.5.0.tar", max compression
+gzip compressed data, was "cim_11_certic-0.6.0.tar", max compression
```

## Comparing `cim_11_certic-0.5.0.tar` & `cim_11_certic-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.5.0/README.md
--rw-r--r--   0        0        0     8473 2024-04-30 09:45:07.872728 cim_11_certic-0.5.0/cim_11/__init__.py
--rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.5.0/cim_11/cim-11.sqlite3
--rw-r--r--   0        0        0      534 2024-04-30 09:46:23.303604 cim_11_certic-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3448 2023-12-18 17:23:25.585872 cim_11_certic-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1823 2024-03-12 12:11:37.118412 cim_11_certic-0.6.0/README.md
+-rw-r--r--   0        0        0     8931 2024-05-01 10:05:28.579052 cim_11_certic-0.6.0/cim_11/__init__.py
+-rw-r--r--   0        0        0 11919360 2024-03-12 10:47:06.046802 cim_11_certic-0.6.0/cim_11/cim-11.sqlite3
+-rw-r--r--   0        0        0   403379 2024-05-01 09:48:10.188567 cim_11_certic-0.6.0/cim_11/stopwords.py
+-rw-r--r--   0        0        0      534 2024-05-01 09:54:19.725552 cim_11_certic-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 cim_11_certic-0.6.0/PKG-INFO
```

### Comparing `cim_11_certic-0.5.0/LICENSE.txt` & `cim_11_certic-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.5.0/README.md` & `cim_11_certic-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.5.0/cim_11/__init__.py` & `cim_11_certic-0.6.0/cim_11/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sqlite3
 import os
 from typing import List, Union, Iterator
 from contextlib import contextmanager
+from .stopwords import stopwords
 
 _DB_FILE = "{}/cim-11.sqlite3".format(os.path.dirname(__file__))
 
 
 @contextmanager
 def _db_cursor():
     db = sqlite3.connect(f"file:{_DB_FILE}?mode=ro", uri=True)
@@ -95,30 +96,38 @@
             q,
             (f"%{terms.strip()}%",),
         ):
             items.append(Concept(row[0], row[1], row[2], row[3], row[4]))
     return items
 
 
-def label_search(terms: str, lang="fr", search_type: str = "AND") -> List[Concept]:
+def label_search(
+    terms: str, lang="fr", search_type: str = "AND", filter_stopwords=False
+) -> List[Concept]:
     """
     Search for concepts based on given terms.
 
     :param terms: The terms to search for.
+    :param lang: iso-639-1 language. Can be "fr" or "en". Defaults to "fr".
+    :param search_type: Can be "AND" or "OR". Defaults to "AND".
+    :param filter_stopwords: Filter selected language stopwords. Defaults to False.
     :return: A list of concepts matching the search terms.
     """
     if search_type == "OR":
         search_type = " OR "
     else:
         search_type = " "
 
     def fts_escape(user_input: str) -> str:
         wrds = []
-        for wrd in user_input.split(" "):
-            wrds.append('"' + wrd.replace('"', '""') + '"')
+        for wrd in user_input.replace("'", " ").replace("’", " ").split(" "):
+            if not filter_stopwords or (
+                filter_stopwords and wrd not in stopwords.get(lang, [])
+            ):
+                wrds.append('"' + wrd.replace('"', '""') + '"')
         return search_type.join(wrds)
 
     dedup = []
     terms = fts_escape(terms)
     items = []
     q = "SELECT idc_id, icode, label, parent_idc_id, label_en from cim11 where label match ? and icode is not null order by icode"
     if lang == "en":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cim_11_certic-0.5.0/cim_11/cim-11.sqlite3` & `cim_11_certic-0.6.0/cim_11/cim-11.sqlite3`

 * *Files identical despite different names*

### Comparing `cim_11_certic-0.5.0/pyproject.toml` & `cim_11_certic-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cim-11-CERTIC"
-version = "0.5.0"
+version = "0.6.0"
 description = "Classification Internationale des Maladies Onzième Révision en français. Données OMS."
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>", "Arnaud Daret <arnaud.daret@unicaen.fr>"]
 readme = "README.md"
 license = "LICENSE.txt"
 packages = [{include = "cim_11"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cim_11_certic-0.5.0/PKG-INFO` & `cim_11_certic-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-11-CERTIC
-Version: 0.5.0
+Version: 0.6.0
 Summary: Classification Internationale des Maladies Onzième Révision en français. Données OMS.
 License: LICENSE.txt
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

