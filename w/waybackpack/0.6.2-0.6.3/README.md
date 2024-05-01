# Comparing `tmp/waybackpack-0.6.2.tar.gz` & `tmp/waybackpack-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waybackpack-0.6.2.tar", last modified: Sat Feb 10 21:21:05 2024, max compression
+gzip compressed data, was "waybackpack-0.6.3.tar", last modified: Wed May  1 12:34:54 2024, max compression
```

## Comparing `waybackpack-0.6.2.tar` & `waybackpack-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-02-10 21:21:05.586969 waybackpack-0.6.2/
--rw-r--r--   0 jeremy     (501) staff       (20)     1091 2024-02-10 21:19:40.000000 waybackpack-0.6.2/LICENSE.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-01-18 20:58:28.000000 waybackpack-0.6.2/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)     1108 2024-02-10 21:21:05.586794 waybackpack-0.6.2/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     5439 2024-02-10 21:20:30.000000 waybackpack-0.6.2/README.md
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2024-02-10 21:21:05.587003 waybackpack-0.6.2/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1545 2024-02-10 21:20:30.000000 waybackpack-0.6.2/setup.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-02-10 21:21:05.583951 waybackpack-0.6.2/tests/
--rw-r--r--   0 jeremy     (501) staff       (20)      398 2023-01-18 21:53:05.000000 waybackpack-0.6.2/tests/test_bad_statuses.py
--rw-r--r--   0 jeremy     (501) staff       (20)      612 2023-01-18 21:32:38.000000 waybackpack-0.6.2/tests/test_cdx.py
--rw-r--r--   0 jeremy     (501) staff       (20)      506 2023-01-18 21:32:38.000000 waybackpack-0.6.2/tests/test_dol.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1250 2024-01-17 19:58:58.000000 waybackpack-0.6.2/tests/test_download.py
--rw-r--r--   0 jeremy     (501) staff       (20)      482 2023-01-18 21:32:38.000000 waybackpack-0.6.2/tests/test_empty_results.py
--rw-r--r--   0 jeremy     (501) staff       (20)      660 2024-01-17 20:03:21.000000 waybackpack-0.6.2/tests/test_redirect.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-02-10 21:21:05.585677 waybackpack-0.6.2/waybackpack/
--rw-r--r--   0 jeremy     (501) staff       (20)      199 2023-01-18 21:16:23.000000 waybackpack-0.6.2/waybackpack/__init__.py
--rw-r--r--   0 jeremy     (501) staff       (20)     2920 2024-02-10 20:47:38.000000 waybackpack-0.6.2/waybackpack/asset.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1137 2024-01-17 21:27:08.000000 waybackpack-0.6.2/waybackpack/cdx.py
--rw-r--r--   0 jeremy     (501) staff       (20)     5116 2024-01-17 21:19:07.000000 waybackpack-0.6.2/waybackpack/cli.py
--rw-r--r--   0 jeremy     (501) staff       (20)     3842 2024-02-10 21:20:30.000000 waybackpack-0.6.2/waybackpack/pack.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1895 2024-01-17 22:57:58.000000 waybackpack-0.6.2/waybackpack/session.py
--rw-r--r--   0 jeremy     (501) staff       (20)       76 2018-09-20 12:27:54.000000 waybackpack-0.6.2/waybackpack/settings.py
--rw-r--r--   0 jeremy     (501) staff       (20)       22 2024-02-10 21:20:30.000000 waybackpack-0.6.2/waybackpack/version.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-02-10 21:21:05.586527 waybackpack-0.6.2/waybackpack.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     1108 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/PKG-INFO
--rwxrwxrwx   0 jeremy     (501) staff       (20)      564 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/SOURCES.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)        1 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/dependency_links.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)       53 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/entry_points.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)       22 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/requires.txt
--rwxrwxrwx   0 jeremy     (501) staff       (20)       12 2024-02-10 21:21:05.000000 waybackpack-0.6.2/waybackpack.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-05-01 12:34:54.592057 waybackpack-0.6.3/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1091 2024-02-10 21:19:40.000000 waybackpack-0.6.3/LICENSE.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-01-18 20:58:28.000000 waybackpack-0.6.3/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     1108 2024-05-01 12:34:54.591843 waybackpack-0.6.3/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     5439 2024-02-10 21:20:30.000000 waybackpack-0.6.3/README.md
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2024-05-01 12:34:54.592100 waybackpack-0.6.3/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1545 2024-02-10 21:20:30.000000 waybackpack-0.6.3/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-05-01 12:34:54.588059 waybackpack-0.6.3/tests/
+-rw-r--r--   0 jeremy     (501) staff       (20)      398 2023-01-18 21:53:05.000000 waybackpack-0.6.3/tests/test_bad_statuses.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      612 2023-01-18 21:32:38.000000 waybackpack-0.6.3/tests/test_cdx.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      506 2023-01-18 21:32:38.000000 waybackpack-0.6.3/tests/test_dol.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1250 2024-01-17 19:58:58.000000 waybackpack-0.6.3/tests/test_download.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      482 2023-01-18 21:32:38.000000 waybackpack-0.6.3/tests/test_empty_results.py
+-rw-r--r--   0 jeremy     (501) staff       (20)      660 2024-01-17 20:03:21.000000 waybackpack-0.6.3/tests/test_redirect.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-05-01 12:34:54.590604 waybackpack-0.6.3/waybackpack/
+-rw-r--r--   0 jeremy     (501) staff       (20)      199 2023-01-18 21:16:23.000000 waybackpack-0.6.3/waybackpack/__init__.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     2920 2024-02-10 20:47:38.000000 waybackpack-0.6.3/waybackpack/asset.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1137 2024-01-17 21:27:08.000000 waybackpack-0.6.3/waybackpack/cdx.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     5116 2024-01-17 21:19:07.000000 waybackpack-0.6.3/waybackpack/cli.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     3842 2024-05-01 12:28:07.000000 waybackpack-0.6.3/waybackpack/pack.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1895 2024-01-17 22:57:58.000000 waybackpack-0.6.3/waybackpack/session.py
+-rw-r--r--   0 jeremy     (501) staff       (20)       76 2018-09-20 12:27:54.000000 waybackpack-0.6.3/waybackpack/settings.py
+-rw-r--r--   0 jeremy     (501) staff       (20)       22 2024-05-01 12:32:03.000000 waybackpack-0.6.3/waybackpack/version.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2024-05-01 12:34:54.591460 waybackpack-0.6.3/waybackpack.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1108 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/PKG-INFO
+-rwxrwxrwx   0 jeremy     (501) staff       (20)      564 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)        1 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       53 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/entry_points.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       22 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/requires.txt
+-rwxrwxrwx   0 jeremy     (501) staff       (20)       12 2024-05-01 12:34:54.000000 waybackpack-0.6.3/waybackpack.egg-info/top_level.txt
```

### Comparing `waybackpack-0.6.2/LICENSE.txt` & `waybackpack-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/PKG-INFO` & `waybackpack-0.6.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waybackpack
-Version: 0.6.2
+Version: 0.6.3
 Summary: Command-line tool that lets you download the entire Wayback Machine archive for a given URL.
 Home-page: https://github.com/jsvine/waybackpack
 Author: Jeremy Singer-Vine
 Author-email: jsvine@gmail.com
 License: MIT
 Keywords: wayback machine archive
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `waybackpack-0.6.2/README.md` & `waybackpack-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/setup.py` & `waybackpack-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/tests/test_cdx.py` & `waybackpack-0.6.3/tests/test_cdx.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/tests/test_download.py` & `waybackpack-0.6.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/tests/test_redirect.py` & `waybackpack-0.6.3/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/waybackpack/asset.py` & `waybackpack-0.6.3/waybackpack/asset.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/waybackpack/cdx.py` & `waybackpack-0.6.3/waybackpack/cdx.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/waybackpack/cli.py` & `waybackpack-0.6.3/waybackpack/cli.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/waybackpack/pack.py` & `waybackpack-0.6.3/waybackpack/pack.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,18 +75,14 @@
 
         if progress and not has_tqdm:
             raise Exception(
                 "To print progress bars, you must have `tqdm` installed. To install: pip install tqdm."
             )
 
         for i, asset in enumerate(tqdm(self.assets) if progress else self.assets):
-            if i > 0 and delay:
-                logger.info("Sleeping {0} seconds".format(delay))
-                time.sleep(delay)
-
             path_head, path_tail = os.path.split(self.parsed_url.path)
             if path_tail == "":
                 path_tail = "index.html"
 
             filedir = os.path.join(
                 directory,
                 asset.timestamp,
@@ -99,14 +95,18 @@
             )
 
             if no_clobber and (
                 os.path.exists(filepath) and os.path.getsize(filepath) > 0
             ):
                 continue
 
+            if i > 0 and delay:
+                logger.info("Sleeping {0} seconds".format(delay))
+                time.sleep(delay)
+
             logger.info(
                 "Fetching {0} @ {1}".format(asset.original_url, asset.timestamp)
             )
 
             try:
                 content = asset.fetch(session=self.session, raw=raw, root=root)
```

### Comparing `waybackpack-0.6.2/waybackpack/session.py` & `waybackpack-0.6.3/waybackpack/session.py`

 * *Files identical despite different names*

### Comparing `waybackpack-0.6.2/waybackpack.egg-info/PKG-INFO` & `waybackpack-0.6.3/waybackpack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waybackpack
-Version: 0.6.2
+Version: 0.6.3
 Summary: Command-line tool that lets you download the entire Wayback Machine archive for a given URL.
 Home-page: https://github.com/jsvine/waybackpack
 Author: Jeremy Singer-Vine
 Author-email: jsvine@gmail.com
 License: MIT
 Keywords: wayback machine archive
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `waybackpack-0.6.2/waybackpack.egg-info/SOURCES.txt` & `waybackpack-0.6.3/waybackpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

