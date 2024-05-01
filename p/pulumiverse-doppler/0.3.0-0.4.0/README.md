# Comparing `tmp/pulumiverse_doppler-0.3.0.tar.gz` & `tmp/pulumiverse_doppler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.3.0.tar", last modified: Wed May  1 08:15:34 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.4.0.tar", last modified: Wed May  1 18:57:22 2024, max compression
```

## Comparing `pulumiverse_doppler-0.3.0.tar` & `pulumiverse_doppler-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.515970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.898080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/setup.py
```

### Comparing `pulumiverse_doppler-0.3.0/PKG-INFO` & `pulumiverse_doppler-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.3.0/README.md` & `pulumiverse_doppler-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/__init__.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/branch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/get_secrets.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/group.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_parameter_store.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_secrets_manager.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_secrets_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,18 @@
             name="Production",
             assume_role_arn=doppler_secrets_manager.arn)
         backend_prod = doppler.secrets_sync.AwsSecretsManager("backend_prod",
             integration=prod.id,
             project="backend",
             config="prd",
             region="us-east-1",
-            path="/backend/")
+            path="/backend/",
+            tags={
+                "myTag": "enabled",
+            })
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] assume_role_arn: The ARN of the AWS role for Doppler to assume
         :param pulumi.Input[str] name: The name of the integration
         """
@@ -217,15 +220,18 @@
             name="Production",
             assume_role_arn=doppler_secrets_manager.arn)
         backend_prod = doppler.secrets_sync.AwsSecretsManager("backend_prod",
             integration=prod.id,
             project="backend",
             config="prd",
             region="us-east-1",
-            path="/backend/")
+            path="/backend/",
+            tags={
+                "myTag": "enabled",
+            })
         ```
 
         :param str resource_name: The name of the resource.
         :param AwsSecretsManagerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/group.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/service_account.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_parameter_store.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 @pulumi.input_type
 class AwsSecretsManagerArgs:
     def __init__(__self__, *,
                  config: pulumi.Input[str],
                  integration: pulumi.Input[str],
                  path: pulumi.Input[str],
                  project: pulumi.Input[str],
-                 region: pulumi.Input[str]):
+                 region: pulumi.Input[str],
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a AwsSecretsManager resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] path: The path to the secret in AWS
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] region: The AWS region
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: AWS tags to attach to the secrets
         """
         pulumi.set(__self__, "config", config)
         pulumi.set(__self__, "integration", integration)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "region", region)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def config(self) -> pulumi.Input[str]:
         """
         The name of the Doppler config
         """
@@ -89,41 +93,57 @@
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        AWS tags to attach to the secrets
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
 
 @pulumi.input_type
 class _AwsSecretsManagerState:
     def __init__(__self__, *,
                  config: Optional[pulumi.Input[str]] = None,
                  integration: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None):
+                 region: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering AwsSecretsManager resources.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] path: The path to the secret in AWS
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] region: The AWS region
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: AWS tags to attach to the secrets
         """
         if config is not None:
             pulumi.set(__self__, "config", config)
         if integration is not None:
             pulumi.set(__self__, "integration", integration)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def config(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the Doppler config
         """
@@ -177,25 +197,38 @@
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        AWS tags to attach to the secrets
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
 
 class AwsSecretsManager(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  integration: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manage an AWS Secrets Manager Doppler sync.
 
         ## Example Usage
 
         ```python
@@ -244,24 +277,28 @@
             name="Production",
             assume_role_arn=doppler_secrets_manager.arn)
         backend_prod = doppler.secrets_sync.AwsSecretsManager("backend_prod",
             integration=prod.id,
             project="backend",
             config="prd",
             region="us-east-1",
-            path="/backend/")
+            path="/backend/",
+            tags={
+                "myTag": "enabled",
+            })
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] path: The path to the secret in AWS
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] region: The AWS region
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: AWS tags to attach to the secrets
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AwsSecretsManagerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -316,15 +353,18 @@
             name="Production",
             assume_role_arn=doppler_secrets_manager.arn)
         backend_prod = doppler.secrets_sync.AwsSecretsManager("backend_prod",
             integration=prod.id,
             project="backend",
             config="prd",
             region="us-east-1",
-            path="/backend/")
+            path="/backend/",
+            tags={
+                "myTag": "enabled",
+            })
         ```
 
         :param str resource_name: The name of the resource.
         :param AwsSecretsManagerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -339,14 +379,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  integration: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -363,51 +404,55 @@
             __props__.__dict__["path"] = path
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
+            __props__.__dict__["tags"] = tags
         super(AwsSecretsManager, __self__).__init__(
             'doppler:secretsSync/awsSecretsManager:AwsSecretsManager',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             config: Optional[pulumi.Input[str]] = None,
             integration: Optional[pulumi.Input[str]] = None,
             path: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
-            region: Optional[pulumi.Input[str]] = None) -> 'AwsSecretsManager':
+            region: Optional[pulumi.Input[str]] = None,
+            tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None) -> 'AwsSecretsManager':
         """
         Get an existing AwsSecretsManager resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] path: The path to the secret in AWS
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] region: The AWS region
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: AWS tags to attach to the secrets
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AwsSecretsManagerState.__new__(_AwsSecretsManagerState)
 
         __props__.__dict__["config"] = config
         __props__.__dict__["integration"] = integration
         __props__.__dict__["path"] = path
         __props__.__dict__["project"] = project
         __props__.__dict__["region"] = region
+        __props__.__dict__["tags"] = tags
         return AwsSecretsManager(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def config(self) -> pulumi.Output[str]:
         """
         The name of the Doppler config
@@ -442,7 +487,15 @@
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The AWS region
         """
         return pulumi.get(self, "region")
 
+    @property
+    @pulumi.getter
+    def tags(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
+        """
+        AWS tags to attach to the secrets
+        """
+        return pulumi.get(self, "tags")
+
```

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_account.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.3.0/setup.py` & `pulumiverse_doppler-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

