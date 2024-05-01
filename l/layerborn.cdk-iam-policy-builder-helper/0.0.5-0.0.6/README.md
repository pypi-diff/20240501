# Comparing `tmp/layerborn.cdk-iam-policy-builder-helper-0.0.5.tar.gz` & `tmp/layerborn.cdk-iam-policy-builder-helper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerborn.cdk-iam-policy-builder-helper-0.0.5.tar", last modified: Tue Feb  6 16:21:54 2024, max compression
+gzip compressed data, was "layerborn.cdk-iam-policy-builder-helper-0.0.6.tar", last modified: Wed May  1 00:17:04 2024, max compression
```

## Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5.tar` & `layerborn.cdk-iam-policy-builder-helper-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.892511 layerborn.cdk-iam-policy-builder-helper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-06 16:21:54.892511 layerborn.cdk-iam-policy-builder-helper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 16:21:54.892511 layerborn.cdk-iam-policy-builder-helper-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.884512 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.884512 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.884512 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn/cdk_iam_policy_builder_helper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.888512 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn/cdk_iam_policy_builder_helper/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn/cdk_iam_policy_builder_helper/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2212036 2024-02-06 16:21:43.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn/cdk_iam_policy_builder_helper/_jsii/cdk-iam-policy-builder-helper@0.0.5.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:21:54.888512 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-06 16:21:54.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-06 16:21:54.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 16:21:54.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-06 16:21:54.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-06 16:21:54.000000 layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.884425 layerborn.cdk-iam-policy-builder-helper-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-01 00:17:04.884425 layerborn.cdk-iam-policy-builder-helper-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:17:04.884425 layerborn.cdk-iam-policy-builder-helper-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.880425 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.880425 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.880425 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn/cdk_iam_policy_builder_helper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.880425 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn/cdk_iam_policy_builder_helper/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn/cdk_iam_policy_builder_helper/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2212049 2024-05-01 00:16:49.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn/cdk_iam_policy_builder_helper/_jsii/cdk-iam-policy-builder-helper@0.0.6.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:17:04.880425 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-01 00:17:04.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 00:17:04.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:17:04.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 00:17:04.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 00:17:04.000000 layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/top_level.txt
```

### Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5/LICENSE` & `layerborn.cdk-iam-policy-builder-helper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5/PKG-INFO` & `layerborn.cdk-iam-policy-builder-helper-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-iam-policy-builder-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CDK construct that helps build IAM policies using the AWS IAM Policy Builder dump. Normally it is better to use cdk-iam-floyd, However, I found that cdk-iam-floyd currently is not jsii compliant so I wasn't able to use it in my jsii compliant projects in languages that are not typescript or python.
 Home-page: https://github.com/layerborn/cdk-iam-policy-builder-helper-construct.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-iam-policy-builder-helper-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5/setup.py` & `layerborn.cdk-iam-policy-builder-helper-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "layerborn.cdk-iam-policy-builder-helper",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "A CDK construct that helps build IAM policies using the AWS IAM Policy Builder dump. Normally it is better to use cdk-iam-floyd, However, I found that cdk-iam-floyd currently is not jsii compliant so I wasn't able to use it in my jsii compliant projects in languages that are not typescript or python.",
     "license": "Apache-2.0",
     "url": "https://github.com/layerborn/cdk-iam-policy-builder-helper-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "Jayson Rawlins<jayson.rawlins@layerborn.io>",
     "bdist_wheel": {
         "universal": true
@@ -21,15 +21,15 @@
         "": "src"
     },
     "packages": [
         "layerborn.cdk_iam_policy_builder_helper._jsii"
     ],
     "package_data": {
         "layerborn.cdk_iam_policy_builder_helper._jsii": [
-            "cdk-iam-policy-builder-helper@0.0.5.jsii.tgz"
+            "cdk-iam-policy-builder-helper@0.0.6.jsii.tgz"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
         "jsii>=1.94.0, <2.0.0",
```

### Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/PKG-INFO` & `layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerborn.cdk-iam-policy-builder-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CDK construct that helps build IAM policies using the AWS IAM Policy Builder dump. Normally it is better to use cdk-iam-floyd, However, I found that cdk-iam-floyd currently is not jsii compliant so I wasn't able to use it in my jsii compliant projects in languages that are not typescript or python.
 Home-page: https://github.com/layerborn/cdk-iam-policy-builder-helper-construct.git
 Author: Jayson Rawlins<jayson.rawlins@layerborn.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/layerborn/cdk-iam-policy-builder-helper-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `layerborn.cdk-iam-policy-builder-helper-0.0.5/src/layerborn.cdk_iam_policy_builder_helper.egg-info/SOURCES.txt` & `layerborn.cdk-iam-policy-builder-helper-0.0.6/src/layerborn.cdk_iam_policy_builder_helper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 setup.py
 src/layerborn.cdk_iam_policy_builder_helper.egg-info/PKG-INFO
 src/layerborn.cdk_iam_policy_builder_helper.egg-info/SOURCES.txt
 src/layerborn.cdk_iam_policy_builder_helper.egg-info/dependency_links.txt
 src/layerborn.cdk_iam_policy_builder_helper.egg-info/requires.txt
 src/layerborn.cdk_iam_policy_builder_helper.egg-info/top_level.txt
 src/layerborn/cdk_iam_policy_builder_helper/_jsii/__init__.py
-src/layerborn/cdk_iam_policy_builder_helper/_jsii/cdk-iam-policy-builder-helper@0.0.5.jsii.tgz
+src/layerborn/cdk_iam_policy_builder_helper/_jsii/cdk-iam-policy-builder-helper@0.0.6.jsii.tgz
```

