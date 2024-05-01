# Comparing `tmp/pbsrollout-0.3.4.9.tar.gz` & `tmp/pbsrollout-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.4.9.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.5.tar", max compression
```

## Comparing `pbsrollout-0.3.4.9.tar` & `pbsrollout-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.4.9/LICENSE
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.4.9/pbsrollout/__init__.py
--rw-r--r--   0        0        0       48 2024-04-26 16:50:25.049516 pbsrollout-0.3.4.9/pbsrollout/config/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.4.9/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.4.9/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.4.9/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.4.9/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.4.9/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.4.9/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1344 2024-04-26 16:50:20.323610 pbsrollout-0.3.4.9/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.4.9/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.4.9/pbsrollout/internal/test_utils.py
--rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.4.9/pbsrollout/internal/test_utils_gh.py
--rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.4.9/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     2958 2024-04-25 22:53:25.462662 pbsrollout-0.3.4.9/pbsrollout/internal/utils_gh.py
--rw-r--r--   0        0        0     6571 2024-04-26 16:50:46.668815 pbsrollout-0.3.4.9/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.4.9/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0    10013 2024-04-26 16:51:05.778066 pbsrollout-0.3.4.9/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.4.9/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     7411 2024-04-26 18:15:28.386339 pbsrollout-0.3.4.9/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.4.9/pbsrollout/test_main.py
--rw-r--r--   0        0        0      585 2024-04-26 18:15:32.085209 pbsrollout-0.3.4.9/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.5/pbsrollout/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-01 19:51:05.039744 pbsrollout-0.3.5/pbsrollout/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.5/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.5/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.5/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.5/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.5/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.5/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1344 2024-04-26 16:50:20.323610 pbsrollout-0.3.5/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.5/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.5/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.5/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.5/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2958 2024-04-25 22:53:25.462662 pbsrollout-0.3.5/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     6637 2024-05-01 19:51:35.830148 pbsrollout-0.3.5/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.5/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9974 2024-05-01 19:53:56.271504 pbsrollout-0.3.5/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.5/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     7451 2024-05-01 19:53:24.960608 pbsrollout-0.3.5/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.5/pbsrollout/test_main.py
+-rw-r--r--   0        0        0      583 2024-05-01 19:53:38.977021 pbsrollout-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 pbsrollout-0.3.5/PKG-INFO
```

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.5/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.5/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.5/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.5/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.5/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/test_utils_gh.py` & `pbsrollout-0.3.5/pbsrollout/internal/test_utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/utils.py` & `pbsrollout-0.3.5/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/internal/utils_gh.py` & `pbsrollout-0.3.5/pbsrollout/internal/utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.9/pbsrollout/main.py` & `pbsrollout-0.3.5/pbsrollout/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 
 from botocore.exceptions import ClientError
 from kubernetes.client import ApiException
 from rich.console import Console
 from simple_term_menu import TerminalMenu
 
-from pbsrollout.config import REPOSITORY_NAME
+from pbsrollout.config import STAGING_REPOSITORY_NAME, PROD_REPOSITORY_NAME
 from pbsrollout.internal.utils import notify, get_latest_version, is_dev
 
 VERSION = ""
 try:
     import importlib.metadata
 
     VERSION = importlib.metadata.version("pbsrollout")
@@ -161,15 +161,15 @@
             console.print("[bold red]\nerror: please run `zaws_ctv_engineer` to login")
             return 1
         elif isinstance(e, RuntimeError):
             console.print(f"[bold red]\nError: {e}")
         elif isinstance(e, TimeoutExpired):
             console.print(f"[bold red]\nerror: {e}")
         elif isinstance(e, UnicodeDecodeError) and 'codec can\'t decode byte' in e.reason:
-            console.print(f"\nerror: {e}\n\n[bold red] You might want to run `git-crypt unlock` in the `{REPOSITORY_NAME}` repository\nit should fix this issue. Otherwise please send this to Dimitri Wyzlic on Slack!")
+            console.print(f"\nerror: {e}\n\n[bold red] You might want to run `git-crypt unlock` in the `{STAGING_REPOSITORY_NAME}` or `{PROD_REPOSITORY_NAME}` repository\nit should fix this issue. Otherwise please send this to Dimitri Wyzlic on Slack!")
         else:
             console.print_exception()
             console.print('[orange3]please send this to Dimitri Wyzlic on Slack!')
             return 1
     except KeyboardInterrupt:
         console.print("\n\n[bold red]Interrupted by user (CTRL-C)")
     return 0
```

