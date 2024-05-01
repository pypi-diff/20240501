# Comparing `tmp/lsst-resources-26.2024.500.tar.gz` & `tmp/lsst_resources-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-resources-26.2024.500.tar", last modified: Thu Feb  1 10:58:10 2024, max compression
+gzip compressed data, was "lsst_resources-27.0.0rc1.tar", last modified: Wed May  1 21:17:10 2024, max compression
```

## Comparing `lsst-resources-26.2024.500.tar` & `lsst_resources-27.0.0rc1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/doc/lsst.resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.707503 lsst-resources-26.2024.500/python/lsst/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.707503 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    57585 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourcePath.py
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/packageresource.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20076 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/schemeless.py
--rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst/resources/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/python/lsst_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38967 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_schemeless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.747386 lsst_resources-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.735386 lsst_resources-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/doc/lsst.resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/doc/lsst.resources/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.735386 lsst_resources-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.739386 lsst_resources-27.0.0rc1/python/lsst/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57619 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/_resourcePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/packageresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/schemeless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/python/lsst/resources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst/resources/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:17:10.000000 lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-01 21:17:10.747386 lsst_resources-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:10.743386 lsst_resources-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-01 21:17:04.000000 lsst_resources-27.0.0rc1/tests/test_schemeless.py
```

### Comparing `lsst-resources-26.2024.500/LICENSE` & `lsst_resources-27.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/PKG-INFO` & `lsst_resources-27.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 26.2024.500
+Version: 27.0.0rc1
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-resources-26.2024.500/README.md` & `lsst_resources-27.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/doc/lsst.resources/CHANGES.rst` & `lsst_resources-27.0.0rc1/doc/lsst.resources/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/doc/lsst.resources/index.rst` & `lsst_resources-27.0.0rc1/doc/lsst.resources/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/pyproject.toml` & `lsst_resources-27.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/__init__.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_baseResourceHandle.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_baseResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_fileResourceHandle.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_fileResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_httpResourceHandle.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_httpResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/_resourcePath.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/_resourcePath.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         """Return the base root URI.
 
         Returns
         -------
         uri : `ResourcePath`
             Root URI.
         """
