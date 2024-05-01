# Comparing `tmp/mypy-boto3-sesv2-1.34.56.tar.gz` & `tmp/mypy_boto3_sesv2-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.34.56.tar", last modified: Tue Mar  5 20:22:18 2024, max compression
+gzip compressed data, was "mypy_boto3_sesv2-1.34.96.tar", last modified: Wed May  1 19:21:17 2024, max compression
```

## Comparing `mypy-boto3-sesv2-1.34.56.tar` & `mypy_boto3_sesv2-1.34.96.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:18.223455 mypy-boto3-sesv2-1.34.56/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-03-05 20:22:18.223455 mypy-boto3-sesv2-1.34.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:18.223455 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59785 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59782 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    66705 2024-03-05 20:22:07.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66705 2024-03-05 20:22:07.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:18.223455 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 20:22:18.000000 mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 20:22:18.223455 mypy-boto3-sesv2-1.34.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-05 20:22:05.000000 mypy-boto3-sesv2-1.34.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59825 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59822 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    70365 2024-05-01 19:21:04.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70365 2024-05-01 19:21:04.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 19:21:17.000000 mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:17.132335 mypy_boto3_sesv2-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-01 19:21:03.000000 mypy_boto3_sesv2-1.34.96/setup.py
```

### Comparing `mypy-boto3-sesv2-1.34.56/LICENSE` & `mypy_boto3_sesv2-1.34.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.34.56/PKG-INFO` & `mypy_boto3_sesv2-1.34.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.34.56
-Summary: Type annotations for boto3.SESV2 1.34.56 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.34.56/README.md` & `mypy_boto3_sesv2-1.34.96/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/__main__.py` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.34.56\n"
-        "Version:         1.34.56\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.SESV2 1.34.96\n"
+        "Version:         1.34.96\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.56")
+    print("1.34.96")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/client.py` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateExportJobResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
-    ExportDataSourceTypeDef,
+    ExportDataSourceUnionTypeDef,
     ExportDestinationTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetContactListResponseTypeDef,
     GetContactResponseTypeDef,
@@ -86,20 +86,20 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -187,18 +187,18 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -329,15 +329,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_email_template)
         """
 
     def create_export_job(
         self,
         *,
-        ExportDataSource: ExportDataSourceTypeDef,
+        ExportDataSource: ExportDataSourceUnionTypeDef,
         ExportDestination: ExportDestinationTypeDef,
     ) -> CreateExportJobResponseTypeDef:
         """
         Creates an export job for a data source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_export_job)
@@ -1014,15 +1014,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/client.pyi` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateExportJobResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
-    ExportDataSourceTypeDef,
+    ExportDataSourceUnionTypeDef,
     ExportDestinationTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetContactListResponseTypeDef,
     GetContactResponseTypeDef,
@@ -86,20 +86,20 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -184,18 +184,18 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -326,15 +326,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_email_template)
         """
 
     def create_export_job(
         self,
         *,
-        ExportDataSource: ExportDataSourceTypeDef,
+        ExportDataSource: ExportDataSourceUnionTypeDef,
         ExportDestination: ExportDestinationTypeDef,
     ) -> CreateExportJobResponseTypeDef:
         """
         Creates an export job for a data source and destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_export_job)
@@ -1011,15 +1011,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...,
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/literals.py` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -235,24 +236,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -313,15 +316,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -450,14 +452,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -501,14 +504,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/literals.pyi` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -235,24 +236,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -313,15 +316,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -450,14 +452,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -501,14 +504,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/type_defs.py` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,28 +120,31 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "ExportJobSummaryTypeDef",
     "ExportMetricTypeDef",
     "ExportStatisticsTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
@@ -171,14 +174,15 @@
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageHeaderTypeDef",
+    "MessageInsightsFiltersOutputTypeDef",
     "MessageInsightsFiltersTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
