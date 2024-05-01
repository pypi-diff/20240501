# Comparing `tmp/pulumi_mailgun-3.6.0a1714456243.tar.gz` & `tmp/pulumi_mailgun-3.6.0a1714542487.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mailgun-3.6.0a1714456243.tar", last modified: Tue Apr 30 05:55:26 2024, max compression
+gzip compressed data, was "pulumi_mailgun-3.6.0a1714542487.tar", last modified: Wed May  1 05:55:55 2024, max compression
```

## Comparing `pulumi_mailgun-3.6.0a1714456243.tar` & `pulumi_mailgun-3.6.0a1714542487.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/domain_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-30 05:55:26.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 05:55:26.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:55:26.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 05:55:26.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 05:55:26.000000 pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 05:55:20.000000 pulumi_mailgun-3.6.0a1714456243/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:55:26.717398 pulumi_mailgun-3.6.0a1714456243/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/setup.cfg
```

### Comparing `pulumi_mailgun-3.6.0a1714456243/PKG-INFO` & `pulumi_mailgun-3.6.0a1714542487/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1714456243
+Version: 3.6.0a1714542487
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1714456243/README.md` & `pulumi_mailgun-3.6.0a1714542487/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/__init__.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/_inputs.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/_utilities.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/config/vars.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/domain.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/domain_credential.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/get_domain.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/outputs.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/provider.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/route.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun/webhook.py` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/PKG-INFO` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1714456243
+Version: 3.6.0a1714542487
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1714456243/pulumi_mailgun.egg-info/SOURCES.txt` & `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714456243/pyproject.toml` & `pulumi_mailgun-3.6.0a1714542487/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mailgun"
   description = "A Pulumi package for creating and managing Mailgun resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mailgun"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.6.0a1714456243"
+  version = "3.6.0a1714542487"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mailgun"
 
 [build-system]
```
