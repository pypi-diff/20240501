# Comparing `tmp/pylliterate-0.0.3.tar.gz` & `tmp/pylliterate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylliterate-0.0.3.tar", max compression
+gzip compressed data, was "pylliterate-0.0.4.tar", max compression
```

## Comparing `pylliterate-0.0.3.tar` & `pylliterate-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2024-04-24 01:28:01.016185 pylliterate-0.0.3/LICENSE
--rw-r--r--   0        0        0    10157 2024-04-25 20:23:18.036017 pylliterate-0.0.3/pylliterate/__init__.py
--rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.3/pylliterate/__main__.py
--rw-r--r--   0        0        0     3817 2024-04-25 20:23:18.036017 pylliterate-0.0.3/pylliterate/cli.py
--rw-r--r--   0        0        0     3145 2024-04-25 20:23:18.038504 pylliterate-0.0.3/pylliterate/config.py
--rw-r--r--   0        0        0    14790 2024-04-25 20:23:18.038504 pylliterate-0.0.3/pylliterate/core.py
--rw-r--r--   0        0        0      665 2024-04-30 05:05:03.220100 pylliterate-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.3/Readme.md
--rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pylliterate-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-01 05:46:13.332526 pylliterate-0.0.4/LICENSE
+-rw-r--r--   0        0        0    10157 2024-04-25 20:23:18.036017 pylliterate-0.0.4/pylliterate/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.4/pylliterate/__main__.py
+-rw-r--r--   0        0        0     3817 2024-04-25 20:23:18.036017 pylliterate-0.0.4/pylliterate/cli.py
+-rw-r--r--   0        0        0     3145 2024-04-25 20:23:18.038504 pylliterate-0.0.4/pylliterate/config.py
+-rw-r--r--   0        0        0    14790 2024-04-25 20:23:18.038504 pylliterate-0.0.4/pylliterate/core.py
+-rw-r--r--   0        0        0      665 2024-05-01 05:46:13.333422 pylliterate-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.4/Readme.md
+-rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pylliterate-0.0.4/PKG-INFO
```

### Comparing `pylliterate-0.0.3/LICENSE` & `pylliterate-0.0.4/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Alejandro Piad Morffis
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Jesús Enrique Fuentes
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pylliterate-0.0.3/pylliterate/__init__.py` & `pylliterate-0.0.4/pylliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.3/pylliterate/cli.py` & `pylliterate-0.0.4/pylliterate/cli.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.3/pylliterate/config.py` & `pylliterate-0.0.4/pylliterate/config.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.3/pylliterate/core.py` & `pylliterate-0.0.4/pylliterate/core.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.3/pyproject.toml` & `pylliterate-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylliterate"
-version = "0.0.3"
+version = "0.0.4"
 description = "Unobtrusive literate programming experience for Python pragmatists"
 authors = ["Jesús Enrique Fuentes <jesusefg12@gmail.com>", "Alejandro Piad <alepiad@gmail.com>"]
 license = "MIT"
 readme = "Readme.md"
 
 [tool.poetry.scripts]
 pylliterate = "pylliterate.cli:app"
```

### Comparing `pylliterate-0.0.3/Readme.md` & `pylliterate-0.0.4/Readme.md`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.3/PKG-INFO` & `pylliterate-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylliterate
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unobtrusive literate programming experience for Python pragmatists
 License: MIT
 Author: Jesús Enrique Fuentes
 Author-email: jesusefg12@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

