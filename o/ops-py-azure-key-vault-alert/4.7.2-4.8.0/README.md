# Comparing `tmp/ops_py_azure_key_vault_alert-4.7.2.tar.gz` & `tmp/ops_py_azure_key_vault_alert-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_alert-4.7.2.tar", last modified: Thu Apr 25 10:55:03 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_alert-4.8.0.tar", last modified: Wed May  1 08:13:58 2024, max compression
```

## Comparing `ops_py_azure_key_vault_alert-4.7.2.tar` & `ops_py_azure_key_vault_alert-4.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:55:03.103237 ops_py_azure_key_vault_alert-4.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 10:55:00.000000 ops_py_azure_key_vault_alert-4.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 10:55:03.103237 ops_py_azure_key_vault_alert-4.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:55:03.103237 ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-25 10:54:55.000000 ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10826 2024-04-25 10:54:55.000000 ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2531 2024-04-25 10:54:55.000000 ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/slack_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2281 2024-04-25 10:54:55.000000 ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:55:03.103237 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 10:55:03.000000 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 10:55:03.000000 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:55:03.000000 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 10:55:03.000000 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 10:55:03.000000 ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 10:55:00.000000 ops_py_azure_key_vault_alert-4.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 10:55:00.000000 ops_py_azure_key_vault_alert-4.7.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 10:54:55.000000 ops_py_azure_key_vault_alert-4.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:55:03.103237 ops_py_azure_key_vault_alert-4.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 10:55:00.000000 ops_py_azure_key_vault_alert-4.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.157855 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11035 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2531 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/slack_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2281 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 08:13:58.000000 ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 08:13:51.000000 ops_py_azure_key_vault_alert-4.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:13:58.161855 ops_py_azure_key_vault_alert-4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 08:13:56.000000 ops_py_azure_key_vault_alert-4.8.0/setup.py
```

### Comparing `ops_py_azure_key_vault_alert-4.7.2/LICENSE` & `ops_py_azure_key_vault_alert-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.7.2/PKG-INFO` & `ops_py_azure_key_vault_alert-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.7.2
+Version: 4.8.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/azure_key_vault_alert.py` & `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
     # Get the full report which will be written to file, and may be used for future references (logging / monitoring).
     # The name of the Workflow and Azure resource information are added to the json object.
     report_full = kv_report.get_report_full()
     if isinstance(report_full, dict):
         workflow_output_name = str(WORKFLOW_OUTPUT_NAME).strip().lower().replace(" ", "_")[:40]
         report_full["name"] = workflow_output_name
+        report_full["repository_name"] = str(GITHUB_REPOSITORY).split("/")[-1]
         report_full["client_id"] = AZURE_CLIENT_ID
         report_full["subscription_id"] = AZURE_SUBSCRIPTION_ID
         report_full["tenant_id"] = AZURE_TENANT_ID
 
         # Ensure a valid filename is set. If that is not the case, then 'output.json' is used as default.
         workflow_output_file = str(workflow_output_file.lower()).replace(" ", "_")
         if not bool(re.match("^[a-z0-9_-]*$", workflow_output_file)):
@@ -211,16 +212,20 @@
     # the following environment variable
     WEBHOOK_REPORT = os.getenv("WEBHOOK_REPORT")
 
     # When all the reports have been posted, an additional POST is performed
     # to the webhook exported in following environment variable:
     WEBHOOK_NOTIFY = os.getenv("WEBHOOK_NOTIFY")
 
+    # The value of the name key in the full json logfile
+    WORKFLOW_OUTPUT_NAME = os.getenv("WORKFLOW_OUTPUT_NAME", "")
+
+    # The value of the github_repo name key in the full json logfile
+    GITHUB_REPOSITORY = os.getenv("GITHUB_REPOSITORY", "")
+
     # These Azure environment variables will be used in the full json logfile
     AZURE_CLIENT_ID = os.getenv("AZURE_CLIENT_ID")
     AZURE_SUBSCRIPTION_ID = os.getenv("AZURE_SUBSCRIPTION_ID")
     AZURE_TENANT_ID = os.getenv("AZURE_TENANT_ID")
 
-    # The value of the name key in the full json logfile
-    WORKFLOW_OUTPUT_NAME = os.getenv("WORKFLOW_OUTPUT_NAME", "")
 
     main()
```

### Comparing `ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/slack_post.py` & `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/slack_post.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.7.2/azure_key_vault_alert/teams_alert.py` & `ops_py_azure_key_vault_alert-4.8.0/azure_key_vault_alert/teams_alert.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.7.2
+Version: 4.8.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_azure_key_vault_alert-4.7.2/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops_py_azure_key_vault_alert-4.8.0/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.7.2/readme.md` & `ops_py_azure_key_vault_alert-4.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.7.2/requirements.txt` & `ops_py_azure_key_vault_alert-4.8.0/requirements.txt`

 * *Files identical despite different names*

