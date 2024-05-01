# Comparing `tmp/hermitage-0.1.6.tar.gz` & `tmp/hermitage-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.6.tar", max compression
+gzip compressed data, was "hermitage-0.1.7.tar", max compression
```

## Comparing `hermitage-0.1.6.tar` & `hermitage-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.6/README.md
--rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.6/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.6/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.6/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.6/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.6/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.6/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2852 2024-04-30 09:25:47.721200 hermitage-0.1.6/hermitage/parsers/query.py
--rw-r--r--   0        0        0      361 2024-04-30 09:27:02.184086 hermitage-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.7/README.md
+-rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.7/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.7/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.7/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.7/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.7/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.7/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-01 16:27:45.315551 hermitage-0.1.7/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      361 2024-05-01 16:28:24.399592 hermitage-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.7/PKG-INFO
```

### Comparing `hermitage-0.1.6/hermitage/definition/contracts.py` & `hermitage-0.1.7/hermitage/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.6/hermitage/mappers/invoice.py` & `hermitage-0.1.7/hermitage/mappers/invoice.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.6/hermitage/parsers/query.py` & `hermitage-0.1.7/hermitage/parsers/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def __iter__(self):
         if not self._query:
             return ()
         for field in dataclasses.fields(self._query):
             field_name = self._substitutes.get(field.name, field.name)
             value = getattr(self._query, field.name)
-            if value is None:
+            if value is zodchy.types.Empty:
                 continue
             if _search_contract(
                 _evoke_types_chain(field.type),
                 zodchy.codex.query.ClauseBit
             ):
                 if not isinstance(value, collections.abc.Sequence):
                     value = (value,)
```

### Comparing `hermitage-0.1.6/PKG-INFO` & `hermitage-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermitage
-Version: 0.1.6
+Version: 0.1.7
 Summary: Universal storage access framework
 Home-page: https://github.com/smairon/hermitage
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

