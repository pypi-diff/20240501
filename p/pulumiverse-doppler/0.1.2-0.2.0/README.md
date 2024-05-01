# Comparing `tmp/pulumiverse_doppler-0.1.2.tar.gz` & `tmp/pulumiverse_doppler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.1.2.tar", last modified: Tue Apr 30 09:20:21 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.2.0.tar", last modified: Tue Apr 30 20:29:12 2024, max compression
```

## Comparing `pulumiverse_doppler-0.1.2.tar` & `pulumiverse_doppler-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.258834 pulumiverse_doppler-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/donfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:20:21.254835 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 09:20:21.000000 pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:20:21.258834 pulumiverse_doppler-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 09:20:20.000000 pulumiverse_doppler-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.676499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/get_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:29:12.680499 pulumiverse_doppler-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 20:29:12.000000 pulumiverse_doppler-0.2.0/setup.py
```

### Comparing `pulumiverse_doppler-0.1.2/PKG-INFO` & `pulumiverse_doppler-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.1.2/README.md` & `pulumiverse_doppler-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/branch_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 
 __all__ = ['BranchConfigArgs', 'BranchConfig']
 
 @pulumi.input_type
 class BranchConfigArgs:
     def __init__(__self__, *,
                  environment: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 project: pulumi.Input[str]):
+                 project: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a BranchConfig resource.
         :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
         :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        :param pulumi.Input[str] name: The name of the Doppler config
         """
         pulumi.set(__self__, "environment", environment)
-        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def environment(self) -> pulumi.Input[str]:
         """
         The name of the Doppler environment where the config is located
         """
@@ -37,36 +38,36 @@
 
     @environment.setter
     def environment(self, value: pulumi.Input[str]):
         pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The name of the Doppler config
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def project(self) -> pulumi.Input[str]:
         """
         The name of the Doppler project where the config is located
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the Doppler config
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
 
 @pulumi.input_type
 class _BranchConfigState:
     def __init__(__self__, *,
                  environment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None):
@@ -134,18 +135,18 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.BranchConfig("backendCiGithub",
+        backend_ci_github = doppler.BranchConfig("backend_ci_github",
+            project="backend",
             environment="ci",
-            name="ci_github",
-            project="backend")
+            name="ci_github")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
         :param pulumi.Input[str] name: The name of the Doppler config
         :param pulumi.Input[str] project: The name of the Doppler project where the config is located