@@ -219,14 +223,15 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "EventDetailsTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
@@ -247,63 +252,71 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
     "ListExportJobsResponseTypeDef",
+    "MetricsDataSourceOutputTypeDef",
     "MetricsDataSourceTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "TemplateTypeDef",
+    "MessageInsightsDataSourceOutputTypeDef",
     "MessageInsightsDataSourceTypeDef",
     "ReplacementEmailContentTypeDef",
     "VerificationInfoTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "InsightsEventTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailContentTypeDef",
+    "ExportDataSourceOutputTypeDef",
     "ExportDataSourceTypeDef",
     "BulkEmailEntryTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "EmailInsightsTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
-    "CreateExportJobRequestRequestTypeDef",
     "GetExportJobResponseTypeDef",
+    "CreateExportJobRequestRequestTypeDef",
+    "ExportDataSourceUnionTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
     "GetMessageInsightsResponseTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -677,19 +690,26 @@
         "ReadRate": NotRequired[float],
         "DeleteRate": NotRequired[float],
         "ReadDeleteRate": NotRequired[float],
         "ProjectedVolume": NotRequired[int],
         "Esps": NotRequired[List[str]],
     },
 )
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
+    {
+        "Global": NotRequired[bool],
+        "TrackedIsps": NotRequired[List[str]],
+    },
+)
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": NotRequired[bool],
-        "TrackedIsps": NotRequired[List[str]],
+        "TrackedIsps": NotRequired[Sequence[str]],
     },
 )
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": NotRequired[str],
         "CreatedTimestamp": NotRequired[datetime],
@@ -773,14 +793,27 @@
 )
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": NotRequired[bool],
+        "LastFreshStart": NotRequired[datetime],
+    },
+)
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": NotRequired[List[SuppressionListReasonType]],
+    },
+)
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 GetContactRequestRequestTypeDef = TypedDict(
@@ -1032,14 +1065,25 @@
 MessageHeaderTypeDef = TypedDict(
     "MessageHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
+MessageInsightsFiltersOutputTypeDef = TypedDict(
+    "MessageInsightsFiltersOutputTypeDef",
+    {
+        "FromEmailAddress": NotRequired[List[str]],
+        "Destination": NotRequired[List[str]],
+        "Subject": NotRequired[List[str]],
+        "Isp": NotRequired[List[str]],
+        "LastDeliveryEvent": NotRequired[List[DeliveryEventTypeType]],
+        "LastEngagementEvent": NotRequired[List[EngagementEventTypeType]],
+    },
+)
 MessageInsightsFiltersTypeDef = TypedDict(
     "MessageInsightsFiltersTypeDef",
     {
         "FromEmailAddress": NotRequired[Sequence[str]],
         "Destination": NotRequired[Sequence[str]],
         "Subject": NotRequired[Sequence[str]],
         "Isp": NotRequired[Sequence[str]],
@@ -1337,24 +1381,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListConfigurationSetsResponseTypeDef = TypedDict(
     "ListConfigurationSetsResponseTypeDef",
     {
         "ConfigurationSets": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDedicatedIpPoolsResponseTypeDef = TypedDict(
     "ListDedicatedIpPoolsResponseTypeDef",
     {
         "DedicatedIpPools": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
     "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     {
         "DkimStatus": DkimStatusType,
         "DkimTokens": List[str],
@@ -1405,14 +1449,20 @@
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
+    },
+)
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 EventDetailsTypeDef = TypedDict(
@@ -1422,16 +1472,16 @@
         "Complaint": NotRequired[ComplaintTypeDef],
     },
 )
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": NotRequired[str],
         "TopicPreferences": NotRequired[List[TopicPreferenceTypeDef]],
@@ -1573,16 +1623,16 @@
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": NotRequired[datetime],
         "VolumeStatistics": NotRequired[VolumeStatisticsTypeDef],
@@ -1611,75 +1661,94 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "SubscriptionStartDate": NotRequired[datetime],
+        "InboxPlacementTrackingOption": NotRequired[InboxPlacementTrackingOptionOutputTypeDef],
     },
 )
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": NotRequired[str],
-        "SubscriptionStartDate": NotRequired[datetime],
+        "SubscriptionStartDate": NotRequired[TimestampTypeDef],
         "InboxPlacementTrackingOption": NotRequired[InboxPlacementTrackingOptionTypeDef],
     },
 )
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListExportJobsResponseTypeDef = TypedDict(
     "ListExportJobsResponseTypeDef",
     {
         "ExportJobs": List[ExportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MetricsDataSourceOutputTypeDef = TypedDict(
+    "MetricsDataSourceOutputTypeDef",
+    {
+        "Dimensions": Dict[MetricDimensionNameType, List[str]],
+        "Namespace": Literal["VDM"],
+        "Metrics": List[ExportMetricTypeDef],
+        "StartDate": datetime,
+        "EndDate": datetime,
     },
 )
 MetricsDataSourceTypeDef = TypedDict(
     "MetricsDataSourceTypeDef",
     {
         "Dimensions": Mapping[MetricDimensionNameType, Sequence[str]],
         "Namespace": Literal["VDM"],
         "Metrics": Sequence[ExportMetricTypeDef],
         "StartDate": TimestampTypeDef,
         "EndDate": TimestampTypeDef,
     },
 )
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": NotRequired[str],
         "PlacementStatistics": NotRequired[PlacementStatisticsTypeDef],
     },
 )
@@ -1698,16 +1767,16 @@
         "GuardianOptions": NotRequired[GuardianOptionsTypeDef],
     },
 )
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": NotRequired[SuppressionListDestinationTypeDef],
         "ContactListDestination": NotRequired[ContactListDestinationTypeDef],
