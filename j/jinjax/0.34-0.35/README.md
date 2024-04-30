# Comparing `tmp/jinjax-0.34.tar.gz` & `tmp/jinjax-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjax-0.34.tar", max compression
+gzip compressed data, was "jinjax-0.35.tar", max compression
```

## Comparing `jinjax-0.34.tar` & `jinjax-0.35.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      497 2024-04-22 18:48:27.025337 jinjax-0.34/README.md
--rw-r--r--   0        0        0     3839 2024-04-22 18:48:27.033337 jinjax-0.34/pyproject.toml
--rw-r--r--   0        0        0      189 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/__init__.py
--rw-r--r--   0        0        0    13732 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/catalog.py
--rw-r--r--   0        0        0     6416 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/component.py
--rw-r--r--   0        0        0      409 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/exceptions.py
--rw-r--r--   0        0        0     5250 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/html_attrs.py
--rw-r--r--   0        0        0     4599 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/jinjax.py
--rw-r--r--   0        0        0     1304 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/middleware.py
--rw-r--r--   0        0        0        0 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/py.typed
--rw-r--r--   0        0        0       54 2024-04-22 18:48:27.033337 jinjax-0.34/src/jinjax/utils.py
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.34/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-04-30 22:45:12.583815 jinjax-0.35/README.md
+-rw-r--r--   0        0        0     3839 2024-04-30 22:45:12.591815 jinjax-0.35/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/__init__.py
+-rw-r--r--   0        0        0    13762 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/catalog.py
+-rw-r--r--   0        0        0     6416 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/component.py
+-rw-r--r--   0        0        0      409 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/exceptions.py
+-rw-r--r--   0        0        0     5289 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/html_attrs.py
+-rw-r--r--   0        0        0     4657 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/jinjax.py
+-rw-r--r--   0        0        0     1304 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/py.typed
+-rw-r--r--   0        0        0       54 2024-04-30 22:45:12.591815 jinjax-0.35/src/jinjax/utils.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.35/PKG-INFO
```

### Comparing `jinjax-0.34/pyproject.toml` & `jinjax-0.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jinjax"
-version = "0.34"
+version = "0.35"
 description = "Replace your HTML templates with Python server-Side components"
 authors = ["Juan-Pablo Scaletti <juanpablo@jpscaletti.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://jinjax.scaletti.dev/"
 repository = "https://github.com/jpsca/jinjax"
 documentation = "https://jinjax.scaletti.dev/guides/"
```

### Comparing `jinjax-0.34/src/jinjax/catalog.py` & `jinjax-0.35/src/jinjax/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,17 @@
             props[PROP_ATTRS] = HTMLAttrs(extra)
         except Exception as exc:
             raise InvalidArgument(
                 f"The arguments of the component <{component.name}>"
                 f"were parsed incorrectly as:\n {str(kw)}"
             ) from exc
 
-        props[PROP_CONTENT] = content if content or not caller else caller().strip()
+        props[PROP_CONTENT] = Markup(
+            content if content or not caller else caller().strip()
+        )
         return component.render(**props)
 
     def get_middleware(
         self,
         application: t.Callable,
         allowed_ext: "t.Iterable[str] | None" = ALLOWED_EXTENSIONS,
         **kwargs,
```

### Comparing `jinjax-0.34/src/jinjax/component.py` & `jinjax-0.35/src/jinjax/component.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.34/src/jinjax/html_attrs.py` & `jinjax-0.35/src/jinjax/html_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from collections import UserString
 from functools import cached_property
 from typing import Any
 
+from markupsafe import Markup
+
 
 CLASS_KEY = "class"
 CLASS_ALT_KEY = "classes"
 CLASS_KEYS = (CLASS_KEY, CLASS_ALT_KEY)
 
 
 def split(ssl: str) -> list[str]:
@@ -174,8 +176,8 @@
 
         html_attrs = [
             f"{name}={quote(str(value))}"
             for name, value in attributes.items()
         ]
         html_attrs.extend(properties)
 
-        return " ".join(html_attrs)
+        return Markup(" ".join(html_attrs))
```

### Comparing `jinjax-0.34/src/jinjax/jinjax.py` & `jinjax-0.35/src/jinjax/jinjax.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import typing as t
 from uuid import uuid4
 
 from jinja2.exceptions import TemplateSyntaxError
 from jinja2.ext import Extension
+from jinja2.filters import do_forceescape
 
 from .utils import logger
 
 
 RENDER_CMD = "catalog.irender"
 BLOCK_CALL = '{% call [CMD]("[TAG]"[ATTRS]) -%}[CONTENT]{%- endcall %}'
 BLOCK_CALL = BLOCK_CALL.replace("[CMD]", RENDER_CMD)
@@ -62,15 +63,15 @@
             repl = self._replace_raw_block(match)
             source = f"{source[:start]}{repl}{source[end:]}"
 
         return source
 
     def _replace_raw_block(self, match: re.Match) -> str:
         uid = f"--RAW-{uuid4().hex}--"
-        self.__raw_blocks[uid] = match.group(0)
+        self.__raw_blocks[uid] = do_forceescape(match.group(0))
         return uid
 
     def _restore_raw_blocks(self, source: str) -> str:
         for uid, code in self.__raw_blocks.items():
             source = source.replace(uid, code)
         return source
```

### Comparing `jinjax-0.34/src/jinjax/middleware.py` & `jinjax-0.35/src/jinjax/middleware.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.34/PKG-INFO` & `jinjax-0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjax
-Version: 0.34
+Version: 0.35
 Summary: Replace your HTML templates with Python server-Side components
 Home-page: https://jinjax.scaletti.dev/
 License: MIT
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

