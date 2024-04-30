# Comparing `tmp/datasurface-0.0.6.tar.gz` & `tmp/datasurface-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasurface-0.0.6.tar", last modified: Sat Feb 24 12:35:07 2024, max compression
+gzip compressed data, was "datasurface-0.0.9.tar", last modified: Thu Feb 29 02:32:14 2024, max compression
```

## Comparing `datasurface-0.0.6.tar` & `datasurface-0.0.9.tar`

### file list

```diff
@@ -1,107 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.013333 datasurface-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-24 12:34:59.000000 datasurface-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-24 12:34:59.000000 datasurface-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-02-24 12:35:07.013333 datasurface-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-24 12:34:59.000000 datasurface-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:06.997333 datasurface-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/DataClassification.md
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/DataContainers.md
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/DataPlatform.md
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/DataTransformer.md
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Datastores.md
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Ecosystem.md
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/GettingStarted.md
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Glossary.md
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/GovernanceZone.md
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/HowGitHubIsUsed.md
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/PullRequests.md
--rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Teams.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-24 12:34:59.000000 datasurface-0.0.6/docs/Workspaces.md
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-24 12:34:59.000000 datasurface-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 12:35:07.013333 datasurface-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-24 12:34:59.000000 datasurface-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:06.993333 datasurface-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:06.997333 datasurface-0.0.6/src/datasurface/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.001333 datasurface-0.0.6/src/datasurface/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/codegen/CodeGen.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.001333 datasurface-0.0.6/src/datasurface/codegen/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/codegen/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/codegen/templates/datastore.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.001333 datasurface-0.0.6/src/datasurface/handler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/handler/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/handler/check-files-changed.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/handler/pull-request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.005334 datasurface-0.0.6/src/datasurface/md/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/AmazonAWS.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/AvroSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/GitOps.py
--rw-r--r--   0 runner    (1001) docker     (127)   109534 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Governance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/PipelineGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/RenderDataPlatform.py
--rw-r--r--   0 runner    (1001) docker     (127)    36977 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/SqlAlchemyUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.005334 datasurface-0.0.6/src/datasurface/md/azureTemplates/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/azureTemplates/AzureBatch.bicep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/azureTemplates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/datasurface/md/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/datasurface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-02-24 12:35:06.000000 datasurface-0.0.6/src/datasurface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-02-24 12:35:06.000000 datasurface-0.0.6/src/datasurface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 12:35:06.000000 datasurface-0.0.6/src/datasurface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-24 12:35:06.000000 datasurface-0.0.6/src/datasurface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-24 12:35:06.000000 datasurface-0.0.6/src/datasurface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:06.993333 datasurface-0.0.6/src/tests/actionHandlerResources/step1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step1/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step1/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step1/base/eco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:06.993333 datasurface-0.0.6/src/tests/actionHandlerResources/step2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_EU/
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_EU/eco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_USA/
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_USA/eco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step3/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step3/defineEU_GZ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step3/eco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/actionHandlerResources/step4/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step4/defineEU_GZ.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step4/defineUSA_GZ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/actionHandlerResources/step4/eco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 12:35:07.009333 datasurface-0.0.6/src/tests/nwdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/nwdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/nwdb/eco.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/nwdb/nwdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_ActionHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_GitOps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_PlatformGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_SchemaCompatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_SimpleZone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_StoragePolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_TypeToPython.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_Workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_authorized_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_cyclic_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-02-24 12:34:59.000000 datasurface-0.0.6/src/tests/test_nwdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.806239 datasurface-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 02:32:02.000000 datasurface-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-29 02:32:02.000000 datasurface-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-02-29 02:32:14.806239 datasurface-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-02-29 02:32:02.000000 datasurface-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.782239 datasurface-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/DataClassification.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/DataContainers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/DataPlatform.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/DataTransformer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Datastores.md
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Ecosystem.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/GettingStarted.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Glossary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/GovernanceZone.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/HowGitHubIsUsed.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/PullRequests.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Teams.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-29 02:32:02.000000 datasurface-0.0.9/docs/Workspaces.md
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-29 02:32:02.000000 datasurface-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 02:32:14.806239 datasurface-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-29 02:32:02.000000 datasurface-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.778239 datasurface-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.782239 datasurface-0.0.9/src/datasurface/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/codegen/CodeGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/codegen/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/codegen/__pycache__/CodeGen.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/codegen/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/codegen/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/codegen/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/codegen/templates/datastore.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/datasurface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/datasurface/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/codegen/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.786239 datasurface-0.0.9/src/datasurface/datasurface/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/handler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/handler/action.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.790239 datasurface-0.0.9/src/datasurface/datasurface/md/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/AmazonAWS.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/AvroSchema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Documentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/GitOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Governance.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/IaCPlatform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Lint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/PipelineGraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/Schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/SqlAlchemyUtils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.790239 datasurface-0.0.9/src/datasurface/datasurface/md/azureTemplates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/azureTemplates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-29 02:32:08.000000 datasurface-0.0.9/src/datasurface/datasurface/md/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.790239 datasurface-0.0.9/src/datasurface/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.790239 datasurface-0.0.9/src/datasurface/handler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/handler/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/handler/__pycache__/action.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/handler/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/handler/check-files-changed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/handler/pull-request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.794239 datasurface-0.0.9/src/datasurface/md/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/AmazonAWS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/AvroSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.794239 datasurface-0.0.9/src/datasurface/md/DataContainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/DataContainers/Databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/DataContainers/Snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/GitOps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115055 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Governance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/IaCPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/PipelineGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36977 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/SqlAlchemyUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.798239 datasurface-0.0.9/src/datasurface/md/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/AmazonAWS.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/AvroSchema.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Azure.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Documentation.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Exceptions.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    13871 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/GitOps.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)   166612 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Governance.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/IaCPlatform.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Lint.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    22862 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/PipelineGraph.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Policy.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    59471 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/Schema.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/SqlAlchemyUtils.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/__pycache__/utils.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.798239 datasurface-0.0.9/src/datasurface/md/azureTemplates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/azureTemplates/AzureBatch.bicep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/azureTemplates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.798239 datasurface-0.0.9/src/datasurface/md/azureTemplates/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-29 02:32:07.000000 datasurface-0.0.9/src/datasurface/md/azureTemplates/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/md/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.778239 datasurface-0.0.9/src/datasurface/platforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.778239 datasurface-0.0.9/src/datasurface/platforms/estuary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.798239 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/__init__py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/captureMulti.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/captureSingle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/materialize.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/datasurface/platforms/estuary/templates/materielize_sql_dbms.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.806239 datasurface-0.0.9/src/datasurface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-02-29 02:32:14.000000 datasurface-0.0.9/src/datasurface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-02-29 02:32:14.000000 datasurface-0.0.9/src/datasurface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:32:14.000000 datasurface-0.0.9/src/datasurface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-29 02:32:14.000000 datasurface-0.0.9/src/datasurface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-29 02:32:14.000000 datasurface-0.0.9/src/datasurface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.778239 datasurface-0.0.9/src/tests/actionHandlerResources/step1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step1/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step1/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step1/base/eco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.778239 datasurface-0.0.9/src/tests/actionHandlerResources/step2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_EU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_EU/eco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_USA/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_USA/eco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step3/defineEU_GZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step3/eco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/actionHandlerResources/step4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step4/defineEU_GZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step4/defineUSA_GZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/actionHandlerResources/step4/eco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:14.802239 datasurface-0.0.9/src/tests/nwdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/nwdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/nwdb/eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/nwdb/nwdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_ActionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_GitOps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_PlatformGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_SchemaCompatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_SimpleZone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_StoragePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_TypeToPython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24078 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_Workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_authorized_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_cyclic_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-02-29 02:32:02.000000 datasurface-0.0.9/src/tests/test_nwdb.py
```

### Comparing `datasurface-0.0.6/LICENSE.txt` & `datasurface-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/DataClassification.md` & `datasurface-0.0.9/docs/DataClassification.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/DataContainers.md` & `datasurface-0.0.9/docs/DataContainers.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/DataPlatform.md` & `datasurface-0.0.9/docs/DataPlatform.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/DataTransformer.md` & `datasurface-0.0.9/docs/DataTransformer.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Datastores.md` & `datasurface-0.0.9/docs/Datastores.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Documentation.md` & `datasurface-0.0.9/docs/Documentation.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Ecosystem.md` & `datasurface-0.0.9/docs/Ecosystem.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/GettingStarted.md` & `datasurface-0.0.9/docs/GettingStarted.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Glossary.md` & `datasurface-0.0.9/docs/Glossary.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/GovernanceZone.md` & `datasurface-0.0.9/docs/GovernanceZone.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/HowGitHubIsUsed.md` & `datasurface-0.0.9/docs/HowGitHubIsUsed.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/PullRequests.md` & `datasurface-0.0.9/docs/PullRequests.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/README.md` & `datasurface-0.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Teams.md` & `datasurface-0.0.9/docs/Teams.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/docs/Workspaces.md` & `datasurface-0.0.9/docs/Workspaces.md`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/setup.py` & `datasurface-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='datasurface',
-    version='0.0.6',
+    version='0.0.9',
     license='Apache License 2.0',
     description='Automate the governance, management and movement of data within your enterprise',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Billy Newport',
     author_email='billy@billynewport.com',
     url='https://github.com/billynewport/datasurface',
@@ -24,9 +24,10 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3.11',
         'Topic :: Database :: Database Engines/Servers',
     ],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
+    package_data={"": ["*.pyi", "py.typed"]},  # Include .pyi files and py.typed file
     install_requires=requirements
 )
```

