# Comparing `tmp/chartreuse-4.3.4.tar.gz` & `tmp/chartreuse-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartreuse-4.3.4.tar", last modified: Thu Nov 23 12:32:49 2023, max compression
+gzip compressed data, was "chartreuse-4.3.5.tar", last modified: Wed May  1 12:56:07 2024, max compression
```

## Comparing `chartreuse-4.3.4.tar` & `chartreuse-4.3.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:32:49.103093 chartreuse-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2023-11-23 12:32:39.000000 chartreuse-4.3.4/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-23 12:32:39.000000 chartreuse-4.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-23 12:32:49.103093 chartreuse-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2023-11-23 12:32:39.000000 chartreuse-4.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-23 12:32:39.000000 chartreuse-4.3.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-23 12:32:39.000000 chartreuse-4.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-11-23 12:32:49.103093 chartreuse-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-11-23 12:32:39.000000 chartreuse-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:32:49.099093 chartreuse-4.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:32:49.103093 chartreuse-4.3.4/src/chartreuse/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-23 12:32:39.000000 chartreuse-4.3.4/src/chartreuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-11-23 12:32:39.000000 chartreuse-4.3.4/src/chartreuse/chartreuse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4101 2023-11-23 12:32:39.000000 chartreuse-4.3.4/src/chartreuse/chartreuse_upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:32:49.103093 chartreuse-4.3.4/src/chartreuse/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-23 12:32:39.000000 chartreuse-4.3.4/src/chartreuse/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6418 2023-11-23 12:32:39.000000 chartreuse-4.3.4/src/chartreuse/utils/alembic_migration_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:32:49.103093 chartreuse-4.3.4/src/chartreuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-23 12:32:49.000000 chartreuse-4.3.4/src/chartreuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 12:32:48.000000 chartreuse-4.3.4/src/chartreuse.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:07.004820 chartreuse-4.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-01 12:56:02.000000 chartreuse-4.3.5/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 12:56:02.000000 chartreuse-4.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 12:56:07.004820 chartreuse-4.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 12:56:02.000000 chartreuse-4.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:56:02.000000 chartreuse-4.3.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 12:56:02.000000 chartreuse-4.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-01 12:56:07.004820 chartreuse-4.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-01 12:56:02.000000 chartreuse-4.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:07.000820 chartreuse-4.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:07.000820 chartreuse-4.3.5/src/chartreuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 12:56:02.000000 chartreuse-4.3.5/src/chartreuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-01 12:56:02.000000 chartreuse-4.3.5/src/chartreuse/chartreuse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4101 2024-05-01 12:56:02.000000 chartreuse-4.3.5/src/chartreuse/chartreuse_upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:07.004820 chartreuse-4.3.5/src/chartreuse/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 12:56:02.000000 chartreuse-4.3.5/src/chartreuse/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6418 2024-05-01 12:56:02.000000 chartreuse-4.3.5/src/chartreuse/utils/alembic_migration_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:07.004820 chartreuse-4.3.5/src/chartreuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:56:06.000000 chartreuse-4.3.5/src/chartreuse.egg-info/zip-safe
```

### Comparing `chartreuse-4.3.4/LICENCE.md` & `chartreuse-4.3.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/PKG-INFO` & `chartreuse-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartreuse
-Version: 4.3.4
+Version: 4.3.5
 Summary: Helper for Alembic migrations within Kubernetes.
 Home-page: https://github.com/wiremind/chartreuse
 Author: wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Platform: posix
 Requires-Python: >=3.7.0
```

### Comparing `chartreuse-4.3.4/README.md` & `chartreuse-4.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 ## Usage
 
 ### Requirements
 
 - Python >= 3.7
 - Using Helm to deploy you application
-- This Python package requires the `expecteddeploymentscales.wiremind.io` Kubernetes `Custom Resource Definition` from `wiremind-kubernetes` repository:
+- This Python package requires the `expecteddeploymentscales.wiremind.io` Kubernetes `Custom Resource Definition`:
 
 ```bash
-kubectl apply -f https://raw.githubusercontent.com/wiremind/wiremind-kubernetes/main/CustomResourceDefinition-expecteddeploymentscales.yaml
+helm repo add wiremind https://wiremind.github.io/wiremind-helm-charts
+helm install wiremind-crds wiremind/wiremind-crds --version 0.1.0
 ```
 
 - Please make sure Chartreuse Python **Package version** and Chartreuse **Helm Chart version**, you use, share `major.minor` otherwise Chartreuse won't start.
 
 ## Configuration
 
 ### Using Helm
```

### Comparing `chartreuse-4.3.4/setup.cfg` & `chartreuse-4.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/setup.py` & `chartreuse-4.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/src/chartreuse/chartreuse.py` & `chartreuse-4.3.5/src/chartreuse/chartreuse.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/src/chartreuse/chartreuse_upgrade.py` & `chartreuse-4.3.5/src/chartreuse/chartreuse_upgrade.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/src/chartreuse/utils/alembic_migration_helper.py` & `chartreuse-4.3.5/src/chartreuse/utils/alembic_migration_helper.py`

 * *Files identical despite different names*

### Comparing `chartreuse-4.3.4/src/chartreuse.egg-info/PKG-INFO` & `chartreuse-4.3.5/src/chartreuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartreuse
-Version: 4.3.4
+Version: 4.3.5
 Summary: Helper for Alembic migrations within Kubernetes.
 Home-page: https://github.com/wiremind/chartreuse
 Author: wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Platform: posix
 Requires-Python: >=3.7.0
```

### Comparing `chartreuse-4.3.4/src/chartreuse.egg-info/SOURCES.txt` & `chartreuse-4.3.5/src/chartreuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

