# Comparing `tmp/mypy_boto3_bedrock_agent-1.34.90.tar.gz` & `tmp/mypy_boto3_bedrock_agent-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.90.tar", last modified: Tue Apr 23 19:34:19 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.96.tar", last modified: Wed May  1 19:21:15 2024, max compression
```

## Comparing `mypy_boto3_bedrock_agent-1.34.90.tar` & `mypy_boto3_bedrock_agent-1.34.96.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.308555 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34392 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42365 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42365 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.308555 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34440 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34437 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45674 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45674 2024-05-01 19:19:59.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 19:21:15.000000 mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:15.448320 mypy_boto3_bedrock_agent-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-01 19:19:58.000000 mypy_boto3_bedrock_agent-1.34.96/setup.py
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/LICENSE` & `mypy_boto3_bedrock_agent-1.34.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.90
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [mypy-boto3-bedrock-agent docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/README.md` & `mypy_boto3_bedrock_agent-1.34.96/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [mypy-boto3-bedrock-agent docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.pyi` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__main__.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AgentsforBedrock 1.34.90\n"
-        "Version:         1.34.90\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.AgentsforBedrock 1.34.96\n"
+        "Version:         1.34.96\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.90")
+    print("1.34.96")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,21 +36,21 @@
     APISchemaTypeDef,
     AssociateAgentKnowledgeBaseResponseTypeDef,
     CreateAgentActionGroupResponseTypeDef,
     CreateAgentAliasResponseTypeDef,
     CreateAgentResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateKnowledgeBaseResponseTypeDef,
-    DataSourceConfigurationTypeDef,
+    DataSourceConfigurationUnionTypeDef,
     DeleteAgentAliasResponseTypeDef,
     DeleteAgentResponseTypeDef,
     DeleteAgentVersionResponseTypeDef,
     DeleteDataSourceResponseTypeDef,
     DeleteKnowledgeBaseResponseTypeDef,
-    FunctionSchemaTypeDef,
+    FunctionSchemaUnionTypeDef,
     GetAgentActionGroupResponseTypeDef,
     GetAgentAliasResponseTypeDef,
     GetAgentKnowledgeBaseResponseTypeDef,
     GetAgentResponseTypeDef,
     GetAgentVersionResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetIngestionJobResponseTypeDef,
@@ -64,15 +64,15 @@
     ListAgentsResponseTypeDef,
     ListAgentVersionsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListIngestionJobsResponseTypeDef,
     ListKnowledgeBasesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PrepareAgentResponseTypeDef,
-    PromptOverrideConfigurationTypeDef,
+    PromptOverrideConfigurationUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartIngestionJobResponseTypeDef,
     StorageConfigurationTypeDef,
     UpdateAgentActionGroupResponseTypeDef,
     UpdateAgentAliasResponseTypeDef,
     UpdateAgentKnowledgeBaseResponseTypeDef,
     UpdateAgentResponseTypeDef,
@@ -164,15 +164,15 @@
         agentResourceRoleArn: str = ...,
         clientToken: str = ...,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         foundationModel: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
+        promptOverrideConfiguration: PromptOverrideConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Creates an agent that orchestrates interactions between foundation models, data
         sources, software applications, user conversations, and APIs to carry out tasks
         to help
         customers.
@@ -188,15 +188,15 @@
         agentId: str,
         agentVersion: str,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
         apiSchema: APISchemaTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
-        functionSchema: FunctionSchemaTypeDef = ...,
+        functionSchema: FunctionSchemaUnionTypeDef = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
     ) -> CreateAgentActionGroupResponseTypeDef:
         """
         Creates an action group for an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#create_agent_action_group)
@@ -218,15 +218,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#create_agent_alias)
         """
 
     def create_data_source(
         self,
         *,
-        dataSourceConfiguration: DataSourceConfigurationTypeDef,
+        dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,
         knowledgeBaseId: str,
         name: str,
         clientToken: str = ...,
         dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
@@ -562,15 +562,15 @@
         agentName: str,
         agentResourceRoleArn: str,
         foundationModel: str,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
+        promptOverrideConfiguration: PromptOverrideConfigurationUnionTypeDef = ...,
     ) -> UpdateAgentResponseTypeDef:
         """
         Updates the configuration of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent)
         """
@@ -582,15 +582,15 @@
         actionGroupName: str,
         agentId: str,
         agentVersion: str,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
         apiSchema: APISchemaTypeDef = ...,
         description: str = ...,
-        functionSchema: FunctionSchemaTypeDef = ...,
+        functionSchema: FunctionSchemaUnionTypeDef = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
     ) -> UpdateAgentActionGroupResponseTypeDef:
         """
         Updates the configuration for an action group for an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent_action_group)
@@ -628,15 +628,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent_knowledge_base)
         """
 
     def update_data_source(
         self,
         *,
-        dataSourceConfiguration: DataSourceConfigurationTypeDef,
+        dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,
         dataSourceId: str,
         knowledgeBaseId: str,
         name: str,
         dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.pyi` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,21 +36,21 @@
     APISchemaTypeDef,
     AssociateAgentKnowledgeBaseResponseTypeDef,
     CreateAgentActionGroupResponseTypeDef,
     CreateAgentAliasResponseTypeDef,
     CreateAgentResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateKnowledgeBaseResponseTypeDef,
-    DataSourceConfigurationTypeDef,
+    DataSourceConfigurationUnionTypeDef,
     DeleteAgentAliasResponseTypeDef,
     DeleteAgentResponseTypeDef,
     DeleteAgentVersionResponseTypeDef,
     DeleteDataSourceResponseTypeDef,
     DeleteKnowledgeBaseResponseTypeDef,
-    FunctionSchemaTypeDef,
+    FunctionSchemaUnionTypeDef,
     GetAgentActionGroupResponseTypeDef,
     GetAgentAliasResponseTypeDef,
     GetAgentKnowledgeBaseResponseTypeDef,
     GetAgentResponseTypeDef,
     GetAgentVersionResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetIngestionJobResponseTypeDef,
@@ -64,15 +64,15 @@
     ListAgentsResponseTypeDef,
     ListAgentVersionsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListIngestionJobsResponseTypeDef,
     ListKnowledgeBasesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PrepareAgentResponseTypeDef,
-    PromptOverrideConfigurationTypeDef,
+    PromptOverrideConfigurationUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartIngestionJobResponseTypeDef,
     StorageConfigurationTypeDef,
     UpdateAgentActionGroupResponseTypeDef,
     UpdateAgentAliasResponseTypeDef,
     UpdateAgentKnowledgeBaseResponseTypeDef,
     UpdateAgentResponseTypeDef,
@@ -161,15 +161,15 @@
         agentResourceRoleArn: str = ...,
         clientToken: str = ...,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         foundationModel: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
+        promptOverrideConfiguration: PromptOverrideConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateAgentResponseTypeDef:
         """
         Creates an agent that orchestrates interactions between foundation models, data
         sources, software applications, user conversations, and APIs to carry out tasks
         to help
         customers.
@@ -185,15 +185,15 @@
         agentId: str,
         agentVersion: str,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
         apiSchema: APISchemaTypeDef = ...,
         clientToken: str = ...,
         description: str = ...,
-        functionSchema: FunctionSchemaTypeDef = ...,
+        functionSchema: FunctionSchemaUnionTypeDef = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
     ) -> CreateAgentActionGroupResponseTypeDef:
         """
         Creates an action group for an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#create_agent_action_group)
@@ -215,15 +215,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#create_agent_alias)
         """
 
     def create_data_source(
         self,
         *,
-        dataSourceConfiguration: DataSourceConfigurationTypeDef,
+        dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,
         knowledgeBaseId: str,
         name: str,
         clientToken: str = ...,
         dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
@@ -559,15 +559,15 @@
         agentName: str,
         agentResourceRoleArn: str,
         foundationModel: str,
         customerEncryptionKeyArn: str = ...,
         description: str = ...,
         idleSessionTTLInSeconds: int = ...,
         instruction: str = ...,
-        promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,
+        promptOverrideConfiguration: PromptOverrideConfigurationUnionTypeDef = ...,
     ) -> UpdateAgentResponseTypeDef:
         """
         Updates the configuration of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent)
         """
@@ -579,15 +579,15 @@
         actionGroupName: str,
         agentId: str,
         agentVersion: str,
         actionGroupExecutor: ActionGroupExecutorTypeDef = ...,
         actionGroupState: ActionGroupStateType = ...,
         apiSchema: APISchemaTypeDef = ...,
         description: str = ...,
-        functionSchema: FunctionSchemaTypeDef = ...,
+        functionSchema: FunctionSchemaUnionTypeDef = ...,
         parentActionGroupSignature: Literal["AMAZON.UserInput"] = ...,
     ) -> UpdateAgentActionGroupResponseTypeDef:
         """
         Updates the configuration for an action group for an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent_action_group)
