# Comparing `tmp/lcz-0.1.4.tar.gz` & `tmp/lcz-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcz-0.1.4.tar", last modified: Tue Apr 16 07:34:28 2024, max compression
+gzip compressed data, was "lcz-0.1.6.tar", last modified: Wed May  1 18:09:05 2024, max compression
```

## Comparing `lcz-0.1.4.tar` & `lcz-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:34:28.948845 lcz-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-01-24 08:48:19.000000 lcz-0.1.4/MANIFEST.in
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      430 2024-04-16 07:34:28.948845 lcz-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       66 2024-04-16 07:32:55.000000 lcz-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-16 07:34:23.000000 lcz-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 07:34:28.948845 lcz-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:34:28.938845 lcz-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:34:28.938845 lcz-0.1.4/src/lcz/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      121 2024-01-24 08:08:17.000000 lcz-0.1.4/src/lcz/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-01-24 07:57:30.000000 lcz-0.1.4/src/lcz/backends.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1012 2024-04-16 07:33:46.000000 lcz-0.1.4/src/lcz/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      472 2024-01-24 07:57:02.000000 lcz-0.1.4/src/lcz/uci.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:34:28.948845 lcz-0.1.4/src/lcz/weights/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-01-24 08:06:45.000000 lcz-0.1.4/src/lcz/weights/__init__.py
--rwxr-xr-x   0 m4rs      (1000) m4rs      (1000)  1262607 2024-01-24 07:54:09.000000 lcz-0.1.4/src/lcz/weights/maia-1900.pb.gz
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-01-24 08:06:27.000000 lcz-0.1.4/src/lcz/weights/weights.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:34:28.948845 lcz-0.1.4/src/lcz.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      430 2024-04-16 07:34:28.000000 lcz-0.1.4/src/lcz.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      348 2024-04-16 07:34:28.000000 lcz-0.1.4/src/lcz.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 07:34:28.000000 lcz-0.1.4/src/lcz.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-04-16 07:34:28.000000 lcz-0.1.4/src/lcz.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        4 2024-04-16 07:34:28.000000 lcz-0.1.4/src/lcz.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 18:09:05.399057 lcz-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-05-01 18:06:31.000000 lcz-0.1.6/MANIFEST.in
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1214 2024-05-01 18:09:05.399057 lcz-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-05-01 18:07:43.000000 lcz-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-05-01 18:09:02.000000 lcz-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-01 18:09:05.399057 lcz-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 18:09:05.389056 lcz-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 18:09:05.399057 lcz-0.1.6/src/lcz/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      188 2024-05-01 18:05:38.000000 lcz-0.1.6/src/lcz/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-05-01 18:05:02.000000 lcz-0.1.6/src/lcz/backends.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1012 2024-05-01 18:05:02.000000 lcz-0.1.6/src/lcz/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      418 2024-05-01 18:05:08.000000 lcz-0.1.6/src/lcz/uci.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 18:09:05.399057 lcz-0.1.6/src/lcz/weights/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-05-01 18:04:39.000000 lcz-0.1.6/src/lcz/weights/__init__.py
+-rwxr-xr-x   0 m4rs      (1000) m4rs      (1000)  1262607 2024-05-01 18:04:39.000000 lcz-0.1.6/src/lcz/weights/maia-1900.pb.gz
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-05-01 18:04:39.000000 lcz-0.1.6/src/lcz/weights/weights.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-01 18:09:05.399057 lcz-0.1.6/src/lcz.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1214 2024-05-01 18:09:05.000000 lcz-0.1.6/src/lcz.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      348 2024-05-01 18:09:05.000000 lcz-0.1.6/src/lcz.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-01 18:09:05.000000 lcz-0.1.6/src/lcz.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-05-01 18:09:05.000000 lcz-0.1.6/src/lcz.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        4 2024-05-01 18:09:05.000000 lcz-0.1.6/src/lcz.egg-info/top_level.txt
```

### Comparing `lcz-0.1.4/src/lcz/main.py` & `lcz-0.1.6/src/lcz/main.py`

 * *Files identical despite different names*

### Comparing `lcz-0.1.4/src/lcz/weights/maia-1900.pb.gz` & `lcz-0.1.6/src/lcz/weights/maia-1900.pb.gz`

 * *Files identical despite different names*

