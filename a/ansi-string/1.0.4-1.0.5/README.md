# Comparing `tmp/ansi-string-1.0.4.tar.gz` & `tmp/ansi-string-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-1.0.4.tar", last modified: Wed Apr 24 02:56:59 2024, max compression
+gzip compressed data, was "ansi-string-1.0.5.tar", last modified: Wed May  1 00:08:14 2024, max compression
```

## Comparing `ansi-string-1.0.4.tar` & `ansi-string-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 02:56:51.000000 ansi-string-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 02:56:51.000000 ansi-string-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-24 02:56:59.545862 ansi-string-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-24 02:56:51.000000 ansi-string-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 02:56:51.000000 ansi-string-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 02:56:59.545862 ansi-string-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 02:56:51.000000 ansi-string-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47399 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_param.py
--rw-r--r--   0 runner    (1001) docker     (127)    40618 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:08:14.979158 ansi-string-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 00:08:07.000000 ansi-string-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 00:08:07.000000 ansi-string-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-01 00:08:14.979158 ansi-string-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-01 00:08:07.000000 ansi-string-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-01 00:08:07.000000 ansi-string-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 00:08:14.979158 ansi-string-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-01 00:08:07.000000 ansi-string-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:08:14.979158 ansi-string-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:08:14.979158 ansi-string-1.0.5/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 00:08:07.000000 ansi-string-1.0.5/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47399 2024-05-01 00:08:07.000000 ansi-string-1.0.5/src/ansi_string/ansi_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-01 00:08:07.000000 ansi-string-1.0.5/src/ansi_string/ansi_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58503 2024-05-01 00:08:07.000000 ansi-string-1.0.5/src/ansi_string/ansi_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-01 00:08:07.000000 ansi-string-1.0.5/src/ansi_string/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:08:14.979158 ansi-string-1.0.5/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-01 00:08:14.000000 ansi-string-1.0.5/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 00:08:14.000000 ansi-string-1.0.5/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:08:14.000000 ansi-string-1.0.5/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 00:08:14.000000 ansi-string-1.0.5/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 00:08:14.000000 ansi-string-1.0.5/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-1.0.4/LICENSE` & `ansi-string-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.4/PKG-INFO` & `ansi-string-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.4
+Version: 1.0.5
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -46,15 +46,15 @@
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/9d49f88da0275c7a77a63b6d6a90a4e75a80585a/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -71,15 +71,15 @@
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY (i.e. isatty()); no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -102,14 +102,15 @@
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
+
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
 # Enable italics using explicit string directive ("3")
 # Enable bold using explicit integer directive (1)
 s = AnsiString("This is an ANSI string", "light_sea_green", AnsiFormat.BG_CHOCOLATE, "ul_rgb(0x808080)", "3", 1)
@@ -120,35 +121,44 @@
 
 - The static method `AnsiString.join()` is provided to join together 0 to many `str` and `AnsiString` values into a single `AnsiString`.
 - The `+` operator may be used to join an `AnsiString` with another `AnsiString` or `str` into a new `AnsiString`
     - The `+` operator may not be used if the left-hand-side value is a `str` and the right-hand-side values is an `AnsiString`
 - The `+=` operator may be used to append an `AnsiString` or `str` to an `AnsiString`
 
 Examples:
+
 ```py
 s = AnsiString.join("This ", AnsiString("string", AnsiFormat.BOLD))
 s += AnsiString(" contains ") + AnsiString("multiple", AnsiFormat.BG_BLUE)
 s += AnsiString(" color ", AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC) + "settings accross different ranges"
 print(s)
 ```
 
 ### Formatting
 
+#### apply_formatting
+
 The method `AnsiString.apply_formatting()` is provided to append formatting to a previously constructed `AnsiString`.
+
 Example:
+
 ```py
 s = AnsiString("This string contains multiple color settings across different ranges")
 s.apply_formatting(AnsiFormat.BOLD, 5, 11)
 s.apply_formatting(AnsiFormat.BG_BLUE, 21, 29)
 s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 35)
 print(s)
 ```
 
+#### Format String
+
 A format string may be used to format an AnsiString before printing. The format specification string must be in the format `"[string_format][:ansi_format]"` where `string_format` is the standard string format specifier and `ansi_format` contains 0 or more ANSI directives separated by semicolons (;). The ANSI directives may be any of the same string values that can be passed to the `AnsiString` constructor. If no `string_format` is desired, then it can be set to an empty string.
+
 Examples:
+
 ```py
 ansi_str = AnsiString("This is an ANSI string")
 # Right justify with width of 100, formatted bold and red
 print("{:>100:bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
 print("{::bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
@@ -158,19 +168,83 @@
 # Format text, background, and underline with custom colors
 fg_color = 0x8A2BE2
 bg_colors = [100, 232, 170]
 ul_colors = [0xFF, 0x63, 0x47]
 print(f"{ansi_str::rgb({fg_color});bg_rgb({bg_colors});ul_rgb({ul_colors})}")
 ```
 
-The method `AnsiString.format_matching()` is provided to apply formatting to an `AnsiString` based on a match specification.
+#### format_matching and unformat_matching
+
+The method `AnsiString.format_matching()` and `AnsiString.unformat_matching()` are provided to apply or remove formatting of an `AnsiString` based on a match specification.
+
 Example:
+
 ```py
-s = AnsiString("Here is a strING that I will match formatting")
+s = AnsiString("Here is a strING that I will match formatting", AnsiFormat.BOLD)
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
+# This will remove BOLD from "strING" and "formatting"
+s.unformat_matching("[A-Za-z]+ing", AnsiFormat.BOLD, regex=True)
 print(s)
 ```
 
-### Other String Manipulation Methods
+#### clear_formatting
+
+Calling the method `AnsiString.clear_formatting()` will clear all formatting applied.
+
+### String Assignment
+
+The method `AnsiString.assign_str()` may be used to assign the internal string and adjust formatting as necessary.
+
+### Base String Retrieval
+
+The attribute `AnsiString.base_str` may be used to retrieve the unformatted base string.
+
+### Format Status
+
+The methods `AnsiString.ansi_settings_at()` and `AnsiString.settings_at()` may be used to retrieve the settings applied over a single character.
+
+### Other String Methods
 
 Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
+
+- capitalize
+- casefold
+- center
+- count
+- encode
+- endswith
+- expandtabs
+- find
+- index
+- isalnum
+- isalpha
+- isascii
+- isdecimal
+- isdigit
+- isidentifier
+- islower
+- isnumeric
+- isprintable
+- isspace
+- istitle
+- isupper
+- ljust
+- lower
+- lstrip
+- partition
+- removeprefix
+- removesuffix
+- replace
+- rfind
+- rindex
+- rjust
+- rpartition
+- rsplit
+- rstrip
+- split
+- splitlines
+- strip
+- swapcase
+- title
+- upper
+- zfill
```

### Comparing `ansi-string-1.0.4/README.md` & `ansi-string-1.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/9d49f88da0275c7a77a63b6d6a90a4e75a80585a/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -43,15 +43,15 @@
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY (i.e. isatty()); no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -74,14 +74,15 @@
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
+
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
 # Enable italics using explicit string directive ("3")
 # Enable bold using explicit integer directive (1)
 s = AnsiString("This is an ANSI string", "light_sea_green", AnsiFormat.BG_CHOCOLATE, "ul_rgb(0x808080)", "3", 1)