-        return self.replace(path="", forceDirectory=True)
+        return self.replace(path="", query="", fragment="", params="", forceDirectory=True)
 
     def split(self) -> tuple[ResourcePath, str]:
         """Split URI into head and tail.
 
         Returns
         -------
         head: `ResourcePath`
```

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/file.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/file.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/gs.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/gs.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/http.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/http.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/location.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/location.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/mem.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/mem.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/packageresource.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/packageresource.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/s3.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -188,62 +188,97 @@
             transfer_config = TransferConfig(use_threads=self.use_threads)
 
         return transfer_config
 
     @property
     def client(self) -> boto3.client:
         """Client object to address remote resource."""
-        # Defer import for circular dependencies
-        return getS3Client()
+        return getS3Client(self._profile)
+
+    @property
+    def _profile(self) -> str | None:
+        """Profile name to use for looking up S3 credentials and endpoint."""
+        return self._uri.username
+
+    @property
+    def _bucket(self) -> str:
+        """S3 bucket where the files are stored."""
+        # Notionally the bucket is stored in the 'hostname' part of the URI.
+        # However, Ceph S3 uses a "multi-tenant" syntax for bucket names in the
+        # form 'tenant:bucket'.  The part after the colon is parsed as the port
+        # portion of the URI, and urllib throws an exception if you try to read
+        # a non-integer port value.  So manually split off this portion of the
+        # URI.
+        split = self._uri.netloc.split("@")
+        num_components = len(split)
+        if num_components == 2:
+            # There is a profile@ portion of the URL, so take the second half.
+            bucket = split[1]
+        elif num_components == 1:
+            # There is no profile@, so take the whole netloc.
+            bucket = split[0]
+        else:
+            raise ValueError(f"Unexpected extra '@' in S3 URI: '{str(self)}'")
+
+        if not bucket:
+            raise ValueError(f"S3 URI does not include bucket name: '{str(self)}'")
+
+        return bucket
 
     @classmethod
     def _mexists(cls, uris: Iterable[ResourcePath]) -> dict[ResourcePath, bool]:
-        # Force client to be created before creating threads.
-        getS3Client()
+        # Force client to be created for each profile before creating threads.
+        profiles = set[str | None]()
+        for path in uris:
+            if path.scheme == "s3":
+                path = cast(S3ResourcePath, path)
+                profiles.add(path._profile)
+        for profile in profiles:
+            getS3Client(profile)
 
         return super()._mexists(uris)
 
     @backoff.on_exception(backoff.expo, retryable_io_errors, max_time=max_retry_time)
     def exists(self) -> bool:
         """Check that the S3 resource exists."""
         if self.is_root:
             # Only check for the bucket since the path is irrelevant
-            return bucketExists(self.netloc)
-        exists, _ = s3CheckFileExists(self, client=self.client)
+            return bucketExists(self._bucket, self.client)
+        exists, _ = s3CheckFileExists(self, bucket=self._bucket, client=self.client)
         return exists
 
     @backoff.on_exception(backoff.expo, retryable_io_errors, max_time=max_retry_time)
     def size(self) -> int:
         """Return the size of the resource in bytes."""
         if self.dirLike:
             return 0
-        exists, sz = s3CheckFileExists(self, client=self.client)
+        exists, sz = s3CheckFileExists(self, bucket=self._bucket, client=self.client)
         if not exists:
             raise FileNotFoundError(f"Resource {self} does not exist")
         return sz
 
     @backoff.on_exception(backoff.expo, retryable_io_errors, max_time=max_retry_time)
     def remove(self) -> None:
         """Remove the resource."""
         # https://github.com/boto/boto3/issues/507 - there is no
         # way of knowing if the file was actually deleted except
         # for checking all the keys again, reponse is  HTTP 204 OK
         # response all the time
         try:
-            self.client.delete_object(Bucket=self.netloc, Key=self.relativeToPathRoot)
+            self.client.delete_object(Bucket=self._bucket, Key=self.relativeToPathRoot)
         except (self.client.exceptions.NoSuchKey, self.client.exceptions.NoSuchBucket) as err:
             raise FileNotFoundError("No such resource: {self}") from err
 
     @backoff.on_exception(backoff.expo, all_retryable_errors, max_time=max_retry_time)
     def read(self, size: int = -1) -> bytes:
         args = {}
         if size > 0:
             args["Range"] = f"bytes=0-{size-1}"
         try:
-            response = self.client.get_object(Bucket=self.netloc, Key=self.relativeToPathRoot, **args)
+            response = self.client.get_object(Bucket=self._bucket, Key=self.relativeToPathRoot, **args)
         except (self.client.exceptions.NoSuchKey, self.client.exceptions.NoSuchBucket) as err:
             raise FileNotFoundError(f"No such resource: {self}") from err
         except ClientError as err:
             _translate_client_error(err)
             raise
         with time_this(log, msg="Read from %s", args=(self,)):
             body = response["Body"].read()
@@ -251,39 +286,39 @@
         return body
 
     @backoff.on_exception(backoff.expo, all_retryable_errors, max_time=max_retry_time)
     def write(self, data: bytes, overwrite: bool = True) -> None:
         if not overwrite and self.exists():
             raise FileExistsError(f"Remote resource {self} exists and overwrite has been disabled")
         with time_this(log, msg="Write to %s", args=(self,)):
-            self.client.put_object(Bucket=self.netloc, Key=self.relativeToPathRoot, Body=data)
+            self.client.put_object(Bucket=self._bucket, Key=self.relativeToPathRoot, Body=data)
 
     @backoff.on_exception(backoff.expo, all_retryable_errors, max_time=max_retry_time)
     def mkdir(self) -> None:
         """Write a directory key to S3."""
-        if not bucketExists(self.netloc):
-            raise ValueError(f"Bucket {self.netloc} does not exist for {self}!")
+        if not bucketExists(self._bucket, self.client):
+            raise ValueError(f"Bucket {self._bucket} does not exist for {self}!")
 
         if not self.dirLike:
             raise NotADirectoryError(f"Can not create a 'directory' for file-like URI {self}")
 
         # don't create S3 key when root is at the top-level of an Bucket
         if self.path != "/":
-            self.client.put_object(Bucket=self.netloc, Key=self.relativeToPathRoot)
+            self.client.put_object(Bucket=self._bucket, Key=self.relativeToPathRoot)
 
     @backoff.on_exception(backoff.expo, all_retryable_errors, max_time=max_retry_time)
     def _download_file(self, local_file: IO, progress: ProgressPercentage | None) -> None:
         """Download the remote resource to a local file.
 
         Helper routine for _as_local to allow backoff without regenerating
         the temporary file.
         """
         try:
             self.client.download_fileobj(
-                self.netloc,
+                self._bucket,
                 self.relativeToPathRoot,
                 local_file,
                 Callback=progress,
                 Config=self._transfer_config,
             )
         except (
             self.client.exceptions.NoSuchKey,
@@ -320,30 +355,30 @@
     def _upload_file(self, local_file: ResourcePath, progress: ProgressPercentage | None) -> None:
         """Upload a local file with backoff.
 
         Helper method to wrap file uploading in backoff for transfer_from.
         """
         try:
             self.client.upload_file(
-                local_file.ospath, self.netloc, self.relativeToPathRoot, Callback=progress
+                local_file.ospath, self._bucket, self.relativeToPathRoot, Callback=progress
             )
         except self.client.exceptions.NoSuchBucket as err:
             raise NotADirectoryError(f"Target does not exist: {err}") from err
         except ClientError as err:
             _translate_client_error(err)
             raise
 
     @backoff.on_exception(backoff.expo, all_retryable_errors, max_time=max_retry_time)
-    def _copy_from(self, src: ResourcePath) -> None:
+    def _copy_from(self, src: S3ResourcePath) -> None:
         copy_source = {
-            "Bucket": src.netloc,
+            "Bucket": src._bucket,
             "Key": src.relativeToPathRoot,
         }
         try:
-            self.client.copy_object(CopySource=copy_source, Bucket=self.netloc, Key=self.relativeToPathRoot)
+            self.client.copy_object(CopySource=copy_source, Bucket=self._bucket, Key=self.relativeToPathRoot)
         except (self.client.exceptions.NoSuchKey, self.client.exceptions.NoSuchBucket) as err:
             raise FileNotFoundError("No such resource to transfer: {self}") from err
         except ClientError as err:
             _translate_client_error(err)
             raise
 
     def transfer_from(
@@ -465,15 +500,15 @@
         # them all grouped properly across the 1000 limit boundary.
         prefix = self.relativeToPathRoot if not self.is_root else ""
         prefix_len = len(prefix)
         dirnames = []
         filenames = []
         files_there = False
 
-        for page in s3_paginator.paginate(Bucket=self.netloc, Prefix=prefix, Delimiter="/"):
+        for page in s3_paginator.paginate(Bucket=self._bucket, Prefix=prefix, Delimiter="/"):
             # All results are returned as full key names and we must
             # convert them back to the root form. The prefix is fixed
             # and delimited so that is a simple trim
 
             # Directories are reported in the CommonPrefixes result
             # which reports the entire key and must be stripped.
             found_dirs = [dir["Prefix"][prefix_len:] for dir in page.get("CommonPrefixes", ())]
@@ -503,15 +538,15 @@
     @contextlib.contextmanager
     def _openImpl(
         self,
         mode: str = "r",
         *,
         encoding: str | None = None,
     ) -> Iterator[ResourceHandleProtocol]:
-        with S3ResourceHandle(mode, log, self.client, self.netloc, self.relativeToPathRoot) as handle:
+        with S3ResourceHandle(mode, log, self.client, self._bucket, self.relativeToPathRoot) as handle:
             if "b" in mode:
                 yield handle
             else:
                 if encoding is None:
                     encoding = sys.getdefaultencoding()
                 # cast because the protocol is compatible, but does not have
                 # BytesIO in the inheritance tree
@@ -525,10 +560,10 @@
     def generate_presigned_put_url(self, *, expiration_time_seconds: int) -> str:
         # Docstring inherited
         return self._generate_presigned_url("put_object", expiration_time_seconds)
 
     def _generate_presigned_url(self, method: str, expiration_time_seconds: int) -> str:
         return self.client.generate_presigned_url(
             method,
-            Params={"Bucket": self.netloc, "Key": self.relativeToPathRoot},
+            Params={"Bucket": self._bucket, "Key": self.relativeToPathRoot},
             ExpiresIn=expiration_time_seconds,
         )
```

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/s3utils.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/s3utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,25 +26,27 @@
     "_TooManyRequestsError",
     "clean_test_environment_for_s3",
 )
 
 import functools
 import os
 import re
+import urllib.parse
 from collections.abc import Callable, Iterator
 from contextlib import contextmanager
 from http.client import HTTPException, ImproperConnectionState
 from types import ModuleType
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, NamedTuple, cast
 from unittest.mock import patch
 
 from botocore.exceptions import ClientError
 from botocore.handlers import validate_bucket_name
 from deprecated.sphinx import deprecated
 from urllib3.exceptions import HTTPError, RequestError
+from urllib3.util import Url, parse_url
 
 if TYPE_CHECKING:
     from unittest import TestCase
 
 
 try:
     import boto3
@@ -174,58 +176,127 @@
         # This helps us avoid a potential situation where the client could be
         # instantiated before moto mocks are installed, which would prevent the
         # mocks from taking effect.
         _get_s3_client.cache_clear()
         yield
 
 
-def getS3Client() -> boto3.client:
+def getS3Client(profile: str | None = None) -> boto3.client:
     """Create a S3 client with AWS (default) or the specified endpoint.
 
