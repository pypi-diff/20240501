# Comparing `tmp/zyx-0.0.10.tar.gz` & `tmp/zyx-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.10.tar", last modified: Wed May  1 02:19:43 2024, max compression
+gzip compressed data, was "zyx-0.0.11.tar", last modified: Wed May  1 02:25:53 2024, max compression
```

## Comparing `zyx-0.0.10.tar` & `zyx-0.0.11.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.368854 zyx-0.0.10/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:19:43.368854 zyx-0.0.10/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)       58 2024-04-30 22:57:31.000000 zyx-0.0.10/README.md
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 02:19:43.368854 zyx-0.0.10/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)      918 2024-05-01 01:52:47.000000 zyx-0.0.10/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.363854 zyx-0.0.10/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.364854 zyx-0.0.10/src/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.10/src/zyx/__cli__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      145 2024-05-01 02:17:07.000000 zyx-0.0.10/src/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.366854 zyx-0.0.10/src/zyx/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.10/src/zyx/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.10/src/zyx/core/chat.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.10/src/zyx/core/input.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.10/src/zyx/core/lightning.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.10/src/zyx/core/loaders.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2173 2024-05-01 01:31:23.000000 zyx-0.0.10/src/zyx/core/print.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.10/src/zyx/core/validate_path.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.10/src/zyx/core/validate_type.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.366854 zyx-0.0.10/src/zyx/functions/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:12:32.000000 zyx-0.0.10/src/zyx/functions/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.10/src/zyx/functions/create_id.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.10/src/zyx/functions/generate_name.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.10/src/zyx/functions/get_system_info.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx/jupyter/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.10/src/zyx/jupyter/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.10/src/zyx/jupyter/tailwind.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx/text/
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.10/src/zyx/text/__chunker__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.10/src/zyx/text/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.10/src/zyx/text/__read_doc__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:19:43.367854 zyx-0.0.10/src/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       96 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 02:19:43.000000 zyx-0.0.10/src/zyx.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.733267 zyx-0.0.11/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:25:53.732267 zyx-0.0.11/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       58 2024-04-30 22:57:31.000000 zyx-0.0.11/README.md
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 02:25:53.733267 zyx-0.0.11/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      918 2024-05-01 02:24:59.000000 zyx-0.0.11/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.727267 zyx-0.0.11/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.728267 zyx-0.0.11/src/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.11/src/zyx/__cli__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      145 2024-05-01 02:17:07.000000 zyx-0.0.11/src/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.730267 zyx-0.0.11/src/zyx/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.11/src/zyx/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.11/src/zyx/core/chat.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.11/src/zyx/core/input.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.11/src/zyx/core/lightning.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.11/src/zyx/core/loaders.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2157 2024-05-01 02:25:43.000000 zyx-0.0.11/src/zyx/core/print.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.11/src/zyx/core/validate_path.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.11/src/zyx/core/validate_type.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.731267 zyx-0.0.11/src/zyx/functions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:12:32.000000 zyx-0.0.11/src/zyx/functions/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.11/src/zyx/functions/create_id.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.11/src/zyx/functions/generate_name.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.11/src/zyx/functions/get_system_info.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx/jupyter/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.11/src/zyx/jupyter/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.11/src/zyx/jupyter/tailwind.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx/text/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.11/src/zyx/text/__chunker__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.11/src/zyx/text/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.11/src/zyx/text/__read_doc__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       96 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/top_level.txt
```

### Comparing `zyx-0.0.10/setup.py` & `zyx-0.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     author = "Hammad Saeed",
     author_email="hammad@supportvectors.com",
 
     name = 'zyx',
-    version = '0.0.10',
+    version = '0.0.11',
     packages = find_packages(where='src'),
     package_dir = {'': 'src'},
 
     python_requires = '>=3.8',
 
     install_requires = [
         # General Utility Libraries
```

### Comparing `zyx-0.0.10/src/zyx/core/chat.py` & `zyx-0.0.11/src/zyx/core/chat.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/core/input.py` & `zyx-0.0.11/src/zyx/core/input.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/core/lightning.py` & `zyx-0.0.11/src/zyx/core/lightning.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/core/loaders.py` & `zyx-0.0.11/src/zyx/core/loaders.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/core/print.py` & `zyx-0.0.11/src/zyx/core/print.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rich import box
 from rich.columns import Columns
 from typing import Optional, Literal, Any
 
 # Define the Literal type for box styles
 BoxStyle = Optional[Literal['SQUARE', 'ROUNDED', 'SIMPLE', 'DOUBLE', 'MINIMAL', 'HEAVY', 'ASCII']]
 
-def _print_(*values: Any, _style_: Optional[str] = "white", _box_style_: BoxStyle = None, sep: str = ' ', end: str = '\n'):
+def _print_(*values: Any, style: Optional[str] = "white", box_style: BoxStyle = None, sep: str = ' ', end: str = '\n'):
     """
     Prints a message with the specified style and optionally in a box with the chosen style.
 
     Example:
         ```python
         from zyx import print
 
@@ -35,21 +35,21 @@
 
     if not values:
         values = ("No message provided.",)
 
     message = sep.join(str(value) for value in values)
 
     if isinstance(values, list):
-        panels = [Panel(item, expand=False, box=getattr(box, _box_style_) if _box_style_ else None) for item in values]
+        panels = [Panel(item, expand=False, box=getattr(box, box_style) if box_style else None) for item in values]
         columns = Columns(panels)
-        console.print(columns, style=_style_, end=end)
+        console.print(columns, style=style, end=end)
     else:
-        if _box_style_:
-            message = Panel(message, expand=False, box=getattr(box, _box_style_))
-        console.print(message, style=_style_, end=end)
+        if box_style:
+            message = Panel(message, expand=False, box=getattr(box, box_style))
+        console.print(message, style=style, end=end)
 
     return console
 
 if __name__ == "__main__":
     _print_("[bold red]This is a message with a box![/bold red]", _box_style_="ROUNDED")
     _print_("This is a message without a box.")
     _print_("Multiple", "values", "printed", "with", "a", "separator", sep="-")
```

### Comparing `zyx-0.0.10/src/zyx/core/validate_path.py` & `zyx-0.0.11/src/zyx/core/validate_path.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/core/validate_type.py` & `zyx-0.0.11/src/zyx/core/validate_type.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/functions/__init__.py` & `zyx-0.0.11/src/zyx/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/functions/create_id.py` & `zyx-0.0.11/src/zyx/functions/create_id.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/functions/generate_name.py` & `zyx-0.0.11/src/zyx/functions/generate_name.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/functions/get_system_info.py` & `zyx-0.0.11/src/zyx/functions/get_system_info.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/jupyter/tailwind.py` & `zyx-0.0.11/src/zyx/jupyter/tailwind.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/text/__chunker__.py` & `zyx-0.0.11/src/zyx/text/__chunker__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx/text/__read_doc__.py` & `zyx-0.0.11/src/zyx/text/__read_doc__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.10/src/zyx.egg-info/SOURCES.txt` & `zyx-0.0.11/src/zyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