### Comparing `datasurface-0.0.6/src/datasurface/.DS_Store` & `datasurface-0.0.9/src/datasurface/.DS_Store`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/codegen/CodeGen.py` & `datasurface-0.0.9/src/datasurface/codegen/CodeGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datasurface.md import DDLTable
 from datasurface.md.Schema import DDLColumn, DEFAULT_nullable, DEFAULT_primaryKey
 
 
 def getDatasets(store: Datastore) -> list[Any]:
     datasets: list[Any] = []
     for dataset in store.datasets.values():
-        if(dataset):
+        if (dataset):
             datasets.append(dataset)
     return datasets
 
 
 def getColumns(dataset: Dataset) -> list[DDLColumn]:
     columns: list[DDLColumn] = []
     if (dataset.originalSchema and isinstance(dataset.originalSchema, DDLTable)):
@@ -25,15 +25,15 @@
     return columns
 
 
 def convertColumnAttributesToString(column: DDLColumn) -> str:
     rc: str = ""
     if (column.nullable != DEFAULT_nullable):
         rc += f", {column.nullable}"
-    if (column.classification != None):
+    if (column.classification is not None):
         rc += f", {column.classification}"
     if (column.primaryKey != DEFAULT_primaryKey):
         rc += f", {column.primaryKey}"
     return rc
 
 
 def generate_code(store: Datastore) -> str:
```

### Comparing `datasurface-0.0.6/src/datasurface/codegen/templates/datastore.jinja2` & `datasurface-0.0.9/src/datasurface/codegen/templates/datastore.jinja2`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/handler/action.py` & `datasurface-0.0.9/src/datasurface/handler/action.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/handler/check-files-changed.yml` & `datasurface-0.0.9/src/datasurface/handler/check-files-changed.yml`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/handler/pull-request.yml` & `datasurface-0.0.9/src/datasurface/handler/pull-request.yml`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/.DS_Store` & `datasurface-0.0.9/src/datasurface/md/.DS_Store`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/AmazonAWS.py` & `datasurface-0.0.9/src/datasurface/md/AmazonAWS.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-
-
 from typing import Optional
 from datasurface.md import Documentation
-from datasurface.md.Governance import DataContainer, DataPlatform, Ecosystem, InfrastructureLocation, \
+from datasurface.md.Governance import CloudVendor, DataContainer, DataPlatform, Ecosystem, InfrastructureLocation, \
     InfrastructureVendor, ObjectStorage
 from datasurface.md.Lint import ValidationTree
 
 
 class AmazonAWSDataPlatform(DataPlatform):
     def __init__(self, name: str, doc: Documentation):
         super().__init__(name, doc)
@@ -22,17 +20,24 @@
 
     def _str__(self) -> str:
         return f"AmazonAWSDataPlatform({self.name})"
 
     def __eq__(self, __value: object) -> bool:
         return super().__eq__(__value) and isinstance(__value, AmazonAWSDataPlatform)
 
+    def isContainerSupported(self, eco: Ecosystem, dc: DataContainer) -> bool:
+        return dc.isUsingVendorsOnly(eco, {CloudVendor.AWS})
+
     def lint(self, eco: Ecosystem, tree: ValidationTree):
         pass
 
+    def getInternalDataContainers(self) -> set[DataContainer]:
+        # TODO: Implement this method
+        return set()
+
 
 class AmazonAWSS3Bucket(ObjectStorage):
     def __init__(self, name: str, loc: InfrastructureLocation, endPointURI: Optional[str], bucketName: str, prefix: Optional[str]):
         super().__init__(name, loc, endPointURI, bucketName, prefix)
 
     def __eq__(self, o: object) -> bool:
         return super().__eq__(o) and isinstance(o, AmazonAWSS3Bucket)
```

### Comparing `datasurface-0.0.6/src/datasurface/md/AvroSchema.py` & `datasurface-0.0.9/src/datasurface/md/AvroSchema.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/Azure.py` & `datasurface-0.0.9/src/datasurface/md/Azure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+from enum import Enum
 from datasurface.md import Documentation
-from datasurface.md.Governance import InfrastructureVendor
-from .Governance import Credential, DataPlatform, EncryptionSystem, Ecosystem, GovernanceZone, InfrastructureLocation, SQLDatabase, Team
+from datasurface.md.Governance import DataContainer, InfrastructureVendor
+from .Governance import CloudVendor, Credential, DataPlatform, EncryptionSystem, Ecosystem, GovernanceZone, HostPortSQLDatabase, InfrastructureLocation, Team
 from .Lint import ValidationTree
 from .utils import is_valid_azure_key_vault_name
 
 
+class AzureVaultObjectType(Enum):
+    HSM_KEYS = 1
+    SOFTWARE_KEYS = 2
+    SECRETS = 3
+    CERTIFICATES = 4
+    STORAGE_ACCOUNT_KEYS = 5
+
+
 class AzureKeyVaultCredential(Credential):
     """This allows a secret to be read from Azure Key Vault. The secret should be in the
     form of 2 lines, first line is user name, second line is password"""
     def __init__(self, keyVaultName: str, objectName: str) -> None:
         super().__init__()
         self.keyVaultName: str = keyVaultName
         self.objectName: str = objectName
-        self.objectType: str = "secrets"
+        self.objectType: AzureVaultObjectType = AzureVaultObjectType.SECRETS
 
     def __eq__(self, __value: object) -> bool:
         return super().__eq__(__value) and type(__value) is AzureKeyVaultCredential and self.keyVaultName == __value.keyVaultName and \
             self.objectName == __value.objectName
 
     def lint(self, eco: 'Ecosystem', tree: ValidationTree) -> None:
         super().lint(eco, tree)
