# Comparing `tmp/terraform-backend-s3-bucket-1.0.3.tar.gz` & `tmp/terraform-backend-s3-bucket-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-backend-s3-bucket-1.0.3.tar", last modified: Mon Apr  1 07:26:22 2024, max compression
+gzip compressed data, was "terraform-backend-s3-bucket-1.0.4.tar", last modified: Wed May  1 06:29:12 2024, max compression
```

## Comparing `terraform-backend-s3-bucket-1.0.3.tar` & `terraform-backend-s3-bucket-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:26:12.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:26:22.628984 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 07:26:22.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 07:26:22.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:26:22.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 07:26:22.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 07:26:22.000000 terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/top_level.txt
```

### Comparing `terraform-backend-s3-bucket-1.0.3/LICENSE` & `terraform-backend-s3-bucket-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-1.0.3/PKG-INFO` & `terraform-backend-s3-bucket-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-1.0.3/setup.py` & `terraform-backend-s3-bucket-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "terraform-backend-s3-bucket",
-    "version": "1.0.3",
+    "version": "1.0.4",
     "description": "Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/terraform-backend-s3-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "terraform_backend_s3_bucket",
         "terraform_backend_s3_bucket._jsii"
     ],
     "package_data": {
         "terraform_backend_s3_bucket._jsii": [
-            "terraform-backend-s3-bucket@1.0.3.jsii.tgz"
+            "terraform-backend-s3-bucket@1.0.4.jsii.tgz"
         ],
         "terraform_backend_s3_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.117.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket/__init__.py` & `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/PKG-INFO` & `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-1.0.3/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt` & `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/terraform_backend_s3_bucket/py.typed
 src/terraform_backend_s3_bucket.egg-info/PKG-INFO
 src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
 src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
 src/terraform_backend_s3_bucket.egg-info/requires.txt
 src/terraform_backend_s3_bucket.egg-info/top_level.txt
 src/terraform_backend_s3_bucket/_jsii/__init__.py
-src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.3.jsii.tgz
+src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.4.jsii.tgz
```