@@ -161,18 +162,18 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.BranchConfig("backendCiGithub",
+        backend_ci_github = doppler.BranchConfig("backend_ci_github",
+            project="backend",
             environment="ci",
-            name="ci_github",
-            project="backend")
+            name="ci_github")
         ```
 
         :param str resource_name: The name of the resource.
         :param BranchConfigArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -197,16 +198,14 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BranchConfigArgs.__new__(BranchConfigArgs)
 
             if environment is None and not opts.urn:
                 raise TypeError("Missing required property 'environment'")
             __props__.__dict__["environment"] = environment
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
         alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="doppler:index/config:Config")])
         opts = pulumi.ResourceOptions.merge(opts, alias_opts)
         super(BranchConfig, __self__).__init__(
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/config.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/environment.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,262 +5,262 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ConfigArgs', 'Config']
+__all__ = ['EnvironmentArgs', 'Environment']
 
 @pulumi.input_type
-class ConfigArgs:
+class EnvironmentArgs:
     def __init__(__self__, *,
-                 environment: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 project: pulumi.Input[str]):
+                 project: pulumi.Input[str],
+                 slug: pulumi.Input[str]):
         """
-        The set of arguments for constructing a Config resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        The set of arguments for constructing a Environment resource.
+        :param pulumi.Input[str] name: The name of the Doppler environment
+        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
+        :param pulumi.Input[str] slug: The slug of the Doppler environment
         """
-        pulumi.set(__self__, "environment", environment)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
-
-    @property
-    @pulumi.getter
-    def environment(self) -> pulumi.Input[str]:
-        """
-        The name of the Doppler environment where the config is located
-        """
-        return pulumi.get(self, "environment")
-
-    @environment.setter
-    def environment(self, value: pulumi.Input[str]):
-        pulumi.set(self, "environment", value)
+        pulumi.set(__self__, "slug", slug)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler config
+        The name of the Doppler environment
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler project where the config is located
+        The name of the Doppler project where the environment is located
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
+    @property
+    @pulumi.getter
+    def slug(self) -> pulumi.Input[str]:
+        """
+        The slug of the Doppler environment
+        """
+        return pulumi.get(self, "slug")
+
+    @slug.setter
+    def slug(self, value: pulumi.Input[str]):
+        pulumi.set(self, "slug", value)
+
 
 @pulumi.input_type
-class _ConfigState:
+class _EnvironmentState:
     def __init__(__self__, *,
-                 environment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None):
+                 project: Optional[pulumi.Input[str]] = None,
+                 slug: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Config resources.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        Input properties used for looking up and filtering Environment resources.
+        :param pulumi.Input[str] name: The name of the Doppler environment
+        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
+        :param pulumi.Input[str] slug: The slug of the Doppler environment
         """
-        if environment is not None:
-            pulumi.set(__self__, "environment", environment)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
-
-    @property
-    @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the Doppler environment where the config is located
-        """
-        return pulumi.get(self, "environment")
-
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "environment", value)
+        if slug is not None:
+            pulumi.set(__self__, "slug", slug)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler config
+        The name of the Doppler environment
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler project where the config is located
+        The name of the Doppler project where the environment is located
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project", value)
 
+    @property
+    @pulumi.getter
+    def slug(self) -> Optional[pulumi.Input[str]]:
+        """
+        The slug of the Doppler environment
+        """
+        return pulumi.get(self, "slug")
+
+    @slug.setter
+    def slug(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "slug", value)
+
 
-class Config(pulumi.CustomResource):
+class Environment(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 environment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage a Doppler config.
+        Manage a Doppler environment.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.Config("backendCiGithub",
-            environment="ci",
-            name="ci_github",
-            project="backend")
+        backend_ci = doppler.Environment("backend_ci",
+            project="backend",
+            slug="ci",
+            name="Continuous Integration")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        :param pulumi.Input[str] name: The name of the Doppler environment
+        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
+        :param pulumi.Input[str] slug: The slug of the Doppler environment
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ConfigArgs,
+                 args: EnvironmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage a Doppler config.
+        Manage a Doppler environment.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.Config("backendCiGithub",
-            environment="ci",
-            name="ci_github",
-            project="backend")
+        backend_ci = doppler.Environment("backend_ci",
+            project="backend",
+            slug="ci",
+            name="Continuous Integration")
         ```
 
         :param str resource_name: The name of the resource.
-        :param ConfigArgs args: The arguments to use to populate this resource's properties.
+        :param EnvironmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ConfigArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EnvironmentArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 environment: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ConfigArgs.__new__(ConfigArgs)
+            __props__ = EnvironmentArgs.__new__(EnvironmentArgs)
 
-            if environment is None and not opts.urn:
-                raise TypeError("Missing required property 'environment'")
-            __props__.__dict__["environment"] = environment
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
-        super(Config, __self__).__init__(
-            'doppler:index/config:Config',
+            if slug is None and not opts.urn:
+                raise TypeError("Missing required property 'slug'")
+            __props__.__dict__["slug"] = slug
+        super(Environment, __self__).__init__(
+            'doppler:index/environment:Environment',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            environment: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            project: Optional[pulumi.Input[str]] = None) -> 'Config':
+            project: Optional[pulumi.Input[str]] = None,
+            slug: Optional[pulumi.Input[str]] = None) -> 'Environment':
         """
-        Get an existing Config resource's state with the given name, id, and optional extra
+        Get an existing Environment resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        :param pulumi.Input[str] name: The name of the Doppler environment
+        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
+        :param pulumi.Input[str] slug: The slug of the Doppler environment
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ConfigState.__new__(_ConfigState)
+        __props__ = _EnvironmentState.__new__(_EnvironmentState)
 
-        __props__.__dict__["environment"] = environment
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
-        return Config(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["slug"] = slug
+        return Environment(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[str]:
+    def name(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler environment where the config is located
+        The name of the Doppler environment
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def project(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler config
+        The name of the Doppler project where the environment is located
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    def slug(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler project where the config is located
+        The slug of the Doppler environment
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "slug")
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/donfig.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/service_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,262 +5,341 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['DonfigArgs', 'Donfig']
+__all__ = ['ServiceTokenArgs', 'ServiceToken']
 
 @pulumi.input_type
-class DonfigArgs:
+class ServiceTokenArgs:
     def __init__(__self__, *,
-                 environment: pulumi.Input[str],
+                 config: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 project: pulumi.Input[str]):
+                 project: pulumi.Input[str],
+                 access: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Donfig resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        The set of arguments for constructing a ServiceToken resource.
+        :param pulumi.Input[str] config: The name of the Doppler config where the service token is located
+        :param pulumi.Input[str] name: The name of the Doppler service token
+        :param pulumi.Input[str] project: The name of the Doppler project where the service token is located
+        :param pulumi.Input[str] access: The access level (read or read/write)
         """
