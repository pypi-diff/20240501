# Comparing `tmp/mrgrain.cdk-esbuild-5.0.9.tar.gz` & `tmp/mrgrain.cdk-esbuild-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-5.0.9.tar", last modified: Mon Jan  1 05:06:42 2024, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-5.1.0.tar", last modified: Wed May  1 05:05:37 2024, max compression
```

## Comparing `mrgrain.cdk-esbuild-5.0.9.tar` & `mrgrain.cdk-esbuild-5.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19422 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (127)   354597 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.645526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80145 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.0.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 05:06:31.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 05:06:42.641526 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19422 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-01 05:06:42.000000 mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.447649 mrgrain.cdk-esbuild-5.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.447649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (127)   354404 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80581 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@5.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:05:26.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:05:37.451649 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 05:05:37.000000 mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-5.0.9/LICENSE` & `mrgrain.cdk-esbuild-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-5.0.9/PKG-INFO` & `mrgrain.cdk-esbuild-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.0.9
+Version: 5.1.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -103,18 +103,14 @@
 
 ### Amazon CloudWatch Synthetics: Canary monitoring
 
 > 💡 See [Monitored Website (TypeScript)](examples/typescript/website) for a working example of a deployed and monitored website.
 
 Synthetics runs a canary to produce traffic to an application for monitoring purposes. Use `TypeScriptCode` as the `code` of a Canary test:
 
-> ℹ️ This feature depends on `@aws-cdk/aws-synthetics-alpha` which is in developer preview.
-> Please install the package using the respective tool of your language.
-> You may need to update your source code when upgrading to a newer version of this alpha package.
-
 ```python
 bundled_code = TypeScriptCode("src/canary.ts",
     build_options=BuildOptions(
         outdir="nodejs/node_modules"
     )
 )
```

### Comparing `mrgrain.cdk-esbuild-5.0.9/README.md` & `mrgrain.cdk-esbuild-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,14 @@
 
 ### Amazon CloudWatch Synthetics: Canary monitoring
 
 > 💡 See [Monitored Website (TypeScript)](examples/typescript/website) for a working example of a deployed and monitored website.
 
 Synthetics runs a canary to produce traffic to an application for monitoring purposes. Use `TypeScriptCode` as the `code` of a Canary test:
 
-> ℹ️ This feature depends on `@aws-cdk/aws-synthetics-alpha` which is in developer preview.
-> Please install the package using the respective tool of your language.
-> You may need to update your source code when upgrading to a newer version of this alpha package.
-
 ```python
 bundled_code = TypeScriptCode("src/canary.ts",
     build_options=BuildOptions(
         outdir="nodejs/node_modules"
     )
 )
```

### Comparing `mrgrain.cdk-esbuild-5.0.9/setup.py` & `mrgrain.cdk-esbuild-5.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "5.0.9",
+    "version": "5.1.0",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@5.0.9.jsii.tgz"
+            "cdk-esbuild@5.1.0.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.51.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.93.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `mrgrain.cdk-esbuild-5.0.9/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-5.1.0/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,18 +81,14 @@
 
 ### Amazon CloudWatch Synthetics: Canary monitoring
 
 > 💡 See [Monitored Website (TypeScript)](examples/typescript/website) for a working example of a deployed and monitored website.
 
 Synthetics runs a canary to produce traffic to an application for monitoring purposes. Use `TypeScriptCode` as the `code` of a Canary test:
 
-> ℹ️ This feature depends on `@aws-cdk/aws-synthetics-alpha` which is in developer preview.
-> Please install the package using the respective tool of your language.
-> You may need to update your source code when upgrading to a newer version of this alpha package.
-
 ```python
 bundled_code = TypeScriptCode("src/canary.ts",
     build_options=BuildOptions(
         outdir="nodejs/node_modules"
     )
 )
 
@@ -403,14 +399,17 @@
 Yes, `v2` of `cdk-esbuild` is compatible with AWS CDK v1.
 You can find the [documentation for it on the v2 branch](https://github.com/mrgrain/cdk-esbuild/tree/v2).
 
 Support for AWS CDK v1 and `cdk-esbuild` v2 has ended on June 1, 2023.
 Both packages are not receiving any updates or bug fixes, including for security related issues.
 You are strongly advised to upgrade to a supported version of these packages.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `mrgrain.cdk-esbuild-5.0.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-5.1.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 5.0.9
+Version: 5.1.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -103,18 +103,14 @@
 
 ### Amazon CloudWatch Synthetics: Canary monitoring
 
 > 💡 See [Monitored Website (TypeScript)](examples/typescript/website) for a working example of a deployed and monitored website.
 
 Synthetics runs a canary to produce traffic to an application for monitoring purposes. Use `TypeScriptCode` as the `code` of a Canary test:
 
-> ℹ️ This feature depends on `@aws-cdk/aws-synthetics-alpha` which is in developer preview.
-> Please install the package using the respective tool of your language.
-> You may need to update your source code when upgrading to a newer version of this alpha package.
-
 ```python
 bundled_code = TypeScriptCode("src/canary.ts",
     build_options=BuildOptions(
         outdir="nodejs/node_modules"
     )
 )
```

