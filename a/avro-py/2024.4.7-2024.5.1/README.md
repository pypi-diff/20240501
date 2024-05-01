# Comparing `tmp/avro.py-2024.4.7.tar.gz` & `tmp/avro_py-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2024.4.7.tar", last modified: Sun Apr  7 06:59:50 2024, max compression
+gzip compressed data, was "avro_py-2024.5.1.tar", max compression
```

## Comparing `avro.py-2024.4.7.tar` & `avro_py-2024.5.1.tar`

### file list

```diff
@@ -1,31 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 06:59:46.000000 avro.py-2024.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-07 06:59:46.000000 avro.py-2024.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.337261 avro.py-2024.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-07 06:59:46.000000 avro.py-2024.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/
--rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12937 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      576 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2389 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 06:59:46.000000 avro.py-2024.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:59:50.337261 avro.py-2024.4.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1804 2024-04-07 06:59:46.000000 avro.py-2024.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5589 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1051 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3923 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_validate.py
+-rw-r--r--   0        0        0     1072 2024-05-01 12:02:57.923729 avro_py-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     6156 2024-05-01 12:02:57.923729 avro_py-2024.5.1/README.md
+-rwxr-xr-x   0        0        0       77 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/__init__.py
+-rw-r--r--   0        0        0     2883 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/cli.py
+-rwxr-xr-x   0        0        0      799 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/config.py
+-rwxr-xr-x   0        0        0    12937 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/main.py
+-rw-r--r--   0        0        0       83 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/resources/__init__.py
+-rw-r--r--   0        0        0    39017 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/resources/dictionary.py
+-rw-r--r--   0        0        0       31 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/__init__.py
+-rwxr-xr-x   0        0        0      472 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/count.py
+-rwxr-xr-x   0        0        0     2311 2024-05-01 12:02:57.927729 avro_py-2024.5.1/avro/utils/validate.py
+-rw-r--r--   0        0        0     1746 2024-05-01 12:02:57.927729 avro_py-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 avro_py-2024.5.1/PKG-INFO
```

### Comparing `avro.py-2024.4.7/LICENSE` & `avro_py-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avro.py-2024.4.7/PKG-INFO` & `avro_py-2024.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
-Name: avro.py
-Version: 2024.4.7
+Name: avro-py
+Version: 2024.5.1
 Summary: A modern Pythonic implementation of Avro Phonetic.
-Home-page: https://github.com/hitblast/avro.py
-Author: HitBlast
-Author-email: hitblastlive@gmail.com
+Home-page: https://pypi.org/project/avro-py
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
+Author: HitBlast
+Author-email: hitblastlive@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: cli
-Requires-Dist: click>=8.0.0; extra == "cli"
-Requires-Dist: pyclip>=0.7.0; extra == "cli"
-
+Requires-Dist: click (>=8,<9) ; extra == "cli"
+Requires-Dist: pyclip (>=0.7.0,<0.8.0) ; extra == "cli"
+Requires-Dist: rich (>=13,<14) ; extra == "cli"
+Project-URL: Documentation, https://hitblast.github.io/avro.py
+Project-URL: Repository, https://github.com/hitblast/avro.py
+Description-Content-Type: text/markdown
 
 <!-- SPDX-License-Identifier: MIT -->
 
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
@@ -146,28 +148,28 @@
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
 
 ---
 
 **Additional Developer Notes**
 
-In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools. <br>
+In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools.
 