@@ -1720,35 +1789,45 @@
         "TopicFilter": NotRequired[TopicFilterTypeDef],
     },
 )
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": NotRequired[str],
         "TemplateArn": NotRequired[str],
         "TemplateData": NotRequired[str],
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
+MessageInsightsDataSourceOutputTypeDef = TypedDict(
+    "MessageInsightsDataSourceOutputTypeDef",
+    {
+        "StartDate": datetime,
+        "EndDate": datetime,
+        "Include": NotRequired[MessageInsightsFiltersOutputTypeDef],
+        "Exclude": NotRequired[MessageInsightsFiltersOutputTypeDef],
+        "MaxResults": NotRequired[int],
+    },
+)
 MessageInsightsDataSourceTypeDef = TypedDict(
     "MessageInsightsDataSourceTypeDef",
     {
         "StartDate": TimestampTypeDef,
         "EndDate": TimestampTypeDef,
         "Include": NotRequired[MessageInsightsFiltersTypeDef],
         "Exclude": NotRequired[MessageInsightsFiltersTypeDef],
@@ -1781,39 +1860,40 @@
 )
 BatchGetMetricDataRequestRequestTypeDef = TypedDict(
     "BatchGetMetricDataRequestRequestTypeDef",
     {
         "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
     },
 )
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
+EventDestinationTypeDef = TypedDict(
+    "EventDestinationTypeDef",
     {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
-        "MatchingEventTypes": NotRequired[Sequence[EventTypeType]],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
-        "CloudWatchDestination": NotRequired[CloudWatchDestinationTypeDef],
+        "CloudWatchDestination": NotRequired[CloudWatchDestinationOutputTypeDef],
         "SnsDestination": NotRequired[SnsDestinationTypeDef],
         "PinpointDestination": NotRequired[PinpointDestinationTypeDef],
     },
 )
-EventDestinationTypeDef = TypedDict(
-    "EventDestinationTypeDef",
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
     {
-        "Name": str,
-        "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
+        "MatchingEventTypes": NotRequired[Sequence[EventTypeType]],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
         "CloudWatchDestination": NotRequired[CloudWatchDestinationTypeDef],
         "SnsDestination": NotRequired[SnsDestinationTypeDef],
         "PinpointDestination": NotRequired[PinpointDestinationTypeDef],
     },
 )
 InsightsEventTypeDef = TypedDict(
@@ -1824,16 +1904,16 @@
         "Details": NotRequired[EventDetailsTypeDef],
     },
 )
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
@@ -1842,26 +1922,22 @@
 )
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-        "SubscribedDomains": NotRequired[Sequence[DomainDeliverabilityTrackingOptionTypeDef]],
-    },
-)
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -1904,18 +1980,18 @@
 )
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
@@ -1967,14 +2043,21 @@
 )
 BulkEmailContentTypeDef = TypedDict(
     "BulkEmailContentTypeDef",
     {
         "Template": NotRequired[TemplateTypeDef],
     },
 )
