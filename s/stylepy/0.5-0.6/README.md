# Comparing `tmp/stylepy-0.5.tar.gz` & `tmp/stylepy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylepy-0.5.tar", last modified: Wed May  1 16:02:07 2024, max compression
+gzip compressed data, was "stylepy-0.6.tar", last modified: Wed May  1 16:09:38 2024, max compression
```

## Comparing `stylepy-0.5.tar` & `stylepy-0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:02:07.082557 stylepy-0.5/
--rw-r--r--   0 alamelu    (501) staff       (20)       23 2024-05-01 04:23:55.000000 stylepy-0.5/AUTHORS.txt
--rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 16:02:07.082275 stylepy-0.5/PKG-INFO
--rw-r--r--   0 alamelu    (501) staff       (20)     1394 2024-05-01 05:23:31.000000 stylepy-0.5/README.md
--rw-r--r--   0 alamelu    (501) staff       (20)       38 2024-05-01 16:02:07.082665 stylepy-0.5/setup.cfg
--rw-r--r--   0 alamelu    (501) staff       (20)      489 2024-05-01 16:01:27.000000 stylepy-0.5/setup.py
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:02:07.080224 stylepy-0.5/stylepy/
--rw-r--r--   0 alamelu    (501) staff       (20)      214 2024-05-01 16:01:28.000000 stylepy-0.5/stylepy/__init__.py
--rw-r--r--   0 alamelu    (501) staff       (20)      202 2024-05-01 03:38:44.000000 stylepy-0.5/stylepy/blockquote.py
--rw-r--r--   0 alamelu    (501) staff       (20)      952 2024-05-01 15:51:04.000000 stylepy-0.5/stylepy/header.py
--rw-r--r--   0 alamelu    (501) staff       (20)      295 2024-05-01 03:38:11.000000 stylepy-0.5/stylepy/inline.py
--rw-r--r--   0 alamelu    (501) staff       (20)      104 2024-05-01 03:38:09.000000 stylepy-0.5/stylepy/json.py
--rw-r--r--   0 alamelu    (501) staff       (20)      246 2024-05-01 03:37:36.000000 stylepy-0.5/stylepy/list.py
--rw-r--r--   0 alamelu    (501) staff       (20)      251 2024-05-01 03:19:57.000000 stylepy-0.5/stylepy/space_complexity.py
--rw-r--r--   0 alamelu    (501) staff       (20)     1121 2024-05-01 03:39:40.000000 stylepy-0.5/stylepy/table.py
--rw-r--r--   0 alamelu    (501) staff       (20)      266 2024-05-01 03:19:59.000000 stylepy-0.5/stylepy/time_complexity.py
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:02:07.081838 stylepy-0.5/stylepy.egg-info/
--rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 16:02:07.000000 stylepy-0.5/stylepy.egg-info/PKG-INFO
--rw-r--r--   0 alamelu    (501) staff       (20)      336 2024-05-01 16:02:07.000000 stylepy-0.5/stylepy.egg-info/SOURCES.txt
--rw-r--r--   0 alamelu    (501) staff       (20)        1 2024-05-01 16:02:07.000000 stylepy-0.5/stylepy.egg-info/dependency_links.txt
--rw-r--r--   0 alamelu    (501) staff       (20)        8 2024-05-01 16:02:07.000000 stylepy-0.5/stylepy.egg-info/top_level.txt
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:09:38.800931 stylepy-0.6/
+-rw-r--r--   0 alamelu    (501) staff       (20)       23 2024-05-01 04:23:55.000000 stylepy-0.6/AUTHORS.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 16:09:38.800251 stylepy-0.6/PKG-INFO
+-rw-r--r--   0 alamelu    (501) staff       (20)     1394 2024-05-01 05:23:31.000000 stylepy-0.6/README.md
+-rw-r--r--   0 alamelu    (501) staff       (20)       38 2024-05-01 16:09:38.801106 stylepy-0.6/setup.cfg
+-rw-r--r--   0 alamelu    (501) staff       (20)      489 2024-05-01 16:08:35.000000 stylepy-0.6/setup.py
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:09:38.797303 stylepy-0.6/stylepy/
+-rw-r--r--   0 alamelu    (501) staff       (20)      489 2024-05-01 16:08:30.000000 stylepy-0.6/stylepy/__init__.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      202 2024-05-01 03:38:44.000000 stylepy-0.6/stylepy/blockquote.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      952 2024-05-01 15:51:04.000000 stylepy-0.6/stylepy/header.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      295 2024-05-01 03:38:11.000000 stylepy-0.6/stylepy/inline.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      104 2024-05-01 03:38:09.000000 stylepy-0.6/stylepy/json.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      246 2024-05-01 03:37:36.000000 stylepy-0.6/stylepy/list.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      251 2024-05-01 03:19:57.000000 stylepy-0.6/stylepy/space_complexity.py
+-rw-r--r--   0 alamelu    (501) staff       (20)     1121 2024-05-01 03:39:40.000000 stylepy-0.6/stylepy/table.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      266 2024-05-01 03:19:59.000000 stylepy-0.6/stylepy/time_complexity.py
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 16:09:38.798647 stylepy-0.6/stylepy.egg-info/
+-rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 16:09:38.000000 stylepy-0.6/stylepy.egg-info/PKG-INFO
+-rw-r--r--   0 alamelu    (501) staff       (20)      336 2024-05-01 16:09:38.000000 stylepy-0.6/stylepy.egg-info/SOURCES.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)        1 2024-05-01 16:09:38.000000 stylepy-0.6/stylepy.egg-info/dependency_links.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)        8 2024-05-01 16:09:38.000000 stylepy-0.6/stylepy.egg-info/top_level.txt
```

### Comparing `stylepy-0.5/PKG-INFO` & `stylepy-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylepy
-Version: 0.5
+Version: 0.6
 Summary: Format CLI output like HTML.
 Home-page: https://github.com/web-slate/stylepy
 Author: Venkatraman.R
 Author-email: ramsunvtech@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```

### Comparing `stylepy-0.5/README.md` & `stylepy-0.6/README.md`

 * *Files identical despite different names*

### Comparing `stylepy-0.5/stylepy/header.py` & `stylepy-0.6/stylepy/header.py`

 * *Files identical despite different names*

### Comparing `stylepy-0.5/stylepy/table.py` & `stylepy-0.6/stylepy/table.py`

 * *Files identical despite different names*

### Comparing `stylepy-0.5/stylepy.egg-info/PKG-INFO` & `stylepy-0.6/stylepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylepy
-Version: 0.5
+Version: 0.6
 Summary: Format CLI output like HTML.
 Home-page: https://github.com/web-slate/stylepy
 Author: Venkatraman.R
 Author-email: ramsunvtech@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```
