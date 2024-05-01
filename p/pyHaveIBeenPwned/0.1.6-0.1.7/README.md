# Comparing `tmp/pyHaveIBeenPwned-0.1.6.tar.gz` & `tmp/pyhaveibeenpwned-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHaveIBeenPwned-0.1.6.tar", last modified: Fri Feb 23 16:35:29 2024, max compression
+gzip compressed data, was "pyhaveibeenpwned-0.1.7.tar", last modified: Wed May  1 18:16:49 2024, max compression
```

## Comparing `pyHaveIBeenPwned-0.1.6.tar` & `pyhaveibeenpwned-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:35:29.509724 pyHaveIBeenPwned-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-23 16:35:07.000000 pyHaveIBeenPwned-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-23 16:35:29.509724 pyHaveIBeenPwned-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-23 16:35:07.000000 pyHaveIBeenPwned-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:35:29.505724 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-23 16:35:07.000000 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:35:29.509724 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-23 16:35:29.000000 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-23 16:35:29.000000 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 16:35:29.000000 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-23 16:35:29.000000 pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-23 16:35:29.509724 pyHaveIBeenPwned-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-23 16:35:07.000000 pyHaveIBeenPwned-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 18:16:49.000000 pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 18:16:49.804299 pyhaveibeenpwned-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-01 18:16:25.000000 pyhaveibeenpwned-0.1.7/setup.py
```

### Comparing `pyHaveIBeenPwned-0.1.6/LICENSE` & `pyhaveibeenpwned-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHaveIBeenPwned-0.1.6/PKG-INFO` & `pyhaveibeenpwned-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyHaveIBeenPwned
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot 
 Home-page: https://github.com/GoVanguard/pyHaveIBeenPwned
 Author: Shane Scott
-Author-email: sscott@gvit.com
+Author-email: sscott@gotham-security.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyHaveIBeenPwned-0.1.6/README.md` & `pyhaveibeenpwned-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyHaveIBeenPwned-0.1.6/pyHaveIBeenPwned.egg-info/PKG-INFO` & `pyhaveibeenpwned-0.1.7/pyHaveIBeenPwned.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyHaveIBeenPwned
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot 
 Home-page: https://github.com/GoVanguard/pyHaveIBeenPwned
 Author: Shane Scott
-Author-email: sscott@gvit.com
+Author-email: sscott@gotham-security.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyHaveIBeenPwned-0.1.6/setup.py` & `pyhaveibeenpwned-0.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyHaveIBeenPwned",
-    version="0.1.6",
+    version="0.1.7",
     author="Shane Scott",
-    author_email="sscott@gvit.com",
+    author_email="sscott@gotham-security.com",
     description="Library to query HaveIBeenPwned.com with handeling for CloudFlare anti-bot ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GoVanguard/pyHaveIBeenPwned",
     packages=['pyHaveIBeenPwned'],
     classifiers=(
         'Development Status :: 3 - Alpha',
```

