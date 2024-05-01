# Comparing `tmp/sinli-1.1.5.tar.gz` & `tmp/sinli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.1.5.tar", last modified: Wed Apr 10 12:20:30 2024, max compression
+gzip compressed data, was "sinli-1.2.0.tar", last modified: Wed May  1 13:40:29 2024, max compression
```

## Comparing `sinli-1.1.5.tar` & `sinli-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2024-04-10 12:04:33.000000 sinli-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46399 2024-04-10 12:20:30.565737 sinli-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6102 2024-04-10 12:04:33.000000 sinli-1.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-10 12:20:20.000000 sinli-1.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:20:30.565737 sinli-1.1.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.561737 sinli-1.1.5/src/sinli/doctype/devolu/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/devolu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/devolu/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     5491 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     7418 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/line.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-04-10 12:04:33.000000 sinli-1.1.5/src/sinli/subject.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46399 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 12:20:30.000000 sinli-1.1.5/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:20:30.565737 sinli-1.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-10 12:04:33.000000 sinli-1.1.5/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2024-05-01 13:40:18.000000 sinli-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46399 2024-05-01 13:40:29.183218 sinli-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6102 2024-05-01 13:40:18.000000 sinli-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-01 13:40:18.000000 sinli-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 13:40:29.187218 sinli-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.179218 sinli-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5523 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/devolu/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/devolu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/devolu/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5490 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/subject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46399 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-01 13:40:18.000000 sinli-1.2.0/tests/test_document.py
```

### Comparing `sinli-1.1.5/LICENSE` & `sinli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/PKG-INFO` & `sinli-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.5
+Version: 1.2.0
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.5/README.md` & `sinli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/pyproject.toml` & `sinli-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.1.5"
+version = "1.2.0"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.1.5/src/sinli/doctype/__init__.py` & `sinli-1.2.0/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/devolu/v2.py` & `sinli-1.2.0/src/sinli/doctype/devolu/v2.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/envio/v8.py` & `sinli-1.2.0/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/factul/v1.py` & `sinli-1.2.0/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/libros/v8.py` & `sinli-1.2.0/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/libros/v9.py` & `sinli-1.2.0/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/mensaj/v1.py` & `sinli-1.2.0/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/doctype/pedido/v7.py` & `sinli-1.2.0/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli/document.py` & `sinli-1.2.0/src/sinli/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             doc = consume_line(line, doc)
         return doc
 
     @classmethod
     def from_str(cls, s: str) -> Self:
         doc = cls()
         doctype_s = ""
-        cls.consume_lines(s.split_lines(), doc)
+        cls.consume_lines(s.splitlines(), doc)
         return doc
 
     @classmethod
     def from_filename(cls, filename: str) -> Self:
         """
         El juego de caracteres recomendado es el 850 OEM – Multilingual Latín I // (DOS Latin 1 = CP 850)
         https://docs.python.org/3/library/codecs.html#module-codecs
```

### Comparing `sinli-1.1.5/src/sinli/line.py` & `sinli-1.2.0/src/sinli/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .common.encoded_values import SinliCode as c, BasicType as t
+from .common.encoded_values import SinliCode as c, BasicType as t, EncodedField
 from enum import Enum
 from typing_extensions import Self
 from dataclasses import dataclass
 from pycountry import countries, languages, currencies
 from datetime import date
-import datetime
+from datetime import datetime
 
 @dataclass(repr=False)
 class Line:
     country_class = countries.get(alpha_2="es").__class__
     lang_class = languages.get(alpha_3="cat").__class__
     currency_class = currencies.get(alpha_3="EUR").__class__
 
@@ -35,27 +35,27 @@
 
     def __str__(self) -> str:
         """Export to SINLI string"""
 
         field_l = []
         for field in self.Field:
             deflen = field.value[1]
-            val = self.encode(deflen, getattr(self, field.name))
+            f_type = field.value[2]
+            val = self.encode(deflen, getattr(self, field.name), f_type)
             vallen = len(val)
 
             if vallen < deflen:
-                f_type = field.value[2]
                 if f_type in [t.INT, t.FLOAT]:
                     padding = "0" # pad left with zeroes
                     val = "".join([padding for i in range(0, deflen-vallen)]) + val
                 else:
                     padding = " " # pad right with spaces
                     val = val + "".join([padding for i in range(0, deflen-vallen)])
             elif vallen > deflen: # truncate
-                print(f"[WARN] Unexpected: field {field.name}={val} shouldn't have been longer than {deflen} chars. Truncating to val[0:deflen]")
+                print(f"[WARN] Unexpected: field {field.name}={val} shouldn't have been longer than {deflen} chars. Truncating to {val[0:deflen]}")
                 val = val[0:deflen]
 
             field_l.append(val)
 
         return "".join(field_l)
 
     def to_csv(self) -> str:
@@ -69,15 +69,16 @@
         Returns a new dictionary with "pretified" values, that is,
         resolved from sinli codes
         """
         ld = vars(self)
         newld = {}
         for k,v in ld.items():
             newld[k] = self.pretify(k,v)
