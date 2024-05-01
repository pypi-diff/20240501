# Comparing `tmp/ytdlmusic-2.4.2.tar.gz` & `tmp/ytdlmusic-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdlmusic-2.4.2.tar", last modified: Sun Mar 31 09:54:04 2024, max compression
+gzip compressed data, was "ytdlmusic-2.4.3.tar", last modified: Wed May  1 06:17:51 2024, max compression
```

## Comparing `ytdlmusic-2.4.2.tar` & `ytdlmusic-2.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:54:04.547388 ytdlmusic-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-31 09:54:04.547388 ytdlmusic-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:54:04.547388 ytdlmusic-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:54:04.547388 ytdlmusic-2.4.2/ytdlmusic/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/print.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-31 09:53:58.000000 ytdlmusic-2.4.2/ytdlmusic/ytdlmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:54:04.547388 ytdlmusic-2.4.2/ytdlmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 09:54:04.000000 ytdlmusic-2.4.2/ytdlmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:51.202081 ytdlmusic-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 06:17:51.202081 ytdlmusic-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:17:51.202081 ytdlmusic-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:51.202081 ytdlmusic-2.4.3/ytdlmusic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-01 06:17:47.000000 ytdlmusic-2.4.3/ytdlmusic/ytdlmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:51.202081 ytdlmusic-2.4.3/ytdlmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 06:17:51.000000 ytdlmusic-2.4.3/ytdlmusic.egg-info/top_level.txt
```

### Comparing `ytdlmusic-2.4.2/LICENSE.txt` & `ytdlmusic-2.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/PKG-INFO` & `ytdlmusic-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdlmusic
-Version: 2.4.2
+Version: 2.4.3
 Summary: ytdlmusic is a command-line program to search and download music files from YouTube without use browser.
 Home-page: https://github.com/thib1984/ytdlmusic
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ytdlmusic-2.4.2/README.md` & `ytdlmusic-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/setup.py` & `ytdlmusic-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="ytdlmusic",
-    version="2.4.2",
+    version="2.4.3",
     description="ytdlmusic is a command-line program to search and download music files from YouTube without use browser.",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/ytdlmusic#readme",
     long_description_content_type="text/markdown",
     url="https://github.com/thib1984/ytdlmusic",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
```

### Comparing `ytdlmusic-2.4.2/ytdlmusic/__init__.py` & `ytdlmusic-2.4.3/ytdlmusic/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/batch.py` & `ytdlmusic-2.4.3/ytdlmusic/batch.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/choice.py` & `ytdlmusic-2.4.3/ytdlmusic/choice.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/const.py` & `ytdlmusic-2.4.3/ytdlmusic/const.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/download.py` & `ytdlmusic-2.4.3/ytdlmusic/download.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/file.py` & `ytdlmusic-2.4.3/ytdlmusic/file.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/params.py` & `ytdlmusic-2.4.3/ytdlmusic/params.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/print.py` & `ytdlmusic-2.4.3/ytdlmusic/print.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/search.py` & `ytdlmusic-2.4.3/ytdlmusic/search.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/tag.py` & `ytdlmusic-2.4.3/ytdlmusic/tag.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/update.py` & `ytdlmusic-2.4.3/ytdlmusic/update.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/version.py` & `ytdlmusic-2.4.3/ytdlmusic/version.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic/ytdlmusic.py` & `ytdlmusic-2.4.3/ytdlmusic/ytdlmusic.py`

 * *Files identical despite different names*

### Comparing `ytdlmusic-2.4.2/ytdlmusic.egg-info/PKG-INFO` & `ytdlmusic-2.4.3/ytdlmusic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdlmusic
-Version: 2.4.2
+Version: 2.4.3
 Summary: ytdlmusic is a command-line program to search and download music files from YouTube without use browser.
 Home-page: https://github.com/thib1984/ytdlmusic
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ytdlmusic-2.4.2/ytdlmusic.egg-info/SOURCES.txt` & `ytdlmusic-2.4.3/ytdlmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