+    Parameters
+    ----------
+    profile : `str`, optional
+        The name of an S3 profile describing which S3 service to use.
+
     Returns
     -------
     s3client : `botocore.client.S3`
         A client of the S3 service.
 
     Notes
     -----
-    The endpoint URL is from the environment variable S3_ENDPOINT_URL.
-    If none is specified, the default AWS one is used.
+    If an explicit profile name is specified, its configuration will be read
+    from an environment variable named ``LSST_RESOURCES_S3_PROFILE_<profile>``
+    if it exists.  Note that the name of the profile is case sensitive.  This
+    configuration is specified in the format: ``https://<access key ID>:<secret
+    key>@<s3 endpoint hostname>``. If the access key ID or secret key values
+    contain slashes, the slashes must be URI-encoded (replace "/" with "%2F").
+
+    If profile is `None` or the profile environment variable was not set, the
+    configuration is read from the environment variable ``S3_ENDPOINT_URL``.
+    If it is not specified, the default AWS endpoint is used.
+
+    The access key ID and secret key are optional -- if not specified, they
+    will be looked up via the `AWS credentials file
+    <https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html>`_.
 
     If the environment variable LSST_DISABLE_BUCKET_VALIDATION exists
     and has a value that is not empty, "0", "f", "n", or "false"
     (case-insensitive), then bucket name validation is disabled.  This
     disabling allows Ceph multi-tenancy colon separators to appear in
     bucket names.
     """
     if boto3 is None:
         raise ModuleNotFoundError("Could not find boto3. Are you sure it is installed?")
     if botocore is None:
         raise ModuleNotFoundError("Could not find botocore. Are you sure it is installed?")
 
-    endpoint = os.environ.get("S3_ENDPOINT_URL", None)
+    endpoint = None
+    if profile is not None:
+        var_name = f"LSST_RESOURCES_S3_PROFILE_{profile}"
+        endpoint = os.environ.get(var_name, None)
+    if not endpoint:
+        endpoint = os.environ.get("S3_ENDPOINT_URL", None)
     if not endpoint:
         endpoint = None  # Handle ""
+
     disable_value = os.environ.get("LSST_DISABLE_BUCKET_VALIDATION", "0")
     skip_validation = not re.search(r"^(0|f|n|false)?$", disable_value, re.I)
 
-    return _get_s3_client(endpoint, skip_validation)
+    return _get_s3_client(endpoint, profile, skip_validation)
 
 
 @functools.lru_cache
-def _get_s3_client(endpoint: str, skip_validation: bool) -> boto3.client:
+def _get_s3_client(endpoint: str | None, profile: str | None, skip_validation: bool) -> boto3.client:
     # Helper function to cache the client for this endpoint
     config = botocore.config.Config(read_timeout=180, retries={"mode": "adaptive", "max_attempts": 10})
 
-    client = boto3.client("s3", endpoint_url=endpoint, config=config)
+    endpoint_config = _parse_endpoint_config(endpoint)
+
+    if endpoint_config.access_key_id is not None and endpoint_config.secret_access_key is not None:
+        # We already have the necessary configuration for the profile, so do
+        # not pass the profile to boto3.  boto3 will raise an exception if the
+        # profile is not defined in its configuration file, whether or not it
+        # needs to read the configuration from it.
+        profile = None
+    session = boto3.Session(profile_name=profile)
+
+    client = session.client(
+        "s3",
+        endpoint_url=endpoint_config.endpoint_url,
+        aws_access_key_id=endpoint_config.access_key_id,
+        aws_secret_access_key=endpoint_config.secret_access_key,
+        config=config,
+    )
     if skip_validation:
         client.meta.events.unregister("before-parameter-build.s3", validate_bucket_name)
     return client
 
 
+class _EndpointConfig(NamedTuple):
+    endpoint_url: str | None = None
+    access_key_id: str | None = None
+    secret_access_key: str | None = None
+
+
+def _parse_endpoint_config(endpoint: str | None) -> _EndpointConfig:
+    if not endpoint:
+        return _EndpointConfig()
+
+    parsed = parse_url(endpoint)
+
+    # Strip the username/password portion of the URL from the result.
+    endpoint_url = Url(host=parsed.host, path=parsed.path, port=parsed.port, scheme=parsed.scheme).url
+
+    access_key_id = None
+    secret_access_key = None
+    if parsed.auth:
+        split = parsed.auth.split(":")
+        if len(split) != 2:
+            raise ValueError("S3 access key and secret not in expected format.")
+        access_key_id, secret_access_key = split
+        access_key_id = urllib.parse.unquote(access_key_id)
+        secret_access_key = urllib.parse.unquote(secret_access_key)
+
+    return _EndpointConfig(
+        endpoint_url=endpoint_url, access_key_id=access_key_id, secret_access_key=secret_access_key
+    )
+
+
 def s3CheckFileExists(
     path: Location | ResourcePath | str,
     bucket: str | None = None,
     client: boto3.client | None = None,
 ) -> tuple[bool, int]:
     """Return if the file exists in the bucket or not.
 