@@ -92,35 +93,44 @@
 
 - The static method `AnsiString.join()` is provided to join together 0 to many `str` and `AnsiString` values into a single `AnsiString`.
 - The `+` operator may be used to join an `AnsiString` with another `AnsiString` or `str` into a new `AnsiString`
     - The `+` operator may not be used if the left-hand-side value is a `str` and the right-hand-side values is an `AnsiString`
 - The `+=` operator may be used to append an `AnsiString` or `str` to an `AnsiString`
 
 Examples:
+
 ```py
 s = AnsiString.join("This ", AnsiString("string", AnsiFormat.BOLD))
 s += AnsiString(" contains ") + AnsiString("multiple", AnsiFormat.BG_BLUE)
 s += AnsiString(" color ", AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC) + "settings accross different ranges"
 print(s)
 ```
 
 ### Formatting
 
+#### apply_formatting
+
 The method `AnsiString.apply_formatting()` is provided to append formatting to a previously constructed `AnsiString`.
+
 Example:
+
 ```py
 s = AnsiString("This string contains multiple color settings across different ranges")
 s.apply_formatting(AnsiFormat.BOLD, 5, 11)
 s.apply_formatting(AnsiFormat.BG_BLUE, 21, 29)
 s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 35)
 print(s)
 ```
 
+#### Format String
+
 A format string may be used to format an AnsiString before printing. The format specification string must be in the format `"[string_format][:ansi_format]"` where `string_format` is the standard string format specifier and `ansi_format` contains 0 or more ANSI directives separated by semicolons (;). The ANSI directives may be any of the same string values that can be passed to the `AnsiString` constructor. If no `string_format` is desired, then it can be set to an empty string.
+
 Examples:
+
 ```py
 ansi_str = AnsiString("This is an ANSI string")
 # Right justify with width of 100, formatted bold and red
 print("{:>100:bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
 print("{::bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
@@ -130,19 +140,83 @@
 # Format text, background, and underline with custom colors
 fg_color = 0x8A2BE2
 bg_colors = [100, 232, 170]
 ul_colors = [0xFF, 0x63, 0x47]
 print(f"{ansi_str::rgb({fg_color});bg_rgb({bg_colors});ul_rgb({ul_colors})}")
 ```
 
-The method `AnsiString.format_matching()` is provided to apply formatting to an `AnsiString` based on a match specification.
+#### format_matching and unformat_matching
+
+The method `AnsiString.format_matching()` and `AnsiString.unformat_matching()` are provided to apply or remove formatting of an `AnsiString` based on a match specification.
+
 Example:
+
 ```py
-s = AnsiString("Here is a strING that I will match formatting")
+s = AnsiString("Here is a strING that I will match formatting", AnsiFormat.BOLD)
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
+# This will remove BOLD from "strING" and "formatting"
+s.unformat_matching("[A-Za-z]+ing", AnsiFormat.BOLD, regex=True)
 print(s)
 ```
 
-### Other String Manipulation Methods
+#### clear_formatting
+
+Calling the method `AnsiString.clear_formatting()` will clear all formatting applied.
+
+### String Assignment
+
+The method `AnsiString.assign_str()` may be used to assign the internal string and adjust formatting as necessary.
+
+### Base String Retrieval
+
+The attribute `AnsiString.base_str` may be used to retrieve the unformatted base string.
+
+### Format Status
+
+The methods `AnsiString.ansi_settings_at()` and `AnsiString.settings_at()` may be used to retrieve the settings applied over a single character.
+
+### Other String Methods
 
 Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
+
+- capitalize
+- casefold
+- center
+- count
+- encode
+- endswith
+- expandtabs
+- find
+- index
+- isalnum
+- isalpha
+- isascii
+- isdecimal
+- isdigit
+- isidentifier
+- islower
+- isnumeric
+- isprintable
+- isspace
+- istitle
+- isupper
+- ljust
+- lower
+- lstrip
+- partition
+- removeprefix
+- removesuffix
+- replace
+- rfind
+- rindex
+- rjust
+- rpartition
+- rsplit
+- rstrip
+- split
+- splitlines
+- strip
+- swapcase
+- title
+- upper
+- zfill
```

### Comparing `ansi-string-1.0.4/setup.py` & `ansi-string-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.4/src/ansi_string/ansi_format.py` & `ansi-string-1.0.5/src/ansi_string/ansi_format.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.4/src/ansi_string/ansi_param.py` & `ansi-string-1.0.5/src/ansi_string/ansi_param.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.4/src/ansi_string/ansi_string.py` & `ansi-string-1.0.5/src/ansi_string/ansi_string.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,38 +22,40 @@
 
 import re
 import math
 from typing import Any, Union, List, Dict, Tuple
 from .ansi_param import AnsiParam
 from .ansi_format import AnsiFormat, AnsiSetting, ColorComponentType, ColourComponentType, ansi_sep, ansi_escape_format, ansi_escape_clear
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 PACKAGE_NAME = 'ansi-string'
 
+# Constant: all characters considered to be whitespaces
 WHITESPACE_CHARS = ' \t\n\r\v\f'
 
 class AnsiString:
     '''
     Represents an ANSI colorized/formatted string. All or part of the string may contain style and
     color formatting which may be used to print out to an ANSI-supported terminal such as those
     on Linux, Mac, and Windows 10+.
     '''
 
     # Change this to True for testing
     WITH_ASSERTIONS = False
 
     def __init__(
         self,
-        s:str='',
-        *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting']
+        s:Union[str,'AnsiString']='',
+        *settings:Union[AnsiFormat, AnsiSetting, str, int, list, tuple]
     ):
         '''
         Creates an AnsiString
-        s: The underlying string
-        setting_or_settings: setting(s) in any of the listed formats below
+        Parameters:
+        s - The underlying string or an AnsiString to copy from
+        settings - setting(s) in any of the listed formats below
             - An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
             - The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`,
               `AnsiFormat.ul_rgb()`, or `AnsiFormat.dul_rgb()`
             - A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
             - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
                 - `rgb(...)` or `fg_rgb(...)` to adjust text color
                 - `bg_rgb(...)` to adjust background color
@@ -68,183 +70,319 @@
             - An AnsiSetting object
             - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
                 - The string will normally be parsed into separate settings unless the character "[" is the first
                   character of the string (ex: `"[38;5;214"`)
                 - Never specify the reset directive (0) because this is implicitly handled internally
             - A single ANSI directive as an integer
         '''
-        self._s = s
         # Key is the string index to make a color change at
         self._fmts:Dict[int,'_AnsiSettingPoint'] = {}
 
+        if isinstance(s, AnsiString):
+            self._s = s._s
+            for k, v in s._fmts.items():
+                self._fmts[k] = _AnsiSettingPoint(list(v.add), list(v.rem))
+        elif isinstance(s, str):
+            self._s = s
+        else:
+            raise TypeError('Invalid type for s')
+
         # Unpack settings
-        settings = []
-        for sos in setting_or_settings:
-            if not isinstance(sos, list) and not isinstance(sos, tuple):
-                settings.append(sos)
+        ansi_settings = []
+        for s in settings:
+            if not isinstance(s, list) and not isinstance(s, tuple):
+                ansi_settings.append(s)
             else:
-                settings += sos
+                ansi_settings += s
 
-        if settings:
-            self.apply_formatting(settings)
+        if ansi_settings:
+            self.apply_formatting(ansi_settings)
 
     def assign_str(self, s:str):
         '''
         Assigns the base string and adjusts the ANSI settings based on the new length.
+        Parameters:
+            s - the new string to set
         '''
         if len(s) > len(self._s):
             if len(self._s) in self._fmts:
                 self._fmts[len(s)] = self._fmts.pop(len(self._s))
         elif len(s) < len(self._s):
             # This may erase some settings that will no longer apply
             self.clip(end=len(s), inplace=True)
         self._s = s
 
     @property
     def base_str(self) -> str:
