# Comparing `tmp/dpd_lib-0.2.0.tar.gz` & `tmp/dpd_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.2.0.tar", last modified: Tue Apr 30 21:42:43 2024, max compression
+gzip compressed data, was "dpd_lib-0.2.1.tar", last modified: Tue Apr 30 22:48:47 2024, max compression
```

## Comparing `dpd_lib-0.2.0.tar` & `dpd_lib-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/PYPI.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 21:42:36.000000 dpd_lib-0.2.0/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 21:42:36.000000 dpd_lib-0.2.0/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11658 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-30 21:42:43.000000 dpd_lib-0.2.0/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-30 21:42:43.000000 dpd_lib-0.2.0/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 21:42:43.000000 dpd_lib-0.2.0/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-30 21:42:43.000000 dpd_lib-0.2.0/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-30 21:42:43.000000 dpd_lib-0.2.0/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-30 21:42:12.000000 dpd_lib-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 21:42:43.700652 dpd_lib-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 22:48:47.583387 dpd_lib-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-30 22:48:47.583387 dpd_lib-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/PYPI.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 22:48:47.575387 dpd_lib-0.2.1/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 22:48:39.000000 dpd_lib-0.2.1/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 22:48:47.583387 dpd_lib-0.2.1/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 22:48:39.000000 dpd_lib-0.2.1/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11658 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 22:48:47.583387 dpd_lib-0.2.1/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-30 22:48:47.000000 dpd_lib-0.2.1/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-30 22:48:47.000000 dpd_lib-0.2.1/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 22:48:47.000000 dpd_lib-0.2.1/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-30 22:48:47.000000 dpd_lib-0.2.1/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-30 22:48:47.000000 dpd_lib-0.2.1/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-30 22:46:23.000000 dpd_lib-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 22:48:47.583387 dpd_lib-0.2.1/setup.cfg
```

### Comparing `dpd_lib-0.2.0/PKG-INFO` & `dpd_lib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.2.0/PYPI.md` & `dpd_lib-0.2.1/PYPI.md`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.2.0/dpd_lib/client/exceptions.py` & `dpd_lib-0.2.1/dpd_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.2.0/dpd_lib/client/influx.py` & `dpd_lib-0.2.1/dpd_lib/client/influx.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.2.0/dpd_lib/config.py` & `dpd_lib-0.2.1/dpd_lib/config.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.2.0/dpd_lib/models.py` & `dpd_lib-0.2.1/dpd_lib/models.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.2.0/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.2.1/dpd_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.2.0/pyproject.toml` & `dpd_lib-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "PYPI.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

