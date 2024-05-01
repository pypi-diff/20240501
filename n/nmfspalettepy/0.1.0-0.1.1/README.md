# Comparing `tmp/nmfspalettepy-0.1.0.tar.gz` & `tmp/nmfspalettepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmfspalettepy-0.1.0.tar", last modified: Wed May  1 20:17:58 2024, max compression
+gzip compressed data, was "nmfspalettepy-0.1.1.tar", last modified: Wed May  1 20:25:54 2024, max compression
```

## Comparing `nmfspalettepy-0.1.0.tar` & `nmfspalettepy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:17:58.043748 nmfspalettepy-0.1.0/
--rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0      217 2024-05-01 20:17:58.043748 nmfspalettepy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3116 2024-05-01 20:12:45.000000 nmfspalettepy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 20:17:58.024641 nmfspalettepy-0.1.0/nmfspalettepy/
--rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.0/nmfspalettepy/__init__.py
--rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.0/nmfspalettepy/palettes.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:17:58.043748 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/
--rw-rw-rw-   0        0        0      217 2024-05-01 20:17:57.000000 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-01 20:17:57.000000 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:17:57.000000 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-01 20:17:57.000000 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 20:17:57.000000 nmfspalettepy-0.1.0/nmfspalettepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 20:17:58.043748 nmfspalettepy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      298 2024-05-01 19:27:25.000000 nmfspalettepy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.184908 nmfspalettepy-0.1.1/
+-rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     3366 2024-05-01 20:25:54.169282 nmfspalettepy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3116 2024-05-01 20:12:45.000000 nmfspalettepy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.160234 nmfspalettepy-0.1.1/nmfspalettepy/
+-rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.1/nmfspalettepy/__init__.py
+-rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.1/nmfspalettepy/palettes.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:25:54.169282 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/
+-rw-rw-rw-   0        0        0     3366 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-01 20:25:54.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 20:25:53.000000 nmfspalettepy-0.1.1/nmfspalettepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:25:54.184908 nmfspalettepy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-01 20:25:50.000000 nmfspalettepy-0.1.1/setup.py
```

### Comparing `nmfspalettepy-0.1.0/LICENSE.md` & `nmfspalettepy-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.0/README.md` & `nmfspalettepy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.0/nmfspalettepy/palettes.py` & `nmfspalettepy-0.1.1/nmfspalettepy/palettes.py`

 * *Files identical despite different names*