-        '''
-        Returns the base string without any formatting set.
-        '''
+        ''' Returns the base string without any formatting set. '''
         return self._s
 
     def copy(self) -> 'AnsiString':
-        return self[:]
+        ''' Creates a new AnsiString which is a copy of the original '''
+        return AnsiString(self)
 
-    @staticmethod
-    def _shift_settings_idx(settings_dict:Dict[int,'_AnsiSettingPoint'], num:int, keep_origin:bool):
+    def _shift_settings_idx(self, num:int, keep_origin:bool):
         '''
-        Not fully supported for when num is negative
+        Shifts format settings to the right by the given index
+        Parameters:
+            num - positive number of elements to shift right
+            keep_origin - true to keep format at index 0; false to shift as well
         '''
-        for key in sorted(settings_dict.keys(), reverse=(num > 0)):
+        if num < 0:
+            raise ValueError('num cannot be negative')
+
+        for key in sorted(self._fmts.keys(), reverse=True):
             if not keep_origin or key != 0:
                 new_key = max(key + num, 0)
-                # new_key could be negative when num is negative - TODO: either handle or raise exception
-                settings_dict[new_key] = settings_dict.pop(key)
-
-    def _insert_settings(
-        self,
-        idx:int,
-        apply:bool,
-        settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
-        topmost:bool=True
-    ) -> List['AnsiSetting']:
-        if idx not in self._fmts:
-            self._fmts[idx] = _AnsiSettingPoint()
-        return self._fmts[idx].insert_settings(apply, settings, topmost)
+                self._fmts[new_key] = self._fmts.pop(key)
 
     def apply_formatting(
             self,
-            setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
+            settings:Union[AnsiFormat, AnsiSetting, str, int, list, tuple],
             start:int=0,
             end:Union[int,None]=None,
             topmost:bool=True
     ):
         '''
         Sets the formatting for a given range of characters.
-        Inputs: setting_or_settings - setting or list of settings to apply
-                start - The string start index where setting(s) are to be applied
-                end - The string index where the setting(s) should be removed
-                topmost - When true, this setting is placed at the end of the set for the given
-                          start_index meaning it takes precedent over others; when false, setting is
-                          applied first
+        Parameters:
+            settings - setting or list of settings to apply
+            start - The string start index where setting(s) are to be applied
+            end - The string index where the setting(s) should be removed
+            topmost - When true, the settings placed at the end of the set for the given
+                      start_index, meaning it takes precedent over others; the opposite when False
         '''
         start = self._slice_val_to_idx(start, 0)
         end = self._slice_val_to_idx(end, len(self._s))
 
-        if not setting_or_settings or start >= len(self._s) or end <= start:
+        if not settings or start >= len(self._s) or end <= start:
             # Ignore - nothing to apply
             return
 
-        if not isinstance(setting_or_settings, list) and not isinstance(setting_or_settings, tuple):
-            settings = [setting_or_settings]
-        else:
-            settings = list(setting_or_settings)
-
-        # Settings are removed by reference (using "is" instead of "==") because this is easier than generating unique
-        # IDs, so it is necessary to ensure the incoming settings have distinct references. It would be possible to do
-        # so only if the setting is not already in self._fmts[*].add, but it doesn't add much more overhead to just make
-        # a copy for every incoming AnsiSetting.
-        for i in range(len(settings)):
-            if isinstance(settings[i], AnsiSetting):
-                settings[i] = AnsiSetting(str(settings[i]))
+        ansi_settings = _AnsiSettingPoint._scrub_ansi_settings(settings, make_unique=True)
 
         # Apply settings
-        inserted_settings = self._insert_settings(start, True, settings, topmost)
+        if start not in self._fmts:
+            self._fmts[start] = _AnsiSettingPoint()
+        self._fmts[start].insert_settings(True, ansi_settings, topmost)
 
         # Remove settings
-        self._insert_settings(end, False, inserted_settings, topmost)
+        if end not in self._fmts:
+            self._fmts[end] = _AnsiSettingPoint()
+        self._fmts[end].insert_settings(False, ansi_settings, topmost)
+
+    def remove_formatting(
+            self,
+            settings:Union[None, AnsiFormat, AnsiSetting, str, int, list, tuple]=None,
+            start:int=0,
+            end:Union[int,None]=None
+    ):
+        '''
+        Remove the given formatting settings from the given range
+        Parameters:
+            settings - setting or list of settings to apply (remove all if None specified)
+            start - The string start index where setting(s) are to be applied
+            end - The string index where the setting(s) should be removed
+        '''
+        start = self._slice_val_to_idx(start, 0)
+        end = self._slice_val_to_idx(end, len(self._s))
+
+        if (settings is not None and not settings) or start >= len(self._s) or end <= start:
+            # Ignore - nothing to apply
+            return
+
+        if start not in self._fmts:
+            self._fmts[start] = _AnsiSettingPoint()
+
+        if end not in self._fmts:
+            self._fmts[end] = _AnsiSettingPoint()
+
+        if not settings:
+            ansi_settings = None
+        else:
+            ansi_settings = _AnsiSettingPoint._scrub_ansi_settings(settings)
+
+        removed_settings = []
+        for idx, settings_point, current_settings in _AnsiSettingsIterator(self._fmts):
+            if idx < start:
+                continue
+            elif idx > end:
+                break
+
+            if idx == start:
+                for s in current_settings:
+                    if ansi_settings is None or s in ansi_settings:
+                        add_idx = __class__._find_setting_reference(s, settings_point.add)
+                        if add_idx < 0:
+                            settings_point.rem.append(s)
+                            removed_settings.append(s)
+                        else:
+                            del settings_point.add[add_idx]
+                            removed_settings.append(s)
+            else:
+                for i in reversed(range(len(settings_point.rem))):
+                    s = settings_point.rem[i]
+                    rem_idx = __class__._find_setting_reference(s, removed_settings)
+                    if rem_idx >= 0:
+                        del removed_settings[rem_idx]
+                        del settings_point.rem[i]
+
+                if idx == end:
+                    if end != len(self._s):
+                        settings_point.add += removed_settings
+                else:
+                    for i in reversed(range(len(settings_point.add))):
+                        if ansi_settings is None or settings_point.add[i] in ansi_settings:
+                            removed_settings.append(settings_point.add[i])
+                            del settings_point.add[i]
+
+        # Clean up now empty entries
+        for idx in list(self._fmts.keys()):
+            if not self._fmts[idx]:
+                del self._fmts[idx]
 
     def apply_formatting_for_match(
             self,
-            setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
+            settings:Union[AnsiFormat, AnsiSetting, str, int, list, tuple],
             match_object,
             group:int=0
     ):
         '''
         Apply formatting using a match object generated from re
-        setting_or_settings - setting or list of settings to apply to matching strings
-        match_object - the match object to use (result of re.search() or re.finditer())
-        group - match the group to set
+        Parameters:
+            settings - setting or list of settings to apply to matching strings
+            match_object - the match object to use (result of re.search() or re.finditer())
+            group - match the group to set
         '''
         s = match_object.start(group)
         e = match_object.end(group)
-        self.apply_formatting(setting_or_settings, s, e)
+        self.apply_formatting(settings, s, e)
 