@@ -55,24 +64,31 @@
 
     def __eq__(self, __value: object) -> bool:
         return super().__eq__(__value) and isinstance(__value, AzureDataplatform)
 
     def _str__(self) -> str:
         return f"AzureDataPlatform({self.name})"
 
+    def isContainerSupported(self, eco: Ecosystem, dc: DataContainer) -> bool:
+        return dc.isUsingVendorsOnly(eco, {CloudVendor.AZURE})
+
+    def getInternalDataContainers(self) -> set[DataContainer]:
+        # TODO: Implement this method
+        return set()
+
 
 class AzureBatchDataPlatform(AzureDataplatform):
     def __init__(self, name: str, doc: Documentation, platformCredential: AzureKeyVaultCredential):
         super().__init__(name, doc, platformCredential)
 
 
-class AzureSQLDatabase(SQLDatabase):
+class AzureSQLDatabase(HostPortSQLDatabase):
     """This is an Azure SQL Database resource. """
-    def __init__(self, name: str, hostNameAndPort: str, databaseName: str, loc: InfrastructureLocation):
-        super().__init__(name, loc, hostNameAndPort, databaseName)
+    def __init__(self, name: str, hostName: str, port: int, databaseName: str, loc: InfrastructureLocation):
+        super().__init__(name, loc, hostName, port, databaseName)
 
     def __str__(self) -> str:
         return f"AzureDatabaseResource({self.name})"
 
     def __hash__(self) -> int:
         return hash(self.name)
```

### Comparing `datasurface-0.0.6/src/datasurface/md/Documentation.py` & `datasurface-0.0.9/src/datasurface/md/Documentation.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/Exceptions.py` & `datasurface-0.0.9/src/datasurface/md/Exceptions.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/GitOps.py` & `datasurface-0.0.9/src/datasurface/md/GitOps.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/Governance.py` & `datasurface-0.0.9/src/datasurface/md/Governance.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,51 +370,77 @@
                     return loc
                 else:
                     return loc.findLocationUsingKey(locationPath[1:])
             else:
                 return None
 
 
+class CloudVendor(Enum):
+    """Cloud vendor. This is used with InfrastructureVendor types to associate them with a hard cloud vendor"""
+    AWS = 0
+    """Amazon Web Services"""
+    AZURE = 1
+    """Microsoft Azure"""
+    GCP = 2
+    """Google Cloud Platform"""
+    IBM = 3
+    """IBM Cloud"""
+    ORACLE = 4
+    """Oracle Cloud"""
+    ALIBABA = 5
+    """Alibaba Cloud"""
+    AWS_CHINA = 6
+    """AWS China"""
+    TEN_CENT = 7
+    HUAWEI = 8
+    AZURE_CHINA = 9  # 21Vianet
+
+
 class InfrastructureVendor(Documentable):
     """This is a vendor which supplies infrastructure for storage and compute. It could be an internal supplier within an
     enterprise or an external cloud provider"""
-    def __init__(self, name: str, *args: Union[InfrastructureLocation, Documentation]) -> None:
+    def __init__(self, name: str, *args: Union[InfrastructureLocation, Documentation, CloudVendor]) -> None:
         super().__init__(None)
         self.name: str = name
         self.key: Optional[InfrastructureVendorKey] = None
         self.locations: dict[str, 'InfrastructureLocation'] = OrderedDict()
+        self.hardCloudVendor: Optional[CloudVendor] = None
+
         self.add(*args)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def setEcosystem(self, eco: 'Ecosystem') -> None:
         self.key = InfrastructureVendorKey(eco.key, self.name)
 
         self.add()
 
-    def add(self, *args: Union['InfrastructureLocation', Documentation]) -> None:
+    def add(self, *args: Union['InfrastructureLocation', Documentation, CloudVendor]) -> None:
         for loc in args:
             if (isinstance(loc, InfrastructureLocation)):
                 self.addLocation(loc)
+            elif (isinstance(loc, CloudVendor)):
+                self.hardCloudVendor = loc
             else:
                 self.documentation = loc
         if (self.key):
             topLocationKey: InfraLocationKey = InfraLocationKey(self.key, [])
             for loc in self.locations.values():
                 loc.setParentLocation(topLocationKey)
 
     def addLocation(self, loc: 'InfrastructureLocation'):
         if self.locations.get(loc.name) is not None:
             raise Exception(f"Duplicate Location {loc.name}")
         self.locations[loc.name] = loc
 
     def __eq__(self, __value: object) -> bool:
         if super().__eq__(__value) and isinstance(__value, InfrastructureVendor):
-            return self.name == __value.name and self.key == __value.key and self.locations == __value.locations
+            return self.name == __value.name and self.key == __value.key and self.locations == __value.locations and \
+                self.hardCloudVendor == __value.hardCloudVendor
         else:
             return False
 
     def getLocationOrThrow(self, locationName: str) -> 'InfrastructureLocation':
         """Returns the location with the specified name or throws an exception"""
         loc: Optional[InfrastructureLocation] = self.locations.get(locationName)
         if (loc):
@@ -451,15 +477,15 @@
             self.documentation.lint(tree)
 
         for loc in self.locations.values():
             lTree: ValidationTree = tree.createChild(loc)
             loc.lint(lTree)
 
     def __str__(self) -> str:
-        return f"InfrastructureVendor({self.name})"
+        return f"InfrastructureVendor({self.name}, {self.hardCloudVendor})"
 
 
 class InfraStructureVendorPolicy(AllowDisallowPolicy[InfrastructureVendor]):
     """Allows a GZ to police which vendors can be used with datastore or workspaces within itself"""
     def __init__(self, name: str, doc: Documentation, allowed: Optional[set[InfrastructureVendor]] = None,
                  notAllowed: Optional[set[InfrastructureVendor]] = None):
         super().__init__(name, doc, allowed, notAllowed)
@@ -470,14 +496,30 @@
     def __eq__(self, v: object) -> bool:
         return super().__eq__(v) and isinstance(v, InfraStructureVendorPolicy) and self.allowed == v.allowed and self.notAllowed == v.notAllowed
 
     def __hash__(self) -> int:
         return super().__hash__()
 
 
+class InfraHardVendorPolicy(AllowDisallowPolicy[CloudVendor]):
+    """Allows a GZ to police which vendors can be used with datastore or workspaces within itself"""
+    def __init__(self, name: str, doc: Documentation, allowed: Optional[set[CloudVendor]] = None,
+                 notAllowed: Optional[set[CloudVendor]] = None):
+        super().__init__(name, doc, allowed, notAllowed)
+
+    def __str__(self):
+        return f"InfraStructureVendorPolicy({self.name})"
+
+    def __eq__(self, v: object) -> bool:
+        return super().__eq__(v) and isinstance(v, InfraStructureVendorPolicy) and self.allowed == v.allowed and self.notAllowed == v.notAllowed
+
+    def __hash__(self) -> int:
+        return super().__hash__()
+
+
 class InfraStructureLocationPolicy(AllowDisallowPolicy[InfrastructureLocation]):
     """Allows a GZ to police which locations can be used with datastores or workspaces within itself"""
     def __init__(self, name: str, doc: Documentation, allowed: Optional[set[InfrastructureLocation]] = None,
                  notAllowed: Optional[set[InfrastructureLocation]] = None):
         super().__init__(name, doc, allowed, notAllowed)
 
     def __str__(self):
@@ -520,36 +562,40 @@
         """Are keys stored on site or at a third party?"""
         self.hasThirdPartySuperUser: bool = False
 
     def __eq__(self, __value: object) -> bool:
         return cyclic_safe_eq(self, __value, set())
 
 
