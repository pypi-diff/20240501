# Comparing `tmp/mypy-boto3-personalize-runtime-1.34.20.tar.gz` & `tmp/mypy_boto3_personalize_runtime-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-runtime-1.34.20.tar", last modified: Tue Jan 16 20:32:46 2024, max compression
+gzip compressed data, was "mypy_boto3_personalize_runtime-1.34.96.tar", last modified: Wed May  1 19:21:16 2024, max compression
```

## Comparing `mypy-boto3-personalize-runtime-1.34.20.tar` & `mypy_boto3_personalize_runtime-1.34.96.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.460973 mypy-boto3-personalize-runtime-1.34.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-01-16 20:32:46.460973 mypy-boto3-personalize-runtime-1.34.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.460973 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.460973 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-16 20:32:46.000000 mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 20:32:46.460973 mypy-boto3-personalize-runtime-1.34.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-16 20:32:10.000000 mypy-boto3-personalize-runtime-1.34.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.380329 mypy_boto3_personalize_runtime-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-05-01 19:21:16.380329 mypy_boto3_personalize_runtime-1.34.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.376329 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.380329 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 19:21:16.000000 mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:16.380329 mypy_boto3_personalize_runtime-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-01 19:20:40.000000 mypy_boto3_personalize_runtime-1.34.96/setup.py
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/LICENSE` & `mypy_boto3_personalize_runtime-1.34.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.34.20/PKG-INFO` & `mypy_boto3_personalize_runtime-1.34.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.34.20
-Summary: Type annotations for boto3.PersonalizeRuntime 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.96
+Summary: Type annotations for boto3.PersonalizeRuntime 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/README.md` & `mypy_boto3_personalize_runtime-1.34.96/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/client.py` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/client.pyi` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/literals.py` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -62,14 +63,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -87,14 +89,15 @@
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
@@ -107,24 +110,26 @@
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
@@ -185,15 +190,14 @@
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
@@ -322,14 +326,15 @@
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
@@ -373,14 +378,15 @@
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

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/literals.pyi` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -62,14 +63,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -87,14 +89,15 @@
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
@@ -107,24 +110,26 @@
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
@@ -185,15 +190,14 @@
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
@@ -322,14 +326,15 @@
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
@@ -373,14 +378,15 @@
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

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/type_defs.py` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         "score": NotRequired[float],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GetPersonalizedRankingRequestRequestTypeDef = TypedDict(
     "GetPersonalizedRankingRequestRequestTypeDef",
     {
         "campaignArn": str,
         "inputList": Sequence[str],
@@ -79,14 +79,15 @@
 PredictedItemTypeDef = TypedDict(
     "PredictedItemTypeDef",
     {
         "itemId": NotRequired[str],
         "score": NotRequired[float],
         "promotionName": NotRequired[str],
         "metadata": NotRequired[Dict[str, str]],
+        "reason": NotRequired[List[str]],
     },
 )
 PromotionTypeDef = TypedDict(
     "PromotionTypeDef",
     {
         "name": NotRequired[str],
         "percentPromotedItems": NotRequired[int],
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime/type_defs.pyi` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         "score": NotRequired[float],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 GetPersonalizedRankingRequestRequestTypeDef = TypedDict(
     "GetPersonalizedRankingRequestRequestTypeDef",
     {
         "campaignArn": str,
         "inputList": Sequence[str],
@@ -79,14 +79,15 @@
 PredictedItemTypeDef = TypedDict(
     "PredictedItemTypeDef",
     {
         "itemId": NotRequired[str],
         "score": NotRequired[float],
         "promotionName": NotRequired[str],
         "metadata": NotRequired[Dict[str, str]],
+        "reason": NotRequired[List[str]],
     },
 )
 PromotionTypeDef = TypedDict(
     "PromotionTypeDef",
     {
         "name": NotRequired[str],
         "percentPromotedItems": NotRequired[int],
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/PKG-INFO` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.34.20
-Summary: Type annotations for boto3.PersonalizeRuntime 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.96
+Summary: Type annotations for boto3.PersonalizeRuntime 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-runtime)](https://pepy.tech/project/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-runtime-1.34.20/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt` & `mypy_boto3_personalize_runtime-1.34.96/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.34.20/setup.py` & `mypy_boto3_personalize_runtime-1.34.96/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-runtime",
-    version="1.34.20",
+    version="1.34.96",
     packages=["mypy_boto3_personalize_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.PersonalizeRuntime 1.34.20 service generated with"
-        " mypy-boto3-builder 7.23.1"
-    ),
+    description="Type annotations for boto3.PersonalizeRuntime 1.34.96 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -41,17 +38,15 @@
     ],
     keywords="boto3 personalize-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_personalize_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.8",
     project_urls={
-        "Documentation": (
-            "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/"
-        ),
+        "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
     ],
     zip_safe=False,
```