@@ -264,15 +335,16 @@
         if bucket is not None:
             filepath = path
         else:
             uri = ResourcePath(path)
             bucket = uri.netloc
             filepath = uri.relativeToPathRoot
     elif isinstance(path, ResourcePath | Location):
-        bucket = path.netloc
+        if bucket is None:
+            bucket = path.netloc
         filepath = path.relativeToPathRoot
     else:
         raise TypeError(f"Unsupported path type: {path!r}.")
 
     try:
         obj = client.head_object(Bucket=bucket, Key=filepath)
         return (True, obj["ContentLength"])
```

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/schemeless.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/schemeless.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/tests.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst/resources/utils.py` & `lsst_resources-27.0.0rc1/python/lsst/resources/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/python/lsst_resources.egg-info/PKG-INFO` & `lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 26.2024.500
+Version: 27.0.0rc1
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-resources-26.2024.500/python/lsst_resources.egg-info/SOURCES.txt` & `lsst_resources-27.0.0rc1/python/lsst_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_file.py` & `lsst_resources-27.0.0rc1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_gs.py` & `lsst_resources-27.0.0rc1/tests/test_gs.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_http.py` & `lsst_resources-27.0.0rc1/tests/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,37 @@
 
 class GenericHttpTestCase(GenericTestCase, unittest.TestCase):
     """Generic tests of http URIs."""
 
     scheme = "http"
     netloc = "server.example"
 
+    def test_root_uri(self):
+        self.assertEqual(ResourcePath("http://server.com").root_uri(), ResourcePath("http://server.com/"))
+        self.assertEqual(
+            ResourcePath("http://user:password@server.com:3000/").root_uri(),
+            ResourcePath("http://user:password@server.com:3000/"),
+        )
+        self.assertEqual(
+            ResourcePath("http://user:password@server.com:3000/some/path").root_uri(),
+            ResourcePath("http://user:password@server.com:3000/"),
+        )
+        self.assertEqual(
+            ResourcePath("http://user:password@server.com:3000/some/path#fragment").root_uri(),
+            ResourcePath("http://user:password@server.com:3000/"),
+        )
+        self.assertEqual(
+            ResourcePath("http://user:password@server.com:3000/some/path?param=value").root_uri(),
+            ResourcePath("http://user:password@server.com:3000/"),
+        )
+        self.assertEqual(
+            ResourcePath("http://user:password@server.com:3000/some/path;parameters").root_uri(),
+            ResourcePath("http://user:password@server.com:3000/"),
+        )
+
 
 class HttpReadWriteWebdavTestCase(GenericReadWriteTestCase, unittest.TestCase):
     """Test with a real webDAV server, as opposed to mocking responses."""
 
     scheme = "http"
 
     @classmethod
```