-class DataContainer(ABC):
+class DataContainer(ABC, Documentable):
     """This is a container for data. It's a logical container. The data can be physically stored in
     one or more locations through replication or fault tolerance measures. It is owned by a data platform
     and is used to determine whether a dataset is compatible with the container by a governancezone."""
-    def __init__(self, name: str, *args: InfrastructureLocation) -> None:
-        super().__init__()
+    def __init__(self, name: str, *args: Union[InfrastructureLocation, Documentation]) -> None:
+        ABC.__init__(self)
+        Documentable.__init__(self, None)
         self.locations: set[InfrastructureLocation] = set()
         self.name: str = name
         self.serverSideEncryptionKeys: Optional[EncryptionSystem] = None
         """This is the vendor ecnryption system providing the container. For example, if a cloud vendor
         hosts the container, do they have access to the container data?"""
         self.clientSideEncryptionKeys: Optional[EncryptionSystem] = None
         """This is the encryption system used by the client to encrypt data before sending to the container. This could be used
         to encrypt data before sending to a cloud vendor for example"""
         self.isReadOnly: bool = False
         self.add(*args)
 
-    def add(self, *args: InfrastructureLocation) -> None:
-        for loc in args:
-            if (loc in self.locations):
-                raise Exception(f"Duplicate Location {loc}")
-            self.locations.add(loc)
+    def add(self, *args: Union[InfrastructureLocation, Documentation]) -> None:
+        for arg in args:
+            if (isinstance(arg, InfrastructureLocation)):
+                if (arg in self.locations):
+                    raise Exception(f"Duplicate Location {arg}")
+                self.locations.add(arg)
+            else:
+                self.documentation = arg
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, DataContainer):
             return self.name == __value.name and self.locations == __value.locations and \
                 self.serverSideEncryptionKeys == __value.serverSideEncryptionKeys and \
                 self.clientSideEncryptionKeys == __value.clientSideEncryptionKeys and \
                 self.isReadOnly == __value.isReadOnly
@@ -566,32 +612,79 @@
     @abstractmethod
     def lint(self, eco: 'Ecosystem', gz: 'GovernanceZone', t: 'Team', tree: ValidationTree) -> None:
         """This checks if the source is valid for the specified ecosystem, governance zone and team"""
         # Verify that the location on the data container doesn't violate
         # the governance zone policies for vendor or location
         for loc in self.locations:
             gz.checkLocationIsAllowed(eco, loc, tree)
+        if (self.documentation):
+            dTree: ValidationTree = tree.createChild(self.documentation)
+            self.documentation.lint(dTree)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
+    def isUsingVendorsOnly(self, eco: 'Ecosystem', vendors: set[CloudVendor]) -> bool:
+        """Returns true if the container only uses locations managed by the provided set of cloud vendors"""
+        for loc in self.locations:
+            if (loc.key is None):
+                return False
+            v: InfrastructureVendor = eco.getVendorOrThrow(loc.key.ivName)
+            if v.hardCloudVendor != CloudVendor.AWS:
+                return False
+        return True
+
 
 class SQLDatabase(DataContainer):
     """A generic SQL Database data container"""
-    def __init__(self, name: str, location: InfrastructureLocation, hostAndPort: str, databaseName: str) -> None:
+    def __init__(self, name: str, location: InfrastructureLocation, databaseName: str) -> None:
         super().__init__(name, location)
-        self.hostAndPort: str = hostAndPort
         self.databaseName: str = databaseName
 
     def __eq__(self, __value: object) -> bool:
         if (isinstance(__value, SQLDatabase)):
-            return super().__eq__(__value) and self.hostAndPort == __value.hostAndPort and self.databaseName == __value.databaseName
+            return super().__eq__(__value) and self.databaseName == __value.databaseName
+        return False
+
+    def lint(self, eco: 'Ecosystem', gz: 'GovernanceZone', t: 'Team', tree: ValidationTree) -> None:
+        super().lint(eco, gz, t, tree)
+
+
+class URLSQLDatabase(SQLDatabase):
+    """This is a SQL database with a URL"""
+    def __init__(self, name: str, location: InfrastructureLocation, url: str, databaseName: str) -> None:
+        super().__init__(name, location, databaseName)
+        self.url: str = url
+
+    def __eq__(self, __value: object) -> bool:
+        if (isinstance(__value, URLSQLDatabase)):
+            return super().__eq__(__value) and self.url == __value.url
         return False
 
 
+class HostPortSQLDatabase(SQLDatabase):
+    """This is a SQL database with a host and port"""
+    def __init__(self, name: str, location: InfrastructureLocation, host: str, port: int, databaseName: str) -> None:
+        super().__init__(name, location, databaseName)
+        self.host: str = host
+        self.port: int = port
+
+    def __eq__(self, __value: object) -> bool:
+        if (isinstance(__value, HostPortSQLDatabase)):
+            return super().__eq__(__value) and self.host == __value.host and self.port == __value.port
+        return False
+
+    def lint(self, eco: 'Ecosystem', gz: 'GovernanceZone', t: 'Team', tree: ValidationTree) -> None:
+        super().lint(eco, gz, t, tree)
+        if not is_valid_hostname_or_ip(self.host):
+            tree.addProblem(f"Host '{self.host}' is not a valid hostname or IP address")
+        if self.port < 0 or self.port > 65535:
+            tree.addProblem(f"Port {self.port} is not a valid port number")
+
+
 class ObjectStorage(DataContainer):
     """Generic Object storage service. Flat file storage"""
     def __init__(self, name: str, loc: InfrastructureLocation, endPointURI: Optional[str], bucketName: str, prefix: Optional[str]):
         super().__init__(name, loc)
         self.endPointURI: Optional[str] = endPointURI
         self.bucketName: str = bucketName
         self.prefix: Optional[str] = prefix
@@ -740,35 +833,50 @@
         if (self.secretFilePath == ""):
             tree.addProblem("Secret file path is empty")
 
     def __str__(self) -> str:
         return f"FileSecretCredential({self.secretFilePath})"
 
 
-class ClearTextCredential(Credential):
-    """This is implemented for testing but should never be used in production. All
-    credentials should be stored and retrieved using secrets Credential objects also
-    provided."""
+class UserPasswordCredential(Credential):
+    """This is a simple user name and password credential"""
     def __init__(self, username: str, password: str) -> None:
         super().__init__()
         self.username: str = username
         self.password: str = password
 
     def __eq__(self, __value: object) -> bool:
-        return super().__eq__(__value) and type(__value) is ClearTextCredential and self.username == __value.username and self.password == __value.password
+        return super().__eq__(__value) and type(__value) is UserPasswordCredential and self.username == __value.username and self.password == __value.password
 
     def lint(self, eco: 'Ecosystem', tree: ValidationTree) -> None:
         """This checks if the source is valid for the specified ecosystem, governance zone and team"""
-        tree.addProblem("ClearText credential found", ProblemSeverity.WARNING)
         if (self.username == ""):
             tree.addProblem("Username is empty")
         if (self.password == ""):
             tree.addProblem("Password is empty")
 
     def __str__(self) -> str:
