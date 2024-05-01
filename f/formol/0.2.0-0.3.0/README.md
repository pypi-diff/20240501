# Comparing `tmp/formol-0.2.0.tar.gz` & `tmp/formol-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formol-0.2.0.tar", max compression
+gzip compressed data, was "formol-0.3.0.tar", max compression
```

## Comparing `formol-0.2.0.tar` & `formol-0.3.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0    37430 2024-05-01 18:25:45.205126 formol-0.2.0/formol.py
--rw-r--r--   0        0        0     1802 2024-05-01 18:28:46.051131 formol-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    37433 2024-05-01 18:50:43.164200 formol-0.3.0/formol.py
+-rw-r--r--   0        0        0     1802 2024-05-01 18:55:17.977108 formol-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.3.0/PKG-INFO
```

### Comparing `formol-0.2.0/formol.py` & `formol-0.3.0/formol.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,15 +622,15 @@
         # create item from unindented content lines
         return _SimpleListItem(_Parser(self._unindent_lines(lines, prefix_len)).elems)
 
     # Tries to parse an ordered list.
     def _try_parse_ol(self):
         return self._try_parse_simple_list(_Ol, self._try_parse_ol_item)
 
-    _literal_pat = re.compile(r'`[^`]*`')
+    _literal_pat = re.compile(r'`[^`]*`\S*')
     _word_pat = re.compile(r'(.+?)(?=[` ]|$)')
 
     # Converts a paragraph text to a paragraph element containing
     # individual words.
     @staticmethod
     def _p_elem_from_text(text: str):
         elems: List[str] = []
```

### Comparing `formol-0.2.0/pyproject.toml` & `formol-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'formol'
-version = '0.2.0'
+version = '0.3.0'
 description = 'Plain text beautifier'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 repository = 'https://github.com/eepp/formol/'
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'License :: OSI Approved :: MIT License',
```

### Comparing `formol-0.2.0/PKG-INFO` & `formol-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formol
-Version: 0.2.0
+Version: 0.3.0
 Summary: Plain text beautifier
 Home-page: https://github.com/eepp/formol/
 License: MIT
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

