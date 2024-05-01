# Comparing `tmp/cs3560-grading-lib-0.1.0rc2.tar.gz` & `tmp/cs3560_grading_lib-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs3560-grading-lib-0.1.0rc2.tar", last modified: Thu Feb 29 11:53:46 2024, max compression
+gzip compressed data, was "cs3560_grading_lib-0.1.1a2.tar", last modified: Wed May  1 14:20:32 2024, max compression
```

## Comparing `cs3560-grading-lib-0.1.0rc2.tar` & `cs3560_grading_lib-0.1.1a2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-29 11:53:46.000000 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-29 11:53:46.000000 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:53:46.000000 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-29 11:53:46.000000 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 11:53:46.000000 cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/grading_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/grading_lib/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/cli/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/grading_lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/tools/collect_autograding_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/grading_lib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:53:46.022301 cs3560-grading-lib-0.1.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/tests/test_makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 11:53:38.000000 cs3560-grading-lib-0.1.0rc2/tests/test_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-01 14:20:32.000000 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-01 14:20:32.000000 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:20:32.000000 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 14:20:32.000000 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 14:20:32.000000 cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/grading_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/grading_lib/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/cli/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/grading_lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/tools/collect_autograding_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/grading_lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:20:32.062548 cs3560_grading_lib-0.1.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-01 14:20:28.000000 cs3560_grading_lib-0.1.1a2/tests/test_makefile.py
```

### Comparing `cs3560-grading-lib-0.1.0rc2/LICENSE` & `cs3560_grading_lib-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cs3560-grading-lib-0.1.0rc2/PKG-INFO` & `cs3560_grading_lib-0.1.1a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs3560-grading-lib
-Version: 0.1.0rc2
+Version: 0.1.1a2
 Summary: A common library for the grading scripts.
 License: MIT License
         
         Copyright (c) 2024 OU-CS3560
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +21,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://grading-lib.readthedocs.io/en/latest/
-Project-URL: Homepage, https://github.com/OU-CS3560/cs3560-grading-lib
-Project-URL: Repository, https://github.com/OU-CS3560/cs3560-grading-lib.git
-Project-URL: Issues, https://github.com/OU-CS3560/cs3560-grading-lib/issues
+Project-URL: Source Code, https://github.com/OU-CS3560/cs3560-grading-lib
+Project-URL: Issue Tracker, https://github.com/OU-CS3560/cs3560-grading-lib/issues
 Project-URL: Changelog, https://github.com/OU-CS3560/cs3560-grading-lib/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
@@ -42,19 +41,16 @@
 Requires-Dist: tomli
 Requires-Dist: GitPython
 Requires-Dist: importlib-metadata; python_version >= "3.10"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Provides-Extra: doc
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
-Requires-Dist: sphinx-book-theme; extra == "doc"
-Requires-Dist: sphinx-autodoc2; extra == "doc"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # cs3560's grading-lib
 
 A common library for the grading scripts.
 
 ## Install
 
@@ -65,15 +61,15 @@
 ## Features
 
 - Base class for a test case.
 - Utilities functions to grade make related problems.
 
 ## Documentation
 