+        return f"UserPasswordCredential({self.username})"
+
+
+class ClearTextCredential(UserPasswordCredential):
+    """This is implemented for testing but should never be used in production. All
+    credentials should be stored and retrieved using secrets Credential objects also
+    provided."""
+    def __init__(self, username: str, password: str) -> None:
+        super().__init__(username, password)
+
+    def __eq__(self, __value: object) -> bool:
+        return super().__eq__(__value) and type(__value) is ClearTextCredential
+
+    def lint(self, eco: 'Ecosystem', tree: ValidationTree) -> None:
+        super().lint(eco, tree)
+        tree.addProblem("ClearText credential found", ProblemSeverity.WARNING)
+
+    def __str__(self) -> str:
         return f"ClearTextCredential({self.username})"
 
 
 class PyOdbcSourceInfo(DataContainer):
     """This describes how to connect to a database using pyodbc"""
     def __init__(self, name: str, loc: InfrastructureLocation, serverHost: str, databaseName: str, driver: str, connectionStringTemplate: str) -> None:
         if (loc.key is None):
@@ -922,14 +1030,19 @@
 
     @abstractmethod
     def lint(self, eco: 'Ecosystem', gz: 'GovernanceZone', t: 'Team', d: 'Datastore', tree: ValidationTree) -> None:
         """This checks if the source is valid for the specified ecosystem, governance zone and team"""
         if (self.dataContainer):
             capTree: ValidationTree = tree.createChild(self.dataContainer)
             self.dataContainer.lint(eco, gz, t, capTree)
+        # Credential is needed for a platform connect to a datacontainer and ingest data
+        if (self.credential is None):
+            tree.addRaw(AttributeNotSet("credential"))
+        else:
+            self.credential.lint(eco, tree)
         super().lint(eco, gz, t, d, tree)
 
 
 class CDCCaptureIngestion(IngestionMetadata):
     """This indicates CDC can be used to capture deltas from the source"""
     def __init__(self, dc: DataContainer, *args: Union[Credential, StepTrigger, IngestionConsistencyType]) -> None:
         super().__init__(dc, *args)
@@ -1713,27 +1826,28 @@
 
 
 class GovernanceZone(GitControlledObject):
     """This declares the existence of a specific GovernanceZone and defines the teams it manages, the storage policies
     and which repos can be used to pull changes for various metadata"""
     def __init__(self, name: str, ownerRepo: Repository, *args: Union[InfraStructureLocationPolicy, InfraStructureVendorPolicy,
                                                                       StoragePolicy, DataClassificationPolicy, TeamDeclaration,
-                                                                      Documentation, DataPlatformPolicy]) -> None:
+                                                                      Documentation, DataPlatformPolicy, InfraHardVendorPolicy]) -> None:
         super().__init__(ownerRepo)
         self.name: str = name
         self.key: Optional[GovernanceZoneKey] = None
         self.teams: AuthorizedObjectManager[Team, TeamDeclaration] = AuthorizedObjectManager[Team, TeamDeclaration](
             "teams", lambda name, repo: Team(name, repo), ownerRepo)
 
         self.storagePolicies: dict[str, StoragePolicy] = OrderedDict[str, StoragePolicy]()
         # Schemas for datasets defined in this GZ must comply with these classification restrictions
         self.classificationPolicies: dict[str, DataClassificationPolicy] = dict[str, DataClassificationPolicy]()
         # Only these vendors are allowed within this GZ (Datastores and Workspaces)
         self.vendorPolicies: dict[str, InfraStructureVendorPolicy] = dict[str, InfraStructureVendorPolicy]()
         # Only these locations are allowed within this GZ (Datastore and Workspaces)
+        self.hardVendorPolicies: dict[str, InfraHardVendorPolicy] = dict[str, InfraHardVendorPolicy]()
         self.locationPolicies: dict[str, InfraStructureLocationPolicy] = dict[str, InfraStructureLocationPolicy]()
         self.dataplatformPolicies: dict[str, DataPlatformPolicy] = dict[str, DataPlatformPolicy]()
 
         self.add(*args)
 
     def setEcosystem(self, eco: Ecosystem) -> None:
         """Sets the ecosystem for this zone and sets the zone for all teams"""
@@ -1744,23 +1858,28 @@
     def checkLocationIsAllowed(self, eco: 'Ecosystem', loc: InfrastructureLocation, tree: ValidationTree):
         """This checks that the provided location is allowed based on the vendor and location policies
         of the GZ, this allows a GZ to constrain where its data can come from or be used"""
         for locPolicy in self.locationPolicies.values():
             if not locPolicy.isCompatible(loc):
                 tree.addRaw(ObjectNotCompatibleWithPolicy(loc, locPolicy, ProblemSeverity.ERROR))
         if (loc.key):
+            v: InfrastructureVendor = eco.getVendorOrThrow(loc.key.ivName)
             for vendorPolicy in self.vendorPolicies.values():
-                v: InfrastructureVendor = eco.getVendorOrThrow(loc.key.ivName)
                 if not vendorPolicy.isCompatible(v):
                     tree.addRaw(ObjectNotCompatibleWithPolicy(v, vendorPolicy, ProblemSeverity.ERROR))
+            for hardVendorPolicy in self.hardVendorPolicies.values():
+                if (v.hardCloudVendor is None):
+                    tree.addRaw(AttributeNotSet(f"{loc} No hard cloud vendor"))
+                elif not hardVendorPolicy.isCompatible(v.hardCloudVendor):
+                    tree.addRaw(ObjectNotCompatibleWithPolicy(v, hardVendorPolicy, ProblemSeverity.ERROR))
         else:
             tree.addRaw(AttributeNotSet("loc.key"))
 
     def add(self, *args: Union[InfraStructureVendorPolicy, InfraStructureLocationPolicy, StoragePolicy, DataClassificationPolicy,
-                               TeamDeclaration, DataPlatformPolicy, Documentation]) -> None:
+                               TeamDeclaration, DataPlatformPolicy, Documentation, InfraHardVendorPolicy]) -> None:
         for arg in args:
             if (isinstance(arg, DataClassificationPolicy)):
                 dcc: DataClassificationPolicy = arg
                 self.classificationPolicies[dcc.name] = dcc
             elif (isinstance(arg, InfraStructureLocationPolicy)):
                 self.locationPolicies[arg.name] = arg
             elif (isinstance(arg, InfraStructureVendorPolicy)):
@@ -1769,14 +1888,16 @@
                 sp: StoragePolicy = arg
                 if self.storagePolicies.get(sp.name) is not None:
                     raise Exception(f"Duplicate Storage Policy {sp.name}")
                 self.storagePolicies[sp.name] = sp
             elif (type(arg) is TeamDeclaration):
                 t: TeamDeclaration = arg
                 self.teams.addAuthorization(t)
+            elif (isinstance(arg, InfraHardVendorPolicy)):
+                self.hardVendorPolicies[arg.name] = arg
             elif (isinstance(arg, DataPlatformPolicy)):
                 self.dataplatformPolicies[arg. name] = arg
             elif (isinstance(arg, Documentation)):
                 d: Documentation = arg
                 self.documentation = d
 
         # Set softlink keys
@@ -1913,22 +2034,31 @@
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, DataPlatform) and self.name == __value.name
 
     def __hash__(self) -> int:
         return hash(self.name)
 
+    @abstractmethod
+    def getInternalDataContainers(self) -> set[DataContainer]:
+        """A Data platform can have internal data containers which store ingested data or intermediate data"""
+        pass
+
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.name})"
 
     @abstractmethod
     def getSupportedVendors(self, eco: Ecosystem) -> set[InfrastructureVendor]:
         pass
 
     @abstractmethod
+    def isContainerSupported(self, eco: Ecosystem, dc: DataContainer) -> bool:
+        pass
+
+    @abstractmethod
     def lint(self, eco: Ecosystem, tree: ValidationTree):
         if (self.documentation):
             self.documentation.lint(tree)
 
 
 class DataLatency(Enum):
     """Specifies the acceptable latency range from a consumer"""
