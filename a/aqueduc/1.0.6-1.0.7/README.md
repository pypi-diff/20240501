# Comparing `tmp/aqueduc-1.0.6.tar.gz` & `tmp/aqueduc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduc-1.0.6.tar", last modified: Wed May  1 07:33:31 2024, max compression
+gzip compressed data, was "aqueduc-1.0.7.tar", last modified: Wed May  1 07:58:37 2024, max compression
```

## Comparing `aqueduc-1.0.6.tar` & `aqueduc-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:33:31.474032 aqueduc-1.0.6/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.6/LICENSE
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-05-01 07:33:31.474032 aqueduc-1.0.6/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.6/README.md
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      362 2024-05-01 07:30:38.000000 aqueduc-1.0.6/pyproject.toml
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-05-01 07:33:31.474032 aqueduc-1.0.6/setup.cfg
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.6/setup.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:33:31.474032 aqueduc-1.0.6/src/
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:33:31.474032 aqueduc-1.0.6/src/aqueduc/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       84 2024-04-30 11:44:58.000000 aqueduc-1.0.6/src/aqueduc/__main__.py
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.6/src/aqueduc/aqueduc.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:33:31.474032 aqueduc-1.0.6/src/aqueduc.egg-info/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-05-01 07:33:31.000000 aqueduc-1.0.6/src/aqueduc.egg-info/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      278 2024-05-01 07:33:31.000000 aqueduc-1.0.6/src/aqueduc.egg-info/SOURCES.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-05-01 07:33:31.000000 aqueduc-1.0.6/src/aqueduc.egg-info/dependency_links.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       50 2024-05-01 07:33:31.000000 aqueduc-1.0.6/src/aqueduc.egg-info/entry_points.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-05-01 07:33:31.000000 aqueduc-1.0.6/src/aqueduc.egg-info/top_level.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.6/src/test.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:58:37.333574 aqueduc-1.0.7/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.7/LICENSE
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-05-01 07:58:37.333574 aqueduc-1.0.7/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.7/README.md
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      362 2024-05-01 07:57:42.000000 aqueduc-1.0.7/pyproject.toml
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-05-01 07:58:37.333574 aqueduc-1.0.7/setup.cfg
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.7/setup.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:58:37.323574 aqueduc-1.0.7/src/
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:58:37.323574 aqueduc-1.0.7/src/aqueduc/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       85 2024-05-01 07:54:33.000000 aqueduc-1.0.7/src/aqueduc/__main__.py
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4542 2024-04-30 11:44:13.000000 aqueduc-1.0.7/src/aqueduc/aqueduc.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-05-01 07:58:37.323574 aqueduc-1.0.7/src/aqueduc.egg-info/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-05-01 07:58:37.000000 aqueduc-1.0.7/src/aqueduc.egg-info/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      278 2024-05-01 07:58:37.000000 aqueduc-1.0.7/src/aqueduc.egg-info/SOURCES.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-05-01 07:58:37.000000 aqueduc-1.0.7/src/aqueduc.egg-info/dependency_links.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       50 2024-05-01 07:58:37.000000 aqueduc-1.0.7/src/aqueduc.egg-info/entry_points.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-05-01 07:58:37.000000 aqueduc-1.0.7/src/aqueduc.egg-info/top_level.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.7/src/test.py
```

### Comparing `aqueduc-1.0.6/LICENSE` & `aqueduc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.6/PKG-INFO` & `aqueduc-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.6
+Version: 1.0.7
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.6/README.md` & `aqueduc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.6/src/aqueduc/aqueduc.py` & `aqueduc-1.0.7/src/aqueduc/aqueduc.py`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.6/src/aqueduc.egg-info/PKG-INFO` & `aqueduc-1.0.7/src/aqueduc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.6
+Version: 1.0.7
 Author: Mozenn
 License: Copyright 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `aqueduc-1.0.6/src/test.py` & `aqueduc-1.0.7/src/test.py`

 * *Files identical despite different names*

