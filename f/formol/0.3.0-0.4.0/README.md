# Comparing `tmp/formol-0.3.0.tar.gz` & `tmp/formol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formol-0.3.0.tar", max compression
+gzip compressed data, was "formol-0.4.0.tar", max compression
```

## Comparing `formol-0.3.0.tar` & `formol-0.4.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0    37433 2024-05-01 18:50:43.164200 formol-0.3.0/formol.py
--rw-r--r--   0        0        0     1802 2024-05-01 18:55:17.977108 formol-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    37451 2024-05-01 19:03:46.652987 formol-0.4.0/formol.py
+-rw-r--r--   0        0        0     1802 2024-05-01 19:04:32.156250 formol-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.4.0/PKG-INFO
```

### Comparing `formol-0.3.0/formol.py` & `formol-0.4.0/formol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1193,15 +1193,15 @@
     # format contents of comment
     new_content_lines = _Formatter(_Parser(content_lines).elems,
                                    max_line_len - 3).lines
 
     # create and return final comment
     new_comment_lines = ['/*']
     indent_str = _indent_str(start_col)
-    new_comment_lines += list(map(lambda rline: f'{indent_str} * {rline}',
+    new_comment_lines += list(map(lambda rline: f'{indent_str} * {rline}'.rstrip(),
                                   new_content_lines))
     new_comment_lines.append(f'{indent_str} */')
     return '\n'.join(new_comment_lines)
 
 
 # Returns the beautified version of the prefixed block comment text
 # `text` to fit on `max_line_len` columns.
@@ -1250,10 +1250,10 @@
     # format contents of comment
     new_content_lines = _Formatter(_Parser(content_lines).elems,
                                    max_line_len - len(prefix)).lines
 
     # create and return final comment
     new_comment_lines: List[str] = []
     indent_str = _indent_str(start_col)
-    new_comment_lines += list(map(lambda rline: f'{indent_str}{prefix}{rline}',
+    new_comment_lines += list(map(lambda rline: f'{indent_str}{prefix}{rline}'.rstrip(),
                                   new_content_lines))
     return '\n'.join(new_comment_lines)
```

### Comparing `formol-0.3.0/pyproject.toml` & `formol-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'formol'
-version = '0.3.0'
+version = '0.4.0'
 description = 'Plain text beautifier'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 repository = 'https://github.com/eepp/formol/'
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'License :: OSI Approved :: MIT License',
```

### Comparing `formol-0.3.0/PKG-INFO` & `formol-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formol
-Version: 0.3.0
+Version: 0.4.0
 Summary: Plain text beautifier
 Home-page: https://github.com/eepp/formol/
 License: MIT
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