### Comparing `pbsrollout-0.3.4.9/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.5/pbsrollout/pbs_release/main_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os
 import sys
 import time
 from subprocess import TimeoutExpired
 from typing import Dict
 
 from kubernetes import config
-from kubernetes.client import ApiException, ApiClient
+from kubernetes.client import ApiClient
 from rich.columns import Columns
 from rich.console import Console
-from rich.markdown import Markdown
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
-from pbsrollout.config import REPOSITORY_NAME
+from pbsrollout.config import PROD_REPOSITORY_NAME
 from pbsrollout.internal.check_cluster_ready import check_cluster_ready
 from pbsrollout.internal.k8s_utils import import_kube_config
 from pbsrollout.internal.process_cluster import cutover_service, launch_pods, remove_old_pods, Status
 from pbsrollout.internal.utils import notify
 
 CLUSTERS = [
-    "aws.us-east-1-eks-23-v3",
+    "aws.us-east-1-eks-23-v4",
     "aws.us-east-1-eks-24-v3",
     "aws.us-east-1-eks-25-v3",
     "aws.us-east-1-eks-26-v3",
     "aws.eu-west-1-eks-16-v3",
     "aws.ap-southeast-2-eks-33-v1",
     "aws.ap-southeast-2-eks-34-v1",
 ]
@@ -161,15 +160,15 @@
     #  - plz git pull
     if not no_interaction:
         console.print(
             "[bold red]Please run[/bold red] [italic misty_rose1]git pull --rebase[italic misty_rose1] [bold red]before running this script![/bold red]")
         ask_if_git_pull()
 
     # 1. CD Inside the prebid kube manifest directory
-    prebid_k8s_path = gopath + f'/src/github.com/integralads/{REPOSITORY_NAME}'
+    prebid_k8s_path = gopath + f'/src/github.com/integralads/{PROD_REPOSITORY_NAME}'
     with Dir(prebid_k8s_path):
         console.print("\n\n[bold]Step 1: updating prebid tag")
         tag = tag_from_args if tag_from_args != "" else ask_for_tag()
         if tag == "":
             print("error: tag must not be empty")
             return
```

### Comparing `pbsrollout-0.3.4.9/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.5/pbsrollout/stg_release/main_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import copy
 from typing import Tuple, Callable, List, Any
 
 from rich.console import Console
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
-from pbsrollout.config import REPOSITORY_NAME
+from pbsrollout.config import STAGING_REPOSITORY_NAME
 from pbsrollout.internal.aws_utils import get_ecr_images
 from pbsrollout.internal.utils import clean_stderr, print_error_body
 from pbsrollout.internal.utils_gh import get_pr_titles_and_author_from_commit_hash, does_gh_cli_exist
 
 NB_STAGINGS = 20
 
 def get_and_enforce_go_path(console: Console) -> str:
@@ -94,51 +94,51 @@
     # else:
     #     for f in full_img:
     #         if f.endswith(tag[:len('cd1ef6b73')]):
     #             tag = f
     #             break
 
     # put it in the file
-    dir_path = go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/namespace/stg/'
+    dir_path = go_path + f'/src/github.com/integralads/{STAGING_REPOSITORY_NAME}/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
         for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
             console.print(f"[bold light_steel_blue1]{tag_file_path}[/bold light_steel_blue1]")
             with open(tag_file_path, "w") as f:
                 f.write(tag)
 
     # step 2: release pods
     for stg in stg_idx:
         launch_staging_pod(stg,
-                           go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/')
+                           go_path + f'/src/github.com/integralads/{STAGING_REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/')
         console.print('\t[bold green]success!')
 
 
 def exit_fn(console: Console, stg_idx: List[str], go_path: str):
     return
 
 
 def migrate_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
-        dir_path = go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
+        dir_path = go_path + f'/src/github.com/integralads/{STAGING_REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tMigrating staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/migrate-staging-db {stg.lstrip('0')}"
             ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
                 print_error_body(f"ERROR:\n\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
                 return False
 
 
 def sync_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
-        dir_path = go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
+        dir_path = go_path + f'/src/github.com/integralads/{STAGING_REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tSyncing staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/sync-staging-db {stg.lstrip('0')}"
             ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
```

### Comparing `pbsrollout-0.3.4.9/pyproject.toml` & `pbsrollout-0.3.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.4.9"
+version = "0.3.5"
 description = "A tool to help Publica engineer test and release the platform"
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.4.9/PKG-INFO` & `pbsrollout-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.4.9
+Version: 0.3.5
 Summary: A tool to help Publica engineer test and release the platform
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