```

### Comparing `datasurface-0.0.6/src/datasurface/md/Lint.py` & `datasurface-0.0.9/src/datasurface/md/Lint.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/PipelineGraph.py` & `datasurface-0.0.9/src/datasurface/md/PipelineGraph.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/Policy.py` & `datasurface-0.0.9/src/datasurface/md/Policy.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/Schema.py` & `datasurface-0.0.9/src/datasurface/md/Schema.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/SqlAlchemyUtils.py` & `datasurface-0.0.9/src/datasurface/md/SqlAlchemyUtils.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/azureTemplates/AzureBatch.bicep` & `datasurface-0.0.9/src/datasurface/md/azureTemplates/AzureBatch.bicep`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/datasurface/md/utils.py` & `datasurface-0.0.9/src/datasurface/md/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,25 +34,41 @@
 
 def is_valid_azure_key_vault_name(name: str) -> bool:
     # Regular expression for a valid Azure Key Vault name
     pattern = r'^[a-z0-9]{3,24}$'
     return (re.match(pattern, name)) is not None
 
 
-def is_valid_hostname_or_ip(s: str) -> bool:  # Generated by CodeLLama 13B Q5_K_M
+def is_valid_hostname_or_ip(s: str) -> bool:
     """This checks if the string is a valid hostname or IP address"""
-    # Check if it's a valid IP address
-    # Check if the address is valid IPv4 or IPv6 using regular expressions
-    pattern = r"^(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9]{1,3}\.){3,3}[0-9]{1,3})(%[\w]+)?$"
-    if re.match(pattern, s) is not None:
+    # Check if it's a valid IPv4 address
+    pattern_ipv4 = r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$"
+    if re.fullmatch(pattern_ipv4, s) is not None:
         return True
-    else:
-        # Check hostname
-        pattern = r"^([a-zA-Z0-9]([a-zA-Z0-9\-]{0,61}[a-zA-Z0-9])?\.)+[a-zA-Z]{2,}$"
-        return re.match(pattern, s) is not None        # Check if it's a valid hostname
+
+    # Check if it's a valid IPv6 address
+    pattern_ipv6 = (
+        r"^(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|"
+        r"([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}"
+        r"(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|"
+        r"([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|"
+        r"fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|"
+        r"1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|"
+        r"1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9]))$"
+    )
+
+    if re.fullmatch(pattern_ipv6, s) is not None:
+        return True
+
+    # Check hostname
+    pattern_hostname = r"^(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)*([A-Za-z]|[A-Za-z][A-Za-z0-9\-]*[A-Za-z0-9])$"
+    if re.fullmatch(pattern_hostname, s) is not None and len(s) <= 253:
+        return True
+
+    return False
 
 
 class ANSI_SQL_NamedObject:
     """This is the base class for objects in the model which must have an SQL identifier compatible name. These
     objects may have names which are using in creating database artifacts such as Tables, views, columns"""
     def __init__(self, name: str) -> None:
         self.name: str = name
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step1/base/eco.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step1/base/eco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DefaultDataPlatform, Ecosystem, GovernanceZoneDeclaration, InfrastructureLocation, InfrastructureVendor
+from datasurface.md.Governance import CloudVendor, DefaultDataPlatform, Ecosystem, GovernanceZoneDeclaration, InfrastructureLocation, InfrastructureVendor
 
 # Base branch for step 1, define an Ecosystem, data platforms, infrastructure vendors/locations and 3 Governance Zones
 
 
 def createEcosystem() -> Ecosystem:
     e: Ecosystem = Ecosystem(
         "Test", GitHubRepository("billynewport/test_step1", "main"),
@@ -17,14 +17,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/test_step1", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/test_step1", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/test_step1", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -33,14 +34,15 @@
             InfrastructureLocation(
                 "EU",
                 InfrastructureLocation("eu-central-1"),  # Frankfurt
                 InfrastructureLocation("eu-west-3"))),
 
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation(
                     "Central",
                     InfrastructureLocation("Central US"),  # Iowa
                     InfrastructureLocation("North Central US"),  # Illinois
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_EU/eco.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_EU/eco.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, InfraStructureLocationPolicy, \
+from datasurface.md.Governance import CloudVendor, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, InfraStructureLocationPolicy, \
     InfrastructureLocation, InfrastructureVendor, TeamDeclaration
 
 # Base branch for step 1, define an Ecosystem, data platforms, infrastructure vendors/locations and 3 Governance Zones
 
 
 def createEcosystem() -> Ecosystem:
     e: Ecosystem = Ecosystem(
@@ -18,14 +18,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/test_step1", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/test_step1", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/test_step1", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -34,14 +35,15 @@
             InfrastructureLocation(
                 "EU",
                 InfrastructureLocation("eu-central-1"),  # Frankfurt
                 InfrastructureLocation("eu-west-3"))),
 
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation(
                     "Central",
                     InfrastructureLocation("Central US"),  # Iowa
                     InfrastructureLocation("North Central US"),  # Illinois
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step2/head_USA/eco.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step2/head_USA/eco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
+from datasurface.md.Governance import CloudVendor, DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
     InfraStructureLocationPolicy, InfraStructureVendorPolicy, InfrastructureLocation, InfrastructureVendor, TeamDeclaration
 
 # Base branch for step 1, define an Ecosystem, data platforms, infrastructure vendors/locations and 3 Governance Zones
 
 
 def createEcosystem() -> Ecosystem:
     e: Ecosystem = Ecosystem(
@@ -17,14 +17,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/test_step1", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/test_step1", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/test_step1", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -33,14 +34,15 @@
             InfrastructureLocation(
                 "EU",
                 InfrastructureLocation("eu-central-1"),  # Frankfurt
                 InfrastructureLocation("eu-west-3"))),
 
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation(
                     "Central",
                     InfrastructureLocation("Central US"),  # Iowa
                     InfrastructureLocation("North Central US"),  # Illinois
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step3/defineEU_GZ.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step3/defineEU_GZ.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     serverHost="tcp:nwdb.database.windows.net,1433",
                     databaseName="nwdb",
                     driver="{ODBC Driver 17 for SQL Server}",
                     connectionStringTemplate="mssql+pyodbc://{username}:{password}@{serverHost}/{databaseName}?driver={driver}"
                 ),
                 CronTrigger("NW_Data Every 10 mins", "*/10 * * * *"),
                 IngestionConsistencyType.MULTI_DATASET,
-                AzureKeyVaultCredential("https://mykeyvault.vault.azure.net", "NWDB_Creds")),
+                AzureKeyVaultCredential("mykeyvault", "NWDB_Creds")),
             Dataset(
                 "customers",
                 SimpleDC(SimpleDCTypes.PC3),
                 PlainTextDocumentation("This data includes customer information from the Northwind database. It contains PII data."),
                 DDLTable(
                     DDLColumn("customer_id", VarChar(5), NullableStatus.NOT_NULLABLE, PrimaryKeyStatus.PK),
                     DDLColumn("company_name", VarChar(40), NullableStatus.NOT_NULLABLE),
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step3/eco.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step3/eco.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
+from datasurface.md.Governance import CloudVendor, DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
     InfraStructureLocationPolicy, InfraStructureVendorPolicy, InfrastructureLocation, InfrastructureVendor, TeamDeclaration
 from tests.actionHandlerResources.step3.defineEU_GZ import defineEU_GZ
 
 # Base branch for step 1, define an Ecosystem, data platforms, infrastructure vendors/locations and 3 Governance Zones
 
 
 def createEcosystem() -> Ecosystem:
@@ -18,14 +18,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/test_step1", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/test_step1", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/test_step1", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -34,14 +35,15 @@
             InfrastructureLocation(
                 "EU",
                 InfrastructureLocation("eu-central-1"),  # Frankfurt
                 InfrastructureLocation("eu-west-3"))),
 
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation(
                     "Central",
                     InfrastructureLocation("Central US"),  # Iowa
                     InfrastructureLocation("North Central US"),  # Illinois
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step4/defineEU_GZ.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step4/defineEU_GZ.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     serverHost="tcp:nwdb.database.windows.net,1433",
                     databaseName="nwdb",
                     driver="{ODBC Driver 17 for SQL Server}",
                     connectionStringTemplate="mssql+pyodbc://{username}:{password}@{serverHost}/{databaseName}?driver={driver}"
                 ),
                 CronTrigger("NW_Data Every 10 mins", "*/10 * * * *"),
                 IngestionConsistencyType.MULTI_DATASET,
-                AzureKeyVaultCredential("https://mykeyvault.vault.azure.net", "NWDB_Creds")),
+                AzureKeyVaultCredential("mykeyvault", "NWDB_Creds")),
             Dataset(
                 "customers",
                 SimpleDC(SimpleDCTypes.PC3),
                 PlainTextDocumentation("This data includes customer information from the Northwind database. It contains PII data."),
                 DDLTable(
                     DDLColumn("customer_id", VarChar(5), NullableStatus.NOT_NULLABLE, PrimaryKeyStatus.PK),
                     DDLColumn("company_name", VarChar(40), NullableStatus.NOT_NULLABLE),
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step4/defineUSA_GZ.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step4/defineUSA_GZ.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     serverHost="tcp:nwdb.database.windows.net,1433",
                     databaseName="nwdb",
                     driver="{ODBC Driver 17 for SQL Server}",
                     connectionStringTemplate="mssql+pyodbc://{username}:{password}@{serverHost}/{databaseName}?driver={driver}"
                 ),
                 CronTrigger("NW_Data Every 10 mins", "*/10 * * * *"),
                 IngestionConsistencyType.MULTI_DATASET,
-                AzureKeyVaultCredential("https://mykeyvault.vault.azure.net", "NWDB_Creds")),
+                AzureKeyVaultCredential("mykeyvault", "NWDB_Creds")),
             Dataset(
                 "customers",
                 SimpleDC(SimpleDCTypes.PC3),
                 PlainTextDocumentation("This data includes customer information from the Northwind database. It contains PII data."),
                 DDLTable(
                     DDLColumn("customer_id", VarChar(5), NullableStatus.NOT_NULLABLE, PrimaryKeyStatus.PK),
                     DDLColumn("company_name", VarChar(40), NullableStatus.NOT_NULLABLE),
```

