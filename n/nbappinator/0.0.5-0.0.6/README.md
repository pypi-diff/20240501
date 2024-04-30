# Comparing `tmp/nbappinator-0.0.5.tar.gz` & `tmp/nbappinator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.0.5.tar", last modified: Tue Apr 30 20:16:12 2024, max compression
+gzip compressed data, was "nbappinator-0.0.6.tar", last modified: Tue Apr 30 23:08:06 2024, max compression
```

## Comparing `nbappinator-0.0.5.tar` & `nbappinator-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:16:12.281721 nbappinator-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 20:15:22.000000 nbappinator-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 20:16:12.281721 nbappinator-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:16:12.277722 nbappinator-0.0.5/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-30 20:15:22.000000 nbappinator-0.0.5/nbappinator/treew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:16:12.277722 nbappinator-0.0.5/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 20:16:12.000000 nbappinator-0.0.5/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 20:16:12.000000 nbappinator-0.0.5/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:16:12.000000 nbappinator-0.0.5/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 20:16:12.000000 nbappinator-0.0.5/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 20:16:12.000000 nbappinator-0.0.5/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 20:15:22.000000 nbappinator-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-30 20:15:22.000000 nbappinator-0.0.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-30 20:16:12.281721 nbappinator-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.073922 nbappinator-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 23:07:15.000000 nbappinator-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 23:08:06.073922 nbappinator-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.069922 nbappinator-0.0.6/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-30 23:07:15.000000 nbappinator-0.0.6/nbappinator/treew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:06.069922 nbappinator-0.0.6/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 23:08:06.000000 nbappinator-0.0.6/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 23:07:15.000000 nbappinator-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-30 23:07:15.000000 nbappinator-0.0.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 23:08:06.073922 nbappinator-0.0.6/setup.cfg
```

### Comparing `nbappinator-0.0.5/LICENSE.md` & `nbappinator-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/nbappinator/aggridhelper.py` & `nbappinator-0.0.6/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/nbappinator/appinator.py` & `nbappinator-0.0.6/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/nbappinator/datagrid.py` & `nbappinator-0.0.6/nbappinator/datagrid.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/nbappinator/plotly_charts.py` & `nbappinator-0.0.6/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/nbappinator/treew.py` & `nbappinator-0.0.6/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.0.5/pyproject.toml` & `nbappinator-0.0.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "nbappinator"
-version = "0.0.5"
+version = "0.0.6"
 description = "Jupyter Notebook Application Builder"
 authors = [{ name = "Paul Timmins", email = "paul@iqmo.com" }]
-dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid>=0.5.4", "ipytree", "pandas>=1.5.3"]
+dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
 readme = "README.md"
 
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nbappinator-0.0.5/readme.md` & `nbappinator-0.0.6/readme.md`

 * *Files identical despite different names*