@@ -625,15 +625,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/client/#update_agent_knowledge_base)
         """
 
     def update_data_source(
         self,
         *,
-        dataSourceConfiguration: DataSourceConfigurationTypeDef,
+        dataSourceConfiguration: DataSourceConfigurationUnionTypeDef,
         dataSourceId: str,
         knowledgeBaseId: str,
         name: str,
         dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 IngestionJobSortByAttributeType = Literal["STARTED_AT", "STATUS"]
 IngestionJobStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS", "STARTING"]
 KnowledgeBaseStateType = Literal["DISABLED", "ENABLED"]
 KnowledgeBaseStatusType = Literal[
     "ACTIVE", "CREATING", "DELETE_UNSUCCESSFUL", "DELETING", "FAILED", "UPDATING"
 ]
 KnowledgeBaseStorageTypeType = Literal[
-    "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
+    "MONGO_DB_ATLAS", "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
 ]
 KnowledgeBaseTypeType = Literal["VECTOR"]
 ListAgentActionGroupsPaginatorName = Literal["list_agent_action_groups"]
 ListAgentAliasesPaginatorName = Literal["list_agent_aliases"]
 ListAgentKnowledgeBasesPaginatorName = Literal["list_agent_knowledge_bases"]
 ListAgentVersionsPaginatorName = Literal["list_agent_versions"]
 ListAgentsPaginatorName = Literal["list_agents"]
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.pyi` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 IngestionJobSortByAttributeType = Literal["STARTED_AT", "STATUS"]
 IngestionJobStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS", "STARTING"]
 KnowledgeBaseStateType = Literal["DISABLED", "ENABLED"]
 KnowledgeBaseStatusType = Literal[
     "ACTIVE", "CREATING", "DELETE_UNSUCCESSFUL", "DELETING", "FAILED", "UPDATING"
 ]
 KnowledgeBaseStorageTypeType = Literal[
-    "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
+    "MONGO_DB_ATLAS", "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
 ]
 KnowledgeBaseTypeType = Literal["VECTOR"]
 ListAgentActionGroupsPaginatorName = Literal["list_agent_action_groups"]
 ListAgentAliasesPaginatorName = Literal["list_agent_aliases"]
 ListAgentKnowledgeBasesPaginatorName = Literal["list_agent_knowledge_bases"]
 ListAgentVersionsPaginatorName = Literal["list_agent_versions"]
 ListAgentsPaginatorName = Literal["list_agents"]
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.pyi` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.py` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: S3IdentifierTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionGroupStateType,
     AgentAliasStatusType,
     AgentStatusType,
     ChunkingStrategyType,
     CreationModeType,
@@ -57,14 +57,15 @@
     "AgentKnowledgeBaseTypeDef",
     "AgentSummaryTypeDef",
     "AgentVersionSummaryTypeDef",
     "AssociateAgentKnowledgeBaseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "FixedSizeChunkingConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
+    "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "DataSourceSummaryTypeDef",
     "DeleteAgentActionGroupRequestRequestTypeDef",
     "DeleteAgentAliasRequestRequestTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteAgentVersionRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -75,14 +76,15 @@
     "GetAgentAliasRequestRequestTypeDef",
     "GetAgentKnowledgeBaseRequestRequestTypeDef",
     "GetAgentRequestRequestTypeDef",
     "GetAgentVersionRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetIngestionJobRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
+    "InferenceConfigurationOutputTypeDef",
     "InferenceConfigurationTypeDef",
     "IngestionJobFilterTypeDef",
     "IngestionJobSortByTypeDef",
     "IngestionJobStatisticsTypeDef",
     "VectorKnowledgeBaseConfigurationTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "PaginatorConfigTypeDef",
@@ -90,14 +92,15 @@
     "ListAgentAliasesRequestRequestTypeDef",
     "ListAgentKnowledgeBasesRequestRequestTypeDef",
     "ListAgentVersionsRequestRequestTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "MongoDbAtlasFieldMappingTypeDef",
     "OpenSearchServerlessFieldMappingTypeDef",
     "PineconeFieldMappingTypeDef",
     "PrepareAgentRequestRequestTypeDef",
     "RdsFieldMappingTypeDef",
     "RedisEnterpriseCloudFieldMappingTypeDef",
     "StartIngestionJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -119,56 +122,65 @@
     "ListAgentKnowledgeBasesResponseTypeDef",
     "ListAgentVersionsResponseTypeDef",
     "ListAgentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PrepareAgentResponseTypeDef",
     "UpdateAgentKnowledgeBaseResponseTypeDef",
     "ChunkingConfigurationTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "FunctionOutputTypeDef",
     "FunctionTypeDef",
+    "PromptConfigurationOutputTypeDef",
     "PromptConfigurationTypeDef",
     "ListIngestionJobsRequestRequestTypeDef",
     "IngestionJobSummaryTypeDef",
     "IngestionJobTypeDef",
     "KnowledgeBaseConfigurationTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef",
     "ListAgentAliasesRequestListAgentAliasesPaginateTypeDef",
     "ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef",
     "ListAgentVersionsRequestListAgentVersionsPaginateTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListIngestionJobsRequestListIngestionJobsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "MongoDbAtlasConfigurationTypeDef",
     "OpenSearchServerlessConfigurationTypeDef",
     "PineconeConfigurationTypeDef",
     "RdsConfigurationTypeDef",
     "RedisEnterpriseCloudConfigurationTypeDef",
     "AgentAliasTypeDef",
     "ListAgentAliasesResponseTypeDef",
     "VectorIngestionConfigurationTypeDef",
+    "DataSourceConfigurationUnionTypeDef",
+    "FunctionSchemaOutputTypeDef",
     "FunctionSchemaTypeDef",
+    "PromptOverrideConfigurationOutputTypeDef",
     "PromptOverrideConfigurationTypeDef",
     "ListIngestionJobsResponseTypeDef",
     "GetIngestionJobResponseTypeDef",
     "StartIngestionJobResponseTypeDef",
     "StorageConfigurationTypeDef",
     "CreateAgentAliasResponseTypeDef",
     "GetAgentAliasResponseTypeDef",
     "UpdateAgentAliasResponseTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "DataSourceTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "AgentActionGroupTypeDef",
     "CreateAgentActionGroupRequestRequestTypeDef",
+    "FunctionSchemaUnionTypeDef",
     "UpdateAgentActionGroupRequestRequestTypeDef",
     "AgentTypeDef",
     "AgentVersionTypeDef",
     "CreateAgentRequestRequestTypeDef",
+    "PromptOverrideConfigurationUnionTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseTypeDef",
     "UpdateKnowledgeBaseRequestRequestTypeDef",
     "CreateDataSourceResponseTypeDef",
     "GetDataSourceResponseTypeDef",
     "UpdateDataSourceResponseTypeDef",
@@ -286,14 +298,22 @@
 )
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyArn": NotRequired[str],
     },
 )
+S3DataSourceConfigurationOutputTypeDef = TypedDict(
+    "S3DataSourceConfigurationOutputTypeDef",
+    {
+        "bucketArn": str,
+        "bucketOwnerAccountId": NotRequired[str],
+        "inclusionPrefixes": NotRequired[List[str]],
+    },
+)
 S3DataSourceConfigurationTypeDef = TypedDict(
     "S3DataSourceConfigurationTypeDef",
     {
         "bucketArn": str,
         "bucketOwnerAccountId": NotRequired[str],
         "inclusionPrefixes": NotRequired[Sequence[str]],
     },
@@ -422,14 +442,24 @@
 )
 GetKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "GetKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
+InferenceConfigurationOutputTypeDef = TypedDict(
+    "InferenceConfigurationOutputTypeDef",
+    {
+        "maximumLength": NotRequired[int],
+        "stopSequences": NotRequired[List[str]],
+        "temperature": NotRequired[float],
+        "topK": NotRequired[int],
+        "topP": NotRequired[float],
+    },
+)
 InferenceConfigurationTypeDef = TypedDict(
     "InferenceConfigurationTypeDef",
     {
         "maximumLength": NotRequired[int],
         "stopSequences": NotRequired[Sequence[str]],
         "temperature": NotRequired[float],
         "topK": NotRequired[int],
@@ -545,14 +575,22 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+MongoDbAtlasFieldMappingTypeDef = TypedDict(
+    "MongoDbAtlasFieldMappingTypeDef",
+    {
+        "metadataField": str,
+        "textField": str,
+        "vectorField": str,
+    },
+)
 OpenSearchServerlessFieldMappingTypeDef = TypedDict(
     "OpenSearchServerlessFieldMappingTypeDef",
     {
         "metadataField": str,
         "textField": str,
         "vectorField": str,
     },
@@ -788,14 +826,21 @@
 ChunkingConfigurationTypeDef = TypedDict(
     "ChunkingConfigurationTypeDef",
     {
         "chunkingStrategy": ChunkingStrategyType,
         "fixedSizeChunkingConfiguration": NotRequired[FixedSizeChunkingConfigurationTypeDef],
     },
 )
+DataSourceConfigurationOutputTypeDef = TypedDict(
+    "DataSourceConfigurationOutputTypeDef",
+    {
+        "type": Literal["S3"],
+        "s3Configuration": NotRequired[S3DataSourceConfigurationOutputTypeDef],
+    },
+)
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "type": Literal["S3"],
         "s3Configuration": NotRequired[S3DataSourceConfigurationTypeDef],
     },
 )
@@ -803,22 +848,41 @@
     "ListDataSourcesResponseTypeDef",
     {
         "dataSourceSummaries": List[DataSourceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FunctionOutputTypeDef = TypedDict(
+    "FunctionOutputTypeDef",
+    {
+        "name": str,
+        "description": NotRequired[str],
+        "parameters": NotRequired[Dict[str, ParameterDetailTypeDef]],
+    },
+)
 FunctionTypeDef = TypedDict(
     "FunctionTypeDef",
     {
         "name": str,
         "description": NotRequired[str],
         "parameters": NotRequired[Mapping[str, ParameterDetailTypeDef]],
     },
 )
+PromptConfigurationOutputTypeDef = TypedDict(
+    "PromptConfigurationOutputTypeDef",
+    {
+        "basePromptTemplate": NotRequired[str],
+        "inferenceConfiguration": NotRequired[InferenceConfigurationOutputTypeDef],
+        "parserMode": NotRequired[CreationModeType],
+        "promptCreationMode": NotRequired[CreationModeType],
+        "promptState": NotRequired[PromptStateType],
+        "promptType": NotRequired[PromptTypeType],
+    },
+)
 PromptConfigurationTypeDef = TypedDict(
     "PromptConfigurationTypeDef",
     {
         "basePromptTemplate": NotRequired[str],
         "inferenceConfiguration": NotRequired[InferenceConfigurationTypeDef],
         "parserMode": NotRequired[CreationModeType],
         "promptCreationMode": NotRequired[CreationModeType],
@@ -934,14 +998,26 @@
 )
 ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+MongoDbAtlasConfigurationTypeDef = TypedDict(
+    "MongoDbAtlasConfigurationTypeDef",
+    {
+        "collectionName": str,
+        "credentialsSecretArn": str,
+        "databaseName": str,
+        "endpoint": str,
+        "fieldMapping": MongoDbAtlasFieldMappingTypeDef,
+        "vectorIndexName": str,
+        "endpointServiceName": NotRequired[str],
+    },
+)
 OpenSearchServerlessConfigurationTypeDef = TypedDict(
     "OpenSearchServerlessConfigurationTypeDef",
     {
         "collectionArn": str,
         "fieldMapping": OpenSearchServerlessFieldMappingTypeDef,
         "vectorIndexName": str,
     },
@@ -1000,20 +1076,36 @@
 )
 VectorIngestionConfigurationTypeDef = TypedDict(
     "VectorIngestionConfigurationTypeDef",
     {
         "chunkingConfiguration": NotRequired[ChunkingConfigurationTypeDef],
     },
 )
+DataSourceConfigurationUnionTypeDef = Union[
+    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+]
+FunctionSchemaOutputTypeDef = TypedDict(
+    "FunctionSchemaOutputTypeDef",
+    {
+        "functions": NotRequired[List[FunctionOutputTypeDef]],
+    },
+)
 FunctionSchemaTypeDef = TypedDict(
     "FunctionSchemaTypeDef",
     {
         "functions": NotRequired[Sequence[FunctionTypeDef]],
     },
 )
+PromptOverrideConfigurationOutputTypeDef = TypedDict(
+    "PromptOverrideConfigurationOutputTypeDef",
+    {
+        "promptConfigurations": List[PromptConfigurationOutputTypeDef],
+        "overrideLambda": NotRequired[str],
+    },
+)
 PromptOverrideConfigurationTypeDef = TypedDict(
     "PromptOverrideConfigurationTypeDef",
     {
         "promptConfigurations": Sequence[PromptConfigurationTypeDef],
         "overrideLambda": NotRequired[str],
     },
 )
@@ -1039,14 +1131,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "type": KnowledgeBaseStorageTypeType,
+        "mongoDbAtlasConfiguration": NotRequired[MongoDbAtlasConfigurationTypeDef],
         "opensearchServerlessConfiguration": NotRequired[OpenSearchServerlessConfigurationTypeDef],
         "pineconeConfiguration": NotRequired[PineconeConfigurationTypeDef],
         "rdsConfiguration": NotRequired[RdsConfigurationTypeDef],
         "redisEnterpriseCloudConfiguration": NotRequired[RedisEnterpriseCloudConfigurationTypeDef],
     },
 )
 CreateAgentAliasResponseTypeDef = TypedDict(
@@ -1083,15 +1176,15 @@
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "createdAt": datetime,
-        "dataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "dataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
         "status": DataSourceStatusType,
         "updatedAt": datetime,
         "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
@@ -1123,15 +1216,15 @@
         "agentVersion": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "actionGroupExecutor": NotRequired[ActionGroupExecutorTypeDef],
         "apiSchema": NotRequired[APISchemaTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
-        "functionSchema": NotRequired[FunctionSchemaTypeDef],
+        "functionSchema": NotRequired[FunctionSchemaOutputTypeDef],
         "parentActionSignature": NotRequired[Literal["AMAZON.UserInput"]],
     },
 )
 CreateAgentActionGroupRequestRequestTypeDef = TypedDict(
     "CreateAgentActionGroupRequestRequestTypeDef",
     {
         "actionGroupName": str,
@@ -1142,14 +1235,15 @@
         "apiSchema": NotRequired[APISchemaTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
         "functionSchema": NotRequired[FunctionSchemaTypeDef],
         "parentActionGroupSignature": NotRequired[Literal["AMAZON.UserInput"]],
     },
 )
+FunctionSchemaUnionTypeDef = Union[FunctionSchemaTypeDef, FunctionSchemaOutputTypeDef]
 UpdateAgentActionGroupRequestRequestTypeDef = TypedDict(
     "UpdateAgentActionGroupRequestRequestTypeDef",
     {
         "actionGroupId": str,
         "actionGroupName": str,
         "agentId": str,
         "agentVersion": str,
@@ -1176,15 +1270,15 @@
         "clientToken": NotRequired[str],
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "failureReasons": NotRequired[List[str]],
         "foundationModel": NotRequired[str],
         "instruction": NotRequired[str],
         "preparedAt": NotRequired[datetime],
-        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
+        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationOutputTypeDef],
         "recommendedActions": NotRequired[List[str]],
     },
 )
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "agentArn": str,
@@ -1197,15 +1291,15 @@
         "updatedAt": datetime,
         "version": str,
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "failureReasons": NotRequired[List[str]],
         "foundationModel": NotRequired[str],
         "instruction": NotRequired[str],
-        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
+        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationOutputTypeDef],
         "recommendedActions": NotRequired[List[str]],
     },
 )
 CreateAgentRequestRequestTypeDef = TypedDict(
     "CreateAgentRequestRequestTypeDef",
     {
         "agentName": str,
@@ -1216,14 +1310,17 @@
         "foundationModel": NotRequired[str],
         "idleSessionTTLInSeconds": NotRequired[int],
         "instruction": NotRequired[str],
         "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
+PromptOverrideConfigurationUnionTypeDef = Union[
+    PromptOverrideConfigurationTypeDef, PromptOverrideConfigurationOutputTypeDef
+]
 UpdateAgentRequestRequestTypeDef = TypedDict(
     "UpdateAgentRequestRequestTypeDef",
     {
         "agentId": str,
         "agentName": str,
         "agentResourceRoleArn": str,
         "foundationModel": str,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.pyi` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: S3IdentifierTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionGroupStateType,
     AgentAliasStatusType,
     AgentStatusType,
     ChunkingStrategyType,
     CreationModeType,
@@ -57,14 +57,15 @@
     "AgentKnowledgeBaseTypeDef",
     "AgentSummaryTypeDef",
     "AgentVersionSummaryTypeDef",
     "AssociateAgentKnowledgeBaseRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "FixedSizeChunkingConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
+    "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "DataSourceSummaryTypeDef",
     "DeleteAgentActionGroupRequestRequestTypeDef",
     "DeleteAgentAliasRequestRequestTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteAgentVersionRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -75,14 +76,15 @@
     "GetAgentAliasRequestRequestTypeDef",
     "GetAgentKnowledgeBaseRequestRequestTypeDef",
     "GetAgentRequestRequestTypeDef",
     "GetAgentVersionRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetIngestionJobRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
+    "InferenceConfigurationOutputTypeDef",
     "InferenceConfigurationTypeDef",
     "IngestionJobFilterTypeDef",
     "IngestionJobSortByTypeDef",
     "IngestionJobStatisticsTypeDef",
     "VectorKnowledgeBaseConfigurationTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "PaginatorConfigTypeDef",
@@ -90,14 +92,15 @@
     "ListAgentAliasesRequestRequestTypeDef",
     "ListAgentKnowledgeBasesRequestRequestTypeDef",
     "ListAgentVersionsRequestRequestTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "MongoDbAtlasFieldMappingTypeDef",
     "OpenSearchServerlessFieldMappingTypeDef",
     "PineconeFieldMappingTypeDef",
     "PrepareAgentRequestRequestTypeDef",
     "RdsFieldMappingTypeDef",
     "RedisEnterpriseCloudFieldMappingTypeDef",
     "StartIngestionJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -119,56 +122,65 @@
     "ListAgentKnowledgeBasesResponseTypeDef",
     "ListAgentVersionsResponseTypeDef",
     "ListAgentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PrepareAgentResponseTypeDef",
     "UpdateAgentKnowledgeBaseResponseTypeDef",
     "ChunkingConfigurationTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "FunctionOutputTypeDef",
     "FunctionTypeDef",
+    "PromptConfigurationOutputTypeDef",
     "PromptConfigurationTypeDef",
     "ListIngestionJobsRequestRequestTypeDef",
     "IngestionJobSummaryTypeDef",
     "IngestionJobTypeDef",
     "KnowledgeBaseConfigurationTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef",
     "ListAgentAliasesRequestListAgentAliasesPaginateTypeDef",
     "ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef",
     "ListAgentVersionsRequestListAgentVersionsPaginateTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListIngestionJobsRequestListIngestionJobsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "MongoDbAtlasConfigurationTypeDef",
     "OpenSearchServerlessConfigurationTypeDef",
     "PineconeConfigurationTypeDef",
     "RdsConfigurationTypeDef",
     "RedisEnterpriseCloudConfigurationTypeDef",
     "AgentAliasTypeDef",
     "ListAgentAliasesResponseTypeDef",
     "VectorIngestionConfigurationTypeDef",
+    "DataSourceConfigurationUnionTypeDef",
+    "FunctionSchemaOutputTypeDef",
     "FunctionSchemaTypeDef",
+    "PromptOverrideConfigurationOutputTypeDef",
     "PromptOverrideConfigurationTypeDef",
     "ListIngestionJobsResponseTypeDef",
     "GetIngestionJobResponseTypeDef",
     "StartIngestionJobResponseTypeDef",
     "StorageConfigurationTypeDef",
     "CreateAgentAliasResponseTypeDef",
     "GetAgentAliasResponseTypeDef",
     "UpdateAgentAliasResponseTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "DataSourceTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "AgentActionGroupTypeDef",
     "CreateAgentActionGroupRequestRequestTypeDef",
+    "FunctionSchemaUnionTypeDef",
     "UpdateAgentActionGroupRequestRequestTypeDef",
     "AgentTypeDef",
     "AgentVersionTypeDef",
     "CreateAgentRequestRequestTypeDef",
+    "PromptOverrideConfigurationUnionTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseTypeDef",
     "UpdateKnowledgeBaseRequestRequestTypeDef",
     "CreateDataSourceResponseTypeDef",
     "GetDataSourceResponseTypeDef",
     "UpdateDataSourceResponseTypeDef",
@@ -286,14 +298,22 @@
 )
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyArn": NotRequired[str],
     },
 )
+S3DataSourceConfigurationOutputTypeDef = TypedDict(
+    "S3DataSourceConfigurationOutputTypeDef",
+    {
+        "bucketArn": str,
+        "bucketOwnerAccountId": NotRequired[str],
+        "inclusionPrefixes": NotRequired[List[str]],
+    },
+)
 S3DataSourceConfigurationTypeDef = TypedDict(
     "S3DataSourceConfigurationTypeDef",
     {
         "bucketArn": str,
         "bucketOwnerAccountId": NotRequired[str],
         "inclusionPrefixes": NotRequired[Sequence[str]],
     },
@@ -422,14 +442,24 @@
 )
 GetKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "GetKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
+InferenceConfigurationOutputTypeDef = TypedDict(
+    "InferenceConfigurationOutputTypeDef",
+    {
+        "maximumLength": NotRequired[int],
+        "stopSequences": NotRequired[List[str]],
+        "temperature": NotRequired[float],
+        "topK": NotRequired[int],
+        "topP": NotRequired[float],
+    },
+)
 InferenceConfigurationTypeDef = TypedDict(
     "InferenceConfigurationTypeDef",
     {
         "maximumLength": NotRequired[int],
         "stopSequences": NotRequired[Sequence[str]],
         "temperature": NotRequired[float],
         "topK": NotRequired[int],
@@ -545,14 +575,22 @@
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+MongoDbAtlasFieldMappingTypeDef = TypedDict(
+    "MongoDbAtlasFieldMappingTypeDef",
+    {
+        "metadataField": str,
+        "textField": str,
+        "vectorField": str,
+    },
+)
 OpenSearchServerlessFieldMappingTypeDef = TypedDict(
     "OpenSearchServerlessFieldMappingTypeDef",
     {
         "metadataField": str,
         "textField": str,
         "vectorField": str,
     },
@@ -788,14 +826,21 @@
 ChunkingConfigurationTypeDef = TypedDict(
     "ChunkingConfigurationTypeDef",
     {
         "chunkingStrategy": ChunkingStrategyType,
         "fixedSizeChunkingConfiguration": NotRequired[FixedSizeChunkingConfigurationTypeDef],
     },
 )
+DataSourceConfigurationOutputTypeDef = TypedDict(
+    "DataSourceConfigurationOutputTypeDef",
+    {
+        "type": Literal["S3"],
+        "s3Configuration": NotRequired[S3DataSourceConfigurationOutputTypeDef],
+    },
+)
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "type": Literal["S3"],
         "s3Configuration": NotRequired[S3DataSourceConfigurationTypeDef],
     },
 )
@@ -803,22 +848,41 @@
     "ListDataSourcesResponseTypeDef",
     {
         "dataSourceSummaries": List[DataSourceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FunctionOutputTypeDef = TypedDict(
+    "FunctionOutputTypeDef",
+    {
+        "name": str,
+        "description": NotRequired[str],
+        "parameters": NotRequired[Dict[str, ParameterDetailTypeDef]],
+    },
+)
 FunctionTypeDef = TypedDict(
     "FunctionTypeDef",
     {
         "name": str,
         "description": NotRequired[str],
         "parameters": NotRequired[Mapping[str, ParameterDetailTypeDef]],
     },
 )
+PromptConfigurationOutputTypeDef = TypedDict(
+    "PromptConfigurationOutputTypeDef",
+    {
+        "basePromptTemplate": NotRequired[str],
+        "inferenceConfiguration": NotRequired[InferenceConfigurationOutputTypeDef],
+        "parserMode": NotRequired[CreationModeType],
+        "promptCreationMode": NotRequired[CreationModeType],
+        "promptState": NotRequired[PromptStateType],
+        "promptType": NotRequired[PromptTypeType],
+    },
+)
 PromptConfigurationTypeDef = TypedDict(
     "PromptConfigurationTypeDef",
     {
         "basePromptTemplate": NotRequired[str],
         "inferenceConfiguration": NotRequired[InferenceConfigurationTypeDef],
         "parserMode": NotRequired[CreationModeType],
         "promptCreationMode": NotRequired[CreationModeType],
@@ -934,14 +998,26 @@
 )
 ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+MongoDbAtlasConfigurationTypeDef = TypedDict(
+    "MongoDbAtlasConfigurationTypeDef",
+    {
+        "collectionName": str,
+        "credentialsSecretArn": str,
+        "databaseName": str,
+        "endpoint": str,
+        "fieldMapping": MongoDbAtlasFieldMappingTypeDef,
+        "vectorIndexName": str,
+        "endpointServiceName": NotRequired[str],
+    },
+)
 OpenSearchServerlessConfigurationTypeDef = TypedDict(
     "OpenSearchServerlessConfigurationTypeDef",
     {
         "collectionArn": str,
         "fieldMapping": OpenSearchServerlessFieldMappingTypeDef,
         "vectorIndexName": str,
     },
@@ -1000,20 +1076,36 @@
 )
 VectorIngestionConfigurationTypeDef = TypedDict(
     "VectorIngestionConfigurationTypeDef",
     {
         "chunkingConfiguration": NotRequired[ChunkingConfigurationTypeDef],
     },
 )
+DataSourceConfigurationUnionTypeDef = Union[
+    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+]
+FunctionSchemaOutputTypeDef = TypedDict(
+    "FunctionSchemaOutputTypeDef",
+    {
+        "functions": NotRequired[List[FunctionOutputTypeDef]],
+    },
+)
 FunctionSchemaTypeDef = TypedDict(
     "FunctionSchemaTypeDef",
     {
         "functions": NotRequired[Sequence[FunctionTypeDef]],
     },
 )
+PromptOverrideConfigurationOutputTypeDef = TypedDict(
+    "PromptOverrideConfigurationOutputTypeDef",
+    {
+        "promptConfigurations": List[PromptConfigurationOutputTypeDef],
+        "overrideLambda": NotRequired[str],
+    },
+)
 PromptOverrideConfigurationTypeDef = TypedDict(
     "PromptOverrideConfigurationTypeDef",
     {
         "promptConfigurations": Sequence[PromptConfigurationTypeDef],
         "overrideLambda": NotRequired[str],
     },
 )
@@ -1039,14 +1131,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "type": KnowledgeBaseStorageTypeType,
+        "mongoDbAtlasConfiguration": NotRequired[MongoDbAtlasConfigurationTypeDef],
         "opensearchServerlessConfiguration": NotRequired[OpenSearchServerlessConfigurationTypeDef],
         "pineconeConfiguration": NotRequired[PineconeConfigurationTypeDef],
         "rdsConfiguration": NotRequired[RdsConfigurationTypeDef],
         "redisEnterpriseCloudConfiguration": NotRequired[RedisEnterpriseCloudConfigurationTypeDef],
     },
 )
 CreateAgentAliasResponseTypeDef = TypedDict(
@@ -1083,15 +1176,15 @@
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "createdAt": datetime,
-        "dataSourceConfiguration": DataSourceConfigurationTypeDef,
+        "dataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
         "status": DataSourceStatusType,
         "updatedAt": datetime,
         "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
@@ -1123,15 +1216,15 @@
         "agentVersion": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "actionGroupExecutor": NotRequired[ActionGroupExecutorTypeDef],
         "apiSchema": NotRequired[APISchemaTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
-        "functionSchema": NotRequired[FunctionSchemaTypeDef],
+        "functionSchema": NotRequired[FunctionSchemaOutputTypeDef],
         "parentActionSignature": NotRequired[Literal["AMAZON.UserInput"]],
     },
 )
 CreateAgentActionGroupRequestRequestTypeDef = TypedDict(
     "CreateAgentActionGroupRequestRequestTypeDef",
     {
         "actionGroupName": str,
@@ -1142,14 +1235,15 @@
         "apiSchema": NotRequired[APISchemaTypeDef],
         "clientToken": NotRequired[str],
         "description": NotRequired[str],
         "functionSchema": NotRequired[FunctionSchemaTypeDef],
         "parentActionGroupSignature": NotRequired[Literal["AMAZON.UserInput"]],
     },
 )
+FunctionSchemaUnionTypeDef = Union[FunctionSchemaTypeDef, FunctionSchemaOutputTypeDef]
 UpdateAgentActionGroupRequestRequestTypeDef = TypedDict(
     "UpdateAgentActionGroupRequestRequestTypeDef",
     {
         "actionGroupId": str,
         "actionGroupName": str,
         "agentId": str,
         "agentVersion": str,
@@ -1176,15 +1270,15 @@
         "clientToken": NotRequired[str],
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "failureReasons": NotRequired[List[str]],
         "foundationModel": NotRequired[str],
         "instruction": NotRequired[str],
         "preparedAt": NotRequired[datetime],
-        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
+        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationOutputTypeDef],
         "recommendedActions": NotRequired[List[str]],
     },
 )
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "agentArn": str,
@@ -1197,15 +1291,15 @@
         "updatedAt": datetime,
         "version": str,
         "customerEncryptionKeyArn": NotRequired[str],
         "description": NotRequired[str],
         "failureReasons": NotRequired[List[str]],
         "foundationModel": NotRequired[str],
         "instruction": NotRequired[str],
-        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
+        "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationOutputTypeDef],
         "recommendedActions": NotRequired[List[str]],
     },
 )
 CreateAgentRequestRequestTypeDef = TypedDict(
     "CreateAgentRequestRequestTypeDef",
     {
         "agentName": str,
@@ -1216,14 +1310,17 @@
         "foundationModel": NotRequired[str],
         "idleSessionTTLInSeconds": NotRequired[int],
         "instruction": NotRequired[str],
         "promptOverrideConfiguration": NotRequired[PromptOverrideConfigurationTypeDef],
         "tags": NotRequired[Mapping[str, str]],
     },
 )
+PromptOverrideConfigurationUnionTypeDef = Union[
+    PromptOverrideConfigurationTypeDef, PromptOverrideConfigurationOutputTypeDef
+]
 UpdateAgentRequestRequestTypeDef = TypedDict(
     "UpdateAgentRequestRequestTypeDef",
     {
         "agentId": str,
         "agentName": str,
         "agentResourceRoleArn": str,
         "foundationModel": str,
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.90
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
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
 [mypy-boto3-bedrock-agent docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_agent-1.34.96/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.90/setup.py` & `mypy_boto3_bedrock_agent-1.34.96/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-agent",
-    version="1.34.90",
+    version="1.34.96",
     packages=["mypy_boto3_bedrock_agent"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.AgentsforBedrock 1.34.96 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

