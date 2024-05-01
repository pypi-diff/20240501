# Comparing `tmp/riprint-1.0.4-py3-none-any.whl.zip` & `tmp/riprint-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2904 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2712 b- defN 20-Jun-09 20:15 riprint/__init__.py
--rw-r--r--  2.0 unx     1054 b- defN 20-Jun-09 20:18 riprint-1.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      282 b- defN 20-Jun-09 20:18 riprint-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Jun-09 20:18 riprint-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 20-Jun-09 20:18 riprint-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      464 b- defN 20-Jun-09 20:18 riprint-1.0.4.dist-info/RECORD
-6 files, 4612 bytes uncompressed, 2062 bytes compressed:  55.3%
+Zip file size: 2861 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2658 b- defN 24-May-01 08:56 riprint/__init__.py
+-rw-r--r--  2.0 unx     1054 b- defN 24-May-01 08:58 riprint-1.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      263 b- defN 24-May-01 08:58 riprint-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 08:58 riprint-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-01 08:58 riprint-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      464 b- defN 24-May-01 08:58 riprint-1.0.5.dist-info/RECORD
+6 files, 4539 bytes uncompressed, 2019 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: riprint/__init__.py
 Comment: 
 
-Filename: riprint-1.0.4.dist-info/LICENSE.txt
+Filename: riprint-1.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: riprint-1.0.4.dist-info/METADATA
+Filename: riprint-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: riprint-1.0.4.dist-info/WHEEL
+Filename: riprint-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: riprint-1.0.4.dist-info/top_level.txt
+Filename: riprint-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: riprint-1.0.4.dist-info/RECORD
+Filename: riprint-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## riprint/__init__.py

```diff
@@ -1,9 +1,7 @@
-# https://github.com/numpy/numpy/blob/master/numpy/core/arrayprint.py
-
 import numpy as np
 import shutil
 from termcolor import colored
 
 dict_values = type({}.values())
 dict_keys = type({}.keys())
 list_types = (list, dict_values, dict_keys)
@@ -28,15 +26,15 @@
     return colored(value, color, attrs=['bold'])
   elif isinstance(value, (int, float)):
     return colored(value, color or 'yellow')
   elif isinstance(value, str):
     if indent == 0:
       return colored(f"{value}", color)
     else:
-      return colored(f"'{value}'", color or 'green')
+      return colored(f'"{value}"', color or 'green')
   elif isinstance(value, (tuple, set, list_types)):
     open_bracket = colored('[' if isinstance(value, list_types) else '(' if isinstance(value, tuple) else '{', bracket_color)
     close_bracket = colored(']' if isinstance(value, list_types) else ')' if isinstance(value, tuple) else '}', bracket_color)
     children = [_riprint(val, color, indent + 1) for val in value]
     child_str = ', '.join(children)
     terminal_width = get_terminal_width()
     if len(child_str) <= terminal_width and '\n' not in child_str:
@@ -69,7 +67,9 @@
       array_lines = [next_indent_str + line for line in array_lines]
       array_str = '\n'.join(array_lines)
       return f"ndarray [\n{array_str}\n{indent_str}]"
   return str(value)
 
 def riprint(*values, color=None, print=print, **kwargs):
   print(*(_riprint(value, color) for value in values), **kwargs)
+
+print = riprint
```

## Comparing `riprint-1.0.4.dist-info/LICENSE.txt` & `riprint-1.0.5.dist-info/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2020 Hampus Hallman
+Copyright 2024 Hampus Hallman
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

