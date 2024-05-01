# Comparing `tmp/atomicds-0.0.6.tar.gz` & `tmp/atomicds-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomicds-0.0.6.tar", last modified: Wed Apr 10 15:09:45 2024, max compression
+gzip compressed data, was "atomicds-0.0.7.tar", last modified: Wed May  1 21:32:49 2024, max compression
```

## Comparing `atomicds-0.0.6.tar` & `atomicds-0.0.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.539180 atomicds-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.543180 atomicds-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-10 15:09:40.000000 atomicds-0.0.6/.github/workflows/upgrade_dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-10 15:09:40.000000 atomicds-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-10 15:09:40.000000 atomicds-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 15:09:40.000000 atomicds-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 15:09:40.000000 atomicds-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 15:09:40.000000 atomicds-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 15:09:45.551180 atomicds-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:09:40.000000 atomicds-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 15:09:40.000000 atomicds-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 15:09:40.000000 atomicds-0.0.6/requirements/requirements-windows-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:09:45.551180 atomicds-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.539180 atomicds-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/src/atomicds/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.547180 atomicds-0.0.6/src/atomicds/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/src/atomicds/results/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/rheed_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/rheed_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-10 15:09:40.000000 atomicds-0.0.6/src/atomicds/results/xps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/src/atomicds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 15:09:45.000000 atomicds-0.0.6/src/atomicds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:45.551180 atomicds-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-10 15:09:40.000000 atomicds-0.0.6/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.239203 atomicds-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.223203 atomicds-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.227203 atomicds-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-01 21:32:43.000000 atomicds-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-01 21:32:43.000000 atomicds-0.0.7/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-01 21:32:43.000000 atomicds-0.0.7/.github/workflows/upgrade_dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-01 21:32:43.000000 atomicds-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-01 21:32:43.000000 atomicds-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-01 21:32:43.000000 atomicds-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:32:43.000000 atomicds-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 21:32:43.000000 atomicds-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-01 21:32:49.235203 atomicds-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:32:43.000000 atomicds-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-01 21:32:43.000000 atomicds-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.231203 atomicds-0.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-01 21:32:43.000000 atomicds-0.0.7/requirements/requirements-windows-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:32:49.239203 atomicds-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.227203 atomicds-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.231203 atomicds-0.0.7/src/atomicds/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.235203 atomicds-0.0.7/src/atomicds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.235203 atomicds-0.0.7/src/atomicds/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25652 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/results/rheed_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/results/rheed_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-01 21:32:43.000000 atomicds-0.0.7/src/atomicds/results/xps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.235203 atomicds-0.0.7/src/atomicds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-01 21:32:49.000000 atomicds-0.0.7/src/atomicds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-01 21:32:49.000000 atomicds-0.0.7/src/atomicds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:32:49.000000 atomicds-0.0.7/src/atomicds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-01 21:32:49.000000 atomicds-0.0.7/src/atomicds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:32:49.000000 atomicds-0.0.7/src/atomicds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:49.235203 atomicds-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:32:43.000000 atomicds-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-01 21:32:43.000000 atomicds-0.0.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-01 21:32:43.000000 atomicds-0.0.7/tests/test_core.py
```

### Comparing `atomicds-0.0.6/.github/workflows/release.yml` & `atomicds-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/.github/workflows/testing.yml` & `atomicds-0.0.7/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/.github/workflows/upgrade_dependencies.yml` & `atomicds-0.0.7/.github/workflows/upgrade_dependencies.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/.gitignore` & `atomicds-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/.pre-commit-config.yaml` & `atomicds-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/LICENSE` & `atomicds-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/PKG-INFO` & `atomicds-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.6
+Version: 0.0.7
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.6/pyproject.toml` & `atomicds-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.10.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.10_extras.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.11.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.11_extras.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.9.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-macos-latest_py3.9_extras.txt` & `atomicds-0.0.7/requirements/requirements-macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.10_extras.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.11_extras.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-ubuntu-latest_py3.9_extras.txt` & `atomicds-0.0.7/requirements/requirements-ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.10.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.10_extras.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.11.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.11_extras.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.9.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/requirements/requirements-windows-latest_py3.9_extras.txt` & `atomicds-0.0.7/requirements/requirements-windows-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds/client.py` & `atomicds-0.0.7/src/atomicds/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds/core/client.py` & `atomicds-0.0.7/src/atomicds/core/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds/core/utils.py` & `atomicds-0.0.7/src/atomicds/core/utils.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds/results/rheed_image.py` & `atomicds-0.0.7/src/atomicds/results/rheed_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,21 +532,23 @@
 
         image_scales = [
             rheed_image.processed_image.size for rheed_image in self.rheed_images
         ]
         image_scale = np.amax(image_scales, axis=0)
 
         if node_df is None:
+            extra_iter = (
+                self.extra_data if self.extra_data else [None] * len(self.rheed_images)
+            )
             node_dfs = [
                 rheed_image.get_pattern_dataframe(
                     extra_data=extra_data, symmetrize=False, return_as_features=False
                 )
-                for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
+                for rheed_image, extra_data in zip(self.rheed_images, extra_iter)
             ]
-
             node_df = pd.concat(node_dfs, axis=0).reset_index(drop=True)
 
         labels, _ = pd.factorize(node_df["uuid"])
         node_df["pattern_id"] = labels
 
         linked_df = tp.link(
             f=node_df,
```

### Comparing `atomicds-0.0.6/src/atomicds/results/rheed_video.py` & `atomicds-0.0.7/src/atomicds/results/rheed_video.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds/results/xps.py` & `atomicds-0.0.7/src/atomicds/results/xps.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/src/atomicds.egg-info/PKG-INFO` & `atomicds-0.0.7/src/atomicds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.6
+Version: 0.0.7
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.6/src/atomicds.egg-info/SOURCES.txt` & `atomicds-0.0.7/src/atomicds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/tests/test_client.py` & `atomicds-0.0.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.6/tests/test_core.py` & `atomicds-0.0.7/tests/test_core.py`

 * *Files identical despite different names*

