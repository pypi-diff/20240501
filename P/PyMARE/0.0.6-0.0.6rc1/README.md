# Comparing `tmp/PyMARE-0.0.6.tar.gz` & `tmp/PyMARE-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMARE-0.0.6.tar", last modified: Wed May  1 16:59:19 2024, max compression
+gzip compressed data, was "PyMARE-0.0.6rc1.tar", last modified: Wed May  1 16:58:03 2024, max compression
```

## Comparing `PyMARE-0.0.6.tar` & `PyMARE-0.0.6rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:59:11.000000 PyMARE-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 16:59:11.000000 PyMARE-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 16:59:19.778703 PyMARE-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.774703 PyMARE-0.0.6/PyMARE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:59:19.000000 PyMARE-0.0.6/PyMARE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-01 16:59:11.000000 PyMARE-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/datasets/metadat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/effectsize/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/effectsize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21695 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/effectsize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/effectsize/expressions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/effectsize/expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/estimators/combination.py
--rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/estimators/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.774703 PyMARE-0.0.6/pymare/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:19.778703 PyMARE-0.0.6/pymare/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/resources/datasets/michael2013.json
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/resources/datasets/michael2013.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pymare/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-01 16:59:11.000000 PyMARE-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-01 16:59:19.778703 PyMARE-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 16:59:11.000000 PyMARE-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    79886 2024-05-01 16:59:11.000000 PyMARE-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.631931 PyMARE-0.0.6rc1/PyMARE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:58:03.000000 PyMARE-0.0.6rc1/PyMARE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/datasets/metadat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/effectsize/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/effectsize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21695 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/effectsize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/effectsize/expressions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/effectsize/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/estimators/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/estimators/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.631931 PyMARE-0.0.6rc1/pymare/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/pymare/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/resources/datasets/michael2013.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/resources/datasets/michael2013.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pymare/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-01 16:58:03.635931 PyMARE-0.0.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79886 2024-05-01 16:57:54.000000 PyMARE-0.0.6rc1/versioneer.py
```

### Comparing `PyMARE-0.0.6/LICENSE` & `PyMARE-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/PKG-INFO` & `PyMARE-0.0.6rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
```

### Comparing `PyMARE-0.0.6/PyMARE.egg-info/PKG-INFO` & `PyMARE-0.0.6rc1/PyMARE.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
```

### Comparing `PyMARE-0.0.6/PyMARE.egg-info/SOURCES.txt` & `PyMARE-0.0.6rc1/PyMARE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/PyMARE.egg-info/requires.txt` & `PyMARE-0.0.6rc1/PyMARE.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/README.md` & `PyMARE-0.0.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/__init__.py` & `PyMARE-0.0.6rc1/pymare/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/core.py` & `PyMARE-0.0.6rc1/pymare/core.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/datasets/metadat.py` & `PyMARE-0.0.6rc1/pymare/datasets/metadat.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/effectsize/base.py` & `PyMARE-0.0.6rc1/pymare/effectsize/base.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/effectsize/expressions.json` & `PyMARE-0.0.6rc1/pymare/effectsize/expressions.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/effectsize/expressions.py` & `PyMARE-0.0.6rc1/pymare/effectsize/expressions.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/estimators/__init__.py` & `PyMARE-0.0.6rc1/pymare/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/estimators/combination.py` & `PyMARE-0.0.6rc1/pymare/estimators/combination.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/estimators/estimators.py` & `PyMARE-0.0.6rc1/pymare/estimators/estimators.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/resources/datasets/michael2013.json` & `PyMARE-0.0.6rc1/pymare/resources/datasets/michael2013.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/resources/datasets/michael2013.tsv` & `PyMARE-0.0.6rc1/pymare/resources/datasets/michael2013.tsv`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/results.py` & `PyMARE-0.0.6rc1/pymare/results.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/stats.py` & `PyMARE-0.0.6rc1/pymare/stats.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/pymare/utils.py` & `PyMARE-0.0.6rc1/pymare/utils.py`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/setup.cfg` & `PyMARE-0.0.6rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.6/versioneer.py` & `PyMARE-0.0.6rc1/versioneer.py`

 * *Files identical despite different names*

