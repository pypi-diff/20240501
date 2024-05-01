# Comparing `tmp/consolidate-0.0.2.tar.gz` & `tmp/consolidate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolidate-0.0.2.tar", last modified: Tue Dec 19 00:23:40 2023, max compression
+gzip compressed data, was "consolidate-0.0.3.tar", last modified: Wed May  1 06:08:36 2024, max compression
```

## Comparing `consolidate-0.0.2.tar` & `consolidate-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-12-19 00:23:40.965880 consolidate-0.0.2/
--rw-rw-rw-   0        0        0     1215 2023-12-19 00:23:40.965880 consolidate-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-12-18 01:34:20.000000 consolidate-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-12-19 00:23:40.951867 consolidate-0.0.2/consolidate/
--rw-rw-rw-   0        0        0        0 2023-12-17 23:09:23.000000 consolidate-0.0.2/consolidate/__init__.py
--rw-rw-rw-   0        0        0      495 2023-12-19 00:17:21.000000 consolidate-0.0.2/consolidate/consolidatemodule.py
-drwxrwxrwx   0        0        0        0 2023-12-19 00:23:40.964879 consolidate-0.0.2/consolidate.egg-info/
--rw-rw-rw-   0        0        0     1215 2023-12-19 00:23:40.000000 consolidate-0.0.2/consolidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-12-19 00:23:40.000000 consolidate-0.0.2/consolidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-19 00:23:40.000000 consolidate-0.0.2/consolidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-12-19 00:23:40.000000 consolidate-0.0.2/consolidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-19 00:23:40.966881 consolidate-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1784 2023-12-19 00:23:26.000000 consolidate-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:08:36.120732 consolidate-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 06:08:36.116732 consolidate-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-01 06:08:32.000000 consolidate-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:08:36.116732 consolidate-0.0.3/consolidate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:08:32.000000 consolidate-0.0.3/consolidate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-01 06:08:32.000000 consolidate-0.0.3/consolidate/consolidatemodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:08:36.116732 consolidate-0.0.3/consolidate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-01 06:08:36.000000 consolidate-0.0.3/consolidate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 06:08:36.000000 consolidate-0.0.3/consolidate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:08:36.000000 consolidate-0.0.3/consolidate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 06:08:36.000000 consolidate-0.0.3/consolidate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:08:36.120732 consolidate-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-01 06:08:32.000000 consolidate-0.0.3/setup.py
```

### Comparing `consolidate-0.0.2/PKG-INFO` & `consolidate-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: consolidate
-Version: 0.0.2
-Summary: A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
-Home-page: https://github.com/ThePilot4571/consolidate-py/
-Author: ThePilot4571
-Author-email: nocosecantoftheta@gmail.com
-Project-URL: Source, https://github.com/ThePilot4571/consolidate-py/
-Keywords: python,spaces,string,username,spam
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Description-Content-Type: text/markdown
-
-# Consolidate <br> <br> ### A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
+Metadata-Version: 2.1
+Name: consolidate
+Version: 0.0.3
+Summary: A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
+Home-page: https://github.com/ThePilot4571/consolidate-py/
+Author: ThePilot4571
+Author-email: nocosecantoftheta@gmail.com
+Project-URL: Source, https://github.com/ThePilot4571/consolidate-py/
+Keywords: python,spaces,string,username,spam
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Description-Content-Type: text/markdown
+
+Consolidate A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
```

### Comparing `consolidate-0.0.2/README.md` & `consolidate-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-# consolidate-py
-A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
-## What you could use this for
-This module was built to allow for the generation of inputs when duplicate inputs aren't allowed. <br><br>
-I used this in my Kahoot spam bot to allow for me to (for educational purposes, obviously) generate the same username for my bots, because Kahoot doesn't allow duplicate names, and 20 "SpanishInquisition"s are a lot cooler than than "SpanishInquisition7923", "SpanishInquisition8213", etc.
-## Syntax:
-Import module by typing ```from consolidate.consolidatemodule import generate``` in your Python program file<br><br>
-Run the generate function with ```generate(string baseString, int maxCharacterLength (default 6, can't be less than baseString's length), string fillerString (default is a zero width non-joiner U+200C ) )```
-## Example usage:
-print(generate("python", 8, "X")) <br><br>
-&#62; ["python", "Xpython", "XXpython", "pXython", "XpXython", "pyXthon", "XpyXthon", ... ]
+# consolidate-py
+A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
+## What you could use this for
+This module was built to allow for the generation of inputs when duplicate inputs aren't allowed. <br><br>
+I used this in my Kahoot spam bot to allow for me to (for educational purposes, obviously) generate the same username for my bots, because Kahoot doesn't allow duplicate names, and 20 "SpanishInquisition"s are a lot cooler than than "SpanishInquisition7923", "SpanishInquisition8213", etc.
+## Syntax:
+Import module by typing ```from consolidate.consolidatemodule import generate``` in your Python program file<br><br>
+Run the generate function with ```generate(string baseString, int maxCharacterLength (default 6, can't be less than baseString's length), string fillerString (default is a zero width non-joiner U+200C ) )```
+## Example usage:
+print(generate("python", 8, "X")) <br><br>
+&#62; ["python", "Xpython", "XXpython", "pXython", "XpXython", "pyXthon", "XpyXthon", ... ]
+## Supporting consolidate.py:
+Please feel free to modify the code to add functionalities you want to!
+<br> Something I'm missing is the ability to use strings to fill instead of a single character... it compl
```

### Comparing `consolidate-0.0.2/consolidate.egg-info/PKG-INFO` & `consolidate-0.0.3/consolidate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: consolidate
-Version: 0.0.2
-Summary: A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
-Home-page: https://github.com/ThePilot4571/consolidate-py/
-Author: ThePilot4571
-Author-email: nocosecantoftheta@gmail.com
-Project-URL: Source, https://github.com/ThePilot4571/consolidate-py/
-Keywords: python,spaces,string,username,spam
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Description-Content-Type: text/markdown
-
-# Consolidate <br> <br> ### A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
+Metadata-Version: 2.1
+Name: consolidate
+Version: 0.0.3
+Summary: A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
+Home-page: https://github.com/ThePilot4571/consolidate-py/
+Author: ThePilot4571
+Author-email: nocosecantoftheta@gmail.com
+Project-URL: Source, https://github.com/ThePilot4571/consolidate-py/
+Keywords: python,spaces,string,username,spam
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Description-Content-Type: text/markdown
+
+Consolidate A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.
```

### Comparing `consolidate-0.0.2/setup.py` & `consolidate-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""A setuptools based setup module.
-
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setup(
-    name="consolidate",
-    version="0.0.2",
-    description="A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.",
-    long_description="# Consolidate <br> <br> ### A Python library for generating a list of strings with every possible combination of placements of a given string (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.",
-    long_description_content_type='text/markdown',
-    url="https://github.com/ThePilot4571/consolidate-py/", 
-    author="ThePilot4571",
-    author_email="nocosecantoftheta@gmail.com",
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Build Tools",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: Unix",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: MacOS :: MacOS X"
-    ],
-    keywords=['python', 'spaces','string','username','spam'],
-    packages=find_packages(),
-    install_requires=[],
-    project_urls={
-        "Source": "https://github.com/ThePilot4571/consolidate-py/",
-    },
+"""A setuptools based setup module.
+
+See:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+"""
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setup(
+    name="consolidate",
+    version="0.0.3",
+    description="A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.",
+    long_description="Consolidate A Python library for generating a list of strings with every possible combination of placements of a given character (or a zero-width non joiner by default) within another given string, up to a given maximum length of characters.",
+    long_description_content_type='text/markdown',
+    url="https://github.com/ThePilot4571/consolidate-py/", 
+    author="ThePilot4571",
+    author_email="nocosecantoftheta@gmail.com",
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS :: MacOS X"
+    ],
+    keywords=['python', 'spaces','string','username','spam'],
+    packages=find_packages(),
+    install_requires=[],
+    project_urls={
+        "Source": "https://github.com/ThePilot4571/consolidate-py/",
+    },
 )
```