### Comparing `lsst-resources-26.2024.500/tests/test_location.py` & `lsst_resources-27.0.0rc1/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_mem.py` & `lsst_resources-27.0.0rc1/tests/test_mem.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_resource.py` & `lsst_resources-27.0.0rc1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.500/tests/test_s3.py` & `lsst_resources-27.0.0rc1/tests/test_s3.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,53 +40,47 @@
 class GenericS3TestCase(GenericTestCase, unittest.TestCase):
     """Generic tests of S3 URIs."""
 
     scheme = "s3"
     netloc = "my_bucket"
 
 
-@unittest.skipIf(not boto3, "Warning: boto3 AWS SDK not found!")
-class S3ReadWriteTestCase(GenericReadWriteTestCase, unittest.TestCase):
+class S3ReadWriteTestCaseBase(GenericReadWriteTestCase):
     """Tests of reading and writing S3 URIs."""
 
     scheme = "s3"
-    netloc = "my_2nd_bucket"
-
-    mock_aws = mock_aws()
-    """The mocked s3 interface from moto."""
+    s3_endpoint_url: str | None = None
 
     def setUp(self):
         self.enterContext(clean_test_environment_for_s3())
+
         # Enable S3 mocking of tests.
-        self.mock_aws.start()
+        self.enterContext(mock_aws())
 
         # MOTO needs to know that we expect Bucket bucketname to exist
