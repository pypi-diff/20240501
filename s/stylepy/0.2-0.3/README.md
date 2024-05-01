# Comparing `tmp/stylepy-0.2.tar.gz` & `tmp/stylepy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylepy-0.2.tar", last modified: Wed May  1 14:03:11 2024, max compression
+gzip compressed data, was "stylepy-0.3.tar", last modified: Wed May  1 14:52:12 2024, max compression
```

## Comparing `stylepy-0.2.tar` & `stylepy-0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:03:11.337673 stylepy-0.2/
--rw-r--r--   0 alamelu    (501) staff       (20)       23 2024-05-01 04:23:55.000000 stylepy-0.2/AUTHORS.txt
--rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 14:03:11.337162 stylepy-0.2/PKG-INFO
--rw-r--r--   0 alamelu    (501) staff       (20)     1394 2024-05-01 05:23:31.000000 stylepy-0.2/README.md
--rw-r--r--   0 alamelu    (501) staff       (20)       38 2024-05-01 14:03:11.337917 stylepy-0.2/setup.cfg
--rw-r--r--   0 alamelu    (501) staff       (20)      459 2024-05-01 13:40:48.000000 stylepy-0.2/setup.py
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:03:11.331682 stylepy-0.2/stylepy.egg-info/
--rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 14:03:11.000000 stylepy-0.2/stylepy.egg-info/PKG-INFO
--rw-r--r--   0 alamelu    (501) staff       (20)      339 2024-05-01 14:03:11.000000 stylepy-0.2/stylepy.egg-info/SOURCES.txt
--rw-r--r--   0 alamelu    (501) staff       (20)        1 2024-05-01 14:03:11.000000 stylepy-0.2/stylepy.egg-info/dependency_links.txt
--rw-r--r--   0 alamelu    (501) staff       (20)        6 2024-05-01 14:03:11.000000 stylepy-0.2/stylepy.egg-info/top_level.txt
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:03:11.332258 stylepy-0.2/tests/
--rw-r--r--   0 alamelu    (501) staff       (20)      284 2024-05-01 13:58:19.000000 stylepy-0.2/tests/test_header.py
-drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:03:11.336543 stylepy-0.2/utils/
--rw-r--r--   0 alamelu    (501) staff       (20)      214 2024-05-01 13:41:48.000000 stylepy-0.2/utils/__init__.py
--rw-r--r--   0 alamelu    (501) staff       (20)      202 2024-05-01 03:38:44.000000 stylepy-0.2/utils/blockquote.py
--rw-r--r--   0 alamelu    (501) staff       (20)      952 2024-05-01 03:35:59.000000 stylepy-0.2/utils/header.py
--rw-r--r--   0 alamelu    (501) staff       (20)      295 2024-05-01 03:38:11.000000 stylepy-0.2/utils/inline.py
--rw-r--r--   0 alamelu    (501) staff       (20)      104 2024-05-01 03:38:09.000000 stylepy-0.2/utils/json.py
--rw-r--r--   0 alamelu    (501) staff       (20)      246 2024-05-01 03:37:36.000000 stylepy-0.2/utils/list.py
--rw-r--r--   0 alamelu    (501) staff       (20)      251 2024-05-01 03:19:57.000000 stylepy-0.2/utils/space_complexity.py
--rw-r--r--   0 alamelu    (501) staff       (20)     1121 2024-05-01 03:39:40.000000 stylepy-0.2/utils/table.py
--rw-r--r--   0 alamelu    (501) staff       (20)      266 2024-05-01 03:19:59.000000 stylepy-0.2/utils/time_complexity.py
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:52:12.436800 stylepy-0.3/
+-rw-r--r--   0 alamelu    (501) staff       (20)       23 2024-05-01 04:23:55.000000 stylepy-0.3/AUTHORS.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 14:52:12.436305 stylepy-0.3/PKG-INFO
+-rw-r--r--   0 alamelu    (501) staff       (20)     1394 2024-05-01 05:23:31.000000 stylepy-0.3/README.md
+-rw-r--r--   0 alamelu    (501) staff       (20)       38 2024-05-01 14:52:12.436932 stylepy-0.3/setup.cfg
+-rw-r--r--   0 alamelu    (501) staff       (20)      459 2024-05-01 14:51:40.000000 stylepy-0.3/setup.py
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:52:12.435620 stylepy-0.3/stylepy.egg-info/
+-rw-r--r--   0 alamelu    (501) staff       (20)     1690 2024-05-01 14:52:12.000000 stylepy-0.3/stylepy.egg-info/PKG-INFO
+-rw-r--r--   0 alamelu    (501) staff       (20)      339 2024-05-01 14:52:12.000000 stylepy-0.3/stylepy.egg-info/SOURCES.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)        1 2024-05-01 14:52:12.000000 stylepy-0.3/stylepy.egg-info/dependency_links.txt
+-rw-r--r--   0 alamelu    (501) staff       (20)        6 2024-05-01 14:52:12.000000 stylepy-0.3/stylepy.egg-info/top_level.txt
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:52:12.429837 stylepy-0.3/tests/
+-rw-r--r--   0 alamelu    (501) staff       (20)      285 2024-05-01 14:07:00.000000 stylepy-0.3/tests/test_header.py
+drwxr-xr-x   0 alamelu    (501) staff       (20)        0 2024-05-01 14:52:12.434927 stylepy-0.3/utils/
+-rw-r--r--   0 alamelu    (501) staff       (20)      214 2024-05-01 13:41:48.000000 stylepy-0.3/utils/__init__.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      202 2024-05-01 03:38:44.000000 stylepy-0.3/utils/blockquote.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      952 2024-05-01 03:35:59.000000 stylepy-0.3/utils/header.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      295 2024-05-01 03:38:11.000000 stylepy-0.3/utils/inline.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      104 2024-05-01 03:38:09.000000 stylepy-0.3/utils/json.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      246 2024-05-01 03:37:36.000000 stylepy-0.3/utils/list.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      251 2024-05-01 03:19:57.000000 stylepy-0.3/utils/space_complexity.py
+-rw-r--r--   0 alamelu    (501) staff       (20)     1121 2024-05-01 03:39:40.000000 stylepy-0.3/utils/table.py
+-rw-r--r--   0 alamelu    (501) staff       (20)      266 2024-05-01 03:19:59.000000 stylepy-0.3/utils/time_complexity.py
```

### Comparing `stylepy-0.2/PKG-INFO` & `stylepy-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylepy
-Version: 0.2
+Version: 0.3
 Summary: Format CLI output like HTML.
 Home-page: https://github.com/web-slate/stylepy
 Author: Venkatraman.R
 Author-email: ramsunvtech@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```

### Comparing `stylepy-0.2/README.md` & `stylepy-0.3/README.md`

 * *Files identical despite different names*

### Comparing `stylepy-0.2/stylepy.egg-info/PKG-INFO` & `stylepy-0.3/stylepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylepy
-Version: 0.2
+Version: 0.3
 Summary: Format CLI output like HTML.
 Home-page: https://github.com/web-slate/stylepy
 Author: Venkatraman.R
 Author-email: ramsunvtech@gmail.com
 License: MIT
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
```

### Comparing `stylepy-0.2/utils/header.py` & `stylepy-0.3/utils/header.py`

 * *Files identical despite different names*

### Comparing `stylepy-0.2/utils/table.py` & `stylepy-0.3/utils/table.py`

 * *Files identical despite different names*