+ExportDataSourceOutputTypeDef = TypedDict(
+    "ExportDataSourceOutputTypeDef",
+    {
+        "MetricsDataSource": NotRequired[MetricsDataSourceOutputTypeDef],
+        "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceOutputTypeDef],
+    },
+)
 ExportDataSourceTypeDef = TypedDict(
     "ExportDataSourceTypeDef",
     {
         "MetricsDataSource": NotRequired[MetricsDataSourceTypeDef],
         "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceTypeDef],
     },
 )
@@ -2013,14 +2096,21 @@
     "EmailContentTypeDef",
     {
         "Simple": NotRequired[MessageTypeDef],
         "Raw": NotRequired[RawMessageTypeDef],
         "Template": NotRequired[TemplateTypeDef],
     },
 )
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2029,59 +2119,60 @@
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 EmailInsightsTypeDef = TypedDict(
     "EmailInsightsTypeDef",
     {
         "Destination": NotRequired[str],
         "Isp": NotRequired[str],
         "Events": NotRequired[List[InsightsEventTypeDef]],
     },
 )
+PutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+        "SubscribedDomains": NotRequired[Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef]],
+    },
+)
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateExportJobRequestRequestTypeDef = TypedDict(
-    "CreateExportJobRequestRequestTypeDef",
-    {
-        "ExportDataSource": ExportDataSourceTypeDef,
-        "ExportDestination": ExportDestinationTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "JobId": str,
         "ExportSourceType": ExportSourceTypeType,
         "JobStatus": JobStatusType,
         "ExportDestination": ExportDestinationTypeDef,
-        "ExportDataSource": ExportDataSourceTypeDef,
+        "ExportDataSource": ExportDataSourceOutputTypeDef,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "FailureInfo": FailureInfoTypeDef,
         "Statistics": ExportStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateExportJobRequestRequestTypeDef = TypedDict(
+    "CreateExportJobRequestRequestTypeDef",
+    {
+        "ExportDataSource": ExportDataSourceTypeDef,
+        "ExportDestination": ExportDestinationTypeDef,
+    },
+)
+ExportDataSourceUnionTypeDef = Union[ExportDataSourceTypeDef, ExportDataSourceOutputTypeDef]
 SendBulkEmailRequestRequestTypeDef = TypedDict(
     "SendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
         "BulkEmailEntries": Sequence[BulkEmailEntryTypeDef],
         "FromEmailAddress": NotRequired[str],
         "FromEmailAddressIdentityArn": NotRequired[str],
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2/type_defs.pyi` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -120,28 +120,31 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "ExportJobSummaryTypeDef",
     "ExportMetricTypeDef",
     "ExportStatisticsTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
@@ -171,14 +174,15 @@
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageHeaderTypeDef",
+    "MessageInsightsFiltersOutputTypeDef",
     "MessageInsightsFiltersTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
@@ -219,14 +223,15 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "EventDetailsTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
@@ -247,63 +252,71 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
     "ListExportJobsResponseTypeDef",
+    "MetricsDataSourceOutputTypeDef",
     "MetricsDataSourceTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "TemplateTypeDef",
+    "MessageInsightsDataSourceOutputTypeDef",
     "MessageInsightsDataSourceTypeDef",
     "ReplacementEmailContentTypeDef",
     "VerificationInfoTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "InsightsEventTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailContentTypeDef",
+    "ExportDataSourceOutputTypeDef",
     "ExportDataSourceTypeDef",
     "BulkEmailEntryTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "EmailInsightsTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
-    "CreateExportJobRequestRequestTypeDef",
     "GetExportJobResponseTypeDef",
+    "CreateExportJobRequestRequestTypeDef",
+    "ExportDataSourceUnionTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
     "GetMessageInsightsResponseTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -677,19 +690,26 @@
         "ReadRate": NotRequired[float],
         "DeleteRate": NotRequired[float],
         "ReadDeleteRate": NotRequired[float],
         "ProjectedVolume": NotRequired[int],
         "Esps": NotRequired[List[str]],
     },
 )
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
+    {
+        "Global": NotRequired[bool],
+        "TrackedIsps": NotRequired[List[str]],
+    },
+)
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": NotRequired[bool],
-        "TrackedIsps": NotRequired[List[str]],
+        "TrackedIsps": NotRequired[Sequence[str]],
     },
 )
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": NotRequired[str],
         "CreatedTimestamp": NotRequired[datetime],
@@ -773,14 +793,27 @@
 )
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": NotRequired[bool],
+        "LastFreshStart": NotRequired[datetime],
+    },
+)
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": NotRequired[List[SuppressionListReasonType]],
+    },
+)
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 GetContactRequestRequestTypeDef = TypedDict(
@@ -1032,14 +1065,25 @@
 MessageHeaderTypeDef = TypedDict(
     "MessageHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
+MessageInsightsFiltersOutputTypeDef = TypedDict(
+    "MessageInsightsFiltersOutputTypeDef",
+    {
+        "FromEmailAddress": NotRequired[List[str]],
+        "Destination": NotRequired[List[str]],
+        "Subject": NotRequired[List[str]],
+        "Isp": NotRequired[List[str]],
+        "LastDeliveryEvent": NotRequired[List[DeliveryEventTypeType]],
+        "LastEngagementEvent": NotRequired[List[EngagementEventTypeType]],
+    },
+)
 MessageInsightsFiltersTypeDef = TypedDict(
     "MessageInsightsFiltersTypeDef",
     {
         "FromEmailAddress": NotRequired[Sequence[str]],
         "Destination": NotRequired[Sequence[str]],
         "Subject": NotRequired[Sequence[str]],
         "Isp": NotRequired[Sequence[str]],
@@ -1337,24 +1381,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListConfigurationSetsResponseTypeDef = TypedDict(
     "ListConfigurationSetsResponseTypeDef",
     {
         "ConfigurationSets": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDedicatedIpPoolsResponseTypeDef = TypedDict(
     "ListDedicatedIpPoolsResponseTypeDef",
     {
         "DedicatedIpPools": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
     "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     {
         "DkimStatus": DkimStatusType,
         "DkimTokens": List[str],
@@ -1405,14 +1449,20 @@
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
+    },
+)
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 EventDetailsTypeDef = TypedDict(
@@ -1422,16 +1472,16 @@
         "Complaint": NotRequired[ComplaintTypeDef],
     },
 )
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": NotRequired[str],
         "TopicPreferences": NotRequired[List[TopicPreferenceTypeDef]],
@@ -1573,16 +1623,16 @@
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": NotRequired[datetime],
         "VolumeStatistics": NotRequired[VolumeStatisticsTypeDef],
@@ -1611,75 +1661,94 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "SubscriptionStartDate": NotRequired[datetime],
+        "InboxPlacementTrackingOption": NotRequired[InboxPlacementTrackingOptionOutputTypeDef],
     },
 )
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": NotRequired[str],
-        "SubscriptionStartDate": NotRequired[datetime],
+        "SubscriptionStartDate": NotRequired[TimestampTypeDef],
         "InboxPlacementTrackingOption": NotRequired[InboxPlacementTrackingOptionTypeDef],
     },
 )
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListExportJobsResponseTypeDef = TypedDict(
     "ListExportJobsResponseTypeDef",
     {
         "ExportJobs": List[ExportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MetricsDataSourceOutputTypeDef = TypedDict(
+    "MetricsDataSourceOutputTypeDef",
+    {
+        "Dimensions": Dict[MetricDimensionNameType, List[str]],
+        "Namespace": Literal["VDM"],
+        "Metrics": List[ExportMetricTypeDef],
+        "StartDate": datetime,
+        "EndDate": datetime,
     },
 )
 MetricsDataSourceTypeDef = TypedDict(
     "MetricsDataSourceTypeDef",
     {
         "Dimensions": Mapping[MetricDimensionNameType, Sequence[str]],
         "Namespace": Literal["VDM"],
         "Metrics": Sequence[ExportMetricTypeDef],
         "StartDate": TimestampTypeDef,
         "EndDate": TimestampTypeDef,
     },
 )
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": NotRequired[str],
         "PlacementStatistics": NotRequired[PlacementStatisticsTypeDef],
     },
 )
@@ -1698,16 +1767,16 @@
         "GuardianOptions": NotRequired[GuardianOptionsTypeDef],
     },
 )
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": NotRequired[SuppressionListDestinationTypeDef],
         "ContactListDestination": NotRequired[ContactListDestinationTypeDef],
@@ -1720,35 +1789,45 @@
         "TopicFilter": NotRequired[TopicFilterTypeDef],
     },
 )
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": NotRequired[str],
         "TemplateArn": NotRequired[str],
         "TemplateData": NotRequired[str],
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
+MessageInsightsDataSourceOutputTypeDef = TypedDict(
+    "MessageInsightsDataSourceOutputTypeDef",
+    {
+        "StartDate": datetime,
+        "EndDate": datetime,
+        "Include": NotRequired[MessageInsightsFiltersOutputTypeDef],
+        "Exclude": NotRequired[MessageInsightsFiltersOutputTypeDef],
+        "MaxResults": NotRequired[int],
+    },
+)
 MessageInsightsDataSourceTypeDef = TypedDict(
     "MessageInsightsDataSourceTypeDef",
     {
         "StartDate": TimestampTypeDef,
         "EndDate": TimestampTypeDef,
         "Include": NotRequired[MessageInsightsFiltersTypeDef],
         "Exclude": NotRequired[MessageInsightsFiltersTypeDef],
@@ -1781,39 +1860,40 @@
 )
 BatchGetMetricDataRequestRequestTypeDef = TypedDict(
     "BatchGetMetricDataRequestRequestTypeDef",
     {
         "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
     },
 )
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
         "Headers": NotRequired[Sequence[MessageHeaderTypeDef]],
     },
 )
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
+EventDestinationTypeDef = TypedDict(
+    "EventDestinationTypeDef",
     {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
-        "MatchingEventTypes": NotRequired[Sequence[EventTypeType]],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
-        "CloudWatchDestination": NotRequired[CloudWatchDestinationTypeDef],
+        "CloudWatchDestination": NotRequired[CloudWatchDestinationOutputTypeDef],
         "SnsDestination": NotRequired[SnsDestinationTypeDef],
         "PinpointDestination": NotRequired[PinpointDestinationTypeDef],
     },
 )
-EventDestinationTypeDef = TypedDict(
-    "EventDestinationTypeDef",
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
     {
-        "Name": str,
-        "MatchingEventTypes": List[EventTypeType],
         "Enabled": NotRequired[bool],
+        "MatchingEventTypes": NotRequired[Sequence[EventTypeType]],
         "KinesisFirehoseDestination": NotRequired[KinesisFirehoseDestinationTypeDef],
         "CloudWatchDestination": NotRequired[CloudWatchDestinationTypeDef],
         "SnsDestination": NotRequired[SnsDestinationTypeDef],
         "PinpointDestination": NotRequired[PinpointDestinationTypeDef],
     },
 )
 InsightsEventTypeDef = TypedDict(
@@ -1824,16 +1904,16 @@
         "Details": NotRequired[EventDetailsTypeDef],
     },
 )
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
@@ -1842,26 +1922,22 @@
 )
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-        "SubscribedDomains": NotRequired[Sequence[DomainDeliverabilityTrackingOptionTypeDef]],
-    },
-)
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -1904,18 +1980,18 @@
 )
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
@@ -1967,14 +2043,21 @@
 )
 BulkEmailContentTypeDef = TypedDict(
     "BulkEmailContentTypeDef",
     {
         "Template": NotRequired[TemplateTypeDef],
     },
 )
+ExportDataSourceOutputTypeDef = TypedDict(
+    "ExportDataSourceOutputTypeDef",
+    {
+        "MetricsDataSource": NotRequired[MetricsDataSourceOutputTypeDef],
+        "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceOutputTypeDef],
+    },
+)
 ExportDataSourceTypeDef = TypedDict(
     "ExportDataSourceTypeDef",
     {
         "MetricsDataSource": NotRequired[MetricsDataSourceTypeDef],
         "MessageInsightsDataSource": NotRequired[MessageInsightsDataSourceTypeDef],
     },
 )
@@ -2013,14 +2096,21 @@
     "EmailContentTypeDef",
     {
         "Simple": NotRequired[MessageTypeDef],
         "Raw": NotRequired[RawMessageTypeDef],
         "Template": NotRequired[TemplateTypeDef],
     },
 )
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2029,59 +2119,60 @@
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 EmailInsightsTypeDef = TypedDict(
     "EmailInsightsTypeDef",
     {
         "Destination": NotRequired[str],
         "Isp": NotRequired[str],
         "Events": NotRequired[List[InsightsEventTypeDef]],
     },
 )
+PutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+        "SubscribedDomains": NotRequired[Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef]],
+    },
+)
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateExportJobRequestRequestTypeDef = TypedDict(
-    "CreateExportJobRequestRequestTypeDef",
-    {
-        "ExportDataSource": ExportDataSourceTypeDef,
-        "ExportDestination": ExportDestinationTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "JobId": str,
         "ExportSourceType": ExportSourceTypeType,
         "JobStatus": JobStatusType,
         "ExportDestination": ExportDestinationTypeDef,
-        "ExportDataSource": ExportDataSourceTypeDef,
+        "ExportDataSource": ExportDataSourceOutputTypeDef,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "FailureInfo": FailureInfoTypeDef,
         "Statistics": ExportStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateExportJobRequestRequestTypeDef = TypedDict(
+    "CreateExportJobRequestRequestTypeDef",
+    {
+        "ExportDataSource": ExportDataSourceTypeDef,
+        "ExportDestination": ExportDestinationTypeDef,
+    },
+)
+ExportDataSourceUnionTypeDef = Union[ExportDataSourceTypeDef, ExportDataSourceOutputTypeDef]
 SendBulkEmailRequestRequestTypeDef = TypedDict(
     "SendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
         "BulkEmailEntries": Sequence[BulkEmailEntryTypeDef],
         "FromEmailAddress": NotRequired[str],
         "FromEmailAddressIdentityArn": NotRequired[str],
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.34.56
-Summary: Type annotations for boto3.SESV2 1.34.56 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.34.56/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy_boto3_sesv2-1.34.96/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.34.56/setup.py` & `mypy_boto3_sesv2-1.34.96/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.34.56",
+    version="1.34.96",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SESV2 1.34.56 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.SESV2 1.34.96 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

