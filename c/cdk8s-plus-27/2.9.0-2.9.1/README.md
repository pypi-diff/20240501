# Comparing `tmp/cdk8s-plus-27-2.9.0.tar.gz` & `tmp/cdk8s-plus-27-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-27-2.9.0.tar", last modified: Thu Apr 18 17:03:51 2024, max compression
+gzip compressed data, was "cdk8s-plus-27-2.9.1.tar", last modified: Wed May  1 12:08:53 2024, max compression
```

## Comparing `cdk8s-plus-27-2.9.0.tar` & `cdk8s-plus-27-2.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.733981 cdk8s-plus-27-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 17:03:51.733981 cdk8s-plus-27-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:03:51.733981 cdk8s-plus-27-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.725981 cdk8s-plus-27-2.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.725981 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/
--rw-r--r--   0 runner    (1001) docker     (127)  1174767 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.725981 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1324832 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.9.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.729981 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)  2838922 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:03:41.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:03:51.725981 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 17:03:51.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-18 17:03:51.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:03:51.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 17:03:51.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 17:03:51.000000 cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.598265 cdk8s-plus-27-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 12:08:53.598265 cdk8s-plus-27-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:08:53.598265 cdk8s-plus-27-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.586264 cdk8s-plus-27-2.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.590264 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/
+-rw-r--r--   0 runner    (1001) docker     (127)  1174767 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.590264 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1320956 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/_jsii/cdk8s-plus-27@2.9.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.594264 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)  2838922 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:08:40.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:53.590264 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 12:08:53.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 12:08:53.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:08:53.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 12:08:53.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:08:53.000000 cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-27-2.9.0/LICENSE` & `cdk8s-plus-27-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.0/PKG-INFO` & `cdk8s-plus-27-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.9.0
+Version: 2.9.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-27-2.9.0/README.md` & `cdk8s-plus-27-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.0/setup.py` & `cdk8s-plus-27-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-27",
-    "version": "2.9.0",
+    "version": "2.9.1",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,25 +23,25 @@
     "packages": [
         "cdk8s_plus_27",
         "cdk8s_plus_27._jsii",
         "cdk8s_plus_27.k8s"
     ],
     "package_data": {
         "cdk8s_plus_27._jsii": [
-            "cdk8s-plus-27@2.9.0.jsii.tgz"
+            "cdk8s-plus-27@2.9.1.jsii.tgz"
         ],
         "cdk8s_plus_27": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "cdk8s>=2.68.11, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/__init__.py` & `cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.0/src/cdk8s_plus_27/k8s/__init__.py` & `cdk8s-plus-27-2.9.1/src/cdk8s_plus_27/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-27-2.9.0/src/cdk8s_plus_27.egg-info/PKG-INFO` & `cdk8s-plus-27-2.9.1/src/cdk8s_plus_27.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-27
-Version: 2.9.0
+Version: 2.9.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-27 synthesizes Kubernetes manifests for Kubernetes 1.27.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

