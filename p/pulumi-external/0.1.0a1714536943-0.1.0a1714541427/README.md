# Comparing `tmp/pulumi_external-0.1.0a1714536943.tar.gz` & `tmp/pulumi_external-0.1.0a1714541427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_external-0.1.0a1714536943.tar", last modified: Wed May  1 04:18:32 2024, max compression
+gzip compressed data, was "pulumi_external-0.1.0a1714541427.tar", last modified: Wed May  1 05:35:28 2024, max compression
```

## Comparing `pulumi_external-0.1.0a1714536943.tar` & `pulumi_external-0.1.0a1714541427.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:18:32.679618 pulumi_external-0.1.0a1714536943/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-01 04:18:32.679618 pulumi_external-0.1.0a1714536943/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:18:32.675619 pulumi_external-0.1.0a1714536943/pulumi_external/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/get_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pulumi_external/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:18:32.679618 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-01 04:18:32.000000 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 04:18:32.000000 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:18:32.000000 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 04:18:32.000000 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 04:18:32.000000 pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 04:18:26.000000 pulumi_external-0.1.0a1714536943/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:18:32.679618 pulumi_external-0.1.0a1714536943/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:35:28.927644 pulumi_external-0.1.0a1714541427/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-01 05:35:28.927644 pulumi_external-0.1.0a1714541427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:35:28.923644 pulumi_external-0.1.0a1714541427/pulumi_external/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/get_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pulumi_external/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:35:28.927644 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-01 05:35:28.000000 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 05:35:28.000000 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:35:28.000000 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 05:35:28.000000 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 05:35:28.000000 pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 05:35:22.000000 pulumi_external-0.1.0a1714541427/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:35:28.927644 pulumi_external-0.1.0a1714541427/setup.cfg
```

### Comparing `pulumi_external-0.1.0a1714536943/PKG-INFO` & `pulumi_external-0.1.0a1714541427/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_external
-Version: 0.1.0a1714536943
+Version: 0.1.0a1714541427
 Summary: A Pulumi package for creating and managing External cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_external-0.1.0a1714536943/README.md` & `pulumi_external-0.1.0a1714541427/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1714536943/pulumi_external/__init__.py` & `pulumi_external-0.1.0a1714541427/pulumi_external/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1714536943/pulumi_external/_utilities.py` & `pulumi_external-0.1.0a1714541427/pulumi_external/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1714536943/pulumi_external/get_external.py` & `pulumi_external-0.1.0a1714541427/pulumi_external/get_external.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1714536943/pulumi_external/provider.py` & `pulumi_external-0.1.0a1714541427/pulumi_external/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_external-0.1.0a1714536943/pulumi_external.egg-info/PKG-INFO` & `pulumi_external-0.1.0a1714541427/pulumi_external.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_external
-Version: 0.1.0a1714536943
+Version: 0.1.0a1714541427
 Summary: A Pulumi package for creating and managing External cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-external
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_external-0.1.0a1714536943/pyproject.toml` & `pulumi_external-0.1.0a1714541427/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_external"
   description = "A Pulumi package for creating and managing External cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1714536943"
+  version = "0.1.0a1714541427"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-external"
 
 [build-system]
```

