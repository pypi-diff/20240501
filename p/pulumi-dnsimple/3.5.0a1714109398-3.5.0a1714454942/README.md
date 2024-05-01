# Comparing `tmp/pulumi_dnsimple-3.5.0a1714109398.tar.gz` & `tmp/pulumi_dnsimple-3.5.0a1714454942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dnsimple-3.5.0a1714109398.tar", last modified: Fri Apr 26 05:32:59 2024, max compression
+gzip compressed data, was "pulumi_dnsimple-3.5.0a1714454942.tar", last modified: Tue Apr 30 05:31:57 2024, max compression
```

## Comparing `pulumi_dnsimple-3.5.0a1714109398.tar` & `pulumi_dnsimple-3.5.0a1714454942.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:32:59.228958 pulumi_dnsimple-3.5.0a1714109398/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-26 05:32:59.228958 pulumi_dnsimple-3.5.0a1714109398/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:32:59.224958 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:32:59.228958 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/email_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/lets_encrypt_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/zone_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:32:59.228958 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-26 05:32:59.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 05:32:59.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:32:59.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 05:32:59.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 05:32:59.000000 pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 05:32:53.000000 pulumi_dnsimple-3.5.0a1714109398/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:32:59.228958 pulumi_dnsimple-3.5.0a1714109398/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/email_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/lets_encrypt_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/zone_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-30 05:31:57.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 05:31:57.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:31:57.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 05:31:57.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 05:31:57.000000 pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 05:31:50.000000 pulumi_dnsimple-3.5.0a1714454942/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 05:31:57.155815 pulumi_dnsimple-3.5.0a1714454942/setup.cfg
```

### Comparing `pulumi_dnsimple-3.5.0a1714109398/PKG-INFO` & `pulumi_dnsimple-3.5.0a1714454942/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1714109398
+Version: 3.5.0a1714454942
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi,dnsimple
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1714109398/README.md` & `pulumi_dnsimple-3.5.0a1714454942/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/__init__.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/_utilities.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/__init__.pyi` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/config/vars.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/domain.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/email_forward.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/email_forward.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/get_certificate.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/get_zone.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/lets_encrypt_certificate.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/lets_encrypt_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/provider.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/record.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple/zone_record.py` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple/zone_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/PKG-INFO` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1714109398
+Version: 3.5.0a1714454942
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi,dnsimple
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pulumi_dnsimple.egg-info/SOURCES.txt` & `pulumi_dnsimple-3.5.0a1714454942/pulumi_dnsimple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1714109398/pyproject.toml` & `pulumi_dnsimple-3.5.0a1714454942/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_dnsimple"
   description = "A Pulumi package for creating and managing dnsimple cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "dnsimple"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.5.0a1714109398"
+  version = "3.5.0a1714454942"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-dnsimple"
 
 [build-system]
```