-    def format_matching(self, matchspec:str, *format, regex:bool=False, match_case=False):
+    def format_matching(
+        self,
+        matchspec:str,
+        *format:Union[AnsiFormat, AnsiSetting, str, int, list, tuple],
+        regex:bool=False,
+        match_case=False,
+        count=-1
+    ):
         '''
         Apply formatting for anything matching the matchspec
-        matchspec: the string to match
-        format: 0 to many format specifiers
-        regex: set to True to treat matchspec as a regex string
-        match_case: set to True to make matching case-sensitive (false by default)
+        Parameters:
+            matchspec - the string to match
+            format - 0 to many format specifiers
+            regex - set to True to treat matchspec as a regex string
+            match_case - set to True to make matching case-sensitive (false by default)
+            count - the number of matches to format or -1 to match all
         '''
         if not regex:
             matchspec = re.escape(matchspec)
 
         for match in re.finditer(matchspec, self._s, re.IGNORECASE if not match_case else 0):
-            self.apply_formatting_for_match(format, match)
+            if count < 0 or count > 0:
+                self.apply_formatting_for_match(format, match)
+                if count > 0:
+                    count -= 1
+            else:
+                break
 
-    def clear_formatting(self):
+    def unformat_matching(
+        self,
+        matchspec:str,
+        *format:Union[None, AnsiFormat, AnsiSetting, str, int, list, tuple],
+        regex:bool=False,
+        match_case=False,
+        count=-1
+    ):
         '''
-        Clears all internal formatting.
+        Remove the given formatting for anything matching the matchspec
+        Parameters:
+            matchspec - the string to match
+            format - 0 to many format specifiers (remove all if None specified)
+            regex - set to True to treat matchspec as a regex string
+            match_case - set to True to make matching case-sensitive (false by default)
+            count - the number of matches to unformat or -1 to match all
         '''
+        if not regex:
+            matchspec = re.escape(matchspec)
+
+        if not format or None in format:
+            format = None
+
+        for match in re.finditer(matchspec, self._s, re.IGNORECASE if not match_case else 0):
+            if count < 0 or count > 0:
+                self.remove_formatting(format, match.start(0), match.end(0))
+                if count > 0:
+                    count -= 1
+            else:
+                break
+
+    def clear_formatting(self):
+        ''' Clears all internal formatting. '''
         self._fmts = {}
 
     @staticmethod
     def _find_setting_reference(find:AnsiSetting, in_list:List[AnsiSetting]) -> int:
+        '''
+        Parses a list of AnsiSettings for a given AnsiSetting reference
+        Parameters:
+            find - the setting reference to search for
+            in_list - the setting list to search
+        Returns: -1 if setting not found or integer >=0 if found
+        '''
         for i, s in enumerate(in_list):
             if s is find:
                 return i
         return -1
 
     @staticmethod
-    def _find_settings_references(find_list:List[AnsiSetting], in_list:List[AnsiSetting]) -> List[Tuple]:
+    def _find_settings_references(find_list:List[AnsiSetting], in_list:List[AnsiSetting]) -> List[Tuple[int, int]]:
+        '''
+        Parses a list of AniSettings for any AnsiSetting references in a find list
+        Parameters:
+            find_list - a list of AnsiSetting reference to search for
+            in_list - the list to search in
+        Returns:
+            A list of integer pairs, ordered by elements found from find_list. First element in each pair is a find_list
+            index, and second element is an in_list index.
+        '''
         matches = []
         for i, s in enumerate(find_list):
             for i2, s2 in enumerate(in_list):
                 if s is s2:
                     matches.append((i, i2))
         return matches
 
     def _slice_val_to_idx(self, val:int, default:int) -> int:
+        '''
+        Converts a slice start or stop value to a real index into my string
+        Parameters:
+            val - start or stop value
+            default - the default value to use when val is None
+        Returns: a real index into my string
+        '''
         if val is None:
             return default
         elif val < 0:
             ret_val = len(self._s) + val
             if ret_val < 0:
                 ret_val = 0
             return ret_val
         else:
             return val
 
     def __getitem__(self, val:Union[int, slice]) -> 'AnsiString':
         '''
         Returns a new AnsiString object which represents a substring of self.
-        Note: the new copy may contain some references to settings in the origin. This is ok since the value of each
-              setting is not internally modified after creation.
+        Parameters:
+            val - an index or slice to retrieve (step value must be None or 1 when slice is given)
+        Returns: a new AnsiString which represents the given range in val
+
+        Note: the new copy may contain some references to AnsiSettings in the origin. This is ok since AnsiSettings
+              are not internally modified after creation.
         '''
         if isinstance(val, int):
             st = val
             en = val + 1
         elif isinstance(val, slice):
             if val.step is not None and val.step != 1:
                 raise ValueError('Step other than 1 not supported')
@@ -296,20 +434,23 @@
                 new_s._fmts[new_len] = _AnsiSettingPoint()
             settings_to_remove = [s for s in previous_settings if s not in new_s._fmts[new_len].rem]
             new_s._fmts[new_len].rem.extend(settings_to_remove)
 
         return new_s
 
     def __str__(self) -> str:
-        '''
-        Returns a string with ANSI-formatting applied
-        '''
+        ''' Returns a string with ANSI-formatting applied '''
         return self.__format__(None)
 
     def _apply_string_format(self, string_format:str):
+        '''
+        Applies string formatting, given from the format spec (justification settings)
+        Parameters:
+            string_format - the string format to apply
+        '''
         match = re.search(r'^(.?)<([0-9]*)$', string_format)
         if match:
             # Left justify
             num = match.group(2)
             if num:
                 self.ljust(int(num), match.group(1) or ' ', inplace=True)
             return
@@ -340,18 +481,19 @@
 
         raise ValueError('Invalid format specifier')
 
 
     def __format__(self, __format_spec:str) -> str:
         '''
         Returns an ANSI format string with both internal and given formatting spec set.
-        __format_spec: must be in the format "[string_format][:ansi_format]" where string_format is the standard
-                       string format specifier and ansi_format contains 0 or more ansi directives separated by
-                       semicolons (;)
-                       ex: ">10:bold;fg_red" to make output right justify with width of 10, bold and red formatting
+        Parameters:
+            __format_spec - must be in the format "[string_format][:ansi_format]" where string_format is the standard
+                            string format specifier and ansi_format contains 0 or more ansi directives separated by
+                            semicolons (;)
+                            ex: ">10:bold;red" to make output right justify with width of 10, bold and red formatting
         '''
         if not __format_spec and not self._fmts:
             # No formatting
             return self._s
 
         if __format_spec:
             # Make a copy
@@ -396,38 +538,58 @@
         if clear_needed:
             # Clear settings
             out_str += ansi_escape_clear
 
         return out_str
 
     def __iter__(self) -> 'AnsiString':
-        ''' Iterates over each character '''
+        ''' Iterates over each character of this AnsiString '''
         return iter(_AnsiCharIterator(self))
 
     def capitalize(self, inplace:bool=False) -> 'AnsiString':