### Comparing `datasurface-0.0.6/src/tests/actionHandlerResources/step4/eco.py` & `datasurface-0.0.9/src/tests/actionHandlerResources/step4/eco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
+from datasurface.md.Governance import CloudVendor, DataPlatformPolicy, DefaultDataPlatform, Ecosystem, GovernanceZone, GovernanceZoneDeclaration, \
     InfraStructureLocationPolicy, InfraStructureVendorPolicy, InfrastructureLocation, InfrastructureVendor, TeamDeclaration
 from tests.actionHandlerResources.step3.defineEU_GZ import defineEU_GZ
 from tests.actionHandlerResources.step4.defineUSA_GZ import defineUSA_GZ
 
 # Base branch for step 1, define an Ecosystem, data platforms, infrastructure vendors/locations and 3 Governance Zones
 
 
@@ -20,14 +20,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/test_step1", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/test_step1", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/test_step1", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -36,14 +37,15 @@
             InfrastructureLocation(
                 "EU",
                 InfrastructureLocation("eu-central-1"),  # Frankfurt
                 InfrastructureLocation("eu-west-3"))),
 
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation(
                     "Central",
                     InfrastructureLocation("Central US"),  # Iowa
                     InfrastructureLocation("North Central US"),  # Illinois
```

### Comparing `datasurface-0.0.6/src/tests/nwdb/eco.py` & `datasurface-0.0.9/src/tests/nwdb/eco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datasurface.md import Team, GovernanceZoneDeclaration, GovernanceZone, InfrastructureVendor, InfrastructureLocation, TeamDeclaration
 from datasurface.md import Ecosystem
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
-from datasurface.md.Governance import DefaultDataPlatform, InfraStructureLocationPolicy
+from datasurface.md.Governance import CloudVendor, DefaultDataPlatform, InfraStructureLocationPolicy
 from datasurface.md.Lint import ValidationTree
 from tests.nwdb.nwdb import defineTables as defineNWTeamTables
 from tests.nwdb.nwdb import defineWorkspaces as defineNWTeamWorkspaces
 
 
 def createEcosystem() -> Ecosystem:
     ecosys: Ecosystem = Ecosystem(
@@ -23,14 +23,15 @@
         GovernanceZoneDeclaration("USA", GitHubRepository("billynewport/repo", "USAmain")),
         GovernanceZoneDeclaration("EU", GitHubRepository("billynewport/repo", "EUmain")),
         GovernanceZoneDeclaration("UK", GitHubRepository("billynewport/repo", "UKmain")),
 
         # Infra Vendors and locations
         InfrastructureVendor(
             "AWS",
+            CloudVendor.AWS,
             PlainTextDocumentation("Amazon AWS"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("us-east-1"),  # Virginia
                 InfrastructureLocation("us-west-1")),
             InfrastructureLocation(
                 "UK",
@@ -49,14 +50,15 @@
                 InfrastructureLocation("NY_1")),
             InfrastructureLocation(
                 "UK",
                 InfrastructureLocation("London"),
                 InfrastructureLocation("Cambridge"))),
         InfrastructureVendor(
             "Azure",
+            CloudVendor.AZURE,
             PlainTextDocumentation("Microsoft Azure"),
             InfrastructureLocation(
                 "USA",
                 InfrastructureLocation("Central US"),  # Iowa
                 InfrastructureLocation("East US"),  # Virginia
                 InfrastructureLocation("East US 2"),  # Virginia
                 InfrastructureLocation("East US 3"),  # Georgia
```

### Comparing `datasurface-0.0.6/src/tests/nwdb/nwdb.py` & `datasurface-0.0.9/src/tests/nwdb/nwdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 
 def defineTables(eco: Ecosystem, gz: GovernanceZone, t: Team):
     t.add(
         Datastore(
             "NW_Data",
             CDCCaptureIngestion(
-                AzureSQLDatabase("NW_DB", "hostName:port", "DBName", eco.getLocationOrThrow("Azure", ["USA", "East US"])),
+                AzureSQLDatabase("NW_DB", "hostName", 1344, "DBName", eco.getLocationOrThrow("Azure", ["USA", "East US"])),
                 CronTrigger("NW_Data Every 10 mins", "0,10,20,30,40,50 * * * *"),
                 IngestionConsistencyType.MULTI_DATASET,
-                AzureKeyVaultCredential("https://mykeyvault.vault.azure.net", "NWDB_Creds")
+                AzureKeyVaultCredential("mykeyvault", "NWDB_Creds")
                 ),
 
             Dataset(
                 "us_states",
                 SimpleDC(SimpleDCTypes.PUB),
                 DDLTable(
                     DDLColumn("state_id", SmallInt(), NullableStatus.NOT_NULLABLE, PrimaryKeyStatus.PK),
@@ -201,15 +201,15 @@
     )
 
 
 def defineWorkspaces(eco: Ecosystem, t: Team, location: InfrastructureLocation):
     """Create a Workspace and an asset if a location is provided"""
 
     # Warehouse for Workspaces
-    ws_db: DataContainer = AzureSQLDatabase("AzureSQL", "hostName:port", "DBName", location)
+    ws_db: DataContainer = AzureSQLDatabase("AzureSQL", "hostName", 1344, "DBName", location)
 
     w: Workspace = Workspace(
         "ProductLiveAdhocReporting",
         ws_db,
         DatasetGroup(
             "LiveProducts",
             WorkspacePlatformConfig(
```

### Comparing `datasurface-0.0.6/src/tests/test_ActionHandler.py` & `datasurface-0.0.9/src/tests/test_ActionHandler.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_GitOps.py` & `datasurface-0.0.9/src/tests/test_GitOps.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_Lint.py` & `datasurface-0.0.9/src/tests/test_Lint.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_PlatformGraph.py` & `datasurface-0.0.9/src/tests/test_PlatformGraph.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_Policy.py` & `datasurface-0.0.9/src/tests/test_Policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
         # Test case 4: Object is both explicitly allowed and forbidden
         allowed_values = {1, 2, 3}
         not_allowed_values = {3, 4, 5}
         try:
             policy = AllowDisallowPolicy("Test Policy", PlainTextDocumentation("Test"), allowed=allowed_values, notAllowed=not_allowed_values)
             self.fail("Exception not thrown for overlapping allow/disallow sets")
-        except:
+        except Exception:
             # Test is succesful
-            pass
+            pass
```

### Comparing `datasurface-0.0.6/src/tests/test_Postgres.py` & `datasurface-0.0.9/src/tests/test_Postgres.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_Schema.py` & `datasurface-0.0.9/src/tests/test_Schema.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_SchemaCompatibility.py` & `datasurface-0.0.9/src/tests/test_SchemaCompatibility.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_SimpleZone.py` & `datasurface-0.0.9/src/tests/test_SimpleZone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 import unittest
 
 from datasurface.md import InfrastructureVendor, InfrastructureLocation, TeamDeclaration, Ecosystem
 from datasurface.md import GovernanceZone, GovernanceZoneDeclaration
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import GitHubRepository
+from datasurface.md.Governance import CloudVendor
 from datasurface.md.Lint import ValidationTree
 from tests.nwdb.eco import createEcosystem
 
 
 class TestZones(unittest.TestCase):
 
     def test_DuplicateTeamNames(self):
@@ -46,14 +47,15 @@
         eco.add(
             GovernanceZoneDeclaration(usZoneName, GitHubRepository("aa/cc", "bb")),
         )
         gzUSA: GovernanceZone = eco.getZoneOrThrow(usZoneName)
         eco.add(
                 InfrastructureVendor(
                     "AWS",
+                    CloudVendor.AWS,
                     PlainTextDocumentation("AWS is a cloud provider"),
                     InfrastructureLocation(
                         "USA",
                         InfrastructureLocation("us-east-1"),
                         InfrastructureLocation("us-east-2"),
                         InfrastructureLocation("us-west-1"),
                         InfrastructureLocation("us-west-2")
@@ -64,14 +66,15 @@
                         InfrastructureLocation("eu-west-2")
                         ),
                 ))
 
         eco.add(
             InfrastructureVendor(
                 "AZURE",
+                CloudVendor.AZURE,
                 PlainTextDocumentation("AZURE is a cloud provider"),
                 InfrastructureLocation(
                     "USA",
                     InfrastructureLocation("Central US"),
                     InfrastructureLocation("North Central US"),
                     InfrastructureLocation("South Central US"),
                     InfrastructureLocation("West Central US"),
```

### Comparing `datasurface-0.0.6/src/tests/test_StoragePolicy.py` & `datasurface-0.0.9/src/tests/test_StoragePolicy.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_TypeToPython.py` & `datasurface-0.0.9/src/tests/test_TypeToPython.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_Utils.py` & `datasurface-0.0.9/src/tests/test_Utils.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_Workspace.py` & `datasurface-0.0.9/src/tests/test_Workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datasurface.md import Decimal, Variant, TinyInt, SmallInt, BigInt, Float, Double, Vector, GovernanceZoneDeclaration
 from datasurface.md import ConsumerRetentionRequirements, DataRetentionPolicy
 from datetime import timedelta
 from datasurface.md.AmazonAWS import AmazonAWSDataPlatform
 from datasurface.md.Azure import AzureSQLDatabase, AzureDataplatform, AzureKeyVaultCredential
 from datasurface.md.Documentation import PlainTextDocumentation
 from datasurface.md.GitOps import FakeRepository, GitHubRepository
-from datasurface.md.Governance import CDCCaptureIngestion, DataTransformerOutput, DatastoreCacheEntry, DefaultDataPlatform, DependentWorkspaces, \
+from datasurface.md.Governance import CDCCaptureIngestion, CloudVendor, DataTransformerOutput, DatastoreCacheEntry, DefaultDataPlatform, DependentWorkspaces, \
     DeprecationStatus, DeprecationsAllowed, InfrastructureLocation, InfrastructureVendor, IngestionConsistencyType, ProductionStatus
 from datasurface.md.Lint import ValidationTree
 from datasurface.md.Policy import SimpleDC, SimpleDCTypes
 
 from datasurface.md.Schema import NullableStatus, PrimaryKeyStatus
 from tests.nwdb.eco import createEcosystem
 
@@ -360,30 +360,32 @@
         e: Ecosystem = Ecosystem(
                 "BigCorp", FakeRepository("a"),
                 DefaultDataPlatform(
                     AzureDataplatform("Azure", PlainTextDocumentation("Test"), AzureKeyVaultCredential("keyvault", "aa"))
                     ),
                 InfrastructureVendor(
                     "Azure",
+                    CloudVendor.AWS,
                     PlainTextDocumentation("Azure test vendor"),
                     InfrastructureLocation("FL")),
                 GovernanceZoneDeclaration("US", FakeRepository("b")))
 
         # Define US zone and declare a single team Test
         gzUSA: GovernanceZone = e.getZoneOrThrow("US")
         gzUSA.add(TeamDeclaration("Test", FakeRepository("c")))
 
         # Define the team with a single store with 2 datasets and a single Workspace using those datasets
         t: Team = gzUSA.getTeamOrThrow("Test")
         t.add(
             Datastore(
                 "Store1",
                 CDCCaptureIngestion(
-                    AzureSQLDatabase("Test", "mysqlserver.database.windows.net", "dbName", e.getLocationOrThrow("Azure", ["FL"])),
-                    IngestionConsistencyType.MULTI_DATASET
+                    AzureSQLDatabase("Test", "mysqlserver.database.windows.net", 1344, "dbName", e.getLocationOrThrow("Azure", ["FL"])),
+                    IngestionConsistencyType.MULTI_DATASET,
+                    AzureKeyVaultCredential("keyvault", "aa")
                 ),
                 Dataset(
                     "Dataset1",
                     SimpleDC(SimpleDCTypes.PUB),
                     DDLTable(
                         DDLColumn("Col1", Integer(), PrimaryKeyStatus.PK, NullableStatus.NOT_NULLABLE),
                         DDLColumn("Col2", String(10)),
```

### Comparing `datasurface-0.0.6/src/tests/test_authorized_changes.py` & `datasurface-0.0.9/src/tests/test_authorized_changes.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_cyclic_equals.py` & `datasurface-0.0.9/src/tests/test_cyclic_equals.py`

 * *Files identical despite different names*

### Comparing `datasurface-0.0.6/src/tests/test_nwdb.py` & `datasurface-0.0.9/src/tests/test_nwdb.py`

 * *Files identical despite different names*

