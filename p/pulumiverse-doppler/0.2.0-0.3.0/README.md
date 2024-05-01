# Comparing `tmp/pulumiverse_doppler-0.2.0.tar.gz` & `tmp/pulumiverse_doppler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.2.0.tar", last modified: Tue Apr 30 20:29:12 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.3.0.tar", last modified: Wed May  1 08:15:34 2024, max compression
```

## Comparing `pulumiverse_doppler-0.2.0.tar` & `pulumiverse_doppler-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.676499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/get_secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.515970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/projectmember/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:15:34.519970 pulumiverse_doppler-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 08:15:34.000000 pulumiverse_doppler-0.3.0/setup.py
```

### Comparing `pulumiverse_doppler-0.2.0/PKG-INFO` & `pulumiverse_doppler-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.2.0/README.md` & `pulumiverse_doppler-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/branch_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
 
         backend_ci_github = doppler.BranchConfig("backend_ci_github",
             project="backend",
             environment="ci",
             name="ci_github")
         ```
 
+        ## Resource ID Format
+
+        Resource IDs are in the format `<project-name>.<environment-slug>.<config-name>`.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
         :param pulumi.Input[str] name: The name of the Doppler config
         :param pulumi.Input[str] project: The name of the Doppler project where the config is located
         """
         ...
@@ -168,14 +172,18 @@
 
         backend_ci_github = doppler.BranchConfig("backend_ci_github",
             project="backend",
             environment="ci",
             name="ci_github")
         ```
 
+        ## Resource ID Format
+
+        Resource IDs are in the format `<project-name>.<environment-slug>.<config-name>`.
+
         :param str resource_name: The name of the resource.
         :param BranchConfigArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(BranchConfigArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,18 @@
 
         backend_ci = doppler.Environment("backend_ci",
             project="backend",
             slug="ci",
             name="Continuous Integration")
         ```
 
+        ## Resource ID Format
+
+        Resource IDs are in the format `<project-name>.<environment-slug>`.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the Doppler environment
         :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
         :param pulumi.Input[str] slug: The slug of the Doppler environment
         """
         ...
@@ -167,14 +171,18 @@
 
         backend_ci = doppler.Environment("backend_ci",
             project="backend",
             slug="ci",
             name="Continuous Integration")
         ```
 
+        ## Resource ID Format
+
+        Resource IDs are in the format `<project-name>.<environment-slug>`.
+
         :param str resource_name: The name of the resource.
         :param EnvironmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(EnvironmentArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/get_secrets.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_parameter_store.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_secrets_manager.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/integration/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_parameter_store.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.3.0/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 README.md
 setup.py
 pulumiverse_doppler/__init__.py
 pulumiverse_doppler/_utilities.py
 pulumiverse_doppler/branch_config.py
 pulumiverse_doppler/environment.py
 pulumiverse_doppler/get_secrets.py
+pulumiverse_doppler/group.py
 pulumiverse_doppler/project.py
 pulumiverse_doppler/provider.py
 pulumiverse_doppler/pulumi-plugin.json
 pulumiverse_doppler/py.typed
 pulumiverse_doppler/secret.py
+pulumiverse_doppler/service_account.py
 pulumiverse_doppler/service_token.py
 pulumiverse_doppler.egg-info/PKG-INFO
 pulumiverse_doppler.egg-info/SOURCES.txt
 pulumiverse_doppler.egg-info/dependency_links.txt
 pulumiverse_doppler.egg-info/not-zip-safe
 pulumiverse_doppler.egg-info/requires.txt
 pulumiverse_doppler.egg-info/top_level.txt
 pulumiverse_doppler/config/__init__.py
 pulumiverse_doppler/config/vars.py
 pulumiverse_doppler/integration/__init__.py
 pulumiverse_doppler/integration/aws_parameter_store.py
 pulumiverse_doppler/integration/aws_secrets_manager.py
+pulumiverse_doppler/projectmember/__init__.py
+pulumiverse_doppler/projectmember/group.py
+pulumiverse_doppler/projectmember/service_account.py
 pulumiverse_doppler/secretssync/__init__.py
 pulumiverse_doppler/secretssync/aws_parameter_store.py
 pulumiverse_doppler/secretssync/aws_secrets_manager.py
```

### Comparing `pulumiverse_doppler-0.2.0/setup.py` & `pulumiverse_doppler-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

