# Comparing `tmp/pyhaveibeenpwned-0.1.7.tar.gz` & `tmp/pyHaveIBeenPwned-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhaveibeenpwned-0.1.7.tar", last modified: Wed May  1 18:16:49 2024, max compression
+gzip compressed data, was "pyHaveIBeenPwned-0.1.8.tar", last modified: Wed May  1 19:24:47 2024, max compression
```

## Comparing `pyhaveibeenpwned-0.1.7.tar` & `pyHaveIBeenPwned-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:47.592239 pyHaveIBeenPwned-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-01 19:24:21.000000 pyHaveIBeenPwned-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-01 19:24:47.592239 pyHaveIBeenPwned-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-01 19:24:21.000000 pyHaveIBeenPwned-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:47.592239 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-01 19:24:21.000000 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:24:47.592239 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-01 19:24:47.000000 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 19:24:47.000000 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:24:47.000000 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 19:24:47.000000 pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 19:24:47.592239 pyHaveIBeenPwned-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 19:24:21.000000 pyHaveIBeenPwned-0.1.8/setup.py
```

### Comparing `pyhaveibeenpwned-0.1.7/LICENSE` & `pyHaveIBeenPwned-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhaveibeenpwned-0.1.7/PKG-INFO` & `pyHaveIBeenPwned-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: pyHaveIBeenPwned
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot 
 Home-page: https://github.com/GoVanguard/pyHaveIBeenPwned
 Author: Shane Scott
 Author-email: sscott@gotham-security.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyHaveIBeenPwned (https://govanguard.com)
 ==
 [![Build Status](https://github.com/GoVanguard/pyHaveIBeenPwned/actions/workflows/package-installation-build.yml/badge.svg)](https://github.com/GoVanguard/pyHaveIBeenPwned/actions/workflows/package-installation-test.yml)
 [![Known Vulnerabilities](https://snyk.io/test/github/GoVanguard/pyHaveIBeenPwned/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/GoVanguard/pyHaveIBeenPwned?targetFile=requirements.txt)
@@ -23,7 +31,9 @@
 Shane Scott
 
 ## About pyHaveIBeenPwned
 Python library to query HaveIBeenPwned.com with handling for CloudFlare anti-bot.
 
 ## Installation
 pip install pyHaveIBeenPwned
+
+
```

### Comparing `pyhaveibeenpwned-0.1.7/README.md` & `pyHaveIBeenPwned-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned/__init__.py` & `pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/PKG-INFO` & `pyHaveIBeenPwned-0.1.8/pyHaveIBeenPwned.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: pyHaveIBeenPwned
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot 
 Home-page: https://github.com/GoVanguard/pyHaveIBeenPwned
 Author: Shane Scott
 Author-email: sscott@gotham-security.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyHaveIBeenPwned (https://govanguard.com)
 ==
 [![Build Status](https://github.com/GoVanguard/pyHaveIBeenPwned/actions/workflows/package-installation-build.yml/badge.svg)](https://github.com/GoVanguard/pyHaveIBeenPwned/actions/workflows/package-installation-test.yml)
 [![Known Vulnerabilities](https://snyk.io/test/github/GoVanguard/pyHaveIBeenPwned/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/GoVanguard/pyHaveIBeenPwned?targetFile=requirements.txt)
@@ -23,7 +31,9 @@
 Shane Scott
 
 ## About pyHaveIBeenPwned
 Python library to query HaveIBeenPwned.com with handling for CloudFlare anti-bot.
 
 ## Installation
 pip install pyHaveIBeenPwned
+
+
```

### Comparing `pyhaveibeenpwned-0.1.7/setup.py` & `pyHaveIBeenPwned-0.1.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyHaveIBeenPwned",
-    version="0.1.7",
+    version="0.1.8",
     author="Shane Scott",
     author_email="sscott@gotham-security.com",
     description="Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GoVanguard/pyHaveIBeenPwned",
     packages=['pyHaveIBeenPwned'],
-    classifiers=(
+    classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
-        'Programming Language :: Python :: 3.6',
-        'Operating System :: OS Independent',
-    ),
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Operating System :: Microsoft :: Windows',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: POSIX :: Linux',
+        'Topic :: Software Development :: Libraries',
+    ],
+    python_requires='>=3.9',
 )
```