-        return self.from_dict(newld)
+        line = self.__class__()
+        return line.from_dict(newld)
 
     # Import
     def from_dict(self, fields: {}):
         for (key, value) in fields.items():
             setattr(self, key, value)
         return self
 
@@ -87,15 +88,23 @@
     @classmethod
     def from_str(cls, line_s: str) -> Self:
         line_dict = {}
         for field in cls.Field:
             start = field.value[0]
             end = start + field.value[1]
             vtype = field.value[2]
-            line_dict[field.name] = cls.decode(vtype, line_s[start:end].strip())
+            try:
+                line_dict[field.name] = cls.decode(vtype, line_s[start:end].strip())
+            except ValueError as err:
+                print(f"[ERROR] Decode error. {field} with value \"{line_s[start:end]}\" can't be converted to a float or int.", err)
+                line_dict[field.name] = 0
+            except NameError as err:
+                print(f"[ERROR] Decode error. {field} with value \"{line_s[start:end]}\" can't be converted to a language, currency or country.", err)
+                line_dict[field.name] = None
+
             print(f"[DEBUG] {field} → {line_dict[field.name]}")
         line = cls()
         return line.from_dict(line_dict)
 
     @staticmethod
     def decode(vtype, value) -> object:
         """
@@ -106,38 +115,40 @@
         if vtype == t.STR:
             return value
         elif vtype == t.INT:
             return int(value or '0')
         elif vtype == t.FLOAT:
             return float(value or '0')/100
         elif vtype == t.BOOL:
-            return True if "S" else False # "N"
+            return True if value == "S" else False # "N"
         elif vtype == t.MONTH_YEAR:
-            return datetime.datetime.strptime(value or "011970", "%m%Y").date()
+            return datetime.strptime(value or "011970", "%m%Y").date()
         elif vtype == t.DATE:
-            return datetime.datetime.strptime(value or "19700101", "%Y%m%d").date()
+            return datetime.strptime(value or "19700101", "%Y%m%d").date()
         elif vtype == t.LANG:
             return languages.get(alpha_3 = value)
         elif vtype == t.COUNTRY:
             return countries.get(alpha_2 = value)
         elif vtype == t.CURRENCY1:
             return value # TODO understand meaning of P or E values
         elif vtype == t.CURRENCY3:
             return currencies.get(alpha_3 = value)
-        elif vtype in c:
-            return value # resolve code only when printing as it's not reversible
+        elif isinstance(vtype, EncodedField):
+            return vtype.decode(value) or None
         else:
             print(f"[WARN] Unexpected case: var {value} is of type {vtype}")
             return value
 
     @classmethod
-    def encode(cls, vlen, value) -> str:
+    def encode(cls, vlen, value, ftype) -> str:
         """
         Convert an attribute from an object to a string, appendable to a sinli line
         """
+        if type(value) == datetime:
+            value = value.date()
         if type(value) == float:
             return str(int(value * 100))
         elif type(value) == date:
             if vlen == 6: return value.strftime("%m%Y")
             elif vlen == 8: return value.strftime("%Y%m%d")
             else: raise(f"BUG! unexpected situation to SINLI-encode {value} to a length of {vlen} bytes")
         elif type(value) == bool:
@@ -145,31 +156,34 @@
         elif type(value) == cls.country_class:
             return value.alpha_2
         elif type(value) == cls.lang_class:
             return value.alpha_3
         elif type(value) == cls.currency_class:
             if vlen == 3:  return value.alpha_3
             #elif vlen == 1: return value # TODO understand P and E values
+        elif isinstance(ftype, EncodedField):
+            if value == None:
+                return " "
+            return value[0]
         else: # string, integer
             return str(value)
 
     @classmethod
     def pretify(cls, k, v) -> str:
         """
         pretify field with name k and value v.
         it resolves the sinli codes to their description value,
         sinli codes have the same key as line field keys
         """
         if type(k) == cls.currency_class:
             return v.name
         try:
-            return str(c.get(k).value[0].get(v) or c.get(k).value[0].get("??"))
+            return v[1] or "Unknown"
         except:
             return str(v)
-        return str(v)
 
 class LongIdentificationLine(Line):
     def __post_init__(self):
         super().__post_init__()
         self.TYPE = "I"
         self.FORMAT = "N"
```

### Comparing `sinli-1.1.5/src/sinli/subject.py` & `sinli-1.2.0/src/sinli/subject.py`

 * *Files identical despite different names*

### Comparing `sinli-1.1.5/src/sinli.egg-info/PKG-INFO` & `sinli-1.2.0/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.1.5
+Version: 1.2.0
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sinli-1.1.5/src/sinli.egg-info/SOURCES.txt` & `sinli-1.2.0/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