-- [ruff](https://github.com/astral-sh/ruff) - linter
-- [pytest](https://pypi.python.org/pypi/pytest) - testing framework
+**Poetry** has been used to manage the project's dependencies and virtual environment. You can install it by following [the instructions here](https://python-poetry.org/docs/). The dependencies have been configured using the `pyproject.toml` file and doesn't require manual installation. Simply set up your developer environment using the following commands: <br>
 
 ```sh
-# Installing the required developer toolchain.
-$ python3 -m pip install -r requirements.txt
+# Set up virtual environment and activate it.
+$ python3 -m venv venv && source venv/bin/activate
 
-# (Optional) Setting up the package itself for testing purposes.
-$ python3 setup.py develop
+# Install required first-party dependencies and Poetry for dependency management.
+# (Note: Skip this step if Poetry is globally installed and added to PATH.)
+$ pip install -U pip setuptools && pip install poetry
 
-# Running the predetermined tests inside the project.
-$ python3 -m pytest --verbose
+# Setup project using Poetry.
+$ poetry install --all-extras
 ```
 
 ### 🐛 We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
@@ -183,7 +185,8 @@
 - Md Enzam Hossain for helping him understand the ins and outs of the Avro dictionary and the way it works.
 
 <br>
 
 ## 📋 License
 
 Licensed under the [MIT License](https://github.com/hitblast/avro.py/blob/main/LICENSE).
+
```

### Comparing `avro.py-2024.4.7/README.md` & `avro_py-2024.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -120,28 +120,28 @@
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
 
 ---
 
 **Additional Developer Notes**
 
-In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools. <br>
+In short, avro.py doesn't depend on any third-party libraries. However, if you'd like to contribute to the project, you'll need a handful of such useful tools.
 
-- [ruff](https://github.com/astral-sh/ruff) - linter
-- [pytest](https://pypi.python.org/pypi/pytest) - testing framework
+**Poetry** has been used to manage the project's dependencies and virtual environment. You can install it by following [the instructions here](https://python-poetry.org/docs/). The dependencies have been configured using the `pyproject.toml` file and doesn't require manual installation. Simply set up your developer environment using the following commands: <br>
 
 ```sh
-# Installing the required developer toolchain.
-$ python3 -m pip install -r requirements.txt
+# Set up virtual environment and activate it.
+$ python3 -m venv venv && source venv/bin/activate
 
-# (Optional) Setting up the package itself for testing purposes.
-$ python3 setup.py develop
+# Install required first-party dependencies and Poetry for dependency management.
+# (Note: Skip this step if Poetry is globally installed and added to PATH.)
+$ pip install -U pip setuptools && pip install poetry
 
-# Running the predetermined tests inside the project.
-$ python3 -m pytest --verbose
+# Setup project using Poetry.
+$ poetry install --all-extras
 ```
 
 ### 🐛 We're looking for bug hunters, by the way!
 
 If you come across any kind of bug or wanna request a feature, please let us know by opening an issue [here](https://github.com/hitblast/avro.py/issues). We do need more ideas to keep the project alive and running, don't we? :P
 
 ---
```

### Comparing `avro.py-2024.4.7/avro/cli.py` & `avro_py-2024.5.1/avro/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,76 +6,92 @@
 
 import avro
 
 # Try to import the required modules.
 try:
     import click
     import pyclip
+    from rich.console import Console
+
 except ImportError:
-    print('In order to enable CLI, please install avro.py using: pip install avro.py[cli]')
+    print("In order to enable CLI, please install avro.py using: pip install avro.py[cli]")
     exit()
 
 
 # Create a new group for putting the CLI commands.
-@click.group(help=avro.__description__)
+@click.group(help="A modern Pythonic implementation of Avro Phonetic.")
 @click.version_option(
-    package_name='avro.py',
-    message='Package: %(prog)s, version %(version)s\nCore: version {0}'.format(avro.__version__),
+    package_name="avro.py",
+    message="Package: %(prog)s, version %(version)s\n",
 )
 def cli() -> None:
     pass
 
 
+# Initialize Console object for rich-based output.
+console = Console()
+
+
+# Helper functions for CLI commands.
+def _print_err(text: str) -> None:
+    console.print(text, style="red")
+    return click.echo(err=True)
+
+
 # Helper function for CLI actions.
 def _cli_action(
     text: str,
     *,
     bijoy: bool = False,
     from_clipboard: bool = False,
     copy_on_success: bool = False,
     reverse: bool = False,
 ) -> Optional[str]:
     if not text:
         if not from_clipboard:
-            return click.echo('No text provided.')
+            return _print_err("No text provided.")
         else:
             if not (text := pyclip.paste(text=True).strip()):
-                return click.echo('No text found in the clipboard.')
+                return _print_err("No text found in the clipboard.")
 
     if reverse:
-        text = avro.reverse(text)
+        output = avro.reverse(text)
     else:
-        text = avro.parse(text) if not bijoy else avro.parse(text, bijoy=True)
+        output = avro.parse(text) if not bijoy else avro.parse(text, bijoy=True)
+
+    if output == text:
+        return _print_err("No changes in output.")
+
+    console.print(f"\n[bold green]Output[/bold green]\n {text}\n")
 
     if copy_on_success:
         pyclip.copy(text)
-
-    click.echo(text)
+        console.print("[bold yellow](copied to clipboard)[/bold yellow]\n")
 
 
 # usage: avro parse <text> [--bijoy] [--from-clip] [--copy]
-@cli.command('parse', help='Parse a given text to Bangla / Bengali.')
-@click.argument('text', required=False)
-@click.option('--bijoy', is_flag=True, help='Use Bijoy Keyboard format for parsing.')
-@click.option('--from-clip', is_flag=True, help='Parse text from clipboard.')
-@click.option('--copy', is_flag=True, help='Copy the parsed text to clipboard.')
-def _parse(text: str = '', bijoy: bool = False, from_clip: bool = False, copy: bool = False) -> None:
+@cli.command("parse", help="Parse a given text to Bangla / Bengali.")
+@click.argument("text", required=False)
+@click.option("--bijoy", is_flag=True, help="Use Bijoy Keyboard format for parsing.")
+@click.option("--from-clip", is_flag=True, help="Parse text from clipboard.")
+@click.option("--copy", is_flag=True, help="Copy the parsed text to clipboard.")
+def _parse(text: str = "", bijoy: bool = False, from_clip: bool = False, copy: bool = False) -> None:
     _cli_action(
         text,
         bijoy=bijoy,
         from_clipboard=from_clip,
         copy_on_success=copy,
     )
 
 
 # usage: avro reverse <text> [--from-clip] [--copy]
-@cli.command('reverse', help='Reverse a given text to English.')
-@click.argument('text')
-@click.option('--from-clip', is_flag=True, help='Reverse text from clipboard.')
-@click.option('--copy', is_flag=True, help='Copy the reversed text to clipboard.')
+@cli.command("reverse", help="Reverse a given text to English.")
+@click.argument("text")
+@click.option("--from-clip", is_flag=True, help="Reverse text from clipboard.")
+@click.option("--copy", is_flag=True, help="Copy the reversed text to clipboard.")
 def _reverse(text: str, from_clip: bool = False, copy: bool = False) -> None:
     _cli_action(
         text,
         from_clipboard=from_clip,
         copy_on_success=copy,
         reverse=True,
     )
```

### Comparing `avro.py-2024.4.7/avro/main.py` & `avro_py-2024.5.1/avro/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 # Import local modules.
 from . import config
 from .utils import validate
 
 # Constants.
-PATTERNS = config.DICT['avro']['patterns']
-NON_RULE_PATTERNS = [p for p in PATTERNS if 'rules' not in p]
-RULE_PATTERNS = [p for p in PATTERNS if 'rules' in p]
+PATTERNS = config.DICT["avro"]["patterns"]
+NON_RULE_PATTERNS = [p for p in PATTERNS if "rules" not in p]
+RULE_PATTERNS = [p for p in PATTERNS if "rules" in p]
 
 
 # The helper function for handling multithreaded workloads.
 def _concurrency_helper(func: Callable, params: Tuple[str]) -> List[str]:
     output = []
 
     with ThreadPoolExecutor() as executor:
@@ -49,15 +49,15 @@
 
     parsed = avro.parse('ami banglay gan gai')
     print(parsed)
     ```
     """
 
     # Compiled regular expression for UTF-8 validation
-    utf8_regex = re.compile(r'\A[\x00-\x7F]*\Z')
+    utf8_regex = re.compile(r"\A[\x00-\x7F]*\Z")
 
     @lru_cache
     def _parse_backend(text: str) -> str:
         fixed_text = validate.fix_string_case(text)  # Sanitize input text.
         cur_end = 0  # Cursor end point.
 
         def output_generator() -> Generator[str, None, None]:
@@ -69,39 +69,39 @@
 
                 if not uni_pass:
                     cur_end = cur + 1
                     yield i
 
                 elif cur >= cur_end and uni_pass:
                     match = _match_patterns(fixed_text, cur, rule=False)
-                    matched = match['matched']
+                    matched = match["matched"]
 
                     if matched:
-                        yield match['replaced']
-                        cur_end = cur + len(match['found'])
+                        yield match["replaced"]
+                        cur_end = cur + len(match["found"])
                     else:
                         match = _match_patterns(fixed_text, cur, rule=True)
-                        matched = match['matched']
+                        matched = match["matched"]
 
                         if matched:
-                            cur_end = cur + len(match['found'])
+                            cur_end = cur + len(match["found"])
                             replaced = _process_rules(
-                                rules=match['rules'], fixed_text=fixed_text, cur=cur, cur_end=cur_end
+                                rules=match["rules"], fixed_text=fixed_text, cur=cur, cur_end=cur_end
                             )
 
                             if replaced:
                                 yield replaced
                             else:
-                                yield match['replaced']
+                                yield match["replaced"]
 
                     if not matched:
                         cur_end = cur + 1
                         yield i
 
-        return ''.join(chain.from_iterable(output_generator()))
+        return "".join(chain.from_iterable(output_generator()))
 
     output = _concurrency_helper(_parse_backend, texts)
 
     # If the `bijoy` parameter is set to `True`, then convert the output to Bijoy Keyboard format.
     if bijoy:
         return to_bijoy(*output)
     else:
@@ -124,15 +124,15 @@
     converted = avro.to_bijoy('আমার সোনার বাংলা')
     print(converted)
     ```
     """
 
     @lru_cache
     def _convert_backend(text: str) -> str:
-        text = _rearrange_unicode_text(re.sub('ৌ', 'ৌ', re.sub('ো', 'ো', text)))
+        text = _rearrange_unicode_text(re.sub("ৌ", "ৌ", re.sub("ো", "ো", text)))
 
         for unic in config.BIJOY_MAP:
             text = re.sub(unic, config.BIJOY_MAP[unic], text)
 
         return text.strip()
 
     output = _concurrency_helper(_convert_backend, texts)
@@ -162,39 +162,39 @@
     @lru_cache
     def _reverse_backend(text: str) -> str:
         output = []  # The output list of strings.
 
         # Iterate through input text.
         for cur, i in enumerate(text):
             try:
-                i.encode('utf-8')
+                i.encode("utf-8")
                 match = _match_patterns(text, cur, rule=False, reversed=True)
 
-                if match['matched']:
-                    output.append(match['reversed'] if match['reversed'] else match['found'])
+                if match["matched"]:
+                    output.append(match["reversed"] if match["reversed"] else match["found"])
                 else:
                     output.append(i)
 
             except UnicodeDecodeError:
                 output.append(i)
 
-        return ''.join(output)
+        return "".join(output)
 
     # Split using regex to remove noise.
     compiled_regex = re.compile("(\\s|\\.|,|\\?|\\।|\\-|;|')", re.UNICODE)
 
     # Extension for the _reverse_backend() function.
     @lru_cache
     def _reverse_backend_ext(text: str) -> str:
         exceptions = config.AVRO_EXCEPTIONS.get(text, None)
 
         if not exceptions:
             separated_texts = compiled_regex.split(text)
             text_segments = [_reverse_backend(separated_text) for separated_text in separated_texts]
-            return ''.join(text_segments)
+            return "".join(text_segments)
         else:
             return exceptions
 
     # Prepare final output.
     output = _concurrency_helper(_reverse_backend_ext, texts)
     return output[0] if len(output) == 1 else output
 
@@ -221,15 +221,15 @@
 
             chars[i - j], chars[i] = chars[i], chars[i - j]
             barrier = i + 1
 
         if (
             i < length - 1
             and validate.is_bangla_halant(chars[i])
-            and chars[i - 1] == 'র'
+            and chars[i - 1] == "র"
             and not validate.is_bangla_halant(chars[i - 2])
         ):
             j = 1
             found_pre_kar = 0
 
             while True:
                 if validate.is_bangla_banjonborno(chars[i + j]) and validate.is_bangla_halant(
@@ -250,15 +250,15 @@
                 chars[i - 1],
                 chars[i],
                 chars[i + j + found_pre_kar + 1 :],
             )
             i += j + found_pre_kar
             barrier = i + 1
 
-    return ''.join(chars)
+    return "".join(chars)
 
 
 def _match_patterns(
     fixed_text: str, cur: int = 0, rule: bool = False, reversed: bool = False
 ) -> Dict[str, Any]:
     """
     Matches given text at cursor position with rule / non rule patterns.
@@ -269,73 +269,73 @@
     rule_type = NON_RULE_PATTERNS if not rule else RULE_PATTERNS
     pattern = _exact_find_in_pattern(fixed_text, reversed, cur, rule_type)
 
     if pattern:
         p = pattern[0]
 
         return {
-            'matched': True,
-            'found': p.get('find'),
-            'replaced': p.get('replace'),
-            'reversed': _reverse_with_rules(cur, fixed_text, p.get('reverse')) if not rule else None,
-            'rules': p.get('rules') if rule else None,
+            "matched": True,
+            "found": p.get("find"),
+            "replaced": p.get("replace"),
+            "reversed": _reverse_with_rules(cur, fixed_text, p.get("reverse")) if not rule else None,
+            "rules": p.get("rules") if rule else None,
         }
 
     return {
-        'matched': False,
-        'found': None,
-        'replaced': fixed_text[cur],
-        'rules': None if rule else None,
+        "matched": False,
+        "found": None,
+        "replaced": fixed_text[cur],
+        "rules": None if rule else None,
     }
 
 
 def _exact_find_in_pattern(
     fixed_text: str, reversed: bool, cur: int = 0, patterns: Any = PATTERNS
 ) -> List[Dict[str, Any]]:
     """
     Returns pattern items that match given text, cursor position and pattern.
     """
 
     if reversed:
         return [
             x
             for x in patterns
-            if (cur + len(x['replace']) <= len(fixed_text))
-            and x['replace'] == fixed_text[cur : (cur + len(x['replace']))]
+            if (cur + len(x["replace"]) <= len(fixed_text))
+            and x["replace"] == fixed_text[cur : (cur + len(x["replace"]))]
         ]
 
     return [
         x
         for x in patterns
-        if x.get('find', None)
-        and (cur + len(x['find']) <= len(fixed_text))
-        and x['find'] == fixed_text[cur : (cur + len(x['find']))]
+        if x.get("find", None)
+        and (cur + len(x["find"]) <= len(fixed_text))
+        and x["find"] == fixed_text[cur : (cur + len(x["find"]))]
     ]
 
 
 def _reverse_with_rules(cursor: int, fixed_text: str, text_reversed: str) -> str:
     """
     Enhances the word with rules for reverse-parsing.
     """
 
-    added_suffix = ''
+    added_suffix = ""
 
     if not (
         fixed_text[cursor] in config.AVRO_KAR
         or fixed_text[cursor] in config.AVRO_SHORBORNO
         or fixed_text[cursor] in config.AVRO_IGNORE
         or len(fixed_text) == cursor + 1
     ):
-        added_suffix = 'o'
+        added_suffix = "o"
 
     try:
         if (fixed_text[cursor + 1] in config.AVRO_KAR) or (
             fixed_text[cursor + 2] in config.AVRO_KAR and not cursor == 0
         ):
-            added_suffix = ''
+            added_suffix = ""
 
     except IndexError:
         pass
 
     return text_reversed if not text_reversed else text_reversed + added_suffix
 
 
@@ -343,95 +343,95 @@
     """
     Process rules matched in pattern and returns suitable replacement.
 
     If any rule's condition is satisfied, output the rules "replace",
     else output None.
     """
 
-    replaced = ''
+    replaced = ""
 
     # Iterate through rules.
     for rule in rules:
         matched = False
 
-        for match in rule['matches']:
+        for match in rule["matches"]:
             matched = _process_match(match, fixed_text, cur, cur_end)
 
             if not matched:
                 break
 
         if matched:
-            replaced = rule['replace']
+            replaced = rule["replace"]
             break
 
     return replaced if matched else None
 
 
 def _process_match(match: Any, fixed_text: str, cur: int, cur_end: int) -> bool:
     """
     Processes a single match in rules.
     """
 
     # Initial/default value for replace.
     replace = True
 
     # Set check cursor depending on match['type']
-    chk = cur - 1 if match['type'] == 'prefix' else cur_end
+    chk = cur - 1 if match["type"] == "prefix" else cur_end
 
     # Set scope based on whether scope is negative.
-    if match['scope'].startswith('!'):
-        scope = match['scope'][1:]
+    if match["scope"].startswith("!"):
+        scope = match["scope"][1:]
         negative = True
     else:
-        scope = match['scope']
+        scope = match["scope"]
         negative = False
 
     # Let the matching begin!
-    if scope == 'punctuation':
+    if scope == "punctuation":
         if (
             not (
-                (chk < 0 and match['type'] == 'prefix')
-                or (chk >= len(fixed_text) and match['type'] == 'suffix')
+                (chk < 0 and match["type"] == "prefix")
+                or (chk >= len(fixed_text) and match["type"] == "suffix")
                 or validate.is_punctuation(fixed_text[chk])
             )
             != negative
         ):
             replace = False
 
-    elif scope == 'vowel':
+    elif scope == "vowel":
         if (
             not (
                 (
-                    (chk >= 0 and match['type'] == 'prefix')
-                    or (chk < len(fixed_text) and match['type'] == 'suffix')
+                    (chk >= 0 and match["type"] == "prefix")
+                    or (chk < len(fixed_text) and match["type"] == "suffix")
                 )
                 and validate.is_vowel(fixed_text[chk])
             )
             != negative
         ):
             replace = False
 
-    elif scope == 'consonant':
+    elif scope == "consonant":
         if (
             not (
                 (
-                    (chk >= 0 and match['type'] == 'prefix')
-                    or (chk < len(fixed_text) and match['type'] == 'suffix')
+                    (chk >= 0 and match["type"] == "prefix")
+                    or (chk < len(fixed_text) and match["type"] == "suffix")
                 )
                 and validate.is_consonant(fixed_text[chk])
             )
             != negative
         ):
             replace = False
 
-    elif scope == 'exact':
-        if match['type'] == 'prefix':
-            exact_start = cur - len(match['value'])
+    elif scope == "exact":
+        if match["type"] == "prefix":
+            exact_start = cur - len(match["value"])
             exact_end = cur
         else:
             exact_start = cur_end
-            exact_end = cur_end + len(match['value'])
+            exact_end = cur_end + len(match["value"])
 
-        if not validate.is_exact(match['value'], fixed_text, exact_start, exact_end, negative):
+        if not validate.is_exact(match["value"], fixed_text, exact_start, exact_end, negative):
             replace = False
 
     return replace
```

### Comparing `avro.py-2024.4.7/avro/utils/validate.py` & `avro_py-2024.5.1/avro/utils/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,23 +61,16 @@
 
     Case-sensitive characters as defined in config.AVRO_CASESENSITIVES
     retain their case, but others are converted to their lowercase
     equivalents. The result is a string with phonetic-compatible case
     which will the parser will understand without confusion.
     """
 
-    fixed = []
-
-    for i in text:
-        if is_case_sensitive(i):
-            fixed.append(i)
-        else:
-            fixed.append(i.lower())
-
-    return ''.join(fixed)
+    fixed = [i if is_case_sensitive(i) else i.lower() for i in text]
+    return "".join(fixed)
 
 
 # ASCII-specific validation functions.
 # These are used for validating output while converting to ASCII after the initial conversion.
 def is_bangla_prekar(char: str) -> bool:
     """
     Check if given character is a Bengali pre-kar.
@@ -95,8 +88,8 @@
 
 
 def is_bangla_halant(char: str) -> bool:
     """
     Check if given character is a Bengali halant.
     """
 
-    return char == config.BIJOY_EXCEPTIONS['halant']
+    return char == config.BIJOY_EXCEPTIONS["halant"]
```