-        s3 = boto3.resource("s3")
-        s3.create_bucket(Bucket=self.netloc)
+        s3 = boto3.resource("s3", endpoint_url=self.s3_endpoint_url)
+        s3.create_bucket(Bucket=self.bucket)
 
         super().setUp()
 
     def tearDown(self):
         s3 = boto3.resource("s3")
-        bucket = s3.Bucket(self.netloc)
+        bucket = s3.Bucket(self.bucket)
         try:
             bucket.objects.all().delete()
         except botocore.exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "404":
                 # the key was not reachable - pass
                 pass
             else:
                 raise
 
-        bucket = s3.Bucket(self.netloc)
+        bucket = s3.Bucket(self.bucket)
         bucket.delete()
 
-        # Stop the S3 mock.
-        self.mock_aws.stop()
-
         S3ResourcePath.use_threads = None
 
         super().tearDown()
 
     def test_bucket_fail(self):
         # Deliberately create URI with unknown bucket.
         uri = ResourcePath("s3://badbucket/something/")
@@ -219,9 +213,80 @@
             S3ResourcePath.use_threads = None
             test_resource_path = self.root_uri.join("test_file.dat")
             self.assertFalse(test_resource_path._transfer_config.use_threads)
 
             self.test_local()
 
 
+@unittest.skipIf(not boto3, "Warning: boto3 AWS SDK not found!")
+class S3ReadWriteTestCase(S3ReadWriteTestCaseBase, unittest.TestCase):
+    """Test S3 with no explicit profile/endpoint specified.
+    (``s3://bucketname/...``).
+    """
+
+    bucket = "my_2nd_bucket"
+    netloc = bucket
+
+
+@unittest.skipIf(not boto3, "Warning: boto3 AWS SDK not found!")
+class S3WithProfileReadWriteTestCase(S3ReadWriteTestCaseBase, unittest.TestCase):
+    """Test S3 URLs with explicit profile specified.
+    (``s3://profile@bucketname/...``).
+    """
+
+    bucket = "3rd_bucket"
+    netloc = f"myprofile@{bucket}"
+    s3_endpoint_url = "https://endpoint1.test.example"
+
+    def setUp(self):
+        # Configure custom S3 endpoints that we can target from tests using
+        # non-default profile.
+        self.enterContext(
+            mock.patch.dict(
+                os.environ,
+                {
+                    "MOTO_S3_CUSTOM_ENDPOINTS": self.s3_endpoint_url,
+                    "LSST_RESOURCES_S3_PROFILE_myprofile": "https://access_key:security_key@endpoint1.test.example",
+                },
+            )
+        )
+
+        super().setUp()
+
+    def test_missing_profile(self):
+        with self.assertRaises(botocore.exceptions.ProfileNotFound):
+            ResourcePath("s3://otherprofile@bucket").read()
+
+    def test_s3_endpoint_url(self):
+        with mock.patch.dict(
+            os.environ,
+            {"S3_ENDPOINT_URL": self.s3_endpoint_url},
+        ):
+            path = ResourcePath(f"s3://{self.bucket}/test-s3-endpoint-url.txt")
+            data = b"123"
+            path.write(data)
+            self.assertEqual(path.read(), data)
+            self.assertIn(
+                "https://endpoint1.test.example",
+                path.generate_presigned_get_url(expiration_time_seconds=3600),
+            )
+
+    def test_uri_syntax(self):
+        path1 = ResourcePath("s3://profile@bucket/path")
+        self.assertEqual(path1._bucket, "bucket")
+        self.assertEqual(path1._profile, "profile")
+        path2 = ResourcePath("s3://bucket2/path")
+        self.assertEqual(path2._bucket, "bucket2")
+        self.assertIsNone(path2._profile)
+
+    def test_ceph_uri_syntax(self):
+        # The Ceph S3 'multi-tenant' syntax for buckets can include colons.
+        path1 = ResourcePath("s3://profile@ceph:bucket/path")
+        self.assertEqual(path1._bucket, "ceph:bucket")
+        self.assertEqual(path1._profile, "profile")
+        path2 = ResourcePath("s3://ceph:bucket2/path")
+        self.assertEqual(path2._bucket, "ceph:bucket2")
+        self.assertIsNone(path2._profile)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-resources-26.2024.500/tests/test_s3utils.py` & `lsst_resources-27.0.0rc1/tests/test_s3utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,15 +32,22 @@
     except ImportError:
         from moto import mock_s3 as mock_aws
 except ImportError:
     boto3 = None
 
 from lsst.resources import ResourcePath
 from lsst.resources.location import Location
