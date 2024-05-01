# Comparing `tmp/pulumi_rke-3.5.0a1714458609.tar.gz` & `tmp/pulumi_rke-3.5.0a1714544849.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rke-3.5.0a1714458609.tar", last modified: Tue Apr 30 06:43:04 2024, max compression
+gzip compressed data, was "pulumi_rke-3.5.0a1714544849.tar", last modified: Wed May  1 06:34:45 2024, max compression
```

## Comparing `pulumi_rke-3.5.0a1714458609.tar` & `pulumi_rke-3.5.0a1714544849.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/pulumi_rke/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   338457 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   138960 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/pulumi_rke/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)   304657 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-30 06:43:04.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-30 06:43:04.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:43:04.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 06:43:04.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 06:43:04.000000 pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-30 06:42:57.000000 pulumi_rke-3.5.0a1714458609/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:43:04.306851 pulumi_rke-3.5.0a1714458609/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:34:45.263140 pulumi_rke-3.5.0a1714544849/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-01 06:34:45.263140 pulumi_rke-3.5.0a1714544849/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:34:45.259139 pulumi_rke-3.5.0a1714544849/pulumi_rke/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   338457 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138960 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:34:45.259139 pulumi_rke-3.5.0a1714544849/pulumi_rke/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304657 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:34:45.263140 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-01 06:34:45.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 06:34:45.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:34:45.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 06:34:45.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 06:34:45.000000 pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 06:34:37.000000 pulumi_rke-3.5.0a1714544849/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:34:45.263140 pulumi_rke-3.5.0a1714544849/setup.cfg
```

### Comparing `pulumi_rke-3.5.0a1714458609/PKG-INFO` & `pulumi_rke-3.5.0a1714544849/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.5.0a1714458609
+Version: 3.5.0a1714544849
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.5.0a1714458609/README.md` & `pulumi_rke-3.5.0a1714544849/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/__init__.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/_inputs.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/_utilities.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/cluster.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/config/vars.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/outputs.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke/provider.py` & `pulumi_rke-3.5.0a1714544849/pulumi_rke/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1714458609/pulumi_rke.egg-info/PKG-INFO` & `pulumi_rke-3.5.0a1714544849/pulumi_rke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.5.0a1714458609
+Version: 3.5.0a1714544849
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.5.0a1714458609/pyproject.toml` & `pulumi_rke-3.5.0a1714544849/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rke"
   description = "A Pulumi package for creating and managing rke cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rke"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.5.0a1714458609"
+  version = "3.5.0a1714544849"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rke"
 
 [build-system]
```
