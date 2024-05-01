# Comparing `tmp/matplotlib_visual-0.9.6.tar.gz` & `tmp/matplotlib_visual-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_visual-0.9.6.tar", last modified: Sun Apr 21 14:56:38 2024, max compression
+gzip compressed data, was "matplotlib_visual-0.9.9.1.tar", last modified: Wed May  1 17:15:27 2024, max compression
```

## Comparing `matplotlib_visual-0.9.6.tar` & `matplotlib_visual-0.9.9.1.tar`

### file list

```diff
@@ -1,33 +1,19 @@
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-21 14:56:38.201890 matplotlib_visual-0.9.6/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.9.6/LICENSE
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-21 14:56:38.200890 matplotlib_visual-0.9.6/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.9.6/README.md
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-21 14:56:38.197890 matplotlib_visual-0.9.6/matplotlib_visual/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.9.6/matplotlib_visual/__init__.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-21 14:56:38.199890 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-04-21 14:34:56.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/1.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      643 2024-04-21 14:34:57.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-04-21 14:34:58.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-04-21 14:34:59.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     4903 2024-04-21 14:35:00.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      831 2024-04-21 14:55:32.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/55.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      354 2024-04-21 14:35:01.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1179 2024-04-21 14:35:25.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/66.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-04-21 14:35:02.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-04-21 14:35:03.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/__init__.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/ir5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1283 2024-04-10 14:05:44.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/ir5app.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1625 2024-04-10 14:06:38.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/ir5db.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1971 2024-04-21 14:34:52.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/ir5index.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-04-21 14:46:13.000000 matplotlib_visual-0.9.6/matplotlib_visual/code_snippets/z.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      769 2024-04-08 13:57:55.000000 matplotlib_visual-0.9.6/matplotlib_visual/graph.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-04-08 13:57:54.000000 matplotlib_visual-0.9.6/matplotlib_visual/models.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      376 2024-04-08 13:57:53.000000 matplotlib_visual-0.9.6/matplotlib_visual/piechart.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-21 14:56:38.200890 matplotlib_visual-0.9.6/matplotlib_visual.egg-info/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-21 14:56:38.000000 matplotlib_visual-0.9.6/matplotlib_visual.egg-info/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      924 2024-04-21 14:56:38.000000 matplotlib_visual-0.9.6/matplotlib_visual.egg-info/SOURCES.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-21 14:56:38.000000 matplotlib_visual-0.9.6/matplotlib_visual.egg-info/dependency_links.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-21 14:56:38.000000 matplotlib_visual-0.9.6/matplotlib_visual.egg-info/top_level.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-21 14:56:38.201890 matplotlib_visual-0.9.6/setup.cfg
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-04-21 14:56:17.000000 matplotlib_visual-0.9.6/setup.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 17:15:27.022271 matplotlib_visual-0.9.9.1/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/LICENSE
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      214 2024-05-01 17:15:27.021270 matplotlib_visual-0.9.9.1/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/README.md
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 17:15:27.020270 matplotlib_visual-0.9.9.1/matplotlib_visual/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/__init__.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 17:15:27.021270 matplotlib_visual-0.9.9.1/matplotlib_visual/code_snippets/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/code_snippets/__init__.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       22 2024-05-01 17:03:13.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/code_snippets/moo.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      696 2024-05-01 17:03:15.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/graph.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/models.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      376 2024-05-01 16:56:06.000000 matplotlib_visual-0.9.9.1/matplotlib_visual/piechart.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-05-01 17:15:27.021270 matplotlib_visual-0.9.9.1/matplotlib_visual.egg-info/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      214 2024-05-01 17:15:26.000000 matplotlib_visual-0.9.9.1/matplotlib_visual.egg-info/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      388 2024-05-01 17:15:26.000000 matplotlib_visual-0.9.9.1/matplotlib_visual.egg-info/SOURCES.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-05-01 17:15:26.000000 matplotlib_visual-0.9.9.1/matplotlib_visual.egg-info/dependency_links.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-05-01 17:15:26.000000 matplotlib_visual-0.9.9.1/matplotlib_visual.egg-info/top_level.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-05-01 17:15:27.022271 matplotlib_visual-0.9.9.1/setup.cfg
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      335 2024-05-01 17:14:32.000000 matplotlib_visual-0.9.9.1/setup.py
```

### Comparing `matplotlib_visual-0.9.6/LICENSE` & `matplotlib_visual-0.9.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.6/README.md` & `matplotlib_visual-0.9.9.1/README.md`

 * *Files identical despite different names*

