# Comparing `tmp/kahi-0.0.8a0.tar.gz` & `tmp/kahi-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kahi-0.0.8a0.tar", last modified: Mon Apr 22 16:54:20 2024, max compression
+gzip compressed data, was "kahi-0.0.9a0.tar", last modified: Tue Apr 30 22:38:36 2024, max compression
```

## Comparing `kahi-0.0.8a0.tar` & `kahi-0.0.9a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:54:20.506930 kahi-0.0.8a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:54:20.502930 kahi-0.0.8a0/Kahi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-22 16:54:20.000000 kahi-0.0.8a0/Kahi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 16:54:20.000000 kahi-0.0.8a0/Kahi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:54:20.000000 kahi-0.0.8a0/Kahi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 16:54:20.000000 kahi-0.0.8a0/Kahi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 16:54:20.000000 kahi-0.0.8a0/Kahi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-22 16:54:12.000000 kahi-0.0.8a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 16:54:12.000000 kahi-0.0.8a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-22 16:54:20.506930 kahi-0.0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-22 16:54:12.000000 kahi-0.0.8a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:54:20.502930 kahi-0.0.8a0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-22 16:54:12.000000 kahi-0.0.8a0/bin/kahi_run
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:54:20.502930 kahi-0.0.8a0/kahi/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-22 16:54:12.000000 kahi-0.0.8a0/kahi/Kahi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 16:54:12.000000 kahi-0.0.8a0/kahi/KahiBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:54:12.000000 kahi-0.0.8a0/kahi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 16:54:12.000000 kahi-0.0.8a0/kahi/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:54:20.506930 kahi-0.0.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-22 16:54:12.000000 kahi-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:36.759411 kahi-0.0.9a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:36.755411 kahi-0.0.9a0/Kahi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-30 22:38:36.000000 kahi-0.0.9a0/Kahi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 22:38:36.000000 kahi-0.0.9a0/Kahi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:38:36.000000 kahi-0.0.9a0/Kahi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 22:38:36.000000 kahi-0.0.9a0/Kahi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 22:38:36.000000 kahi-0.0.9a0/Kahi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 22:38:28.000000 kahi-0.0.9a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 22:38:28.000000 kahi-0.0.9a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-30 22:38:36.759411 kahi-0.0.9a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-30 22:38:28.000000 kahi-0.0.9a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:36.755411 kahi-0.0.9a0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 22:38:28.000000 kahi-0.0.9a0/bin/kahi_run
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:36.755411 kahi-0.0.9a0/kahi/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-30 22:38:28.000000 kahi-0.0.9a0/kahi/Kahi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-30 22:38:28.000000 kahi-0.0.9a0/kahi/KahiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:28.000000 kahi-0.0.9a0/kahi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 22:38:28.000000 kahi-0.0.9a0/kahi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:38:36.759411 kahi-0.0.9a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-30 22:38:28.000000 kahi-0.0.9a0/setup.py
```

### Comparing `kahi-0.0.8a0/Kahi.egg-info/PKG-INFO` & `kahi-0.0.9a0/Kahi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kahi
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: ETL (Extract, Transform and Load) for bibliographic data using an advance data workflow
 Home-page: https://github.com/colav/Kahi
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kahi-0.0.8a0/LICENSE` & `kahi-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kahi-0.0.8a0/PKG-INFO` & `kahi-0.0.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kahi
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: ETL (Extract, Transform and Load) for bibliographic data using an advance data workflow
 Home-page: https://github.com/colav/Kahi
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kahi-0.0.8a0/README.md` & `kahi-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `kahi-0.0.8a0/bin/kahi_run` & `kahi-0.0.9a0/bin/kahi_run`

 * *Files identical despite different names*

### Comparing `kahi-0.0.8a0/kahi/Kahi.py` & `kahi-0.0.9a0/kahi/Kahi.py`

 * *Files identical despite different names*

### Comparing `kahi-0.0.8a0/kahi/KahiBase.py` & `kahi-0.0.9a0/kahi/KahiBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,16 @@
             "citations_count": [],
             "citations": [],
             "author_count": None,
             "authors": [],
             "source": {},
             "ranking": [],
             "subjects": [],
-            "citations_by_year": []
+            "citations_by_year": [],
+            "groups": []
         }
 
     def run(self):
         """
         entry point for the execution of the plugin, this method must be implemented
         """
         raise NotImplementedError(
```

### Comparing `kahi-0.0.8a0/setup.py` & `kahi-0.0.9a0/setup.py`

 * *Files identical despite different names*

