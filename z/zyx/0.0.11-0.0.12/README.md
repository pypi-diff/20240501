# Comparing `tmp/zyx-0.0.11.tar.gz` & `tmp/zyx-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.11.tar", last modified: Wed May  1 02:25:53 2024, max compression
+gzip compressed data, was "zyx-0.0.12.tar", last modified: Wed May  1 03:01:29 2024, max compression
```

## Comparing `zyx-0.0.11.tar` & `zyx-0.0.12.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.733267 zyx-0.0.11/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:25:53.732267 zyx-0.0.11/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)       58 2024-04-30 22:57:31.000000 zyx-0.0.11/README.md
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 02:25:53.733267 zyx-0.0.11/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)      918 2024-05-01 02:24:59.000000 zyx-0.0.11/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.727267 zyx-0.0.11/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.728267 zyx-0.0.11/src/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.11/src/zyx/__cli__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      145 2024-05-01 02:17:07.000000 zyx-0.0.11/src/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.730267 zyx-0.0.11/src/zyx/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.11/src/zyx/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.11/src/zyx/core/chat.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.11/src/zyx/core/input.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.11/src/zyx/core/lightning.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.11/src/zyx/core/loaders.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2157 2024-05-01 02:25:43.000000 zyx-0.0.11/src/zyx/core/print.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.11/src/zyx/core/validate_path.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.11/src/zyx/core/validate_type.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.731267 zyx-0.0.11/src/zyx/functions/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:12:32.000000 zyx-0.0.11/src/zyx/functions/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.11/src/zyx/functions/create_id.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.11/src/zyx/functions/generate_name.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.11/src/zyx/functions/get_system_info.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx/jupyter/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.11/src/zyx/jupyter/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.11/src/zyx/jupyter/tailwind.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx/text/
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.11/src/zyx/text/__chunker__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.11/src/zyx/text/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.11/src/zyx/text/__read_doc__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:25:53.732267 zyx-0.0.11/src/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      408 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       96 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 02:25:53.000000 zyx-0.0.11/src/zyx.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.583841 zyx-0.0.12/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-01 03:01:29.583841 zyx-0.0.12/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1275 2024-05-01 02:37:02.000000 zyx-0.0.12/README.md
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-01 03:01:29.583841 zyx-0.0.12/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1122 2024-05-01 03:01:12.000000 zyx-0.0.12/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.578841 zyx-0.0.12/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.578841 zyx-0.0.12/src/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 01:28:40.000000 zyx-0.0.12/src/zyx/__cli__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      194 2024-05-01 02:59:31.000000 zyx-0.0.12/src/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.580841 zyx-0.0.12/src/zyx/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 02:11:43.000000 zyx-0.0.12/src/zyx/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-01 02:06:18.000000 zyx-0.0.12/src/zyx/core/chat.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 01:18:32.000000 zyx-0.0.12/src/zyx/core/input.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 01:31:09.000000 zyx-0.0.12/src/zyx/core/lightning.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 02:08:43.000000 zyx-0.0.12/src/zyx/core/loaders.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-01 02:58:35.000000 zyx-0.0.12/src/zyx/core/print.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 01:34:11.000000 zyx-0.0.12/src/zyx/core/validate_path.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 01:46:21.000000 zyx-0.0.12/src/zyx/core/validate_type.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.581841 zyx-0.0.12/src/zyx/functions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 02:59:15.000000 zyx-0.0.12/src/zyx/functions/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 01:40:07.000000 zyx-0.0.12/src/zyx/functions/create_id.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 01:35:35.000000 zyx-0.0.12/src/zyx/functions/generate_name.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 01:43:00.000000 zyx-0.0.12/src/zyx/functions/get_system_info.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.582841 zyx-0.0.12/src/zyx/jupyter/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 01:35:07.000000 zyx-0.0.12/src/zyx/jupyter/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 01:03:56.000000 zyx-0.0.12/src/zyx/jupyter/tailwind.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.582841 zyx-0.0.12/src/zyx/text/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 01:17:17.000000 zyx-0.0.12/src/zyx/text/__chunker__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 02:01:55.000000 zyx-0.0.12/src/zyx/text/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-01 01:32:22.000000 zyx-0.0.12/src/zyx/text/__read_doc__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:01:29.582841 zyx-0.0.12/src/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      716 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-01 03:01:29.000000 zyx-0.0.12/src/zyx.egg-info/top_level.txt
```

### Comparing `zyx-0.0.11/setup.py` & `zyx-0.0.12/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 from setuptools import setup, find_packages
 
 setup(
     author = "Hammad Saeed",
     author_email="hammad@supportvectors.com",
 
     name = 'zyx',
-    version = '0.0.11',
+    version = '0.0.12',
     packages = find_packages(where='src'),
     package_dir = {'': 'src'},
 
     python_requires = '>=3.8',
 
     install_requires = [
-        # General Utility Libraries
+        # Art | ASCII Art
         'art',
-        'pathlib',
-        'prompt_toolkit',
-        'pydantic',
-        'psutil',
+
+        # IPython | Interactive Python
+        'ipython',
 
         # LiteLLM | Easy LLM Completions
         'litellm',
 
         # Loguru | Logging
         'loguru',
 
         # Ollama | Language Models
         'ollama',
 
+        # Pathlib | File Paths
+        'pathlib',
+
+        # Prompt Toolkit | Interactive Prompts
+        'prompt_toolkit',
+
+        # psutil | System Utilities
+        'psutil',
+
+        # Pydantic | Data Validation
+        'pydantic',
+
         # PyMuPDF4 | PDF Parsing
         'PyMuPDF',
 
         # Rich | Pretty Printing
         'rich',
 
         # SemChunk | Semantic Chunking
```

### Comparing `zyx-0.0.11/src/zyx/core/chat.py` & `zyx-0.0.12/src/zyx/core/chat.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/core/input.py` & `zyx-0.0.12/src/zyx/core/input.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/core/lightning.py` & `zyx-0.0.12/src/zyx/core/lightning.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/core/loaders.py` & `zyx-0.0.12/src/zyx/core/loaders.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/core/print.py` & `zyx-0.0.12/src/zyx/core/print.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,54 +3,48 @@
 from rich import box
 from rich.columns import Columns
 from typing import Optional, Literal, Any
 
 # Define the Literal type for box styles
 BoxStyle = Optional[Literal['SQUARE', 'ROUNDED', 'SIMPLE', 'DOUBLE', 'MINIMAL', 'HEAVY', 'ASCII']]
 
-def _print_(*values: Any, style: Optional[str] = "white", box_style: BoxStyle = None, sep: str = ' ', end: str = '\n'):
-    """
-    Prints a message with the specified style and optionally in a box with the chosen style.
+class RichPrint:
+    def __init__(self):
+        self.console = Console()
+
+    def print(self, *values: Any, style: Optional[str] = "white", box_style: BoxStyle = None, sep: str = ' ', end: str = '\n'):
+        """
+        Prints a message with the specified style and optionally in a box with the chosen style.
 
-    Example:
+        Example:
         ```python
         from zyx import print
-
-        print("This is a message with a box!", _box_style_="ROUNDED")
+        print("This is a message with a box!", box_style="ROUNDED")
         print("This is a message without a box.")
         print("Multiple", "values", "printed", "with", "a", "separator", sep="-")
         print(1, 2, 3, 4, 5, sep=", ", end=" | ")
         ```
 
-    Args:
-        *values: The values to print.
-        _style_ (str): The style to apply to the message.
-        _box_style_ (BoxStyle): The style of the box to display the message in, or None to display without a box.
-        sep (str): The separator between the values. Default is ' '.
-        end (str): The string appended after the last value. Default is '\n'.
-
-    Returns:
-        Console: The Rich Console instance used for printing.
-    """
-    console = Console()
-
-    if not values:
-        values = ("No message provided.",)
-
-    message = sep.join(str(value) for value in values)
-
-    if isinstance(values, list):
-        panels = [Panel(item, expand=False, box=getattr(box, box_style) if box_style else None) for item in values]
-        columns = Columns(panels)
-        console.print(columns, style=style, end=end)
-    else:
-        if box_style:
-            message = Panel(message, expand=False, box=getattr(box, box_style))
-        console.print(message, style=style, end=end)
-
-    return console
-
-if __name__ == "__main__":
-    _print_("[bold red]This is a message with a box![/bold red]", _box_style_="ROUNDED")
-    _print_("This is a message without a box.")
-    _print_("Multiple", "values", "printed", "with", "a", "separator", sep="-")
-    _print_(1, 2, 3, 4, 5, sep=", ", end=" | ")
+        Args:
+            *values: The values to print.
+            style (str): The style to apply to the message.
+            box_style (BoxStyle): The style of the box to display the message in, or None to display without a box.
+            sep (str): The separator between the values. Default is ' '.
+            end (str): The string appended after the last value. Default is '\n'.
+
+        Returns:
+            None
+        """
+        if not values:
+            values = ("No message provided.",)
+        message = sep.join(str(value) for value in values)
+
+        if isinstance(values, list):
+            panels = [Panel(item, expand=False, box=getattr(box, box_style) if box_style else None) for item in values]
+            columns = Columns(panels)
+            self.console.print(columns, style=style, end=end)
+        else:
+            if box_style:
+                message = Panel(message, expand=False, box=getattr(box, box_style))
+            self.console.print(message, style=style, end=end)
+
+_print_ = RichPrint().print
```

### Comparing `zyx-0.0.11/src/zyx/core/validate_path.py` & `zyx-0.0.12/src/zyx/core/validate_path.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/core/validate_type.py` & `zyx-0.0.12/src/zyx/core/validate_type.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/functions/__init__.py` & `zyx-0.0.12/src/zyx/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/functions/create_id.py` & `zyx-0.0.12/src/zyx/functions/create_id.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/functions/generate_name.py` & `zyx-0.0.12/src/zyx/functions/generate_name.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/functions/get_system_info.py` & `zyx-0.0.12/src/zyx/functions/get_system_info.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/jupyter/tailwind.py` & `zyx-0.0.12/src/zyx/jupyter/tailwind.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/text/__chunker__.py` & `zyx-0.0.12/src/zyx/text/__chunker__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx/text/__read_doc__.py` & `zyx-0.0.12/src/zyx/text/__read_doc__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.11/src/zyx.egg-info/SOURCES.txt` & `zyx-0.0.12/src/zyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

