# Comparing `tmp/mypy_boto3_ec2-1.34.91.tar.gz` & `tmp/mypy_boto3_ec2-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_ec2-1.34.91.tar", last modified: Wed Apr 24 19:19:05 2024, max compression
+gzip compressed data, was "mypy_boto3_ec2-1.34.96.tar", last modified: Wed May  1 19:21:15 2024, max compression
```

## Comparing `mypy_boto3_ec2-1.34.91.tar` & `mypy_boto3_ec2-1.34.96.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.343903 mypy_boto3_ec2-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-24 19:19:05.343903 mypy_boto3_ec2-1.34.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.339903 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   543508 2024-04-24 19:18:13.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   543505 2024-04-24 19:18:10.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-04-24 19:18:20.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-04-24 19:18:19.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-04-24 19:18:18.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-04-24 19:18:17.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   272056 2024-04-24 19:18:16.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   271978 2024-04-24 19:18:15.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   870702 2024-04-24 19:18:36.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   870702 2024-04-24 19:18:31.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:18:07.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-24 19:18:18.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-04-24 19:18:18.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.343903 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:19:05.000000 mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:05.343903 mypy_boto3_ec2-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-24 19:18:06.000000 mypy_boto3_ec2-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.804324 mypy_boto3_ec2-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   544008 2024-05-01 19:20:17.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   544005 2024-05-01 19:20:14.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-05-01 19:20:23.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-05-01 19:20:23.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   187386 2024-05-01 19:20:21.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187243 2024-05-01 19:20:20.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   272189 2024-05-01 19:20:20.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   272111 2024-05-01 19:20:18.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   885369 2024-05-01 19:20:40.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   885369 2024-05-01 19:20:34.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-05-01 19:20:22.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-05-01 19:20:21.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:15.804324 mypy_boto3_ec2-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-01 19:20:10.000000 mypy_boto3_ec2-1.34.96/setup.py
```

### Comparing `mypy_boto3_ec2-1.34.91/LICENSE` & `mypy_boto3_ec2-1.34.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/PKG-INFO` & `mypy_boto3_ec2-1.34.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.91
-Summary: Type annotations for boto3.EC2 1.34.91 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_ec2-1.34.91/README.md` & `mypy_boto3_ec2-1.34.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__init__.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__init__.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/__main__.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.34.91\n"
-        "Version:         1.34.91\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.EC2 1.34.96\n"
+        "Version:         1.34.96\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.91")
+    print("1.34.96")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/client.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,27 +751,27 @@
     InstanceEventWindowAssociationRequestTypeDef,
     InstanceEventWindowDisassociationRequestTypeDef,
     InstanceEventWindowTimeRangeRequestTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
-    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationUnionTypeDef,
     InstanceRequirementsRequestTypeDef,
     InstanceRequirementsWithMetadataRequestTypeDef,
     InstanceSpecificationTypeDef,
     IntegrateServicesTypeDef,
     IpamCidrAuthorizationContextTypeDef,
     IpamPoolSourceResourceRequestTypeDef,
-    IpPermissionTypeDef,
+    IpPermissionUnionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     KeyPairTypeDef,
     LaunchPermissionModificationsTypeDef,
-    LaunchTemplateConfigTypeDef,
+    LaunchTemplateConfigUnionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LicenseConfigurationRequestTypeDef,
     ListImagesInRecycleBinResultTypeDef,
     ListSnapshotsInRecycleBinResultTypeDef,
     LoadPermissionModificationsTypeDef,
     LockSnapshotResultTypeDef,
     ModifyAddressAttributeResultTypeDef,
@@ -908,25 +908,25 @@
     SearchTransitGatewayRoutesResultTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     SecurityGroupRuleUpdateTypeDef,
     SlotDateTimeRangeRequestTypeDef,
     SlotStartTimeRangeRequestTypeDef,
     SnapshotDiskContainerTypeDef,
     SnapshotResponseTypeDef,
-    SpotFleetRequestConfigDataTypeDef,
+    SpotFleetRequestConfigDataUnionTypeDef,
     SpotOptionsRequestTypeDef,
     StartInstancesResultTypeDef,
     StartNetworkInsightsAccessScopeAnalysisResultTypeDef,
     StartNetworkInsightsAnalysisResultTypeDef,
     StartVpcEndpointServicePrivateDnsVerificationResultTypeDef,
     StopInstancesResultTypeDef,
     StorageLocationTypeDef,
-    StorageTypeDef,
+    StorageUnionTypeDef,
     SubnetConfigurationTypeDef,
-    TagSpecificationTypeDef,
+    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TargetCapacitySpecificationRequestTypeDef,
     TargetConfigurationRequestTypeDef,
     TerminateClientVpnConnectionsResultTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     TrafficMirrorPortRangeRequestTypeDef,
@@ -1022,15 +1022,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#exceptions)
         """
 
     def accept_address_transfer(
         self,
         *,
         Address: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> AcceptAddressTransferResultTypeDef:
         """
         Accepts an Elastic IP address transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.accept_address_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#accept_address_transfer)
@@ -1124,15 +1124,15 @@
         *,
         Domain: DomainTypeType = ...,
         Address: str = ...,
         PublicIpv4Pool: str = ...,
         NetworkBorderGroup: str = ...,
         CustomerOwnedIpv4Pool: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> AllocateAddressResultTypeDef:
         """
         Allocates an Elastic IP address to your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.allocate_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#allocate_address)
         """
@@ -1142,15 +1142,15 @@
         *,
         AvailabilityZone: str,
         AutoPlacement: AutoPlacementType = ...,
         ClientToken: str = ...,
         InstanceType: str = ...,
         InstanceFamily: str = ...,
         Quantity: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         HostRecovery: HostRecoveryType = ...,
         OutpostArn: str = ...,
         HostMaintenance: HostMaintenanceType = ...,
         AssetIds: Sequence[str] = ...,
     ) -> AllocateHostsResultTypeDef:
         """
         Allocates a Dedicated Host to your account.
@@ -1337,15 +1337,15 @@
 
     def associate_ipam_resource_discovery(
         self,
         *,
         IpamId: str,
         IpamResourceDiscoveryId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> AssociateIpamResourceDiscoveryResultTypeDef:
         """
         Associates an IPAM resource discovery with an Amazon VPC IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.associate_ipam_resource_discovery)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#associate_ipam_resource_discovery)
@@ -1578,16 +1578,16 @@
         """
 
     def authorize_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
@@ -1601,31 +1601,31 @@
     def authorize_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> AuthorizeSecurityGroupIngressResultTypeDef:
         """
         Adds the specified inbound (ingress) rules to a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#authorize_security_group_ingress)
         """
 
     def bundle_instance(
-        self, *, InstanceId: str, Storage: StorageTypeDef, DryRun: bool = ...
+        self, *, InstanceId: str, Storage: StorageUnionTypeDef, DryRun: bool = ...
     ) -> BundleInstanceResultTypeDef:
         """
         Bundles an Amazon instance store-backed Windows instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.bundle_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#bundle_instance)
         """
@@ -1785,15 +1785,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         DestinationOutpostArn: str = ...,
         DryRun: bool = ...,
         CopyImageTags: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CopyImageResultTypeDef:
         """
         Initiates the copy of an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#copy_image)
         """
@@ -1805,15 +1805,15 @@
         SourceSnapshotId: str,
         Description: str = ...,
         DestinationOutpostArn: str = ...,
         DestinationRegion: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         PresignedUrl: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a point-in-time snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#copy_snapshot)
@@ -1830,15 +1830,15 @@
         AvailabilityZoneId: str = ...,
         Tenancy: CapacityReservationTenancyType = ...,
         EbsOptimized: bool = ...,
         EphemeralStorage: bool = ...,
         EndDate: TimestampTypeDef = ...,
         EndDateType: EndDateTypeType = ...,
         InstanceMatchCriteria: InstanceMatchCriteriaType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         OutpostArn: str = ...,
         PlacementGroupArn: str = ...,
     ) -> CreateCapacityReservationResultTypeDef:
         """
         Creates a new Capacity Reservation with the specified attributes.
 
@@ -1852,29 +1852,29 @@
         InstanceTypeSpecifications: Sequence[ReservationFleetInstanceSpecificationTypeDef],
         TotalTargetCapacity: int,
         AllocationStrategy: str = ...,
         ClientToken: str = ...,
         Tenancy: Literal["default"] = ...,
         EndDate: TimestampTypeDef = ...,
         InstanceMatchCriteria: Literal["open"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateCapacityReservationFleetResultTypeDef:
         """
         Creates a Capacity Reservation Fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_capacity_reservation_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_capacity_reservation_fleet)
         """
 
     def create_carrier_gateway(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateCarrierGatewayResultTypeDef:
         """
         Creates a carrier gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_carrier_gateway)
@@ -1891,15 +1891,15 @@
         DnsServers: Sequence[str] = ...,
         TransportProtocol: TransportProtocolType = ...,
         VpnPort: int = ...,
         Description: str = ...,
         SplitTunnel: bool = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         VpcId: str = ...,
         SelfServicePortal: SelfServicePortalType = ...,
         ClientConnectOptions: ClientConnectOptionsTypeDef = ...,
         SessionTimeoutHours: int = ...,
         ClientLoginBannerOptions: ClientLoginBannerOptionsTypeDef = ...,
     ) -> CreateClientVpnEndpointResultTypeDef:
@@ -1937,15 +1937,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_coip_cidr)
         """
 
     def create_coip_pool(
         self,
         *,
         LocalGatewayRouteTableId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateCoipPoolResultTypeDef:
         """
         Creates a pool of customer-owned IP (CoIP) addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_coip_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_coip_pool)
@@ -1954,15 +1954,15 @@
     def create_customer_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         BgpAsn: int = ...,
         PublicIp: str = ...,
         CertificateArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DeviceName: str = ...,
         IpAddress: str = ...,
         DryRun: bool = ...,
     ) -> CreateCustomerGatewayResultTypeDef:
         """
         Provides information to Amazon Web Services about your customer gateway device.
 
@@ -1992,15 +1992,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_default_vpc)
         """
 
     def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateDhcpOptionsResultTypeDef:
         """
         Creates a custom set of DHCP options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_dhcp_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_dhcp_options)
@@ -2008,15 +2008,15 @@
 
     def create_egress_only_internet_gateway(
         self,
         *,
         VpcId: str,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateEgressOnlyInternetGatewayResultTypeDef:
         """
         [IPv6 only] Creates an egress-only internet gateway for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_egress_only_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_egress_only_internet_gateway)
         """
@@ -2032,15 +2032,15 @@
         OnDemandOptions: OnDemandOptionsRequestTypeDef = ...,
         ExcessCapacityTerminationPolicy: FleetExcessCapacityTerminationPolicyType = ...,
         TerminateInstancesWithExpiration: bool = ...,
         Type: FleetTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
         ReplaceUnhealthyInstances: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         Context: str = ...,
     ) -> CreateFleetResultTypeDef:
         """
         Creates an EC2 Fleet that contains the configuration information for On-Demand
         Instances and Spot
         Instances.
 
@@ -2058,15 +2058,15 @@
         DeliverLogsPermissionArn: str = ...,
         DeliverCrossAccountRole: str = ...,
         LogGroupName: str = ...,
         TrafficType: TrafficTypeType = ...,
         LogDestinationType: LogDestinationTypeType = ...,
         LogDestination: str = ...,
         LogFormat: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MaxAggregationInterval: int = ...,
         DestinationOptions: DestinationOptionsRequestTypeDef = ...,
     ) -> CreateFlowLogsResultTypeDef:
         """
         Creates one or more flow logs to capture information about IP traffic for a
         specific network interface, subnet, or
         VPC.
@@ -2080,15 +2080,15 @@
         *,
         InputStorageLocation: StorageLocationTypeDef,
         DryRun: bool = ...,
         LogsStorageLocation: StorageLocationTypeDef = ...,
         Description: str = ...,
         Name: str = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateFpgaImageResultTypeDef:
         """
         Creates an Amazon FPGA Image (AFI) from the specified design checkpoint (DCP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fpga_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_fpga_image)
         """
@@ -2098,15 +2098,15 @@
         *,
         InstanceId: str,
         Name: str,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         Description: str = ...,
         DryRun: bool = ...,
         NoReboot: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateImageResultTypeDef:
         """
         Creates an Amazon EBS-backed AMI from an Amazon EBS-backed instance that is
         either running or
         stopped.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_image)
@@ -2117,15 +2117,15 @@
         self,
         *,
         SubnetId: str,
         DryRun: bool = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreserveClientIp: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceConnectEndpointResultTypeDef:
         """
         Creates an EC2 Instance Connect Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_connect_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_instance_connect_endpoint)
         """
@@ -2133,15 +2133,15 @@
     def create_instance_event_window(
         self,
         *,
         DryRun: bool = ...,
         Name: str = ...,
         TimeRanges: Sequence[InstanceEventWindowTimeRangeRequestTypeDef] = ...,
         CronExpression: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceEventWindowResultTypeDef:
         """
         Creates an event window in which scheduled events for the associated Amazon EC2
         instances can
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_event_window)
@@ -2151,40 +2151,40 @@
     def create_instance_export_task(
         self,
         *,
         ExportToS3Task: ExportToS3TaskSpecificationTypeDef,
         InstanceId: str,
         TargetEnvironment: ExportEnvironmentType,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceExportTaskResultTypeDef:
         """
         Exports a running or stopped instance to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_instance_export_task)
         """
 
     def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
     ) -> CreateInternetGatewayResultTypeDef:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_internet_gateway)
         """
 
     def create_ipam(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tier: IpamTierType = ...,
     ) -> CreateIpamResultTypeDef:
         """
         Create an IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam)
@@ -2202,15 +2202,15 @@
         Description: str = ...,
         AutoImport: bool = ...,
         PubliclyAdvertisable: bool = ...,
         AllocationMinNetmaskLength: int = ...,
         AllocationMaxNetmaskLength: int = ...,
         AllocationDefaultNetmaskLength: int = ...,
         AllocationResourceTags: Sequence[RequestIpamResourceTagTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         AwsService: Literal["ec2"] = ...,
         PublicIpSource: IpamPoolPublicIpSourceType = ...,
         SourceResource: IpamPoolSourceResourceRequestTypeDef = ...,
     ) -> CreateIpamPoolResultTypeDef:
         """
         Create an IP address pool for Amazon VPC IP Address Manager (IPAM).
@@ -2221,15 +2221,15 @@
 
     def create_ipam_resource_discovery(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateIpamResourceDiscoveryResultTypeDef:
         """
         Creates an IPAM resource discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_resource_discovery)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_ipam_resource_discovery)
@@ -2237,15 +2237,15 @@
 
     def create_ipam_scope(
         self,
         *,
         IpamId: str,
         DryRun: bool = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateIpamScopeResultTypeDef:
         """
         Create an IPAM scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_ipam_scope)
@@ -2253,15 +2253,15 @@
 
     def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         KeyFormat: KeyFormatType = ...,
     ) -> KeyPairTypeDef:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK
         format.
 
@@ -2273,15 +2273,15 @@
         self,
         *,
         LaunchTemplateName: str,
         LaunchTemplateData: RequestLaunchTemplateDataTypeDef,
         DryRun: bool = ...,
         ClientToken: str = ...,
         VersionDescription: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateLaunchTemplateResultTypeDef:
         """
         Creates a launch template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_launch_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_launch_template)
         """
@@ -2323,45 +2323,45 @@
         """
 
     def create_local_gateway_route_table(
         self,
         *,
         LocalGatewayId: str,
         Mode: LocalGatewayRouteTableModeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableResultTypeDef:
         """
         Creates a local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table)
         """
 
     def create_local_gateway_route_table_virtual_interface_group_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         LocalGatewayVirtualInterfaceGroupId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationResultTypeDef:
         """
         Creates a local gateway route table virtual interface group association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_virtual_interface_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table_virtual_interface_group_association)
         """
 
     def create_local_gateway_route_table_vpc_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableVpcAssociationResultTypeDef:
         """
         Associates the specified VPC with the specified local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table_vpc_association)
@@ -2371,15 +2371,15 @@
         self,
         *,
         PrefixListName: str,
         MaxEntries: int,
         AddressFamily: str,
         DryRun: bool = ...,
         Entries: Sequence[AddPrefixListEntryTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateManagedPrefixListResultTypeDef:
         """
         Creates a managed prefix list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_managed_prefix_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_managed_prefix_list)
@@ -2388,15 +2388,15 @@
     def create_nat_gateway(
         self,
         *,
         SubnetId: str,
         AllocationId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ConnectivityType: ConnectivityTypeType = ...,
         PrivateIpAddress: str = ...,
         SecondaryAllocationIds: Sequence[str] = ...,
         SecondaryPrivateIpAddresses: Sequence[str] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
     ) -> CreateNatGatewayResultTypeDef:
         """
@@ -2407,15 +2407,15 @@
         """
 
     def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateNetworkAclResultTypeDef:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_network_acl)
@@ -2444,15 +2444,15 @@
 
     def create_network_insights_access_scope(
         self,
         *,
         ClientToken: str,
         MatchPaths: Sequence[AccessScopePathRequestTypeDef] = ...,
         ExcludePaths: Sequence[AccessScopePathRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateNetworkInsightsAccessScopeResultTypeDef:
         """
         Creates a Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_insights_access_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_network_insights_access_scope)
@@ -2464,15 +2464,15 @@
         Source: str,
         Protocol: ProtocolType,
         ClientToken: str,
         SourceIp: str = ...,
         DestinationIp: str = ...,
         Destination: str = ...,
         DestinationPort: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         FilterAtSource: PathRequestFilterTypeDef = ...,
         FilterAtDestination: PathRequestFilterTypeDef = ...,
     ) -> CreateNetworkInsightsPathResultTypeDef:
         """
         Creates a path to analyze for reachability.
 
@@ -2493,15 +2493,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         EnablePrimaryIpv6: bool = ...,
         ConnectionTrackingSpecification: ConnectionTrackingSpecificationRequestTypeDef = ...,
     ) -> CreateNetworkInterfaceResultTypeDef:
         """
         Creates a network interface in the specified subnet.
 
@@ -2530,26 +2530,26 @@
     def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...,
     ) -> CreatePlacementGroupResultTypeDef:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_placement_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_placement_group)
         """
 
     def create_public_ipv4_pool(
-        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
+        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
     ) -> CreatePublicIpv4PoolResultTypeDef:
         """
         Creates a public IPv4 address pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_public_ipv4_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_public_ipv4_pool)
         """
@@ -2557,15 +2557,15 @@
     def create_replace_root_volume_task(
         self,
         *,
         InstanceId: str,
         SnapshotId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ImageId: str = ...,
         DeleteReplacedRootVolume: bool = ...,
     ) -> CreateReplaceRootVolumeTaskResultTypeDef:
         """
         Replaces the EBS-backed root volume for a `running` instance with a new volume
         that is restored to the original root volume's launch state, that is restored
         to a specific snapshot taken from the original root volume, or that is restored
@@ -2595,15 +2595,15 @@
 
     def create_restore_image_task(
         self,
         *,
         Bucket: str,
         ObjectKey: str,
         Name: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateRestoreImageTaskResultTypeDef:
         """
         Starts a task that restores an AMI from an Amazon S3 object that was previously
         created by using
         [CreateStoreImageTask](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateStoreImageTask.html).
 
@@ -2639,15 +2639,15 @@
         """
 
     def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateRouteTableResultTypeDef:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_route_table)
@@ -2655,15 +2655,15 @@
 
     def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateSecurityGroupResultTypeDef:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_security_group)
@@ -2671,15 +2671,15 @@
 
     def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> SnapshotResponseTypeDef:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_snapshot)
@@ -2687,15 +2687,15 @@
 
     def create_snapshots(
         self,
         *,
         InstanceSpecification: InstanceSpecificationTypeDef,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         CopyTagsFromSource: Literal["volume"] = ...,
     ) -> CreateSnapshotsResultTypeDef:
         """
         Creates crash-consistent snapshots of multiple EBS volumes and stores the data
         in
         S3.
@@ -2731,15 +2731,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_store_image_task)
         """
 
     def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...,
@@ -2759,15 +2759,15 @@
         self,
         *,
         SubnetId: str,
         Cidr: str,
         ReservationType: SubnetCidrReservationTypeType,
         Description: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateSubnetCidrReservationResultTypeDef:
         """
         Creates a subnet CIDR reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_subnet_cidr_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_subnet_cidr_reservation)
         """
@@ -2784,15 +2784,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_tags)
         """
 
     def create_traffic_mirror_filter(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateTrafficMirrorFilterResultTypeDef:
         """
         Creates a Traffic Mirror filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_filter)
@@ -2828,15 +2828,15 @@
         NetworkInterfaceId: str,
         TrafficMirrorTargetId: str,
         TrafficMirrorFilterId: str,
         SessionNumber: int,
         PacketLength: int = ...,
         VirtualNetworkId: int = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateTrafficMirrorSessionResultTypeDef:
         """
         Creates a Traffic Mirror session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_session)
@@ -2845,15 +2845,15 @@
 
     def create_traffic_mirror_target(
         self,
         *,
         NetworkInterfaceId: str = ...,
         NetworkLoadBalancerArn: str = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
         GatewayLoadBalancerEndpointId: str = ...,
     ) -> CreateTrafficMirrorTargetResultTypeDef:
         """
         Creates a target for your Traffic Mirror session.
 
@@ -2862,30 +2862,30 @@
         """
 
     def create_transit_gateway(
         self,
         *,
         Description: str = ...,
         Options: TransitGatewayRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayResultTypeDef:
         """
         Creates a transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway)
         """
 
     def create_transit_gateway_connect(
         self,
         *,
         TransportTransitGatewayAttachmentId: str,
         Options: CreateTransitGatewayConnectRequestOptionsTypeDef,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayConnectResultTypeDef:
         """
         Creates a Connect attachment from a specified transit gateway attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_connect)
@@ -2895,15 +2895,15 @@
         self,
         *,
         TransitGatewayAttachmentId: str,
         PeerAddress: str,
         InsideCidrBlocks: Sequence[str],
         TransitGatewayAddress: str = ...,
         BgpOptions: TransitGatewayConnectRequestBgpOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayConnectPeerResultTypeDef:
         """
         Creates a Connect peer for a specified transit gateway Connect attachment
         between a transit gateway and an
         appliance.
 
@@ -2912,15 +2912,15 @@
         """
 
     def create_transit_gateway_multicast_domain(
         self,
         *,
         TransitGatewayId: str,
         Options: CreateTransitGatewayMulticastDomainRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayMulticastDomainResultTypeDef:
         """
         Creates a multicast domain using the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_multicast_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_multicast_domain)
@@ -2930,15 +2930,15 @@
         self,
         *,
         TransitGatewayId: str,
         PeerTransitGatewayId: str,
         PeerAccountId: str,
         PeerRegion: str,
         Options: CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayPeeringAttachmentResultTypeDef:
         """
         Requests a transit gateway peering attachment between the specified transit
         gateway (requester) and a peer transit gateway
         (accepter).
 
@@ -2946,15 +2946,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_peering_attachment)
         """
 
     def create_transit_gateway_policy_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayPolicyTableResultTypeDef:
         """
         Creates a transit gateway policy table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_policy_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_policy_table)
@@ -2994,30 +2994,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route)
         """
 
     def create_transit_gateway_route_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayRouteTableResultTypeDef:
         """
         Creates a route table for the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route_table)
         """
 
     def create_transit_gateway_route_table_announcement(
         self,
         *,
         TransitGatewayRouteTableId: str,
         PeeringAttachmentId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayRouteTableAnnouncementResultTypeDef:
         """
         Advertises a new transit gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table_announcement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route_table_announcement)
@@ -3026,15 +3026,15 @@
     def create_transit_gateway_vpc_attachment(
         self,
         *,
         TransitGatewayId: str,
         VpcId: str,
         SubnetIds: Sequence[str],
         Options: CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayVpcAttachmentResultTypeDef:
         """
         Attaches the specified VPC to the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_vpc_attachment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_vpc_attachment)
@@ -3050,15 +3050,15 @@
         ApplicationDomain: str,
         EndpointDomainPrefix: str,
         SecurityGroupIds: Sequence[str] = ...,
         LoadBalancerOptions: CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef = ...,
         NetworkInterfaceOptions: CreateVerifiedAccessEndpointEniOptionsTypeDef = ...,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessEndpointResultTypeDef:
         """
         An Amazon Web Services Verified Access endpoint is where you define your
         application along with an optional endpoint-level access
@@ -3070,15 +3070,15 @@
 
     def create_verified_access_group(
         self,
         *,
         VerifiedAccessInstanceId: str,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessGroupResultTypeDef:
         """
         An Amazon Web Services Verified Access group is a collection of Amazon Web
         Services Verified Access endpoints who's associated applications have similar
@@ -3089,15 +3089,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_verified_access_group)
         """
 
     def create_verified_access_instance(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         FIPSEnabled: bool = ...,
     ) -> CreateVerifiedAccessInstanceResultTypeDef:
         """
         An Amazon Web Services Verified Access instance is a regional entity that
         evaluates application requests and grants access only when your security
@@ -3114,15 +3114,15 @@
         TrustProviderType: TrustProviderTypeType,
         PolicyReferenceName: str,
         UserTrustProviderType: UserTrustProviderTypeType = ...,
         DeviceTrustProviderType: DeviceTrustProviderTypeType = ...,
         OidcOptions: CreateVerifiedAccessTrustProviderOidcOptionsTypeDef = ...,
         DeviceOptions: CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessTrustProviderResultTypeDef:
         """
         A trust provider is a third-party entity that creates, maintains, and manages
         identity information for users and
@@ -3140,15 +3140,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...,
     ) -> VolumeResponseTypeDef:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability
@@ -3168,15 +3168,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcResultTypeDef:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_vpc)
         """
@@ -3192,15 +3192,15 @@
         RouteTableIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SubnetConfigurations: Sequence[SubnetConfigurationTypeDef] = ...,
     ) -> CreateVpcEndpointResultTypeDef:
         """
         Creates a VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_vpc_endpoint)
@@ -3230,15 +3230,15 @@
         DryRun: bool = ...,
         AcceptanceRequired: bool = ...,
         PrivateDnsName: str = ...,
         NetworkLoadBalancerArns: Sequence[str] = ...,
         GatewayLoadBalancerArns: Sequence[str] = ...,
         SupportedIpAddressTypes: Sequence[str] = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcEndpointServiceConfigurationResultTypeDef:
         """
         Creates a VPC endpoint service to which service consumers (Amazon Web Services
         accounts, users, and IAM roles) can
         connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint_service_configuration)
@@ -3249,15 +3249,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcPeeringConnectionResultTypeDef:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you
         own and an accepter VPC with which to create the
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_peering_connection)
@@ -3269,15 +3269,15 @@
         *,
         CustomerGatewayId: str,
         Type: str,
         VpnGatewayId: str = ...,
         TransitGatewayId: str = ...,
         DryRun: bool = ...,
         Options: VpnConnectionOptionsSpecificationTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpnConnectionResultTypeDef:
         """
         Creates a VPN connection between an existing virtual private gateway or transit
         gateway and a customer
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_connection)
@@ -3297,15 +3297,15 @@
         """
 
     def create_vpn_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         AvailabilityZone: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AmazonSideAsn: int = ...,
         DryRun: bool = ...,
     ) -> CreateVpnGatewayResultTypeDef:
         """
         Creates a virtual private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_gateway)
@@ -7208,15 +7208,15 @@
         DiskImageFormat: DiskImageFormatType,
         ImageId: str,
         S3ExportLocation: ExportTaskS3LocationRequestTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ExportImageResultTypeDef:
         """
         Exports an Amazon Machine Image (AMI) to a VM file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.export_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#export_image)
         """
@@ -7968,15 +7968,15 @@
         Encrypted: bool = ...,
         Hypervisor: str = ...,
         KmsKeyId: str = ...,
         LicenseType: str = ...,
         Platform: str = ...,
         RoleName: str = ...,
         LicenseSpecifications: Sequence[ImportImageLicenseConfigurationRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         UsageOperation: str = ...,
         BootMode: BootModeValuesType = ...,
     ) -> ImportImageResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_image)
@@ -8001,15 +8001,15 @@
 
     def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ImportKeyPairResultTypeDef:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_key_pair)
@@ -8023,15 +8023,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         DiskContainer: SnapshotDiskContainerTypeDef = ...,
         DryRun: bool = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ImportSnapshotResultTypeDef:
         """
         Imports a disk into an EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#import_snapshot)
         """
@@ -8702,15 +8702,15 @@
         """
 
     def modify_spot_fleet_request(
         self,
         *,
         SpotFleetRequestId: str,
         ExcessCapacityTerminationPolicy: ExcessCapacityTerminationPolicyType = ...,
-        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigTypeDef] = ...,
+        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigUnionTypeDef] = ...,
         TargetCapacity: int = ...,
         OnDemandTargetCapacity: int = ...,
         Context: str = ...,
     ) -> ModifySpotFleetRequestResponseTypeDef:
         """
         Modifies the specified Spot Fleet request.
 
@@ -9224,15 +9224,15 @@
         self,
         *,
         Cidr: str,
         CidrAuthorizationContext: CidrAuthorizationContextTypeDef = ...,
         PubliclyAdvertisable: bool = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        PoolTagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        PoolTagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiRegion: bool = ...,
         NetworkBorderGroup: str = ...,
     ) -> ProvisionByoipCidrResultTypeDef:
         """
         Provisions an IPv4 or IPv6 address range for use with your Amazon Web Services
         resources through bring your own IP addresses (BYOIP) and creates a
         corresponding address
@@ -9288,15 +9288,15 @@
 
     def purchase_capacity_block(
         self,
         *,
         CapacityBlockOfferingId: str,
         InstancePlatform: CapacityReservationInstancePlatformType,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> PurchaseCapacityBlockResultTypeDef:
         """
         Purchase the Capacity Block for use with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_capacity_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#purchase_capacity_block)
         """
@@ -9305,15 +9305,15 @@
         self,
         *,
         HostIdSet: Sequence[str],
         OfferingId: str,
         ClientToken: str = ...,
         CurrencyCode: Literal["USD"] = ...,
         LimitPrice: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> PurchaseHostReservationResultTypeDef:
         """
         Purchase a reservation with configurations that match those of your Dedicated
         Host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_host_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#purchase_host_reservation)
@@ -9375,15 +9375,15 @@
         RootDeviceName: str = ...,
         SriovNetSupport: str = ...,
         VirtualizationType: str = ...,
         BootMode: BootModeValuesType = ...,
         TpmSupport: Literal["v2.0"] = ...,
         UefiData: str = ...,
         ImdsSupport: Literal["v2.0"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> RegisterImageResultTypeDef:
         """
         Registers an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.register_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#register_image)
         """
@@ -9652,15 +9652,15 @@
         Submits feedback about the status of an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.report_instance_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#report_instance_status)
         """
 
     def request_spot_fleet(
-        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataTypeDef, DryRun: bool = ...
+        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataUnionTypeDef, DryRun: bool = ...
     ) -> RequestSpotFleetResponseTypeDef:
         """
         Creates a Spot Fleet request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#request_spot_fleet)
         """
@@ -9675,15 +9675,15 @@
         InstanceCount: int = ...,
         LaunchGroup: str = ...,
         LaunchSpecification: RequestSpotLaunchSpecificationTypeDef = ...,
         SpotPrice: str = ...,
         Type: SpotInstanceTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         InstanceInterruptionBehavior: InstanceInterruptionBehaviorType = ...,
     ) -> RequestSpotInstancesResultTypeDef:
         """
         Creates a Spot Instance request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#request_spot_instances)
@@ -9840,15 +9840,15 @@
         """
 
     def revoke_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
@@ -9863,15 +9863,15 @@
     def revoke_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
     ) -> RevokeSecurityGroupIngressResultTypeDef:
@@ -9904,19 +9904,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -10025,15 +10025,15 @@
 
     def start_network_insights_access_scope_analysis(
         self,
         *,
         NetworkInsightsAccessScopeId: str,
         ClientToken: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> StartNetworkInsightsAccessScopeAnalysisResultTypeDef:
         """
         Starts analyzing the specified Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_access_scope_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#start_network_insights_access_scope_analysis)
         """
@@ -10042,15 +10042,15 @@
         self,
         *,
         NetworkInsightsPathId: str,
         ClientToken: str,
         AdditionalAccounts: Sequence[str] = ...,
         FilterInArns: Sequence[str] = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> StartNetworkInsightsAnalysisResultTypeDef:
         """
         Starts analyzing the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#start_network_insights_analysis)
         """
@@ -10178,15 +10178,15 @@
 
     def update_security_group_rule_descriptions_egress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...,
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
         Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#update_security_group_rule_descriptions_egress)
@@ -10194,15 +10194,15 @@
 
     def update_security_group_rule_descriptions_ingress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...,
     ) -> UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef:
         """
         Updates the description of an ingress (inbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#update_security_group_rule_descriptions_ingress)
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/client.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -751,27 +751,27 @@
     InstanceEventWindowAssociationRequestTypeDef,
     InstanceEventWindowDisassociationRequestTypeDef,
     InstanceEventWindowTimeRangeRequestTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
-    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationUnionTypeDef,
     InstanceRequirementsRequestTypeDef,
     InstanceRequirementsWithMetadataRequestTypeDef,
     InstanceSpecificationTypeDef,
     IntegrateServicesTypeDef,
     IpamCidrAuthorizationContextTypeDef,
     IpamPoolSourceResourceRequestTypeDef,
-    IpPermissionTypeDef,
+    IpPermissionUnionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     KeyPairTypeDef,
     LaunchPermissionModificationsTypeDef,
-    LaunchTemplateConfigTypeDef,
+    LaunchTemplateConfigUnionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LicenseConfigurationRequestTypeDef,
     ListImagesInRecycleBinResultTypeDef,
     ListSnapshotsInRecycleBinResultTypeDef,
     LoadPermissionModificationsTypeDef,
     LockSnapshotResultTypeDef,
     ModifyAddressAttributeResultTypeDef,
@@ -908,25 +908,25 @@
     SearchTransitGatewayRoutesResultTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     SecurityGroupRuleUpdateTypeDef,
     SlotDateTimeRangeRequestTypeDef,
     SlotStartTimeRangeRequestTypeDef,
     SnapshotDiskContainerTypeDef,
     SnapshotResponseTypeDef,
-    SpotFleetRequestConfigDataTypeDef,
+    SpotFleetRequestConfigDataUnionTypeDef,
     SpotOptionsRequestTypeDef,
     StartInstancesResultTypeDef,
     StartNetworkInsightsAccessScopeAnalysisResultTypeDef,
     StartNetworkInsightsAnalysisResultTypeDef,
     StartVpcEndpointServicePrivateDnsVerificationResultTypeDef,
     StopInstancesResultTypeDef,
     StorageLocationTypeDef,
-    StorageTypeDef,
+    StorageUnionTypeDef,
     SubnetConfigurationTypeDef,
-    TagSpecificationTypeDef,
+    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TargetCapacitySpecificationRequestTypeDef,
     TargetConfigurationRequestTypeDef,
     TerminateClientVpnConnectionsResultTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     TrafficMirrorPortRangeRequestTypeDef,
@@ -1019,15 +1019,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#exceptions)
         """
 
     def accept_address_transfer(
         self,
         *,
         Address: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> AcceptAddressTransferResultTypeDef:
         """
         Accepts an Elastic IP address transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.accept_address_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#accept_address_transfer)
@@ -1121,15 +1121,15 @@
         *,
         Domain: DomainTypeType = ...,
         Address: str = ...,
         PublicIpv4Pool: str = ...,
         NetworkBorderGroup: str = ...,
         CustomerOwnedIpv4Pool: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> AllocateAddressResultTypeDef:
         """
         Allocates an Elastic IP address to your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.allocate_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#allocate_address)
         """
@@ -1139,15 +1139,15 @@
         *,
         AvailabilityZone: str,
         AutoPlacement: AutoPlacementType = ...,
         ClientToken: str = ...,
         InstanceType: str = ...,
         InstanceFamily: str = ...,
         Quantity: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         HostRecovery: HostRecoveryType = ...,
         OutpostArn: str = ...,
         HostMaintenance: HostMaintenanceType = ...,
         AssetIds: Sequence[str] = ...,
     ) -> AllocateHostsResultTypeDef:
         """
         Allocates a Dedicated Host to your account.
@@ -1334,15 +1334,15 @@
 
     def associate_ipam_resource_discovery(
         self,
         *,
         IpamId: str,
         IpamResourceDiscoveryId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> AssociateIpamResourceDiscoveryResultTypeDef:
         """
         Associates an IPAM resource discovery with an Amazon VPC IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.associate_ipam_resource_discovery)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#associate_ipam_resource_discovery)
@@ -1575,16 +1575,16 @@
         """
 
     def authorize_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
@@ -1598,31 +1598,31 @@
     def authorize_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> AuthorizeSecurityGroupIngressResultTypeDef:
         """
         Adds the specified inbound (ingress) rules to a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#authorize_security_group_ingress)
         """
 
     def bundle_instance(
-        self, *, InstanceId: str, Storage: StorageTypeDef, DryRun: bool = ...
+        self, *, InstanceId: str, Storage: StorageUnionTypeDef, DryRun: bool = ...
     ) -> BundleInstanceResultTypeDef:
         """
         Bundles an Amazon instance store-backed Windows instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.bundle_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#bundle_instance)
         """
@@ -1782,15 +1782,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         DestinationOutpostArn: str = ...,
         DryRun: bool = ...,
         CopyImageTags: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CopyImageResultTypeDef:
         """
         Initiates the copy of an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#copy_image)
         """
@@ -1802,15 +1802,15 @@
         SourceSnapshotId: str,
         Description: str = ...,
         DestinationOutpostArn: str = ...,
         DestinationRegion: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         PresignedUrl: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a point-in-time snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#copy_snapshot)
@@ -1827,15 +1827,15 @@
         AvailabilityZoneId: str = ...,
         Tenancy: CapacityReservationTenancyType = ...,
         EbsOptimized: bool = ...,
         EphemeralStorage: bool = ...,
         EndDate: TimestampTypeDef = ...,
         EndDateType: EndDateTypeType = ...,
         InstanceMatchCriteria: InstanceMatchCriteriaType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         OutpostArn: str = ...,
         PlacementGroupArn: str = ...,
     ) -> CreateCapacityReservationResultTypeDef:
         """
         Creates a new Capacity Reservation with the specified attributes.
 
@@ -1849,29 +1849,29 @@
         InstanceTypeSpecifications: Sequence[ReservationFleetInstanceSpecificationTypeDef],
         TotalTargetCapacity: int,
         AllocationStrategy: str = ...,
         ClientToken: str = ...,
         Tenancy: Literal["default"] = ...,
         EndDate: TimestampTypeDef = ...,
         InstanceMatchCriteria: Literal["open"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateCapacityReservationFleetResultTypeDef:
         """
         Creates a Capacity Reservation Fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_capacity_reservation_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_capacity_reservation_fleet)
         """
 
     def create_carrier_gateway(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateCarrierGatewayResultTypeDef:
         """
         Creates a carrier gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_carrier_gateway)
@@ -1888,15 +1888,15 @@
         DnsServers: Sequence[str] = ...,
         TransportProtocol: TransportProtocolType = ...,
         VpnPort: int = ...,
         Description: str = ...,
         SplitTunnel: bool = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         VpcId: str = ...,
         SelfServicePortal: SelfServicePortalType = ...,
         ClientConnectOptions: ClientConnectOptionsTypeDef = ...,
         SessionTimeoutHours: int = ...,
         ClientLoginBannerOptions: ClientLoginBannerOptionsTypeDef = ...,
     ) -> CreateClientVpnEndpointResultTypeDef:
@@ -1934,15 +1934,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_coip_cidr)
         """
 
     def create_coip_pool(
         self,
         *,
         LocalGatewayRouteTableId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateCoipPoolResultTypeDef:
         """
         Creates a pool of customer-owned IP (CoIP) addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_coip_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_coip_pool)
@@ -1951,15 +1951,15 @@
     def create_customer_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         BgpAsn: int = ...,
         PublicIp: str = ...,
         CertificateArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DeviceName: str = ...,
         IpAddress: str = ...,
         DryRun: bool = ...,
     ) -> CreateCustomerGatewayResultTypeDef:
         """
         Provides information to Amazon Web Services about your customer gateway device.
 
@@ -1989,15 +1989,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_default_vpc)
         """
 
     def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateDhcpOptionsResultTypeDef:
         """
         Creates a custom set of DHCP options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_dhcp_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_dhcp_options)
@@ -2005,15 +2005,15 @@
 
     def create_egress_only_internet_gateway(
         self,
         *,
         VpcId: str,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateEgressOnlyInternetGatewayResultTypeDef:
         """
         [IPv6 only] Creates an egress-only internet gateway for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_egress_only_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_egress_only_internet_gateway)
         """
@@ -2029,15 +2029,15 @@
         OnDemandOptions: OnDemandOptionsRequestTypeDef = ...,
         ExcessCapacityTerminationPolicy: FleetExcessCapacityTerminationPolicyType = ...,
         TerminateInstancesWithExpiration: bool = ...,
         Type: FleetTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
         ReplaceUnhealthyInstances: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         Context: str = ...,
     ) -> CreateFleetResultTypeDef:
         """
         Creates an EC2 Fleet that contains the configuration information for On-Demand
         Instances and Spot
         Instances.
 
@@ -2055,15 +2055,15 @@
         DeliverLogsPermissionArn: str = ...,
         DeliverCrossAccountRole: str = ...,
         LogGroupName: str = ...,
         TrafficType: TrafficTypeType = ...,
         LogDestinationType: LogDestinationTypeType = ...,
         LogDestination: str = ...,
         LogFormat: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MaxAggregationInterval: int = ...,
         DestinationOptions: DestinationOptionsRequestTypeDef = ...,
     ) -> CreateFlowLogsResultTypeDef:
         """
         Creates one or more flow logs to capture information about IP traffic for a
         specific network interface, subnet, or
         VPC.
@@ -2077,15 +2077,15 @@
         *,
         InputStorageLocation: StorageLocationTypeDef,
         DryRun: bool = ...,
         LogsStorageLocation: StorageLocationTypeDef = ...,
         Description: str = ...,
         Name: str = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateFpgaImageResultTypeDef:
         """
         Creates an Amazon FPGA Image (AFI) from the specified design checkpoint (DCP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fpga_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_fpga_image)
         """
@@ -2095,15 +2095,15 @@
         *,
         InstanceId: str,
         Name: str,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         Description: str = ...,
         DryRun: bool = ...,
         NoReboot: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateImageResultTypeDef:
         """
         Creates an Amazon EBS-backed AMI from an Amazon EBS-backed instance that is
         either running or
         stopped.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_image)
@@ -2114,15 +2114,15 @@
         self,
         *,
         SubnetId: str,
         DryRun: bool = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreserveClientIp: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceConnectEndpointResultTypeDef:
         """
         Creates an EC2 Instance Connect Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_connect_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_instance_connect_endpoint)
         """
@@ -2130,15 +2130,15 @@
     def create_instance_event_window(
         self,
         *,
         DryRun: bool = ...,
         Name: str = ...,
         TimeRanges: Sequence[InstanceEventWindowTimeRangeRequestTypeDef] = ...,
         CronExpression: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceEventWindowResultTypeDef:
         """
         Creates an event window in which scheduled events for the associated Amazon EC2
         instances can
         run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_event_window)
@@ -2148,40 +2148,40 @@
     def create_instance_export_task(
         self,
         *,
         ExportToS3Task: ExportToS3TaskSpecificationTypeDef,
         InstanceId: str,
         TargetEnvironment: ExportEnvironmentType,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateInstanceExportTaskResultTypeDef:
         """
         Exports a running or stopped instance to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_export_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_instance_export_task)
         """
 
     def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
     ) -> CreateInternetGatewayResultTypeDef:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_internet_gateway)
         """
 
     def create_ipam(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tier: IpamTierType = ...,
     ) -> CreateIpamResultTypeDef:
         """
         Create an IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam)
@@ -2199,15 +2199,15 @@
         Description: str = ...,
         AutoImport: bool = ...,
         PubliclyAdvertisable: bool = ...,
         AllocationMinNetmaskLength: int = ...,
         AllocationMaxNetmaskLength: int = ...,
         AllocationDefaultNetmaskLength: int = ...,
         AllocationResourceTags: Sequence[RequestIpamResourceTagTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         AwsService: Literal["ec2"] = ...,
         PublicIpSource: IpamPoolPublicIpSourceType = ...,
         SourceResource: IpamPoolSourceResourceRequestTypeDef = ...,
     ) -> CreateIpamPoolResultTypeDef:
         """
         Create an IP address pool for Amazon VPC IP Address Manager (IPAM).
@@ -2218,15 +2218,15 @@
 
     def create_ipam_resource_discovery(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateIpamResourceDiscoveryResultTypeDef:
         """
         Creates an IPAM resource discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_resource_discovery)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_ipam_resource_discovery)
@@ -2234,15 +2234,15 @@
 
     def create_ipam_scope(
         self,
         *,
         IpamId: str,
         DryRun: bool = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateIpamScopeResultTypeDef:
         """
         Create an IPAM scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_ipam_scope)
@@ -2250,15 +2250,15 @@
 
     def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         KeyFormat: KeyFormatType = ...,
     ) -> KeyPairTypeDef:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK
         format.
 
@@ -2270,15 +2270,15 @@
         self,
         *,
         LaunchTemplateName: str,
         LaunchTemplateData: RequestLaunchTemplateDataTypeDef,
         DryRun: bool = ...,
         ClientToken: str = ...,
         VersionDescription: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateLaunchTemplateResultTypeDef:
         """
         Creates a launch template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_launch_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_launch_template)
         """
@@ -2320,45 +2320,45 @@
         """
 
     def create_local_gateway_route_table(
         self,
         *,
         LocalGatewayId: str,
         Mode: LocalGatewayRouteTableModeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableResultTypeDef:
         """
         Creates a local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table)
         """
 
     def create_local_gateway_route_table_virtual_interface_group_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         LocalGatewayVirtualInterfaceGroupId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationResultTypeDef:
         """
         Creates a local gateway route table virtual interface group association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_virtual_interface_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table_virtual_interface_group_association)
         """
 
     def create_local_gateway_route_table_vpc_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateLocalGatewayRouteTableVpcAssociationResultTypeDef:
         """
         Associates the specified VPC with the specified local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_local_gateway_route_table_vpc_association)
@@ -2368,15 +2368,15 @@
         self,
         *,
         PrefixListName: str,
         MaxEntries: int,
         AddressFamily: str,
         DryRun: bool = ...,
         Entries: Sequence[AddPrefixListEntryTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateManagedPrefixListResultTypeDef:
         """
         Creates a managed prefix list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_managed_prefix_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_managed_prefix_list)
@@ -2385,15 +2385,15 @@
     def create_nat_gateway(
         self,
         *,
         SubnetId: str,
         AllocationId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ConnectivityType: ConnectivityTypeType = ...,
         PrivateIpAddress: str = ...,
         SecondaryAllocationIds: Sequence[str] = ...,
         SecondaryPrivateIpAddresses: Sequence[str] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
     ) -> CreateNatGatewayResultTypeDef:
         """
@@ -2404,15 +2404,15 @@
         """
 
     def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateNetworkAclResultTypeDef:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_network_acl)
@@ -2441,15 +2441,15 @@
 
     def create_network_insights_access_scope(
         self,
         *,
         ClientToken: str,
         MatchPaths: Sequence[AccessScopePathRequestTypeDef] = ...,
         ExcludePaths: Sequence[AccessScopePathRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateNetworkInsightsAccessScopeResultTypeDef:
         """
         Creates a Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_insights_access_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_network_insights_access_scope)
@@ -2461,15 +2461,15 @@
         Source: str,
         Protocol: ProtocolType,
         ClientToken: str,
         SourceIp: str = ...,
         DestinationIp: str = ...,
         Destination: str = ...,
         DestinationPort: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         FilterAtSource: PathRequestFilterTypeDef = ...,
         FilterAtDestination: PathRequestFilterTypeDef = ...,
     ) -> CreateNetworkInsightsPathResultTypeDef:
         """
         Creates a path to analyze for reachability.
 
@@ -2490,15 +2490,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         EnablePrimaryIpv6: bool = ...,
         ConnectionTrackingSpecification: ConnectionTrackingSpecificationRequestTypeDef = ...,
     ) -> CreateNetworkInterfaceResultTypeDef:
         """
         Creates a network interface in the specified subnet.
 
@@ -2527,26 +2527,26 @@
     def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...,
     ) -> CreatePlacementGroupResultTypeDef:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_placement_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_placement_group)
         """
 
     def create_public_ipv4_pool(
-        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
+        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
     ) -> CreatePublicIpv4PoolResultTypeDef:
         """
         Creates a public IPv4 address pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_public_ipv4_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_public_ipv4_pool)
         """
@@ -2554,15 +2554,15 @@
     def create_replace_root_volume_task(
         self,
         *,
         InstanceId: str,
         SnapshotId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ImageId: str = ...,
         DeleteReplacedRootVolume: bool = ...,
     ) -> CreateReplaceRootVolumeTaskResultTypeDef:
         """
         Replaces the EBS-backed root volume for a `running` instance with a new volume
         that is restored to the original root volume's launch state, that is restored
         to a specific snapshot taken from the original root volume, or that is restored
@@ -2592,15 +2592,15 @@
 
     def create_restore_image_task(
         self,
         *,
         Bucket: str,
         ObjectKey: str,
         Name: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateRestoreImageTaskResultTypeDef:
         """
         Starts a task that restores an AMI from an Amazon S3 object that was previously
         created by using
         [CreateStoreImageTask](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateStoreImageTask.html).
 
@@ -2636,15 +2636,15 @@
         """
 
     def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> CreateRouteTableResultTypeDef:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_route_table)
@@ -2652,15 +2652,15 @@
 
     def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateSecurityGroupResultTypeDef:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_security_group)
@@ -2668,15 +2668,15 @@
 
     def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> SnapshotResponseTypeDef:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_snapshot)
@@ -2684,15 +2684,15 @@
 
     def create_snapshots(
         self,
         *,
         InstanceSpecification: InstanceSpecificationTypeDef,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         CopyTagsFromSource: Literal["volume"] = ...,
     ) -> CreateSnapshotsResultTypeDef:
         """
         Creates crash-consistent snapshots of multiple EBS volumes and stores the data
         in
         S3.
@@ -2728,15 +2728,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_store_image_task)
         """
 
     def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...,
@@ -2756,15 +2756,15 @@
         self,
         *,
         SubnetId: str,
         Cidr: str,
         ReservationType: SubnetCidrReservationTypeType,
         Description: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateSubnetCidrReservationResultTypeDef:
         """
         Creates a subnet CIDR reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_subnet_cidr_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_subnet_cidr_reservation)
         """
@@ -2781,15 +2781,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_tags)
         """
 
     def create_traffic_mirror_filter(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateTrafficMirrorFilterResultTypeDef:
         """
         Creates a Traffic Mirror filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_filter)
@@ -2825,15 +2825,15 @@
         NetworkInterfaceId: str,
         TrafficMirrorTargetId: str,
         TrafficMirrorFilterId: str,
         SessionNumber: int,
         PacketLength: int = ...,
         VirtualNetworkId: int = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
     ) -> CreateTrafficMirrorSessionResultTypeDef:
         """
         Creates a Traffic Mirror session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_session)
@@ -2842,15 +2842,15 @@
 
     def create_traffic_mirror_target(
         self,
         *,
         NetworkInterfaceId: str = ...,
         NetworkLoadBalancerArn: str = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
         GatewayLoadBalancerEndpointId: str = ...,
     ) -> CreateTrafficMirrorTargetResultTypeDef:
         """
         Creates a target for your Traffic Mirror session.
 
@@ -2859,30 +2859,30 @@
         """
 
     def create_transit_gateway(
         self,
         *,
         Description: str = ...,
         Options: TransitGatewayRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayResultTypeDef:
         """
         Creates a transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway)
         """
 
     def create_transit_gateway_connect(
         self,
         *,
         TransportTransitGatewayAttachmentId: str,
         Options: CreateTransitGatewayConnectRequestOptionsTypeDef,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayConnectResultTypeDef:
         """
         Creates a Connect attachment from a specified transit gateway attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_connect)
@@ -2892,15 +2892,15 @@
         self,
         *,
         TransitGatewayAttachmentId: str,
         PeerAddress: str,
         InsideCidrBlocks: Sequence[str],
         TransitGatewayAddress: str = ...,
         BgpOptions: TransitGatewayConnectRequestBgpOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayConnectPeerResultTypeDef:
         """
         Creates a Connect peer for a specified transit gateway Connect attachment
         between a transit gateway and an
         appliance.
 
@@ -2909,15 +2909,15 @@
         """
 
     def create_transit_gateway_multicast_domain(
         self,
         *,
         TransitGatewayId: str,
         Options: CreateTransitGatewayMulticastDomainRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayMulticastDomainResultTypeDef:
         """
         Creates a multicast domain using the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_multicast_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_multicast_domain)
@@ -2927,15 +2927,15 @@
         self,
         *,
         TransitGatewayId: str,
         PeerTransitGatewayId: str,
         PeerAccountId: str,
         PeerRegion: str,
         Options: CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayPeeringAttachmentResultTypeDef:
         """
         Requests a transit gateway peering attachment between the specified transit
         gateway (requester) and a peer transit gateway
         (accepter).
 
@@ -2943,15 +2943,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_peering_attachment)
         """
 
     def create_transit_gateway_policy_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayPolicyTableResultTypeDef:
         """
         Creates a transit gateway policy table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_policy_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_policy_table)
@@ -2991,30 +2991,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route)
         """
 
     def create_transit_gateway_route_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayRouteTableResultTypeDef:
         """
         Creates a route table for the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route_table)
         """
 
     def create_transit_gateway_route_table_announcement(
         self,
         *,
         TransitGatewayRouteTableId: str,
         PeeringAttachmentId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayRouteTableAnnouncementResultTypeDef:
         """
         Advertises a new transit gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table_announcement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_route_table_announcement)
@@ -3023,15 +3023,15 @@
     def create_transit_gateway_vpc_attachment(
         self,
         *,
         TransitGatewayId: str,
         VpcId: str,
         SubnetIds: Sequence[str],
         Options: CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> CreateTransitGatewayVpcAttachmentResultTypeDef:
         """
         Attaches the specified VPC to the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_vpc_attachment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_transit_gateway_vpc_attachment)
@@ -3047,15 +3047,15 @@
         ApplicationDomain: str,
         EndpointDomainPrefix: str,
         SecurityGroupIds: Sequence[str] = ...,
         LoadBalancerOptions: CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef = ...,
         NetworkInterfaceOptions: CreateVerifiedAccessEndpointEniOptionsTypeDef = ...,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessEndpointResultTypeDef:
         """
         An Amazon Web Services Verified Access endpoint is where you define your
         application along with an optional endpoint-level access
@@ -3067,15 +3067,15 @@
 
     def create_verified_access_group(
         self,
         *,
         VerifiedAccessInstanceId: str,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessGroupResultTypeDef:
         """
         An Amazon Web Services Verified Access group is a collection of Amazon Web
         Services Verified Access endpoints who's associated applications have similar
@@ -3086,15 +3086,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_verified_access_group)
         """
 
     def create_verified_access_instance(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         FIPSEnabled: bool = ...,
     ) -> CreateVerifiedAccessInstanceResultTypeDef:
         """
         An Amazon Web Services Verified Access instance is a regional entity that
         evaluates application requests and grants access only when your security
@@ -3111,15 +3111,15 @@
         TrustProviderType: TrustProviderTypeType,
         PolicyReferenceName: str,
         UserTrustProviderType: UserTrustProviderTypeType = ...,
         DeviceTrustProviderType: DeviceTrustProviderTypeType = ...,
         OidcOptions: CreateVerifiedAccessTrustProviderOidcOptionsTypeDef = ...,
         DeviceOptions: CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
         SseSpecification: VerifiedAccessSseSpecificationRequestTypeDef = ...,
     ) -> CreateVerifiedAccessTrustProviderResultTypeDef:
         """
         A trust provider is a third-party entity that creates, maintains, and manages
         identity information for users and
@@ -3137,15 +3137,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...,
     ) -> VolumeResponseTypeDef:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability
@@ -3165,15 +3165,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcResultTypeDef:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_vpc)
         """
@@ -3189,15 +3189,15 @@
         RouteTableIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SubnetConfigurations: Sequence[SubnetConfigurationTypeDef] = ...,
     ) -> CreateVpcEndpointResultTypeDef:
         """
         Creates a VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#create_vpc_endpoint)
@@ -3227,15 +3227,15 @@
         DryRun: bool = ...,
         AcceptanceRequired: bool = ...,
         PrivateDnsName: str = ...,
         NetworkLoadBalancerArns: Sequence[str] = ...,
         GatewayLoadBalancerArns: Sequence[str] = ...,
         SupportedIpAddressTypes: Sequence[str] = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcEndpointServiceConfigurationResultTypeDef:
         """
         Creates a VPC endpoint service to which service consumers (Amazon Web Services
         accounts, users, and IAM roles) can
         connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint_service_configuration)
@@ -3246,15 +3246,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpcPeeringConnectionResultTypeDef:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you
         own and an accepter VPC with which to create the
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_peering_connection)
@@ -3266,15 +3266,15 @@
         *,
         CustomerGatewayId: str,
         Type: str,
         VpnGatewayId: str = ...,
         TransitGatewayId: str = ...,
         DryRun: bool = ...,
         Options: VpnConnectionOptionsSpecificationTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> CreateVpnConnectionResultTypeDef:
         """
         Creates a VPN connection between an existing virtual private gateway or transit
         gateway and a customer
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_connection)
@@ -3294,15 +3294,15 @@
         """
 
     def create_vpn_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         AvailabilityZone: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AmazonSideAsn: int = ...,
         DryRun: bool = ...,
     ) -> CreateVpnGatewayResultTypeDef:
         """
         Creates a virtual private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_gateway)
@@ -7205,15 +7205,15 @@
         DiskImageFormat: DiskImageFormatType,
         ImageId: str,
         S3ExportLocation: ExportTaskS3LocationRequestTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ExportImageResultTypeDef:
         """
         Exports an Amazon Machine Image (AMI) to a VM file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.export_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#export_image)
         """
@@ -7965,15 +7965,15 @@
         Encrypted: bool = ...,
         Hypervisor: str = ...,
         KmsKeyId: str = ...,
         LicenseType: str = ...,
         Platform: str = ...,
         RoleName: str = ...,
         LicenseSpecifications: Sequence[ImportImageLicenseConfigurationRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         UsageOperation: str = ...,
         BootMode: BootModeValuesType = ...,
     ) -> ImportImageResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_image)
@@ -7998,15 +7998,15 @@
 
     def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ImportKeyPairResultTypeDef:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_key_pair)
@@ -8020,15 +8020,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         DiskContainer: SnapshotDiskContainerTypeDef = ...,
         DryRun: bool = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> ImportSnapshotResultTypeDef:
         """
         Imports a disk into an EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#import_snapshot)
         """
@@ -8699,15 +8699,15 @@
         """
 
     def modify_spot_fleet_request(
         self,
         *,
         SpotFleetRequestId: str,
         ExcessCapacityTerminationPolicy: ExcessCapacityTerminationPolicyType = ...,
-        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigTypeDef] = ...,
+        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigUnionTypeDef] = ...,
         TargetCapacity: int = ...,
         OnDemandTargetCapacity: int = ...,
         Context: str = ...,
     ) -> ModifySpotFleetRequestResponseTypeDef:
         """
         Modifies the specified Spot Fleet request.
 
@@ -9221,15 +9221,15 @@
         self,
         *,
         Cidr: str,
         CidrAuthorizationContext: CidrAuthorizationContextTypeDef = ...,
         PubliclyAdvertisable: bool = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        PoolTagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        PoolTagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiRegion: bool = ...,
         NetworkBorderGroup: str = ...,
     ) -> ProvisionByoipCidrResultTypeDef:
         """
         Provisions an IPv4 or IPv6 address range for use with your Amazon Web Services
         resources through bring your own IP addresses (BYOIP) and creates a
         corresponding address
@@ -9285,15 +9285,15 @@
 
     def purchase_capacity_block(
         self,
         *,
         CapacityBlockOfferingId: str,
         InstancePlatform: CapacityReservationInstancePlatformType,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> PurchaseCapacityBlockResultTypeDef:
         """
         Purchase the Capacity Block for use with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_capacity_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#purchase_capacity_block)
         """
@@ -9302,15 +9302,15 @@
         self,
         *,
         HostIdSet: Sequence[str],
         OfferingId: str,
         ClientToken: str = ...,
         CurrencyCode: Literal["USD"] = ...,
         LimitPrice: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> PurchaseHostReservationResultTypeDef:
         """
         Purchase a reservation with configurations that match those of your Dedicated
         Host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_host_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#purchase_host_reservation)
@@ -9372,15 +9372,15 @@
         RootDeviceName: str = ...,
         SriovNetSupport: str = ...,
         VirtualizationType: str = ...,
         BootMode: BootModeValuesType = ...,
         TpmSupport: Literal["v2.0"] = ...,
         UefiData: str = ...,
         ImdsSupport: Literal["v2.0"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> RegisterImageResultTypeDef:
         """
         Registers an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.register_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#register_image)
         """
@@ -9649,15 +9649,15 @@
         Submits feedback about the status of an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.report_instance_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#report_instance_status)
         """
 
     def request_spot_fleet(
-        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataTypeDef, DryRun: bool = ...
+        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataUnionTypeDef, DryRun: bool = ...
     ) -> RequestSpotFleetResponseTypeDef:
         """
         Creates a Spot Fleet request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#request_spot_fleet)
         """
@@ -9672,15 +9672,15 @@
         InstanceCount: int = ...,
         LaunchGroup: str = ...,
         LaunchSpecification: RequestSpotLaunchSpecificationTypeDef = ...,
         SpotPrice: str = ...,
         Type: SpotInstanceTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         InstanceInterruptionBehavior: InstanceInterruptionBehaviorType = ...,
     ) -> RequestSpotInstancesResultTypeDef:
         """
         Creates a Spot Instance request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#request_spot_instances)
@@ -9837,15 +9837,15 @@
         """
 
     def revoke_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
@@ -9860,15 +9860,15 @@
     def revoke_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
     ) -> RevokeSecurityGroupIngressResultTypeDef:
@@ -9901,19 +9901,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -10022,15 +10022,15 @@
 
     def start_network_insights_access_scope_analysis(
         self,
         *,
         NetworkInsightsAccessScopeId: str,
         ClientToken: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> StartNetworkInsightsAccessScopeAnalysisResultTypeDef:
         """
         Starts analyzing the specified Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_access_scope_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#start_network_insights_access_scope_analysis)
         """
@@ -10039,15 +10039,15 @@
         self,
         *,
         NetworkInsightsPathId: str,
         ClientToken: str,
         AdditionalAccounts: Sequence[str] = ...,
         FilterInArns: Sequence[str] = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> StartNetworkInsightsAnalysisResultTypeDef:
         """
         Starts analyzing the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#start_network_insights_analysis)
         """
@@ -10175,15 +10175,15 @@
 
     def update_security_group_rule_descriptions_egress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...,
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
         Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#update_security_group_rule_descriptions_egress)
@@ -10191,15 +10191,15 @@
 
     def update_security_group_rule_descriptions_ingress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...,
     ) -> UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef:
         """
         Updates the description of an ingress (inbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#update_security_group_rule_descriptions_ingress)
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/literals.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,15 @@
     "ResourceTypeType",
     "RootDeviceTypeType",
     "RouteOriginType",
     "RouteStateType",
     "RouteTableAssociationStateCodeType",
     "RuleActionType",
     "SSETypeType",
+    "ScopeType",
     "SearchLocalGatewayRoutesPaginatorName",
     "SearchTransitGatewayMulticastGroupsPaginatorName",
     "SecurityGroupExistsWaiterName",
     "SecurityGroupReferencingSupportValueType",
     "SelfServicePortalType",
     "ServiceConnectivityTypeType",
     "ServiceStateType",
@@ -521,15 +522,14 @@
     "VpnConnectionAvailableWaiterName",
     "VpnConnectionDeletedWaiterName",
     "VpnEcmpSupportValueType",
     "VpnProtocolType",
     "VpnStateType",
     "VpnStaticRouteSourceType",
     "WeekDayType",
-    "scopeType",
     "EC2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
@@ -2212,14 +2212,15 @@
 RouteOriginType = Literal["CreateRoute", "CreateRouteTable", "EnableVgwRoutePropagation"]
 RouteStateType = Literal["active", "blackhole"]
 RouteTableAssociationStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed"
 ]
 RuleActionType = Literal["allow", "deny"]
 SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
+ScopeType = Literal["Availability Zone", "Region"]
 SearchLocalGatewayRoutesPaginatorName = Literal["search_local_gateway_routes"]
 SearchTransitGatewayMulticastGroupsPaginatorName = Literal[
     "search_transit_gateway_multicast_groups"
 ]
 SecurityGroupExistsWaiterName = Literal["security_group_exists"]
 SecurityGroupReferencingSupportValueType = Literal["disable", "enable"]
 SelfServicePortalType = Literal["disabled", "enabled"]
@@ -2399,15 +2400,14 @@
 VpnConnectionAvailableWaiterName = Literal["vpn_connection_available"]
 VpnConnectionDeletedWaiterName = Literal["vpn_connection_deleted"]
 VpnEcmpSupportValueType = Literal["disable", "enable"]
 VpnProtocolType = Literal["openvpn"]
 VpnStateType = Literal["available", "deleted", "deleting", "pending"]
 VpnStaticRouteSourceType = Literal["Static"]
 WeekDayType = Literal["friday", "monday", "saturday", "sunday", "thursday", "tuesday", "wednesday"]
-scopeType = Literal["Availability Zone", "Region"]
 EC2ServiceName = Literal["ec2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/literals.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,15 @@
     "ResourceTypeType",
     "RootDeviceTypeType",
     "RouteOriginType",
     "RouteStateType",
     "RouteTableAssociationStateCodeType",
     "RuleActionType",
     "SSETypeType",
+    "ScopeType",
     "SearchLocalGatewayRoutesPaginatorName",
     "SearchTransitGatewayMulticastGroupsPaginatorName",
     "SecurityGroupExistsWaiterName",
     "SecurityGroupReferencingSupportValueType",
     "SelfServicePortalType",
     "ServiceConnectivityTypeType",
     "ServiceStateType",
@@ -521,15 +522,14 @@
     "VpnConnectionAvailableWaiterName",
     "VpnConnectionDeletedWaiterName",
     "VpnEcmpSupportValueType",
     "VpnProtocolType",
     "VpnStateType",
     "VpnStaticRouteSourceType",
     "WeekDayType",
-    "scopeType",
     "EC2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
@@ -2212,14 +2212,15 @@
 RouteOriginType = Literal["CreateRoute", "CreateRouteTable", "EnableVgwRoutePropagation"]
 RouteStateType = Literal["active", "blackhole"]
 RouteTableAssociationStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed"
 ]
 RuleActionType = Literal["allow", "deny"]
 SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
+ScopeType = Literal["Availability Zone", "Region"]
 SearchLocalGatewayRoutesPaginatorName = Literal["search_local_gateway_routes"]
 SearchTransitGatewayMulticastGroupsPaginatorName = Literal[
     "search_transit_gateway_multicast_groups"
 ]
 SecurityGroupExistsWaiterName = Literal["security_group_exists"]
 SecurityGroupReferencingSupportValueType = Literal["disable", "enable"]
 SelfServicePortalType = Literal["disabled", "enabled"]
@@ -2399,15 +2400,14 @@
 VpnConnectionAvailableWaiterName = Literal["vpn_connection_available"]
 VpnConnectionDeletedWaiterName = Literal["vpn_connection_deleted"]
 VpnEcmpSupportValueType = Literal["disable", "enable"]
 VpnProtocolType = Literal["openvpn"]
 VpnStateType = Literal["available", "deleted", "deleting", "pending"]
 VpnStaticRouteSourceType = Literal["Static"]
 WeekDayType = Literal["friday", "monday", "saturday", "sunday", "thursday", "tuesday", "wednesday"]
-scopeType = Literal["Availability Zone", "Region"]
 EC2ServiceName = Literal["ec2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/paginator.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,19 +391,19 @@
     DescribeReplaceRootVolumeTasksResultTypeDef,
     DescribeReservedInstancesModificationsResultTypeDef,
     DescribeReservedInstancesOfferingsResultTypeDef,
     DescribeRouteTablesResultTypeDef,
     DescribeScheduledInstanceAvailabilityResultTypeDef,
     DescribeScheduledInstancesResultTypeDef,
     DescribeSecurityGroupRulesResultTypeDef,
-    DescribeSecurityGroupsResultPaginatorTypeDef,
+    DescribeSecurityGroupsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeSnapshotTierStatusResultTypeDef,
     DescribeSpotFleetInstancesResponseTypeDef,
-    DescribeSpotFleetRequestsResponsePaginatorTypeDef,
+    DescribeSpotFleetRequestsResponseTypeDef,
     DescribeSpotInstanceRequestsResultTypeDef,
     DescribeSpotPriceHistoryResultTypeDef,
     DescribeStaleSecurityGroupsResultTypeDef,
     DescribeStoreImageTasksResultTypeDef,
     DescribeSubnetsResultTypeDef,
     DescribeTagsResultTypeDef,
     DescribeTrafficMirrorFiltersResultTypeDef,
@@ -2148,15 +2148,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         GroupIds: Sequence[str] = ...,
         GroupNames: Sequence[str] = ...,
         DryRun: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeSecurityGroupsResultPaginatorTypeDef]:
+    ) -> _PageIterator[DescribeSecurityGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/paginators/#describesecuritygroupspaginator)
         """
 
 
 class DescribeSnapshotTierStatusPaginator(Paginator):
@@ -2227,15 +2227,15 @@
 
     def paginate(
         self,
         *,
         DryRun: bool = ...,
         SpotFleetRequestIds: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeSpotFleetRequestsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeSpotFleetRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/paginators/#describespotfleetrequestspaginator)
         """
 
 
 class DescribeSpotInstanceRequestsPaginator(Paginator):
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/paginator.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -391,19 +391,19 @@
     DescribeReplaceRootVolumeTasksResultTypeDef,
     DescribeReservedInstancesModificationsResultTypeDef,
     DescribeReservedInstancesOfferingsResultTypeDef,
     DescribeRouteTablesResultTypeDef,
     DescribeScheduledInstanceAvailabilityResultTypeDef,
     DescribeScheduledInstancesResultTypeDef,
     DescribeSecurityGroupRulesResultTypeDef,
-    DescribeSecurityGroupsResultPaginatorTypeDef,
+    DescribeSecurityGroupsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeSnapshotTierStatusResultTypeDef,
     DescribeSpotFleetInstancesResponseTypeDef,
-    DescribeSpotFleetRequestsResponsePaginatorTypeDef,
+    DescribeSpotFleetRequestsResponseTypeDef,
     DescribeSpotInstanceRequestsResultTypeDef,
     DescribeSpotPriceHistoryResultTypeDef,
     DescribeStaleSecurityGroupsResultTypeDef,
     DescribeStoreImageTasksResultTypeDef,
     DescribeSubnetsResultTypeDef,
     DescribeTagsResultTypeDef,
     DescribeTrafficMirrorFiltersResultTypeDef,
@@ -2072,15 +2072,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         GroupIds: Sequence[str] = ...,
         GroupNames: Sequence[str] = ...,
         DryRun: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeSecurityGroupsResultPaginatorTypeDef]:
+    ) -> _PageIterator[DescribeSecurityGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/paginators/#describesecuritygroupspaginator)
         """
 
 class DescribeSnapshotTierStatusPaginator(Paginator):
     """
@@ -2147,15 +2147,15 @@
 
     def paginate(
         self,
         *,
         DryRun: bool = ...,
         SpotFleetRequestIds: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeSpotFleetRequestsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeSpotFleetRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/paginators/#describespotfleetrequestspaginator)
         """
 
 class DescribeSpotInstanceRequestsPaginator(Paginator):
     """
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/service_resource.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,19 +145,20 @@
     InstanceBlockDeviceMappingTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMaintenanceOptionsResponseTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
     InstanceMetadataOptionsResponseResponseTypeDef,
-    InstanceNetworkInterfaceSpecificationServiceResourceTypeDef,
-    InstanceNetworkInterfaceSpecificationSubnetTypeDef,
+    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationUnionTypeDef,
     InstanceNetworkInterfaceTypeDef,
     InstanceStateResponseTypeDef,
     InternetGatewayAttachmentTypeDef,
+    IpPermissionExtraExtraOutputTypeDef,
     IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv4PrefixSpecificationTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationTypeDef,
     LaunchPermissionModificationsTypeDef,
     LaunchTemplateSpecificationTypeDef,
@@ -191,14 +192,15 @@
     RouteTypeDef,
     RunInstancesMonitoringEnabledTypeDef,
     StartInstancesResultTypeDef,
     StateReasonResponseTypeDef,
     StopInstancesResultTypeDef,
     SubnetIpv6CidrBlockAssociationTypeDef,
     TagSpecificationTypeDef,
+    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     UnmonitorInstancesResultTypeDef,
     VolumeAttachmentResponseTypeDef,
     VolumeAttachmentTypeDef,
     VpcCidrBlockAssociationTypeDef,
@@ -3189,18 +3191,18 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.SecurityGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#securitygroup)
     """
 
     description: str
     group_name: str
-    ip_permissions: List[IpPermissionTypeDef]
+    ip_permissions: List[IpPermissionExtraExtraOutputTypeDef]
     owner_id: str
     group_id: str
-    ip_permissions_egress: List[IpPermissionTypeDef]
+    ip_permissions_egress: List[IpPermissionExtraExtraOutputTypeDef]
     tags: List[TagTypeDef]
     vpc_id: str
     id: str
     meta: "EC2ResourceMeta"
 
     def authorize_egress(
         self,
@@ -4647,15 +4649,15 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
@@ -5280,15 +5282,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcevpcpeeringconnection-method)
         """
 
     def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_DhcpOptions":
         """
         Creates a custom set of DHCP options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_dhcp_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_dhcp_options-method)
@@ -5316,21 +5318,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[
-            InstanceNetworkInterfaceSpecificationServiceResourceTypeDef
-        ] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -5346,30 +5346,30 @@
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_instances-method)
         """
 
     def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
     ) -> "_InternetGateway":
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_internet_gateway-method)
         """
 
     def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         KeyFormat: KeyFormatType = ...,
     ) -> "_KeyPair":
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK
         format.
 
@@ -5378,15 +5378,15 @@
         """
 
     def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> "_NetworkAcl":
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_network_acl-method)
@@ -5405,15 +5405,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         EnablePrimaryIpv6: bool = ...,
         ConnectionTrackingSpecification: ConnectionTrackingSpecificationRequestTypeDef = ...,
     ) -> "_NetworkInterface":
         """
         Creates a network interface in the specified subnet.
 
@@ -5424,30 +5424,30 @@
     def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...,
     ) -> "_PlacementGroup":
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_placement_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_placement_group-method)
         """
 
     def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> "_RouteTable":
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_route_table-method)
@@ -5455,15 +5455,15 @@
 
     def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_SecurityGroup":
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_security_group-method)
@@ -5471,29 +5471,29 @@
 
     def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_Snapshot":
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_snapshot-method)
         """
 
     def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...,
@@ -5525,15 +5525,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...,
     ) -> "_Volume":
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability
@@ -5553,15 +5553,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_Vpc":
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_vpc-method)
         """
@@ -5570,15 +5570,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_VpcPeeringConnection":
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you
         own and an accepter VPC with which to create the
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc_peering_connection)
@@ -5603,15 +5603,15 @@
 
     def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_KeyPairInfo":
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.import_key_pair)
@@ -5634,15 +5634,15 @@
         RootDeviceName: str = ...,
         SriovNetSupport: str = ...,
         VirtualizationType: str = ...,
         BootMode: BootModeValuesType = ...,
         TpmSupport: Literal["v2.0"] = ...,
         UefiData: str = ...,
         ImdsSupport: Literal["v2.0"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_Image":
         """
         Registers an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.register_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourceregister_image-method)
         """
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/service_resource.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -145,19 +145,20 @@
     InstanceBlockDeviceMappingTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMaintenanceOptionsResponseTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
     InstanceMetadataOptionsResponseResponseTypeDef,
-    InstanceNetworkInterfaceSpecificationServiceResourceTypeDef,
-    InstanceNetworkInterfaceSpecificationSubnetTypeDef,
+    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationUnionTypeDef,
     InstanceNetworkInterfaceTypeDef,
     InstanceStateResponseTypeDef,
     InternetGatewayAttachmentTypeDef,
+    IpPermissionExtraExtraOutputTypeDef,
     IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv4PrefixSpecificationTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationTypeDef,
     LaunchPermissionModificationsTypeDef,
     LaunchTemplateSpecificationTypeDef,
@@ -191,14 +192,15 @@
     RouteTypeDef,
     RunInstancesMonitoringEnabledTypeDef,
     StartInstancesResultTypeDef,
     StateReasonResponseTypeDef,
     StopInstancesResultTypeDef,
     SubnetIpv6CidrBlockAssociationTypeDef,
     TagSpecificationTypeDef,
+    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     UnmonitorInstancesResultTypeDef,
     VolumeAttachmentResponseTypeDef,
     VolumeAttachmentTypeDef,
     VpcCidrBlockAssociationTypeDef,
@@ -3136,18 +3138,18 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.SecurityGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#securitygroup)
     """
 
     description: str
     group_name: str
-    ip_permissions: List[IpPermissionTypeDef]
+    ip_permissions: List[IpPermissionExtraExtraOutputTypeDef]
     owner_id: str
     group_id: str
-    ip_permissions_egress: List[IpPermissionTypeDef]
+    ip_permissions_egress: List[IpPermissionExtraExtraOutputTypeDef]
     tags: List[TagTypeDef]
     vpc_id: str
     id: str
     meta: "EC2ResourceMeta"
 
     def authorize_egress(
         self,
@@ -4574,15 +4576,15 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
@@ -5202,15 +5204,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcevpcpeeringconnection-method)
         """
 
     def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_DhcpOptions":
         """
         Creates a custom set of DHCP options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_dhcp_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_dhcp_options-method)
@@ -5238,21 +5240,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[
-            InstanceNetworkInterfaceSpecificationServiceResourceTypeDef
-        ] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -5268,30 +5268,30 @@
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_instances-method)
         """
 
     def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
     ) -> "_InternetGateway":
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_internet_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_internet_gateway-method)
         """
 
     def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         KeyFormat: KeyFormatType = ...,
     ) -> "_KeyPair":
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK
         format.
 
@@ -5300,15 +5300,15 @@
         """
 
     def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> "_NetworkAcl":
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_network_acl-method)
@@ -5327,15 +5327,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
         EnablePrimaryIpv6: bool = ...,
         ConnectionTrackingSpecification: ConnectionTrackingSpecificationRequestTypeDef = ...,
     ) -> "_NetworkInterface":
         """
         Creates a network interface in the specified subnet.
 
@@ -5346,30 +5346,30 @@
     def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...,
     ) -> "_PlacementGroup":
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_placement_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_placement_group-method)
         """
 
     def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         ClientToken: str = ...,
     ) -> "_RouteTable":
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_route_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_route_table-method)
@@ -5377,15 +5377,15 @@
 
     def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_SecurityGroup":
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_security_group-method)
@@ -5393,29 +5393,29 @@
 
     def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         DryRun: bool = ...,
     ) -> "_Snapshot":
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_snapshot-method)
         """
 
     def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...,
@@ -5447,15 +5447,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...,
     ) -> "_Volume":
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability
@@ -5475,15 +5475,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_Vpc":
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourcecreate_vpc-method)
         """
@@ -5492,15 +5492,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_VpcPeeringConnection":
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you
         own and an accepter VPC with which to create the
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc_peering_connection)
@@ -5525,15 +5525,15 @@
 
     def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_KeyPairInfo":
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party
         tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.import_key_pair)
@@ -5556,15 +5556,15 @@
         RootDeviceName: str = ...,
         SriovNetSupport: str = ...,
         VirtualizationType: str = ...,
         BootMode: BootModeValuesType = ...,
         TpmSupport: Literal["v2.0"] = ...,
         UefiData: str = ...,
         ImdsSupport: Literal["v2.0"] = ...,
-        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
     ) -> "_Image":
         """
         Registers an AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.register_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/service_resource/#ec2serviceresourceregister_image-method)
         """
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/type_defs.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
     ResourceTypeType,
     RIProductDescriptionType,
     RootDeviceTypeType,
     RouteOriginType,
     RouteStateType,
     RouteTableAssociationStateCodeType,
     RuleActionType,
+    ScopeType,
     SecurityGroupReferencingSupportValueType,
     SelfServicePortalType,
     ServiceConnectivityTypeType,
     ServiceStateType,
     ServiceTypeType,
     ShutdownBehaviorType,
     SnapshotAttributeNameType,
@@ -306,15 +307,14 @@
     VpcCidrBlockStateCodeType,
     VpcEndpointTypeType,
     VpcPeeringConnectionStateReasonCodeType,
     VpcStateType,
     VpnEcmpSupportValueType,
     VpnStateType,
     WeekDayType,
-    scopeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -876,26 +876,26 @@
     "InstanceIpv6PrefixTypeDef",
     "InstanceMaintenanceOptionsRequestTypeDef",
     "InstanceMaintenanceOptionsTypeDef",
     "InstanceMetadataOptionsRequestTypeDef",
     "InstanceMetadataOptionsResponseTypeDef",
     "MonitoringTypeDef",
     "InstanceNetworkInterfaceAssociationTypeDef",
-    "MemoryGiBPerVCpuRequestTypeDef",
-    "MemoryMiBRequestTypeDef",
-    "NetworkBandwidthGbpsRequestTypeDef",
-    "NetworkInterfaceCountRequestTypeDef",
-    "TotalLocalStorageGBRequestTypeDef",
-    "VCpuCountRangeRequestTypeDef",
     "MemoryGiBPerVCpuTypeDef",
     "MemoryMiBTypeDef",
     "NetworkBandwidthGbpsTypeDef",
     "NetworkInterfaceCountTypeDef",
     "TotalLocalStorageGBTypeDef",
     "VCpuCountRangeTypeDef",
+    "MemoryGiBPerVCpuRequestTypeDef",
+    "MemoryMiBRequestTypeDef",
+    "NetworkBandwidthGbpsRequestTypeDef",
+    "NetworkInterfaceCountRequestTypeDef",
+    "TotalLocalStorageGBRequestTypeDef",
+    "VCpuCountRangeRequestTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
     "NitroTpmInfoTypeDef",
@@ -1089,14 +1089,15 @@
     "RestoreAddressToClassicRequestRequestTypeDef",
     "RestoreImageFromRecycleBinRequestRequestTypeDef",
     "RestoreManagedPrefixListVersionRequestRequestTypeDef",
     "RestoreSnapshotFromRecycleBinRequestRequestTypeDef",
     "RestoreSnapshotTierRequestRequestTypeDef",
     "RevokeClientVpnIngressRequestRequestTypeDef",
     "RouteTypeDef",
+    "S3StorageOutputTypeDef",
     "ScheduledInstanceRecurrenceTypeDef",
     "ScheduledInstancesEbsTypeDef",
     "ScheduledInstancesIamInstanceProfileTypeDef",
     "ScheduledInstancesIpv6AddressTypeDef",
     "ScheduledInstancesMonitoringTypeDef",
     "ScheduledInstancesPlacementTypeDef",
     "ScheduledInstancesPrivateIpAddressConfigTypeDef",
@@ -1350,17 +1351,20 @@
     "PlacementGroupTypeDef",
     "ReplaceRootVolumeTaskTypeDef",
     "SecurityGroupForVpcTypeDef",
     "SnapshotInfoTypeDef",
     "SnapshotResponseTypeDef",
     "SnapshotTierStatusTypeDef",
     "SnapshotTypeDef",
+    "SpotFleetTagSpecificationExtraOutputTypeDef",
+    "SpotFleetTagSpecificationOutputTypeDef",
     "SpotFleetTagSpecificationTypeDef",
     "SubnetCidrReservationTypeDef",
-    "TagSpecificationPaginatorTypeDef",
+    "TagSpecificationExtraOutputTypeDef",
+    "TagSpecificationOutputTypeDef",
     "TagSpecificationTypeDef",
     "TrafficMirrorSessionTypeDef",
     "TrafficMirrorTargetTypeDef",
     "TransitGatewayPolicyTableTypeDef",
     "TransitGatewayRouteTableAnnouncementTypeDef",
     "TransitGatewayRouteTableTypeDef",
     "TrunkInterfaceAssociationTypeDef",
@@ -1447,14 +1451,16 @@
     "CapacityReservationSpecificationResponseResponseTypeDef",
     "CapacityReservationSpecificationResponseTypeDef",
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     "CapacityReservationSpecificationTypeDef",
     "LaunchTemplateCapacityReservationSpecificationRequestTypeDef",
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     "ClassicLinkInstanceTypeDef",
+    "ClassicLoadBalancersConfigExtraOutputTypeDef",
+    "ClassicLoadBalancersConfigOutputTypeDef",
     "ClassicLoadBalancersConfigTypeDef",
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     "ClientConnectResponseOptionsTypeDef",
     "ClientVpnAuthenticationRequestTypeDef",
     "ClientVpnAuthenticationTypeDef",
     "ClientVpnConnectionTypeDef",
     "TerminateConnectionStatusTypeDef",
@@ -1903,20 +1909,23 @@
     "ImportInstanceLaunchSpecificationTypeDef",
     "InferenceDeviceInfoTypeDef",
     "InstanceAttachmentEnaSrdSpecificationTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
-    "InstanceRequirementsRequestTypeDef",
+    "InstanceRequirementsExtraOutputTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
+    "InstanceRequirementsRequestTypeDef",
     "InstanceStateChangeTypeDef",
     "InstanceStatusSummaryTypeDef",
     "ModifyInstanceEventStartTimeResultTypeDef",
-    "IpPermissionPaginatorTypeDef",
+    "IpPermissionExtraExtraOutputTypeDef",
+    "IpPermissionOutputTypeDef",
     "IpPermissionTypeDef",
     "StaleIpPermissionTypeDef",
     "ProvisionIpamPoolCidrRequestRequestTypeDef",
     "IpamDiscoveredAccountTypeDef",
     "IpamDiscoveredResourceCidrTypeDef",
     "IpamResourceCidrTypeDef",
     "IpamResourceDiscoveryTypeDef",
@@ -1964,14 +1973,15 @@
     "PurchaseReservedInstancesOfferingRequestRequestTypeDef",
     "ReservedInstancesOfferingTypeDef",
     "ReservedInstancesTypeDef",
     "SecurityGroupRuleTypeDef",
     "RegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     "RegisterTransitGatewayMulticastGroupMembersResultTypeDef",
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
+    "StorageOutputTypeDef",
     "ScheduledInstanceAvailabilityTypeDef",
     "ScheduledInstanceTypeDef",
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     "ScheduledInstancesNetworkInterfaceTypeDef",
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     "VpcEndpointTypeDef",
     "SecurityGroupRuleUpdateTypeDef",
@@ -1981,14 +1991,16 @@
     "SnapshotTaskDetailTypeDef",
     "SpotMaintenanceStrategiesTypeDef",
     "SpotDatafeedSubscriptionTypeDef",
     "TransitGatewayMulticastDomainAssociationTypeDef",
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     "SubnetIpv6CidrBlockAssociationTypeDef",
     "TargetReservationValueTypeDef",
+    "TargetGroupsConfigExtraOutputTypeDef",
+    "TargetGroupsConfigOutputTypeDef",
     "TargetGroupsConfigTypeDef",
     "TrafficMirrorFilterRuleTypeDef",
     "TransitGatewayAttachmentTypeDef",
     "TransitGatewayConnectPeerConfigurationTypeDef",
     "TransitGatewayConnectTypeDef",
     "TransitGatewayMulticastDomainTypeDef",
     "TransitGatewayTypeDef",
@@ -2070,106 +2082,23 @@
     "GetSecurityGroupsForVpcResultTypeDef",
     "CreateSnapshotsResultTypeDef",
     "DescribeSnapshotTierStatusResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "CreateSubnetCidrReservationResultTypeDef",
     "DeleteSubnetCidrReservationResultTypeDef",
     "GetSubnetCidrReservationsResultTypeDef",
-    "AcceptAddressTransferRequestRequestTypeDef",
-    "AllocateAddressRequestRequestTypeDef",
-    "AllocateHostsRequestRequestTypeDef",
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CopyImageRequestRequestTypeDef",
-    "CopySnapshotRequestRequestTypeDef",
     "CopySnapshotRequestSnapshotCopyTypeDef",
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    "CreateCapacityReservationRequestRequestTypeDef",
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    "CreateCoipPoolRequestRequestTypeDef",
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    "CreateFlowLogsRequestRequestTypeDef",
-    "CreateFpgaImageRequestRequestTypeDef",
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    "CreateInternetGatewayRequestRequestTypeDef",
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    "CreateIpamPoolRequestRequestTypeDef",
-    "CreateIpamRequestRequestTypeDef",
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CreateIpamScopeRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    "CreateNatGatewayRequestRequestTypeDef",
-    "CreateNetworkAclRequestRequestTypeDef",
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
-    "CreatePlacementGroupRequestRequestTypeDef",
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    "CreateRouteTableRequestRequestTypeDef",
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
-    "CreateSecurityGroupRequestRequestTypeDef",
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
-    "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
-    "CreateSnapshotsRequestRequestTypeDef",
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    "CreateSubnetRequestRequestTypeDef",
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    "CreateTransitGatewayRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    "CreateVpcEndpointRequestRequestTypeDef",
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
-    "CreateVpcRequestRequestTypeDef",
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    "CreateVpnGatewayRequestRequestTypeDef",
-    "ExportImageRequestRequestTypeDef",
-    "ImportKeyPairRequestRequestTypeDef",
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    "PurchaseCapacityBlockRequestRequestTypeDef",
-    "PurchaseHostReservationRequestRequestTypeDef",
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
+    "TagSpecificationUnionTypeDef",
     "CreateTrafficMirrorSessionResultTypeDef",
     "DescribeTrafficMirrorSessionsResultTypeDef",
     "ModifyTrafficMirrorSessionResultTypeDef",
     "CreateTrafficMirrorTargetResultTypeDef",
     "DescribeTrafficMirrorTargetsResultTypeDef",
     "CreateTransitGatewayPolicyTableResultTypeDef",
     "DeleteTransitGatewayPolicyTableResultTypeDef",
@@ -2205,28 +2134,24 @@
     "NetworkInterfaceAttachmentTypeDef",
     "DhcpOptionsTypeDef",
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     "DescribeAvailabilityZonesResultTypeDef",
     "HostTypeDef",
     "StorageTypeDef",
     "CreateImageRequestInstanceCreateImageTypeDef",
-    "CreateImageRequestRequestTypeDef",
     "ImageAttributeTypeDef",
     "ImageTypeDef",
-    "RegisterImageRequestRequestTypeDef",
-    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
     "CancelCapacityReservationFleetsResultTypeDef",
     "CancelSpotFleetRequestsResponseTypeDef",
     "CreateCapacityReservationResultTypeDef",
     "DescribeCapacityReservationsResultTypeDef",
     "PurchaseCapacityBlockResultTypeDef",
     "DescribeCapacityReservationFleetsResultTypeDef",
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     "DescribeClassicLinkInstancesResultTypeDef",
-    "CreateClientVpnEndpointRequestRequestTypeDef",
     "ClientVpnEndpointTypeDef",
     "DescribeClientVpnConnectionsResultTypeDef",
     "TerminateClientVpnConnectionsResultTypeDef",
     "DescribeClientVpnRoutesResultTypeDef",
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     "VpnTunnelOptionsSpecificationTypeDef",
     "TunnelOptionTypeDef",
@@ -2247,16 +2172,16 @@
     "ModifyInstanceAttributeRequestRequestTypeDef",
     "InstanceAttributeTypeDef",
     "CreateEgressOnlyInternetGatewayResultTypeDef",
     "DescribeEgressOnlyInternetGatewaysResultTypeDef",
     "CreateInternetGatewayResultTypeDef",
     "DescribeInternetGatewaysResultTypeDef",
     "DescribeElasticGpusResultTypeDef",
-    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
-    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
+    "InstanceNetworkInterfaceSpecificationExtraOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
     "InstanceNetworkInterfaceSpecificationTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "AttachNetworkInterfaceRequestNetworkInterfaceAttachTypeDef",
     "AttachNetworkInterfaceRequestRequestTypeDef",
     "ModifyNetworkInterfaceAttributeRequestNetworkInterfaceModifyAttributeTypeDef",
     "ModifyNetworkInterfaceAttributeRequestRequestTypeDef",
     "EnableFastSnapshotRestoreErrorItemTypeDef",
@@ -2275,48 +2200,42 @@
     "GpuInfoTypeDef",
     "AssociateIamInstanceProfileResultTypeDef",
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
-    "ImportImageRequestRequestTypeDef",
-    "ImportSnapshotRequestRequestTypeDef",
     "CreateLocalGatewayRouteTableResultTypeDef",
     "DeleteLocalGatewayRouteTableResultTypeDef",
     "DescribeLocalGatewayRouteTablesResultTypeDef",
     "ImportInstanceRequestRequestTypeDef",
     "InferenceAcceleratorInfoTypeDef",
     "InstanceNetworkInterfaceAttachmentTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
+    "LaunchTemplateOverridesExtraOutputTypeDef",
+    "FleetLaunchTemplateOverridesTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
+    "LaunchTemplateOverridesTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
-    "FleetLaunchTemplateOverridesTypeDef",
-    "LaunchTemplateOverridesTypeDef",
     "StartInstancesResultTypeDef",
     "StopInstancesResultTypeDef",
     "TerminateInstancesResultTypeDef",
     "InstanceStatusTypeDef",
-    "SecurityGroupPaginatorTypeDef",
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
+    "RevokeSecurityGroupEgressResultTypeDef",
+    "RevokeSecurityGroupIngressResultTypeDef",
+    "SecurityGroupTypeDef",
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
+    "IpPermissionUnionTypeDef",
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
-    "RevokeSecurityGroupEgressResultTypeDef",
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
-    "RevokeSecurityGroupIngressResultTypeDef",
-    "SecurityGroupTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
     "StaleSecurityGroupTypeDef",
     "GetIpamDiscoveredAccountsResultTypeDef",
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     "GetIpamResourceCidrsResultTypeDef",
     "ModifyIpamResourceCidrResultTypeDef",
     "CreateIpamResourceDiscoveryResultTypeDef",
     "DeleteIpamResourceDiscoveryResultTypeDef",
@@ -2348,26 +2267,26 @@
     "CreateNetworkInterfacePermissionResultTypeDef",
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     "NeuronInfoTypeDef",
     "CreateVerifiedAccessTrustProviderResultTypeDef",
     "DeleteVerifiedAccessTrustProviderResultTypeDef",
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
     "AccessScopePathRequestTypeDef",
     "AccessScopePathTypeDef",
     "CancelReservedInstancesListingResultTypeDef",
     "CreateReservedInstancesListingResultTypeDef",
     "DescribeReservedInstancesListingsResultTypeDef",
     "DescribePublicIpv4PoolsResultTypeDef",
     "DescribeReservedInstancesOfferingsResultTypeDef",
     "DescribeReservedInstancesResultTypeDef",
     "AuthorizeSecurityGroupEgressResultTypeDef",
     "AuthorizeSecurityGroupIngressResultTypeDef",
     "DescribeSecurityGroupRulesResultTypeDef",
+    "BundleTaskTypeDef",
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     "DescribeScheduledInstancesResultTypeDef",
     "PurchaseScheduledInstancesResultTypeDef",
     "ScheduledInstancesLaunchSpecificationTypeDef",
     "CreateVpcEndpointResultTypeDef",
     "DescribeVpcEndpointsResultTypeDef",
     "ModifySecurityGroupRulesRequestRequestTypeDef",
@@ -2385,14 +2304,16 @@
     "AssociateTransitGatewayMulticastDomainResultTypeDef",
     "DisassociateTransitGatewayMulticastDomainResultTypeDef",
     "RejectTransitGatewayMulticastDomainAssociationsResultTypeDef",
     "AssociateSubnetCidrBlockResultTypeDef",
     "DisassociateSubnetCidrBlockResultTypeDef",
     "SubnetTypeDef",
     "GetReservedInstancesExchangeQuoteResultTypeDef",
+    "LoadBalancersConfigExtraOutputTypeDef",
+    "LoadBalancersConfigOutputTypeDef",
     "LoadBalancersConfigTypeDef",
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     "ModifyTrafficMirrorFilterRuleResultTypeDef",
     "TrafficMirrorFilterTypeDef",
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     "TransitGatewayConnectPeerTypeDef",
     "CreateTransitGatewayConnectResultTypeDef",
@@ -2455,61 +2376,163 @@
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
+    "AcceptAddressTransferRequestRequestTypeDef",
+    "AllocateAddressRequestRequestTypeDef",
+    "AllocateHostsRequestRequestTypeDef",
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CopyImageRequestRequestTypeDef",
+    "CopySnapshotRequestRequestTypeDef",
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    "CreateCapacityReservationRequestRequestTypeDef",
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    "CreateClientVpnEndpointRequestRequestTypeDef",
+    "CreateCoipPoolRequestRequestTypeDef",
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    "CreateFlowLogsRequestRequestTypeDef",
+    "CreateFpgaImageRequestRequestTypeDef",
+    "CreateImageRequestRequestTypeDef",
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    "CreateInternetGatewayRequestRequestTypeDef",
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    "CreateIpamPoolRequestRequestTypeDef",
+    "CreateIpamRequestRequestTypeDef",
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CreateIpamScopeRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    "CreateNatGatewayRequestRequestTypeDef",
+    "CreateNetworkAclRequestRequestTypeDef",
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    "CreatePlacementGroupRequestRequestTypeDef",
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    "CreateRouteTableRequestRequestTypeDef",
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    "CreateSecurityGroupRequestRequestTypeDef",
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    "CreateSnapshotsRequestRequestTypeDef",
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    "CreateSubnetRequestRequestTypeDef",
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    "CreateTransitGatewayRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    "CreateVpcEndpointRequestRequestTypeDef",
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    "CreateVpcRequestRequestTypeDef",
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    "CreateVpnGatewayRequestRequestTypeDef",
+    "ExportImageRequestRequestTypeDef",
+    "ImportImageRequestRequestTypeDef",
+    "ImportKeyPairRequestRequestTypeDef",
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    "ImportSnapshotRequestRequestTypeDef",
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    "PurchaseCapacityBlockRequestRequestTypeDef",
+    "PurchaseHostReservationRequestRequestTypeDef",
+    "RegisterImageRequestRequestTypeDef",
+    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
     "DescribeRouteTablesResultTypeDef",
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     "DescribeNetworkInterfaceAttributeResultTypeDef",
     "NetworkInterfaceTypeDef",
     "CreateDhcpOptionsResultTypeDef",
     "DescribeDhcpOptionsResultTypeDef",
     "DescribeHostsResultTypeDef",
     "BundleInstanceRequestRequestTypeDef",
-    "BundleTaskTypeDef",
+    "StorageUnionTypeDef",
     "DescribeImagesResultTypeDef",
     "DescribeClientVpnEndpointsResultTypeDef",
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     "VpnConnectionOptionsSpecificationTypeDef",
     "VpnConnectionOptionsTypeDef",
     "CreateNetworkAclResultTypeDef",
     "DescribeNetworkAclsResultTypeDef",
     "DisableFastSnapshotRestoresResultTypeDef",
     "ConversionTaskTypeDef",
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    "RunInstancesRequestSubnetCreateInstancesTypeDef",
+    "SpotFleetLaunchSpecificationExtraOutputTypeDef",
     "LaunchSpecificationTypeDef",
+    "SpotFleetLaunchSpecificationOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationUnionTypeDef",
     "RequestSpotLaunchSpecificationTypeDef",
-    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestSubnetCreateInstancesTypeDef",
     "SpotFleetLaunchSpecificationTypeDef",
     "RequestLaunchTemplateDataTypeDef",
     "EnableFastSnapshotRestoresResultTypeDef",
     "CreateNetworkInsightsPathResultTypeDef",
     "DescribeNetworkInsightsPathsResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
-    "FleetLaunchTemplateConfigRequestTypeDef",
-    "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
-    "GetSpotPlacementScoresRequestRequestTypeDef",
+    "LaunchTemplateConfigExtraOutputTypeDef",
     "FleetLaunchTemplateConfigTypeDef",
     "LaunchTemplateAndOverridesResponseTypeDef",
+    "LaunchTemplateConfigOutputTypeDef",
     "LaunchTemplateConfigTypeDef",
+    "FleetLaunchTemplateConfigRequestTypeDef",
+    "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
+    "GetSpotPlacementScoresRequestRequestTypeDef",
     "DescribeInstanceStatusResultTypeDef",
-    "DescribeSecurityGroupsResultPaginatorTypeDef",
     "DescribeSecurityGroupsResultTypeDef",
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
     "DescribeStaleSecurityGroupsResultTypeDef",
     "GetIpamDiscoveredPublicAddressesResultTypeDef",
     "ResponseLaunchTemplateDataTypeDef",
     "DescribeReservedInstancesModificationsResultTypeDef",
     "InstanceTypeInfoTypeDef",
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     "NetworkInsightsAccessScopeContentTypeDef",
+    "BundleInstanceResultTypeDef",
+    "CancelBundleTaskResultTypeDef",
+    "DescribeBundleTasksResultTypeDef",
     "RunScheduledInstancesRequestRequestTypeDef",
     "DescribeImportImageTasksResultTypeDef",
     "DescribeImportSnapshotTasksResultTypeDef",
     "CreateDefaultSubnetResultTypeDef",
     "CreateSubnetResultTypeDef",
     "DescribeSubnetsResultTypeDef",
     "CreateTrafficMirrorFilterResultTypeDef",
@@ -2527,36 +2550,36 @@
     "AcceptVpcPeeringConnectionResultTypeDef",
     "CreateVpcPeeringConnectionResultTypeDef",
     "DescribeVpcPeeringConnectionsResultTypeDef",
     "AccessScopeAnalysisFindingTypeDef",
     "NetworkInsightsAnalysisTypeDef",
     "CreateNetworkInterfaceResultTypeDef",
     "DescribeNetworkInterfacesResultTypeDef",
-    "BundleInstanceResultTypeDef",
-    "CancelBundleTaskResultTypeDef",
-    "DescribeBundleTasksResultTypeDef",
     "CreateVpnConnectionRequestRequestTypeDef",
     "VpnConnectionTypeDef",
     "DescribeConversionTasksResultTypeDef",
     "ImportInstanceResultTypeDef",
     "ImportVolumeResultTypeDef",
     "SpotInstanceRequestTypeDef",
+    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RequestSpotInstancesRequestRequestTypeDef",
     "CreateLaunchTemplateRequestRequestTypeDef",
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     "InstanceTypeDef",
-    "CreateFleetRequestRequestTypeDef",
-    "ModifyFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataExtraOutputTypeDef",
     "CreateFleetErrorTypeDef",
     "CreateFleetInstanceTypeDef",
     "DescribeFleetErrorTypeDef",
     "DescribeFleetsInstancesTypeDef",
-    "ModifySpotFleetRequestRequestRequestTypeDef",
-    "SpotFleetRequestConfigDataPaginatorTypeDef",
+    "SpotFleetRequestConfigDataOutputTypeDef",
+    "LaunchTemplateConfigUnionTypeDef",
     "SpotFleetRequestConfigDataTypeDef",
+    "CreateFleetRequestRequestTypeDef",
+    "ModifyFleetRequestRequestTypeDef",
     "GetLaunchTemplateDataResultTypeDef",
     "LaunchTemplateVersionTypeDef",
     "DescribeInstanceTypesResultTypeDef",
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     "GetNetworkInsightsAccessScopeContentResultTypeDef",
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
@@ -2571,22 +2594,22 @@
     "ModifyVpnTunnelOptionsResultTypeDef",
     "DescribeSpotInstanceRequestsResultTypeDef",
     "RequestSpotInstancesResultTypeDef",
     "ReservationResponseTypeDef",
     "ReservationTypeDef",
     "CreateFleetResultTypeDef",
     "FleetDataTypeDef",
-    "SpotFleetRequestConfigPaginatorTypeDef",
-    "RequestSpotFleetRequestRequestTypeDef",
     "SpotFleetRequestConfigTypeDef",
+    "ModifySpotFleetRequestRequestRequestTypeDef",
+    "RequestSpotFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataUnionTypeDef",
     "CreateLaunchTemplateVersionResultTypeDef",
     "DescribeLaunchTemplateVersionsResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeFleetsResultTypeDef",
-    "DescribeSpotFleetRequestsResponsePaginatorTypeDef",
     "DescribeSpotFleetRequestsResponseTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": NotRequired[int],
@@ -6927,95 +6950,95 @@
         "CarrierIp": NotRequired[str],
         "CustomerOwnedIp": NotRequired[str],
         "IpOwnerId": NotRequired[str],
         "PublicDnsName": NotRequired[str],
         "PublicIp": NotRequired[str],
     },
 )
-MemoryGiBPerVCpuRequestTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestTypeDef",
+MemoryGiBPerVCpuTypeDef = TypedDict(
+    "MemoryGiBPerVCpuTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-MemoryMiBRequestTypeDef = TypedDict(
-    "MemoryMiBRequestTypeDef",
+MemoryMiBTypeDef = TypedDict(
+    "MemoryMiBTypeDef",
     {
-        "Min": int,
+        "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-NetworkBandwidthGbpsRequestTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestTypeDef",
+NetworkBandwidthGbpsTypeDef = TypedDict(
+    "NetworkBandwidthGbpsTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-NetworkInterfaceCountRequestTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestTypeDef",
+NetworkInterfaceCountTypeDef = TypedDict(
+    "NetworkInterfaceCountTypeDef",
     {
         "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-TotalLocalStorageGBRequestTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestTypeDef",
+TotalLocalStorageGBTypeDef = TypedDict(
+    "TotalLocalStorageGBTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-VCpuCountRangeRequestTypeDef = TypedDict(
-    "VCpuCountRangeRequestTypeDef",
+VCpuCountRangeTypeDef = TypedDict(
+    "VCpuCountRangeTypeDef",
     {
-        "Min": int,
+        "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-MemoryGiBPerVCpuTypeDef = TypedDict(
-    "MemoryGiBPerVCpuTypeDef",
+MemoryGiBPerVCpuRequestTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-MemoryMiBTypeDef = TypedDict(
-    "MemoryMiBTypeDef",
+MemoryMiBRequestTypeDef = TypedDict(
+    "MemoryMiBRequestTypeDef",
     {
-        "Min": NotRequired[int],
+        "Min": int,
         "Max": NotRequired[int],
     },
 )
-NetworkBandwidthGbpsTypeDef = TypedDict(
-    "NetworkBandwidthGbpsTypeDef",
+NetworkBandwidthGbpsRequestTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-NetworkInterfaceCountTypeDef = TypedDict(
-    "NetworkInterfaceCountTypeDef",
+NetworkInterfaceCountRequestTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestTypeDef",
     {
         "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-TotalLocalStorageGBTypeDef = TypedDict(
-    "TotalLocalStorageGBTypeDef",
+TotalLocalStorageGBRequestTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-VCpuCountRangeTypeDef = TypedDict(
-    "VCpuCountRangeTypeDef",
+VCpuCountRangeRequestTypeDef = TypedDict(
+    "VCpuCountRangeRequestTypeDef",
     {
-        "Min": NotRequired[int],
+        "Min": int,
         "Max": NotRequired[int],
     },
 )
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": NotRequired[int],
@@ -7678,15 +7701,15 @@
 ReservedInstancesConfigurationTypeDef = TypedDict(
     "ReservedInstancesConfigurationTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "InstanceCount": NotRequired[int],
         "InstanceType": NotRequired[InstanceTypeType],
         "Platform": NotRequired[str],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
     },
 )
 ModifySnapshotTierRequestRequestTypeDef = TypedDict(
     "ModifySnapshotTierRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "StorageTier": NotRequired[Literal["archive"]],
@@ -8666,14 +8689,24 @@
         "NetworkInterfaceId": NotRequired[str],
         "Origin": NotRequired[RouteOriginType],
         "State": NotRequired[RouteStateType],
         "VpcPeeringConnectionId": NotRequired[str],
         "CoreNetworkArn": NotRequired[str],
     },
 )
+S3StorageOutputTypeDef = TypedDict(
+    "S3StorageOutputTypeDef",
+    {
+        "AWSAccessKeyId": NotRequired[str],
+        "Bucket": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "UploadPolicy": NotRequired[bytes],
+        "UploadPolicySignature": NotRequired[str],
+    },
+)
 ScheduledInstanceRecurrenceTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceTypeDef",
     {
         "Frequency": NotRequired[str],
         "Interval": NotRequired[int],
         "OccurrenceDaySet": NotRequired[List[int]],
         "OccurrenceRelativeToEnd": NotRequired[bool],
@@ -9529,16 +9562,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeAddressTransfersResultTypeDef = TypedDict(
     "DescribeAddressTransfersResultTypeDef",
     {
         "AddressTransfers": List[AddressTransferTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DetachClassicLinkVpcResultTypeDef = TypedDict(
     "DetachClassicLinkVpcResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10337,26 +10370,26 @@
         "AttributeValues": NotRequired[List[AccountAttributeValueTypeDef]],
     },
 )
 DescribeFleetInstancesResultTypeDef = TypedDict(
     "DescribeFleetInstancesResultTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
-        "NextToken": str,
         "FleetId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetInstancesResponseTypeDef = TypedDict(
     "DescribeSpotFleetInstancesResponseTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
-        "NextToken": str,
         "SpotFleetRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpcEndpointServicePermissionsResultTypeDef = TypedDict(
     "ModifyVpcEndpointServicePermissionsResultTypeDef",
     {
         "AddedPrincipals": List[AddedPrincipalTypeDef],
         "ReturnValue": bool,
@@ -10874,35 +10907,56 @@
         "OutpostArn": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "StorageTier": NotRequired[StorageTierType],
         "RestoreExpiryTime": NotRequired[datetime],
         "SseType": NotRequired[SSETypeType],
     },
 )
+SpotFleetTagSpecificationExtraOutputTypeDef = TypedDict(
+    "SpotFleetTagSpecificationExtraOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
+SpotFleetTagSpecificationOutputTypeDef = TypedDict(
+    "SpotFleetTagSpecificationOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": NotRequired[ResourceTypeType],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
         "SubnetCidrReservationId": NotRequired[str],
         "SubnetId": NotRequired[str],
         "Cidr": NotRequired[str],
         "ReservationType": NotRequired[SubnetCidrReservationTypeType],
         "OwnerId": NotRequired[str],
         "Description": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-TagSpecificationPaginatorTypeDef = TypedDict(
-    "TagSpecificationPaginatorTypeDef",
+TagSpecificationExtraOutputTypeDef = TypedDict(
+    "TagSpecificationExtraOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
+TagSpecificationOutputTypeDef = TypedDict(
+    "TagSpecificationOutputTypeDef",
     {
         "ResourceType": NotRequired[ResourceTypeType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 TagSpecificationTypeDef = TypedDict(
     "TagSpecificationTypeDef",
@@ -11011,16 +11065,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetIpamPoolAllocationsResultTypeDef = TypedDict(
     "GetIpamPoolAllocationsResultTypeDef",
     {
         "IpamPoolAllocations": List[IpamPoolAllocationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AnalysisAclRuleTypeDef = TypedDict(
     "AnalysisAclRuleTypeDef",
     {
         "Cidr": NotRequired[str],
         "Egress": NotRequired[bool],
@@ -11234,16 +11288,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayPolicyTableAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayPolicyTableAssociationsResultTypeDef",
     {
         "Associations": List[TransitGatewayPolicyTableAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateTransitGatewayRouteTableResultTypeDef = TypedDict(
     "AssociateTransitGatewayRouteTableResultTypeDef",
     {
         "Association": TransitGatewayAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11607,16 +11661,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamByoasnResultTypeDef = TypedDict(
     "DescribeIpamByoasnResultTypeDef",
     {
         "Byoasns": List[ByoasnTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ProvisionIpamByoasnResultTypeDef = TypedDict(
     "ProvisionIpamByoasnResultTypeDef",
     {
         "Byoasn": ByoasnTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11674,16 +11728,16 @@
         "ReservationType": NotRequired[CapacityReservationTypeType],
     },
 )
 DescribeCapacityBlockOfferingsResultTypeDef = TypedDict(
     "DescribeCapacityBlockOfferingsResultTypeDef",
     {
         "CapacityBlockOfferings": List[CapacityBlockOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CapacityReservationFleetTypeDef = TypedDict(
     "CapacityReservationFleetTypeDef",
     {
         "CapacityReservationFleetId": NotRequired[str],
         "CapacityReservationFleetArn": NotRequired[str],
@@ -11715,17 +11769,17 @@
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetGroupsForCapacityReservationResultTypeDef = TypedDict(
     "GetGroupsForCapacityReservationResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservationGroups": List[CapacityReservationGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 OnDemandOptionsRequestTypeDef = TypedDict(
     "OnDemandOptionsRequestTypeDef",
     {
         "AllocationStrategy": NotRequired[FleetOnDemandAllocationStrategyType],
         "CapacityReservationOptions": NotRequired[CapacityReservationOptionsRequestTypeDef],
@@ -11781,32 +11835,44 @@
         "CapacityReservationPreference": NotRequired[CapacityReservationPreferenceType],
         "CapacityReservationTarget": NotRequired[CapacityReservationTargetTypeDef],
     },
 )
 DescribeVpcClassicLinkDnsSupportResultTypeDef = TypedDict(
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     {
-        "NextToken": str,
         "Vpcs": List[ClassicLinkDnsSupportTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ClassicLinkInstanceTypeDef = TypedDict(
     "ClassicLinkInstanceTypeDef",
     {
         "Groups": NotRequired[List[GroupIdentifierTypeDef]],
         "InstanceId": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
+ClassicLoadBalancersConfigExtraOutputTypeDef = TypedDict(
+    "ClassicLoadBalancersConfigExtraOutputTypeDef",
+    {
+        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+    },
+)
+ClassicLoadBalancersConfigOutputTypeDef = TypedDict(
+    "ClassicLoadBalancersConfigOutputTypeDef",
+    {
+        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+    },
+)
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
-        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+        "ClassicLoadBalancers": NotRequired[Sequence[ClassicLoadBalancerTypeDef]],
     },
 )
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
         "CertificateRevocationList": str,
         "Status": ClientCertificateRevocationListStatusTypeDef,
@@ -11922,16 +11988,16 @@
 )
 GetCoipPoolUsageResultTypeDef = TypedDict(
     "GetCoipPoolUsageResultTypeDef",
     {
         "CoipPoolId": str,
         "CoipAddressUsages": List[CoipAddressUsageTypeDef],
         "LocalGatewayRouteTableId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCoipCidrResultTypeDef = TypedDict(
     "CreateCoipCidrResultTypeDef",
     {
         "CoipCidr": CoipCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11952,16 +12018,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointConnectionNotificationsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionNotificationsResultTypeDef",
     {
         "ConnectionNotificationSet": List[ConnectionNotificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "ModifyInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "DryRun": NotRequired[bool],
@@ -12006,16 +12072,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchLocalGatewayRoutesResultTypeDef = TypedDict(
     "SearchLocalGatewayRoutesResultTypeDef",
     {
         "Routes": List[LocalGatewayRouteTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef = TypedDict(
     "CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef",
     {
         "Egress": bool,
         "Protocol": str,
@@ -15019,17 +15085,17 @@
         "Arn": NotRequired[str],
         "Statuses": NotRequired[List[IdFormatTypeDef]],
     },
 )
 DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef = TypedDict(
     "DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef",
     {
-        "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeBundleTasksRequestBundleTaskCompleteWaitTypeDef = TypedDict(
     "DescribeBundleTasksRequestBundleTaskCompleteWaitTypeDef",
     {
         "BundleIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
@@ -15455,80 +15521,80 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeFastSnapshotRestoresResultTypeDef = TypedDict(
     "DescribeFastSnapshotRestoresResultTypeDef",
     {
         "FastSnapshotRestores": List[DescribeFastSnapshotRestoreSuccessItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostReservationOfferingsResultTypeDef = TypedDict(
     "DescribeHostReservationOfferingsResultTypeDef",
     {
-        "NextToken": str,
         "OfferingSet": List[HostOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceCreditSpecificationsResultTypeDef = TypedDict(
     "DescribeInstanceCreditSpecificationsResultTypeDef",
     {
         "InstanceCreditSpecifications": List[InstanceCreditSpecificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceTopologyResultTypeDef = TypedDict(
     "DescribeInstanceTopologyResultTypeDef",
     {
         "Instances": List[InstanceTopologyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceTypeOfferingsResultTypeDef = TypedDict(
     "DescribeInstanceTypeOfferingsResultTypeDef",
     {
         "InstanceTypeOfferings": List[InstanceTypeOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLockedSnapshotsResultTypeDef = TypedDict(
     "DescribeLockedSnapshotsResultTypeDef",
     {
         "Snapshots": List[LockedSnapshotsInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeMacHostsResultTypeDef = TypedDict(
     "DescribeMacHostsResultTypeDef",
     {
         "MacHosts": List[MacHostTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeMovingAddressesResultTypeDef = TypedDict(
     "DescribeMovingAddressesResultTypeDef",
     {
         "MovingAddressStatuses": List[MovingAddressStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePrefixListsResultTypeDef = TypedDict(
     "DescribePrefixListsResultTypeDef",
     {
-        "NextToken": str,
         "PrefixLists": List[PrefixListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegionsResultTypeDef = TypedDict(
     "DescribeRegionsResultTypeDef",
     {
         "Regions": List[RegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15558,41 +15624,41 @@
         "VolumeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSpotPriceHistoryResultTypeDef = TypedDict(
     "DescribeSpotPriceHistoryResultTypeDef",
     {
-        "NextToken": str,
         "SpotPriceHistory": List[SpotPriceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStoreImageTasksResultTypeDef = TypedDict(
     "DescribeStoreImageTasksResultTypeDef",
     {
         "StoreImageTaskResults": List[StoreImageTaskResultTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeTagsResultTypeDef = TypedDict(
     "DescribeTagsResultTypeDef",
     {
-        "NextToken": str,
         "Tags": List[TagDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVolumesModificationsResultTypeDef = TypedDict(
     "DescribeVolumesModificationsResultTypeDef",
     {
         "VolumesModifications": List[VolumeModificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVolumeResultTypeDef = TypedDict(
     "ModifyVolumeResultTypeDef",
     {
         "VolumeModification": VolumeModificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15928,29 +15994,29 @@
         "InstanceTypes": NotRequired[List[str]],
     },
 )
 GetAssociatedIpv6PoolCidrsResultTypeDef = TypedDict(
     "GetAssociatedIpv6PoolCidrsResultTypeDef",
     {
         "Ipv6CidrAssociations": List[Ipv6CidrAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetCapacityReservationUsageResultTypeDef = TypedDict(
     "GetCapacityReservationUsageResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservationId": str,
         "InstanceType": str,
         "TotalInstanceCount": int,
         "AvailableInstanceCount": int,
         "State": CapacityReservationStateType,
         "InstanceUsages": List[InstanceUsageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDefaultCreditSpecificationResultTypeDef = TypedDict(
     "GetDefaultCreditSpecificationResultTypeDef",
     {
         "InstanceFamilyCreditSpecification": InstanceFamilyCreditSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15991,87 +16057,87 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetInstanceTypesFromInstanceRequirementsResultTypeDef = TypedDict(
     "GetInstanceTypesFromInstanceRequirementsResultTypeDef",
     {
         "InstanceTypes": List[InstanceTypeInfoFromInstanceRequirementsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamAddressHistoryResultTypeDef = TypedDict(
     "GetIpamAddressHistoryResultTypeDef",
     {
         "HistoryRecords": List[IpamAddressHistoryRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetManagedPrefixListAssociationsResultTypeDef = TypedDict(
     "GetManagedPrefixListAssociationsResultTypeDef",
     {
         "PrefixListAssociations": List[PrefixListAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetManagedPrefixListEntriesResultTypeDef = TypedDict(
     "GetManagedPrefixListEntriesResultTypeDef",
     {
         "Entries": List[PrefixListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ReservedInstanceReservationValueTypeDef = TypedDict(
     "ReservedInstanceReservationValueTypeDef",
     {
         "ReservationValue": NotRequired[ReservationValueTypeDef],
         "ReservedInstanceId": NotRequired[str],
     },
 )
 GetSpotPlacementScoresResultTypeDef = TypedDict(
     "GetSpotPlacementScoresResultTypeDef",
     {
         "SpotPlacementScores": List[SpotPlacementScoreTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayAttachmentPropagationsResultTypeDef = TypedDict(
     "GetTransitGatewayAttachmentPropagationsResultTypeDef",
     {
         "TransitGatewayAttachmentPropagations": List[TransitGatewayAttachmentPropagationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayRouteTableAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAssociationsResultTypeDef",
     {
         "Associations": List[TransitGatewayRouteTableAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayRouteTablePropagationsResultTypeDef = TypedDict(
     "GetTransitGatewayRouteTablePropagationsResultTypeDef",
     {
         "TransitGatewayRouteTablePropagations": List[TransitGatewayRouteTablePropagationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVpnConnectionDeviceTypesResultTypeDef = TypedDict(
     "GetVpnConnectionDeviceTypesResultTypeDef",
     {
         "VpnConnectionDeviceTypes": List[VpnConnectionDeviceTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVpnTunnelReplacementStatusResultTypeDef = TypedDict(
     "GetVpnTunnelReplacementStatusResultTypeDef",
     {
         "VpnConnectionId": str,
         "TransitGatewayId": str,
@@ -16128,16 +16194,16 @@
         "UserBucket": NotRequired[UserBucketTypeDef],
     },
 )
 ListImagesInRecycleBinResultTypeDef = TypedDict(
     "ListImagesInRecycleBinResultTypeDef",
     {
         "Images": List[ImageRecycleBinInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LocalGatewayRouteTableTypeDef = TypedDict(
     "LocalGatewayRouteTableTypeDef",
     {
         "LocalGatewayRouteTableId": NotRequired[str],
         "LocalGatewayRouteTableArn": NotRequired[str],
@@ -16210,45 +16276,45 @@
     {
         "Association": NotRequired[InstanceNetworkInterfaceAssociationTypeDef],
         "Primary": NotRequired[bool],
         "PrivateDnsName": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
     },
 )
-InstanceRequirementsRequestTypeDef = TypedDict(
-    "InstanceRequirementsRequestTypeDef",
+InstanceRequirementsExtraOutputTypeDef = TypedDict(
+    "InstanceRequirementsExtraOutputTypeDef",
     {
-        "VCpuCount": VCpuCountRangeRequestTypeDef,
-        "MemoryMiB": MemoryMiBRequestTypeDef,
-        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
-        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuRequestTypeDef],
-        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
-        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
+        "MemoryMiB": NotRequired[MemoryMiBTypeDef],
+        "CpuManufacturers": NotRequired[List[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
+        "ExcludedInstanceTypes": NotRequired[List[str]],
+        "InstanceGenerations": NotRequired[List[InstanceGenerationType]],
         "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
         "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
         "BareMetal": NotRequired[BareMetalType],
         "BurstablePerformance": NotRequired[BurstablePerformanceType],
         "RequireHibernateSupport": NotRequired[bool],
-        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountRequestTypeDef],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountTypeDef],
         "LocalStorage": NotRequired[LocalStorageType],
-        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
-        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBRequestTypeDef],
-        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsRequestTypeDef],
-        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
-        "AcceleratorCount": NotRequired[AcceleratorCountRequestTypeDef],
-        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
-        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
-        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBRequestTypeDef],
-        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsRequestTypeDef],
-        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "LocalStorageTypes": NotRequired[List[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsTypeDef],
+        "AcceleratorTypes": NotRequired[List[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountTypeDef],
+        "AcceleratorManufacturers": NotRequired[List[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[List[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
+        "AllowedInstanceTypes": NotRequired[List[str]],
         "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
     },
 )
-InstanceRequirementsTypeDef = TypedDict(
-    "InstanceRequirementsTypeDef",
+InstanceRequirementsOutputTypeDef = TypedDict(
+    "InstanceRequirementsOutputTypeDef",
     {
         "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
         "MemoryMiB": NotRequired[MemoryMiBTypeDef],
         "CpuManufacturers": NotRequired[List[CpuManufacturerType]],
         "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
         "ExcludedInstanceTypes": NotRequired[List[str]],
         "InstanceGenerations": NotRequired[List[InstanceGenerationType]],
@@ -16268,14 +16334,72 @@
         "AcceleratorNames": NotRequired[List[AcceleratorNameType]],
         "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
         "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
         "AllowedInstanceTypes": NotRequired[List[str]],
         "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
     },
 )
+InstanceRequirementsTypeDef = TypedDict(
+    "InstanceRequirementsTypeDef",
+    {
+        "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
+        "MemoryMiB": NotRequired[MemoryMiBTypeDef],
+        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
+        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
+        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "BareMetal": NotRequired[BareMetalType],
+        "BurstablePerformance": NotRequired[BurstablePerformanceType],
+        "RequireHibernateSupport": NotRequired[bool],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountTypeDef],
+        "LocalStorage": NotRequired[LocalStorageType],
+        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsTypeDef],
+        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountTypeDef],
+        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
+        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
+    },
+)
+InstanceRequirementsRequestTypeDef = TypedDict(
+    "InstanceRequirementsRequestTypeDef",
+    {
+        "VCpuCount": VCpuCountRangeRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
+        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuRequestTypeDef],
+        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
+        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "BareMetal": NotRequired[BareMetalType],
+        "BurstablePerformance": NotRequired[BurstablePerformanceType],
+        "RequireHibernateSupport": NotRequired[bool],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountRequestTypeDef],
+        "LocalStorage": NotRequired[LocalStorageType],
+        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBRequestTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsRequestTypeDef],
+        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountRequestTypeDef],
+        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBRequestTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsRequestTypeDef],
+        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
+    },
+)
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": NotRequired[InstanceStateTypeDef],
         "InstanceId": NotRequired[str],
         "PreviousState": NotRequired[InstanceStateTypeDef],
     },
@@ -16290,16 +16414,28 @@
 ModifyInstanceEventStartTimeResultTypeDef = TypedDict(
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-IpPermissionPaginatorTypeDef = TypedDict(
-    "IpPermissionPaginatorTypeDef",
+IpPermissionExtraExtraOutputTypeDef = TypedDict(
+    "IpPermissionExtraExtraOutputTypeDef",
+    {
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "IpRanges": NotRequired[List[IpRangeTypeDef]],
+        "Ipv6Ranges": NotRequired[List[Ipv6RangeTypeDef]],
+        "PrefixListIds": NotRequired[List[PrefixListIdTypeDef]],
+        "ToPort": NotRequired[int],
+        "UserIdGroupPairs": NotRequired[List[UserIdGroupPairTypeDef]],
+    },
+)
+IpPermissionOutputTypeDef = TypedDict(
+    "IpPermissionOutputTypeDef",
     {
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "IpRanges": NotRequired[List[IpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[List[Ipv6RangeTypeDef]],
         "PrefixListIds": NotRequired[List[PrefixListIdTypeDef]],
         "ToPort": NotRequired[int],
@@ -16506,16 +16642,16 @@
         "SpotOptions": NotRequired[LaunchTemplateSpotMarketOptionsTypeDef],
     },
 )
 ListSnapshotsInRecycleBinResultTypeDef = TypedDict(
     "ListSnapshotsInRecycleBinResultTypeDef",
     {
         "Snapshots": List[SnapshotRecycleBinInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LoadPermissionModificationsTypeDef = TypedDict(
     "LoadPermissionModificationsTypeDef",
     {
         "Add": NotRequired[Sequence[LoadPermissionRequestTypeDef]],
         "Remove": NotRequired[Sequence[LoadPermissionRequestTypeDef]],
@@ -16853,15 +16989,15 @@
         "CurrencyCode": NotRequired[Literal["USD"]],
         "InstanceTenancy": NotRequired[TenancyType],
         "Marketplace": NotRequired[bool],
         "OfferingClass": NotRequired[OfferingClassTypeType],
         "OfferingType": NotRequired[OfferingTypeValuesType],
         "PricingDetails": NotRequired[List[PricingDetailTypeDef]],
         "RecurringCharges": NotRequired[List[RecurringChargeTypeDef]],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
     },
 )
 ReservedInstancesTypeDef = TypedDict(
     "ReservedInstancesTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "Duration": NotRequired[int],
@@ -16875,15 +17011,15 @@
         "State": NotRequired[ReservedInstanceStateType],
         "UsagePrice": NotRequired[float],
         "CurrencyCode": NotRequired[Literal["USD"]],
         "InstanceTenancy": NotRequired[TenancyType],
         "OfferingClass": NotRequired[OfferingClassTypeType],
         "OfferingType": NotRequired[OfferingTypeValuesType],
         "RecurringCharges": NotRequired[List[RecurringChargeTypeDef]],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 SecurityGroupRuleTypeDef = TypedDict(
     "SecurityGroupRuleTypeDef",
     {
         "SecurityGroupRuleId": NotRequired[str],
@@ -16918,14 +17054,20 @@
 RegisterTransitGatewayMulticastGroupSourcesResultTypeDef = TypedDict(
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
     {
         "RegisteredMulticastGroupSources": TransitGatewayMulticastRegisteredGroupSourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StorageOutputTypeDef = TypedDict(
+    "StorageOutputTypeDef",
+    {
+        "S3": NotRequired[S3StorageOutputTypeDef],
+    },
+)
 ScheduledInstanceAvailabilityTypeDef = TypedDict(
     "ScheduledInstanceAvailabilityTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "AvailableInstanceCount": NotRequired[int],
         "FirstSlotStartTime": NotRequired[datetime],
         "HourlyPrice": NotRequired[str],
@@ -16988,16 +17130,16 @@
         "SubnetId": NotRequired[str],
     },
 )
 SearchTransitGatewayMulticastGroupsResultTypeDef = TypedDict(
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     {
         "MulticastGroups": List[TransitGatewayMulticastGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": NotRequired[str],
         "VpcEndpointType": NotRequired[VpcEndpointTypeType],
@@ -17146,18 +17288,30 @@
 TargetReservationValueTypeDef = TypedDict(
     "TargetReservationValueTypeDef",
     {
         "ReservationValue": NotRequired[ReservationValueTypeDef],
         "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
     },
 )
+TargetGroupsConfigExtraOutputTypeDef = TypedDict(
+    "TargetGroupsConfigExtraOutputTypeDef",
+    {
+        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+    },
+)
+TargetGroupsConfigOutputTypeDef = TypedDict(
+    "TargetGroupsConfigOutputTypeDef",
+    {
+        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+    },
+)
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
-        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+        "TargetGroups": NotRequired[Sequence[TargetGroupTypeDef]],
     },
 )
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
         "TrafficMirrorFilterRuleId": NotRequired[str],
         "TrafficMirrorFilterId": NotRequired[str],
@@ -17507,16 +17661,16 @@
         "LoadBalancers": NotRequired[List[AnalysisComponentTypeDef]],
     },
 )
 DescribeAddressesAttributeResultTypeDef = TypedDict(
     "DescribeAddressesAttributeResultTypeDef",
     {
         "Addresses": List[AddressAttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyAddressAttributeResultTypeDef = TypedDict(
     "ModifyAddressAttributeResultTypeDef",
     {
         "Address": AddressAttributeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17536,16 +17690,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointServicePermissionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
     {
         "AllowedPrincipals": List[AllowedPrincipalTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCarrierGatewayResultTypeDef = TypedDict(
     "CreateCarrierGatewayResultTypeDef",
     {
         "CarrierGateway": CarrierGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17558,16 +17712,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCarrierGatewaysResultTypeDef = TypedDict(
     "DescribeCarrierGatewaysResultTypeDef",
     {
         "CarrierGateways": List[CarrierGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCoipPoolResultTypeDef = TypedDict(
     "CreateCoipPoolResultTypeDef",
     {
         "CoipPool": CoipPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17580,16 +17734,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCoipPoolsResultTypeDef = TypedDict(
     "DescribeCoipPoolsResultTypeDef",
     {
         "CoipPools": List[CoipPoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCustomerGatewayResultTypeDef = TypedDict(
     "CreateCustomerGatewayResultTypeDef",
     {
         "CustomerGateway": CustomerGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17617,24 +17771,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInstanceConnectEndpointsResultTypeDef = TypedDict(
     "DescribeInstanceConnectEndpointsResultTypeDef",
     {
         "InstanceConnectEndpoints": List[Ec2InstanceConnectEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostReservationsResultTypeDef = TypedDict(
     "DescribeHostReservationsResultTypeDef",
     {
         "HostReservationSet": List[HostReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "AssociateInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "AssociationTarget": InstanceEventWindowAssociationRequestTypeDef,
@@ -17668,16 +17822,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamResourceDiscoveryAssociationsResultTypeDef = TypedDict(
     "DescribeIpamResourceDiscoveryAssociationsResultTypeDef",
     {
         "IpamResourceDiscoveryAssociations": List[IpamResourceDiscoveryAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateIpamResourceDiscoveryResultTypeDef = TypedDict(
     "DisassociateIpamResourceDiscoveryResultTypeDef",
     {
         "IpamResourceDiscoveryAssociation": IpamResourceDiscoveryAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17696,17 +17850,17 @@
         "IpamScope": IpamScopeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamScopesResultTypeDef = TypedDict(
     "DescribeIpamScopesResultTypeDef",
     {
-        "NextToken": str,
         "IpamScopes": List[IpamScopeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamScopeResultTypeDef = TypedDict(
     "ModifyIpamScopeResultTypeDef",
     {
         "IpamScope": IpamScopeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17726,16 +17880,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLaunchTemplatesResultTypeDef = TypedDict(
     "DescribeLaunchTemplatesResultTypeDef",
     {
         "LaunchTemplates": List[LaunchTemplateTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyLaunchTemplateResultTypeDef = TypedDict(
     "ModifyLaunchTemplateResultTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17757,16 +17911,16 @@
 )
 DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef",
     {
         "LocalGatewayRouteTableVirtualInterfaceGroupAssociations": List[
             LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef
         ],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateLocalGatewayRouteTableVpcAssociationResultTypeDef = TypedDict(
     "CreateLocalGatewayRouteTableVpcAssociationResultTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociation": LocalGatewayRouteTableVpcAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17779,40 +17933,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociations": List[LocalGatewayRouteTableVpcAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewaysResultTypeDef = TypedDict(
     "DescribeLocalGatewaysResultTypeDef",
     {
         "LocalGateways": List[LocalGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef = TypedDict(
     "DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef",
     {
         "LocalGatewayVirtualInterfaceGroups": List[LocalGatewayVirtualInterfaceGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewayVirtualInterfacesResultTypeDef = TypedDict(
     "DescribeLocalGatewayVirtualInterfacesResultTypeDef",
     {
         "LocalGatewayVirtualInterfaces": List[LocalGatewayVirtualInterfaceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateManagedPrefixListResultTypeDef = TypedDict(
     "CreateManagedPrefixListResultTypeDef",
     {
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17824,17 +17978,17 @@
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeManagedPrefixListsResultTypeDef = TypedDict(
     "DescribeManagedPrefixListsResultTypeDef",
     {
-        "NextToken": str,
         "PrefixLists": List[ManagedPrefixListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyManagedPrefixListResultTypeDef = TypedDict(
     "ModifyManagedPrefixListResultTypeDef",
     {
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17847,31 +18001,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalyses": List[NetworkInsightsAccessScopeAnalysisTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartNetworkInsightsAccessScopeAnalysisResultTypeDef = TypedDict(
     "StartNetworkInsightsAccessScopeAnalysisResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysis": NetworkInsightsAccessScopeAnalysisTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsAccessScopesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAccessScopesResultTypeDef",
     {
         "NetworkInsightsAccessScopes": List[NetworkInsightsAccessScopeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreatePlacementGroupResultTypeDef = TypedDict(
     "CreatePlacementGroupResultTypeDef",
     {
         "PlacementGroup": PlacementGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17891,47 +18045,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeReplaceRootVolumeTasksResultTypeDef = TypedDict(
     "DescribeReplaceRootVolumeTasksResultTypeDef",
     {
         "ReplaceRootVolumeTasks": List[ReplaceRootVolumeTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetSecurityGroupsForVpcResultTypeDef = TypedDict(
     "GetSecurityGroupsForVpcResultTypeDef",
     {
-        "NextToken": str,
         "SecurityGroupForVpcs": List[SecurityGroupForVpcTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateSnapshotsResultTypeDef = TypedDict(
     "CreateSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSnapshotTierStatusResultTypeDef = TypedDict(
     "DescribeSnapshotTierStatusResultTypeDef",
     {
         "SnapshotTierStatuses": List[SnapshotTierStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateSubnetCidrReservationResultTypeDef = TypedDict(
     "CreateSubnetCidrReservationResultTypeDef",
     {
         "SubnetCidrReservation": SubnetCidrReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17945,93 +18099,16 @@
     },
 )
 GetSubnetCidrReservationsResultTypeDef = TypedDict(
     "GetSubnetCidrReservationsResultTypeDef",
     {
         "SubnetIpv4CidrReservations": List[SubnetCidrReservationTypeDef],
         "SubnetIpv6CidrReservations": List[SubnetCidrReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-AcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "AcceptAddressTransferRequestRequestTypeDef",
-    {
-        "Address": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-AllocateAddressRequestRequestTypeDef = TypedDict(
-    "AllocateAddressRequestRequestTypeDef",
-    {
-        "Domain": NotRequired[DomainTypeType],
-        "Address": NotRequired[str],
-        "PublicIpv4Pool": NotRequired[str],
-        "NetworkBorderGroup": NotRequired[str],
-        "CustomerOwnedIpv4Pool": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-AllocateHostsRequestRequestTypeDef = TypedDict(
-    "AllocateHostsRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "AutoPlacement": NotRequired[AutoPlacementType],
-        "ClientToken": NotRequired[str],
-        "InstanceType": NotRequired[str],
-        "InstanceFamily": NotRequired[str],
-        "Quantity": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "HostRecovery": NotRequired[HostRecoveryType],
-        "OutpostArn": NotRequired[str],
-        "HostMaintenance": NotRequired[HostMaintenanceType],
-        "AssetIds": NotRequired[Sequence[str]],
-    },
-)
-AssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "IpamResourceDiscoveryId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CopyImageRequestRequestTypeDef = TypedDict(
-    "CopyImageRequestRequestTypeDef",
-    {
-        "Name": str,
-        "SourceImageId": str,
-        "SourceRegion": str,
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "DestinationOutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "CopyImageTags": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CopySnapshotRequestRequestTypeDef = TypedDict(
-    "CopySnapshotRequestRequestTypeDef",
-    {
-        "SourceRegion": str,
-        "SourceSnapshotId": str,
-        "Description": NotRequired[str],
-        "DestinationOutpostArn": NotRequired[str],
-        "DestinationRegion": NotRequired[str],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "PresignedUrl": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
+        "NextToken": NotRequired[str],
     },
 )
 CopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
     "CopySnapshotRequestSnapshotCopyTypeDef",
     {
         "SourceRegion": str,
         "Description": NotRequired[str],
@@ -18040,383 +18117,22 @@
         "Encrypted": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "PresignedUrl": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
-        "TotalTargetCapacity": int,
-        "AllocationStrategy": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "Tenancy": NotRequired[Literal["default"]],
-        "EndDate": NotRequired[TimestampTypeDef],
-        "InstanceMatchCriteria": NotRequired[Literal["open"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "CreateCapacityReservationRequestRequestTypeDef",
-    {
-        "InstanceType": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "InstanceCount": int,
-        "ClientToken": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "Tenancy": NotRequired[CapacityReservationTenancyType],
-        "EbsOptimized": NotRequired[bool],
-        "EphemeralStorage": NotRequired[bool],
-        "EndDate": NotRequired[TimestampTypeDef],
-        "EndDateType": NotRequired[EndDateTypeType],
-        "InstanceMatchCriteria": NotRequired[InstanceMatchCriteriaType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "OutpostArn": NotRequired[str],
-        "PlacementGroupArn": NotRequired[str],
-    },
-)
-CreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "CreateCoipPoolRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-        "BgpAsn": NotRequired[int],
-        "PublicIp": NotRequired[str],
-        "CertificateArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DeviceName": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "CreateFlowLogsRequestRequestTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ResourceType": FlowLogsResourceTypeType,
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "DeliverLogsPermissionArn": NotRequired[str],
-        "DeliverCrossAccountRole": NotRequired[str],
-        "LogGroupName": NotRequired[str],
-        "TrafficType": NotRequired[TrafficTypeType],
-        "LogDestinationType": NotRequired[LogDestinationTypeType],
-        "LogDestination": NotRequired[str],
-        "LogFormat": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MaxAggregationInterval": NotRequired[int],
-        "DestinationOptions": NotRequired[DestinationOptionsRequestTypeDef],
-    },
-)
-CreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "CreateFpgaImageRequestRequestTypeDef",
-    {
-        "InputStorageLocation": StorageLocationTypeDef,
-        "DryRun": NotRequired[bool],
-        "LogsStorageLocation": NotRequired[StorageLocationTypeDef],
-        "Description": NotRequired[str],
-        "Name": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "DryRun": NotRequired[bool],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "PreserveClientIp": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Name": NotRequired[str],
-        "TimeRanges": NotRequired[Sequence[InstanceEventWindowTimeRangeRequestTypeDef]],
-        "CronExpression": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
-        "InstanceId": str,
-        "TargetEnvironment": ExportEnvironmentType,
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateInternetGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    {
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "CreateIpamPoolRequestRequestTypeDef",
-    {
-        "IpamScopeId": str,
-        "AddressFamily": AddressFamilyType,
-        "DryRun": NotRequired[bool],
-        "Locale": NotRequired[str],
-        "SourceIpamPoolId": NotRequired[str],
-        "Description": NotRequired[str],
-        "AutoImport": NotRequired[bool],
-        "PubliclyAdvertisable": NotRequired[bool],
-        "AllocationMinNetmaskLength": NotRequired[int],
-        "AllocationMaxNetmaskLength": NotRequired[int],
-        "AllocationDefaultNetmaskLength": NotRequired[int],
-        "AllocationResourceTags": NotRequired[Sequence[RequestIpamResourceTagTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "AwsService": NotRequired[Literal["ec2"]],
-        "PublicIpSource": NotRequired[IpamPoolPublicIpSourceType],
-        "SourceResource": NotRequired[IpamPoolSourceResourceRequestTypeDef],
-    },
-)
-CreateIpamRequestRequestTypeDef = TypedDict(
-    "CreateIpamRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "Tier": NotRequired[IpamTierType],
-    },
-)
-CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "CreateIpamScopeRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateKeyPairRequestRequestTypeDef = TypedDict(
-    "CreateKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "DryRun": NotRequired[bool],
-        "KeyType": NotRequired[KeyTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "KeyFormat": NotRequired[KeyFormatType],
-    },
-)
-CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "DryRun": NotRequired[bool],
-        "KeyType": NotRequired[KeyTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "KeyFormat": NotRequired[KeyFormatType],
-    },
-)
-CreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "LocalGatewayId": str,
-        "Mode": NotRequired[LocalGatewayRouteTableModeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayVirtualInterfaceGroupId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "PrefixListName": str,
-        "MaxEntries": int,
-        "AddressFamily": str,
-        "DryRun": NotRequired[bool],
-        "Entries": NotRequired[Sequence[AddPrefixListEntryTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "CreateNatGatewayRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "AllocationId": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ConnectivityType": NotRequired[ConnectivityTypeType],
-        "PrivateIpAddress": NotRequired[str],
-        "SecondaryAllocationIds": NotRequired[Sequence[str]],
-        "SecondaryPrivateIpAddresses": NotRequired[Sequence[str]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-    },
-)
-CreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "CreateNetworkAclRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
 CreateNetworkAclRequestVpcCreateNetworkAclTypeDef = TypedDict(
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
     {
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "ClientToken": NotRequired[str],
     },
 )
-CreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Groups": NotRequired[Sequence[str]],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
-        "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
-        "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
-        "Ipv6PrefixCount": NotRequired[int],
-        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "EnablePrimaryIpv6": NotRequired[bool],
-        "ConnectionTrackingSpecification": NotRequired[
-            ConnectionTrackingSpecificationRequestTypeDef
-        ],
-    },
-)
-CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "SubnetId": str,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Groups": NotRequired[Sequence[str]],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
-        "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
-        "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
-        "Ipv6PrefixCount": NotRequired[int],
-        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "EnablePrimaryIpv6": NotRequired[bool],
-        "ConnectionTrackingSpecification": NotRequired[
-            ConnectionTrackingSpecificationRequestTypeDef
-        ],
-    },
-)
 CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef = TypedDict(
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
     {
         "Description": NotRequired[str],
         "DryRun": NotRequired[bool],
         "Groups": NotRequired[Sequence[str]],
         "Ipv6AddressCount": NotRequired[int],
@@ -18433,207 +18149,40 @@
         "ClientToken": NotRequired[str],
         "EnablePrimaryIpv6": NotRequired[bool],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
 )
-CreatePlacementGroupRequestRequestTypeDef = TypedDict(
-    "CreatePlacementGroupRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupName": NotRequired[str],
-        "Strategy": NotRequired[PlacementStrategyType],
-        "PartitionCount": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SpreadLevel": NotRequired[SpreadLevelType],
-    },
-)
-CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupName": NotRequired[str],
-        "Strategy": NotRequired[PlacementStrategyType],
-        "PartitionCount": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SpreadLevel": NotRequired[SpreadLevelType],
-    },
-)
-CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ImageId": NotRequired[str],
-        "DeleteReplacedRootVolume": NotRequired[bool],
-    },
-)
-CreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "ObjectKey": str,
-        "Name": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateRouteTableRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
 CreateRouteTableRequestVpcCreateRouteTableTypeDef = TypedDict(
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
     {
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "ClientToken": NotRequired[str],
     },
 )
-CreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "CreateSecurityGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-        "VpcId": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-        "VpcId": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
 CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef = TypedDict(
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupName": str,
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateSnapshotRequestRequestTypeDef = TypedDict(
-    "CreateSnapshotRequestRequestTypeDef",
-    {
-        "VolumeId": str,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "VolumeId": str,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
 CreateSnapshotRequestVolumeCreateSnapshotTypeDef = TypedDict(
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
     {
         "Description": NotRequired[str],
         "OutpostArn": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "CreateSnapshotsRequestRequestTypeDef",
-    {
-        "InstanceSpecification": InstanceSpecificationTypeDef,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "CopyTagsFromSource": NotRequired[Literal["volume"]],
-    },
-)
-CreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Cidr": str,
-        "ReservationType": SubnetCidrReservationTypeType,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateSubnetRequestRequestTypeDef = TypedDict(
-    "CreateSubnetRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "CidrBlock": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Ipv6Native": NotRequired[bool],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-    },
-)
-CreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "CidrBlock": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Ipv6Native": NotRequired[bool],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-    },
-)
 CreateSubnetRequestVpcCreateSubnetTypeDef = TypedDict(
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
     {
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "AvailabilityZone": NotRequired[str],
         "AvailabilityZoneId": NotRequired[str],
         "CidrBlock": NotRequired[str],
@@ -18643,437 +18192,39 @@
         "Ipv6Native": NotRequired[bool],
         "Ipv4IpamPoolId": NotRequired[str],
         "Ipv4NetmaskLength": NotRequired[int],
         "Ipv6IpamPoolId": NotRequired[str],
         "Ipv6NetmaskLength": NotRequired[int],
     },
 )
-CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "TrafficMirrorTargetId": str,
-        "TrafficMirrorFilterId": str,
-        "SessionNumber": int,
-        "PacketLength": NotRequired[int],
-        "VirtualNetworkId": NotRequired[int],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": NotRequired[str],
-        "NetworkLoadBalancerArn": NotRequired[str],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "GatewayLoadBalancerEndpointId": NotRequired[str],
-    },
-)
-CreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAttachmentId": str,
-        "PeerAddress": str,
-        "InsideCidrBlocks": Sequence[str],
-        "TransitGatewayAddress": NotRequired[str],
-        "BgpOptions": NotRequired[TransitGatewayConnectRequestBgpOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TransportTransitGatewayAttachmentId": str,
-        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "Options": NotRequired[CreateTransitGatewayMulticastDomainRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "PeerTransitGatewayId": str,
-        "PeerAccountId": str,
-        "PeerRegion": str,
-        "Options": NotRequired[CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "Options": NotRequired[TransitGatewayRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TransitGatewayRouteTableId": str,
-        "PeeringAttachmentId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "VpcId": str,
-        "SubnetIds": Sequence[str],
-        "Options": NotRequired[CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "VerifiedAccessGroupId": str,
-        "EndpointType": VerifiedAccessEndpointTypeType,
-        "AttachmentType": Literal["vpc"],
-        "DomainCertificateArn": str,
-        "ApplicationDomain": str,
-        "EndpointDomainPrefix": str,
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "LoadBalancerOptions": NotRequired[CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef],
-        "NetworkInterfaceOptions": NotRequired[CreateVerifiedAccessEndpointEniOptionsTypeDef],
-        "Description": NotRequired[str],
-        "PolicyDocument": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "VerifiedAccessInstanceId": str,
-        "Description": NotRequired[str],
-        "PolicyDocument": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "FIPSEnabled": NotRequired[bool],
-    },
-)
-CreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "TrustProviderType": TrustProviderTypeType,
-        "PolicyReferenceName": str,
-        "UserTrustProviderType": NotRequired[UserTrustProviderTypeType],
-        "DeviceTrustProviderType": NotRequired[DeviceTrustProviderTypeType],
-        "OidcOptions": NotRequired[CreateVerifiedAccessTrustProviderOidcOptionsTypeDef],
-        "DeviceOptions": NotRequired[CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVolumeRequestRequestTypeDef = TypedDict(
-    "CreateVolumeRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "Encrypted": NotRequired[bool],
-        "Iops": NotRequired[int],
-        "KmsKeyId": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "Size": NotRequired[int],
-        "SnapshotId": NotRequired[str],
-        "VolumeType": NotRequired[VolumeTypeType],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiAttachEnabled": NotRequired[bool],
-        "Throughput": NotRequired[int],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "AvailabilityZone": str,
-        "Encrypted": NotRequired[bool],
-        "Iops": NotRequired[int],
-        "KmsKeyId": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "Size": NotRequired[int],
-        "SnapshotId": NotRequired[str],
-        "VolumeType": NotRequired[VolumeTypeType],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiAttachEnabled": NotRequired[bool],
-        "Throughput": NotRequired[int],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ServiceName": str,
-        "DryRun": NotRequired[bool],
-        "VpcEndpointType": NotRequired[VpcEndpointTypeType],
-        "PolicyDocument": NotRequired[str],
-        "RouteTableIds": NotRequired[Sequence[str]],
-        "SubnetIds": NotRequired[Sequence[str]],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "IpAddressType": NotRequired[IpAddressTypeType],
-        "DnsOptions": NotRequired[DnsOptionsSpecificationTypeDef],
-        "ClientToken": NotRequired[str],
-        "PrivateDnsEnabled": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SubnetConfigurations": NotRequired[Sequence[SubnetConfigurationTypeDef]],
-    },
-)
-CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "AcceptanceRequired": NotRequired[bool],
-        "PrivateDnsName": NotRequired[str],
-        "NetworkLoadBalancerArns": NotRequired[Sequence[str]],
-        "GatewayLoadBalancerArns": NotRequired[Sequence[str]],
-        "SupportedIpAddressTypes": NotRequired[Sequence[str]],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "PeerOwnerId": NotRequired[str],
-        "PeerVpcId": NotRequired[str],
-        "PeerRegion": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "PeerOwnerId": NotRequired[str],
-        "PeerVpcId": NotRequired[str],
-        "PeerRegion": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef = TypedDict(
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
     {
         "DryRun": NotRequired[bool],
         "PeerOwnerId": NotRequired[str],
         "PeerVpcId": NotRequired[str],
         "PeerRegion": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-CreateVpcRequestRequestTypeDef = TypedDict(
-    "CreateVpcRequestRequestTypeDef",
-    {
-        "CidrBlock": NotRequired[str],
-        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
-        "Ipv6Pool": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "InstanceTenancy": NotRequired[TenancyType],
-        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    {
-        "CidrBlock": NotRequired[str],
-        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
-        "Ipv6Pool": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "InstanceTenancy": NotRequired[TenancyType],
-        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "CreateVpnGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-        "AvailabilityZone": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AmazonSideAsn": NotRequired[int],
-        "DryRun": NotRequired[bool],
-    },
-)
-ExportImageRequestRequestTypeDef = TypedDict(
-    "ExportImageRequestRequestTypeDef",
-    {
-        "DiskImageFormat": DiskImageFormatType,
-        "ImageId": str,
-        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "RoleName": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ImportKeyPairRequestRequestTypeDef = TypedDict(
-    "ImportKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "Cidr": str,
-        "CidrAuthorizationContext": NotRequired[CidrAuthorizationContextTypeDef],
-        "PubliclyAdvertisable": NotRequired[bool],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "PoolTagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiRegion": NotRequired[bool],
-        "NetworkBorderGroup": NotRequired[str],
-    },
-)
-PurchaseCapacityBlockRequestRequestTypeDef = TypedDict(
-    "PurchaseCapacityBlockRequestRequestTypeDef",
-    {
-        "CapacityBlockOfferingId": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-PurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "PurchaseHostReservationRequestRequestTypeDef",
-    {
-        "HostIdSet": Sequence[str],
-        "OfferingId": str,
-        "ClientToken": NotRequired[str],
-        "CurrencyCode": NotRequired[Literal["USD"]],
-        "LimitPrice": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsAccessScopeId": str,
-        "ClientToken": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-StartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsPathId": str,
-        "ClientToken": str,
-        "AdditionalAccounts": NotRequired[Sequence[str]],
-        "FilterInArns": NotRequired[Sequence[str]],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
+TagSpecificationUnionTypeDef = Union[TagSpecificationTypeDef, TagSpecificationExtraOutputTypeDef]
 CreateTrafficMirrorSessionResultTypeDef = TypedDict(
     "CreateTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorSessionsResultTypeDef = TypedDict(
     "DescribeTrafficMirrorSessionsResultTypeDef",
     {
         "TrafficMirrorSessions": List[TrafficMirrorSessionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTrafficMirrorSessionResultTypeDef = TypedDict(
     "ModifyTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19087,16 +18238,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorTargetsResultTypeDef = TypedDict(
     "DescribeTrafficMirrorTargetsResultTypeDef",
     {
         "TrafficMirrorTargets": List[TrafficMirrorTargetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayPolicyTableResultTypeDef = TypedDict(
     "CreateTransitGatewayPolicyTableResultTypeDef",
     {
         "TransitGatewayPolicyTable": TransitGatewayPolicyTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19109,16 +18260,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayPolicyTablesResultTypeDef = TypedDict(
     "DescribeTransitGatewayPolicyTablesResultTypeDef",
     {
         "TransitGatewayPolicyTables": List[TransitGatewayPolicyTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayRouteTableAnnouncementResultTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableAnnouncementResultTypeDef",
     {
         "TransitGatewayRouteTableAnnouncement": TransitGatewayRouteTableAnnouncementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19131,16 +18282,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef = TypedDict(
     "DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef",
     {
         "TransitGatewayRouteTableAnnouncements": List[TransitGatewayRouteTableAnnouncementTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayRouteTableResultTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableResultTypeDef",
     {
         "TransitGatewayRouteTable": TransitGatewayRouteTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19153,32 +18304,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayRouteTablesResultTypeDef = TypedDict(
     "DescribeTransitGatewayRouteTablesResultTypeDef",
     {
         "TransitGatewayRouteTables": List[TransitGatewayRouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateTrunkInterfaceResultTypeDef = TypedDict(
     "AssociateTrunkInterfaceResultTypeDef",
     {
         "InterfaceAssociation": TrunkInterfaceAssociationTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrunkInterfaceAssociationsResultTypeDef = TypedDict(
     "DescribeTrunkInterfaceAssociationsResultTypeDef",
     {
         "InterfaceAssociations": List[TrunkInterfaceAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVpcClassicLinkResultTypeDef = TypedDict(
     "DescribeVpcClassicLinkResultTypeDef",
     {
         "Vpcs": List[VpcClassicLinkTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19256,16 +18407,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeByoipCidrsResultTypeDef = TypedDict(
     "DescribeByoipCidrsResultTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MoveByoipCidrToIpamResultTypeDef = TypedDict(
     "MoveByoipCidrToIpamResultTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19285,16 +18436,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClientVpnTargetNetworksResultTypeDef = TypedDict(
     "DescribeClientVpnTargetNetworksResultTypeDef",
     {
         "ClientVpnTargetNetworks": List[TargetNetworkTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RouteTableTypeDef = TypedDict(
     "RouteTableTypeDef",
     {
         "Associations": NotRequired[List[RouteTableAssociationTypeDef]],
         "PropagatingVgws": NotRequired[List[PropagatingVgwTypeDef]],
@@ -19423,16 +18574,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 DescribeClientVpnAuthorizationRulesResultTypeDef = TypedDict(
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     {
         "AuthorizationRules": List[AuthorizationRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAvailabilityZonesResultTypeDef = TypedDict(
     "DescribeAvailabilityZonesResultTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19476,26 +18627,14 @@
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "Description": NotRequired[str],
         "DryRun": NotRequired[bool],
         "NoReboot": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-CreateImageRequestRequestTypeDef = TypedDict(
-    "CreateImageRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "NoReboot": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 ImageAttributeTypeDef = TypedDict(
     "ImageAttributeTypeDef",
     {
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "ImageId": str,
         "LaunchPermissions": List[LaunchPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
@@ -19546,60 +18685,14 @@
         "DeprecationTime": NotRequired[str],
         "ImdsSupport": NotRequired[Literal["v2.0"]],
         "SourceInstanceId": NotRequired[str],
         "DeregistrationProtection": NotRequired[str],
         "LastLaunchedTime": NotRequired[str],
     },
 )
-RegisterImageRequestRequestTypeDef = TypedDict(
-    "RegisterImageRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ImageLocation": NotRequired[str],
-        "Architecture": NotRequired[ArchitectureValuesType],
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "EnaSupport": NotRequired[bool],
-        "KernelId": NotRequired[str],
-        "BillingProducts": NotRequired[Sequence[str]],
-        "RamdiskId": NotRequired[str],
-        "RootDeviceName": NotRequired[str],
-        "SriovNetSupport": NotRequired[str],
-        "VirtualizationType": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-        "TpmSupport": NotRequired[Literal["v2.0"]],
-        "UefiData": NotRequired[str],
-        "ImdsSupport": NotRequired[Literal["v2.0"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-RegisterImageRequestServiceResourceRegisterImageTypeDef = TypedDict(
-    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
-    {
-        "Name": str,
-        "ImageLocation": NotRequired[str],
-        "Architecture": NotRequired[ArchitectureValuesType],
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "EnaSupport": NotRequired[bool],
-        "KernelId": NotRequired[str],
-        "BillingProducts": NotRequired[Sequence[str]],
-        "RamdiskId": NotRequired[str],
-        "RootDeviceName": NotRequired[str],
-        "SriovNetSupport": NotRequired[str],
-        "VirtualizationType": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-        "TpmSupport": NotRequired[Literal["v2.0"]],
-        "UefiData": NotRequired[str],
-        "ImdsSupport": NotRequired[Literal["v2.0"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CancelCapacityReservationFleetsResultTypeDef = TypedDict(
     "CancelCapacityReservationFleetsResultTypeDef",
     {
         "SuccessfulFleetCancellations": List[CapacityReservationFleetCancellationStateTypeDef],
         "FailedFleetCancellations": List[FailedCapacityReservationFleetCancellationResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -19618,71 +18711,48 @@
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCapacityReservationsResultTypeDef = TypedDict(
     "DescribeCapacityReservationsResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseCapacityBlockResultTypeDef = TypedDict(
     "PurchaseCapacityBlockResultTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCapacityReservationFleetsResultTypeDef = TypedDict(
     "DescribeCapacityReservationFleetsResultTypeDef",
     {
         "CapacityReservationFleets": List[CapacityReservationFleetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef = TypedDict(
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
 DescribeClassicLinkInstancesResultTypeDef = TypedDict(
     "DescribeClassicLinkInstancesResultTypeDef",
     {
         "Instances": List[ClassicLinkInstanceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "CreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "ClientCidrBlock": str,
-        "ServerCertificateArn": str,
-        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
-        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
-        "DnsServers": NotRequired[Sequence[str]],
-        "TransportProtocol": NotRequired[TransportProtocolType],
-        "VpnPort": NotRequired[int],
-        "Description": NotRequired[str],
-        "SplitTunnel": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "VpcId": NotRequired[str],
-        "SelfServicePortal": NotRequired[SelfServicePortalType],
-        "ClientConnectOptions": NotRequired[ClientConnectOptionsTypeDef],
-        "SessionTimeoutHours": NotRequired[int],
-        "ClientLoginBannerOptions": NotRequired[ClientLoginBannerOptionsTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 ClientVpnEndpointTypeDef = TypedDict(
     "ClientVpnEndpointTypeDef",
     {
         "ClientVpnEndpointId": NotRequired[str],
         "Description": NotRequired[str],
@@ -19709,16 +18779,16 @@
         "ClientLoginBannerOptions": NotRequired[ClientLoginBannerResponseOptionsTypeDef],
     },
 )
 DescribeClientVpnConnectionsResultTypeDef = TypedDict(
     "DescribeClientVpnConnectionsResultTypeDef",
     {
         "Connections": List[ClientVpnConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TerminateClientVpnConnectionsResultTypeDef = TypedDict(
     "TerminateClientVpnConnectionsResultTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Username": str,
@@ -19726,16 +18796,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClientVpnRoutesResultTypeDef = TypedDict(
     "DescribeClientVpnRoutesResultTypeDef",
     {
         "Routes": List[ClientVpnRouteTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpnTunnelOptionsSpecificationTypeDef = TypedDict(
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     {
         "TunnelInsideCidr": NotRequired[str],
         "TunnelInsideIpv6Cidr": NotRequired[str],
@@ -19861,16 +18931,16 @@
         "DryRun": NotRequired[bool],
     },
 )
 GetAwsNetworkPerformanceDataResultTypeDef = TypedDict(
     "GetAwsNetworkPerformanceDataResultTypeDef",
     {
         "DataResponses": List[DataResponseTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DeleteFleetsResultTypeDef = TypedDict(
     "DeleteFleetsResultTypeDef",
     {
         "SuccessfulFleetDeletions": List[DeleteFleetSuccessItemTypeDef],
         "UnsuccessfulFleetDeletions": List[DeleteFleetErrorItemTypeDef],
@@ -19897,32 +18967,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePrincipalIdFormatResultTypeDef = TypedDict(
     "DescribePrincipalIdFormatResultTypeDef",
     {
         "Principals": List[PrincipalIdFormatTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFastLaunchImagesResultTypeDef = TypedDict(
     "DescribeFastLaunchImagesResultTypeDef",
     {
         "FastLaunchImages": List[DescribeFastLaunchImagesSuccessItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFlowLogsResultTypeDef = TypedDict(
     "DescribeFlowLogsResultTypeDef",
     {
         "FlowLogs": List[FlowLogTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": NotRequired[str],
         "FastSnapshotRestoreStateErrors": NotRequired[
@@ -19939,16 +19009,16 @@
         "Volumes": NotRequired[List[ImportInstanceVolumeDetailItemTypeDef]],
     },
 )
 DescribeVpcEndpointConnectionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionsResultTypeDef",
     {
         "VpcEndpointConnections": List[VpcEndpointConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceAttributeRequestInstanceModifyAttributeTypeDef = TypedDict(
     "ModifyInstanceAttributeRequestInstanceModifyAttributeTypeDef",
     {
         "SourceDestCheck": NotRequired[AttributeBooleanValueTypeDef],
         "Attribute": NotRequired[InstanceAttributeNameType],
@@ -20025,92 +19095,92 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeEgressOnlyInternetGatewaysResultTypeDef = TypedDict(
     "DescribeEgressOnlyInternetGatewaysResultTypeDef",
     {
         "EgressOnlyInternetGateways": List[EgressOnlyInternetGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateInternetGatewayResultTypeDef = TypedDict(
     "CreateInternetGatewayResultTypeDef",
     {
         "InternetGateway": InternetGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInternetGatewaysResultTypeDef = TypedDict(
     "DescribeInternetGatewaysResultTypeDef",
     {
         "InternetGateways": List[InternetGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeElasticGpusResultTypeDef = TypedDict(
     "DescribeElasticGpusResultTypeDef",
     {
         "ElasticGpuSet": List[ElasticGpusTypeDef],
         "MaxResults": int,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-InstanceNetworkInterfaceSpecificationServiceResourceTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
+InstanceNetworkInterfaceSpecificationExtraOutputTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationExtraOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[Sequence[str]],
+        "Groups": NotRequired[List[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
 )
-InstanceNetworkInterfaceSpecificationSubnetTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
+InstanceNetworkInterfaceSpecificationOutputTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[Sequence[str]],
+        "Groups": NotRequired[List[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
@@ -20118,28 +19188,28 @@
 InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "InstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[List[str]],
+        "Groups": NotRequired[Sequence[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
@@ -20237,37 +19307,37 @@
     },
 )
 DescribeFleetHistoryResultTypeDef = TypedDict(
     "DescribeFleetHistoryResultTypeDef",
     {
         "HistoryRecords": List[HistoryRecordEntryTypeDef],
         "LastEvaluatedTime": datetime,
-        "NextToken": str,
         "FleetId": str,
         "StartTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetRequestHistoryResponseTypeDef = TypedDict(
     "DescribeSpotFleetRequestHistoryResponseTypeDef",
     {
         "HistoryRecords": List[HistoryRecordTypeDef],
         "LastEvaluatedTime": datetime,
-        "NextToken": str,
         "SpotFleetRequestId": str,
         "StartTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeExportImageTasksResultTypeDef = TypedDict(
     "DescribeExportImageTasksResultTypeDef",
     {
         "ExportImageTasks": List[ExportImageTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateInstanceExportTaskResultTypeDef = TypedDict(
     "CreateInstanceExportTaskResultTypeDef",
     {
         "ExportTask": ExportTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20346,16 +19416,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeFpgaImagesResultTypeDef = TypedDict(
     "DescribeFpgaImagesResultTypeDef",
     {
         "FpgaImages": List[FpgaImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GpuInfoTypeDef = TypedDict(
     "GpuInfoTypeDef",
     {
         "Gpus": NotRequired[List[GpuDeviceInfoTypeDef]],
         "TotalGpuMemoryInMiB": NotRequired[int],
@@ -20368,16 +19438,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIamInstanceProfileAssociationsResultTypeDef = TypedDict(
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     {
         "IamInstanceProfileAssociations": List[IamInstanceProfileAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateIamInstanceProfileResultTypeDef = TypedDict(
     "DisassociateIamInstanceProfileResultTypeDef",
     {
         "IamInstanceProfileAssociation": IamInstanceProfileAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20421,51 +19491,14 @@
         "Value": NotRequired[str],
         "DryRun": NotRequired[bool],
         "OrganizationArns": NotRequired[Sequence[str]],
         "OrganizationalUnitArns": NotRequired[Sequence[str]],
         "ImdsSupport": NotRequired[AttributeValueTypeDef],
     },
 )
-ImportImageRequestRequestTypeDef = TypedDict(
-    "ImportImageRequestRequestTypeDef",
-    {
-        "Architecture": NotRequired[str],
-        "ClientData": NotRequired[ClientDataTypeDef],
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DiskContainers": NotRequired[Sequence[ImageDiskContainerTypeDef]],
-        "DryRun": NotRequired[bool],
-        "Encrypted": NotRequired[bool],
-        "Hypervisor": NotRequired[str],
-        "KmsKeyId": NotRequired[str],
-        "LicenseType": NotRequired[str],
-        "Platform": NotRequired[str],
-        "RoleName": NotRequired[str],
-        "LicenseSpecifications": NotRequired[
-            Sequence[ImportImageLicenseConfigurationRequestTypeDef]
-        ],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "UsageOperation": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-    },
-)
-ImportSnapshotRequestRequestTypeDef = TypedDict(
-    "ImportSnapshotRequestRequestTypeDef",
-    {
-        "ClientData": NotRequired[ClientDataTypeDef],
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DiskContainer": NotRequired[SnapshotDiskContainerTypeDef],
-        "DryRun": NotRequired[bool],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "RoleName": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
     "CreateLocalGatewayRouteTableResultTypeDef",
     {
         "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -20476,16 +19509,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTablesResultTypeDef",
     {
         "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportInstanceRequestRequestTypeDef = TypedDict(
     "ImportInstanceRequestRequestTypeDef",
     {
         "Platform": Literal["windows"],
         "Description": NotRequired[str],
@@ -20523,14 +19556,64 @@
 UnmonitorInstancesResultTypeDef = TypedDict(
     "UnmonitorInstancesResultTypeDef",
     {
         "InstanceMonitorings": List[InstanceMonitoringTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LaunchTemplateOverridesExtraOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesExtraOutputTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsExtraOutputTypeDef],
+    },
+)
+FleetLaunchTemplateOverridesTypeDef = TypedDict(
+    "FleetLaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "MaxPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "Placement": NotRequired[PlacementResponseTypeDef],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
+        "ImageId": NotRequired[str],
+    },
+)
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
+    },
+)
+LaunchTemplateOverridesTypeDef = TypedDict(
+    "LaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
+    },
+)
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": NotRequired[InstanceTypeType],
         "MaxPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "AvailabilityZone": NotRequired[str],
@@ -20566,40 +19649,14 @@
     "InstanceRequirementsWithMetadataRequestTypeDef",
     {
         "ArchitectureTypes": NotRequired[Sequence[ArchitectureTypeType]],
         "VirtualizationTypes": NotRequired[Sequence[VirtualizationTypeType]],
         "InstanceRequirements": NotRequired[InstanceRequirementsRequestTypeDef],
     },
 )
-FleetLaunchTemplateOverridesTypeDef = TypedDict(
-    "FleetLaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": NotRequired[InstanceTypeType],
-        "MaxPrice": NotRequired[str],
-        "SubnetId": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "WeightedCapacity": NotRequired[float],
-        "Priority": NotRequired[float],
-        "Placement": NotRequired[PlacementResponseTypeDef],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
-        "ImageId": NotRequired[str],
-    },
-)
-LaunchTemplateOverridesTypeDef = TypedDict(
-    "LaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": NotRequired[InstanceTypeType],
-        "SpotPrice": NotRequired[str],
-        "SubnetId": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "WeightedCapacity": NotRequired[float],
-        "Priority": NotRequired[float],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
-    },
-)
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -20625,72 +19682,57 @@
         "Events": NotRequired[List[InstanceStatusEventTypeDef]],
         "InstanceId": NotRequired[str],
         "InstanceState": NotRequired[InstanceStateTypeDef],
         "InstanceStatus": NotRequired[InstanceStatusSummaryTypeDef],
         "SystemStatus": NotRequired[InstanceStatusSummaryTypeDef],
     },
 )
-SecurityGroupPaginatorTypeDef = TypedDict(
-    "SecurityGroupPaginatorTypeDef",
+RevokeSecurityGroupEgressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+RevokeSecurityGroupIngressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SecurityGroupTypeDef = TypedDict(
+    "SecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
         "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[List[IpPermissionPaginatorTypeDef]],
+        "IpPermissions": NotRequired[List[IpPermissionOutputTypeDef]],
         "OwnerId": NotRequired[str],
         "GroupId": NotRequired[str],
-        "IpPermissionsEgress": NotRequired[List[IpPermissionPaginatorTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[IpPermissionOutputTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
-AuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-        "DryRun": NotRequired[bool],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "IpProtocol": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-    },
-)
 AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef = TypedDict(
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
     {
         "DryRun": NotRequired[bool],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "ToPort": NotRequired[int],
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
-    {
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "IpProtocol": NotRequired[str],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef = TypedDict(
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
     {
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "GroupName": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
@@ -20698,67 +19740,29 @@
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
         "ToPort": NotRequired[int],
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-RevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-        "DryRun": NotRequired[bool],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "IpProtocol": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-    },
-)
+IpPermissionUnionTypeDef = Union[IpPermissionTypeDef, IpPermissionExtraExtraOutputTypeDef]
 RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef = TypedDict(
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
     {
         "DryRun": NotRequired[bool],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
         "SecurityGroupRuleIds": NotRequired[Sequence[str]],
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "ToPort": NotRequired[int],
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-RevokeSecurityGroupEgressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
-    {
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "IpProtocol": NotRequired[str],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
-    },
-)
 RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef = TypedDict(
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
     {
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "GroupName": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
@@ -20766,55 +19770,14 @@
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
         "ToPort": NotRequired[int],
         "DryRun": NotRequired[bool],
         "SecurityGroupRuleIds": NotRequired[Sequence[str]],
     },
 )
-RevokeSecurityGroupIngressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-SecurityGroupTypeDef = TypedDict(
-    "SecurityGroupTypeDef",
-    {
-        "Description": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[List[IpPermissionTypeDef]],
-        "OwnerId": NotRequired[str],
-        "GroupId": NotRequired[str],
-        "IpPermissionsEgress": NotRequired[List[IpPermissionTypeDef]],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "VpcId": NotRequired[str],
-    },
-)
-UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
-    },
-)
-UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
-    },
-)
 StaleSecurityGroupTypeDef = TypedDict(
     "StaleSecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "StaleIpPermissions": NotRequired[List[StaleIpPermissionTypeDef]],
@@ -20822,32 +19785,32 @@
         "VpcId": NotRequired[str],
     },
 )
 GetIpamDiscoveredAccountsResultTypeDef = TypedDict(
     "GetIpamDiscoveredAccountsResultTypeDef",
     {
         "IpamDiscoveredAccounts": List[IpamDiscoveredAccountTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamDiscoveredResourceCidrsResultTypeDef = TypedDict(
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     {
         "IpamDiscoveredResourceCidrs": List[IpamDiscoveredResourceCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamResourceCidrsResultTypeDef = TypedDict(
     "GetIpamResourceCidrsResultTypeDef",
     {
-        "NextToken": str,
         "IpamResourceCidrs": List[IpamResourceCidrTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResourceCidrResultTypeDef = TypedDict(
     "ModifyIpamResourceCidrResultTypeDef",
     {
         "IpamResourceCidr": IpamResourceCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20867,16 +19830,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamResourceDiscoveriesResultTypeDef = TypedDict(
     "DescribeIpamResourceDiscoveriesResultTypeDef",
     {
         "IpamResourceDiscoveries": List[IpamResourceDiscoveryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResourceDiscoveryResultTypeDef = TypedDict(
     "ModifyIpamResourceDiscoveryResultTypeDef",
     {
         "IpamResourceDiscovery": IpamResourceDiscoveryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20895,17 +19858,17 @@
         "Ipam": IpamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamsResultTypeDef = TypedDict(
     "DescribeIpamsResultTypeDef",
     {
-        "NextToken": str,
         "Ipams": List[IpamTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResultTypeDef = TypedDict(
     "ModifyIpamResultTypeDef",
     {
         "Ipam": IpamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20918,16 +19881,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetIpamPoolCidrsResultTypeDef = TypedDict(
     "GetIpamPoolCidrsResultTypeDef",
     {
         "IpamPoolCidrs": List[IpamPoolCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ProvisionIpamPoolCidrResultTypeDef = TypedDict(
     "ProvisionIpamPoolCidrResultTypeDef",
     {
         "IpamPoolCidr": IpamPoolCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20946,17 +19909,17 @@
         "IpamPool": IpamPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamPoolsResultTypeDef = TypedDict(
     "DescribeIpamPoolsResultTypeDef",
     {
-        "NextToken": str,
         "IpamPools": List[IpamPoolTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamPoolResultTypeDef = TypedDict(
     "ModifyIpamPoolResultTypeDef",
     {
         "IpamPool": IpamPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20986,16 +19949,16 @@
         "SampleTime": NotRequired[datetime],
     },
 )
 DescribeIpv6PoolsResultTypeDef = TypedDict(
     "DescribeIpv6PoolsResultTypeDef",
     {
         "Ipv6Pools": List[Ipv6PoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociateCarrierIpAddress": NotRequired[bool],
         "AssociatePublicIpAddress": NotRequired[bool],
@@ -21071,16 +20034,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessGroupsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessGroupsResultTypeDef",
     {
         "VerifiedAccessGroups": List[VerifiedAccessGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessGroupResultTypeDef = TypedDict(
     "ModifyVerifiedAccessGroupResultTypeDef",
     {
         "VerifiedAccessGroup": VerifiedAccessGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21094,31 +20057,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNatGatewaysResultTypeDef = TypedDict(
     "DescribeNatGatewaysResultTypeDef",
     {
         "NatGateways": List[NatGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkInterfacePermissionResultTypeDef = TypedDict(
     "CreateNetworkInterfacePermissionResultTypeDef",
     {
         "InterfacePermission": NetworkInterfacePermissionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInterfacePermissionsResultTypeDef = TypedDict(
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     {
         "NetworkInterfacePermissions": List[NetworkInterfacePermissionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NeuronInfoTypeDef = TypedDict(
     "NeuronInfoTypeDef",
     {
         "NeuronDevices": NotRequired[List[NeuronDeviceInfoTypeDef]],
         "TotalNeuronDeviceMemoryInMiB": NotRequired[int],
@@ -21138,41 +20101,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessTrustProvidersResultTypeDef = TypedDict(
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     {
         "VerifiedAccessTrustProviders": List[VerifiedAccessTrustProviderTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessTrustProviderResultTypeDef = TypedDict(
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "Source": str,
-        "Protocol": ProtocolType,
-        "ClientToken": str,
-        "SourceIp": NotRequired[str],
-        "DestinationIp": NotRequired[str],
-        "Destination": NotRequired[str],
-        "DestinationPort": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "FilterAtSource": NotRequired[PathRequestFilterTypeDef],
-        "FilterAtDestination": NotRequired[PathRequestFilterTypeDef],
-    },
-)
 AccessScopePathRequestTypeDef = TypedDict(
     "AccessScopePathRequestTypeDef",
     {
         "Source": NotRequired[PathStatementRequestTypeDef],
         "Destination": NotRequired[PathStatementRequestTypeDef],
         "ThroughResources": NotRequired[Sequence[ThroughResourcesStatementRequestTypeDef]],
     },
@@ -21206,24 +20153,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePublicIpv4PoolsResultTypeDef = TypedDict(
     "DescribePublicIpv4PoolsResultTypeDef",
     {
         "PublicIpv4Pools": List[PublicIpv4PoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesOfferingsResultTypeDef = TypedDict(
     "DescribeReservedInstancesOfferingsResultTypeDef",
     {
         "ReservedInstancesOfferings": List[ReservedInstancesOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesResultTypeDef = TypedDict(
     "DescribeReservedInstancesResultTypeDef",
     {
         "ReservedInstances": List[ReservedInstancesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21245,32 +20192,45 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSecurityGroupRulesResultTypeDef = TypedDict(
     "DescribeSecurityGroupRulesResultTypeDef",
     {
         "SecurityGroupRules": List[SecurityGroupRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BundleTaskTypeDef = TypedDict(
+    "BundleTaskTypeDef",
+    {
+        "BundleId": NotRequired[str],
+        "BundleTaskError": NotRequired[BundleTaskErrorTypeDef],
+        "InstanceId": NotRequired[str],
+        "Progress": NotRequired[str],
+        "StartTime": NotRequired[datetime],
+        "State": NotRequired[BundleTaskStateType],
+        "Storage": NotRequired[StorageOutputTypeDef],
+        "UpdateTime": NotRequired[datetime],
     },
 )
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
-        "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeScheduledInstancesResultTypeDef = TypedDict(
     "DescribeScheduledInstancesResultTypeDef",
     {
-        "NextToken": str,
         "ScheduledInstanceSet": List[ScheduledInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseScheduledInstancesResultTypeDef = TypedDict(
     "PurchaseScheduledInstancesResultTypeDef",
     {
         "ScheduledInstanceSet": List[ScheduledInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21303,16 +20263,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointsResultTypeDef = TypedDict(
     "DescribeVpcEndpointsResultTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifySecurityGroupRulesRequestRequestTypeDef = TypedDict(
     "ModifySecurityGroupRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "SecurityGroupRules": Sequence[SecurityGroupRuleUpdateTypeDef],
@@ -21327,25 +20287,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointServiceConfigurationsResultTypeDef = TypedDict(
     "DescribeVpcEndpointServiceConfigurationsResultTypeDef",
     {
         "ServiceConfigurations": List[ServiceConfigurationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVpcEndpointServicesResultTypeDef = TypedDict(
     "DescribeVpcEndpointServicesResultTypeDef",
     {
         "ServiceNames": List[str],
         "ServiceDetails": List[ServiceDetailTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportImageResultTypeDef = TypedDict(
     "ImportImageResultTypeDef",
     {
         "Architecture": str,
         "Description": str,
@@ -21421,16 +20381,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayMulticastDomainAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayMulticastDomainAssociationsResultTypeDef",
     {
         "MulticastDomainAssociations": List[TransitGatewayMulticastDomainAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptTransitGatewayMulticastDomainAssociationsResultTypeDef = TypedDict(
     "AcceptTransitGatewayMulticastDomainAssociationsResultTypeDef",
     {
         "Associations": TransitGatewayMulticastDomainAssociationsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21510,14 +20470,28 @@
         "ReservedInstanceValueSet": List[ReservedInstanceReservationValueTypeDef],
         "TargetConfigurationValueRollup": ReservationValueTypeDef,
         "TargetConfigurationValueSet": List[TargetReservationValueTypeDef],
         "ValidationFailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LoadBalancersConfigExtraOutputTypeDef = TypedDict(
+    "LoadBalancersConfigExtraOutputTypeDef",
+    {
+        "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigExtraOutputTypeDef],
+        "TargetGroupsConfig": NotRequired[TargetGroupsConfigExtraOutputTypeDef],
+    },
+)
+LoadBalancersConfigOutputTypeDef = TypedDict(
+    "LoadBalancersConfigOutputTypeDef",
+    {
+        "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigOutputTypeDef],
+        "TargetGroupsConfig": NotRequired[TargetGroupsConfigOutputTypeDef],
+    },
+)
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigTypeDef],
         "TargetGroupsConfig": NotRequired[TargetGroupsConfigTypeDef],
     },
 )
@@ -21547,16 +20521,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 DescribeTransitGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     {
         "TransitGatewayAttachments": List[TransitGatewayAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TransitGatewayConnectPeerTypeDef = TypedDict(
     "TransitGatewayConnectPeerTypeDef",
     {
         "TransitGatewayAttachmentId": NotRequired[str],
         "TransitGatewayConnectPeerId": NotRequired[str],
@@ -21580,16 +20554,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayConnectsResultTypeDef = TypedDict(
     "DescribeTransitGatewayConnectsResultTypeDef",
     {
         "TransitGatewayConnects": List[TransitGatewayConnectTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayMulticastDomainResultTypeDef = TypedDict(
     "CreateTransitGatewayMulticastDomainResultTypeDef",
     {
         "TransitGatewayMulticastDomain": TransitGatewayMulticastDomainTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21602,16 +20576,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayMulticastDomainsResultTypeDef = TypedDict(
     "DescribeTransitGatewayMulticastDomainsResultTypeDef",
     {
         "TransitGatewayMulticastDomains": List[TransitGatewayMulticastDomainTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayResultTypeDef = TypedDict(
     "CreateTransitGatewayResultTypeDef",
     {
         "TransitGateway": TransitGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21624,16 +20598,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewaysResultTypeDef = TypedDict(
     "DescribeTransitGatewaysResultTypeDef",
     {
         "TransitGateways": List[TransitGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayResultTypeDef = TypedDict(
     "ModifyTransitGatewayResultTypeDef",
     {
         "TransitGateway": TransitGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21660,16 +20634,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayPeeringAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayPeeringAttachmentsResultTypeDef",
     {
         "TransitGatewayPeeringAttachments": List[TransitGatewayPeeringAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RejectTransitGatewayPeeringAttachmentResultTypeDef = TypedDict(
     "RejectTransitGatewayPeeringAttachmentResultTypeDef",
     {
         "TransitGatewayPeeringAttachment": TransitGatewayPeeringAttachmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21697,16 +20671,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayPrefixListReferencesResultTypeDef = TypedDict(
     "GetTransitGatewayPrefixListReferencesResultTypeDef",
     {
         "TransitGatewayPrefixListReferences": List[TransitGatewayPrefixListReferenceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayPrefixListReferenceResultTypeDef = TypedDict(
     "ModifyTransitGatewayPrefixListReferenceResultTypeDef",
     {
         "TransitGatewayPrefixListReference": TransitGatewayPrefixListReferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21762,16 +20736,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayVpcAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayVpcAttachmentsResultTypeDef",
     {
         "TransitGatewayVpcAttachments": List[TransitGatewayVpcAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayVpcAttachmentResultTypeDef = TypedDict(
     "ModifyTransitGatewayVpcAttachmentResultTypeDef",
     {
         "TransitGatewayVpcAttachment": TransitGatewayVpcAttachmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21885,16 +20859,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessEndpointsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessEndpointsResultTypeDef",
     {
         "VerifiedAccessEndpoints": List[VerifiedAccessEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessEndpointResultTypeDef = TypedDict(
     "ModifyVerifiedAccessEndpointResultTypeDef",
     {
         "VerifiedAccessEndpoint": VerifiedAccessEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21922,16 +20896,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessInstancesResultTypeDef = TypedDict(
     "DescribeVerifiedAccessInstancesResultTypeDef",
     {
         "VerifiedAccessInstances": List[VerifiedAccessInstanceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DetachVerifiedAccessTrustProviderResultTypeDef = TypedDict(
     "DetachVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "VerifiedAccessInstance": VerifiedAccessInstanceTypeDef,
@@ -21964,16 +20938,16 @@
         "ClientToken": NotRequired[str],
     },
 )
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VolumeStatusItemTypeDef = TypedDict(
     "VolumeStatusItemTypeDef",
     {
         "Actions": NotRequired[List[VolumeStatusActionTypeDef]],
         "AvailabilityZone": NotRequired[str],
@@ -22042,16 +21016,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInstanceEventWindowsResultTypeDef = TypedDict(
     "DescribeInstanceEventWindowsResultTypeDef",
     {
         "InstanceEventWindows": List[InstanceEventWindowTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateInstanceEventWindowResultTypeDef = TypedDict(
     "DisassociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22060,14 +21034,1152 @@
 ModifyInstanceEventWindowResultTypeDef = TypedDict(
     "ModifyInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "AcceptAddressTransferRequestRequestTypeDef",
+    {
+        "Address": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+AllocateAddressRequestRequestTypeDef = TypedDict(
+    "AllocateAddressRequestRequestTypeDef",
+    {
+        "Domain": NotRequired[DomainTypeType],
+        "Address": NotRequired[str],
+        "PublicIpv4Pool": NotRequired[str],
+        "NetworkBorderGroup": NotRequired[str],
+        "CustomerOwnedIpv4Pool": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+AllocateHostsRequestRequestTypeDef = TypedDict(
+    "AllocateHostsRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "AutoPlacement": NotRequired[AutoPlacementType],
+        "ClientToken": NotRequired[str],
+        "InstanceType": NotRequired[str],
+        "InstanceFamily": NotRequired[str],
+        "Quantity": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "HostRecovery": NotRequired[HostRecoveryType],
+        "OutpostArn": NotRequired[str],
+        "HostMaintenance": NotRequired[HostMaintenanceType],
+        "AssetIds": NotRequired[Sequence[str]],
+    },
+)
+AssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "IpamResourceDiscoveryId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CopyImageRequestRequestTypeDef = TypedDict(
+    "CopyImageRequestRequestTypeDef",
+    {
+        "Name": str,
+        "SourceImageId": str,
+        "SourceRegion": str,
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DestinationOutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "CopyImageTags": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CopySnapshotRequestRequestTypeDef = TypedDict(
+    "CopySnapshotRequestRequestTypeDef",
+    {
+        "SourceRegion": str,
+        "SourceSnapshotId": str,
+        "Description": NotRequired[str],
+        "DestinationOutpostArn": NotRequired[str],
+        "DestinationRegion": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "PresignedUrl": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
+        "TotalTargetCapacity": int,
+        "AllocationStrategy": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "Tenancy": NotRequired[Literal["default"]],
+        "EndDate": NotRequired[TimestampTypeDef],
+        "InstanceMatchCriteria": NotRequired[Literal["open"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "CreateCapacityReservationRequestRequestTypeDef",
+    {
+        "InstanceType": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "InstanceCount": int,
+        "ClientToken": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "Tenancy": NotRequired[CapacityReservationTenancyType],
+        "EbsOptimized": NotRequired[bool],
+        "EphemeralStorage": NotRequired[bool],
+        "EndDate": NotRequired[TimestampTypeDef],
+        "EndDateType": NotRequired[EndDateTypeType],
+        "InstanceMatchCriteria": NotRequired[InstanceMatchCriteriaType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "OutpostArn": NotRequired[str],
+        "PlacementGroupArn": NotRequired[str],
+    },
+)
+CreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "CreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "ClientCidrBlock": str,
+        "ServerCertificateArn": str,
+        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
+        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
+        "DnsServers": NotRequired[Sequence[str]],
+        "TransportProtocol": NotRequired[TransportProtocolType],
+        "VpnPort": NotRequired[int],
+        "Description": NotRequired[str],
+        "SplitTunnel": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "VpcId": NotRequired[str],
+        "SelfServicePortal": NotRequired[SelfServicePortalType],
+        "ClientConnectOptions": NotRequired[ClientConnectOptionsTypeDef],
+        "SessionTimeoutHours": NotRequired[int],
+        "ClientLoginBannerOptions": NotRequired[ClientLoginBannerOptionsTypeDef],
+    },
+)
+CreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "CreateCoipPoolRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+        "BgpAsn": NotRequired[int],
+        "PublicIp": NotRequired[str],
+        "CertificateArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DeviceName": NotRequired[str],
+        "IpAddress": NotRequired[str],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "CreateFlowLogsRequestRequestTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ResourceType": FlowLogsResourceTypeType,
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "DeliverLogsPermissionArn": NotRequired[str],
+        "DeliverCrossAccountRole": NotRequired[str],
+        "LogGroupName": NotRequired[str],
+        "TrafficType": NotRequired[TrafficTypeType],
+        "LogDestinationType": NotRequired[LogDestinationTypeType],
+        "LogDestination": NotRequired[str],
+        "LogFormat": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MaxAggregationInterval": NotRequired[int],
+        "DestinationOptions": NotRequired[DestinationOptionsRequestTypeDef],
+    },
+)
+CreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "CreateFpgaImageRequestRequestTypeDef",
+    {
+        "InputStorageLocation": StorageLocationTypeDef,
+        "DryRun": NotRequired[bool],
+        "LogsStorageLocation": NotRequired[StorageLocationTypeDef],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateImageRequestRequestTypeDef = TypedDict(
+    "CreateImageRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "NoReboot": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "DryRun": NotRequired[bool],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "PreserveClientIp": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Name": NotRequired[str],
+        "TimeRanges": NotRequired[Sequence[InstanceEventWindowTimeRangeRequestTypeDef]],
+        "CronExpression": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
+        "InstanceId": str,
+        "TargetEnvironment": ExportEnvironmentType,
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateInternetGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    {
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "CreateIpamPoolRequestRequestTypeDef",
+    {
+        "IpamScopeId": str,
+        "AddressFamily": AddressFamilyType,
+        "DryRun": NotRequired[bool],
+        "Locale": NotRequired[str],
+        "SourceIpamPoolId": NotRequired[str],
+        "Description": NotRequired[str],
+        "AutoImport": NotRequired[bool],
+        "PubliclyAdvertisable": NotRequired[bool],
+        "AllocationMinNetmaskLength": NotRequired[int],
+        "AllocationMaxNetmaskLength": NotRequired[int],
+        "AllocationDefaultNetmaskLength": NotRequired[int],
+        "AllocationResourceTags": NotRequired[Sequence[RequestIpamResourceTagTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "AwsService": NotRequired[Literal["ec2"]],
+        "PublicIpSource": NotRequired[IpamPoolPublicIpSourceType],
+        "SourceResource": NotRequired[IpamPoolSourceResourceRequestTypeDef],
+    },
+)
+CreateIpamRequestRequestTypeDef = TypedDict(
+    "CreateIpamRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "Tier": NotRequired[IpamTierType],
+    },
+)
+CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "CreateIpamScopeRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateKeyPairRequestRequestTypeDef = TypedDict(
+    "CreateKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "DryRun": NotRequired[bool],
+        "KeyType": NotRequired[KeyTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "KeyFormat": NotRequired[KeyFormatType],
+    },
+)
+CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "DryRun": NotRequired[bool],
+        "KeyType": NotRequired[KeyTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "KeyFormat": NotRequired[KeyFormatType],
+    },
+)
+CreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "LocalGatewayId": str,
+        "Mode": NotRequired[LocalGatewayRouteTableModeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayVirtualInterfaceGroupId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "PrefixListName": str,
+        "MaxEntries": int,
+        "AddressFamily": str,
+        "DryRun": NotRequired[bool],
+        "Entries": NotRequired[Sequence[AddPrefixListEntryTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "CreateNatGatewayRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "AllocationId": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ConnectivityType": NotRequired[ConnectivityTypeType],
+        "PrivateIpAddress": NotRequired[str],
+        "SecondaryAllocationIds": NotRequired[Sequence[str]],
+        "SecondaryPrivateIpAddresses": NotRequired[Sequence[str]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+    },
+)
+CreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "CreateNetworkAclRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Protocol": ProtocolType,
+        "ClientToken": str,
+        "SourceIp": NotRequired[str],
+        "DestinationIp": NotRequired[str],
+        "Destination": NotRequired[str],
+        "DestinationPort": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "FilterAtSource": NotRequired[PathRequestFilterTypeDef],
+        "FilterAtDestination": NotRequired[PathRequestFilterTypeDef],
+    },
+)
+CreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Groups": NotRequired[Sequence[str]],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6PrefixCount": NotRequired[int],
+        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "EnablePrimaryIpv6": NotRequired[bool],
+        "ConnectionTrackingSpecification": NotRequired[
+            ConnectionTrackingSpecificationRequestTypeDef
+        ],
+    },
+)
+CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "SubnetId": str,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Groups": NotRequired[Sequence[str]],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6PrefixCount": NotRequired[int],
+        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "EnablePrimaryIpv6": NotRequired[bool],
+        "ConnectionTrackingSpecification": NotRequired[
+            ConnectionTrackingSpecificationRequestTypeDef
+        ],
+    },
+)
+CreatePlacementGroupRequestRequestTypeDef = TypedDict(
+    "CreatePlacementGroupRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupName": NotRequired[str],
+        "Strategy": NotRequired[PlacementStrategyType],
+        "PartitionCount": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SpreadLevel": NotRequired[SpreadLevelType],
+    },
+)
+CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupName": NotRequired[str],
+        "Strategy": NotRequired[PlacementStrategyType],
+        "PartitionCount": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SpreadLevel": NotRequired[SpreadLevelType],
+    },
+)
+CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ImageId": NotRequired[str],
+        "DeleteReplacedRootVolume": NotRequired[bool],
+    },
+)
+CreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "ObjectKey": str,
+        "Name": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateRouteTableRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "CreateSecurityGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "VpcId": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "VpcId": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotRequestRequestTypeDef = TypedDict(
+    "CreateSnapshotRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "VolumeId": str,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "CreateSnapshotsRequestRequestTypeDef",
+    {
+        "InstanceSpecification": InstanceSpecificationTypeDef,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "CopyTagsFromSource": NotRequired[Literal["volume"]],
+    },
+)
+CreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Cidr": str,
+        "ReservationType": SubnetCidrReservationTypeType,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateSubnetRequestRequestTypeDef = TypedDict(
+    "CreateSubnetRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Ipv6Native": NotRequired[bool],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+    },
+)
+CreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Ipv6Native": NotRequired[bool],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+    },
+)
+CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "TrafficMirrorTargetId": str,
+        "TrafficMirrorFilterId": str,
+        "SessionNumber": int,
+        "PacketLength": NotRequired[int],
+        "VirtualNetworkId": NotRequired[int],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": NotRequired[str],
+        "NetworkLoadBalancerArn": NotRequired[str],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "GatewayLoadBalancerEndpointId": NotRequired[str],
+    },
+)
+CreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAttachmentId": str,
+        "PeerAddress": str,
+        "InsideCidrBlocks": Sequence[str],
+        "TransitGatewayAddress": NotRequired[str],
+        "BgpOptions": NotRequired[TransitGatewayConnectRequestBgpOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TransportTransitGatewayAttachmentId": str,
+        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "Options": NotRequired[CreateTransitGatewayMulticastDomainRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "PeerTransitGatewayId": str,
+        "PeerAccountId": str,
+        "PeerRegion": str,
+        "Options": NotRequired[CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Options": NotRequired[TransitGatewayRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TransitGatewayRouteTableId": str,
+        "PeeringAttachmentId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "VpcId": str,
+        "SubnetIds": Sequence[str],
+        "Options": NotRequired[CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "VerifiedAccessGroupId": str,
+        "EndpointType": VerifiedAccessEndpointTypeType,
+        "AttachmentType": Literal["vpc"],
+        "DomainCertificateArn": str,
+        "ApplicationDomain": str,
+        "EndpointDomainPrefix": str,
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "LoadBalancerOptions": NotRequired[CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef],
+        "NetworkInterfaceOptions": NotRequired[CreateVerifiedAccessEndpointEniOptionsTypeDef],
+        "Description": NotRequired[str],
+        "PolicyDocument": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "VerifiedAccessInstanceId": str,
+        "Description": NotRequired[str],
+        "PolicyDocument": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "FIPSEnabled": NotRequired[bool],
+    },
+)
+CreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "TrustProviderType": TrustProviderTypeType,
+        "PolicyReferenceName": str,
+        "UserTrustProviderType": NotRequired[UserTrustProviderTypeType],
+        "DeviceTrustProviderType": NotRequired[DeviceTrustProviderTypeType],
+        "OidcOptions": NotRequired[CreateVerifiedAccessTrustProviderOidcOptionsTypeDef],
+        "DeviceOptions": NotRequired[CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVolumeRequestRequestTypeDef = TypedDict(
+    "CreateVolumeRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "Encrypted": NotRequired[bool],
+        "Iops": NotRequired[int],
+        "KmsKeyId": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "VolumeType": NotRequired[VolumeTypeType],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiAttachEnabled": NotRequired[bool],
+        "Throughput": NotRequired[int],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "AvailabilityZone": str,
+        "Encrypted": NotRequired[bool],
+        "Iops": NotRequired[int],
+        "KmsKeyId": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "VolumeType": NotRequired[VolumeTypeType],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiAttachEnabled": NotRequired[bool],
+        "Throughput": NotRequired[int],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ServiceName": str,
+        "DryRun": NotRequired[bool],
+        "VpcEndpointType": NotRequired[VpcEndpointTypeType],
+        "PolicyDocument": NotRequired[str],
+        "RouteTableIds": NotRequired[Sequence[str]],
+        "SubnetIds": NotRequired[Sequence[str]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "IpAddressType": NotRequired[IpAddressTypeType],
+        "DnsOptions": NotRequired[DnsOptionsSpecificationTypeDef],
+        "ClientToken": NotRequired[str],
+        "PrivateDnsEnabled": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SubnetConfigurations": NotRequired[Sequence[SubnetConfigurationTypeDef]],
+    },
+)
+CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "AcceptanceRequired": NotRequired[bool],
+        "PrivateDnsName": NotRequired[str],
+        "NetworkLoadBalancerArns": NotRequired[Sequence[str]],
+        "GatewayLoadBalancerArns": NotRequired[Sequence[str]],
+        "SupportedIpAddressTypes": NotRequired[Sequence[str]],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "PeerOwnerId": NotRequired[str],
+        "PeerVpcId": NotRequired[str],
+        "PeerRegion": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "PeerOwnerId": NotRequired[str],
+        "PeerVpcId": NotRequired[str],
+        "PeerRegion": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcRequestRequestTypeDef = TypedDict(
+    "CreateVpcRequestRequestTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
+        "Ipv6Pool": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "InstanceTenancy": NotRequired[TenancyType],
+        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
+        "Ipv6Pool": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "InstanceTenancy": NotRequired[TenancyType],
+        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "CreateVpnGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+        "AvailabilityZone": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AmazonSideAsn": NotRequired[int],
+        "DryRun": NotRequired[bool],
+    },
+)
+ExportImageRequestRequestTypeDef = TypedDict(
+    "ExportImageRequestRequestTypeDef",
+    {
+        "DiskImageFormat": DiskImageFormatType,
+        "ImageId": str,
+        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "RoleName": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportImageRequestRequestTypeDef = TypedDict(
+    "ImportImageRequestRequestTypeDef",
+    {
+        "Architecture": NotRequired[str],
+        "ClientData": NotRequired[ClientDataTypeDef],
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DiskContainers": NotRequired[Sequence[ImageDiskContainerTypeDef]],
+        "DryRun": NotRequired[bool],
+        "Encrypted": NotRequired[bool],
+        "Hypervisor": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "LicenseType": NotRequired[str],
+        "Platform": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "LicenseSpecifications": NotRequired[
+            Sequence[ImportImageLicenseConfigurationRequestTypeDef]
+        ],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "UsageOperation": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+    },
+)
+ImportKeyPairRequestRequestTypeDef = TypedDict(
+    "ImportKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportSnapshotRequestRequestTypeDef = TypedDict(
+    "ImportSnapshotRequestRequestTypeDef",
+    {
+        "ClientData": NotRequired[ClientDataTypeDef],
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DiskContainer": NotRequired[SnapshotDiskContainerTypeDef],
+        "DryRun": NotRequired[bool],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "Cidr": str,
+        "CidrAuthorizationContext": NotRequired[CidrAuthorizationContextTypeDef],
+        "PubliclyAdvertisable": NotRequired[bool],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "PoolTagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiRegion": NotRequired[bool],
+        "NetworkBorderGroup": NotRequired[str],
+    },
+)
+PurchaseCapacityBlockRequestRequestTypeDef = TypedDict(
+    "PurchaseCapacityBlockRequestRequestTypeDef",
+    {
+        "CapacityBlockOfferingId": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+PurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "PurchaseHostReservationRequestRequestTypeDef",
+    {
+        "HostIdSet": Sequence[str],
+        "OfferingId": str,
+        "ClientToken": NotRequired[str],
+        "CurrencyCode": NotRequired[Literal["USD"]],
+        "LimitPrice": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+RegisterImageRequestRequestTypeDef = TypedDict(
+    "RegisterImageRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ImageLocation": NotRequired[str],
+        "Architecture": NotRequired[ArchitectureValuesType],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "EnaSupport": NotRequired[bool],
+        "KernelId": NotRequired[str],
+        "BillingProducts": NotRequired[Sequence[str]],
+        "RamdiskId": NotRequired[str],
+        "RootDeviceName": NotRequired[str],
+        "SriovNetSupport": NotRequired[str],
+        "VirtualizationType": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+        "TpmSupport": NotRequired[Literal["v2.0"]],
+        "UefiData": NotRequired[str],
+        "ImdsSupport": NotRequired[Literal["v2.0"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+RegisterImageRequestServiceResourceRegisterImageTypeDef = TypedDict(
+    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
+    {
+        "Name": str,
+        "ImageLocation": NotRequired[str],
+        "Architecture": NotRequired[ArchitectureValuesType],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "EnaSupport": NotRequired[bool],
+        "KernelId": NotRequired[str],
+        "BillingProducts": NotRequired[Sequence[str]],
+        "RamdiskId": NotRequired[str],
+        "RootDeviceName": NotRequired[str],
+        "SriovNetSupport": NotRequired[str],
+        "VirtualizationType": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+        "TpmSupport": NotRequired[Literal["v2.0"]],
+        "UefiData": NotRequired[str],
+        "ImdsSupport": NotRequired[Literal["v2.0"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsAccessScopeId": str,
+        "ClientToken": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+StartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsPathId": str,
+        "ClientToken": str,
+        "AdditionalAccounts": NotRequired[Sequence[str]],
+        "FilterInArns": NotRequired[Sequence[str]],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "SequenceNumber": NotRequired[int],
         "AclRule": NotRequired[AnalysisAclRuleTypeDef],
         "AttachedTo": NotRequired[AnalysisComponentTypeDef],
         "Component": NotRequired[AnalysisComponentTypeDef],
@@ -22097,16 +22209,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeRouteTablesResultTypeDef = TypedDict(
     "DescribeRouteTablesResultTypeDef",
     {
         "RouteTables": List[RouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetFlowLogsIntegrationTemplateRequestRequestTypeDef = TypedDict(
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     {
         "FlowLogId": str,
         "ConfigDeliveryS3DestinationArn": str,
@@ -22165,61 +22277,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeDhcpOptionsResultTypeDef = TypedDict(
     "DescribeDhcpOptionsResultTypeDef",
     {
         "DhcpOptions": List[DhcpOptionsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostsResultTypeDef = TypedDict(
     "DescribeHostsResultTypeDef",
     {
         "Hosts": List[HostTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BundleInstanceRequestRequestTypeDef = TypedDict(
     "BundleInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Storage": StorageTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
-BundleTaskTypeDef = TypedDict(
-    "BundleTaskTypeDef",
-    {
-        "BundleId": NotRequired[str],
-        "BundleTaskError": NotRequired[BundleTaskErrorTypeDef],
-        "InstanceId": NotRequired[str],
-        "Progress": NotRequired[str],
-        "StartTime": NotRequired[datetime],
-        "State": NotRequired[BundleTaskStateType],
-        "Storage": NotRequired[StorageTypeDef],
-        "UpdateTime": NotRequired[datetime],
-    },
-)
+StorageUnionTypeDef = Union[StorageTypeDef, StorageOutputTypeDef]
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeClientVpnEndpointsResultTypeDef = TypedDict(
     "DescribeClientVpnEndpointsResultTypeDef",
     {
         "ClientVpnEndpoints": List[ClientVpnEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpnTunnelOptionsRequestRequestTypeDef = TypedDict(
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     {
         "VpnConnectionId": str,
         "VpnTunnelOutsideIpAddress": str,
@@ -22266,16 +22366,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkAclsResultTypeDef = TypedDict(
     "DescribeNetworkAclsResultTypeDef",
     {
         "NetworkAcls": List[NetworkAclTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisableFastSnapshotRestoresResultTypeDef = TypedDict(
     "DisableFastSnapshotRestoresResultTypeDef",
     {
         "Successful": List[DisableFastSnapshotRestoreSuccessItemTypeDef],
         "Unsuccessful": List[DisableFastSnapshotRestoreErrorItemTypeDef],
@@ -22290,129 +22390,88 @@
         "ImportInstance": NotRequired[ImportInstanceTaskDetailsTypeDef],
         "ImportVolume": NotRequired[ImportVolumeTaskDetailsTypeDef],
         "State": NotRequired[ConversionTaskStateType],
         "StatusMessage": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-RunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
+SpotFleetLaunchSpecificationExtraOutputTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationExtraOutputTypeDef",
     {
-        "MaxCount": int,
-        "MinCount": int,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "AddressingType": NotRequired[str],
+        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
-        "Placement": NotRequired[PlacementTypeDef],
+        "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
+        "NetworkInterfaces": NotRequired[
+            List[InstanceNetworkInterfaceSpecificationExtraOutputTypeDef]
+        ],
+        "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "SecurityGroups": NotRequired[Sequence[str]],
+        "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
-        "AdditionalInfo": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DisableApiTermination": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "EbsOptimized": NotRequired[bool],
-        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
-        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
-        "NetworkInterfaces": NotRequired[
-            Sequence[InstanceNetworkInterfaceSpecificationServiceResourceTypeDef]
-        ],
-        "PrivateIpAddress": NotRequired[str],
-        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
-        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
-        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
-        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
-        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
-        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
-        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
-        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
-        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
-        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
-        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
-        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
-        "DisableApiStop": NotRequired[bool],
-        "EnablePrimaryIpv6": NotRequired[bool],
+        "WeightedCapacity": NotRequired[float],
+        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationExtraOutputTypeDef]],
+        "InstanceRequirements": NotRequired[InstanceRequirementsExtraOutputTypeDef],
     },
 )
-RunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
-    "RunInstancesRequestSubnetCreateInstancesTypeDef",
+LaunchSpecificationTypeDef = TypedDict(
+    "LaunchSpecificationTypeDef",
     {
-        "MaxCount": int,
-        "MinCount": int,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "UserData": NotRequired[str],
+        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "AddressingType": NotRequired[str],
+        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
-        "Placement": NotRequired[PlacementTypeDef],
+        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationOutputTypeDef]],
+        "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "SecurityGroups": NotRequired[Sequence[str]],
-        "UserData": NotRequired[str],
-        "AdditionalInfo": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DisableApiTermination": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "EbsOptimized": NotRequired[bool],
-        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
-        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
-        "NetworkInterfaces": NotRequired[
-            Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef]
-        ],
-        "PrivateIpAddress": NotRequired[str],
-        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
-        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
-        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
-        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
-        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
-        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
-        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
-        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
-        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
-        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
-        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
-        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
-        "DisableApiStop": NotRequired[bool],
-        "EnablePrimaryIpv6": NotRequired[bool],
+        "SubnetId": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
     },
 )
-LaunchSpecificationTypeDef = TypedDict(
-    "LaunchSpecificationTypeDef",
+SpotFleetLaunchSpecificationOutputTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationOutputTypeDef",
     {
-        "UserData": NotRequired[str],
         "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
         "AddressingType": NotRequired[str],
         "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationTypeDef]],
+        "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
+        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationOutputTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
+        "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "UserData": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationOutputTypeDef]],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
     },
 )
+InstanceNetworkInterfaceSpecificationUnionTypeDef = Union[
+    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationExtraOutputTypeDef,
+]
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SecurityGroups": NotRequired[Sequence[str]],
         "AddressingType": NotRequired[str],
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
@@ -22426,16 +22485,16 @@
         "NetworkInterfaces": NotRequired[Sequence[InstanceNetworkInterfaceSpecificationTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
     },
 )
-RunInstancesRequestRequestTypeDef = TypedDict(
-    "RunInstancesRequestRequestTypeDef",
+RunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
+    "RunInstancesRequestSubnetCreateInstancesTypeDef",
     {
         "MaxCount": int,
         "MinCount": int,
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "Ipv6AddressCount": NotRequired[int],
@@ -22443,15 +22502,14 @@
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
         "Placement": NotRequired[PlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SecurityGroups": NotRequired[Sequence[str]],
-        "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
         "AdditionalInfo": NotRequired[str],
         "ClientToken": NotRequired[str],
         "DisableApiTermination": NotRequired[bool],
         "DryRun": NotRequired[bool],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
@@ -22475,32 +22533,32 @@
         "DisableApiStop": NotRequired[bool],
         "EnablePrimaryIpv6": NotRequired[bool],
     },
 )
 SpotFleetLaunchSpecificationTypeDef = TypedDict(
     "SpotFleetLaunchSpecificationTypeDef",
     {
-        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "SecurityGroups": NotRequired[Sequence[GroupIdentifierTypeDef]],
         "AddressingType": NotRequired[str],
-        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
-        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationTypeDef]],
+        "NetworkInterfaces": NotRequired[Sequence[InstanceNetworkInterfaceSpecificationTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
         "WeightedCapacity": NotRequired[float],
-        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[SpotFleetTagSpecificationTypeDef]],
         "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
     },
 )
 RequestLaunchTemplateDataTypeDef = TypedDict(
     "RequestLaunchTemplateDataTypeDef",
     {
         "KernelId": NotRequired[str],
@@ -22563,16 +22621,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsPathsResultTypeDef = TypedDict(
     "DescribeNetworkInsightsPathsResultTypeDef",
     {
         "NetworkInsightsPaths": List[NetworkInsightsPathTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceNetworkInterfaceTypeDef = TypedDict(
     "InstanceNetworkInterfaceTypeDef",
     {
         "Association": NotRequired[InstanceNetworkInterfaceAssociationTypeDef],
         "Attachment": NotRequired[InstanceNetworkInterfaceAttachmentTypeDef],
@@ -22593,14 +22651,49 @@
         "Ipv4Prefixes": NotRequired[List[InstanceIpv4PrefixTypeDef]],
         "Ipv6Prefixes": NotRequired[List[InstanceIpv6PrefixTypeDef]],
         "ConnectionTrackingConfiguration": NotRequired[
             ConnectionTrackingSpecificationResponseTypeDef
         ],
     },
 )
+LaunchTemplateConfigExtraOutputTypeDef = TypedDict(
+    "LaunchTemplateConfigExtraOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[LaunchTemplateOverridesExtraOutputTypeDef]],
+    },
+)
+FleetLaunchTemplateConfigTypeDef = TypedDict(
+    "FleetLaunchTemplateConfigTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[FleetLaunchTemplateOverridesTypeDef]],
+    },
+)
+LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
+    "LaunchTemplateAndOverridesResponseTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[FleetLaunchTemplateOverridesTypeDef],
+    },
+)
+LaunchTemplateConfigOutputTypeDef = TypedDict(
+    "LaunchTemplateConfigOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[LaunchTemplateOverridesOutputTypeDef]],
+    },
+)
+LaunchTemplateConfigTypeDef = TypedDict(
+    "LaunchTemplateConfigTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[Sequence[LaunchTemplateOverridesTypeDef]],
+    },
+)
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationRequestTypeDef],
         "Overrides": NotRequired[Sequence[FleetLaunchTemplateOverridesRequestTypeDef]],
     },
 )
@@ -22631,74 +22724,127 @@
             InstanceRequirementsWithMetadataRequestTypeDef
         ],
         "DryRun": NotRequired[bool],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-FleetLaunchTemplateConfigTypeDef = TypedDict(
-    "FleetLaunchTemplateConfigTypeDef",
+DescribeInstanceStatusResultTypeDef = TypedDict(
+    "DescribeInstanceStatusResultTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[List[FleetLaunchTemplateOverridesTypeDef]],
+        "InstanceStatuses": List[InstanceStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
-    "LaunchTemplateAndOverridesResponseTypeDef",
+DescribeSecurityGroupsResultTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[FleetLaunchTemplateOverridesTypeDef],
+        "SecurityGroups": List[SecurityGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LaunchTemplateConfigTypeDef = TypedDict(
-    "LaunchTemplateConfigTypeDef",
+AuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[List[LaunchTemplateOverridesTypeDef]],
+        "GroupId": str,
+        "DryRun": NotRequired[bool],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-DescribeInstanceStatusResultTypeDef = TypedDict(
-    "DescribeInstanceStatusResultTypeDef",
+AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     {
-        "InstanceStatuses": List[InstanceStatusTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "IpProtocol": NotRequired[str],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
-DescribeSecurityGroupsResultPaginatorTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultPaginatorTypeDef",
+RevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "SecurityGroups": List[SecurityGroupPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "GroupId": str,
+        "DryRun": NotRequired[bool],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-DescribeSecurityGroupsResultTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultTypeDef",
+RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     {
-        "SecurityGroups": List[SecurityGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "IpProtocol": NotRequired[str],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
+    },
+)
+UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
+    },
+)
+UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
     },
 )
 DescribeStaleSecurityGroupsResultTypeDef = TypedDict(
     "DescribeStaleSecurityGroupsResultTypeDef",
     {
-        "NextToken": str,
         "StaleSecurityGroupSet": List[StaleSecurityGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamDiscoveredPublicAddressesResultTypeDef = TypedDict(
     "GetIpamDiscoveredPublicAddressesResultTypeDef",
     {
         "IpamDiscoveredPublicAddresses": List[IpamDiscoveredPublicAddressTypeDef],
         "OldestSampleTime": datetime,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ResponseLaunchTemplateDataTypeDef = TypedDict(
     "ResponseLaunchTemplateDataTypeDef",
     {
         "KernelId": NotRequired[str],
         "EbsOptimized": NotRequired[bool],
@@ -22729,26 +22875,26 @@
         "CapacityReservationSpecification": NotRequired[
             LaunchTemplateCapacityReservationSpecificationResponseTypeDef
         ],
         "LicenseSpecifications": NotRequired[List[LaunchTemplateLicenseConfigurationTypeDef]],
         "HibernationOptions": NotRequired[LaunchTemplateHibernationOptionsTypeDef],
         "MetadataOptions": NotRequired[LaunchTemplateInstanceMetadataOptionsTypeDef],
         "EnclaveOptions": NotRequired[LaunchTemplateEnclaveOptionsTypeDef],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
         "PrivateDnsNameOptions": NotRequired[LaunchTemplatePrivateDnsNameOptionsTypeDef],
         "MaintenanceOptions": NotRequired[LaunchTemplateInstanceMaintenanceOptionsTypeDef],
         "DisableApiStop": NotRequired[bool],
     },
 )
 DescribeReservedInstancesModificationsResultTypeDef = TypedDict(
     "DescribeReservedInstancesModificationsResultTypeDef",
     {
-        "NextToken": str,
         "ReservedInstancesModifications": List[ReservedInstancesModificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceTypeInfoTypeDef = TypedDict(
     "InstanceTypeInfoTypeDef",
     {
         "InstanceType": NotRequired[InstanceTypeType],
         "CurrentGeneration": NotRequired[bool],
@@ -22783,50 +22929,71 @@
 )
 CreateNetworkInsightsAccessScopeRequestRequestTypeDef = TypedDict(
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     {
         "ClientToken": str,
         "MatchPaths": NotRequired[Sequence[AccessScopePathRequestTypeDef]],
         "ExcludePaths": NotRequired[Sequence[AccessScopePathRequestTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
 NetworkInsightsAccessScopeContentTypeDef = TypedDict(
     "NetworkInsightsAccessScopeContentTypeDef",
     {
         "NetworkInsightsAccessScopeId": NotRequired[str],
         "MatchPaths": NotRequired[List[AccessScopePathTypeDef]],
         "ExcludePaths": NotRequired[List[AccessScopePathTypeDef]],
     },
 )
+BundleInstanceResultTypeDef = TypedDict(
+    "BundleInstanceResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CancelBundleTaskResultTypeDef = TypedDict(
+    "CancelBundleTaskResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeBundleTasksResultTypeDef = TypedDict(
+    "DescribeBundleTasksResultTypeDef",
+    {
+        "BundleTasks": List[BundleTaskTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 RunScheduledInstancesRequestRequestTypeDef = TypedDict(
     "RunScheduledInstancesRequestRequestTypeDef",
     {
         "LaunchSpecification": ScheduledInstancesLaunchSpecificationTypeDef,
         "ScheduledInstanceId": str,
         "ClientToken": NotRequired[str],
         "DryRun": NotRequired[bool],
         "InstanceCount": NotRequired[int],
     },
 )
 DescribeImportImageTasksResultTypeDef = TypedDict(
     "DescribeImportImageTasksResultTypeDef",
     {
         "ImportImageTasks": List[ImportImageTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeImportSnapshotTasksResultTypeDef = TypedDict(
     "DescribeImportSnapshotTasksResultTypeDef",
     {
         "ImportSnapshotTasks": List[ImportSnapshotTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateDefaultSubnetResultTypeDef = TypedDict(
     "CreateDefaultSubnetResultTypeDef",
     {
         "Subnet": SubnetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22839,32 +23006,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSubnetsResultTypeDef = TypedDict(
     "DescribeSubnetsResultTypeDef",
     {
         "Subnets": List[SubnetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTrafficMirrorFilterResultTypeDef = TypedDict(
     "CreateTrafficMirrorFilterResultTypeDef",
     {
         "TrafficMirrorFilter": TrafficMirrorFilterTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorFiltersResultTypeDef = TypedDict(
     "DescribeTrafficMirrorFiltersResultTypeDef",
     {
         "TrafficMirrorFilters": List[TrafficMirrorFilterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTrafficMirrorFilterNetworkServicesResultTypeDef = TypedDict(
     "ModifyTrafficMirrorFilterNetworkServicesResultTypeDef",
     {
         "TrafficMirrorFilter": TrafficMirrorFilterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22884,16 +23051,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayConnectPeersResultTypeDef = TypedDict(
     "DescribeTransitGatewayConnectPeersResultTypeDef",
     {
         "TransitGatewayConnectPeers": List[TransitGatewayConnectPeerTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayPolicyTableEntriesResultTypeDef = TypedDict(
     "GetTransitGatewayPolicyTableEntriesResultTypeDef",
     {
         "TransitGatewayPolicyTableEntries": List[TransitGatewayPolicyTableEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22905,17 +23072,17 @@
         "VerifiedAccessInstanceId": NotRequired[str],
         "AccessLogs": NotRequired[VerifiedAccessLogsTypeDef],
     },
 )
 DescribeVolumeStatusResultTypeDef = TypedDict(
     "DescribeVolumeStatusResultTypeDef",
     {
-        "NextToken": str,
         "VolumeStatuses": List[VolumeStatusItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateDefaultVpcResultTypeDef = TypedDict(
     "CreateDefaultVpcResultTypeDef",
     {
         "Vpc": VpcTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22928,16 +23095,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcsResultTypeDef = TypedDict(
     "DescribeVpcsResultTypeDef",
     {
         "Vpcs": List[VpcTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptVpcPeeringConnectionResultTypeDef = TypedDict(
     "AcceptVpcPeeringConnectionResultTypeDef",
     {
         "VpcPeeringConnection": VpcPeeringConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22950,16 +23117,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcPeeringConnectionsResultTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsResultTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AccessScopeAnalysisFindingTypeDef = TypedDict(
     "AccessScopeAnalysisFindingTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": NotRequired[str],
         "NetworkInsightsAccessScopeId": NotRequired[str],
@@ -22996,49 +23163,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInterfacesResultTypeDef = TypedDict(
     "DescribeNetworkInterfacesResultTypeDef",
     {
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BundleInstanceResultTypeDef = TypedDict(
-    "BundleInstanceResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CancelBundleTaskResultTypeDef = TypedDict(
-    "CancelBundleTaskResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBundleTasksResultTypeDef = TypedDict(
-    "DescribeBundleTasksResultTypeDef",
-    {
-        "BundleTasks": List[BundleTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "CreateVpnConnectionRequestRequestTypeDef",
     {
         "CustomerGatewayId": str,
         "Type": str,
         "VpnGatewayId": NotRequired[str],
         "TransitGatewayId": NotRequired[str],
         "DryRun": NotRequired[bool],
         "Options": NotRequired[VpnConnectionOptionsSpecificationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
 VpnConnectionTypeDef = TypedDict(
     "VpnConnectionTypeDef",
     {
         "CustomerGatewayConfiguration": NotRequired[str],
         "CustomerGatewayId": NotRequired[str],
@@ -23098,41 +23244,137 @@
         "Tags": NotRequired[List[TagTypeDef]],
         "Type": NotRequired[SpotInstanceTypeType],
         "ValidFrom": NotRequired[datetime],
         "ValidUntil": NotRequired[datetime],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
     },
 )
+RunInstancesRequestRequestTypeDef = TypedDict(
+    "RunInstancesRequestRequestTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "ImageId": NotRequired[str],
+        "InstanceType": NotRequired[InstanceTypeType],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "Placement": NotRequired[PlacementTypeDef],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "SecurityGroups": NotRequired[Sequence[str]],
+        "SubnetId": NotRequired[str],
+        "UserData": NotRequired[str],
+        "AdditionalInfo": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DisableApiTermination": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
+        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
+        "NetworkInterfaces": NotRequired[
+            Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef]
+        ],
+        "PrivateIpAddress": NotRequired[str],
+        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
+        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
+        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
+        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
+        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
+        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
+        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
+        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
+        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
+        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
+        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
+        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
+        "DisableApiStop": NotRequired[bool],
+        "EnablePrimaryIpv6": NotRequired[bool],
+    },
+)
+RunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "ImageId": NotRequired[str],
+        "InstanceType": NotRequired[InstanceTypeType],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "Placement": NotRequired[PlacementTypeDef],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "SecurityGroups": NotRequired[Sequence[str]],
+        "SubnetId": NotRequired[str],
+        "UserData": NotRequired[str],
+        "AdditionalInfo": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DisableApiTermination": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
+        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
+        "NetworkInterfaces": NotRequired[
+            Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef]
+        ],
+        "PrivateIpAddress": NotRequired[str],
+        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
+        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
+        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
+        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
+        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
+        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
+        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
+        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
+        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
+        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
+        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
+        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
+        "DisableApiStop": NotRequired[bool],
+        "EnablePrimaryIpv6": NotRequired[bool],
+    },
+)
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": NotRequired[str],
         "BlockDurationMinutes": NotRequired[int],
         "ClientToken": NotRequired[str],
         "DryRun": NotRequired[bool],
         "InstanceCount": NotRequired[int],
         "LaunchGroup": NotRequired[str],
         "LaunchSpecification": NotRequired[RequestSpotLaunchSpecificationTypeDef],
         "SpotPrice": NotRequired[str],
         "Type": NotRequired[SpotInstanceTypeType],
         "ValidFrom": NotRequired[TimestampTypeDef],
         "ValidUntil": NotRequired[TimestampTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
     },
 )
 CreateLaunchTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchTemplateRequestRequestTypeDef",
     {
         "LaunchTemplateName": str,
         "LaunchTemplateData": RequestLaunchTemplateDataTypeDef,
         "DryRun": NotRequired[bool],
         "ClientToken": NotRequired[str],
         "VersionDescription": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
 CreateLaunchTemplateVersionRequestRequestTypeDef = TypedDict(
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     {
         "LaunchTemplateData": RequestLaunchTemplateDataTypeDef,
         "DryRun": NotRequired[bool],
@@ -23206,42 +23448,43 @@
         "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsResponseTypeDef],
         "Ipv6Address": NotRequired[str],
         "TpmSupport": NotRequired[str],
         "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsTypeDef],
         "CurrentInstanceBootMode": NotRequired[InstanceBootModeValuesType],
     },
 )
-CreateFleetRequestRequestTypeDef = TypedDict(
-    "CreateFleetRequestRequestTypeDef",
+SpotFleetRequestConfigDataExtraOutputTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataExtraOutputTypeDef",
     {
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
-        "DryRun": NotRequired[bool],
+        "IamFleetRole": str,
+        "TargetCapacity": int,
+        "AllocationStrategy": NotRequired[AllocationStrategyType],
+        "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
+        "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
-        "SpotOptions": NotRequired[SpotOptionsRequestTypeDef],
-        "OnDemandOptions": NotRequired[OnDemandOptionsRequestTypeDef],
-        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
+        "FulfilledCapacity": NotRequired[float],
+        "OnDemandFulfilledCapacity": NotRequired[float],
+        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationExtraOutputTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigExtraOutputTypeDef]],
+        "SpotPrice": NotRequired[str],
+        "OnDemandTargetCapacity": NotRequired[int],
+        "OnDemandMaxTotalPrice": NotRequired[str],
+        "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
-        "ValidFrom": NotRequired[TimestampTypeDef],
-        "ValidUntil": NotRequired[TimestampTypeDef],
+        "ValidFrom": NotRequired[datetime],
+        "ValidUntil": NotRequired[datetime],
         "ReplaceUnhealthyInstances": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "Context": NotRequired[str],
-    },
-)
-ModifyFleetRequestRequestTypeDef = TypedDict(
-    "ModifyFleetRequestRequestTypeDef",
-    {
-        "FleetId": str,
-        "DryRun": NotRequired[bool],
-        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
-        "LaunchTemplateConfigs": NotRequired[Sequence[FleetLaunchTemplateConfigRequestTypeDef]],
-        "TargetCapacitySpecification": NotRequired[TargetCapacitySpecificationRequestTypeDef],
+        "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
+        "LoadBalancersConfig": NotRequired[LoadBalancersConfigExtraOutputTypeDef],
+        "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
+        "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
+        "TagSpecifications": NotRequired[List[TagSpecificationExtraOutputTypeDef]],
     },
 )
 CreateFleetErrorTypeDef = TypedDict(
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": NotRequired[LaunchTemplateAndOverridesResponseTypeDef],
         "Lifecycle": NotRequired[InstanceLifecycleType],
@@ -23274,85 +23517,107 @@
         "LaunchTemplateAndOverrides": NotRequired[LaunchTemplateAndOverridesResponseTypeDef],
         "Lifecycle": NotRequired[InstanceLifecycleType],
         "InstanceIds": NotRequired[List[str]],
         "InstanceType": NotRequired[InstanceTypeType],
         "Platform": NotRequired[Literal["windows"]],
     },
 )
-ModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "ModifySpotFleetRequestRequestRequestTypeDef",
-    {
-        "SpotFleetRequestId": str,
-        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
-        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigTypeDef]],
-        "TargetCapacity": NotRequired[int],
-        "OnDemandTargetCapacity": NotRequired[int],
-        "Context": NotRequired[str],
-    },
-)
-SpotFleetRequestConfigDataPaginatorTypeDef = TypedDict(
-    "SpotFleetRequestConfigDataPaginatorTypeDef",
+SpotFleetRequestConfigDataOutputTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataOutputTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
         "AllocationStrategy": NotRequired[AllocationStrategyType],
         "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
         "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
         "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
         "FulfilledCapacity": NotRequired[float],
         "OnDemandFulfilledCapacity": NotRequired[float],
-        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationTypeDef]],
-        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigTypeDef]],
+        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationOutputTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigOutputTypeDef]],
         "SpotPrice": NotRequired[str],
         "OnDemandTargetCapacity": NotRequired[int],
         "OnDemandMaxTotalPrice": NotRequired[str],
         "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
         "ValidFrom": NotRequired[datetime],
         "ValidUntil": NotRequired[datetime],
         "ReplaceUnhealthyInstances": NotRequired[bool],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
-        "LoadBalancersConfig": NotRequired[LoadBalancersConfigTypeDef],
+        "LoadBalancersConfig": NotRequired[LoadBalancersConfigOutputTypeDef],
         "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
         "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
-        "TagSpecifications": NotRequired[List[TagSpecificationPaginatorTypeDef]],
+        "TagSpecifications": NotRequired[List[TagSpecificationOutputTypeDef]],
     },
 )
+LaunchTemplateConfigUnionTypeDef = Union[
+    LaunchTemplateConfigTypeDef, LaunchTemplateConfigExtraOutputTypeDef
+]
 SpotFleetRequestConfigDataTypeDef = TypedDict(
     "SpotFleetRequestConfigDataTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
         "AllocationStrategy": NotRequired[AllocationStrategyType],
         "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
         "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
         "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
         "FulfilledCapacity": NotRequired[float],
         "OnDemandFulfilledCapacity": NotRequired[float],
-        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationTypeDef]],
-        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigTypeDef]],
+        "LaunchSpecifications": NotRequired[Sequence[SpotFleetLaunchSpecificationTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigTypeDef]],
         "SpotPrice": NotRequired[str],
         "OnDemandTargetCapacity": NotRequired[int],
         "OnDemandMaxTotalPrice": NotRequired[str],
         "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
-        "ValidFrom": NotRequired[datetime],
-        "ValidUntil": NotRequired[datetime],
+        "ValidFrom": NotRequired[TimestampTypeDef],
+        "ValidUntil": NotRequired[TimestampTypeDef],
         "ReplaceUnhealthyInstances": NotRequired[bool],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
         "LoadBalancersConfig": NotRequired[LoadBalancersConfigTypeDef],
         "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
         "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
-        "TagSpecifications": NotRequired[List[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+    },
+)
+CreateFleetRequestRequestTypeDef = TypedDict(
+    "CreateFleetRequestRequestTypeDef",
+    {
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "SpotOptions": NotRequired[SpotOptionsRequestTypeDef],
+        "OnDemandOptions": NotRequired[OnDemandOptionsRequestTypeDef],
+        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "TerminateInstancesWithExpiration": NotRequired[bool],
+        "Type": NotRequired[FleetTypeType],
+        "ValidFrom": NotRequired[TimestampTypeDef],
+        "ValidUntil": NotRequired[TimestampTypeDef],
+        "ReplaceUnhealthyInstances": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "Context": NotRequired[str],
+    },
+)
+ModifyFleetRequestRequestTypeDef = TypedDict(
+    "ModifyFleetRequestRequestTypeDef",
+    {
+        "FleetId": str,
+        "DryRun": NotRequired[bool],
+        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "LaunchTemplateConfigs": NotRequired[Sequence[FleetLaunchTemplateConfigRequestTypeDef]],
+        "TargetCapacitySpecification": NotRequired[TargetCapacitySpecificationRequestTypeDef],
+        "Context": NotRequired[str],
     },
 )
 GetLaunchTemplateDataResultTypeDef = TypedDict(
     "GetLaunchTemplateDataResultTypeDef",
     {
         "LaunchTemplateData": ResponseLaunchTemplateDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23371,16 +23636,16 @@
         "LaunchTemplateData": NotRequired[ResponseLaunchTemplateDataTypeDef],
     },
 )
 DescribeInstanceTypesResultTypeDef = TypedDict(
     "DescribeInstanceTypesResultTypeDef",
     {
         "InstanceTypes": List[InstanceTypeInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkInsightsAccessScopeResultTypeDef = TypedDict(
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     {
         "NetworkInsightsAccessScope": NetworkInsightsAccessScopeTypeDef,
         "NetworkInsightsAccessScopeContent": NetworkInsightsAccessScopeContentTypeDef,
@@ -23394,16 +23659,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     {
         "LoggingConfigurations": List[VerifiedAccessInstanceLoggingConfigurationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef = TypedDict(
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
     {
         "LoggingConfiguration": VerifiedAccessInstanceLoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23411,24 +23676,24 @@
 )
 GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef = TypedDict(
     "GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "AnalysisStatus": AnalysisStatusType,
         "AnalysisFindings": List[AccessScopeAnalysisFindingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeNetworkInsightsAnalysesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAnalysesResultTypeDef",
     {
         "NetworkInsightsAnalyses": List[NetworkInsightsAnalysisTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartNetworkInsightsAnalysisResultTypeDef = TypedDict(
     "StartNetworkInsightsAnalysisResultTypeDef",
     {
         "NetworkInsightsAnalysis": NetworkInsightsAnalysisTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23476,16 +23741,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSpotInstanceRequestsResultTypeDef = TypedDict(
     "DescribeSpotInstanceRequestsResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RequestSpotInstancesResultTypeDef = TypedDict(
     "RequestSpotInstancesResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23543,84 +23808,79 @@
         "OnDemandOptions": NotRequired[OnDemandOptionsTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
         "Errors": NotRequired[List[DescribeFleetErrorTypeDef]],
         "Instances": NotRequired[List[DescribeFleetsInstancesTypeDef]],
         "Context": NotRequired[str],
     },
 )
-SpotFleetRequestConfigPaginatorTypeDef = TypedDict(
-    "SpotFleetRequestConfigPaginatorTypeDef",
+SpotFleetRequestConfigTypeDef = TypedDict(
+    "SpotFleetRequestConfigTypeDef",
     {
         "ActivityStatus": NotRequired[ActivityStatusType],
         "CreateTime": NotRequired[datetime],
-        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataPaginatorTypeDef],
+        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataOutputTypeDef],
         "SpotFleetRequestId": NotRequired[str],
         "SpotFleetRequestState": NotRequired[BatchStateType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+ModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "ModifySpotFleetRequestRequestRequestTypeDef",
+    {
+        "SpotFleetRequestId": str,
+        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
+        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigUnionTypeDef]],
+        "TargetCapacity": NotRequired[int],
+        "OnDemandTargetCapacity": NotRequired[int],
+        "Context": NotRequired[str],
+    },
+)
 RequestSpotFleetRequestRequestTypeDef = TypedDict(
     "RequestSpotFleetRequestRequestTypeDef",
     {
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
-SpotFleetRequestConfigTypeDef = TypedDict(
-    "SpotFleetRequestConfigTypeDef",
-    {
-        "ActivityStatus": NotRequired[ActivityStatusType],
-        "CreateTime": NotRequired[datetime],
-        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataTypeDef],
-        "SpotFleetRequestId": NotRequired[str],
-        "SpotFleetRequestState": NotRequired[BatchStateType],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
+SpotFleetRequestConfigDataUnionTypeDef = Union[
+    SpotFleetRequestConfigDataTypeDef, SpotFleetRequestConfigDataExtraOutputTypeDef
+]
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
         "LaunchTemplateVersion": LaunchTemplateVersionTypeDef,
         "Warning": ValidationWarningTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLaunchTemplateVersionsResultTypeDef = TypedDict(
     "DescribeLaunchTemplateVersionsResultTypeDef",
     {
         "LaunchTemplateVersions": List[LaunchTemplateVersionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Reservations": List[ReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
-        "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeSpotFleetRequestsResponsePaginatorTypeDef = TypedDict(
-    "DescribeSpotFleetRequestsResponsePaginatorTypeDef",
-    {
-        "NextToken": str,
-        "SpotFleetRequestConfigs": List[SpotFleetRequestConfigPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetRequestsResponseTypeDef = TypedDict(
     "DescribeSpotFleetRequestsResponseTypeDef",
     {
-        "NextToken": str,
         "SpotFleetRequestConfigs": List[SpotFleetRequestConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/type_defs.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
     ResourceTypeType,
     RIProductDescriptionType,
     RootDeviceTypeType,
     RouteOriginType,
     RouteStateType,
     RouteTableAssociationStateCodeType,
     RuleActionType,
+    ScopeType,
     SecurityGroupReferencingSupportValueType,
     SelfServicePortalType,
     ServiceConnectivityTypeType,
     ServiceStateType,
     ServiceTypeType,
     ShutdownBehaviorType,
     SnapshotAttributeNameType,
@@ -306,15 +307,14 @@
     VpcCidrBlockStateCodeType,
     VpcEndpointTypeType,
     VpcPeeringConnectionStateReasonCodeType,
     VpcStateType,
     VpnEcmpSupportValueType,
     VpnStateType,
     WeekDayType,
-    scopeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -876,26 +876,26 @@
     "InstanceIpv6PrefixTypeDef",
     "InstanceMaintenanceOptionsRequestTypeDef",
     "InstanceMaintenanceOptionsTypeDef",
     "InstanceMetadataOptionsRequestTypeDef",
     "InstanceMetadataOptionsResponseTypeDef",
     "MonitoringTypeDef",
     "InstanceNetworkInterfaceAssociationTypeDef",
-    "MemoryGiBPerVCpuRequestTypeDef",
-    "MemoryMiBRequestTypeDef",
-    "NetworkBandwidthGbpsRequestTypeDef",
-    "NetworkInterfaceCountRequestTypeDef",
-    "TotalLocalStorageGBRequestTypeDef",
-    "VCpuCountRangeRequestTypeDef",
     "MemoryGiBPerVCpuTypeDef",
     "MemoryMiBTypeDef",
     "NetworkBandwidthGbpsTypeDef",
     "NetworkInterfaceCountTypeDef",
     "TotalLocalStorageGBTypeDef",
     "VCpuCountRangeTypeDef",
+    "MemoryGiBPerVCpuRequestTypeDef",
+    "MemoryMiBRequestTypeDef",
+    "NetworkBandwidthGbpsRequestTypeDef",
+    "NetworkInterfaceCountRequestTypeDef",
+    "TotalLocalStorageGBRequestTypeDef",
+    "VCpuCountRangeRequestTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
     "NitroTpmInfoTypeDef",
@@ -1089,14 +1089,15 @@
     "RestoreAddressToClassicRequestRequestTypeDef",
     "RestoreImageFromRecycleBinRequestRequestTypeDef",
     "RestoreManagedPrefixListVersionRequestRequestTypeDef",
     "RestoreSnapshotFromRecycleBinRequestRequestTypeDef",
     "RestoreSnapshotTierRequestRequestTypeDef",
     "RevokeClientVpnIngressRequestRequestTypeDef",
     "RouteTypeDef",
+    "S3StorageOutputTypeDef",
     "ScheduledInstanceRecurrenceTypeDef",
     "ScheduledInstancesEbsTypeDef",
     "ScheduledInstancesIamInstanceProfileTypeDef",
     "ScheduledInstancesIpv6AddressTypeDef",
     "ScheduledInstancesMonitoringTypeDef",
     "ScheduledInstancesPlacementTypeDef",
     "ScheduledInstancesPrivateIpAddressConfigTypeDef",
@@ -1350,17 +1351,20 @@
     "PlacementGroupTypeDef",
     "ReplaceRootVolumeTaskTypeDef",
     "SecurityGroupForVpcTypeDef",
     "SnapshotInfoTypeDef",
     "SnapshotResponseTypeDef",
     "SnapshotTierStatusTypeDef",
     "SnapshotTypeDef",
+    "SpotFleetTagSpecificationExtraOutputTypeDef",
+    "SpotFleetTagSpecificationOutputTypeDef",
     "SpotFleetTagSpecificationTypeDef",
     "SubnetCidrReservationTypeDef",
-    "TagSpecificationPaginatorTypeDef",
+    "TagSpecificationExtraOutputTypeDef",
+    "TagSpecificationOutputTypeDef",
     "TagSpecificationTypeDef",
     "TrafficMirrorSessionTypeDef",
     "TrafficMirrorTargetTypeDef",
     "TransitGatewayPolicyTableTypeDef",
     "TransitGatewayRouteTableAnnouncementTypeDef",
     "TransitGatewayRouteTableTypeDef",
     "TrunkInterfaceAssociationTypeDef",
@@ -1447,14 +1451,16 @@
     "CapacityReservationSpecificationResponseResponseTypeDef",
     "CapacityReservationSpecificationResponseTypeDef",
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     "CapacityReservationSpecificationTypeDef",
     "LaunchTemplateCapacityReservationSpecificationRequestTypeDef",
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     "ClassicLinkInstanceTypeDef",
+    "ClassicLoadBalancersConfigExtraOutputTypeDef",
+    "ClassicLoadBalancersConfigOutputTypeDef",
     "ClassicLoadBalancersConfigTypeDef",
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     "ClientConnectResponseOptionsTypeDef",
     "ClientVpnAuthenticationRequestTypeDef",
     "ClientVpnAuthenticationTypeDef",
     "ClientVpnConnectionTypeDef",
     "TerminateConnectionStatusTypeDef",
@@ -1903,20 +1909,23 @@
     "ImportInstanceLaunchSpecificationTypeDef",
     "InferenceDeviceInfoTypeDef",
     "InstanceAttachmentEnaSrdSpecificationTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
-    "InstanceRequirementsRequestTypeDef",
+    "InstanceRequirementsExtraOutputTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
+    "InstanceRequirementsRequestTypeDef",
     "InstanceStateChangeTypeDef",
     "InstanceStatusSummaryTypeDef",
     "ModifyInstanceEventStartTimeResultTypeDef",
-    "IpPermissionPaginatorTypeDef",
+    "IpPermissionExtraExtraOutputTypeDef",
+    "IpPermissionOutputTypeDef",
     "IpPermissionTypeDef",
     "StaleIpPermissionTypeDef",
     "ProvisionIpamPoolCidrRequestRequestTypeDef",
     "IpamDiscoveredAccountTypeDef",
     "IpamDiscoveredResourceCidrTypeDef",
     "IpamResourceCidrTypeDef",
     "IpamResourceDiscoveryTypeDef",
@@ -1964,14 +1973,15 @@
     "PurchaseReservedInstancesOfferingRequestRequestTypeDef",
     "ReservedInstancesOfferingTypeDef",
     "ReservedInstancesTypeDef",
     "SecurityGroupRuleTypeDef",
     "RegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     "RegisterTransitGatewayMulticastGroupMembersResultTypeDef",
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
+    "StorageOutputTypeDef",
     "ScheduledInstanceAvailabilityTypeDef",
     "ScheduledInstanceTypeDef",
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     "ScheduledInstancesNetworkInterfaceTypeDef",
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     "VpcEndpointTypeDef",
     "SecurityGroupRuleUpdateTypeDef",
@@ -1981,14 +1991,16 @@
     "SnapshotTaskDetailTypeDef",
     "SpotMaintenanceStrategiesTypeDef",
     "SpotDatafeedSubscriptionTypeDef",
     "TransitGatewayMulticastDomainAssociationTypeDef",
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     "SubnetIpv6CidrBlockAssociationTypeDef",
     "TargetReservationValueTypeDef",
+    "TargetGroupsConfigExtraOutputTypeDef",
+    "TargetGroupsConfigOutputTypeDef",
     "TargetGroupsConfigTypeDef",
     "TrafficMirrorFilterRuleTypeDef",
     "TransitGatewayAttachmentTypeDef",
     "TransitGatewayConnectPeerConfigurationTypeDef",
     "TransitGatewayConnectTypeDef",
     "TransitGatewayMulticastDomainTypeDef",
     "TransitGatewayTypeDef",
@@ -2070,106 +2082,23 @@
     "GetSecurityGroupsForVpcResultTypeDef",
     "CreateSnapshotsResultTypeDef",
     "DescribeSnapshotTierStatusResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "CreateSubnetCidrReservationResultTypeDef",
     "DeleteSubnetCidrReservationResultTypeDef",
     "GetSubnetCidrReservationsResultTypeDef",
-    "AcceptAddressTransferRequestRequestTypeDef",
-    "AllocateAddressRequestRequestTypeDef",
-    "AllocateHostsRequestRequestTypeDef",
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CopyImageRequestRequestTypeDef",
-    "CopySnapshotRequestRequestTypeDef",
     "CopySnapshotRequestSnapshotCopyTypeDef",
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    "CreateCapacityReservationRequestRequestTypeDef",
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    "CreateCoipPoolRequestRequestTypeDef",
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    "CreateFlowLogsRequestRequestTypeDef",
-    "CreateFpgaImageRequestRequestTypeDef",
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    "CreateInternetGatewayRequestRequestTypeDef",
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    "CreateIpamPoolRequestRequestTypeDef",
-    "CreateIpamRequestRequestTypeDef",
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CreateIpamScopeRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    "CreateNatGatewayRequestRequestTypeDef",
-    "CreateNetworkAclRequestRequestTypeDef",
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
-    "CreatePlacementGroupRequestRequestTypeDef",
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    "CreateRouteTableRequestRequestTypeDef",
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
-    "CreateSecurityGroupRequestRequestTypeDef",
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
-    "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
-    "CreateSnapshotsRequestRequestTypeDef",
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    "CreateSubnetRequestRequestTypeDef",
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    "CreateTransitGatewayRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    "CreateVpcEndpointRequestRequestTypeDef",
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
-    "CreateVpcRequestRequestTypeDef",
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    "CreateVpnGatewayRequestRequestTypeDef",
-    "ExportImageRequestRequestTypeDef",
-    "ImportKeyPairRequestRequestTypeDef",
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    "PurchaseCapacityBlockRequestRequestTypeDef",
-    "PurchaseHostReservationRequestRequestTypeDef",
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
+    "TagSpecificationUnionTypeDef",
     "CreateTrafficMirrorSessionResultTypeDef",
     "DescribeTrafficMirrorSessionsResultTypeDef",
     "ModifyTrafficMirrorSessionResultTypeDef",
     "CreateTrafficMirrorTargetResultTypeDef",
     "DescribeTrafficMirrorTargetsResultTypeDef",
     "CreateTransitGatewayPolicyTableResultTypeDef",
     "DeleteTransitGatewayPolicyTableResultTypeDef",
@@ -2205,28 +2134,24 @@
     "NetworkInterfaceAttachmentTypeDef",
     "DhcpOptionsTypeDef",
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     "DescribeAvailabilityZonesResultTypeDef",
     "HostTypeDef",
     "StorageTypeDef",
     "CreateImageRequestInstanceCreateImageTypeDef",
-    "CreateImageRequestRequestTypeDef",
     "ImageAttributeTypeDef",
     "ImageTypeDef",
-    "RegisterImageRequestRequestTypeDef",
-    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
     "CancelCapacityReservationFleetsResultTypeDef",
     "CancelSpotFleetRequestsResponseTypeDef",
     "CreateCapacityReservationResultTypeDef",
     "DescribeCapacityReservationsResultTypeDef",
     "PurchaseCapacityBlockResultTypeDef",
     "DescribeCapacityReservationFleetsResultTypeDef",
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     "DescribeClassicLinkInstancesResultTypeDef",
-    "CreateClientVpnEndpointRequestRequestTypeDef",
     "ClientVpnEndpointTypeDef",
     "DescribeClientVpnConnectionsResultTypeDef",
     "TerminateClientVpnConnectionsResultTypeDef",
     "DescribeClientVpnRoutesResultTypeDef",
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     "VpnTunnelOptionsSpecificationTypeDef",
     "TunnelOptionTypeDef",
@@ -2247,16 +2172,16 @@
     "ModifyInstanceAttributeRequestRequestTypeDef",
     "InstanceAttributeTypeDef",
     "CreateEgressOnlyInternetGatewayResultTypeDef",
     "DescribeEgressOnlyInternetGatewaysResultTypeDef",
     "CreateInternetGatewayResultTypeDef",
     "DescribeInternetGatewaysResultTypeDef",
     "DescribeElasticGpusResultTypeDef",
-    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
-    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
+    "InstanceNetworkInterfaceSpecificationExtraOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
     "InstanceNetworkInterfaceSpecificationTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "AttachNetworkInterfaceRequestNetworkInterfaceAttachTypeDef",
     "AttachNetworkInterfaceRequestRequestTypeDef",
     "ModifyNetworkInterfaceAttributeRequestNetworkInterfaceModifyAttributeTypeDef",
     "ModifyNetworkInterfaceAttributeRequestRequestTypeDef",
     "EnableFastSnapshotRestoreErrorItemTypeDef",
@@ -2275,48 +2200,42 @@
     "GpuInfoTypeDef",
     "AssociateIamInstanceProfileResultTypeDef",
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
-    "ImportImageRequestRequestTypeDef",
-    "ImportSnapshotRequestRequestTypeDef",
     "CreateLocalGatewayRouteTableResultTypeDef",
     "DeleteLocalGatewayRouteTableResultTypeDef",
     "DescribeLocalGatewayRouteTablesResultTypeDef",
     "ImportInstanceRequestRequestTypeDef",
     "InferenceAcceleratorInfoTypeDef",
     "InstanceNetworkInterfaceAttachmentTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
+    "LaunchTemplateOverridesExtraOutputTypeDef",
+    "FleetLaunchTemplateOverridesTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
+    "LaunchTemplateOverridesTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
-    "FleetLaunchTemplateOverridesTypeDef",
-    "LaunchTemplateOverridesTypeDef",
     "StartInstancesResultTypeDef",
     "StopInstancesResultTypeDef",
     "TerminateInstancesResultTypeDef",
     "InstanceStatusTypeDef",
-    "SecurityGroupPaginatorTypeDef",
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
+    "RevokeSecurityGroupEgressResultTypeDef",
+    "RevokeSecurityGroupIngressResultTypeDef",
+    "SecurityGroupTypeDef",
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
+    "IpPermissionUnionTypeDef",
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
-    "RevokeSecurityGroupEgressResultTypeDef",
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
-    "RevokeSecurityGroupIngressResultTypeDef",
-    "SecurityGroupTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
     "StaleSecurityGroupTypeDef",
     "GetIpamDiscoveredAccountsResultTypeDef",
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     "GetIpamResourceCidrsResultTypeDef",
     "ModifyIpamResourceCidrResultTypeDef",
     "CreateIpamResourceDiscoveryResultTypeDef",
     "DeleteIpamResourceDiscoveryResultTypeDef",
@@ -2348,26 +2267,26 @@
     "CreateNetworkInterfacePermissionResultTypeDef",
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     "NeuronInfoTypeDef",
     "CreateVerifiedAccessTrustProviderResultTypeDef",
     "DeleteVerifiedAccessTrustProviderResultTypeDef",
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
     "AccessScopePathRequestTypeDef",
     "AccessScopePathTypeDef",
     "CancelReservedInstancesListingResultTypeDef",
     "CreateReservedInstancesListingResultTypeDef",
     "DescribeReservedInstancesListingsResultTypeDef",
     "DescribePublicIpv4PoolsResultTypeDef",
     "DescribeReservedInstancesOfferingsResultTypeDef",
     "DescribeReservedInstancesResultTypeDef",
     "AuthorizeSecurityGroupEgressResultTypeDef",
     "AuthorizeSecurityGroupIngressResultTypeDef",
     "DescribeSecurityGroupRulesResultTypeDef",
+    "BundleTaskTypeDef",
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     "DescribeScheduledInstancesResultTypeDef",
     "PurchaseScheduledInstancesResultTypeDef",
     "ScheduledInstancesLaunchSpecificationTypeDef",
     "CreateVpcEndpointResultTypeDef",
     "DescribeVpcEndpointsResultTypeDef",
     "ModifySecurityGroupRulesRequestRequestTypeDef",
@@ -2385,14 +2304,16 @@
     "AssociateTransitGatewayMulticastDomainResultTypeDef",
     "DisassociateTransitGatewayMulticastDomainResultTypeDef",
     "RejectTransitGatewayMulticastDomainAssociationsResultTypeDef",
     "AssociateSubnetCidrBlockResultTypeDef",
     "DisassociateSubnetCidrBlockResultTypeDef",
     "SubnetTypeDef",
     "GetReservedInstancesExchangeQuoteResultTypeDef",
+    "LoadBalancersConfigExtraOutputTypeDef",
+    "LoadBalancersConfigOutputTypeDef",
     "LoadBalancersConfigTypeDef",
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     "ModifyTrafficMirrorFilterRuleResultTypeDef",
     "TrafficMirrorFilterTypeDef",
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     "TransitGatewayConnectPeerTypeDef",
     "CreateTransitGatewayConnectResultTypeDef",
@@ -2455,61 +2376,163 @@
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
+    "AcceptAddressTransferRequestRequestTypeDef",
+    "AllocateAddressRequestRequestTypeDef",
+    "AllocateHostsRequestRequestTypeDef",
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CopyImageRequestRequestTypeDef",
+    "CopySnapshotRequestRequestTypeDef",
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    "CreateCapacityReservationRequestRequestTypeDef",
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    "CreateClientVpnEndpointRequestRequestTypeDef",
+    "CreateCoipPoolRequestRequestTypeDef",
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    "CreateFlowLogsRequestRequestTypeDef",
+    "CreateFpgaImageRequestRequestTypeDef",
+    "CreateImageRequestRequestTypeDef",
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    "CreateInternetGatewayRequestRequestTypeDef",
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    "CreateIpamPoolRequestRequestTypeDef",
+    "CreateIpamRequestRequestTypeDef",
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CreateIpamScopeRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    "CreateNatGatewayRequestRequestTypeDef",
+    "CreateNetworkAclRequestRequestTypeDef",
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    "CreatePlacementGroupRequestRequestTypeDef",
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    "CreateRouteTableRequestRequestTypeDef",
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    "CreateSecurityGroupRequestRequestTypeDef",
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    "CreateSnapshotsRequestRequestTypeDef",
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    "CreateSubnetRequestRequestTypeDef",
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    "CreateTransitGatewayRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    "CreateVpcEndpointRequestRequestTypeDef",
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    "CreateVpcRequestRequestTypeDef",
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    "CreateVpnGatewayRequestRequestTypeDef",
+    "ExportImageRequestRequestTypeDef",
+    "ImportImageRequestRequestTypeDef",
+    "ImportKeyPairRequestRequestTypeDef",
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    "ImportSnapshotRequestRequestTypeDef",
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    "PurchaseCapacityBlockRequestRequestTypeDef",
+    "PurchaseHostReservationRequestRequestTypeDef",
+    "RegisterImageRequestRequestTypeDef",
+    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
     "DescribeRouteTablesResultTypeDef",
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     "DescribeNetworkInterfaceAttributeResultTypeDef",
     "NetworkInterfaceTypeDef",
     "CreateDhcpOptionsResultTypeDef",
     "DescribeDhcpOptionsResultTypeDef",
     "DescribeHostsResultTypeDef",
     "BundleInstanceRequestRequestTypeDef",
-    "BundleTaskTypeDef",
+    "StorageUnionTypeDef",
     "DescribeImagesResultTypeDef",
     "DescribeClientVpnEndpointsResultTypeDef",
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     "VpnConnectionOptionsSpecificationTypeDef",
     "VpnConnectionOptionsTypeDef",
     "CreateNetworkAclResultTypeDef",
     "DescribeNetworkAclsResultTypeDef",
     "DisableFastSnapshotRestoresResultTypeDef",
     "ConversionTaskTypeDef",
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    "RunInstancesRequestSubnetCreateInstancesTypeDef",
+    "SpotFleetLaunchSpecificationExtraOutputTypeDef",
     "LaunchSpecificationTypeDef",
+    "SpotFleetLaunchSpecificationOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationUnionTypeDef",
     "RequestSpotLaunchSpecificationTypeDef",
-    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestSubnetCreateInstancesTypeDef",
     "SpotFleetLaunchSpecificationTypeDef",
     "RequestLaunchTemplateDataTypeDef",
     "EnableFastSnapshotRestoresResultTypeDef",
     "CreateNetworkInsightsPathResultTypeDef",
     "DescribeNetworkInsightsPathsResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
-    "FleetLaunchTemplateConfigRequestTypeDef",
-    "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
-    "GetSpotPlacementScoresRequestRequestTypeDef",
+    "LaunchTemplateConfigExtraOutputTypeDef",
     "FleetLaunchTemplateConfigTypeDef",
     "LaunchTemplateAndOverridesResponseTypeDef",
+    "LaunchTemplateConfigOutputTypeDef",
     "LaunchTemplateConfigTypeDef",
+    "FleetLaunchTemplateConfigRequestTypeDef",
+    "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
+    "GetSpotPlacementScoresRequestRequestTypeDef",
     "DescribeInstanceStatusResultTypeDef",
-    "DescribeSecurityGroupsResultPaginatorTypeDef",
     "DescribeSecurityGroupsResultTypeDef",
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
     "DescribeStaleSecurityGroupsResultTypeDef",
     "GetIpamDiscoveredPublicAddressesResultTypeDef",
     "ResponseLaunchTemplateDataTypeDef",
     "DescribeReservedInstancesModificationsResultTypeDef",
     "InstanceTypeInfoTypeDef",
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     "NetworkInsightsAccessScopeContentTypeDef",
+    "BundleInstanceResultTypeDef",
+    "CancelBundleTaskResultTypeDef",
+    "DescribeBundleTasksResultTypeDef",
     "RunScheduledInstancesRequestRequestTypeDef",
     "DescribeImportImageTasksResultTypeDef",
     "DescribeImportSnapshotTasksResultTypeDef",
     "CreateDefaultSubnetResultTypeDef",
     "CreateSubnetResultTypeDef",
     "DescribeSubnetsResultTypeDef",
     "CreateTrafficMirrorFilterResultTypeDef",
@@ -2527,36 +2550,36 @@
     "AcceptVpcPeeringConnectionResultTypeDef",
     "CreateVpcPeeringConnectionResultTypeDef",
     "DescribeVpcPeeringConnectionsResultTypeDef",
     "AccessScopeAnalysisFindingTypeDef",
     "NetworkInsightsAnalysisTypeDef",
     "CreateNetworkInterfaceResultTypeDef",
     "DescribeNetworkInterfacesResultTypeDef",
-    "BundleInstanceResultTypeDef",
-    "CancelBundleTaskResultTypeDef",
-    "DescribeBundleTasksResultTypeDef",
     "CreateVpnConnectionRequestRequestTypeDef",
     "VpnConnectionTypeDef",
     "DescribeConversionTasksResultTypeDef",
     "ImportInstanceResultTypeDef",
     "ImportVolumeResultTypeDef",
     "SpotInstanceRequestTypeDef",
+    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RequestSpotInstancesRequestRequestTypeDef",
     "CreateLaunchTemplateRequestRequestTypeDef",
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     "InstanceTypeDef",
-    "CreateFleetRequestRequestTypeDef",
-    "ModifyFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataExtraOutputTypeDef",
     "CreateFleetErrorTypeDef",
     "CreateFleetInstanceTypeDef",
     "DescribeFleetErrorTypeDef",
     "DescribeFleetsInstancesTypeDef",
-    "ModifySpotFleetRequestRequestRequestTypeDef",
-    "SpotFleetRequestConfigDataPaginatorTypeDef",
+    "SpotFleetRequestConfigDataOutputTypeDef",
+    "LaunchTemplateConfigUnionTypeDef",
     "SpotFleetRequestConfigDataTypeDef",
+    "CreateFleetRequestRequestTypeDef",
+    "ModifyFleetRequestRequestTypeDef",
     "GetLaunchTemplateDataResultTypeDef",
     "LaunchTemplateVersionTypeDef",
     "DescribeInstanceTypesResultTypeDef",
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     "GetNetworkInsightsAccessScopeContentResultTypeDef",
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
@@ -2571,22 +2594,22 @@
     "ModifyVpnTunnelOptionsResultTypeDef",
     "DescribeSpotInstanceRequestsResultTypeDef",
     "RequestSpotInstancesResultTypeDef",
     "ReservationResponseTypeDef",
     "ReservationTypeDef",
     "CreateFleetResultTypeDef",
     "FleetDataTypeDef",
-    "SpotFleetRequestConfigPaginatorTypeDef",
-    "RequestSpotFleetRequestRequestTypeDef",
     "SpotFleetRequestConfigTypeDef",
+    "ModifySpotFleetRequestRequestRequestTypeDef",
+    "RequestSpotFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataUnionTypeDef",
     "CreateLaunchTemplateVersionResultTypeDef",
     "DescribeLaunchTemplateVersionsResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeFleetsResultTypeDef",
-    "DescribeSpotFleetRequestsResponsePaginatorTypeDef",
     "DescribeSpotFleetRequestsResponseTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": NotRequired[int],
@@ -6927,95 +6950,95 @@
         "CarrierIp": NotRequired[str],
         "CustomerOwnedIp": NotRequired[str],
         "IpOwnerId": NotRequired[str],
         "PublicDnsName": NotRequired[str],
         "PublicIp": NotRequired[str],
     },
 )
-MemoryGiBPerVCpuRequestTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestTypeDef",
+MemoryGiBPerVCpuTypeDef = TypedDict(
+    "MemoryGiBPerVCpuTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-MemoryMiBRequestTypeDef = TypedDict(
-    "MemoryMiBRequestTypeDef",
+MemoryMiBTypeDef = TypedDict(
+    "MemoryMiBTypeDef",
     {
-        "Min": int,
+        "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-NetworkBandwidthGbpsRequestTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestTypeDef",
+NetworkBandwidthGbpsTypeDef = TypedDict(
+    "NetworkBandwidthGbpsTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-NetworkInterfaceCountRequestTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestTypeDef",
+NetworkInterfaceCountTypeDef = TypedDict(
+    "NetworkInterfaceCountTypeDef",
     {
         "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-TotalLocalStorageGBRequestTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestTypeDef",
+TotalLocalStorageGBTypeDef = TypedDict(
+    "TotalLocalStorageGBTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-VCpuCountRangeRequestTypeDef = TypedDict(
-    "VCpuCountRangeRequestTypeDef",
+VCpuCountRangeTypeDef = TypedDict(
+    "VCpuCountRangeTypeDef",
     {
-        "Min": int,
+        "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-MemoryGiBPerVCpuTypeDef = TypedDict(
-    "MemoryGiBPerVCpuTypeDef",
+MemoryGiBPerVCpuRequestTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-MemoryMiBTypeDef = TypedDict(
-    "MemoryMiBTypeDef",
+MemoryMiBRequestTypeDef = TypedDict(
+    "MemoryMiBRequestTypeDef",
     {
-        "Min": NotRequired[int],
+        "Min": int,
         "Max": NotRequired[int],
     },
 )
-NetworkBandwidthGbpsTypeDef = TypedDict(
-    "NetworkBandwidthGbpsTypeDef",
+NetworkBandwidthGbpsRequestTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-NetworkInterfaceCountTypeDef = TypedDict(
-    "NetworkInterfaceCountTypeDef",
+NetworkInterfaceCountRequestTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestTypeDef",
     {
         "Min": NotRequired[int],
         "Max": NotRequired[int],
     },
 )
-TotalLocalStorageGBTypeDef = TypedDict(
-    "TotalLocalStorageGBTypeDef",
+TotalLocalStorageGBRequestTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestTypeDef",
     {
         "Min": NotRequired[float],
         "Max": NotRequired[float],
     },
 )
-VCpuCountRangeTypeDef = TypedDict(
-    "VCpuCountRangeTypeDef",
+VCpuCountRangeRequestTypeDef = TypedDict(
+    "VCpuCountRangeRequestTypeDef",
     {
-        "Min": NotRequired[int],
+        "Min": int,
         "Max": NotRequired[int],
     },
 )
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": NotRequired[int],
@@ -7678,15 +7701,15 @@
 ReservedInstancesConfigurationTypeDef = TypedDict(
     "ReservedInstancesConfigurationTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "InstanceCount": NotRequired[int],
         "InstanceType": NotRequired[InstanceTypeType],
         "Platform": NotRequired[str],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
     },
 )
 ModifySnapshotTierRequestRequestTypeDef = TypedDict(
     "ModifySnapshotTierRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "StorageTier": NotRequired[Literal["archive"]],
@@ -8666,14 +8689,24 @@
         "NetworkInterfaceId": NotRequired[str],
         "Origin": NotRequired[RouteOriginType],
         "State": NotRequired[RouteStateType],
         "VpcPeeringConnectionId": NotRequired[str],
         "CoreNetworkArn": NotRequired[str],
     },
 )
+S3StorageOutputTypeDef = TypedDict(
+    "S3StorageOutputTypeDef",
+    {
+        "AWSAccessKeyId": NotRequired[str],
+        "Bucket": NotRequired[str],
+        "Prefix": NotRequired[str],
+        "UploadPolicy": NotRequired[bytes],
+        "UploadPolicySignature": NotRequired[str],
+    },
+)
 ScheduledInstanceRecurrenceTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceTypeDef",
     {
         "Frequency": NotRequired[str],
         "Interval": NotRequired[int],
         "OccurrenceDaySet": NotRequired[List[int]],
         "OccurrenceRelativeToEnd": NotRequired[bool],
@@ -9529,16 +9562,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeAddressTransfersResultTypeDef = TypedDict(
     "DescribeAddressTransfersResultTypeDef",
     {
         "AddressTransfers": List[AddressTransferTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DetachClassicLinkVpcResultTypeDef = TypedDict(
     "DetachClassicLinkVpcResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10337,26 +10370,26 @@
         "AttributeValues": NotRequired[List[AccountAttributeValueTypeDef]],
     },
 )
 DescribeFleetInstancesResultTypeDef = TypedDict(
     "DescribeFleetInstancesResultTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
-        "NextToken": str,
         "FleetId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetInstancesResponseTypeDef = TypedDict(
     "DescribeSpotFleetInstancesResponseTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
-        "NextToken": str,
         "SpotFleetRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpcEndpointServicePermissionsResultTypeDef = TypedDict(
     "ModifyVpcEndpointServicePermissionsResultTypeDef",
     {
         "AddedPrincipals": List[AddedPrincipalTypeDef],
         "ReturnValue": bool,
@@ -10874,35 +10907,56 @@
         "OutpostArn": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "StorageTier": NotRequired[StorageTierType],
         "RestoreExpiryTime": NotRequired[datetime],
         "SseType": NotRequired[SSETypeType],
     },
 )
+SpotFleetTagSpecificationExtraOutputTypeDef = TypedDict(
+    "SpotFleetTagSpecificationExtraOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
+SpotFleetTagSpecificationOutputTypeDef = TypedDict(
+    "SpotFleetTagSpecificationOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": NotRequired[ResourceTypeType],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
         "SubnetCidrReservationId": NotRequired[str],
         "SubnetId": NotRequired[str],
         "Cidr": NotRequired[str],
         "ReservationType": NotRequired[SubnetCidrReservationTypeType],
         "OwnerId": NotRequired[str],
         "Description": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-TagSpecificationPaginatorTypeDef = TypedDict(
-    "TagSpecificationPaginatorTypeDef",
+TagSpecificationExtraOutputTypeDef = TypedDict(
+    "TagSpecificationExtraOutputTypeDef",
+    {
+        "ResourceType": NotRequired[ResourceTypeType],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
+TagSpecificationOutputTypeDef = TypedDict(
+    "TagSpecificationOutputTypeDef",
     {
         "ResourceType": NotRequired[ResourceTypeType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 TagSpecificationTypeDef = TypedDict(
     "TagSpecificationTypeDef",
@@ -11011,16 +11065,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetIpamPoolAllocationsResultTypeDef = TypedDict(
     "GetIpamPoolAllocationsResultTypeDef",
     {
         "IpamPoolAllocations": List[IpamPoolAllocationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AnalysisAclRuleTypeDef = TypedDict(
     "AnalysisAclRuleTypeDef",
     {
         "Cidr": NotRequired[str],
         "Egress": NotRequired[bool],
@@ -11234,16 +11288,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayPolicyTableAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayPolicyTableAssociationsResultTypeDef",
     {
         "Associations": List[TransitGatewayPolicyTableAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateTransitGatewayRouteTableResultTypeDef = TypedDict(
     "AssociateTransitGatewayRouteTableResultTypeDef",
     {
         "Association": TransitGatewayAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11607,16 +11661,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamByoasnResultTypeDef = TypedDict(
     "DescribeIpamByoasnResultTypeDef",
     {
         "Byoasns": List[ByoasnTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ProvisionIpamByoasnResultTypeDef = TypedDict(
     "ProvisionIpamByoasnResultTypeDef",
     {
         "Byoasn": ByoasnTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11674,16 +11728,16 @@
         "ReservationType": NotRequired[CapacityReservationTypeType],
     },
 )
 DescribeCapacityBlockOfferingsResultTypeDef = TypedDict(
     "DescribeCapacityBlockOfferingsResultTypeDef",
     {
         "CapacityBlockOfferings": List[CapacityBlockOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CapacityReservationFleetTypeDef = TypedDict(
     "CapacityReservationFleetTypeDef",
     {
         "CapacityReservationFleetId": NotRequired[str],
         "CapacityReservationFleetArn": NotRequired[str],
@@ -11715,17 +11769,17 @@
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetGroupsForCapacityReservationResultTypeDef = TypedDict(
     "GetGroupsForCapacityReservationResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservationGroups": List[CapacityReservationGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 OnDemandOptionsRequestTypeDef = TypedDict(
     "OnDemandOptionsRequestTypeDef",
     {
         "AllocationStrategy": NotRequired[FleetOnDemandAllocationStrategyType],
         "CapacityReservationOptions": NotRequired[CapacityReservationOptionsRequestTypeDef],
@@ -11781,32 +11835,44 @@
         "CapacityReservationPreference": NotRequired[CapacityReservationPreferenceType],
         "CapacityReservationTarget": NotRequired[CapacityReservationTargetTypeDef],
     },
 )
 DescribeVpcClassicLinkDnsSupportResultTypeDef = TypedDict(
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     {
-        "NextToken": str,
         "Vpcs": List[ClassicLinkDnsSupportTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ClassicLinkInstanceTypeDef = TypedDict(
     "ClassicLinkInstanceTypeDef",
     {
         "Groups": NotRequired[List[GroupIdentifierTypeDef]],
         "InstanceId": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
+ClassicLoadBalancersConfigExtraOutputTypeDef = TypedDict(
+    "ClassicLoadBalancersConfigExtraOutputTypeDef",
+    {
+        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+    },
+)
+ClassicLoadBalancersConfigOutputTypeDef = TypedDict(
+    "ClassicLoadBalancersConfigOutputTypeDef",
+    {
+        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+    },
+)
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
-        "ClassicLoadBalancers": NotRequired[List[ClassicLoadBalancerTypeDef]],
+        "ClassicLoadBalancers": NotRequired[Sequence[ClassicLoadBalancerTypeDef]],
     },
 )
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
         "CertificateRevocationList": str,
         "Status": ClientCertificateRevocationListStatusTypeDef,
@@ -11922,16 +11988,16 @@
 )
 GetCoipPoolUsageResultTypeDef = TypedDict(
     "GetCoipPoolUsageResultTypeDef",
     {
         "CoipPoolId": str,
         "CoipAddressUsages": List[CoipAddressUsageTypeDef],
         "LocalGatewayRouteTableId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCoipCidrResultTypeDef = TypedDict(
     "CreateCoipCidrResultTypeDef",
     {
         "CoipCidr": CoipCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11952,16 +12018,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointConnectionNotificationsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionNotificationsResultTypeDef",
     {
         "ConnectionNotificationSet": List[ConnectionNotificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "ModifyInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "DryRun": NotRequired[bool],
@@ -12006,16 +12072,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchLocalGatewayRoutesResultTypeDef = TypedDict(
     "SearchLocalGatewayRoutesResultTypeDef",
     {
         "Routes": List[LocalGatewayRouteTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef = TypedDict(
     "CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef",
     {
         "Egress": bool,
         "Protocol": str,
@@ -15019,17 +15085,17 @@
         "Arn": NotRequired[str],
         "Statuses": NotRequired[List[IdFormatTypeDef]],
     },
 )
 DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef = TypedDict(
     "DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef",
     {
-        "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeBundleTasksRequestBundleTaskCompleteWaitTypeDef = TypedDict(
     "DescribeBundleTasksRequestBundleTaskCompleteWaitTypeDef",
     {
         "BundleIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[FilterTypeDef]],
@@ -15455,80 +15521,80 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeFastSnapshotRestoresResultTypeDef = TypedDict(
     "DescribeFastSnapshotRestoresResultTypeDef",
     {
         "FastSnapshotRestores": List[DescribeFastSnapshotRestoreSuccessItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostReservationOfferingsResultTypeDef = TypedDict(
     "DescribeHostReservationOfferingsResultTypeDef",
     {
-        "NextToken": str,
         "OfferingSet": List[HostOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceCreditSpecificationsResultTypeDef = TypedDict(
     "DescribeInstanceCreditSpecificationsResultTypeDef",
     {
         "InstanceCreditSpecifications": List[InstanceCreditSpecificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceTopologyResultTypeDef = TypedDict(
     "DescribeInstanceTopologyResultTypeDef",
     {
         "Instances": List[InstanceTopologyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstanceTypeOfferingsResultTypeDef = TypedDict(
     "DescribeInstanceTypeOfferingsResultTypeDef",
     {
         "InstanceTypeOfferings": List[InstanceTypeOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLockedSnapshotsResultTypeDef = TypedDict(
     "DescribeLockedSnapshotsResultTypeDef",
     {
         "Snapshots": List[LockedSnapshotsInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeMacHostsResultTypeDef = TypedDict(
     "DescribeMacHostsResultTypeDef",
     {
         "MacHosts": List[MacHostTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeMovingAddressesResultTypeDef = TypedDict(
     "DescribeMovingAddressesResultTypeDef",
     {
         "MovingAddressStatuses": List[MovingAddressStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePrefixListsResultTypeDef = TypedDict(
     "DescribePrefixListsResultTypeDef",
     {
-        "NextToken": str,
         "PrefixLists": List[PrefixListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegionsResultTypeDef = TypedDict(
     "DescribeRegionsResultTypeDef",
     {
         "Regions": List[RegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15558,41 +15624,41 @@
         "VolumeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSpotPriceHistoryResultTypeDef = TypedDict(
     "DescribeSpotPriceHistoryResultTypeDef",
     {
-        "NextToken": str,
         "SpotPriceHistory": List[SpotPriceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStoreImageTasksResultTypeDef = TypedDict(
     "DescribeStoreImageTasksResultTypeDef",
     {
         "StoreImageTaskResults": List[StoreImageTaskResultTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeTagsResultTypeDef = TypedDict(
     "DescribeTagsResultTypeDef",
     {
-        "NextToken": str,
         "Tags": List[TagDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVolumesModificationsResultTypeDef = TypedDict(
     "DescribeVolumesModificationsResultTypeDef",
     {
         "VolumesModifications": List[VolumeModificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVolumeResultTypeDef = TypedDict(
     "ModifyVolumeResultTypeDef",
     {
         "VolumeModification": VolumeModificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15928,29 +15994,29 @@
         "InstanceTypes": NotRequired[List[str]],
     },
 )
 GetAssociatedIpv6PoolCidrsResultTypeDef = TypedDict(
     "GetAssociatedIpv6PoolCidrsResultTypeDef",
     {
         "Ipv6CidrAssociations": List[Ipv6CidrAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetCapacityReservationUsageResultTypeDef = TypedDict(
     "GetCapacityReservationUsageResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservationId": str,
         "InstanceType": str,
         "TotalInstanceCount": int,
         "AvailableInstanceCount": int,
         "State": CapacityReservationStateType,
         "InstanceUsages": List[InstanceUsageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDefaultCreditSpecificationResultTypeDef = TypedDict(
     "GetDefaultCreditSpecificationResultTypeDef",
     {
         "InstanceFamilyCreditSpecification": InstanceFamilyCreditSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15991,87 +16057,87 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetInstanceTypesFromInstanceRequirementsResultTypeDef = TypedDict(
     "GetInstanceTypesFromInstanceRequirementsResultTypeDef",
     {
         "InstanceTypes": List[InstanceTypeInfoFromInstanceRequirementsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamAddressHistoryResultTypeDef = TypedDict(
     "GetIpamAddressHistoryResultTypeDef",
     {
         "HistoryRecords": List[IpamAddressHistoryRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetManagedPrefixListAssociationsResultTypeDef = TypedDict(
     "GetManagedPrefixListAssociationsResultTypeDef",
     {
         "PrefixListAssociations": List[PrefixListAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetManagedPrefixListEntriesResultTypeDef = TypedDict(
     "GetManagedPrefixListEntriesResultTypeDef",
     {
         "Entries": List[PrefixListEntryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ReservedInstanceReservationValueTypeDef = TypedDict(
     "ReservedInstanceReservationValueTypeDef",
     {
         "ReservationValue": NotRequired[ReservationValueTypeDef],
         "ReservedInstanceId": NotRequired[str],
     },
 )
 GetSpotPlacementScoresResultTypeDef = TypedDict(
     "GetSpotPlacementScoresResultTypeDef",
     {
         "SpotPlacementScores": List[SpotPlacementScoreTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayAttachmentPropagationsResultTypeDef = TypedDict(
     "GetTransitGatewayAttachmentPropagationsResultTypeDef",
     {
         "TransitGatewayAttachmentPropagations": List[TransitGatewayAttachmentPropagationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayRouteTableAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAssociationsResultTypeDef",
     {
         "Associations": List[TransitGatewayRouteTableAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayRouteTablePropagationsResultTypeDef = TypedDict(
     "GetTransitGatewayRouteTablePropagationsResultTypeDef",
     {
         "TransitGatewayRouteTablePropagations": List[TransitGatewayRouteTablePropagationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVpnConnectionDeviceTypesResultTypeDef = TypedDict(
     "GetVpnConnectionDeviceTypesResultTypeDef",
     {
         "VpnConnectionDeviceTypes": List[VpnConnectionDeviceTypeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVpnTunnelReplacementStatusResultTypeDef = TypedDict(
     "GetVpnTunnelReplacementStatusResultTypeDef",
     {
         "VpnConnectionId": str,
         "TransitGatewayId": str,
@@ -16128,16 +16194,16 @@
         "UserBucket": NotRequired[UserBucketTypeDef],
     },
 )
 ListImagesInRecycleBinResultTypeDef = TypedDict(
     "ListImagesInRecycleBinResultTypeDef",
     {
         "Images": List[ImageRecycleBinInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LocalGatewayRouteTableTypeDef = TypedDict(
     "LocalGatewayRouteTableTypeDef",
     {
         "LocalGatewayRouteTableId": NotRequired[str],
         "LocalGatewayRouteTableArn": NotRequired[str],
@@ -16210,45 +16276,45 @@
     {
         "Association": NotRequired[InstanceNetworkInterfaceAssociationTypeDef],
         "Primary": NotRequired[bool],
         "PrivateDnsName": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
     },
 )
-InstanceRequirementsRequestTypeDef = TypedDict(
-    "InstanceRequirementsRequestTypeDef",
+InstanceRequirementsExtraOutputTypeDef = TypedDict(
+    "InstanceRequirementsExtraOutputTypeDef",
     {
-        "VCpuCount": VCpuCountRangeRequestTypeDef,
-        "MemoryMiB": MemoryMiBRequestTypeDef,
-        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
-        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuRequestTypeDef],
-        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
-        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
+        "MemoryMiB": NotRequired[MemoryMiBTypeDef],
+        "CpuManufacturers": NotRequired[List[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
+        "ExcludedInstanceTypes": NotRequired[List[str]],
+        "InstanceGenerations": NotRequired[List[InstanceGenerationType]],
         "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
         "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
         "BareMetal": NotRequired[BareMetalType],
         "BurstablePerformance": NotRequired[BurstablePerformanceType],
         "RequireHibernateSupport": NotRequired[bool],
-        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountRequestTypeDef],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountTypeDef],
         "LocalStorage": NotRequired[LocalStorageType],
-        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
-        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBRequestTypeDef],
-        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsRequestTypeDef],
-        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
-        "AcceleratorCount": NotRequired[AcceleratorCountRequestTypeDef],
-        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
-        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
-        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBRequestTypeDef],
-        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsRequestTypeDef],
-        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "LocalStorageTypes": NotRequired[List[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsTypeDef],
+        "AcceleratorTypes": NotRequired[List[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountTypeDef],
+        "AcceleratorManufacturers": NotRequired[List[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[List[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
+        "AllowedInstanceTypes": NotRequired[List[str]],
         "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
     },
 )
-InstanceRequirementsTypeDef = TypedDict(
-    "InstanceRequirementsTypeDef",
+InstanceRequirementsOutputTypeDef = TypedDict(
+    "InstanceRequirementsOutputTypeDef",
     {
         "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
         "MemoryMiB": NotRequired[MemoryMiBTypeDef],
         "CpuManufacturers": NotRequired[List[CpuManufacturerType]],
         "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
         "ExcludedInstanceTypes": NotRequired[List[str]],
         "InstanceGenerations": NotRequired[List[InstanceGenerationType]],
@@ -16268,14 +16334,72 @@
         "AcceleratorNames": NotRequired[List[AcceleratorNameType]],
         "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
         "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
         "AllowedInstanceTypes": NotRequired[List[str]],
         "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
     },
 )
+InstanceRequirementsTypeDef = TypedDict(
+    "InstanceRequirementsTypeDef",
+    {
+        "VCpuCount": NotRequired[VCpuCountRangeTypeDef],
+        "MemoryMiB": NotRequired[MemoryMiBTypeDef],
+        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuTypeDef],
+        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
+        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "BareMetal": NotRequired[BareMetalType],
+        "BurstablePerformance": NotRequired[BurstablePerformanceType],
+        "RequireHibernateSupport": NotRequired[bool],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountTypeDef],
+        "LocalStorage": NotRequired[LocalStorageType],
+        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsTypeDef],
+        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountTypeDef],
+        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsTypeDef],
+        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
+    },
+)
+InstanceRequirementsRequestTypeDef = TypedDict(
+    "InstanceRequirementsRequestTypeDef",
+    {
+        "VCpuCount": VCpuCountRangeRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
+        "CpuManufacturers": NotRequired[Sequence[CpuManufacturerType]],
+        "MemoryGiBPerVCpu": NotRequired[MemoryGiBPerVCpuRequestTypeDef],
+        "ExcludedInstanceTypes": NotRequired[Sequence[str]],
+        "InstanceGenerations": NotRequired[Sequence[InstanceGenerationType]],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "BareMetal": NotRequired[BareMetalType],
+        "BurstablePerformance": NotRequired[BurstablePerformanceType],
+        "RequireHibernateSupport": NotRequired[bool],
+        "NetworkInterfaceCount": NotRequired[NetworkInterfaceCountRequestTypeDef],
+        "LocalStorage": NotRequired[LocalStorageType],
+        "LocalStorageTypes": NotRequired[Sequence[LocalStorageTypeType]],
+        "TotalLocalStorageGB": NotRequired[TotalLocalStorageGBRequestTypeDef],
+        "BaselineEbsBandwidthMbps": NotRequired[BaselineEbsBandwidthMbpsRequestTypeDef],
+        "AcceleratorTypes": NotRequired[Sequence[AcceleratorTypeType]],
+        "AcceleratorCount": NotRequired[AcceleratorCountRequestTypeDef],
+        "AcceleratorManufacturers": NotRequired[Sequence[AcceleratorManufacturerType]],
+        "AcceleratorNames": NotRequired[Sequence[AcceleratorNameType]],
+        "AcceleratorTotalMemoryMiB": NotRequired[AcceleratorTotalMemoryMiBRequestTypeDef],
+        "NetworkBandwidthGbps": NotRequired[NetworkBandwidthGbpsRequestTypeDef],
+        "AllowedInstanceTypes": NotRequired[Sequence[str]],
+        "MaxSpotPriceAsPercentageOfOptimalOnDemandPrice": NotRequired[int],
+    },
+)
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": NotRequired[InstanceStateTypeDef],
         "InstanceId": NotRequired[str],
         "PreviousState": NotRequired[InstanceStateTypeDef],
     },
@@ -16290,16 +16414,28 @@
 ModifyInstanceEventStartTimeResultTypeDef = TypedDict(
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-IpPermissionPaginatorTypeDef = TypedDict(
-    "IpPermissionPaginatorTypeDef",
+IpPermissionExtraExtraOutputTypeDef = TypedDict(
+    "IpPermissionExtraExtraOutputTypeDef",
+    {
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "IpRanges": NotRequired[List[IpRangeTypeDef]],
+        "Ipv6Ranges": NotRequired[List[Ipv6RangeTypeDef]],
+        "PrefixListIds": NotRequired[List[PrefixListIdTypeDef]],
+        "ToPort": NotRequired[int],
+        "UserIdGroupPairs": NotRequired[List[UserIdGroupPairTypeDef]],
+    },
+)
+IpPermissionOutputTypeDef = TypedDict(
+    "IpPermissionOutputTypeDef",
     {
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "IpRanges": NotRequired[List[IpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[List[Ipv6RangeTypeDef]],
         "PrefixListIds": NotRequired[List[PrefixListIdTypeDef]],
         "ToPort": NotRequired[int],
@@ -16506,16 +16642,16 @@
         "SpotOptions": NotRequired[LaunchTemplateSpotMarketOptionsTypeDef],
     },
 )
 ListSnapshotsInRecycleBinResultTypeDef = TypedDict(
     "ListSnapshotsInRecycleBinResultTypeDef",
     {
         "Snapshots": List[SnapshotRecycleBinInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LoadPermissionModificationsTypeDef = TypedDict(
     "LoadPermissionModificationsTypeDef",
     {
         "Add": NotRequired[Sequence[LoadPermissionRequestTypeDef]],
         "Remove": NotRequired[Sequence[LoadPermissionRequestTypeDef]],
@@ -16853,15 +16989,15 @@
         "CurrencyCode": NotRequired[Literal["USD"]],
         "InstanceTenancy": NotRequired[TenancyType],
         "Marketplace": NotRequired[bool],
         "OfferingClass": NotRequired[OfferingClassTypeType],
         "OfferingType": NotRequired[OfferingTypeValuesType],
         "PricingDetails": NotRequired[List[PricingDetailTypeDef]],
         "RecurringCharges": NotRequired[List[RecurringChargeTypeDef]],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
     },
 )
 ReservedInstancesTypeDef = TypedDict(
     "ReservedInstancesTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "Duration": NotRequired[int],
@@ -16875,15 +17011,15 @@
         "State": NotRequired[ReservedInstanceStateType],
         "UsagePrice": NotRequired[float],
         "CurrencyCode": NotRequired[Literal["USD"]],
         "InstanceTenancy": NotRequired[TenancyType],
         "OfferingClass": NotRequired[OfferingClassTypeType],
         "OfferingType": NotRequired[OfferingTypeValuesType],
         "RecurringCharges": NotRequired[List[RecurringChargeTypeDef]],
-        "Scope": NotRequired[scopeType],
+        "Scope": NotRequired[ScopeType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 SecurityGroupRuleTypeDef = TypedDict(
     "SecurityGroupRuleTypeDef",
     {
         "SecurityGroupRuleId": NotRequired[str],
@@ -16918,14 +17054,20 @@
 RegisterTransitGatewayMulticastGroupSourcesResultTypeDef = TypedDict(
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
     {
         "RegisteredMulticastGroupSources": TransitGatewayMulticastRegisteredGroupSourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StorageOutputTypeDef = TypedDict(
+    "StorageOutputTypeDef",
+    {
+        "S3": NotRequired[S3StorageOutputTypeDef],
+    },
+)
 ScheduledInstanceAvailabilityTypeDef = TypedDict(
     "ScheduledInstanceAvailabilityTypeDef",
     {
         "AvailabilityZone": NotRequired[str],
         "AvailableInstanceCount": NotRequired[int],
         "FirstSlotStartTime": NotRequired[datetime],
         "HourlyPrice": NotRequired[str],
@@ -16988,16 +17130,16 @@
         "SubnetId": NotRequired[str],
     },
 )
 SearchTransitGatewayMulticastGroupsResultTypeDef = TypedDict(
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     {
         "MulticastGroups": List[TransitGatewayMulticastGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": NotRequired[str],
         "VpcEndpointType": NotRequired[VpcEndpointTypeType],
@@ -17146,18 +17288,30 @@
 TargetReservationValueTypeDef = TypedDict(
     "TargetReservationValueTypeDef",
     {
         "ReservationValue": NotRequired[ReservationValueTypeDef],
         "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
     },
 )
+TargetGroupsConfigExtraOutputTypeDef = TypedDict(
+    "TargetGroupsConfigExtraOutputTypeDef",
+    {
+        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+    },
+)
+TargetGroupsConfigOutputTypeDef = TypedDict(
+    "TargetGroupsConfigOutputTypeDef",
+    {
+        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+    },
+)
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
-        "TargetGroups": NotRequired[List[TargetGroupTypeDef]],
+        "TargetGroups": NotRequired[Sequence[TargetGroupTypeDef]],
     },
 )
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
         "TrafficMirrorFilterRuleId": NotRequired[str],
         "TrafficMirrorFilterId": NotRequired[str],
@@ -17507,16 +17661,16 @@
         "LoadBalancers": NotRequired[List[AnalysisComponentTypeDef]],
     },
 )
 DescribeAddressesAttributeResultTypeDef = TypedDict(
     "DescribeAddressesAttributeResultTypeDef",
     {
         "Addresses": List[AddressAttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyAddressAttributeResultTypeDef = TypedDict(
     "ModifyAddressAttributeResultTypeDef",
     {
         "Address": AddressAttributeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17536,16 +17690,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointServicePermissionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
     {
         "AllowedPrincipals": List[AllowedPrincipalTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCarrierGatewayResultTypeDef = TypedDict(
     "CreateCarrierGatewayResultTypeDef",
     {
         "CarrierGateway": CarrierGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17558,16 +17712,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCarrierGatewaysResultTypeDef = TypedDict(
     "DescribeCarrierGatewaysResultTypeDef",
     {
         "CarrierGateways": List[CarrierGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCoipPoolResultTypeDef = TypedDict(
     "CreateCoipPoolResultTypeDef",
     {
         "CoipPool": CoipPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17580,16 +17734,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCoipPoolsResultTypeDef = TypedDict(
     "DescribeCoipPoolsResultTypeDef",
     {
         "CoipPools": List[CoipPoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateCustomerGatewayResultTypeDef = TypedDict(
     "CreateCustomerGatewayResultTypeDef",
     {
         "CustomerGateway": CustomerGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17617,24 +17771,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInstanceConnectEndpointsResultTypeDef = TypedDict(
     "DescribeInstanceConnectEndpointsResultTypeDef",
     {
         "InstanceConnectEndpoints": List[Ec2InstanceConnectEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostReservationsResultTypeDef = TypedDict(
     "DescribeHostReservationsResultTypeDef",
     {
         "HostReservationSet": List[HostReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "AssociateInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "AssociationTarget": InstanceEventWindowAssociationRequestTypeDef,
@@ -17668,16 +17822,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamResourceDiscoveryAssociationsResultTypeDef = TypedDict(
     "DescribeIpamResourceDiscoveryAssociationsResultTypeDef",
     {
         "IpamResourceDiscoveryAssociations": List[IpamResourceDiscoveryAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateIpamResourceDiscoveryResultTypeDef = TypedDict(
     "DisassociateIpamResourceDiscoveryResultTypeDef",
     {
         "IpamResourceDiscoveryAssociation": IpamResourceDiscoveryAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17696,17 +17850,17 @@
         "IpamScope": IpamScopeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamScopesResultTypeDef = TypedDict(
     "DescribeIpamScopesResultTypeDef",
     {
-        "NextToken": str,
         "IpamScopes": List[IpamScopeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamScopeResultTypeDef = TypedDict(
     "ModifyIpamScopeResultTypeDef",
     {
         "IpamScope": IpamScopeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17726,16 +17880,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLaunchTemplatesResultTypeDef = TypedDict(
     "DescribeLaunchTemplatesResultTypeDef",
     {
         "LaunchTemplates": List[LaunchTemplateTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyLaunchTemplateResultTypeDef = TypedDict(
     "ModifyLaunchTemplateResultTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17757,16 +17911,16 @@
 )
 DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef",
     {
         "LocalGatewayRouteTableVirtualInterfaceGroupAssociations": List[
             LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef
         ],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateLocalGatewayRouteTableVpcAssociationResultTypeDef = TypedDict(
     "CreateLocalGatewayRouteTableVpcAssociationResultTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociation": LocalGatewayRouteTableVpcAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17779,40 +17933,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociations": List[LocalGatewayRouteTableVpcAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewaysResultTypeDef = TypedDict(
     "DescribeLocalGatewaysResultTypeDef",
     {
         "LocalGateways": List[LocalGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef = TypedDict(
     "DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef",
     {
         "LocalGatewayVirtualInterfaceGroups": List[LocalGatewayVirtualInterfaceGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeLocalGatewayVirtualInterfacesResultTypeDef = TypedDict(
     "DescribeLocalGatewayVirtualInterfacesResultTypeDef",
     {
         "LocalGatewayVirtualInterfaces": List[LocalGatewayVirtualInterfaceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateManagedPrefixListResultTypeDef = TypedDict(
     "CreateManagedPrefixListResultTypeDef",
     {
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17824,17 +17978,17 @@
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeManagedPrefixListsResultTypeDef = TypedDict(
     "DescribeManagedPrefixListsResultTypeDef",
     {
-        "NextToken": str,
         "PrefixLists": List[ManagedPrefixListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyManagedPrefixListResultTypeDef = TypedDict(
     "ModifyManagedPrefixListResultTypeDef",
     {
         "PrefixList": ManagedPrefixListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17847,31 +18001,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalyses": List[NetworkInsightsAccessScopeAnalysisTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartNetworkInsightsAccessScopeAnalysisResultTypeDef = TypedDict(
     "StartNetworkInsightsAccessScopeAnalysisResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysis": NetworkInsightsAccessScopeAnalysisTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsAccessScopesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAccessScopesResultTypeDef",
     {
         "NetworkInsightsAccessScopes": List[NetworkInsightsAccessScopeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreatePlacementGroupResultTypeDef = TypedDict(
     "CreatePlacementGroupResultTypeDef",
     {
         "PlacementGroup": PlacementGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17891,47 +18045,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeReplaceRootVolumeTasksResultTypeDef = TypedDict(
     "DescribeReplaceRootVolumeTasksResultTypeDef",
     {
         "ReplaceRootVolumeTasks": List[ReplaceRootVolumeTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetSecurityGroupsForVpcResultTypeDef = TypedDict(
     "GetSecurityGroupsForVpcResultTypeDef",
     {
-        "NextToken": str,
         "SecurityGroupForVpcs": List[SecurityGroupForVpcTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateSnapshotsResultTypeDef = TypedDict(
     "CreateSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSnapshotTierStatusResultTypeDef = TypedDict(
     "DescribeSnapshotTierStatusResultTypeDef",
     {
         "SnapshotTierStatuses": List[SnapshotTierStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateSubnetCidrReservationResultTypeDef = TypedDict(
     "CreateSubnetCidrReservationResultTypeDef",
     {
         "SubnetCidrReservation": SubnetCidrReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -17945,93 +18099,16 @@
     },
 )
 GetSubnetCidrReservationsResultTypeDef = TypedDict(
     "GetSubnetCidrReservationsResultTypeDef",
     {
         "SubnetIpv4CidrReservations": List[SubnetCidrReservationTypeDef],
         "SubnetIpv6CidrReservations": List[SubnetCidrReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-AcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "AcceptAddressTransferRequestRequestTypeDef",
-    {
-        "Address": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-AllocateAddressRequestRequestTypeDef = TypedDict(
-    "AllocateAddressRequestRequestTypeDef",
-    {
-        "Domain": NotRequired[DomainTypeType],
-        "Address": NotRequired[str],
-        "PublicIpv4Pool": NotRequired[str],
-        "NetworkBorderGroup": NotRequired[str],
-        "CustomerOwnedIpv4Pool": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-AllocateHostsRequestRequestTypeDef = TypedDict(
-    "AllocateHostsRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "AutoPlacement": NotRequired[AutoPlacementType],
-        "ClientToken": NotRequired[str],
-        "InstanceType": NotRequired[str],
-        "InstanceFamily": NotRequired[str],
-        "Quantity": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "HostRecovery": NotRequired[HostRecoveryType],
-        "OutpostArn": NotRequired[str],
-        "HostMaintenance": NotRequired[HostMaintenanceType],
-        "AssetIds": NotRequired[Sequence[str]],
-    },
-)
-AssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "IpamResourceDiscoveryId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CopyImageRequestRequestTypeDef = TypedDict(
-    "CopyImageRequestRequestTypeDef",
-    {
-        "Name": str,
-        "SourceImageId": str,
-        "SourceRegion": str,
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "DestinationOutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "CopyImageTags": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CopySnapshotRequestRequestTypeDef = TypedDict(
-    "CopySnapshotRequestRequestTypeDef",
-    {
-        "SourceRegion": str,
-        "SourceSnapshotId": str,
-        "Description": NotRequired[str],
-        "DestinationOutpostArn": NotRequired[str],
-        "DestinationRegion": NotRequired[str],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "PresignedUrl": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
+        "NextToken": NotRequired[str],
     },
 )
 CopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
     "CopySnapshotRequestSnapshotCopyTypeDef",
     {
         "SourceRegion": str,
         "Description": NotRequired[str],
@@ -18040,383 +18117,22 @@
         "Encrypted": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "PresignedUrl": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
-        "TotalTargetCapacity": int,
-        "AllocationStrategy": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "Tenancy": NotRequired[Literal["default"]],
-        "EndDate": NotRequired[TimestampTypeDef],
-        "InstanceMatchCriteria": NotRequired[Literal["open"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "CreateCapacityReservationRequestRequestTypeDef",
-    {
-        "InstanceType": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "InstanceCount": int,
-        "ClientToken": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "Tenancy": NotRequired[CapacityReservationTenancyType],
-        "EbsOptimized": NotRequired[bool],
-        "EphemeralStorage": NotRequired[bool],
-        "EndDate": NotRequired[TimestampTypeDef],
-        "EndDateType": NotRequired[EndDateTypeType],
-        "InstanceMatchCriteria": NotRequired[InstanceMatchCriteriaType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "OutpostArn": NotRequired[str],
-        "PlacementGroupArn": NotRequired[str],
-    },
-)
-CreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "CreateCoipPoolRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-        "BgpAsn": NotRequired[int],
-        "PublicIp": NotRequired[str],
-        "CertificateArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DeviceName": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "CreateFlowLogsRequestRequestTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ResourceType": FlowLogsResourceTypeType,
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "DeliverLogsPermissionArn": NotRequired[str],
-        "DeliverCrossAccountRole": NotRequired[str],
-        "LogGroupName": NotRequired[str],
-        "TrafficType": NotRequired[TrafficTypeType],
-        "LogDestinationType": NotRequired[LogDestinationTypeType],
-        "LogDestination": NotRequired[str],
-        "LogFormat": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MaxAggregationInterval": NotRequired[int],
-        "DestinationOptions": NotRequired[DestinationOptionsRequestTypeDef],
-    },
-)
-CreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "CreateFpgaImageRequestRequestTypeDef",
-    {
-        "InputStorageLocation": StorageLocationTypeDef,
-        "DryRun": NotRequired[bool],
-        "LogsStorageLocation": NotRequired[StorageLocationTypeDef],
-        "Description": NotRequired[str],
-        "Name": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "DryRun": NotRequired[bool],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "PreserveClientIp": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Name": NotRequired[str],
-        "TimeRanges": NotRequired[Sequence[InstanceEventWindowTimeRangeRequestTypeDef]],
-        "CronExpression": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
-        "InstanceId": str,
-        "TargetEnvironment": ExportEnvironmentType,
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateInternetGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    {
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "CreateIpamPoolRequestRequestTypeDef",
-    {
-        "IpamScopeId": str,
-        "AddressFamily": AddressFamilyType,
-        "DryRun": NotRequired[bool],
-        "Locale": NotRequired[str],
-        "SourceIpamPoolId": NotRequired[str],
-        "Description": NotRequired[str],
-        "AutoImport": NotRequired[bool],
-        "PubliclyAdvertisable": NotRequired[bool],
-        "AllocationMinNetmaskLength": NotRequired[int],
-        "AllocationMaxNetmaskLength": NotRequired[int],
-        "AllocationDefaultNetmaskLength": NotRequired[int],
-        "AllocationResourceTags": NotRequired[Sequence[RequestIpamResourceTagTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "AwsService": NotRequired[Literal["ec2"]],
-        "PublicIpSource": NotRequired[IpamPoolPublicIpSourceType],
-        "SourceResource": NotRequired[IpamPoolSourceResourceRequestTypeDef],
-    },
-)
-CreateIpamRequestRequestTypeDef = TypedDict(
-    "CreateIpamRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "Tier": NotRequired[IpamTierType],
-    },
-)
-CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "CreateIpamScopeRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "DryRun": NotRequired[bool],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateKeyPairRequestRequestTypeDef = TypedDict(
-    "CreateKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "DryRun": NotRequired[bool],
-        "KeyType": NotRequired[KeyTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "KeyFormat": NotRequired[KeyFormatType],
-    },
-)
-CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "DryRun": NotRequired[bool],
-        "KeyType": NotRequired[KeyTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "KeyFormat": NotRequired[KeyFormatType],
-    },
-)
-CreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "LocalGatewayId": str,
-        "Mode": NotRequired[LocalGatewayRouteTableModeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayVirtualInterfaceGroupId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "PrefixListName": str,
-        "MaxEntries": int,
-        "AddressFamily": str,
-        "DryRun": NotRequired[bool],
-        "Entries": NotRequired[Sequence[AddPrefixListEntryTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "CreateNatGatewayRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "AllocationId": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ConnectivityType": NotRequired[ConnectivityTypeType],
-        "PrivateIpAddress": NotRequired[str],
-        "SecondaryAllocationIds": NotRequired[Sequence[str]],
-        "SecondaryPrivateIpAddresses": NotRequired[Sequence[str]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-    },
-)
-CreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "CreateNetworkAclRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
 CreateNetworkAclRequestVpcCreateNetworkAclTypeDef = TypedDict(
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
     {
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "ClientToken": NotRequired[str],
     },
 )
-CreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Groups": NotRequired[Sequence[str]],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
-        "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
-        "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
-        "Ipv6PrefixCount": NotRequired[int],
-        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "EnablePrimaryIpv6": NotRequired[bool],
-        "ConnectionTrackingSpecification": NotRequired[
-            ConnectionTrackingSpecificationRequestTypeDef
-        ],
-    },
-)
-CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "SubnetId": str,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Groups": NotRequired[Sequence[str]],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
-        "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
-        "SecondaryPrivateIpAddressCount": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
-        "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
-        "Ipv6PrefixCount": NotRequired[int],
-        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "EnablePrimaryIpv6": NotRequired[bool],
-        "ConnectionTrackingSpecification": NotRequired[
-            ConnectionTrackingSpecificationRequestTypeDef
-        ],
-    },
-)
 CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef = TypedDict(
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
     {
         "Description": NotRequired[str],
         "DryRun": NotRequired[bool],
         "Groups": NotRequired[Sequence[str]],
         "Ipv6AddressCount": NotRequired[int],
@@ -18433,207 +18149,40 @@
         "ClientToken": NotRequired[str],
         "EnablePrimaryIpv6": NotRequired[bool],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
 )
-CreatePlacementGroupRequestRequestTypeDef = TypedDict(
-    "CreatePlacementGroupRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupName": NotRequired[str],
-        "Strategy": NotRequired[PlacementStrategyType],
-        "PartitionCount": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SpreadLevel": NotRequired[SpreadLevelType],
-    },
-)
-CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupName": NotRequired[str],
-        "Strategy": NotRequired[PlacementStrategyType],
-        "PartitionCount": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SpreadLevel": NotRequired[SpreadLevelType],
-    },
-)
-CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ImageId": NotRequired[str],
-        "DeleteReplacedRootVolume": NotRequired[bool],
-    },
-)
-CreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "ObjectKey": str,
-        "Name": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateRouteTableRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-    },
-)
 CreateRouteTableRequestVpcCreateRouteTableTypeDef = TypedDict(
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
     {
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "ClientToken": NotRequired[str],
     },
 )
-CreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "CreateSecurityGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-        "VpcId": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-        "VpcId": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
 CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef = TypedDict(
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupName": str,
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateSnapshotRequestRequestTypeDef = TypedDict(
-    "CreateSnapshotRequestRequestTypeDef",
-    {
-        "VolumeId": str,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "VolumeId": str,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
 CreateSnapshotRequestVolumeCreateSnapshotTypeDef = TypedDict(
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
     {
         "Description": NotRequired[str],
         "OutpostArn": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
-CreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "CreateSnapshotsRequestRequestTypeDef",
-    {
-        "InstanceSpecification": InstanceSpecificationTypeDef,
-        "Description": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "CopyTagsFromSource": NotRequired[Literal["volume"]],
-    },
-)
-CreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Cidr": str,
-        "ReservationType": SubnetCidrReservationTypeType,
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateSubnetRequestRequestTypeDef = TypedDict(
-    "CreateSubnetRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "CidrBlock": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Ipv6Native": NotRequired[bool],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-    },
-)
-CreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AvailabilityZone": NotRequired[str],
-        "AvailabilityZoneId": NotRequired[str],
-        "CidrBlock": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "Ipv6Native": NotRequired[bool],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-    },
-)
 CreateSubnetRequestVpcCreateSubnetTypeDef = TypedDict(
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
     {
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "AvailabilityZone": NotRequired[str],
         "AvailabilityZoneId": NotRequired[str],
         "CidrBlock": NotRequired[str],
@@ -18643,437 +18192,39 @@
         "Ipv6Native": NotRequired[bool],
         "Ipv4IpamPoolId": NotRequired[str],
         "Ipv4NetmaskLength": NotRequired[int],
         "Ipv6IpamPoolId": NotRequired[str],
         "Ipv6NetmaskLength": NotRequired[int],
     },
 )
-CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "TrafficMirrorTargetId": str,
-        "TrafficMirrorFilterId": str,
-        "SessionNumber": int,
-        "PacketLength": NotRequired[int],
-        "VirtualNetworkId": NotRequired[int],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": NotRequired[str],
-        "NetworkLoadBalancerArn": NotRequired[str],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "GatewayLoadBalancerEndpointId": NotRequired[str],
-    },
-)
-CreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAttachmentId": str,
-        "PeerAddress": str,
-        "InsideCidrBlocks": Sequence[str],
-        "TransitGatewayAddress": NotRequired[str],
-        "BgpOptions": NotRequired[TransitGatewayConnectRequestBgpOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TransportTransitGatewayAttachmentId": str,
-        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "Options": NotRequired[CreateTransitGatewayMulticastDomainRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "PeerTransitGatewayId": str,
-        "PeerAccountId": str,
-        "PeerRegion": str,
-        "Options": NotRequired[CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "Options": NotRequired[TransitGatewayRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TransitGatewayRouteTableId": str,
-        "PeeringAttachmentId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "VpcId": str,
-        "SubnetIds": Sequence[str],
-        "Options": NotRequired[CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-    },
-)
-CreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "VerifiedAccessGroupId": str,
-        "EndpointType": VerifiedAccessEndpointTypeType,
-        "AttachmentType": Literal["vpc"],
-        "DomainCertificateArn": str,
-        "ApplicationDomain": str,
-        "EndpointDomainPrefix": str,
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "LoadBalancerOptions": NotRequired[CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef],
-        "NetworkInterfaceOptions": NotRequired[CreateVerifiedAccessEndpointEniOptionsTypeDef],
-        "Description": NotRequired[str],
-        "PolicyDocument": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "VerifiedAccessInstanceId": str,
-        "Description": NotRequired[str],
-        "PolicyDocument": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    {
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "FIPSEnabled": NotRequired[bool],
-    },
-)
-CreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "TrustProviderType": TrustProviderTypeType,
-        "PolicyReferenceName": str,
-        "UserTrustProviderType": NotRequired[UserTrustProviderTypeType],
-        "DeviceTrustProviderType": NotRequired[DeviceTrustProviderTypeType],
-        "OidcOptions": NotRequired[CreateVerifiedAccessTrustProviderOidcOptionsTypeDef],
-        "DeviceOptions": NotRequired[CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef],
-        "Description": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "ClientToken": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
-    },
-)
-CreateVolumeRequestRequestTypeDef = TypedDict(
-    "CreateVolumeRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "Encrypted": NotRequired[bool],
-        "Iops": NotRequired[int],
-        "KmsKeyId": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "Size": NotRequired[int],
-        "SnapshotId": NotRequired[str],
-        "VolumeType": NotRequired[VolumeTypeType],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiAttachEnabled": NotRequired[bool],
-        "Throughput": NotRequired[int],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "AvailabilityZone": str,
-        "Encrypted": NotRequired[bool],
-        "Iops": NotRequired[int],
-        "KmsKeyId": NotRequired[str],
-        "OutpostArn": NotRequired[str],
-        "Size": NotRequired[int],
-        "SnapshotId": NotRequired[str],
-        "VolumeType": NotRequired[VolumeTypeType],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiAttachEnabled": NotRequired[bool],
-        "Throughput": NotRequired[int],
-        "ClientToken": NotRequired[str],
-    },
-)
-CreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ServiceName": str,
-        "DryRun": NotRequired[bool],
-        "VpcEndpointType": NotRequired[VpcEndpointTypeType],
-        "PolicyDocument": NotRequired[str],
-        "RouteTableIds": NotRequired[Sequence[str]],
-        "SubnetIds": NotRequired[Sequence[str]],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "IpAddressType": NotRequired[IpAddressTypeType],
-        "DnsOptions": NotRequired[DnsOptionsSpecificationTypeDef],
-        "ClientToken": NotRequired[str],
-        "PrivateDnsEnabled": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SubnetConfigurations": NotRequired[Sequence[SubnetConfigurationTypeDef]],
-    },
-)
-CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "AcceptanceRequired": NotRequired[bool],
-        "PrivateDnsName": NotRequired[str],
-        "NetworkLoadBalancerArns": NotRequired[Sequence[str]],
-        "GatewayLoadBalancerArns": NotRequired[Sequence[str]],
-        "SupportedIpAddressTypes": NotRequired[Sequence[str]],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "PeerOwnerId": NotRequired[str],
-        "PeerVpcId": NotRequired[str],
-        "PeerRegion": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "VpcId": str,
-        "DryRun": NotRequired[bool],
-        "PeerOwnerId": NotRequired[str],
-        "PeerVpcId": NotRequired[str],
-        "PeerRegion": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef = TypedDict(
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
     {
         "DryRun": NotRequired[bool],
         "PeerOwnerId": NotRequired[str],
         "PeerVpcId": NotRequired[str],
         "PeerRegion": NotRequired[str],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-CreateVpcRequestRequestTypeDef = TypedDict(
-    "CreateVpcRequestRequestTypeDef",
-    {
-        "CidrBlock": NotRequired[str],
-        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
-        "Ipv6Pool": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "InstanceTenancy": NotRequired[TenancyType],
-        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    {
-        "CidrBlock": NotRequired[str],
-        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
-        "Ipv6Pool": NotRequired[str],
-        "Ipv6CidrBlock": NotRequired[str],
-        "Ipv4IpamPoolId": NotRequired[str],
-        "Ipv4NetmaskLength": NotRequired[int],
-        "Ipv6IpamPoolId": NotRequired[str],
-        "Ipv6NetmaskLength": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "InstanceTenancy": NotRequired[TenancyType],
-        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-CreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "CreateVpnGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-        "AvailabilityZone": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "AmazonSideAsn": NotRequired[int],
-        "DryRun": NotRequired[bool],
-    },
-)
-ExportImageRequestRequestTypeDef = TypedDict(
-    "ExportImageRequestRequestTypeDef",
-    {
-        "DiskImageFormat": DiskImageFormatType,
-        "ImageId": str,
-        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "RoleName": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ImportKeyPairRequestRequestTypeDef = TypedDict(
-    "ImportKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-ProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "Cidr": str,
-        "CidrAuthorizationContext": NotRequired[CidrAuthorizationContextTypeDef],
-        "PubliclyAdvertisable": NotRequired[bool],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "PoolTagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "MultiRegion": NotRequired[bool],
-        "NetworkBorderGroup": NotRequired[str],
-    },
-)
-PurchaseCapacityBlockRequestRequestTypeDef = TypedDict(
-    "PurchaseCapacityBlockRequestRequestTypeDef",
-    {
-        "CapacityBlockOfferingId": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-PurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "PurchaseHostReservationRequestRequestTypeDef",
-    {
-        "HostIdSet": Sequence[str],
-        "OfferingId": str,
-        "ClientToken": NotRequired[str],
-        "CurrencyCode": NotRequired[Literal["USD"]],
-        "LimitPrice": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsAccessScopeId": str,
-        "ClientToken": str,
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-StartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsPathId": str,
-        "ClientToken": str,
-        "AdditionalAccounts": NotRequired[Sequence[str]],
-        "FilterInArns": NotRequired[Sequence[str]],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
+TagSpecificationUnionTypeDef = Union[TagSpecificationTypeDef, TagSpecificationExtraOutputTypeDef]
 CreateTrafficMirrorSessionResultTypeDef = TypedDict(
     "CreateTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorSessionsResultTypeDef = TypedDict(
     "DescribeTrafficMirrorSessionsResultTypeDef",
     {
         "TrafficMirrorSessions": List[TrafficMirrorSessionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTrafficMirrorSessionResultTypeDef = TypedDict(
     "ModifyTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19087,16 +18238,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorTargetsResultTypeDef = TypedDict(
     "DescribeTrafficMirrorTargetsResultTypeDef",
     {
         "TrafficMirrorTargets": List[TrafficMirrorTargetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayPolicyTableResultTypeDef = TypedDict(
     "CreateTransitGatewayPolicyTableResultTypeDef",
     {
         "TransitGatewayPolicyTable": TransitGatewayPolicyTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19109,16 +18260,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayPolicyTablesResultTypeDef = TypedDict(
     "DescribeTransitGatewayPolicyTablesResultTypeDef",
     {
         "TransitGatewayPolicyTables": List[TransitGatewayPolicyTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayRouteTableAnnouncementResultTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableAnnouncementResultTypeDef",
     {
         "TransitGatewayRouteTableAnnouncement": TransitGatewayRouteTableAnnouncementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19131,16 +18282,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef = TypedDict(
     "DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef",
     {
         "TransitGatewayRouteTableAnnouncements": List[TransitGatewayRouteTableAnnouncementTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayRouteTableResultTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableResultTypeDef",
     {
         "TransitGatewayRouteTable": TransitGatewayRouteTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19153,32 +18304,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayRouteTablesResultTypeDef = TypedDict(
     "DescribeTransitGatewayRouteTablesResultTypeDef",
     {
         "TransitGatewayRouteTables": List[TransitGatewayRouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AssociateTrunkInterfaceResultTypeDef = TypedDict(
     "AssociateTrunkInterfaceResultTypeDef",
     {
         "InterfaceAssociation": TrunkInterfaceAssociationTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrunkInterfaceAssociationsResultTypeDef = TypedDict(
     "DescribeTrunkInterfaceAssociationsResultTypeDef",
     {
         "InterfaceAssociations": List[TrunkInterfaceAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVpcClassicLinkResultTypeDef = TypedDict(
     "DescribeVpcClassicLinkResultTypeDef",
     {
         "Vpcs": List[VpcClassicLinkTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19256,16 +18407,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeByoipCidrsResultTypeDef = TypedDict(
     "DescribeByoipCidrsResultTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MoveByoipCidrToIpamResultTypeDef = TypedDict(
     "MoveByoipCidrToIpamResultTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19285,16 +18436,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClientVpnTargetNetworksResultTypeDef = TypedDict(
     "DescribeClientVpnTargetNetworksResultTypeDef",
     {
         "ClientVpnTargetNetworks": List[TargetNetworkTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RouteTableTypeDef = TypedDict(
     "RouteTableTypeDef",
     {
         "Associations": NotRequired[List[RouteTableAssociationTypeDef]],
         "PropagatingVgws": NotRequired[List[PropagatingVgwTypeDef]],
@@ -19423,16 +18574,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 DescribeClientVpnAuthorizationRulesResultTypeDef = TypedDict(
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     {
         "AuthorizationRules": List[AuthorizationRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAvailabilityZonesResultTypeDef = TypedDict(
     "DescribeAvailabilityZonesResultTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -19476,26 +18627,14 @@
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "Description": NotRequired[str],
         "DryRun": NotRequired[bool],
         "NoReboot": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-CreateImageRequestRequestTypeDef = TypedDict(
-    "CreateImageRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "NoReboot": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 ImageAttributeTypeDef = TypedDict(
     "ImageAttributeTypeDef",
     {
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "ImageId": str,
         "LaunchPermissions": List[LaunchPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
@@ -19546,60 +18685,14 @@
         "DeprecationTime": NotRequired[str],
         "ImdsSupport": NotRequired[Literal["v2.0"]],
         "SourceInstanceId": NotRequired[str],
         "DeregistrationProtection": NotRequired[str],
         "LastLaunchedTime": NotRequired[str],
     },
 )
-RegisterImageRequestRequestTypeDef = TypedDict(
-    "RegisterImageRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ImageLocation": NotRequired[str],
-        "Architecture": NotRequired[ArchitectureValuesType],
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "EnaSupport": NotRequired[bool],
-        "KernelId": NotRequired[str],
-        "BillingProducts": NotRequired[Sequence[str]],
-        "RamdiskId": NotRequired[str],
-        "RootDeviceName": NotRequired[str],
-        "SriovNetSupport": NotRequired[str],
-        "VirtualizationType": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-        "TpmSupport": NotRequired[Literal["v2.0"]],
-        "UefiData": NotRequired[str],
-        "ImdsSupport": NotRequired[Literal["v2.0"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
-RegisterImageRequestServiceResourceRegisterImageTypeDef = TypedDict(
-    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
-    {
-        "Name": str,
-        "ImageLocation": NotRequired[str],
-        "Architecture": NotRequired[ArchitectureValuesType],
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
-        "Description": NotRequired[str],
-        "DryRun": NotRequired[bool],
-        "EnaSupport": NotRequired[bool],
-        "KernelId": NotRequired[str],
-        "BillingProducts": NotRequired[Sequence[str]],
-        "RamdiskId": NotRequired[str],
-        "RootDeviceName": NotRequired[str],
-        "SriovNetSupport": NotRequired[str],
-        "VirtualizationType": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-        "TpmSupport": NotRequired[Literal["v2.0"]],
-        "UefiData": NotRequired[str],
-        "ImdsSupport": NotRequired[Literal["v2.0"]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CancelCapacityReservationFleetsResultTypeDef = TypedDict(
     "CancelCapacityReservationFleetsResultTypeDef",
     {
         "SuccessfulFleetCancellations": List[CapacityReservationFleetCancellationStateTypeDef],
         "FailedFleetCancellations": List[FailedCapacityReservationFleetCancellationResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -19618,71 +18711,48 @@
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCapacityReservationsResultTypeDef = TypedDict(
     "DescribeCapacityReservationsResultTypeDef",
     {
-        "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseCapacityBlockResultTypeDef = TypedDict(
     "PurchaseCapacityBlockResultTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeCapacityReservationFleetsResultTypeDef = TypedDict(
     "DescribeCapacityReservationFleetsResultTypeDef",
     {
         "CapacityReservationFleets": List[CapacityReservationFleetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef = TypedDict(
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
 DescribeClassicLinkInstancesResultTypeDef = TypedDict(
     "DescribeClassicLinkInstancesResultTypeDef",
     {
         "Instances": List[ClassicLinkInstanceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "CreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "ClientCidrBlock": str,
-        "ServerCertificateArn": str,
-        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
-        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
-        "DnsServers": NotRequired[Sequence[str]],
-        "TransportProtocol": NotRequired[TransportProtocolType],
-        "VpnPort": NotRequired[int],
-        "Description": NotRequired[str],
-        "SplitTunnel": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "ClientToken": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "VpcId": NotRequired[str],
-        "SelfServicePortal": NotRequired[SelfServicePortalType],
-        "ClientConnectOptions": NotRequired[ClientConnectOptionsTypeDef],
-        "SessionTimeoutHours": NotRequired[int],
-        "ClientLoginBannerOptions": NotRequired[ClientLoginBannerOptionsTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 ClientVpnEndpointTypeDef = TypedDict(
     "ClientVpnEndpointTypeDef",
     {
         "ClientVpnEndpointId": NotRequired[str],
         "Description": NotRequired[str],
@@ -19709,16 +18779,16 @@
         "ClientLoginBannerOptions": NotRequired[ClientLoginBannerResponseOptionsTypeDef],
     },
 )
 DescribeClientVpnConnectionsResultTypeDef = TypedDict(
     "DescribeClientVpnConnectionsResultTypeDef",
     {
         "Connections": List[ClientVpnConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TerminateClientVpnConnectionsResultTypeDef = TypedDict(
     "TerminateClientVpnConnectionsResultTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Username": str,
@@ -19726,16 +18796,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClientVpnRoutesResultTypeDef = TypedDict(
     "DescribeClientVpnRoutesResultTypeDef",
     {
         "Routes": List[ClientVpnRouteTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpnTunnelOptionsSpecificationTypeDef = TypedDict(
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     {
         "TunnelInsideCidr": NotRequired[str],
         "TunnelInsideIpv6Cidr": NotRequired[str],
@@ -19861,16 +18931,16 @@
         "DryRun": NotRequired[bool],
     },
 )
 GetAwsNetworkPerformanceDataResultTypeDef = TypedDict(
     "GetAwsNetworkPerformanceDataResultTypeDef",
     {
         "DataResponses": List[DataResponseTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DeleteFleetsResultTypeDef = TypedDict(
     "DeleteFleetsResultTypeDef",
     {
         "SuccessfulFleetDeletions": List[DeleteFleetSuccessItemTypeDef],
         "UnsuccessfulFleetDeletions": List[DeleteFleetErrorItemTypeDef],
@@ -19897,32 +18967,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePrincipalIdFormatResultTypeDef = TypedDict(
     "DescribePrincipalIdFormatResultTypeDef",
     {
         "Principals": List[PrincipalIdFormatTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFastLaunchImagesResultTypeDef = TypedDict(
     "DescribeFastLaunchImagesResultTypeDef",
     {
         "FastLaunchImages": List[DescribeFastLaunchImagesSuccessItemTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFlowLogsResultTypeDef = TypedDict(
     "DescribeFlowLogsResultTypeDef",
     {
         "FlowLogs": List[FlowLogTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": NotRequired[str],
         "FastSnapshotRestoreStateErrors": NotRequired[
@@ -19939,16 +19009,16 @@
         "Volumes": NotRequired[List[ImportInstanceVolumeDetailItemTypeDef]],
     },
 )
 DescribeVpcEndpointConnectionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionsResultTypeDef",
     {
         "VpcEndpointConnections": List[VpcEndpointConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyInstanceAttributeRequestInstanceModifyAttributeTypeDef = TypedDict(
     "ModifyInstanceAttributeRequestInstanceModifyAttributeTypeDef",
     {
         "SourceDestCheck": NotRequired[AttributeBooleanValueTypeDef],
         "Attribute": NotRequired[InstanceAttributeNameType],
@@ -20025,92 +19095,92 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeEgressOnlyInternetGatewaysResultTypeDef = TypedDict(
     "DescribeEgressOnlyInternetGatewaysResultTypeDef",
     {
         "EgressOnlyInternetGateways": List[EgressOnlyInternetGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateInternetGatewayResultTypeDef = TypedDict(
     "CreateInternetGatewayResultTypeDef",
     {
         "InternetGateway": InternetGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInternetGatewaysResultTypeDef = TypedDict(
     "DescribeInternetGatewaysResultTypeDef",
     {
         "InternetGateways": List[InternetGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeElasticGpusResultTypeDef = TypedDict(
     "DescribeElasticGpusResultTypeDef",
     {
         "ElasticGpuSet": List[ElasticGpusTypeDef],
         "MaxResults": int,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-InstanceNetworkInterfaceSpecificationServiceResourceTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
+InstanceNetworkInterfaceSpecificationExtraOutputTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationExtraOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[Sequence[str]],
+        "Groups": NotRequired[List[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
 )
-InstanceNetworkInterfaceSpecificationSubnetTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
+InstanceNetworkInterfaceSpecificationOutputTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[Sequence[str]],
+        "Groups": NotRequired[List[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
@@ -20118,28 +19188,28 @@
 InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "InstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
-        "Groups": NotRequired[List[str]],
+        "Groups": NotRequired[Sequence[str]],
         "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[List[InstanceIpv6AddressTypeDef]],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "NetworkInterfaceId": NotRequired[str],
         "PrivateIpAddress": NotRequired[str],
-        "PrivateIpAddresses": NotRequired[List[PrivateIpAddressSpecificationTypeDef]],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
         "SecondaryPrivateIpAddressCount": NotRequired[int],
         "SubnetId": NotRequired[str],
         "AssociateCarrierIpAddress": NotRequired[bool],
         "InterfaceType": NotRequired[str],
         "NetworkCardIndex": NotRequired[int],
-        "Ipv4Prefixes": NotRequired[List[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
         "Ipv4PrefixCount": NotRequired[int],
-        "Ipv6Prefixes": NotRequired[List[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
         "Ipv6PrefixCount": NotRequired[int],
         "PrimaryIpv6": NotRequired[bool],
         "EnaSrdSpecification": NotRequired[EnaSrdSpecificationRequestTypeDef],
         "ConnectionTrackingSpecification": NotRequired[
             ConnectionTrackingSpecificationRequestTypeDef
         ],
     },
@@ -20237,37 +19307,37 @@
     },
 )
 DescribeFleetHistoryResultTypeDef = TypedDict(
     "DescribeFleetHistoryResultTypeDef",
     {
         "HistoryRecords": List[HistoryRecordEntryTypeDef],
         "LastEvaluatedTime": datetime,
-        "NextToken": str,
         "FleetId": str,
         "StartTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetRequestHistoryResponseTypeDef = TypedDict(
     "DescribeSpotFleetRequestHistoryResponseTypeDef",
     {
         "HistoryRecords": List[HistoryRecordTypeDef],
         "LastEvaluatedTime": datetime,
-        "NextToken": str,
         "SpotFleetRequestId": str,
         "StartTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeExportImageTasksResultTypeDef = TypedDict(
     "DescribeExportImageTasksResultTypeDef",
     {
         "ExportImageTasks": List[ExportImageTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateInstanceExportTaskResultTypeDef = TypedDict(
     "CreateInstanceExportTaskResultTypeDef",
     {
         "ExportTask": ExportTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20346,16 +19416,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeFpgaImagesResultTypeDef = TypedDict(
     "DescribeFpgaImagesResultTypeDef",
     {
         "FpgaImages": List[FpgaImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GpuInfoTypeDef = TypedDict(
     "GpuInfoTypeDef",
     {
         "Gpus": NotRequired[List[GpuDeviceInfoTypeDef]],
         "TotalGpuMemoryInMiB": NotRequired[int],
@@ -20368,16 +19438,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIamInstanceProfileAssociationsResultTypeDef = TypedDict(
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     {
         "IamInstanceProfileAssociations": List[IamInstanceProfileAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateIamInstanceProfileResultTypeDef = TypedDict(
     "DisassociateIamInstanceProfileResultTypeDef",
     {
         "IamInstanceProfileAssociation": IamInstanceProfileAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20421,51 +19491,14 @@
         "Value": NotRequired[str],
         "DryRun": NotRequired[bool],
         "OrganizationArns": NotRequired[Sequence[str]],
         "OrganizationalUnitArns": NotRequired[Sequence[str]],
         "ImdsSupport": NotRequired[AttributeValueTypeDef],
     },
 )
-ImportImageRequestRequestTypeDef = TypedDict(
-    "ImportImageRequestRequestTypeDef",
-    {
-        "Architecture": NotRequired[str],
-        "ClientData": NotRequired[ClientDataTypeDef],
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DiskContainers": NotRequired[Sequence[ImageDiskContainerTypeDef]],
-        "DryRun": NotRequired[bool],
-        "Encrypted": NotRequired[bool],
-        "Hypervisor": NotRequired[str],
-        "KmsKeyId": NotRequired[str],
-        "LicenseType": NotRequired[str],
-        "Platform": NotRequired[str],
-        "RoleName": NotRequired[str],
-        "LicenseSpecifications": NotRequired[
-            Sequence[ImportImageLicenseConfigurationRequestTypeDef]
-        ],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "UsageOperation": NotRequired[str],
-        "BootMode": NotRequired[BootModeValuesType],
-    },
-)
-ImportSnapshotRequestRequestTypeDef = TypedDict(
-    "ImportSnapshotRequestRequestTypeDef",
-    {
-        "ClientData": NotRequired[ClientDataTypeDef],
-        "ClientToken": NotRequired[str],
-        "Description": NotRequired[str],
-        "DiskContainer": NotRequired[SnapshotDiskContainerTypeDef],
-        "DryRun": NotRequired[bool],
-        "Encrypted": NotRequired[bool],
-        "KmsKeyId": NotRequired[str],
-        "RoleName": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
     "CreateLocalGatewayRouteTableResultTypeDef",
     {
         "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -20476,16 +19509,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
     "DescribeLocalGatewayRouteTablesResultTypeDef",
     {
         "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportInstanceRequestRequestTypeDef = TypedDict(
     "ImportInstanceRequestRequestTypeDef",
     {
         "Platform": Literal["windows"],
         "Description": NotRequired[str],
@@ -20523,14 +19556,64 @@
 UnmonitorInstancesResultTypeDef = TypedDict(
     "UnmonitorInstancesResultTypeDef",
     {
         "InstanceMonitorings": List[InstanceMonitoringTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LaunchTemplateOverridesExtraOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesExtraOutputTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsExtraOutputTypeDef],
+    },
+)
+FleetLaunchTemplateOverridesTypeDef = TypedDict(
+    "FleetLaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "MaxPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "Placement": NotRequired[PlacementResponseTypeDef],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
+        "ImageId": NotRequired[str],
+    },
+)
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
+    },
+)
+LaunchTemplateOverridesTypeDef = TypedDict(
+    "LaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": NotRequired[InstanceTypeType],
+        "SpotPrice": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "Priority": NotRequired[float],
+        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
+    },
+)
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": NotRequired[InstanceTypeType],
         "MaxPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "AvailabilityZone": NotRequired[str],
@@ -20566,40 +19649,14 @@
     "InstanceRequirementsWithMetadataRequestTypeDef",
     {
         "ArchitectureTypes": NotRequired[Sequence[ArchitectureTypeType]],
         "VirtualizationTypes": NotRequired[Sequence[VirtualizationTypeType]],
         "InstanceRequirements": NotRequired[InstanceRequirementsRequestTypeDef],
     },
 )
-FleetLaunchTemplateOverridesTypeDef = TypedDict(
-    "FleetLaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": NotRequired[InstanceTypeType],
-        "MaxPrice": NotRequired[str],
-        "SubnetId": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "WeightedCapacity": NotRequired[float],
-        "Priority": NotRequired[float],
-        "Placement": NotRequired[PlacementResponseTypeDef],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
-        "ImageId": NotRequired[str],
-    },
-)
-LaunchTemplateOverridesTypeDef = TypedDict(
-    "LaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": NotRequired[InstanceTypeType],
-        "SpotPrice": NotRequired[str],
-        "SubnetId": NotRequired[str],
-        "AvailabilityZone": NotRequired[str],
-        "WeightedCapacity": NotRequired[float],
-        "Priority": NotRequired[float],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
-    },
-)
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -20625,72 +19682,57 @@
         "Events": NotRequired[List[InstanceStatusEventTypeDef]],
         "InstanceId": NotRequired[str],
         "InstanceState": NotRequired[InstanceStateTypeDef],
         "InstanceStatus": NotRequired[InstanceStatusSummaryTypeDef],
         "SystemStatus": NotRequired[InstanceStatusSummaryTypeDef],
     },
 )
-SecurityGroupPaginatorTypeDef = TypedDict(
-    "SecurityGroupPaginatorTypeDef",
+RevokeSecurityGroupEgressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+RevokeSecurityGroupIngressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+SecurityGroupTypeDef = TypedDict(
+    "SecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
         "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[List[IpPermissionPaginatorTypeDef]],
+        "IpPermissions": NotRequired[List[IpPermissionOutputTypeDef]],
         "OwnerId": NotRequired[str],
         "GroupId": NotRequired[str],
-        "IpPermissionsEgress": NotRequired[List[IpPermissionPaginatorTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[IpPermissionOutputTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
-AuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-        "DryRun": NotRequired[bool],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "IpProtocol": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-    },
-)
 AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef = TypedDict(
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
     {
         "DryRun": NotRequired[bool],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "ToPort": NotRequired[int],
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
-    {
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "IpProtocol": NotRequired[str],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-    },
-)
 AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef = TypedDict(
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
     {
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "GroupName": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
@@ -20698,67 +19740,29 @@
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
         "ToPort": NotRequired[int],
         "DryRun": NotRequired[bool],
         "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
     },
 )
-RevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-        "DryRun": NotRequired[bool],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "IpProtocol": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-    },
-)
+IpPermissionUnionTypeDef = Union[IpPermissionTypeDef, IpPermissionExtraExtraOutputTypeDef]
 RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef = TypedDict(
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
     {
         "DryRun": NotRequired[bool],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
         "SecurityGroupRuleIds": NotRequired[Sequence[str]],
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "IpProtocol": NotRequired[str],
         "ToPort": NotRequired[int],
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-RevokeSecurityGroupEgressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
-    {
-        "CidrIp": NotRequired[str],
-        "FromPort": NotRequired[int],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "IpProtocol": NotRequired[str],
-        "SourceSecurityGroupName": NotRequired[str],
-        "SourceSecurityGroupOwnerId": NotRequired[str],
-        "ToPort": NotRequired[int],
-        "DryRun": NotRequired[bool],
-        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
-    },
-)
 RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef = TypedDict(
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
     {
         "CidrIp": NotRequired[str],
         "FromPort": NotRequired[int],
         "GroupName": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
@@ -20766,55 +19770,14 @@
         "SourceSecurityGroupName": NotRequired[str],
         "SourceSecurityGroupOwnerId": NotRequired[str],
         "ToPort": NotRequired[int],
         "DryRun": NotRequired[bool],
         "SecurityGroupRuleIds": NotRequired[Sequence[str]],
     },
 )
-RevokeSecurityGroupIngressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-SecurityGroupTypeDef = TypedDict(
-    "SecurityGroupTypeDef",
-    {
-        "Description": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[List[IpPermissionTypeDef]],
-        "OwnerId": NotRequired[str],
-        "GroupId": NotRequired[str],
-        "IpPermissionsEgress": NotRequired[List[IpPermissionTypeDef]],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "VpcId": NotRequired[str],
-    },
-)
-UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
-    },
-)
-UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
-    {
-        "DryRun": NotRequired[bool],
-        "GroupId": NotRequired[str],
-        "GroupName": NotRequired[str],
-        "IpPermissions": NotRequired[Sequence[IpPermissionTypeDef]],
-        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
-    },
-)
 StaleSecurityGroupTypeDef = TypedDict(
     "StaleSecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "StaleIpPermissions": NotRequired[List[StaleIpPermissionTypeDef]],
@@ -20822,32 +19785,32 @@
         "VpcId": NotRequired[str],
     },
 )
 GetIpamDiscoveredAccountsResultTypeDef = TypedDict(
     "GetIpamDiscoveredAccountsResultTypeDef",
     {
         "IpamDiscoveredAccounts": List[IpamDiscoveredAccountTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamDiscoveredResourceCidrsResultTypeDef = TypedDict(
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     {
         "IpamDiscoveredResourceCidrs": List[IpamDiscoveredResourceCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamResourceCidrsResultTypeDef = TypedDict(
     "GetIpamResourceCidrsResultTypeDef",
     {
-        "NextToken": str,
         "IpamResourceCidrs": List[IpamResourceCidrTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResourceCidrResultTypeDef = TypedDict(
     "ModifyIpamResourceCidrResultTypeDef",
     {
         "IpamResourceCidr": IpamResourceCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20867,16 +19830,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamResourceDiscoveriesResultTypeDef = TypedDict(
     "DescribeIpamResourceDiscoveriesResultTypeDef",
     {
         "IpamResourceDiscoveries": List[IpamResourceDiscoveryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResourceDiscoveryResultTypeDef = TypedDict(
     "ModifyIpamResourceDiscoveryResultTypeDef",
     {
         "IpamResourceDiscovery": IpamResourceDiscoveryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20895,17 +19858,17 @@
         "Ipam": IpamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamsResultTypeDef = TypedDict(
     "DescribeIpamsResultTypeDef",
     {
-        "NextToken": str,
         "Ipams": List[IpamTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamResultTypeDef = TypedDict(
     "ModifyIpamResultTypeDef",
     {
         "Ipam": IpamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20918,16 +19881,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetIpamPoolCidrsResultTypeDef = TypedDict(
     "GetIpamPoolCidrsResultTypeDef",
     {
         "IpamPoolCidrs": List[IpamPoolCidrTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ProvisionIpamPoolCidrResultTypeDef = TypedDict(
     "ProvisionIpamPoolCidrResultTypeDef",
     {
         "IpamPoolCidr": IpamPoolCidrTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20946,17 +19909,17 @@
         "IpamPool": IpamPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeIpamPoolsResultTypeDef = TypedDict(
     "DescribeIpamPoolsResultTypeDef",
     {
-        "NextToken": str,
         "IpamPools": List[IpamPoolTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyIpamPoolResultTypeDef = TypedDict(
     "ModifyIpamPoolResultTypeDef",
     {
         "IpamPool": IpamPoolTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -20986,16 +19949,16 @@
         "SampleTime": NotRequired[datetime],
     },
 )
 DescribeIpv6PoolsResultTypeDef = TypedDict(
     "DescribeIpv6PoolsResultTypeDef",
     {
         "Ipv6Pools": List[Ipv6PoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociateCarrierIpAddress": NotRequired[bool],
         "AssociatePublicIpAddress": NotRequired[bool],
@@ -21071,16 +20034,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessGroupsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessGroupsResultTypeDef",
     {
         "VerifiedAccessGroups": List[VerifiedAccessGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessGroupResultTypeDef = TypedDict(
     "ModifyVerifiedAccessGroupResultTypeDef",
     {
         "VerifiedAccessGroup": VerifiedAccessGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21094,31 +20057,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNatGatewaysResultTypeDef = TypedDict(
     "DescribeNatGatewaysResultTypeDef",
     {
         "NatGateways": List[NatGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkInterfacePermissionResultTypeDef = TypedDict(
     "CreateNetworkInterfacePermissionResultTypeDef",
     {
         "InterfacePermission": NetworkInterfacePermissionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInterfacePermissionsResultTypeDef = TypedDict(
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     {
         "NetworkInterfacePermissions": List[NetworkInterfacePermissionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 NeuronInfoTypeDef = TypedDict(
     "NeuronInfoTypeDef",
     {
         "NeuronDevices": NotRequired[List[NeuronDeviceInfoTypeDef]],
         "TotalNeuronDeviceMemoryInMiB": NotRequired[int],
@@ -21138,41 +20101,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessTrustProvidersResultTypeDef = TypedDict(
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     {
         "VerifiedAccessTrustProviders": List[VerifiedAccessTrustProviderTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessTrustProviderResultTypeDef = TypedDict(
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "Source": str,
-        "Protocol": ProtocolType,
-        "ClientToken": str,
-        "SourceIp": NotRequired[str],
-        "DestinationIp": NotRequired[str],
-        "Destination": NotRequired[str],
-        "DestinationPort": NotRequired[int],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "DryRun": NotRequired[bool],
-        "FilterAtSource": NotRequired[PathRequestFilterTypeDef],
-        "FilterAtDestination": NotRequired[PathRequestFilterTypeDef],
-    },
-)
 AccessScopePathRequestTypeDef = TypedDict(
     "AccessScopePathRequestTypeDef",
     {
         "Source": NotRequired[PathStatementRequestTypeDef],
         "Destination": NotRequired[PathStatementRequestTypeDef],
         "ThroughResources": NotRequired[Sequence[ThroughResourcesStatementRequestTypeDef]],
     },
@@ -21206,24 +20153,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePublicIpv4PoolsResultTypeDef = TypedDict(
     "DescribePublicIpv4PoolsResultTypeDef",
     {
         "PublicIpv4Pools": List[PublicIpv4PoolTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesOfferingsResultTypeDef = TypedDict(
     "DescribeReservedInstancesOfferingsResultTypeDef",
     {
         "ReservedInstancesOfferings": List[ReservedInstancesOfferingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesResultTypeDef = TypedDict(
     "DescribeReservedInstancesResultTypeDef",
     {
         "ReservedInstances": List[ReservedInstancesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21245,32 +20192,45 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSecurityGroupRulesResultTypeDef = TypedDict(
     "DescribeSecurityGroupRulesResultTypeDef",
     {
         "SecurityGroupRules": List[SecurityGroupRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BundleTaskTypeDef = TypedDict(
+    "BundleTaskTypeDef",
+    {
+        "BundleId": NotRequired[str],
+        "BundleTaskError": NotRequired[BundleTaskErrorTypeDef],
+        "InstanceId": NotRequired[str],
+        "Progress": NotRequired[str],
+        "StartTime": NotRequired[datetime],
+        "State": NotRequired[BundleTaskStateType],
+        "Storage": NotRequired[StorageOutputTypeDef],
+        "UpdateTime": NotRequired[datetime],
     },
 )
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
-        "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeScheduledInstancesResultTypeDef = TypedDict(
     "DescribeScheduledInstancesResultTypeDef",
     {
-        "NextToken": str,
         "ScheduledInstanceSet": List[ScheduledInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseScheduledInstancesResultTypeDef = TypedDict(
     "PurchaseScheduledInstancesResultTypeDef",
     {
         "ScheduledInstanceSet": List[ScheduledInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21303,16 +20263,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointsResultTypeDef = TypedDict(
     "DescribeVpcEndpointsResultTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifySecurityGroupRulesRequestRequestTypeDef = TypedDict(
     "ModifySecurityGroupRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "SecurityGroupRules": Sequence[SecurityGroupRuleUpdateTypeDef],
@@ -21327,25 +20287,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcEndpointServiceConfigurationsResultTypeDef = TypedDict(
     "DescribeVpcEndpointServiceConfigurationsResultTypeDef",
     {
         "ServiceConfigurations": List[ServiceConfigurationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVpcEndpointServicesResultTypeDef = TypedDict(
     "DescribeVpcEndpointServicesResultTypeDef",
     {
         "ServiceNames": List[str],
         "ServiceDetails": List[ServiceDetailTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportImageResultTypeDef = TypedDict(
     "ImportImageResultTypeDef",
     {
         "Architecture": str,
         "Description": str,
@@ -21421,16 +20381,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayMulticastDomainAssociationsResultTypeDef = TypedDict(
     "GetTransitGatewayMulticastDomainAssociationsResultTypeDef",
     {
         "MulticastDomainAssociations": List[TransitGatewayMulticastDomainAssociationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptTransitGatewayMulticastDomainAssociationsResultTypeDef = TypedDict(
     "AcceptTransitGatewayMulticastDomainAssociationsResultTypeDef",
     {
         "Associations": TransitGatewayMulticastDomainAssociationsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21510,14 +20470,28 @@
         "ReservedInstanceValueSet": List[ReservedInstanceReservationValueTypeDef],
         "TargetConfigurationValueRollup": ReservationValueTypeDef,
         "TargetConfigurationValueSet": List[TargetReservationValueTypeDef],
         "ValidationFailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LoadBalancersConfigExtraOutputTypeDef = TypedDict(
+    "LoadBalancersConfigExtraOutputTypeDef",
+    {
+        "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigExtraOutputTypeDef],
+        "TargetGroupsConfig": NotRequired[TargetGroupsConfigExtraOutputTypeDef],
+    },
+)
+LoadBalancersConfigOutputTypeDef = TypedDict(
+    "LoadBalancersConfigOutputTypeDef",
+    {
+        "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigOutputTypeDef],
+        "TargetGroupsConfig": NotRequired[TargetGroupsConfigOutputTypeDef],
+    },
+)
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": NotRequired[ClassicLoadBalancersConfigTypeDef],
         "TargetGroupsConfig": NotRequired[TargetGroupsConfigTypeDef],
     },
 )
@@ -21547,16 +20521,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
 DescribeTransitGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     {
         "TransitGatewayAttachments": List[TransitGatewayAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TransitGatewayConnectPeerTypeDef = TypedDict(
     "TransitGatewayConnectPeerTypeDef",
     {
         "TransitGatewayAttachmentId": NotRequired[str],
         "TransitGatewayConnectPeerId": NotRequired[str],
@@ -21580,16 +20554,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayConnectsResultTypeDef = TypedDict(
     "DescribeTransitGatewayConnectsResultTypeDef",
     {
         "TransitGatewayConnects": List[TransitGatewayConnectTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayMulticastDomainResultTypeDef = TypedDict(
     "CreateTransitGatewayMulticastDomainResultTypeDef",
     {
         "TransitGatewayMulticastDomain": TransitGatewayMulticastDomainTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21602,16 +20576,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayMulticastDomainsResultTypeDef = TypedDict(
     "DescribeTransitGatewayMulticastDomainsResultTypeDef",
     {
         "TransitGatewayMulticastDomains": List[TransitGatewayMulticastDomainTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTransitGatewayResultTypeDef = TypedDict(
     "CreateTransitGatewayResultTypeDef",
     {
         "TransitGateway": TransitGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21624,16 +20598,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewaysResultTypeDef = TypedDict(
     "DescribeTransitGatewaysResultTypeDef",
     {
         "TransitGateways": List[TransitGatewayTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayResultTypeDef = TypedDict(
     "ModifyTransitGatewayResultTypeDef",
     {
         "TransitGateway": TransitGatewayTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21660,16 +20634,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayPeeringAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayPeeringAttachmentsResultTypeDef",
     {
         "TransitGatewayPeeringAttachments": List[TransitGatewayPeeringAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RejectTransitGatewayPeeringAttachmentResultTypeDef = TypedDict(
     "RejectTransitGatewayPeeringAttachmentResultTypeDef",
     {
         "TransitGatewayPeeringAttachment": TransitGatewayPeeringAttachmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21697,16 +20671,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetTransitGatewayPrefixListReferencesResultTypeDef = TypedDict(
     "GetTransitGatewayPrefixListReferencesResultTypeDef",
     {
         "TransitGatewayPrefixListReferences": List[TransitGatewayPrefixListReferenceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayPrefixListReferenceResultTypeDef = TypedDict(
     "ModifyTransitGatewayPrefixListReferenceResultTypeDef",
     {
         "TransitGatewayPrefixListReference": TransitGatewayPrefixListReferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21762,16 +20736,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayVpcAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayVpcAttachmentsResultTypeDef",
     {
         "TransitGatewayVpcAttachments": List[TransitGatewayVpcAttachmentTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTransitGatewayVpcAttachmentResultTypeDef = TypedDict(
     "ModifyTransitGatewayVpcAttachmentResultTypeDef",
     {
         "TransitGatewayVpcAttachment": TransitGatewayVpcAttachmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21885,16 +20859,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessEndpointsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessEndpointsResultTypeDef",
     {
         "VerifiedAccessEndpoints": List[VerifiedAccessEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessEndpointResultTypeDef = TypedDict(
     "ModifyVerifiedAccessEndpointResultTypeDef",
     {
         "VerifiedAccessEndpoint": VerifiedAccessEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -21922,16 +20896,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessInstancesResultTypeDef = TypedDict(
     "DescribeVerifiedAccessInstancesResultTypeDef",
     {
         "VerifiedAccessInstances": List[VerifiedAccessInstanceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DetachVerifiedAccessTrustProviderResultTypeDef = TypedDict(
     "DetachVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "VerifiedAccessInstance": VerifiedAccessInstanceTypeDef,
@@ -21964,16 +20938,16 @@
         "ClientToken": NotRequired[str],
     },
 )
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VolumeStatusItemTypeDef = TypedDict(
     "VolumeStatusItemTypeDef",
     {
         "Actions": NotRequired[List[VolumeStatusActionTypeDef]],
         "AvailabilityZone": NotRequired[str],
@@ -22042,16 +21016,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInstanceEventWindowsResultTypeDef = TypedDict(
     "DescribeInstanceEventWindowsResultTypeDef",
     {
         "InstanceEventWindows": List[InstanceEventWindowTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateInstanceEventWindowResultTypeDef = TypedDict(
     "DisassociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22060,14 +21034,1152 @@
 ModifyInstanceEventWindowResultTypeDef = TypedDict(
     "ModifyInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "AcceptAddressTransferRequestRequestTypeDef",
+    {
+        "Address": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+AllocateAddressRequestRequestTypeDef = TypedDict(
+    "AllocateAddressRequestRequestTypeDef",
+    {
+        "Domain": NotRequired[DomainTypeType],
+        "Address": NotRequired[str],
+        "PublicIpv4Pool": NotRequired[str],
+        "NetworkBorderGroup": NotRequired[str],
+        "CustomerOwnedIpv4Pool": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+AllocateHostsRequestRequestTypeDef = TypedDict(
+    "AllocateHostsRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "AutoPlacement": NotRequired[AutoPlacementType],
+        "ClientToken": NotRequired[str],
+        "InstanceType": NotRequired[str],
+        "InstanceFamily": NotRequired[str],
+        "Quantity": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "HostRecovery": NotRequired[HostRecoveryType],
+        "OutpostArn": NotRequired[str],
+        "HostMaintenance": NotRequired[HostMaintenanceType],
+        "AssetIds": NotRequired[Sequence[str]],
+    },
+)
+AssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "IpamResourceDiscoveryId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CopyImageRequestRequestTypeDef = TypedDict(
+    "CopyImageRequestRequestTypeDef",
+    {
+        "Name": str,
+        "SourceImageId": str,
+        "SourceRegion": str,
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DestinationOutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "CopyImageTags": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CopySnapshotRequestRequestTypeDef = TypedDict(
+    "CopySnapshotRequestRequestTypeDef",
+    {
+        "SourceRegion": str,
+        "SourceSnapshotId": str,
+        "Description": NotRequired[str],
+        "DestinationOutpostArn": NotRequired[str],
+        "DestinationRegion": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "PresignedUrl": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
+        "TotalTargetCapacity": int,
+        "AllocationStrategy": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "Tenancy": NotRequired[Literal["default"]],
+        "EndDate": NotRequired[TimestampTypeDef],
+        "InstanceMatchCriteria": NotRequired[Literal["open"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "CreateCapacityReservationRequestRequestTypeDef",
+    {
+        "InstanceType": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "InstanceCount": int,
+        "ClientToken": NotRequired[str],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "Tenancy": NotRequired[CapacityReservationTenancyType],
+        "EbsOptimized": NotRequired[bool],
+        "EphemeralStorage": NotRequired[bool],
+        "EndDate": NotRequired[TimestampTypeDef],
+        "EndDateType": NotRequired[EndDateTypeType],
+        "InstanceMatchCriteria": NotRequired[InstanceMatchCriteriaType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "OutpostArn": NotRequired[str],
+        "PlacementGroupArn": NotRequired[str],
+    },
+)
+CreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "CreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "ClientCidrBlock": str,
+        "ServerCertificateArn": str,
+        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
+        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
+        "DnsServers": NotRequired[Sequence[str]],
+        "TransportProtocol": NotRequired[TransportProtocolType],
+        "VpnPort": NotRequired[int],
+        "Description": NotRequired[str],
+        "SplitTunnel": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "VpcId": NotRequired[str],
+        "SelfServicePortal": NotRequired[SelfServicePortalType],
+        "ClientConnectOptions": NotRequired[ClientConnectOptionsTypeDef],
+        "SessionTimeoutHours": NotRequired[int],
+        "ClientLoginBannerOptions": NotRequired[ClientLoginBannerOptionsTypeDef],
+    },
+)
+CreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "CreateCoipPoolRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+        "BgpAsn": NotRequired[int],
+        "PublicIp": NotRequired[str],
+        "CertificateArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DeviceName": NotRequired[str],
+        "IpAddress": NotRequired[str],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "CreateFlowLogsRequestRequestTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ResourceType": FlowLogsResourceTypeType,
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "DeliverLogsPermissionArn": NotRequired[str],
+        "DeliverCrossAccountRole": NotRequired[str],
+        "LogGroupName": NotRequired[str],
+        "TrafficType": NotRequired[TrafficTypeType],
+        "LogDestinationType": NotRequired[LogDestinationTypeType],
+        "LogDestination": NotRequired[str],
+        "LogFormat": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MaxAggregationInterval": NotRequired[int],
+        "DestinationOptions": NotRequired[DestinationOptionsRequestTypeDef],
+    },
+)
+CreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "CreateFpgaImageRequestRequestTypeDef",
+    {
+        "InputStorageLocation": StorageLocationTypeDef,
+        "DryRun": NotRequired[bool],
+        "LogsStorageLocation": NotRequired[StorageLocationTypeDef],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateImageRequestRequestTypeDef = TypedDict(
+    "CreateImageRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "NoReboot": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "DryRun": NotRequired[bool],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "PreserveClientIp": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Name": NotRequired[str],
+        "TimeRanges": NotRequired[Sequence[InstanceEventWindowTimeRangeRequestTypeDef]],
+        "CronExpression": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
+        "InstanceId": str,
+        "TargetEnvironment": ExportEnvironmentType,
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateInternetGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    {
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "CreateIpamPoolRequestRequestTypeDef",
+    {
+        "IpamScopeId": str,
+        "AddressFamily": AddressFamilyType,
+        "DryRun": NotRequired[bool],
+        "Locale": NotRequired[str],
+        "SourceIpamPoolId": NotRequired[str],
+        "Description": NotRequired[str],
+        "AutoImport": NotRequired[bool],
+        "PubliclyAdvertisable": NotRequired[bool],
+        "AllocationMinNetmaskLength": NotRequired[int],
+        "AllocationMaxNetmaskLength": NotRequired[int],
+        "AllocationDefaultNetmaskLength": NotRequired[int],
+        "AllocationResourceTags": NotRequired[Sequence[RequestIpamResourceTagTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "AwsService": NotRequired[Literal["ec2"]],
+        "PublicIpSource": NotRequired[IpamPoolPublicIpSourceType],
+        "SourceResource": NotRequired[IpamPoolSourceResourceRequestTypeDef],
+    },
+)
+CreateIpamRequestRequestTypeDef = TypedDict(
+    "CreateIpamRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "Tier": NotRequired[IpamTierType],
+    },
+)
+CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "OperatingRegions": NotRequired[Sequence[AddIpamOperatingRegionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "CreateIpamScopeRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "DryRun": NotRequired[bool],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateKeyPairRequestRequestTypeDef = TypedDict(
+    "CreateKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "DryRun": NotRequired[bool],
+        "KeyType": NotRequired[KeyTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "KeyFormat": NotRequired[KeyFormatType],
+    },
+)
+CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "DryRun": NotRequired[bool],
+        "KeyType": NotRequired[KeyTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "KeyFormat": NotRequired[KeyFormatType],
+    },
+)
+CreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "LocalGatewayId": str,
+        "Mode": NotRequired[LocalGatewayRouteTableModeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayVirtualInterfaceGroupId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "PrefixListName": str,
+        "MaxEntries": int,
+        "AddressFamily": str,
+        "DryRun": NotRequired[bool],
+        "Entries": NotRequired[Sequence[AddPrefixListEntryTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "CreateNatGatewayRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "AllocationId": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ConnectivityType": NotRequired[ConnectivityTypeType],
+        "PrivateIpAddress": NotRequired[str],
+        "SecondaryAllocationIds": NotRequired[Sequence[str]],
+        "SecondaryPrivateIpAddresses": NotRequired[Sequence[str]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+    },
+)
+CreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "CreateNetworkAclRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Protocol": ProtocolType,
+        "ClientToken": str,
+        "SourceIp": NotRequired[str],
+        "DestinationIp": NotRequired[str],
+        "Destination": NotRequired[str],
+        "DestinationPort": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "FilterAtSource": NotRequired[PathRequestFilterTypeDef],
+        "FilterAtDestination": NotRequired[PathRequestFilterTypeDef],
+    },
+)
+CreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Groups": NotRequired[Sequence[str]],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6PrefixCount": NotRequired[int],
+        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "EnablePrimaryIpv6": NotRequired[bool],
+        "ConnectionTrackingSpecification": NotRequired[
+            ConnectionTrackingSpecificationRequestTypeDef
+        ],
+    },
+)
+CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "SubnetId": str,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Groups": NotRequired[Sequence[str]],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[Sequence[PrivateIpAddressSpecificationTypeDef]],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[Sequence[Ipv4PrefixSpecificationRequestTypeDef]],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[Sequence[Ipv6PrefixSpecificationRequestTypeDef]],
+        "Ipv6PrefixCount": NotRequired[int],
+        "InterfaceType": NotRequired[NetworkInterfaceCreationTypeType],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "EnablePrimaryIpv6": NotRequired[bool],
+        "ConnectionTrackingSpecification": NotRequired[
+            ConnectionTrackingSpecificationRequestTypeDef
+        ],
+    },
+)
+CreatePlacementGroupRequestRequestTypeDef = TypedDict(
+    "CreatePlacementGroupRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupName": NotRequired[str],
+        "Strategy": NotRequired[PlacementStrategyType],
+        "PartitionCount": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SpreadLevel": NotRequired[SpreadLevelType],
+    },
+)
+CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupName": NotRequired[str],
+        "Strategy": NotRequired[PlacementStrategyType],
+        "PartitionCount": NotRequired[int],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SpreadLevel": NotRequired[SpreadLevelType],
+    },
+)
+CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ImageId": NotRequired[str],
+        "DeleteReplacedRootVolume": NotRequired[bool],
+    },
+)
+CreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "ObjectKey": str,
+        "Name": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateRouteTableRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "CreateSecurityGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "VpcId": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "VpcId": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotRequestRequestTypeDef = TypedDict(
+    "CreateSnapshotRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "VolumeId": str,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "CreateSnapshotsRequestRequestTypeDef",
+    {
+        "InstanceSpecification": InstanceSpecificationTypeDef,
+        "Description": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "CopyTagsFromSource": NotRequired[Literal["volume"]],
+    },
+)
+CreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Cidr": str,
+        "ReservationType": SubnetCidrReservationTypeType,
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateSubnetRequestRequestTypeDef = TypedDict(
+    "CreateSubnetRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Ipv6Native": NotRequired[bool],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+    },
+)
+CreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "Ipv6Native": NotRequired[bool],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+    },
+)
+CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "TrafficMirrorTargetId": str,
+        "TrafficMirrorFilterId": str,
+        "SessionNumber": int,
+        "PacketLength": NotRequired[int],
+        "VirtualNetworkId": NotRequired[int],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": NotRequired[str],
+        "NetworkLoadBalancerArn": NotRequired[str],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "GatewayLoadBalancerEndpointId": NotRequired[str],
+    },
+)
+CreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAttachmentId": str,
+        "PeerAddress": str,
+        "InsideCidrBlocks": Sequence[str],
+        "TransitGatewayAddress": NotRequired[str],
+        "BgpOptions": NotRequired[TransitGatewayConnectRequestBgpOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TransportTransitGatewayAttachmentId": str,
+        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "Options": NotRequired[CreateTransitGatewayMulticastDomainRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "PeerTransitGatewayId": str,
+        "PeerAccountId": str,
+        "PeerRegion": str,
+        "Options": NotRequired[CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Options": NotRequired[TransitGatewayRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TransitGatewayRouteTableId": str,
+        "PeeringAttachmentId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "VpcId": str,
+        "SubnetIds": Sequence[str],
+        "Options": NotRequired[CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "DryRun": NotRequired[bool],
+    },
+)
+CreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "VerifiedAccessGroupId": str,
+        "EndpointType": VerifiedAccessEndpointTypeType,
+        "AttachmentType": Literal["vpc"],
+        "DomainCertificateArn": str,
+        "ApplicationDomain": str,
+        "EndpointDomainPrefix": str,
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "LoadBalancerOptions": NotRequired[CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef],
+        "NetworkInterfaceOptions": NotRequired[CreateVerifiedAccessEndpointEniOptionsTypeDef],
+        "Description": NotRequired[str],
+        "PolicyDocument": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "VerifiedAccessInstanceId": str,
+        "Description": NotRequired[str],
+        "PolicyDocument": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    {
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "FIPSEnabled": NotRequired[bool],
+    },
+)
+CreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "TrustProviderType": TrustProviderTypeType,
+        "PolicyReferenceName": str,
+        "UserTrustProviderType": NotRequired[UserTrustProviderTypeType],
+        "DeviceTrustProviderType": NotRequired[DeviceTrustProviderTypeType],
+        "OidcOptions": NotRequired[CreateVerifiedAccessTrustProviderOidcOptionsTypeDef],
+        "DeviceOptions": NotRequired[CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef],
+        "Description": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "ClientToken": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "SseSpecification": NotRequired[VerifiedAccessSseSpecificationRequestTypeDef],
+    },
+)
+CreateVolumeRequestRequestTypeDef = TypedDict(
+    "CreateVolumeRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "Encrypted": NotRequired[bool],
+        "Iops": NotRequired[int],
+        "KmsKeyId": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "VolumeType": NotRequired[VolumeTypeType],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiAttachEnabled": NotRequired[bool],
+        "Throughput": NotRequired[int],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "AvailabilityZone": str,
+        "Encrypted": NotRequired[bool],
+        "Iops": NotRequired[int],
+        "KmsKeyId": NotRequired[str],
+        "OutpostArn": NotRequired[str],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "VolumeType": NotRequired[VolumeTypeType],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiAttachEnabled": NotRequired[bool],
+        "Throughput": NotRequired[int],
+        "ClientToken": NotRequired[str],
+    },
+)
+CreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ServiceName": str,
+        "DryRun": NotRequired[bool],
+        "VpcEndpointType": NotRequired[VpcEndpointTypeType],
+        "PolicyDocument": NotRequired[str],
+        "RouteTableIds": NotRequired[Sequence[str]],
+        "SubnetIds": NotRequired[Sequence[str]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "IpAddressType": NotRequired[IpAddressTypeType],
+        "DnsOptions": NotRequired[DnsOptionsSpecificationTypeDef],
+        "ClientToken": NotRequired[str],
+        "PrivateDnsEnabled": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "SubnetConfigurations": NotRequired[Sequence[SubnetConfigurationTypeDef]],
+    },
+)
+CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "AcceptanceRequired": NotRequired[bool],
+        "PrivateDnsName": NotRequired[str],
+        "NetworkLoadBalancerArns": NotRequired[Sequence[str]],
+        "GatewayLoadBalancerArns": NotRequired[Sequence[str]],
+        "SupportedIpAddressTypes": NotRequired[Sequence[str]],
+        "ClientToken": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "PeerOwnerId": NotRequired[str],
+        "PeerVpcId": NotRequired[str],
+        "PeerRegion": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "VpcId": str,
+        "DryRun": NotRequired[bool],
+        "PeerOwnerId": NotRequired[str],
+        "PeerVpcId": NotRequired[str],
+        "PeerRegion": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcRequestRequestTypeDef = TypedDict(
+    "CreateVpcRequestRequestTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
+        "Ipv6Pool": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "InstanceTenancy": NotRequired[TenancyType],
+        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "AmazonProvidedIpv6CidrBlock": NotRequired[bool],
+        "Ipv6Pool": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
+        "Ipv4IpamPoolId": NotRequired[str],
+        "Ipv4NetmaskLength": NotRequired[int],
+        "Ipv6IpamPoolId": NotRequired[str],
+        "Ipv6NetmaskLength": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "InstanceTenancy": NotRequired[TenancyType],
+        "Ipv6CidrBlockNetworkBorderGroup": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+CreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "CreateVpnGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+        "AvailabilityZone": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "AmazonSideAsn": NotRequired[int],
+        "DryRun": NotRequired[bool],
+    },
+)
+ExportImageRequestRequestTypeDef = TypedDict(
+    "ExportImageRequestRequestTypeDef",
+    {
+        "DiskImageFormat": DiskImageFormatType,
+        "ImageId": str,
+        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "RoleName": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportImageRequestRequestTypeDef = TypedDict(
+    "ImportImageRequestRequestTypeDef",
+    {
+        "Architecture": NotRequired[str],
+        "ClientData": NotRequired[ClientDataTypeDef],
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DiskContainers": NotRequired[Sequence[ImageDiskContainerTypeDef]],
+        "DryRun": NotRequired[bool],
+        "Encrypted": NotRequired[bool],
+        "Hypervisor": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "LicenseType": NotRequired[str],
+        "Platform": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "LicenseSpecifications": NotRequired[
+            Sequence[ImportImageLicenseConfigurationRequestTypeDef]
+        ],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "UsageOperation": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+    },
+)
+ImportKeyPairRequestRequestTypeDef = TypedDict(
+    "ImportKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ImportSnapshotRequestRequestTypeDef = TypedDict(
+    "ImportSnapshotRequestRequestTypeDef",
+    {
+        "ClientData": NotRequired[ClientDataTypeDef],
+        "ClientToken": NotRequired[str],
+        "Description": NotRequired[str],
+        "DiskContainer": NotRequired[SnapshotDiskContainerTypeDef],
+        "DryRun": NotRequired[bool],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+ProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "Cidr": str,
+        "CidrAuthorizationContext": NotRequired[CidrAuthorizationContextTypeDef],
+        "PubliclyAdvertisable": NotRequired[bool],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "PoolTagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "MultiRegion": NotRequired[bool],
+        "NetworkBorderGroup": NotRequired[str],
+    },
+)
+PurchaseCapacityBlockRequestRequestTypeDef = TypedDict(
+    "PurchaseCapacityBlockRequestRequestTypeDef",
+    {
+        "CapacityBlockOfferingId": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+PurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "PurchaseHostReservationRequestRequestTypeDef",
+    {
+        "HostIdSet": Sequence[str],
+        "OfferingId": str,
+        "ClientToken": NotRequired[str],
+        "CurrencyCode": NotRequired[Literal["USD"]],
+        "LimitPrice": NotRequired[str],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+RegisterImageRequestRequestTypeDef = TypedDict(
+    "RegisterImageRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ImageLocation": NotRequired[str],
+        "Architecture": NotRequired[ArchitectureValuesType],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "EnaSupport": NotRequired[bool],
+        "KernelId": NotRequired[str],
+        "BillingProducts": NotRequired[Sequence[str]],
+        "RamdiskId": NotRequired[str],
+        "RootDeviceName": NotRequired[str],
+        "SriovNetSupport": NotRequired[str],
+        "VirtualizationType": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+        "TpmSupport": NotRequired[Literal["v2.0"]],
+        "UefiData": NotRequired[str],
+        "ImdsSupport": NotRequired[Literal["v2.0"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+RegisterImageRequestServiceResourceRegisterImageTypeDef = TypedDict(
+    "RegisterImageRequestServiceResourceRegisterImageTypeDef",
+    {
+        "Name": str,
+        "ImageLocation": NotRequired[str],
+        "Architecture": NotRequired[ArchitectureValuesType],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "Description": NotRequired[str],
+        "DryRun": NotRequired[bool],
+        "EnaSupport": NotRequired[bool],
+        "KernelId": NotRequired[str],
+        "BillingProducts": NotRequired[Sequence[str]],
+        "RamdiskId": NotRequired[str],
+        "RootDeviceName": NotRequired[str],
+        "SriovNetSupport": NotRequired[str],
+        "VirtualizationType": NotRequired[str],
+        "BootMode": NotRequired[BootModeValuesType],
+        "TpmSupport": NotRequired[Literal["v2.0"]],
+        "UefiData": NotRequired[str],
+        "ImdsSupport": NotRequired[Literal["v2.0"]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsAccessScopeId": str,
+        "ClientToken": str,
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
+StartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsPathId": str,
+        "ClientToken": str,
+        "AdditionalAccounts": NotRequired[Sequence[str]],
+        "FilterInArns": NotRequired[Sequence[str]],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+    },
+)
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "SequenceNumber": NotRequired[int],
         "AclRule": NotRequired[AnalysisAclRuleTypeDef],
         "AttachedTo": NotRequired[AnalysisComponentTypeDef],
         "Component": NotRequired[AnalysisComponentTypeDef],
@@ -22097,16 +22209,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeRouteTablesResultTypeDef = TypedDict(
     "DescribeRouteTablesResultTypeDef",
     {
         "RouteTables": List[RouteTableTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetFlowLogsIntegrationTemplateRequestRequestTypeDef = TypedDict(
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     {
         "FlowLogId": str,
         "ConfigDeliveryS3DestinationArn": str,
@@ -22165,61 +22277,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeDhcpOptionsResultTypeDef = TypedDict(
     "DescribeDhcpOptionsResultTypeDef",
     {
         "DhcpOptions": List[DhcpOptionsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHostsResultTypeDef = TypedDict(
     "DescribeHostsResultTypeDef",
     {
         "Hosts": List[HostTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BundleInstanceRequestRequestTypeDef = TypedDict(
     "BundleInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Storage": StorageTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
-BundleTaskTypeDef = TypedDict(
-    "BundleTaskTypeDef",
-    {
-        "BundleId": NotRequired[str],
-        "BundleTaskError": NotRequired[BundleTaskErrorTypeDef],
-        "InstanceId": NotRequired[str],
-        "Progress": NotRequired[str],
-        "StartTime": NotRequired[datetime],
-        "State": NotRequired[BundleTaskStateType],
-        "Storage": NotRequired[StorageTypeDef],
-        "UpdateTime": NotRequired[datetime],
-    },
-)
+StorageUnionTypeDef = Union[StorageTypeDef, StorageOutputTypeDef]
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeClientVpnEndpointsResultTypeDef = TypedDict(
     "DescribeClientVpnEndpointsResultTypeDef",
     {
         "ClientVpnEndpoints": List[ClientVpnEndpointTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVpnTunnelOptionsRequestRequestTypeDef = TypedDict(
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     {
         "VpnConnectionId": str,
         "VpnTunnelOutsideIpAddress": str,
@@ -22266,16 +22366,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkAclsResultTypeDef = TypedDict(
     "DescribeNetworkAclsResultTypeDef",
     {
         "NetworkAcls": List[NetworkAclTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisableFastSnapshotRestoresResultTypeDef = TypedDict(
     "DisableFastSnapshotRestoresResultTypeDef",
     {
         "Successful": List[DisableFastSnapshotRestoreSuccessItemTypeDef],
         "Unsuccessful": List[DisableFastSnapshotRestoreErrorItemTypeDef],
@@ -22290,129 +22390,88 @@
         "ImportInstance": NotRequired[ImportInstanceTaskDetailsTypeDef],
         "ImportVolume": NotRequired[ImportVolumeTaskDetailsTypeDef],
         "State": NotRequired[ConversionTaskStateType],
         "StatusMessage": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-RunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
+SpotFleetLaunchSpecificationExtraOutputTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationExtraOutputTypeDef",
     {
-        "MaxCount": int,
-        "MinCount": int,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "AddressingType": NotRequired[str],
+        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
-        "Placement": NotRequired[PlacementTypeDef],
+        "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
+        "NetworkInterfaces": NotRequired[
+            List[InstanceNetworkInterfaceSpecificationExtraOutputTypeDef]
+        ],
+        "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "SecurityGroups": NotRequired[Sequence[str]],
+        "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
-        "AdditionalInfo": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DisableApiTermination": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "EbsOptimized": NotRequired[bool],
-        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
-        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
-        "NetworkInterfaces": NotRequired[
-            Sequence[InstanceNetworkInterfaceSpecificationServiceResourceTypeDef]
-        ],
-        "PrivateIpAddress": NotRequired[str],
-        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
-        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
-        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
-        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
-        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
-        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
-        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
-        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
-        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
-        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
-        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
-        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
-        "DisableApiStop": NotRequired[bool],
-        "EnablePrimaryIpv6": NotRequired[bool],
+        "WeightedCapacity": NotRequired[float],
+        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationExtraOutputTypeDef]],
+        "InstanceRequirements": NotRequired[InstanceRequirementsExtraOutputTypeDef],
     },
 )
-RunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
-    "RunInstancesRequestSubnetCreateInstancesTypeDef",
+LaunchSpecificationTypeDef = TypedDict(
+    "LaunchSpecificationTypeDef",
     {
-        "MaxCount": int,
-        "MinCount": int,
-        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "UserData": NotRequired[str],
+        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "AddressingType": NotRequired[str],
+        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
-        "Ipv6AddressCount": NotRequired[int],
-        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
-        "Placement": NotRequired[PlacementTypeDef],
+        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationOutputTypeDef]],
+        "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
-        "SecurityGroupIds": NotRequired[Sequence[str]],
-        "SecurityGroups": NotRequired[Sequence[str]],
-        "UserData": NotRequired[str],
-        "AdditionalInfo": NotRequired[str],
-        "ClientToken": NotRequired[str],
-        "DisableApiTermination": NotRequired[bool],
-        "DryRun": NotRequired[bool],
-        "EbsOptimized": NotRequired[bool],
-        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
-        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
-        "NetworkInterfaces": NotRequired[
-            Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef]
-        ],
-        "PrivateIpAddress": NotRequired[str],
-        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
-        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
-        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
-        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
-        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
-        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
-        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
-        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
-        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
-        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
-        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
-        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
-        "DisableApiStop": NotRequired[bool],
-        "EnablePrimaryIpv6": NotRequired[bool],
+        "SubnetId": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
     },
 )
-LaunchSpecificationTypeDef = TypedDict(
-    "LaunchSpecificationTypeDef",
+SpotFleetLaunchSpecificationOutputTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationOutputTypeDef",
     {
-        "UserData": NotRequired[str],
         "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
         "AddressingType": NotRequired[str],
         "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
-        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationTypeDef]],
+        "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
+        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationOutputTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
+        "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
-        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "UserData": NotRequired[str],
+        "WeightedCapacity": NotRequired[float],
+        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationOutputTypeDef]],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
     },
 )
+InstanceNetworkInterfaceSpecificationUnionTypeDef = Union[
+    InstanceNetworkInterfaceSpecificationTypeDef,
+    InstanceNetworkInterfaceSpecificationExtraOutputTypeDef,
+]
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SecurityGroups": NotRequired[Sequence[str]],
         "AddressingType": NotRequired[str],
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
@@ -22426,16 +22485,16 @@
         "NetworkInterfaces": NotRequired[Sequence[InstanceNetworkInterfaceSpecificationTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
     },
 )
-RunInstancesRequestRequestTypeDef = TypedDict(
-    "RunInstancesRequestRequestTypeDef",
+RunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
+    "RunInstancesRequestSubnetCreateInstancesTypeDef",
     {
         "MaxCount": int,
         "MinCount": int,
         "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "Ipv6AddressCount": NotRequired[int],
@@ -22443,15 +22502,14 @@
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
         "Placement": NotRequired[PlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SecurityGroups": NotRequired[Sequence[str]],
-        "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
         "AdditionalInfo": NotRequired[str],
         "ClientToken": NotRequired[str],
         "DisableApiTermination": NotRequired[bool],
         "DryRun": NotRequired[bool],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
@@ -22475,32 +22533,32 @@
         "DisableApiStop": NotRequired[bool],
         "EnablePrimaryIpv6": NotRequired[bool],
     },
 )
 SpotFleetLaunchSpecificationTypeDef = TypedDict(
     "SpotFleetLaunchSpecificationTypeDef",
     {
-        "SecurityGroups": NotRequired[List[GroupIdentifierTypeDef]],
+        "SecurityGroups": NotRequired[Sequence[GroupIdentifierTypeDef]],
         "AddressingType": NotRequired[str],
-        "BlockDeviceMappings": NotRequired[List[BlockDeviceMappingTypeDef]],
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
         "EbsOptimized": NotRequired[bool],
         "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
         "ImageId": NotRequired[str],
         "InstanceType": NotRequired[InstanceTypeType],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "Monitoring": NotRequired[SpotFleetMonitoringTypeDef],
-        "NetworkInterfaces": NotRequired[List[InstanceNetworkInterfaceSpecificationTypeDef]],
+        "NetworkInterfaces": NotRequired[Sequence[InstanceNetworkInterfaceSpecificationTypeDef]],
         "Placement": NotRequired[SpotPlacementTypeDef],
         "RamdiskId": NotRequired[str],
         "SpotPrice": NotRequired[str],
         "SubnetId": NotRequired[str],
         "UserData": NotRequired[str],
         "WeightedCapacity": NotRequired[float],
-        "TagSpecifications": NotRequired[List[SpotFleetTagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[SpotFleetTagSpecificationTypeDef]],
         "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
     },
 )
 RequestLaunchTemplateDataTypeDef = TypedDict(
     "RequestLaunchTemplateDataTypeDef",
     {
         "KernelId": NotRequired[str],
@@ -22563,16 +22621,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInsightsPathsResultTypeDef = TypedDict(
     "DescribeNetworkInsightsPathsResultTypeDef",
     {
         "NetworkInsightsPaths": List[NetworkInsightsPathTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceNetworkInterfaceTypeDef = TypedDict(
     "InstanceNetworkInterfaceTypeDef",
     {
         "Association": NotRequired[InstanceNetworkInterfaceAssociationTypeDef],
         "Attachment": NotRequired[InstanceNetworkInterfaceAttachmentTypeDef],
@@ -22593,14 +22651,49 @@
         "Ipv4Prefixes": NotRequired[List[InstanceIpv4PrefixTypeDef]],
         "Ipv6Prefixes": NotRequired[List[InstanceIpv6PrefixTypeDef]],
         "ConnectionTrackingConfiguration": NotRequired[
             ConnectionTrackingSpecificationResponseTypeDef
         ],
     },
 )
+LaunchTemplateConfigExtraOutputTypeDef = TypedDict(
+    "LaunchTemplateConfigExtraOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[LaunchTemplateOverridesExtraOutputTypeDef]],
+    },
+)
+FleetLaunchTemplateConfigTypeDef = TypedDict(
+    "FleetLaunchTemplateConfigTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[FleetLaunchTemplateOverridesTypeDef]],
+    },
+)
+LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
+    "LaunchTemplateAndOverridesResponseTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[FleetLaunchTemplateOverridesTypeDef],
+    },
+)
+LaunchTemplateConfigOutputTypeDef = TypedDict(
+    "LaunchTemplateConfigOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[List[LaunchTemplateOverridesOutputTypeDef]],
+    },
+)
+LaunchTemplateConfigTypeDef = TypedDict(
+    "LaunchTemplateConfigTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
+        "Overrides": NotRequired[Sequence[LaunchTemplateOverridesTypeDef]],
+    },
+)
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationRequestTypeDef],
         "Overrides": NotRequired[Sequence[FleetLaunchTemplateOverridesRequestTypeDef]],
     },
 )
@@ -22631,74 +22724,127 @@
             InstanceRequirementsWithMetadataRequestTypeDef
         ],
         "DryRun": NotRequired[bool],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-FleetLaunchTemplateConfigTypeDef = TypedDict(
-    "FleetLaunchTemplateConfigTypeDef",
+DescribeInstanceStatusResultTypeDef = TypedDict(
+    "DescribeInstanceStatusResultTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[List[FleetLaunchTemplateOverridesTypeDef]],
+        "InstanceStatuses": List[InstanceStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
-    "LaunchTemplateAndOverridesResponseTypeDef",
+DescribeSecurityGroupsResultTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[FleetLaunchTemplateOverridesTypeDef],
+        "SecurityGroups": List[SecurityGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LaunchTemplateConfigTypeDef = TypedDict(
-    "LaunchTemplateConfigTypeDef",
+AuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "LaunchTemplateSpecification": NotRequired[FleetLaunchTemplateSpecificationTypeDef],
-        "Overrides": NotRequired[List[LaunchTemplateOverridesTypeDef]],
+        "GroupId": str,
+        "DryRun": NotRequired[bool],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-DescribeInstanceStatusResultTypeDef = TypedDict(
-    "DescribeInstanceStatusResultTypeDef",
+AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     {
-        "InstanceStatuses": List[InstanceStatusTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "IpProtocol": NotRequired[str],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
-DescribeSecurityGroupsResultPaginatorTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultPaginatorTypeDef",
+RevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "SecurityGroups": List[SecurityGroupPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "GroupId": str,
+        "DryRun": NotRequired[bool],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "IpProtocol": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
     },
 )
-DescribeSecurityGroupsResultTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultTypeDef",
+RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     {
-        "SecurityGroups": List[SecurityGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CidrIp": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "IpProtocol": NotRequired[str],
+        "SourceSecurityGroupName": NotRequired[str],
+        "SourceSecurityGroupOwnerId": NotRequired[str],
+        "ToPort": NotRequired[int],
+        "DryRun": NotRequired[bool],
+        "SecurityGroupRuleIds": NotRequired[Sequence[str]],
+    },
+)
+UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
+    },
+)
+UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    {
+        "DryRun": NotRequired[bool],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "IpPermissions": NotRequired[Sequence[IpPermissionUnionTypeDef]],
+        "SecurityGroupRuleDescriptions": NotRequired[Sequence[SecurityGroupRuleDescriptionTypeDef]],
     },
 )
 DescribeStaleSecurityGroupsResultTypeDef = TypedDict(
     "DescribeStaleSecurityGroupsResultTypeDef",
     {
-        "NextToken": str,
         "StaleSecurityGroupSet": List[StaleSecurityGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetIpamDiscoveredPublicAddressesResultTypeDef = TypedDict(
     "GetIpamDiscoveredPublicAddressesResultTypeDef",
     {
         "IpamDiscoveredPublicAddresses": List[IpamDiscoveredPublicAddressTypeDef],
         "OldestSampleTime": datetime,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ResponseLaunchTemplateDataTypeDef = TypedDict(
     "ResponseLaunchTemplateDataTypeDef",
     {
         "KernelId": NotRequired[str],
         "EbsOptimized": NotRequired[bool],
@@ -22729,26 +22875,26 @@
         "CapacityReservationSpecification": NotRequired[
             LaunchTemplateCapacityReservationSpecificationResponseTypeDef
         ],
         "LicenseSpecifications": NotRequired[List[LaunchTemplateLicenseConfigurationTypeDef]],
         "HibernationOptions": NotRequired[LaunchTemplateHibernationOptionsTypeDef],
         "MetadataOptions": NotRequired[LaunchTemplateInstanceMetadataOptionsTypeDef],
         "EnclaveOptions": NotRequired[LaunchTemplateEnclaveOptionsTypeDef],
-        "InstanceRequirements": NotRequired[InstanceRequirementsTypeDef],
+        "InstanceRequirements": NotRequired[InstanceRequirementsOutputTypeDef],
         "PrivateDnsNameOptions": NotRequired[LaunchTemplatePrivateDnsNameOptionsTypeDef],
         "MaintenanceOptions": NotRequired[LaunchTemplateInstanceMaintenanceOptionsTypeDef],
         "DisableApiStop": NotRequired[bool],
     },
 )
 DescribeReservedInstancesModificationsResultTypeDef = TypedDict(
     "DescribeReservedInstancesModificationsResultTypeDef",
     {
-        "NextToken": str,
         "ReservedInstancesModifications": List[ReservedInstancesModificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InstanceTypeInfoTypeDef = TypedDict(
     "InstanceTypeInfoTypeDef",
     {
         "InstanceType": NotRequired[InstanceTypeType],
         "CurrentGeneration": NotRequired[bool],
@@ -22783,50 +22929,71 @@
 )
 CreateNetworkInsightsAccessScopeRequestRequestTypeDef = TypedDict(
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     {
         "ClientToken": str,
         "MatchPaths": NotRequired[Sequence[AccessScopePathRequestTypeDef]],
         "ExcludePaths": NotRequired[Sequence[AccessScopePathRequestTypeDef]],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
         "DryRun": NotRequired[bool],
     },
 )
 NetworkInsightsAccessScopeContentTypeDef = TypedDict(
     "NetworkInsightsAccessScopeContentTypeDef",
     {
         "NetworkInsightsAccessScopeId": NotRequired[str],
         "MatchPaths": NotRequired[List[AccessScopePathTypeDef]],
         "ExcludePaths": NotRequired[List[AccessScopePathTypeDef]],
     },
 )
+BundleInstanceResultTypeDef = TypedDict(
+    "BundleInstanceResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CancelBundleTaskResultTypeDef = TypedDict(
+    "CancelBundleTaskResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeBundleTasksResultTypeDef = TypedDict(
+    "DescribeBundleTasksResultTypeDef",
+    {
+        "BundleTasks": List[BundleTaskTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 RunScheduledInstancesRequestRequestTypeDef = TypedDict(
     "RunScheduledInstancesRequestRequestTypeDef",
     {
         "LaunchSpecification": ScheduledInstancesLaunchSpecificationTypeDef,
         "ScheduledInstanceId": str,
         "ClientToken": NotRequired[str],
         "DryRun": NotRequired[bool],
         "InstanceCount": NotRequired[int],
     },
 )
 DescribeImportImageTasksResultTypeDef = TypedDict(
     "DescribeImportImageTasksResultTypeDef",
     {
         "ImportImageTasks": List[ImportImageTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeImportSnapshotTasksResultTypeDef = TypedDict(
     "DescribeImportSnapshotTasksResultTypeDef",
     {
         "ImportSnapshotTasks": List[ImportSnapshotTaskTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateDefaultSubnetResultTypeDef = TypedDict(
     "CreateDefaultSubnetResultTypeDef",
     {
         "Subnet": SubnetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22839,32 +23006,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSubnetsResultTypeDef = TypedDict(
     "DescribeSubnetsResultTypeDef",
     {
         "Subnets": List[SubnetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateTrafficMirrorFilterResultTypeDef = TypedDict(
     "CreateTrafficMirrorFilterResultTypeDef",
     {
         "TrafficMirrorFilter": TrafficMirrorFilterTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTrafficMirrorFiltersResultTypeDef = TypedDict(
     "DescribeTrafficMirrorFiltersResultTypeDef",
     {
         "TrafficMirrorFilters": List[TrafficMirrorFilterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyTrafficMirrorFilterNetworkServicesResultTypeDef = TypedDict(
     "ModifyTrafficMirrorFilterNetworkServicesResultTypeDef",
     {
         "TrafficMirrorFilter": TrafficMirrorFilterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22884,16 +23051,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeTransitGatewayConnectPeersResultTypeDef = TypedDict(
     "DescribeTransitGatewayConnectPeersResultTypeDef",
     {
         "TransitGatewayConnectPeers": List[TransitGatewayConnectPeerTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTransitGatewayPolicyTableEntriesResultTypeDef = TypedDict(
     "GetTransitGatewayPolicyTableEntriesResultTypeDef",
     {
         "TransitGatewayPolicyTableEntries": List[TransitGatewayPolicyTableEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22905,17 +23072,17 @@
         "VerifiedAccessInstanceId": NotRequired[str],
         "AccessLogs": NotRequired[VerifiedAccessLogsTypeDef],
     },
 )
 DescribeVolumeStatusResultTypeDef = TypedDict(
     "DescribeVolumeStatusResultTypeDef",
     {
-        "NextToken": str,
         "VolumeStatuses": List[VolumeStatusItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateDefaultVpcResultTypeDef = TypedDict(
     "CreateDefaultVpcResultTypeDef",
     {
         "Vpc": VpcTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22928,16 +23095,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcsResultTypeDef = TypedDict(
     "DescribeVpcsResultTypeDef",
     {
         "Vpcs": List[VpcTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptVpcPeeringConnectionResultTypeDef = TypedDict(
     "AcceptVpcPeeringConnectionResultTypeDef",
     {
         "VpcPeeringConnection": VpcPeeringConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -22950,16 +23117,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVpcPeeringConnectionsResultTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsResultTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AccessScopeAnalysisFindingTypeDef = TypedDict(
     "AccessScopeAnalysisFindingTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": NotRequired[str],
         "NetworkInsightsAccessScopeId": NotRequired[str],
@@ -22996,49 +23163,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNetworkInterfacesResultTypeDef = TypedDict(
     "DescribeNetworkInterfacesResultTypeDef",
     {
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BundleInstanceResultTypeDef = TypedDict(
-    "BundleInstanceResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CancelBundleTaskResultTypeDef = TypedDict(
-    "CancelBundleTaskResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBundleTasksResultTypeDef = TypedDict(
-    "DescribeBundleTasksResultTypeDef",
-    {
-        "BundleTasks": List[BundleTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "CreateVpnConnectionRequestRequestTypeDef",
     {
         "CustomerGatewayId": str,
         "Type": str,
         "VpnGatewayId": NotRequired[str],
         "TransitGatewayId": NotRequired[str],
         "DryRun": NotRequired[bool],
         "Options": NotRequired[VpnConnectionOptionsSpecificationTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
 VpnConnectionTypeDef = TypedDict(
     "VpnConnectionTypeDef",
     {
         "CustomerGatewayConfiguration": NotRequired[str],
         "CustomerGatewayId": NotRequired[str],
@@ -23098,41 +23244,137 @@
         "Tags": NotRequired[List[TagTypeDef]],
         "Type": NotRequired[SpotInstanceTypeType],
         "ValidFrom": NotRequired[datetime],
         "ValidUntil": NotRequired[datetime],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
     },
 )
+RunInstancesRequestRequestTypeDef = TypedDict(
+    "RunInstancesRequestRequestTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "ImageId": NotRequired[str],
+        "InstanceType": NotRequired[InstanceTypeType],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "Placement": NotRequired[PlacementTypeDef],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "SecurityGroups": NotRequired[Sequence[str]],
+        "SubnetId": NotRequired[str],
+        "UserData": NotRequired[str],
+        "AdditionalInfo": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DisableApiTermination": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
+        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
+        "NetworkInterfaces": NotRequired[
+            Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef]
+        ],
+        "PrivateIpAddress": NotRequired[str],
+        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
+        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
+        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
+        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
+        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
+        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
+        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
+        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
+        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
+        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
+        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
+        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
+        "DisableApiStop": NotRequired[bool],
+        "EnablePrimaryIpv6": NotRequired[bool],
+    },
+)
+RunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+        "BlockDeviceMappings": NotRequired[Sequence[BlockDeviceMappingTypeDef]],
+        "ImageId": NotRequired[str],
+        "InstanceType": NotRequired[InstanceTypeType],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[Sequence[InstanceIpv6AddressTypeDef]],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "Monitoring": NotRequired[RunInstancesMonitoringEnabledTypeDef],
+        "Placement": NotRequired[PlacementTypeDef],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "SecurityGroups": NotRequired[Sequence[str]],
+        "SubnetId": NotRequired[str],
+        "UserData": NotRequired[str],
+        "AdditionalInfo": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "DisableApiTermination": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[IamInstanceProfileSpecificationTypeDef],
+        "InstanceInitiatedShutdownBehavior": NotRequired[ShutdownBehaviorType],
+        "NetworkInterfaces": NotRequired[
+            Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef]
+        ],
+        "PrivateIpAddress": NotRequired[str],
+        "ElasticGpuSpecification": NotRequired[Sequence[ElasticGpuSpecificationTypeDef]],
+        "ElasticInferenceAccelerators": NotRequired[Sequence[ElasticInferenceAcceleratorTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "LaunchTemplate": NotRequired[LaunchTemplateSpecificationTypeDef],
+        "InstanceMarketOptions": NotRequired[InstanceMarketOptionsRequestTypeDef],
+        "CreditSpecification": NotRequired[CreditSpecificationRequestTypeDef],
+        "CpuOptions": NotRequired[CpuOptionsRequestTypeDef],
+        "CapacityReservationSpecification": NotRequired[CapacityReservationSpecificationTypeDef],
+        "HibernationOptions": NotRequired[HibernationOptionsRequestTypeDef],
+        "LicenseSpecifications": NotRequired[Sequence[LicenseConfigurationRequestTypeDef]],
+        "MetadataOptions": NotRequired[InstanceMetadataOptionsRequestTypeDef],
+        "EnclaveOptions": NotRequired[EnclaveOptionsRequestTypeDef],
+        "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsRequestTypeDef],
+        "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsRequestTypeDef],
+        "DisableApiStop": NotRequired[bool],
+        "EnablePrimaryIpv6": NotRequired[bool],
+    },
+)
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": NotRequired[str],
         "BlockDurationMinutes": NotRequired[int],
         "ClientToken": NotRequired[str],
         "DryRun": NotRequired[bool],
         "InstanceCount": NotRequired[int],
         "LaunchGroup": NotRequired[str],
         "LaunchSpecification": NotRequired[RequestSpotLaunchSpecificationTypeDef],
         "SpotPrice": NotRequired[str],
         "Type": NotRequired[SpotInstanceTypeType],
         "ValidFrom": NotRequired[TimestampTypeDef],
         "ValidUntil": NotRequired[TimestampTypeDef],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
     },
 )
 CreateLaunchTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchTemplateRequestRequestTypeDef",
     {
         "LaunchTemplateName": str,
         "LaunchTemplateData": RequestLaunchTemplateDataTypeDef,
         "DryRun": NotRequired[bool],
         "ClientToken": NotRequired[str],
         "VersionDescription": NotRequired[str],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
     },
 )
 CreateLaunchTemplateVersionRequestRequestTypeDef = TypedDict(
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     {
         "LaunchTemplateData": RequestLaunchTemplateDataTypeDef,
         "DryRun": NotRequired[bool],
@@ -23206,42 +23448,43 @@
         "PrivateDnsNameOptions": NotRequired[PrivateDnsNameOptionsResponseTypeDef],
         "Ipv6Address": NotRequired[str],
         "TpmSupport": NotRequired[str],
         "MaintenanceOptions": NotRequired[InstanceMaintenanceOptionsTypeDef],
         "CurrentInstanceBootMode": NotRequired[InstanceBootModeValuesType],
     },
 )
-CreateFleetRequestRequestTypeDef = TypedDict(
-    "CreateFleetRequestRequestTypeDef",
+SpotFleetRequestConfigDataExtraOutputTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataExtraOutputTypeDef",
     {
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
-        "DryRun": NotRequired[bool],
+        "IamFleetRole": str,
+        "TargetCapacity": int,
+        "AllocationStrategy": NotRequired[AllocationStrategyType],
+        "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
+        "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
-        "SpotOptions": NotRequired[SpotOptionsRequestTypeDef],
-        "OnDemandOptions": NotRequired[OnDemandOptionsRequestTypeDef],
-        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
+        "FulfilledCapacity": NotRequired[float],
+        "OnDemandFulfilledCapacity": NotRequired[float],
+        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationExtraOutputTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigExtraOutputTypeDef]],
+        "SpotPrice": NotRequired[str],
+        "OnDemandTargetCapacity": NotRequired[int],
+        "OnDemandMaxTotalPrice": NotRequired[str],
+        "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
-        "ValidFrom": NotRequired[TimestampTypeDef],
-        "ValidUntil": NotRequired[TimestampTypeDef],
+        "ValidFrom": NotRequired[datetime],
+        "ValidUntil": NotRequired[datetime],
         "ReplaceUnhealthyInstances": NotRequired[bool],
-        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
-        "Context": NotRequired[str],
-    },
-)
-ModifyFleetRequestRequestTypeDef = TypedDict(
-    "ModifyFleetRequestRequestTypeDef",
-    {
-        "FleetId": str,
-        "DryRun": NotRequired[bool],
-        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
-        "LaunchTemplateConfigs": NotRequired[Sequence[FleetLaunchTemplateConfigRequestTypeDef]],
-        "TargetCapacitySpecification": NotRequired[TargetCapacitySpecificationRequestTypeDef],
+        "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
+        "LoadBalancersConfig": NotRequired[LoadBalancersConfigExtraOutputTypeDef],
+        "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
+        "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
+        "TagSpecifications": NotRequired[List[TagSpecificationExtraOutputTypeDef]],
     },
 )
 CreateFleetErrorTypeDef = TypedDict(
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": NotRequired[LaunchTemplateAndOverridesResponseTypeDef],
         "Lifecycle": NotRequired[InstanceLifecycleType],
@@ -23274,85 +23517,107 @@
         "LaunchTemplateAndOverrides": NotRequired[LaunchTemplateAndOverridesResponseTypeDef],
         "Lifecycle": NotRequired[InstanceLifecycleType],
         "InstanceIds": NotRequired[List[str]],
         "InstanceType": NotRequired[InstanceTypeType],
         "Platform": NotRequired[Literal["windows"]],
     },
 )
-ModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "ModifySpotFleetRequestRequestRequestTypeDef",
-    {
-        "SpotFleetRequestId": str,
-        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
-        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigTypeDef]],
-        "TargetCapacity": NotRequired[int],
-        "OnDemandTargetCapacity": NotRequired[int],
-        "Context": NotRequired[str],
-    },
-)
-SpotFleetRequestConfigDataPaginatorTypeDef = TypedDict(
-    "SpotFleetRequestConfigDataPaginatorTypeDef",
+SpotFleetRequestConfigDataOutputTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataOutputTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
         "AllocationStrategy": NotRequired[AllocationStrategyType],
         "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
         "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
         "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
         "FulfilledCapacity": NotRequired[float],
         "OnDemandFulfilledCapacity": NotRequired[float],
-        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationTypeDef]],
-        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigTypeDef]],
+        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationOutputTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigOutputTypeDef]],
         "SpotPrice": NotRequired[str],
         "OnDemandTargetCapacity": NotRequired[int],
         "OnDemandMaxTotalPrice": NotRequired[str],
         "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
         "ValidFrom": NotRequired[datetime],
         "ValidUntil": NotRequired[datetime],
         "ReplaceUnhealthyInstances": NotRequired[bool],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
-        "LoadBalancersConfig": NotRequired[LoadBalancersConfigTypeDef],
+        "LoadBalancersConfig": NotRequired[LoadBalancersConfigOutputTypeDef],
         "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
         "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
-        "TagSpecifications": NotRequired[List[TagSpecificationPaginatorTypeDef]],
+        "TagSpecifications": NotRequired[List[TagSpecificationOutputTypeDef]],
     },
 )
+LaunchTemplateConfigUnionTypeDef = Union[
+    LaunchTemplateConfigTypeDef, LaunchTemplateConfigExtraOutputTypeDef
+]
 SpotFleetRequestConfigDataTypeDef = TypedDict(
     "SpotFleetRequestConfigDataTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
         "AllocationStrategy": NotRequired[AllocationStrategyType],
         "OnDemandAllocationStrategy": NotRequired[OnDemandAllocationStrategyType],
         "SpotMaintenanceStrategies": NotRequired[SpotMaintenanceStrategiesTypeDef],
         "ClientToken": NotRequired[str],
         "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
         "FulfilledCapacity": NotRequired[float],
         "OnDemandFulfilledCapacity": NotRequired[float],
-        "LaunchSpecifications": NotRequired[List[SpotFleetLaunchSpecificationTypeDef]],
-        "LaunchTemplateConfigs": NotRequired[List[LaunchTemplateConfigTypeDef]],
+        "LaunchSpecifications": NotRequired[Sequence[SpotFleetLaunchSpecificationTypeDef]],
+        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigTypeDef]],
         "SpotPrice": NotRequired[str],
         "OnDemandTargetCapacity": NotRequired[int],
         "OnDemandMaxTotalPrice": NotRequired[str],
         "SpotMaxTotalPrice": NotRequired[str],
         "TerminateInstancesWithExpiration": NotRequired[bool],
         "Type": NotRequired[FleetTypeType],
-        "ValidFrom": NotRequired[datetime],
-        "ValidUntil": NotRequired[datetime],
+        "ValidFrom": NotRequired[TimestampTypeDef],
+        "ValidUntil": NotRequired[TimestampTypeDef],
         "ReplaceUnhealthyInstances": NotRequired[bool],
         "InstanceInterruptionBehavior": NotRequired[InstanceInterruptionBehaviorType],
         "LoadBalancersConfig": NotRequired[LoadBalancersConfigTypeDef],
         "InstancePoolsToUseCount": NotRequired[int],
         "Context": NotRequired[str],
         "TargetCapacityUnitType": NotRequired[TargetCapacityUnitTypeType],
-        "TagSpecifications": NotRequired[List[TagSpecificationTypeDef]],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationTypeDef]],
+    },
+)
+CreateFleetRequestRequestTypeDef = TypedDict(
+    "CreateFleetRequestRequestTypeDef",
+    {
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "DryRun": NotRequired[bool],
+        "ClientToken": NotRequired[str],
+        "SpotOptions": NotRequired[SpotOptionsRequestTypeDef],
+        "OnDemandOptions": NotRequired[OnDemandOptionsRequestTypeDef],
+        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "TerminateInstancesWithExpiration": NotRequired[bool],
+        "Type": NotRequired[FleetTypeType],
+        "ValidFrom": NotRequired[TimestampTypeDef],
+        "ValidUntil": NotRequired[TimestampTypeDef],
+        "ReplaceUnhealthyInstances": NotRequired[bool],
+        "TagSpecifications": NotRequired[Sequence[TagSpecificationUnionTypeDef]],
+        "Context": NotRequired[str],
+    },
+)
+ModifyFleetRequestRequestTypeDef = TypedDict(
+    "ModifyFleetRequestRequestTypeDef",
+    {
+        "FleetId": str,
+        "DryRun": NotRequired[bool],
+        "ExcessCapacityTerminationPolicy": NotRequired[FleetExcessCapacityTerminationPolicyType],
+        "LaunchTemplateConfigs": NotRequired[Sequence[FleetLaunchTemplateConfigRequestTypeDef]],
+        "TargetCapacitySpecification": NotRequired[TargetCapacitySpecificationRequestTypeDef],
+        "Context": NotRequired[str],
     },
 )
 GetLaunchTemplateDataResultTypeDef = TypedDict(
     "GetLaunchTemplateDataResultTypeDef",
     {
         "LaunchTemplateData": ResponseLaunchTemplateDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23371,16 +23636,16 @@
         "LaunchTemplateData": NotRequired[ResponseLaunchTemplateDataTypeDef],
     },
 )
 DescribeInstanceTypesResultTypeDef = TypedDict(
     "DescribeInstanceTypesResultTypeDef",
     {
         "InstanceTypes": List[InstanceTypeInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateNetworkInsightsAccessScopeResultTypeDef = TypedDict(
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     {
         "NetworkInsightsAccessScope": NetworkInsightsAccessScopeTypeDef,
         "NetworkInsightsAccessScopeContent": NetworkInsightsAccessScopeContentTypeDef,
@@ -23394,16 +23659,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef = TypedDict(
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     {
         "LoggingConfigurations": List[VerifiedAccessInstanceLoggingConfigurationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef = TypedDict(
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
     {
         "LoggingConfiguration": VerifiedAccessInstanceLoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23411,24 +23676,24 @@
 )
 GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef = TypedDict(
     "GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "AnalysisStatus": AnalysisStatusType,
         "AnalysisFindings": List[AccessScopeAnalysisFindingTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeNetworkInsightsAnalysesResultTypeDef = TypedDict(
     "DescribeNetworkInsightsAnalysesResultTypeDef",
     {
         "NetworkInsightsAnalyses": List[NetworkInsightsAnalysisTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartNetworkInsightsAnalysisResultTypeDef = TypedDict(
     "StartNetworkInsightsAnalysisResultTypeDef",
     {
         "NetworkInsightsAnalysis": NetworkInsightsAnalysisTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23476,16 +23741,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSpotInstanceRequestsResultTypeDef = TypedDict(
     "DescribeSpotInstanceRequestsResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RequestSpotInstancesResultTypeDef = TypedDict(
     "RequestSpotInstancesResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -23543,84 +23808,79 @@
         "OnDemandOptions": NotRequired[OnDemandOptionsTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
         "Errors": NotRequired[List[DescribeFleetErrorTypeDef]],
         "Instances": NotRequired[List[DescribeFleetsInstancesTypeDef]],
         "Context": NotRequired[str],
     },
 )
-SpotFleetRequestConfigPaginatorTypeDef = TypedDict(
-    "SpotFleetRequestConfigPaginatorTypeDef",
+SpotFleetRequestConfigTypeDef = TypedDict(
+    "SpotFleetRequestConfigTypeDef",
     {
         "ActivityStatus": NotRequired[ActivityStatusType],
         "CreateTime": NotRequired[datetime],
-        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataPaginatorTypeDef],
+        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataOutputTypeDef],
         "SpotFleetRequestId": NotRequired[str],
         "SpotFleetRequestState": NotRequired[BatchStateType],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+ModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "ModifySpotFleetRequestRequestRequestTypeDef",
+    {
+        "SpotFleetRequestId": str,
+        "ExcessCapacityTerminationPolicy": NotRequired[ExcessCapacityTerminationPolicyType],
+        "LaunchTemplateConfigs": NotRequired[Sequence[LaunchTemplateConfigUnionTypeDef]],
+        "TargetCapacity": NotRequired[int],
+        "OnDemandTargetCapacity": NotRequired[int],
+        "Context": NotRequired[str],
+    },
+)
 RequestSpotFleetRequestRequestTypeDef = TypedDict(
     "RequestSpotFleetRequestRequestTypeDef",
     {
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
         "DryRun": NotRequired[bool],
     },
 )
-SpotFleetRequestConfigTypeDef = TypedDict(
-    "SpotFleetRequestConfigTypeDef",
-    {
-        "ActivityStatus": NotRequired[ActivityStatusType],
-        "CreateTime": NotRequired[datetime],
-        "SpotFleetRequestConfig": NotRequired[SpotFleetRequestConfigDataTypeDef],
-        "SpotFleetRequestId": NotRequired[str],
-        "SpotFleetRequestState": NotRequired[BatchStateType],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
+SpotFleetRequestConfigDataUnionTypeDef = Union[
+    SpotFleetRequestConfigDataTypeDef, SpotFleetRequestConfigDataExtraOutputTypeDef
+]
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
         "LaunchTemplateVersion": LaunchTemplateVersionTypeDef,
         "Warning": ValidationWarningTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeLaunchTemplateVersionsResultTypeDef = TypedDict(
     "DescribeLaunchTemplateVersionsResultTypeDef",
     {
         "LaunchTemplateVersions": List[LaunchTemplateVersionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Reservations": List[ReservationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
-        "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeSpotFleetRequestsResponsePaginatorTypeDef = TypedDict(
-    "DescribeSpotFleetRequestsResponsePaginatorTypeDef",
-    {
-        "NextToken": str,
-        "SpotFleetRequestConfigs": List[SpotFleetRequestConfigPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpotFleetRequestsResponseTypeDef = TypedDict(
     "DescribeSpotFleetRequestsResponseTypeDef",
     {
-        "NextToken": str,
         "SpotFleetRequestConfigs": List[SpotFleetRequestConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/waiter.py` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2/waiter.pyi` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.91
-Summary: Type annotations for boto3.EC2 1.34.91 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_ec2-1.34.91/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.91/setup.py` & `mypy_boto3_ec2-1.34.96/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.34.91",
+    version="1.34.96",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EC2 1.34.91 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