-from lsst.resources.s3utils import bucketExists, clean_test_environment_for_s3, getS3Client, s3CheckFileExists
+from lsst.resources.s3utils import (
+    _parse_endpoint_config,
+    bucketExists,
+    clean_test_environment_for_s3,
+    getS3Client,
+    s3CheckFileExists,
+)
+from urllib3.exceptions import LocationParseError
 
 
 @unittest.skipIf(not boto3, "Warning: boto3 AWS SDK not found!")
 class S3UtilsTestCase(unittest.TestCase):
     """Test for the S3 related utilities."""
 
     bucketName = "test_bucket_name"
@@ -97,10 +104,31 @@
         self.assertTrue(s3CheckFileExists(buri, client=self.client)[0])
         self.assertTrue(s3CheckFileExists(client=self.client, path=location)[0])
 
         # make sure supplying strings resolves correctly too
         self.assertTrue(s3CheckFileExists(uri, client=self.client))
         self.assertTrue(s3CheckFileExists(uri))
 
+    def test_parsing_profile_config(self):
+        with self.assertRaises(LocationParseError):
+            _parse_endpoint_config(
+                "https://AKIAIOSFODNN7EXAMPLE:wJalrXUtnFEMI/FK7MDENG/FbPxRfiCYEXAMPLEKEY@endpoint.com"
+            )
+
+        parsed = _parse_endpoint_config(
+            "https://AKIAIOSFODNN7EXAMPLE:wJalrXUtnFEMI%2FK7MDENG%2FbPxRfiCYEXAMPLEKEY@endpoint.com"
+        )
+        self.assertEqual(parsed.endpoint_url, "https://endpoint.com")
+        self.assertEqual(parsed.access_key_id, "AKIAIOSFODNN7EXAMPLE")
+        self.assertEqual(parsed.secret_access_key, "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY")
+
+        simple = _parse_endpoint_config("https://other.endpoint.com")
+        self.assertEqual(simple.endpoint_url, "https://other.endpoint.com")
+        self.assertIsNone(simple.access_key_id)
+        self.assertIsNone(simple.secret_access_key)
+
+        with self.assertRaisesRegex(ValueError, "S3 access key and secret not in expected format."):
+            _parse_endpoint_config("https://key@endpoint.com")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-resources-26.2024.500/tests/test_schemeless.py` & `lsst_resources-27.0.0rc1/tests/test_schemeless.py`

 * *Files identical despite different names*