-        pulumi.set(__self__, "environment", environment)
+        pulumi.set(__self__, "config", config)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
+        if access is not None:
+            pulumi.set(__self__, "access", access)
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Input[str]:
+    def config(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler environment where the config is located
+        The name of the Doppler config where the service token is located
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "config")
 
-    @environment.setter
-    def environment(self, value: pulumi.Input[str]):
-        pulumi.set(self, "environment", value)
+    @config.setter
+    def config(self, value: pulumi.Input[str]):
+        pulumi.set(self, "config", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler config
+        The name of the Doppler service token
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler project where the config is located
+        The name of the Doppler project where the service token is located
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
+    @property
+    @pulumi.getter
+    def access(self) -> Optional[pulumi.Input[str]]:
+        """
+        The access level (read or read/write)
+        """
+        return pulumi.get(self, "access")
+
+    @access.setter
+    def access(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access", value)
+
 
 @pulumi.input_type
-class _DonfigState:
+class _ServiceTokenState:
     def __init__(__self__, *,
-                 environment: Optional[pulumi.Input[str]] = None,
+                 access: Optional[pulumi.Input[str]] = None,
+                 config: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Donfig resources.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
-        """
-        if environment is not None:
-            pulumi.set(__self__, "environment", environment)
+        Input properties used for looking up and filtering ServiceToken resources.
+        :param pulumi.Input[str] access: The access level (read or read/write)
+        :param pulumi.Input[str] config: The name of the Doppler config where the service token is located
+        :param pulumi.Input[str] key: The key for the Doppler service token
+        :param pulumi.Input[str] name: The name of the Doppler service token
+        :param pulumi.Input[str] project: The name of the Doppler project where the service token is located
+        """
+        if access is not None:
+            pulumi.set(__self__, "access", access)
+        if config is not None:
+            pulumi.set(__self__, "config", config)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
 
     @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[str]]:
+    def access(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler environment where the config is located
+        The access level (read or read/write)
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "access")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "environment", value)
+    @access.setter
+    def access(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access", value)
+
+    @property
+    @pulumi.getter
+    def config(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the Doppler config where the service token is located
+        """
+        return pulumi.get(self, "config")
+
+    @config.setter
+    def config(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "config", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The key for the Doppler service token
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler config
+        The name of the Doppler service token
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler project where the config is located
+        The name of the Doppler project where the service token is located
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project", value)
 
 
-class Donfig(pulumi.CustomResource):
+class ServiceToken(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 environment: Optional[pulumi.Input[str]] = None,
+                 access: Optional[pulumi.Input[str]] = None,
+                 config: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage a Doppler config.
+        Manage a Doppler service token.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.Donfig("backendCiGithub",
-            environment="ci",
-            name="ci_github",
-            project="backend")
+        backend_ci_token = doppler.ServiceToken("backend_ci_token",
+            project="backend",
+            config="ci",
+            name="Builder Token",
+            access="read")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        :param pulumi.Input[str] access: The access level (read or read/write)
+        :param pulumi.Input[str] config: The name of the Doppler config where the service token is located
+        :param pulumi.Input[str] name: The name of the Doppler service token
+        :param pulumi.Input[str] project: The name of the Doppler project where the service token is located
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DonfigArgs,
+                 args: ServiceTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage a Doppler config.
+        Manage a Doppler service token.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci_github = doppler.Donfig("backendCiGithub",
-            environment="ci",
-            name="ci_github",
-            project="backend")
+        backend_ci_token = doppler.ServiceToken("backend_ci_token",
+            project="backend",
+            config="ci",
+            name="Builder Token",
+            access="read")
         ```
 
         :param str resource_name: The name of the resource.
-        :param DonfigArgs args: The arguments to use to populate this resource's properties.
+        :param ServiceTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DonfigArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ServiceTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 environment: Optional[pulumi.Input[str]] = None,
+                 access: Optional[pulumi.Input[str]] = None,
+                 config: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DonfigArgs.__new__(DonfigArgs)
+            __props__ = ServiceTokenArgs.__new__(ServiceTokenArgs)
 
-            if environment is None and not opts.urn:
-                raise TypeError("Missing required property 'environment'")
-            __props__.__dict__["environment"] = environment
+            __props__.__dict__["access"] = access
+            if config is None and not opts.urn:
+                raise TypeError("Missing required property 'config'")
+            __props__.__dict__["config"] = config
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
-        super(Donfig, __self__).__init__(
-            'doppler:index/donfig:Donfig',
+            __props__.__dict__["key"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["key"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(ServiceToken, __self__).__init__(
+            'doppler:index/serviceToken:ServiceToken',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            environment: Optional[pulumi.Input[str]] = None,
+            access: Optional[pulumi.Input[str]] = None,
+            config: Optional[pulumi.Input[str]] = None,
+            key: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            project: Optional[pulumi.Input[str]] = None) -> 'Donfig':
+            project: Optional[pulumi.Input[str]] = None) -> 'ServiceToken':
         """
-        Get an existing Donfig resource's state with the given name, id, and optional extra
+        Get an existing ServiceToken resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] environment: The name of the Doppler environment where the config is located
-        :param pulumi.Input[str] name: The name of the Doppler config
-        :param pulumi.Input[str] project: The name of the Doppler project where the config is located
+        :param pulumi.Input[str] access: The access level (read or read/write)
+        :param pulumi.Input[str] config: The name of the Doppler config where the service token is located
+        :param pulumi.Input[str] key: The key for the Doppler service token
+        :param pulumi.Input[str] name: The name of the Doppler service token
+        :param pulumi.Input[str] project: The name of the Doppler project where the service token is located
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DonfigState.__new__(_DonfigState)
+        __props__ = _ServiceTokenState.__new__(_ServiceTokenState)
 
-        __props__.__dict__["environment"] = environment
+        __props__.__dict__["access"] = access
+        __props__.__dict__["config"] = config
+        __props__.__dict__["key"] = key
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
-        return Donfig(resource_name, opts=opts, __props__=__props__)
+        return ServiceToken(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter
+    def access(self) -> pulumi.Output[Optional[str]]:
+        """
+        The access level (read or read/write)
+        """
+        return pulumi.get(self, "access")
+
+    @property
+    @pulumi.getter
+    def config(self) -> pulumi.Output[str]:
+        """
+        The name of the Doppler config where the service token is located
+        """
+        return pulumi.get(self, "config")
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[str]:
+    def key(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler environment where the config is located
+        The key for the Doppler service token
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler config
+        The name of the Doppler service token
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Output[str]:
         """
-        The name of the Doppler project where the config is located
+        The name of the Doppler project where the service token is located
         """
         return pulumi.get(self, "project")
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/project.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,262 +5,211 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['EnvironmentArgs', 'Environment']
+__all__ = ['ProjectArgs', 'Project']
 
 @pulumi.input_type
-class EnvironmentArgs:
+class ProjectArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
-                 project: pulumi.Input[str],
-                 slug: pulumi.Input[str]):
+                 description: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Environment resource.
-        :param pulumi.Input[str] name: The name of the Doppler environment
-        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
-        :param pulumi.Input[str] slug: The slug of the Doppler environment
+        The set of arguments for constructing a Project resource.
+        :param pulumi.Input[str] name: The name of the Doppler project
+        :param pulumi.Input[str] description: The description of the Doppler project
         """
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "project", project)
-        pulumi.set(__self__, "slug", slug)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The name of the Doppler environment
+        The name of the Doppler project
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Input[str]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler project where the environment is located
+        The description of the Doppler project
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "description")
 
-    @project.setter
-    def project(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project", value)
-
-    @property
-    @pulumi.getter
-    def slug(self) -> pulumi.Input[str]:
-        """
-        The slug of the Doppler environment
-        """
-        return pulumi.get(self, "slug")
-
-    @slug.setter
-    def slug(self, value: pulumi.Input[str]):
-        pulumi.set(self, "slug", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
 
 @pulumi.input_type
-class _EnvironmentState:
+class _ProjectState:
     def __init__(__self__, *,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 slug: Optional[pulumi.Input[str]] = None):
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Environment resources.
-        :param pulumi.Input[str] name: The name of the Doppler environment
-        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
-        :param pulumi.Input[str] slug: The slug of the Doppler environment
+        Input properties used for looking up and filtering Project resources.
+        :param pulumi.Input[str] description: The description of the Doppler project
+        :param pulumi.Input[str] name: The name of the Doppler project
         """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if project is not None:
-            pulumi.set(__self__, "project", project)
-        if slug is not None:
-            pulumi.set(__self__, "slug", slug)
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of the Doppler environment
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def project(self) -> Optional[pulumi.Input[str]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Doppler project where the environment is located
+        The description of the Doppler project
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "description")
 
-    @project.setter
-    def project(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def slug(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The slug of the Doppler environment
+        The name of the Doppler project
         """
-        return pulumi.get(self, "slug")
+        return pulumi.get(self, "name")
 
-    @slug.setter
-    def slug(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "slug", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
-class Environment(pulumi.CustomResource):
+class Project(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manage a Doppler environment.
+        Manage a Doppler project.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci = doppler.Environment("backendCi",
-            name="Continuous Integration",
-            project="backend",
-            slug="ci")
+        backend = doppler.Project("backend",
+            name="backend",
+            description="The main backend project")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name of the Doppler environment
-        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
-        :param pulumi.Input[str] slug: The slug of the Doppler environment
+        :param pulumi.Input[str] description: The description of the Doppler project
+        :param pulumi.Input[str] name: The name of the Doppler project
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EnvironmentArgs,
+                 args: ProjectArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manage a Doppler environment.
+        Manage a Doppler project.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_doppler as doppler
 
-        backend_ci = doppler.Environment("backendCi",
-            name="Continuous Integration",
-            project="backend",
-            slug="ci")
+        backend = doppler.Project("backend",
+            name="backend",
+            description="The main backend project")
         ```
 
         :param str resource_name: The name of the resource.
-        :param EnvironmentArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EnvironmentArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EnvironmentArgs.__new__(EnvironmentArgs)
+            __props__ = ProjectArgs.__new__(ProjectArgs)
 
+            __props__.__dict__["description"] = description
             if name is None and not opts.urn:
                 raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            if project is None and not opts.urn:
-                raise TypeError("Missing required property 'project'")
-            __props__.__dict__["project"] = project
-            if slug is None and not opts.urn:
-                raise TypeError("Missing required property 'slug'")
-            __props__.__dict__["slug"] = slug
-        super(Environment, __self__).__init__(
-            'doppler:index/environment:Environment',
+        super(Project, __self__).__init__(
+            'doppler:index/project:Project',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            project: Optional[pulumi.Input[str]] = None,
-            slug: Optional[pulumi.Input[str]] = None) -> 'Environment':
+            description: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None) -> 'Project':
         """
-        Get an existing Environment resource's state with the given name, id, and optional extra
+        Get an existing Project resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name of the Doppler environment
-        :param pulumi.Input[str] project: The name of the Doppler project where the environment is located
-        :param pulumi.Input[str] slug: The slug of the Doppler environment
+        :param pulumi.Input[str] description: The description of the Doppler project
+        :param pulumi.Input[str] name: The name of the Doppler project
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _EnvironmentState.__new__(_EnvironmentState)
+        __props__ = _ProjectState.__new__(_ProjectState)
 
+        __props__.__dict__["description"] = description
         __props__.__dict__["name"] = name
-        __props__.__dict__["project"] = project
-        __props__.__dict__["slug"] = slug
-        return Environment(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        """
-        The name of the Doppler environment
-        """
-        return pulumi.get(self, "name")
+        return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        The name of the Doppler project where the environment is located
+        The description of the Doppler project
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def slug(self) -> pulumi.Output[str]:
+    def name(self) -> pulumi.Output[str]:
         """
-        The slug of the Doppler environment
+        The name of the Doppler project
         """
-        return pulumi.get(self, "slug")
+        return pulumi.get(self, "name")
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/secret.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 
 @pulumi.input_type
 class SecretArgs:
     def __init__(__self__, *,
                  config: pulumi.Input[str],
                  name: pulumi.Input[str],
                  project: pulumi.Input[str],
-                 value: pulumi.Input[str]):
+                 value: pulumi.Input[str],
+                 visibility: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Secret resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] name: The name of the Doppler secret
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] value: The raw secret value
+        :param pulumi.Input[str] visibility: The visibility of the secret
         """
         pulumi.set(__self__, "config", config)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "value", value)
+        if visibility is not None:
+            pulumi.set(__self__, "visibility", visibility)
 
     @property
     @pulumi.getter
     def config(self) -> pulumi.Input[str]:
         """
         The name of the Doppler config
         """
@@ -74,41 +78,57 @@
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
+    @property
+    @pulumi.getter
+    def visibility(self) -> Optional[pulumi.Input[str]]:
+        """
+        The visibility of the secret
+        """
+        return pulumi.get(self, "visibility")
+
+    @visibility.setter
+    def visibility(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "visibility", value)
+
 
 @pulumi.input_type
 class _SecretState:
     def __init__(__self__, *,
                  computed: Optional[pulumi.Input[str]] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
+                 value: Optional[pulumi.Input[str]] = None,
+                 visibility: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Secret resources.
         :param pulumi.Input[str] computed: The computed secret value, after resolving secret references
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] name: The name of the Doppler secret
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] value: The raw secret value
+        :param pulumi.Input[str] visibility: The visibility of the secret
         """
         if computed is not None:
             pulumi.set(__self__, "computed", computed)
         if config is not None:
             pulumi.set(__self__, "config", config)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if value is not None:
             pulumi.set(__self__, "value", value)
+        if visibility is not None:
+            pulumi.set(__self__, "visibility", visibility)
 
     @property
     @pulumi.getter
     def computed(self) -> Optional[pulumi.Input[str]]:
         """
         The computed secret value, after resolving secret references
         """
@@ -162,34 +182,48 @@
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value", value)
 
+    @property
+    @pulumi.getter
+    def visibility(self) -> Optional[pulumi.Input[str]]:
+        """
+        The visibility of the secret
+        """
+        return pulumi.get(self, "visibility")
+
+    @visibility.setter
+    def visibility(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "visibility", value)
+
 
 class Secret(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None,
+                 visibility: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage a single Doppler secret in a config.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] name: The name of the Doppler secret
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] value: The raw secret value
+        :param pulumi.Input[str] visibility: The visibility of the secret
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SecretArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -211,14 +245,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None,
+                 visibility: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -232,14 +267,15 @@
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if value is None and not opts.urn:
                 raise TypeError("Missing required property 'value'")
             __props__.__dict__["value"] = None if value is None else pulumi.Output.secret(value)
+            __props__.__dict__["visibility"] = visibility
             __props__.__dict__["computed"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["computed", "value"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Secret, __self__).__init__(
             'doppler:index/secret:Secret',
             resource_name,
             __props__,
@@ -249,37 +285,40 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             computed: Optional[pulumi.Input[str]] = None,
             config: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
-            value: Optional[pulumi.Input[str]] = None) -> 'Secret':
+            value: Optional[pulumi.Input[str]] = None,
+            visibility: Optional[pulumi.Input[str]] = None) -> 'Secret':
         """
         Get an existing Secret resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] computed: The computed secret value, after resolving secret references
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] name: The name of the Doppler secret
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] value: The raw secret value
+        :param pulumi.Input[str] visibility: The visibility of the secret
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecretState.__new__(_SecretState)
 
         __props__.__dict__["computed"] = computed
         __props__.__dict__["config"] = config
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
         __props__.__dict__["value"] = value
+        __props__.__dict__["visibility"] = visibility
         return Secret(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def computed(self) -> pulumi.Output[str]:
         """
         The computed secret value, after resolving secret references
@@ -314,7 +353,15 @@
     @pulumi.getter
     def value(self) -> pulumi.Output[str]:
         """
         The raw secret value
         """
         return pulumi.get(self, "value")
 
+    @property
+    @pulumi.getter
+    def visibility(self) -> pulumi.Output[Optional[str]]:
+        """
+        The visibility of the secret
+        """
+        return pulumi.get(self, "visibility")
+
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler/secrets.py` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler/get_secrets.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'SecretsResult',
-    'AwaitableSecretsResult',
-    'secrets',
-    'secrets_output',
+    'GetSecretsResult',
+    'AwaitableGetSecretsResult',
+    'get_secrets',
+    'get_secrets_output',
 ]
 
 @pulumi.output_type
-class SecretsResult:
+class GetSecretsResult:
     """
-    A collection of values returned by Secrets.
+    A collection of values returned by getSecrets.
     """
     def __init__(__self__, config=None, id=None, map=None, project=None):
         if config and not isinstance(config, str):
             raise TypeError("Expected argument 'config' to be a str")
         pulumi.set(__self__, "config", config)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
@@ -64,53 +64,53 @@
     def project(self) -> Optional[str]:
         """
         The name of the Doppler project (required for personal tokens)
         """
         return pulumi.get(self, "project")
 
 
-class AwaitableSecretsResult(SecretsResult):
+class AwaitableGetSecretsResult(GetSecretsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return SecretsResult(
+        return GetSecretsResult(
             config=self.config,
             id=self.id,
             map=self.map,
             project=self.project)
 
 
-def secrets(config: Optional[str] = None,
-            project: Optional[str] = None,
-            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableSecretsResult:
+def get_secrets(config: Optional[str] = None,
+                project: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecretsResult:
     """
     Retrieve all secrets in the config.
 
 
     :param str config: The name of the Doppler config (required for personal tokens)
     :param str project: The name of the Doppler project (required for personal tokens)
     """
     __args__ = dict()
     __args__['config'] = config
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('doppler:index/secrets:Secrets', __args__, opts=opts, typ=SecretsResult).value
+    __ret__ = pulumi.runtime.invoke('doppler:index/getSecrets:getSecrets', __args__, opts=opts, typ=GetSecretsResult).value
 
-    return AwaitableSecretsResult(
+    return AwaitableGetSecretsResult(
         config=pulumi.get(__ret__, 'config'),
         id=pulumi.get(__ret__, 'id'),
         map=pulumi.get(__ret__, 'map'),
         project=pulumi.get(__ret__, 'project'))
 
 
-@_utilities.lift_output_func(secrets)
-def secrets_output(config: Optional[pulumi.Input[Optional[str]]] = None,
-                   project: Optional[pulumi.Input[Optional[str]]] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[SecretsResult]:
+@_utilities.lift_output_func(get_secrets)
+def get_secrets_output(config: Optional[pulumi.Input[Optional[str]]] = None,
+                       project: Optional[pulumi.Input[Optional[str]]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretsResult]:
     """
     Retrieve all secrets in the config.
 
 
     :param str config: The name of the Doppler config (required for personal tokens)
     :param str project: The name of the Doppler project (required for personal tokens)
     """
```

### Comparing `pulumiverse_doppler-0.1.2/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.2.0/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.1.2/setup.py` & `pulumiverse_doppler-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.2"
+VERSION = "0.2.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