+        '''
+        Return a capitalized version of the string.
+        More specifically, make the first character have upper case and the rest lower case.
+        Parameters:
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+        '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.capitalize()
         return obj
 
     def casefold(self, inplace:bool=False) -> 'AnsiString':
+        '''
+        Return a version of the string suitable for caseless comparisons.
+        Parameters:
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+        '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.casefold()
         return obj
 
     def center(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Center justification.
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            width - the number of characters to center over
+            fillchar - the character used to fill empty spaces
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
+        if len(fillchar) != 1:
+            raise ValueError('fillchar must be exactly 1 character in length')
+
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         old_len = len(obj._s)
         num = width - old_len
@@ -435,23 +597,30 @@
             left_spaces = math.floor((num) / 2)
             right_spaces = num - left_spaces
             obj._s = fillchar * left_spaces + obj._s + fillchar * right_spaces
             # Move the removal settings from previous end to new end (formats the right fillchars with same as last char)
             if old_len in obj._fmts:
                 obj._fmts[len(obj._s)] = obj._fmts.pop(old_len)
             # Shift all indices except for the origin (formats the left fillchars with same as first char)
-            __class__._shift_settings_idx(obj._fmts, left_spaces, True)
+            obj._shift_settings_idx(left_spaces, True)
 
         return obj
 
     def ljust(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Left justification.
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            width - the number of characters to left justify over
+            fillchar - the character used to fill empty spaces
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
+        if len(fillchar) != 1:
+            raise ValueError('fillchar must be exactly 1 character in length')
+
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         old_len = len(obj._s)
         num = width - old_len
@@ -462,94 +631,56 @@
                 obj._fmts[len(obj._s)] = obj._fmts.pop(old_len)
 
         return obj
 
     def rjust(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Right justification.
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            width - the number of characters to right justify over
+            fillchar - the character used to fill empty spaces
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
+        if len(fillchar) != 1:
+            raise ValueError('fillchar must be exactly 1 character in length')
+
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         old_len = len(obj._s)
         num = width - old_len
         if num > 0:
             obj._s = fillchar * num + obj._s
             # Shift all indices except for the origin (formats the left fillchars with same as first char)
-            __class__._shift_settings_idx(obj._fmts, num, True)
+            obj._shift_settings_idx(num, True)
 
         return obj
 
-    def count(self, sub:str, start:int=None, end:int=None) -> int:
-        return self._s.count(sub, start, end)
-
-    def encode(self, encoding:str="utf-8", errors:str="strict") -> bytes:
-        return str(self).encode(encoding, errors)
-
-    def endswith(self, suffix:str, start:int=None, end:int=None) -> bool:
-        return self._s.endswith(suffix, start, end)
-
-    def expandtabs(self, tabsize:int=8, inplace:bool=False) -> 'AnsiString':
-        return self.replace('\t', ' ' * tabsize, inplace=inplace)
-
-    def find(self, sub:str, start:int=None, end:int=None) -> int:
-        return self._s.find(sub, start, end)
-
-    def index(self, sub:str, start:int=None, end:int=None) -> int:
-        return self._s.index(sub, start, end)
-
-    def isalnum(self) -> bool:
-        return self._s.isalnum()
-
-    def isalpha(self) -> bool:
-        return self._s.isalpha()
-
-    def isascii(self) -> bool:
+    def __add__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
         '''
-        This is only available for Python >=3.7; exception will be raised in Python 3.6
+        Appends a str or AnsiString to an AnsiString
+        Note: an appended str will take on the formatting of the last character in the AnsiString
+        Parameters:
+            value - the right-hand-side value as str or AnsiString
+        Returns: a new AnsiString
         '''
-        return self._s.isascii()
-
-    def isdecimal(self) -> bool:
-        return self._s.isdecimal()
-
-    def isdigit(self) -> bool:
-        return self._s.isdigit()
-
-    def isidentifier(self) -> bool:
-        return self._s.isidentifier()
-
-    def islower(self) -> bool:
-        return self._s.islower()
-
-    def isnumeric(self) -> bool:
-        return self._s.isnumeric()
-
-    def isprintable(self) -> bool:
-        return self._s.isprintable()
-
-    def isspace(self) -> bool:
-        return self._s.isspace()
-
-    def istitle(self) -> bool:
-        return self._s.istitle()
-
-    def isupper(self) -> bool:
-        return self._s.isupper()
-
-    def __add__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
         cpy = self.copy()
         cpy += value
         return cpy
 
     def __iadd__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
-        ''' Appends a string or AnsiString to this AnsiString '''
+        '''
+        Appends a string or AnsiString to this AnsiString
+        Parameters:
+            value - the right-hand-side value as str or AnsiString
+        Returns: self
+        '''
         if isinstance(value, str):
             self._s += value
         elif isinstance(value, AnsiString):
             shift = len(self._s)
             self._s += value._s
             find_settings = []
             replace_settings = []
@@ -587,27 +718,33 @@
                             del replace_settings[find_idx]
 
         else:
             raise TypeError(f'value is invalid type: {type(value)}')
         return self
 
     def __eq__(self, value:'AnsiString') -> bool:
-        ''' == operator - returns True if exactly equal '''
+        '''
+        == operator - returns True if exactly equal
+        Note: this may return False even if the two strings look the same. To be exactly equal means the format settings
+              are the same, arranged in the same order, and any duplicate entries match between the two.
+        '''
         if not isinstance(value, AnsiString):
             return False
         return self._s == value._s and self._fmts == value._fmts
 
     def __contains__(self, value:Union[str,'AnsiString',Any]) -> bool:
+        ''' Returns True iff the str or the underlying str of an AnsiString is in this AnsiString '''
         if isinstance(value, str):
             return value in self._s
         elif isinstance(value, AnsiString):
             return value._s in self._s
         return False
 
     def __len__(self) -> int:
+        ''' Returns the length of the underlying string '''
         return len(self._s)
 
     @staticmethod
     def join(*args:Union[str,'AnsiString']) -> 'AnsiString':
         ''' Joins strings and AnsiStrings into a single AnsiString object '''
         if not args:
             return AnsiString()
@@ -622,77 +759,96 @@
         for arg in args[1:]:
             joint += arg
         return joint
 
     def lower(self, inplace:bool=False) -> 'AnsiString':
         '''
         Convert to lowercase.
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.lower()
         return obj
 
     def upper(self, inplace:bool=False) -> 'AnsiString':
         '''
         Convert to uppercase.
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.upper()
         return obj
 
     def lstrip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove leading whitespace
-        chars: If not None, remove characters in chars instead
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            chars - If not None, remove characters in chars instead
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=True, do_rstrip=False)
 
     def clip(self, start:int=None, end:int=None, inplace:bool=False) -> 'AnsiString':
         '''
         Calls [] operator and optionally assigns in-place
+        Parameters:
+            start - start index
+            end - end index
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         obj = self[start:end]
         if inplace:
             self._s = obj._s
             self._fmts = obj._fmts
             del obj
             return self
         else:
             return obj
 
     def rstrip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove trailing whitespace
-        chars: If not None, remove characters in chars instead
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            chars - If not None, remove characters in chars instead
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=False, do_rstrip=True)
 
     def strip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove leading and trailing whitespace
-        chars: If not None, remove characters in chars instead
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            chars - If not None, remove characters in chars instead
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=True, do_rstrip=True)
 
     def _strip(self, chars:str=None, inplace:bool=False, do_lstrip:bool=True, do_rstrip:bool=True) -> 'AnsiString':
         '''
         Remove leading and trailing whitespace
-        chars: If not None, remove characters in chars instead
-        inplace: True to execute in-place; False to return a copy
+        Parameters:
+            chars - If not None, remove characters in chars instead
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+            do_lstrip - True to do left strip
+            do_rstrip - Trie to do right strip
         '''
         if chars is None:
             chars = WHITESPACE_CHARS
 
         lcount = 0
         if do_lstrip:
             for char in self._s:
@@ -748,80 +904,301 @@
         if idx >= 0:
             sep_len = len(sep)
             idx_end = idx + sep_len
             return (self[0:idx], self[idx:idx_end], self[idx_end:])
         else:
             return (self.copy(), AnsiString(), AnsiString())
 
-    def _settings_at(self, idx:int) -> List[AnsiSetting]:
+    def ansi_settings_at(self, idx:int) -> List[AnsiSetting]:
+        '''
+        Returns a list of AnsiSettings at the given index
+        Parameters:
+            idx - the index to get settings of
+        '''
         if idx >= 0 and idx < len(self._s):
             previous_settings = []
             for sidx, _, current_settings in _AnsiSettingsIterator(self._fmts):
                 if sidx > idx:
                     break
                 previous_settings = list(current_settings)
             return previous_settings
         else:
             return []
 
     def settings_at(self, idx:int) -> str:
         '''
         Returns a string which represents the settings being used at the given index
+        Parameters:
+            idx - the index to get settings of
         '''
-        return ansi_sep.join([str(s) for s in self._settings_at(idx)])
+        return ansi_sep.join([str(s) for s in self.ansi_settings_at(idx)])
 
     def removeprefix(self, prefix:str, inplace:bool=False) -> 'AnsiString':
+        '''
+        Return a str with the given prefix string removed if present.
+
+        If the string starts with the prefix string, return string[len(prefix):]. Otherwise, return the original string.
+
+        Parameters:
+            prefix - the prefix to remove
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+        '''
         if not self._s.startswith(prefix):
             if inplace:
                 return self
             else:
                 return self.copy()
         else:
             return self.clip(start=len(prefix), inplace=inplace)
 
     def removesuffix(self, suffix:str, inplace:bool=False) -> 'AnsiString':
+        '''
+        Return a str with the given suffix string removed if present.
+
+        If the string ends with the suffix string and that suffix is not empty, return string[:-len(suffix)]. Otherwise,
+        return the original string.
+
+        Parameters:
+            suffix - the suffix to remove
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+        '''
         if not self._s.endswith(suffix):
             if inplace:
                 return self
             else:
                 return self.copy()
         else:
             return self.clip(end=-len(suffix), inplace=inplace)
 
     def replace(self, old:str, new:Union[str,'AnsiString'], count:int=-1, inplace:bool=False) -> 'AnsiString':
         '''
         Does a find-and-replace - if new is a str, the string the is applied will take on the format settings of the
         first character of the old string in each replaced item.
+        Parameters:
+            old - the string to search for
+            new - the string to replace; if this is a str type, the formatting of the replacement will match the
+                  formatting of the first character of the old string
+            count - the number of occurrences to replace or -1 to replace all occurrences
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
         '''
         obj = self
         idx = obj._s.find(old)
         while (count < 0 or count > 0) and idx >= 0:
             if isinstance(new, str):
-                replace = AnsiString(new, obj._settings_at(idx))
+                replace = AnsiString(new, obj.ansi_settings_at(idx))
             else:
                 replace = new
             obj = obj[:idx] + replace + obj[idx+len(old):]
             if count > 0:
                 count -= 1
             idx = obj._s.find(old, idx + len(new))
 
         if inplace:
             self._s = obj._s
             self._fmts = obj._fmts
             return self
         else:
             return obj
 
+    def count(self, sub:str, start:int=None, end:int=None) -> int:
+        '''
+        Return the number of non-overlapping occurrences of substring sub in
+        string S[start:end]. Optional arguments start and end are interpreted as in slice notation.
+        '''
+        return self._s.count(sub, start, end)
+
+    def encode(self, encoding:str="utf-8", errors:str="strict") -> bytes:
+        '''
+        Encode the string using the codec registered for encoding.
+
+        encoding
+        The encoding in which to encode the string.
+        errors
+        The error handling scheme to use for encoding errors. The default is 'strict' meaning that encoding errors raise
+        a UnicodeEncodeError. Other possible values are 'ignore', 'replace' and 'xmlcharrefreplace' as well as any other
+        name registered with codecs.register_error that can handle UnicodeEncodeErrors.
+        '''
+        return str(self).encode(encoding, errors)
+
+    def endswith(self, suffix:str, start:int=None, end:int=None) -> bool:
+        '''
+        Return True if S ends with the specified suffix, False otherwise. With optional start, test S beginning at that
+        position. With optional end, stop comparing S at that position. suffix can also be a tuple of strings to try.
+        '''
+        return self._s.endswith(suffix, start, end)
+
+    def expandtabs(self, tabsize:int=8, inplace:bool=False) -> 'AnsiString':
+        '''
+        Replaces all tab characters with the given number of spaces
+        Parameters:
+            tabsize - number of spaces to replace each tab with
+            inplace - when True, do the conversion in-place and return self;
+                      when False, do the conversion on a copy and return the copy
+        '''
+        return self.replace('\t', ' ' * tabsize, inplace=inplace)
+
+    def find(self, sub:str, start:int=None, end:int=None) -> int:
+        '''
+        Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].
+        Optional arguments start and end are interpreted as in slice notation.
+
+        Return -1 on failure.
+        '''
+        return self._s.find(sub, start, end)
+
+    def index(self, sub:str, start:int=None, end:int=None) -> int:
+        '''
+        Return the lowest index in S where substring sub is found, such that sub is contained within S[start:end].
+        Optional arguments start and end are interpreted as in slice notation.
+
+        Raises ValueError when the substring is not found.
+        '''
+        return self._s.index(sub, start, end)
+
+    def isalnum(self) -> bool:
+        '''
+        Return True if the string is an alpha-numeric string, False otherwise.
+
+        A string is alpha-numeric if all characters in the string are alpha-numeric and there is at least one character
+        in the string
+        '''
+        return self._s.isalnum()
+
+    def isalpha(self) -> bool:
+        '''
+        Return True if the string is an alphabetic string, False otherwise.
+
+        A string is alphabetic if all characters in the string are alphabetic and there is at least one character in the
+        string.
+        '''
+        return self._s.isalpha()
+
+    def isascii(self) -> bool:
+        '''
+        This is only available for Python >=3.7; exception will be raised in Python 3.6
+
+        Return True if all characters in the string are ASCII, False otherwise.
+
+        ASCII characters have code points in the range U+0000-U+007F. Empty string is ASCII too.
+        '''
+        return self._s.isascii()
+
+    def isdecimal(self) -> bool:
+        '''
+        Return True if the string is a decimal string, False otherwise.
+
+        A string is a decimal string if all characters in the string are decimal and there is at least one character in
+        the string.
+        '''
+        return self._s.isdecimal()
+
+    def isdigit(self) -> bool:
+        '''
+        Return True if the string is a digit string, False otherwise.
+
+        A string is a digit string if all characters in the string are digits and there is at least one character in the
+        string.
+        '''
+        return self._s.isdigit()
+
+    def isidentifier(self) -> bool:
+        '''
+        Return True if the string is a valid Python identifier, False otherwise.
+
+        Call keyword.iskeyword(s) to test whether string s is a reserved identifier, such as "def" or "class".
+        '''
+        return self._s.isidentifier()
+
+    def islower(self) -> bool:
+        '''
+        Return True if the string is a lowercase string, False otherwise.
+
+        A string is lowercase if all cased characters in the string are lowercase and there is at least one cased
+        character in the string.
+        '''
+        return self._s.islower()
+
+    def isnumeric(self) -> bool:
+        '''
+        Return True if the string is a numeric string, False otherwise.
+
+        A string is numeric if all characters in the string are numeric and there is at least one character in the
+        string.
+        '''
+        return self._s.isnumeric()
+
+    def isprintable(self) -> bool:
+        '''
+        Return True if the string is printable, False otherwise.
+
+        A string is printable if all of its characters are considered printable in repr() or if it is empty.
+        '''
+        return self._s.isprintable()
+
+    def isspace(self) -> bool:
+        '''
+        Return True if the string is a whitespace string, False otherwise.
+
+        A string is whitespace if all characters in the string are whitespace and there is at least one character in the string.
+        '''
+        return self._s.isspace()
+
+    def istitle(self) -> bool:
+        '''
+        Return True if the string is a title-cased string, False otherwise.
+
+        In a title-cased string, upper- and title-case characters may only follow uncased characters and lowercase
+        characters only cased ones.
+        '''
+        return self._s.istitle()
+
+    def isupper(self) -> bool:
+        '''
+        Return True if the string is an uppercase string, False otherwise.
+
+        A string is uppercase if all cased characters in the string are uppercase and there is at least one cased
+        character in the string.
+        '''
+        return self._s.isupper()
+
     def rfind(self, sub:str, start:int=None, end:int=None) -> int:
+        '''
+        S.rfind(sub[, start[, end]]) -> int
+
+        Return the highest index in S where substring sub is found,
+        such that sub is contained within S[start:end]. Optional arguments start and end are interpreted as in slice
+        notation.
+
+        Return -1 on failure.
+        '''
         return self._s.rfind(sub, start, end)
 
     def rindex(self, sub:str, start:int=None, end:int=None) -> int:
+        '''
+        S.rindex(sub[, start[, end]]) -> int
+
+        Return the highest index in S where substring sub is found,
+        such that sub is contained within S[start:end]. Optional arguments start and end are interpreted as in slice
+        notation.
+
+        Raises ValueError when the substring is not found.
+        '''
         return self._s.rindex(sub, start, end)
 
     def _split(self, sep:Union[str,None]=None, maxsplit:int=-1, r:bool=False) -> List['AnsiString']:
+        '''
+        Return a list of substrings in the string, using sep as the separator string.
+        Parameters:
+            sep - the separator string (use whitespace characters if None)
+            maxsplit - maximum number of splits to make or -1 for no limit
+            r - True to search from right; False to search from left
+        '''
         if r:
             str_splits = self._s.rsplit(sep, maxsplit)
         else:
             str_splits = self._s.split(sep, maxsplit)
         split_idx_len = []
         idx = 0
         for s in str_splits:
@@ -832,20 +1209,52 @@
         ansi_str_splits = []
         for idx, length in split_idx_len:
             ansi_str_splits.append(self[idx:idx+length])
 
         return ansi_str_splits
 
     def split(self, sep:Union[str,None]=None, maxsplit:int=-1) -> List['AnsiString']:
+        '''
+        Return a list of the substrings in the string, using sep as the separator string.
+
+        sep
+            The separator used to split the string.
+
+            When set to None (the default value), will split on any whitespace character (including \n \r \t \f and
+            spaces) and will discard empty strings from the result.
+        maxsplit
+            Maximum number of splits (starting from the left). -1 (the default value) means no limit.
+
+        Note, str.split() is mainly useful for data that has been intentionally delimited. With natural text that
+        includes punctuation, consider using the regular expression module.
+        '''
         return self._split(sep, maxsplit, False)
 
     def rsplit(self, sep:Union[str,None]=None, maxsplit:int=-1) -> List['AnsiString']:
+        '''
+        Return a list of the substrings in the string, using sep as the separator string.
+
+        sep
+            The separator used to split the string.
+
+            When set to None (the default value), will split on any whitespace character (including \n \r \t \f and
+            spaces) and will discard empty strings from the result.
+        maxsplit
+            Maximum number of splits (starting from the left). -1 (the default value) means no limit.
+
+        Splitting starts at the end of the string and works to the front.
+        '''
         return self._split(sep, maxsplit, True)
 
     def splitlines(self, keepends:bool=False) -> List['AnsiString']:
+        '''
+        Return a list of the lines in the string, breaking at line boundaries.
+
+        Line breaks are not included in the resulting list unless keepends is given and true.
+        '''
         str_splits = self._s.splitlines(keepends)
         split_idx_len = []
         idx = 0
         for s in str_splits:
             idx = self._s.find(s, idx)
             split_idx_len.append((idx, len(s)))
             idx += len(s)
@@ -853,34 +1262,45 @@
         ansi_str_splits = []
         for idx, length in split_idx_len:
             ansi_str_splits.append(self[idx:idx+length])
 
         return ansi_str_splits
 
     def swapcase(self, inplace:bool=False) -> 'AnsiString':
+        ''' Convert uppercase characters to lowercase and lowercase characters to uppercase. '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         obj._s = obj._s.swapcase()
 
         return obj
 
     def title(self, inplace:bool=False) -> 'AnsiString':
+        '''
+        Return a version of the string where each word is titlecased.
+
+        More specifically, words start with uppercased characters and all remaining cased characters have lower case.
+        '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         obj._s = obj._s.title()
 
         return obj
 
     def zfill(self, width:int, inplace:bool=False) -> 'AnsiString':
+        '''
+        Pad a numeric string with zeros on the left, to fill a field of the given width.
+
+        The string is never truncated.
+        '''
         return self.rjust(width, "0", inplace)
 
 
 class _AnsiSettingPoint:
     '''
     This class is used internally to keep track of ANSI settings at a specific string index
     '''
@@ -930,14 +1350,20 @@
             except ValueError:
                 raise ValueError('Invalid rgb value')
             # Get RGB format and remove the leading '['
             return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
         return None
 
     @staticmethod
+    def _scrub_ansi_format_int(ansi_format:int) -> AnsiSetting:
+        if ansi_format < 0:
+            raise ValueError(f'Invalid value [{ansi_format}]; must be greater than or equal to 0')
+        return AnsiSetting(ansi_format)
+
+    @staticmethod
     def _scrub_ansi_format_string(ansi_format:str) -> List[AnsiSetting]:
         if ansi_format.startswith("["):
             # Use the rest of the string as-is for settings
             return [AnsiSetting(ansi_format[1:])]
         else:
             # The format string contains names within AnsiFormat or integers, separated by semicolon
             formats = ansi_format.split(ansi_sep)
@@ -952,76 +1378,71 @@
                     format_settings.append(ansi_fmt_enum.setting)
 
                 if ansi_fmt_enum is None:
                     rgb_format = __class__._parse_rgb_string(format)
                     if not rgb_format:
                         try:
                             int_value = int(format)
-                            # 0 should never be used because it will mess with internal assumptions
-                            # Negative values are invalid
-                            if int_value < 0:
-                                raise ValueError(f'Invalid value [{int_value}]; must be greater than or equal to 0')
                         except ValueError:
                             raise ValueError(
                                 'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
                                 .format(ansi_format, format)
                             )
                         else:
                             # Value is an integer - use the format verbatim
-                            format_settings.append(AnsiSetting(format))
+                            format_settings.append(__class__._scrub_ansi_format_int(int_value))
                     else:
                         format_settings.append(rgb_format)
             return format_settings
 
-    def insert_setting(self, apply:bool, setting:'AnsiSetting', topmost:bool=True):
-        lst = self.add if apply else self.rem
-        if topmost:
-            lst.append(setting)
-        else:
-            lst.insert(0, setting)
-
-    def insert_settings(
-        self,
-        apply:bool,
+    @staticmethod
+    def _scrub_ansi_settings(
         settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
-        topmost:bool=True
-    ) -> List['AnsiSetting']:
+        make_unique=False
+    ) -> List[AnsiSetting]:
         if not isinstance(settings, list) and not isinstance(settings, tuple):
             settings = [settings]
 
-        settings_to_insert = []
+        settings_out = []
         for setting in settings:
             if isinstance(setting, AnsiSetting):
-                settings_to_insert.append(setting)
-            elif isinstance(setting, str) or isinstance(setting, int):
-                settings_to_insert.extend(__class__._scrub_ansi_format_string(str(setting)))
+                if make_unique:
+                    setting = AnsiSetting(setting)
+                settings_out.append(setting)
+            elif isinstance(setting, str):
+                settings_out.extend(__class__._scrub_ansi_format_string(setting))
+            elif isinstance(setting, int):
+                settings_out.append(__class__._scrub_ansi_format_int(setting))
             elif hasattr(setting, "setting"):
-                settings_to_insert.append(setting.setting)
+                settings_out.append(setting.setting)
+        return settings_out
+
+    def insert_settings(self, apply:bool, settings:Union[List[AnsiSetting], AnsiSetting], topmost:bool=True):
+        if not isinstance(settings, list) and not isinstance(settings, tuple):
+            settings = [settings]
 
         lst = self.add if apply else self.rem
         if topmost:
-            lst.extend(settings_to_insert)
+            lst.extend(settings)
         else:
-            lst[:0] = settings_to_insert
-
-        return settings_to_insert
+            lst[:0] = settings
 
 class _AnsiSettingsIterator:
     '''
     Internally-used class which helps iterate over settings
     '''
-    def __init__(self, settings_dict:Dict[int,'_AnsiSettingPoint']):
+    def __init__(self, settings_dict:Dict[int,_AnsiSettingPoint]):
         self.settings_dict:Dict[int,_AnsiSettingPoint] = settings_dict
         self.current_settings:List[AnsiSetting] = []
         self.dict_iter = iter(sorted(self.settings_dict))
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> Tuple[int,'_AnsiSettingPoint',List['AnsiSetting']]:
+    def __next__(self) -> Tuple[int,_AnsiSettingPoint,List[AnsiSetting]]:
         # Will raise StopIteration when complete
         idx = next(self.dict_iter)
         settings = self.settings_dict[idx]
         # Remove settings that it is time to remove
         for setting in settings.rem:
             # setting object will only be matched and removed if it is the same reference to one
             # previously added - will raise exception otherwise which should not happen if the
@@ -1047,8 +1468,8 @@
     def __iter__(self):
         return self
 
     def __next__(self) -> 'AnsiString':
         self.current_idx += 1
         if self.current_idx >= len(self.s):
             raise StopIteration
-        return self.s[self.current_idx]
+        return self.s[self.current_idx]
```

### Comparing `ansi-string-1.0.4/src/ansi_string/utils.py` & `ansi-string-1.0.5/src/ansi_string/utils.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.4/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-1.0.5/src/ansi_string.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.4
+Version: 1.0.5
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -46,15 +46,15 @@
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/9d49f88da0275c7a77a63b6d6a90a4e75a80585a/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -71,15 +71,15 @@
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY (i.e. isatty()); no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -102,14 +102,15 @@
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
+
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
 # Enable italics using explicit string directive ("3")
 # Enable bold using explicit integer directive (1)
 s = AnsiString("This is an ANSI string", "light_sea_green", AnsiFormat.BG_CHOCOLATE, "ul_rgb(0x808080)", "3", 1)
@@ -120,35 +121,44 @@
 
 - The static method `AnsiString.join()` is provided to join together 0 to many `str` and `AnsiString` values into a single `AnsiString`.
 - The `+` operator may be used to join an `AnsiString` with another `AnsiString` or `str` into a new `AnsiString`
     - The `+` operator may not be used if the left-hand-side value is a `str` and the right-hand-side values is an `AnsiString`
 - The `+=` operator may be used to append an `AnsiString` or `str` to an `AnsiString`
 
 Examples:
+
 ```py
 s = AnsiString.join("This ", AnsiString("string", AnsiFormat.BOLD))
 s += AnsiString(" contains ") + AnsiString("multiple", AnsiFormat.BG_BLUE)
 s += AnsiString(" color ", AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC) + "settings accross different ranges"
 print(s)
 ```
 
 ### Formatting
 
+#### apply_formatting
+
 The method `AnsiString.apply_formatting()` is provided to append formatting to a previously constructed `AnsiString`.
+
 Example:
+
 ```py
 s = AnsiString("This string contains multiple color settings across different ranges")
 s.apply_formatting(AnsiFormat.BOLD, 5, 11)
 s.apply_formatting(AnsiFormat.BG_BLUE, 21, 29)
 s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 35)
 print(s)
 ```
 
+#### Format String
+
 A format string may be used to format an AnsiString before printing. The format specification string must be in the format `"[string_format][:ansi_format]"` where `string_format` is the standard string format specifier and `ansi_format` contains 0 or more ANSI directives separated by semicolons (;). The ANSI directives may be any of the same string values that can be passed to the `AnsiString` constructor. If no `string_format` is desired, then it can be set to an empty string.
+
 Examples:
+
 ```py
 ansi_str = AnsiString("This is an ANSI string")
 # Right justify with width of 100, formatted bold and red
 print("{:>100:bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
 print("{::bold;red}".format(ansi_str))
 # No justification settings, formatted bold and red
@@ -158,19 +168,83 @@
 # Format text, background, and underline with custom colors
 fg_color = 0x8A2BE2
 bg_colors = [100, 232, 170]
 ul_colors = [0xFF, 0x63, 0x47]
 print(f"{ansi_str::rgb({fg_color});bg_rgb({bg_colors});ul_rgb({ul_colors})}")
 ```
 
-The method `AnsiString.format_matching()` is provided to apply formatting to an `AnsiString` based on a match specification.
+#### format_matching and unformat_matching
+
+The method `AnsiString.format_matching()` and `AnsiString.unformat_matching()` are provided to apply or remove formatting of an `AnsiString` based on a match specification.
+
 Example:
+
 ```py
-s = AnsiString("Here is a strING that I will match formatting")
+s = AnsiString("Here is a strING that I will match formatting", AnsiFormat.BOLD)
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
+# This will remove BOLD from "strING" and "formatting"
+s.unformat_matching("[A-Za-z]+ing", AnsiFormat.BOLD, regex=True)
 print(s)
 ```
 
-### Other String Manipulation Methods
+#### clear_formatting
+
+Calling the method `AnsiString.clear_formatting()` will clear all formatting applied.
+
+### String Assignment
+
+The method `AnsiString.assign_str()` may be used to assign the internal string and adjust formatting as necessary.
+
+### Base String Retrieval
+
+The attribute `AnsiString.base_str` may be used to retrieve the unformatted base string.
+
+### Format Status
+
+The methods `AnsiString.ansi_settings_at()` and `AnsiString.settings_at()` may be used to retrieve the settings applied over a single character.
+
+### Other String Methods
 
 Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
+
+- capitalize
+- casefold
+- center
+- count
+- encode
+- endswith
+- expandtabs
+- find
+- index
+- isalnum
+- isalpha
+- isascii
+- isdecimal
+- isdigit
+- isidentifier
+- islower
+- isnumeric
+- isprintable
+- isspace
+- istitle
+- isupper
+- ljust
+- lower
+- lstrip
+- partition
+- removeprefix
+- removesuffix
+- replace
+- rfind
+- rindex
+- rjust
+- rpartition
+- rsplit
+- rstrip
+- split
+- splitlines
+- strip
+- swapcase
+- title
+- upper
+- zfill
```