-View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/)
+View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/) or the documentation for the [stable version](https://grading-lib.readthedocs.io/en/stable/).
 
 ## Similar Projects / More Mature Projects
 
 If you are looking for a more mature projects, please see
 
 - [OK](https://okpy.org/) which is used in [CS 61A](https://cs61a.org/) at University of California, Berkeley. It implements the concept of
   "test case unlocking" that promotes "multi-stage problem solving process." [paper](http://denero.org/content/pubs/las15_basu_unlocking.pdf).
```

### Comparing `cs3560-grading-lib-0.1.0rc2/README.md` & `cs3560_grading_lib-0.1.1a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## Features
 
 - Base class for a test case.
 - Utilities functions to grade make related problems.
 
 ## Documentation
 
-View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/)
+View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/) or the documentation for the [stable version](https://grading-lib.readthedocs.io/en/stable/).
 
 ## Similar Projects / More Mature Projects
 
 If you are looking for a more mature projects, please see
 
 - [OK](https://okpy.org/) which is used in [CS 61A](https://cs61a.org/) at University of California, Berkeley. It implements the concept of
   "test case unlocking" that promotes "multi-stage problem solving process." [paper](http://denero.org/content/pubs/las15_basu_unlocking.pdf).
```

### Comparing `cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/PKG-INFO` & `cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs3560-grading-lib
-Version: 0.1.0rc2
+Version: 0.1.1a2
 Summary: A common library for the grading scripts.
 License: MIT License
         
         Copyright (c) 2024 OU-CS3560
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +21,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://grading-lib.readthedocs.io/en/latest/
-Project-URL: Homepage, https://github.com/OU-CS3560/cs3560-grading-lib
-Project-URL: Repository, https://github.com/OU-CS3560/cs3560-grading-lib.git
-Project-URL: Issues, https://github.com/OU-CS3560/cs3560-grading-lib/issues
+Project-URL: Source Code, https://github.com/OU-CS3560/cs3560-grading-lib
+Project-URL: Issue Tracker, https://github.com/OU-CS3560/cs3560-grading-lib/issues
 Project-URL: Changelog, https://github.com/OU-CS3560/cs3560-grading-lib/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
@@ -42,19 +41,16 @@
 Requires-Dist: tomli
 Requires-Dist: GitPython
 Requires-Dist: importlib-metadata; python_version >= "3.10"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Provides-Extra: doc
-Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
-Requires-Dist: sphinx-book-theme; extra == "doc"
-Requires-Dist: sphinx-autodoc2; extra == "doc"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # cs3560's grading-lib
 
 A common library for the grading scripts.
 
 ## Install
 
@@ -65,15 +61,15 @@
 ## Features
 
 - Base class for a test case.
 - Utilities functions to grade make related problems.
 
 ## Documentation
 
-View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/)
+View the [latest documentation](https://grading-lib.readthedocs.io/en/latest/) or the documentation for the [stable version](https://grading-lib.readthedocs.io/en/stable/).
 
 ## Similar Projects / More Mature Projects
 
 If you are looking for a more mature projects, please see
 
 - [OK](https://okpy.org/) which is used in [CS 61A](https://cs61a.org/) at University of California, Berkeley. It implements the concept of
   "test case unlocking" that promotes "multi-stage problem solving process." [paper](http://denero.org/content/pubs/las15_basu_unlocking.pdf).
```

### Comparing `cs3560-grading-lib-0.1.0rc2/cs3560_grading_lib.egg-info/SOURCES.txt` & `cs3560_grading_lib-0.1.1a2/cs3560_grading_lib.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 grading_lib/repository.py
 grading_lib/util.py
 grading_lib/cli/__init__.py
 grading_lib/cli/dev.py
 grading_lib/cli/internal.py
 grading_lib/tools/__init__.py
 grading_lib/tools/collect_autograding_tests.py
+tests/test_cli.py
 tests/test_common.py
-tests/test_makefile.py
-tests/test_repository.py
+tests/test_makefile.py
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/__init__.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/cli/__init__.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from ..util import get_problem_total_points, load_problems_metadata
 from .dev import dev
 from .internal import internal
 
 
 @click.group()
-def cli():
+def cli() -> None:
     pass
 
 
 @cli.command(name="help")
 @click.pass_context
-def show_help(ctx):
+def show_help(ctx: click.Context) -> None:
     """Show this help messages."""
     click.echo(cli.get_help(ctx))
 
 
 @cli.command(name="summary")
 def summary_command() -> None:
     """
@@ -27,15 +27,15 @@
     problem_points: list[float] = []
     for problem in problems:
         problem_points.append(get_problem_total_points(problem))
 
     total_points = sum(problem_points)
     print(f"Problem Count: {len(problems)}")
     print(f"Total Points: {total_points:.2f}")
-    for problem, points in zip(problems, problem_points):
+    for problem, points in zip(problems, problem_points, strict=False):
         name = problem["problem"]["name"]
         score_section = f"{points:.2f} / {total_points:.2f}"
         print(f" - {name:<40} {score_section:>20}")
 
 
 cli.add_command(dev)
 cli.add_command(internal)
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/cli/dev.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/cli/dev.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import click
 
 from ..util import load_problems_metadata
 
 
 @click.group()
-def dev():
+def dev() -> None:
     """Grading script's development related commands."""
     pass
 
 
 @dev.command(name="mypy")
-def run_mypy_command():
+def run_mypy_command() -> None:
     """
     Run mypy on each problem's scripts/ individually.
 
     If mypy is run on the template's root. It will complain saying that
     there are multiple grade.py module.
     """
     problems = load_problems_metadata()
     for metadata in problems:
         target_dir = Path(".") / metadata["problem"]["name"] / "scripts"
-        click.echo(f"Running mypy for {str(target_dir)} ...")
+        click.echo(f"Running mypy for {target_dir!s} ...")
         subprocess.run([sys.executable, "-m", "mypy", target_dir])
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/cli/internal.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/cli/internal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 import json
-import os
 from pathlib import Path
 
 import click
 import tomli
 
 
 @click.group()
-def internal():
+def internal() -> None:
     """
     Commands that are not meant for user's direct use.
 
     These commands are menat to be used by CI or to facilitate a step
     in CI.
     """
     pass
 
 
 @internal.command(name="collect-autograding-tests")
-@click.argument("src_dir", required=False, default=os.getcwd())
+@click.argument("src_dir", required=False, default=".")
 @click.option("--out-dir", default=Path(".") / ".github" / "classroom")
-def collect_autograding_tests_command(src_dir, out_dir):
+@click.pass_context
+def collect_autograding_tests_command(
+    ctx: click.Context, src_dir: str | Path, out_dir: str | Path
+) -> None:
     """
     Collect all test cases and put them in .github/classroom/autograding.json.
 
     This is meant to be used by the GitHub Action's workflow.
     """
     if isinstance(src_dir, str):
         src_dir = Path(src_dir)
 
     if not src_dir.exists():
-        print(f"[error]: target directory '{str(src_dir)}' does not exist")
-        click.exit(1)
+        print(f"[error]: target directory '{src_dir!s}' does not exist")
+        ctx.exit(1)
 
     if isinstance(out_dir, str):
         out_dir = Path(out_dir)
 
     out_dir.mkdir(parents=True, exist_ok=True)
 
     tests = []
     for problem_file_path in src_dir.glob("*/problem.toml"):
         print(f"processing {problem_file_path}")
         with open(problem_file_path, "rb") as in_file:
             data = tomli.load(in_file)
             problem_name = data["problem"]["name"]
 
             if "tests" in data["problem"]:
-                for key, data in data["problem"]["tests"].items():
+                for _, test_data in data["problem"]["tests"].items():
                     # Modify the run command by preprend it with the
                     # cd command.
                     test = dict()
-                    test.update(data)
+                    test.update(test_data)
                     test["name"] = f"{problem_name} - {test['name']}"
                     if len(test["run"].strip()) != 0:
                         test["run"] = f"cd {problem_name} && {test['run']}"
 
                     tests.append(test)
             else:
                 print(
-                    " - warning: No test cases found. They may be hidden from the students or not yet implemented."
+                    " - warning: No test cases found. They may be hidden from the "
+                    "students or not yet implemented."
                 )
 
     autograding_filepath = out_dir / "autograding.json"
     with open(autograding_filepath, "w") as out_file:
         json.dump({"tests": tests}, out_file, indent=2)
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/common.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import datetime
 import os
-import random
 import subprocess
+import sys
 import tempfile
 import time
 import unittest
 from collections import namedtuple
 from pathlib import Path
-from typing import Optional
+from typing import Any, TypeVar
+
+T = TypeVar("T")
 
 COMMAND_FAILED_TEXT_TEMPLATE = "An error occurred while trying to run a command '{command}'. The command's output is\n\n{output}"
 FILE_NOT_EXIST_TEXT_TEMPLATE = "File '{path}' does not exist"
 DEFAULT_FILENAME_POOL = ["main.cpp", "file.txt"]
 FILE_SUFFIX_POOL = [".cpp", ".txt", ".md", ".zip", ".py", ".toml", ".yml", ".yaml"]
 NAME_POOL = ["herta", "cat", "dog", "dolphin", "falcon", "dandilion", "fox", "jett"]
 
 
 def is_debug_mode(
     variable_name: str = "DEBUG",
-    vals_for_true: list[str] = ["true", "t", "on", "1"],
+    vals_for_true: tuple[str, ...] = ("true", "t", "on", "1"),
 ) -> bool:
     """Return True if the DEBUG envrionment variable is presence with value representing 'True'."""
     raw_val = os.environ.get(variable_name, None)
 
     if raw_val is not None:
         val = raw_val.strip().lower()
         return val in vals_for_true
@@ -33,15 +35,15 @@
     raw_val = os.environ.get(variable_name, None)
     # The test case is done too quickly to use second.
     seed_val = int(time.time() * 1000.0)
 
     if raw_val is not None:
         try:
             seed_val = int(raw_val)
-        except:
+        except ValueError:
             pass
 
     return seed_val
 
 
 def get_mtime_as_datetime(path: Path | str) -> datetime.datetime:
     if isinstance(path, str):
@@ -53,15 +55,15 @@
 
 
 def has_file_changed(last_known_mtime: datetime.datetime, path: Path | str) -> bool:
     new_mtime = get_mtime_as_datetime(path)
     return new_mtime > last_known_mtime
 
 
-def populate_folder_with_filenames(path: Path | str, filnames: list[str]):
+def populate_folder_with_filenames(path: Path | str, filnames: list[str]) -> None:
     if isinstance(path, str):
         path = Path(path)
     if not path.exists():
         raise ValueError("'path' does not exist")
     if not path.is_dir():
         raise ValueError("'path' is not a directory")
 
@@ -69,63 +71,77 @@
         with open(path / name, "w") as f:
             f.write("")
 
 
 CommandResult = namedtuple("CommandResult", ["success", "command", "output"])
 
 
-def run_executable(args, cwd: Optional[str | Path] = None) -> CommandResult:
+def run_executable(
+    args: list[str], cwd: str | Path | None = None, timeout: float = 15.0
+) -> CommandResult:
     """
     Run a command at the cwd.
 
     Return
     - (True, command, output) when the command completes without any error.
     - (False, command, output) when the command completes with error.
 
     It will redirect stderr to stdout and capture stdout as output.
     """
     try:
         make_cmd_output = subprocess.check_output(
-            args, stderr=subprocess.STDOUT, cwd=cwd
+            args, stderr=subprocess.STDOUT, cwd=cwd, timeout=timeout
         )
         return CommandResult(True, " ".join(args), make_cmd_output.decode())
     except subprocess.CalledProcessError as e:
         return CommandResult(False, " ".join(args), e.output.decode())
+    except subprocess.TimeoutExpired as e:
+        return CommandResult(False, " ".join(args), e.output.decode())
+
+
+def ensure_lf_line_ending(path: Path | str) -> CommandResult:
+    """Run dos2unix on the file at path.
+
+    Students who are using Windows OS may submit answer.sh that has CRLF as its line
+    ending. The CR will ofen get mixed into shell commands in the file and produces
+    strange result / error.
+    """
+    return run_executable(["dos2unix", str(path)])
 
 
 class MinimalistTestResult(unittest.TextTestResult):
     """TextTestResult without the traceback.
 
     Traceback is too verbose for our purpose.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.dots = False
 
-    def getDescription(self, test):
+    def getDescription(self, test: unittest.TestCase) -> str:
         doc_first_line = test.shortDescription()
         if self.descriptions and doc_first_line:
             return doc_first_line
         else:
             return str(test)
 
-    def addFailure(self, test, err):
+    def addFailure(self, test: unittest.TestCase, err) -> None:
         self.failures.append((test, str(err[1]) + "\n"))
         self._mirrorOutput = True
 
         if self.showAll:
             self._write_status(test, "FAIL")
         elif self.dots:
             self.stream.write("F")
             self.stream.flush()
 
 
 class BaseTestCaseMeta(type):
-    def __new__(cls, name: str, bases, attrs: dict):
+    def __new__(cls: T, name: str, bases: list[Any], attrs: dict[str, Any]) -> T:
         if "with_temporary_dir" not in attrs:
             attrs["with_temporary_dir"] = False
 
         o = super().__new__(cls, name, bases, attrs)
         return o
 
 
@@ -134,44 +150,63 @@
     A base class for test case.
 
     :cvar with_temporary_dir: When `True`, create a temporary directory for each test.
     """
 
     with_temporary_dir: bool  # Added by metaclass.
 
-    def setUp(self):
+    def setUp(self) -> None:
         self.is_debug_mode = is_debug_mode()
         self.seed = get_seed_from_env()
 
         self.temporary_dir = None
         if self.with_temporary_dir:
-            self.temporary_dir = tempfile.TemporaryDirectory(dir=Path("."))
+            if sys.version_info < (3, 12, 0):
+                self.temporary_dir = tempfile.TemporaryDirectory(dir=Path("."))
+            else:
+                self.temporary_dir = tempfile.TemporaryDirectory(
+                    dir=Path("."), delete=False
+                )
             self.temporary_dir_path = Path(self.temporary_dir.name)
 
     def tearDown(self) -> None:
-        if not self.is_debug_mode and self.with_temporary_dir:
+        if not self.is_debug_mode and self.temporary_dir is not None:
             self.temporary_dir.cleanup()
+        elif self.is_debug_mode and self.temporary_dir is not None:
+            print(
+                f"[info]: The temporary directory at '{self.temporary_dir_path}' is not deleted since the DEBUG is set to True."
+            )
+
+    def assertArchiveFileIsGzip(self, path: Path):
+        cmd_result = run_executable(["gunzip", "-t", str(path)])
+        self.assertTrue(
+            "not in gzip format" not in cmd_result.output,
+            msg="Hint: Did you forget to use '-z' flag when creating the archive?",
+        )
+        self.assertCommandSuccessful(
+            cmd_result,
+        )
 
     def assertFileExists(
         self, path: Path, msg_template: str = FILE_NOT_EXIST_TEXT_TEMPLATE
     ) -> None:
         """Pass if the file at `path` exist."""
         if not path.exists():
             msg = msg_template.format(path=str(path))
             raise self.failureException(msg)
 
-    def assertAllFilesExist(self, paths: list[Path], msg=None) -> None:
+    def assertAllFilesExist(self, paths: list[Path], msg: str | None = None) -> None:
         """Pass if all the listed files exist."""
         not_exist: list[Path] = []
         for path in paths:
             if not path.exists():
                 not_exist.append(path)
             elif not path.is_file():
                 raise self.failureException(
-                    f"Expect a file, but '{str(path)}' is not a file."
+                    f"Expect a file, but '{path!s}' is not a file."
                 )
 
         if len(not_exist) != 0:
             path_strs = [str(p) for p in paths]
             not_exist_strs = [str(p) for p in not_exist]
             if msg is None:
                 if len(path_strs) == len(not_exist_strs):
@@ -187,15 +222,15 @@
     ) -> None:
         """Pass if the command run successfully."""
         if not result.success:
             msg = msg_template.format(command=result.command, output=result.output)
             raise self.failureException(msg)
 
     def assertCommandOutputEqual(
-        self, result: CommandResult, expected_output: str, msg: Optional[str] = None
+        self, result: CommandResult, expected_output: str, msg: str | None = None
     ) -> None:
         """
         Pass if the command's output is equal to `output`.
 
         The `msg` will be formatted with  `command`, `expected_output`, `output`
         """
         if result.output != expected_output:
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/makefile.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/makefile.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 
 from __future__ import annotations
 
 import re
 import shutil
 from pathlib import Path
-from typing import Optional
 
 from .common import BaseTestCase, CommandResult, is_debug_mode, run_executable
 
 RULE_PATTERN = re.compile(
     r"(?P<targets>[\w\.\-%$()\ +]+):(?!=|:=|::=)(?P<prereqs>[\w\.\-%$()\ +]*)"
 )
 
@@ -26,23 +25,26 @@
 # Thus, parsing variable definition is dropped in v0.0.3
 VAR_DEF_PATTERN = re.compile(r"(?P<name>[\w\.-]+)\s*(:*|\?|!|\+)?=\s*(?P<value>.*)")
 
 
 def run_targets(
     targets: list[str],
     makefile_name: str = "answer.mk",
-    cwd: Optional[str | Path] = None,
+    cwd: str | Path | None = None,
+    timeout: float = 15.0,
 ) -> CommandResult:
     """
     Invoke the target(s) in the Makefile.
 
     Return True if the call is successful, False otherwise.
     Also return the output of the executation.
     """
-    return run_executable(["make", "-f", makefile_name] + targets, cwd=cwd)
+    return run_executable(
+        ["make", "-f", makefile_name, *targets], cwd=cwd, timeout=timeout
+    )
 
 
 class Rule:
     def __init__(
         self, targets: str | list[str], prerequisites: list[str], recipe: list[str]
     ):
         self.targets = targets
@@ -89,26 +91,26 @@
         rules: list[Rule],
     ):
         self.path = path
         self.rules = rules
 
     @classmethod
     def from_path(cls, path: Path | str) -> Makefile:
-        with open(path, "r") as f:
+        with open(path) as f:
             content = f.read()
             return cls.from_text(content)
 
     @classmethod
-    def from_text(cls, text: str):
+    def from_text(cls, text: str) -> Makefile:
         DEBUG: bool = is_debug_mode()
 
         rules: list[Rule] = []
 
-        lines = [l.replace("\r", "") for l in text.split("\n")]
-        current_rule: Optional[Rule] = None
+        lines = [line.replace("\r", "") for line in text.split("\n")]
+        current_rule: Rule | None = None
         for line in lines:
             line = line.strip()
 
             if DEBUG:
                 print(f"parsing '{line}'")
 
             if len(line.strip()) != 0:
@@ -155,15 +157,15 @@
                     rules.append(current_rule)
                     current_rule = None
 
         if current_rule is not None:
             rules.append(current_rule)
         return cls("memory://Makefile", rules)
 
-    def get_rule(self, targets: str | list[str]) -> Optional[Rule]:
+    def get_rule(self, targets: str | list[str]) -> Rule | None:
         for rule in self.rules:
             if rule.targets == targets:
                 return rule
 
         return None
 
     def has_rule(self, targets: str | list[str]) -> bool:
@@ -179,48 +181,47 @@
     def setUpClass(cls) -> None:
         if not hasattr(cls, "makefile_path"):
             raise AttributeError("'makefile_path' is required")
 
         if isinstance(cls.makefile_path, str):
             cls.makefile_path = Path(cls.makefile_path)
 
-        if not cls.makefile_path.exists():
-            assert False, f"Expect a file '{cls.makefile_path}', but it does not exist."
+        assert (
+            not cls.makefile_path.exists()
+        ), f"Expect a file '{cls.makefile_path}', but it does not exist."
 
         cls.makefile = Makefile.from_path(cls.makefile_path)
 
     def copy_makefile(
-        self, dest: Optional[Path] = None, as_name: str = "answer.mk"
+        self, dest: Path | None = None, as_name: str = "answer.mk"
     ) -> None:
         """Copy the student's Makefile.
 
         When `dest` is `None`, make a copy of the student's Makefile in the same folder but
         with the name `answer.mk`.
         """
         shutil.copy(self.makefile_path, self.temporary_dir_path / as_name)
 
     def assertHasRuleForTarget(
         self,
         target_name: str,
         msg_template: str = "Rule for a target '{target_name}' does not exist. Its behavior cannot be verified.",
-    ):
+    ) -> None:
         """
         The Makefile must have target `target_name`.
         """
         if not self.makefile.has_rule(target_name):
             msg = msg_template.format(target_name=target_name)
             raise self.failureException(msg)
 
     def assertRuleRecipeIsEmpty(
         self,
         target_name: str,
         msg_template: str = "Recipe of the rule for a target '{target_name}' is not empty.",
-    ):
+    ) -> None:
         rule = self.makefile.get_rule(target_name)
         if rule is None:
-            msg = "Rule for a target '{target_name}' does not exist. Its behavior cannot be verified.".format(
-                target_name=target_name
-            )
+            msg = f"Rule for a target '{target_name}' does not exist. Its behavior cannot be verified."
             raise self.failureException(msg)
         if not rule.is_empty():
             msg = msg_template.format(target_name=target_name)
             raise self.failureException(msg)
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/tools/collect_autograding_tests.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/tools/collect_autograding_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 that we can add or remove them as we please.
 """
 
 import json
 import os
 import sys
 import warnings
+from argparse import Namespace
 from pathlib import Path
 
 import tomli
 
 
-def main(args):
+def main(args: Namespace) -> None:
     warnings.warn(
         "This is depreated in the favor of cli module", DeprecationWarning, stacklevel=2
     )
     target_dir = args.dir
     if isinstance(target_dir, str):
         target_dir = Path(target_dir)
 
     if not target_dir.exists():
-        print(f"[error]: target directory '{str(target_dir)}' does not exist")
+        print(f"[error]: target directory '{target_dir!s}' does not exist")
         sys.exit(1)
 
     out_dir = args.out_dir
     if isinstance(out_dir, str):
         out_dir = Path(out_dir)
 
     out_dir.mkdir(parents=True, exist_ok=True)
 
     tests = []
     for problem_file_path in target_dir.glob("*/problem.toml"):
         print(f"processing {problem_file_path}")
         with open(problem_file_path, "rb") as in_file:
             data = tomli.load(in_file)
             problem_name = data["problem"]["name"]
-            for key, data in data["problem"]["tests"].items():
+            for _, test_entry in data["problem"]["tests"].items():
                 # Modify the run command by preprend it with the
                 # cd command.
                 test = dict()
-                test.update(data)
+                test.update(test_entry)
                 test["name"] = f"{problem_name} - {test['name']}"
                 if len(test["run"].strip()) != 0:
                     test["run"] = f"cd {problem_name} && {test['run']}"
 
                 tests.append(test)
 
     autograding_filepath = out_dir / "autograding.json"
```

### Comparing `cs3560-grading-lib-0.1.0rc2/grading_lib/util.py` & `cs3560_grading_lib-0.1.1a2/grading_lib/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
+from typing import Any
 
 import tomli
 
 
-def load_problems_metadata(path=Path(".")) -> list[dict]:
+def load_problems_metadata(path: Path = Path(".")) -> list[dict[str, Any]]:
     """Parse all problem.toml of problems."""
-    problems: list[dict] = []
+    problems: list[dict[str, Any]] = []
     for problem_file_path in path.glob("*/problem.toml"):
         with open(problem_file_path, "rb") as in_file:
             data = tomli.load(in_file)
             problems.append(data)
     return problems
 
 
-def get_problem_total_points(problem: dict) -> float:
+def get_problem_total_points(problem: dict[str, Any]) -> float:
     total_points = 0.0
 
     if "tests" not in problem["problem"]:
         return total_points
 
-    for key, test in problem["problem"]["tests"].items():
+    for _, test in problem["problem"]["tests"].items():
         total_points += test["points"]
     return total_points
```

### Comparing `cs3560-grading-lib-0.1.0rc2/tests/test_common.py` & `cs3560_grading_lib-0.1.1a2/tests/test_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import tempfile
 import time
 from pathlib import Path
 
 import pytest
 
 from grading_lib import is_debug_mode
-from grading_lib.common import get_mtime_as_datetime, has_file_changed
+from grading_lib.common import (
+    get_mtime_as_datetime,
+    get_seed_from_env,
+    has_file_changed,
+)
 
 
 def test_is_debug_mode():
     vals_for_true = ["1", "True", "T", "On", "ON", "t", "true"]
     for val in vals_for_true:
         os.environ["test_DEBUG"] = val
         assert is_debug_mode("test_DEBUG")
@@ -20,14 +24,20 @@
         if val is None:
             del os.environ["test_DEBUG"]
         else:
             os.environ["test_DEBUG"] = val
         assert is_debug_mode("test_DEBUG") is False
 
 
+def test_get_seed_from_env():
+    val = 123
+    os.environ["test_SEED"] = str(val)
+    assert get_seed_from_env("test_SEED") == val
+
+
 @pytest.fixture
 def a_temp_file():
     f = tempfile.NamedTemporaryFile()
     f.seek(0)
     yield f
     f.close()
```

### Comparing `cs3560-grading-lib-0.1.0rc2/tests/test_makefile.py` & `cs3560_grading_lib-0.1.1a2/tests/test_makefile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from grading_lib.makefile import Makefile, VariableDefinition
+from grading_lib.makefile import Makefile
 
 
 @pytest.fixture
 def makefile_1():
     """
     First line is empty and two equal signs on a var-def line.
     """
@@ -18,15 +18,15 @@
 
 
 @pytest.fixture
 def makefile_2():
     return """
 # https://www.gnu.org/software/make/manual/html_node/Phony-Targets.html
 
-.PHONY: Date 
+.PHONY: Date
 
 weekend := $(shell date  | grep -E '^(Sat|Sun)' | wc -l | tr -d ' ')
 
 ifeq ($(weekend),0)
 	output := Weekday
 else
 	output := Weekend
@@ -76,34 +76,34 @@
 
 def test_makefile_from_text(makefile_1):
     """
     A verification test for `:` showing up twice.
     """
 
     try:
-        mk = Makefile.from_text(makefile_1)
+        _ = Makefile.from_text(makefile_1)
     except Exception:
-        assert False, "Exception raises while parsing a makefile."
+        pytest.fail("Exception raises while parsing a makefile.")
 
 
 def test_makefile_from_text_2(makefile_2):
     try:
         mk = Makefile.from_text(makefile_2)
     except Exception:
-        assert False, "Exception raises while parsing a makefile."
+        pytest.fail("Exception raises while parsing a makefile.")
 
     assert mk.rules[0].is_empty()
     assert not mk.rules[1].is_empty()
 
 
 def test_makefile_from_text_3(makefile_3):
     try:
         mk = Makefile.from_text(makefile_3)
     except Exception:
-        assert False, "Exception raises while parsing a makefile."
+        pytest.fail("Exception raises while parsing a makefile.")
 
     assert mk.has_rule("a")
     assert mk.get_rule("a").prerequisites == ["e", "f"]
 
     assert mk.has_rule("b")
     assert mk.get_rule("b").prerequisites == ["g"]
 
@@ -113,10 +113,10 @@
 
     assert mk.has_rule("d")
     assert mk.get_rule("d").prerequisites == ["i", "j"]
 
 
 def test_makefile_var_defs_parsing(makefile_var_defs):
     try:
-        mk = Makefile.from_text(makefile_var_defs)
+        _ = Makefile.from_text(makefile_var_defs)
     except Exception:
-        assert False, "Exception raises while parsing a makefile."
+        pytest.fail("Exception raises while parsing a makefile.")
```

