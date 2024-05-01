# Comparing `tmp/ecs_connect_cli-1.8.0.tar.gz` & `tmp/ecs_connect_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_connect_cli-1.8.0.tar", last modified: Wed Feb 14 16:13:02 2024, max compression
+gzip compressed data, was "ecs_connect_cli-1.9.0.tar", last modified: Thu Feb 15 11:14:05 2024, max compression
```

## Comparing `ecs_connect_cli-1.8.0.tar` & `ecs_connect_cli-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/ecs_connect/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/ecs_connect/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-02-14 16:13:02.000000 ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-14 16:13:02.000000 ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:13:02.000000 ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-14 16:13:02.000000 ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:13:02.633438 ecs_connect_cli-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-14 16:12:52.000000 ecs_connect_cli-1.8.0/tests/test_ecs_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:14:05.806896 ecs_connect_cli-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-02-15 11:14:05.806896 ecs_connect_cli-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:14:05.802896 ecs_connect_cli-1.9.0/ecs_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/ecs_connect/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:14:05.806896 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-02-15 11:14:05.000000 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-15 11:14:05.000000 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 11:14:05.000000 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-15 11:14:05.000000 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-15 11:14:05.000000 ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 11:14:05.806896 ecs_connect_cli-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 11:14:05.802896 ecs_connect_cli-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-15 11:13:52.000000 ecs_connect_cli-1.9.0/tests/test_ecs_connect.py
```

### Comparing `ecs_connect_cli-1.8.0/LICENSE` & `ecs_connect_cli-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/PKG-INFO` & `ecs_connect_cli-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ecs_connect_cli
-Version: 1.8.0
-Summary: AWS ECS Cli tool for connecting to ecs container and update secret manager
-Author-email: Frederic Egmorte <frederic.egmorte@gmail.com>
-Project-URL: Homepage, https://github.com/fegmorte/aws-ecs-exec-command-cli
-Project-URL: Issues, https://github.com/fegmorte/aws-ecs-exec-command-cli/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # aws-ecs-exec-command-cli
 
 AWS ECS Exec command cli tool is aimed to :
 
 - connect to your container instance running under ECS Fargate.
 - tail the log from cloudwatch logs (if you configure a logconfiguration in your task definition)
 - update secret value into secret manager
@@ -104,8 +90,8 @@
 
 ```
 
 &nbsp;
 
 Thanks to Typer from [@tiangolo](https://typer.tiangolo.com/)
 
-Thanks to [@kraymer](https://github.com/kraymer) for echoprompt :sunglasses:
+Thanks to [@kraymer](https://github.com/kraymer) for echoprompt :sunglasses:
```

### Comparing `ecs_connect_cli-1.8.0/README.md` & `ecs_connect_cli-1.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: ecs_connect_cli
+Version: 1.9.0
+Summary: AWS ECS Cli tool for connecting to ecs container and update secret manager
+Author-email: Frederic Egmorte <frederic.egmorte@gmail.com>
+Project-URL: Homepage, https://github.com/fegmorte/aws-ecs-exec-command-cli
+Project-URL: Issues, https://github.com/fegmorte/aws-ecs-exec-command-cli/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3==1.26.13
+Requires-Dist: typer[all]==0.9.0
+Requires-Dist: pytest==6.2.4
+Requires-Dist: echoprompt==0.2.0
+Requires-Dist: deepdiff
+
 # aws-ecs-exec-command-cli
 
 AWS ECS Exec command cli tool is aimed to :
 
 - connect to your container instance running under ECS Fargate.
 - tail the log from cloudwatch logs (if you configure a logconfiguration in your task definition)
 - update secret value into secret manager
@@ -90,8 +109,8 @@
 
 ```
 
 &nbsp;
 
 Thanks to Typer from [@tiangolo](https://typer.tiangolo.com/)
 
-Thanks to [@kraymer](https://github.com/kraymer) for echoprompt :sunglasses:
+Thanks to [@kraymer](https://github.com/kraymer) for echoprompt :sunglasses:
```

### Comparing `ecs_connect_cli-1.8.0/ecs_connect/cli.py` & `ecs_connect_cli-1.9.0/ecs_connect/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/ecs_connect/credentials.py` & `ecs_connect_cli-1.9.0/ecs_connect/credentials.py`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/ecs_connect/helpers.py` & `ecs_connect_cli-1.9.0/ecs_connect/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/ecs_connect/menu.py` & `ecs_connect_cli-1.9.0/ecs_connect/menu.py`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/ecs_connect/session.py` & `ecs_connect_cli-1.9.0/ecs_connect/session.py`

 * *Files identical despite different names*

### Comparing `ecs_connect_cli-1.8.0/ecs_connect_cli.egg-info/PKG-INFO` & `ecs_connect_cli-1.9.0/ecs_connect_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: ecs_connect_cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: AWS ECS Cli tool for connecting to ecs container and update secret manager
 Author-email: Frederic Egmorte <frederic.egmorte@gmail.com>
 Project-URL: Homepage, https://github.com/fegmorte/aws-ecs-exec-command-cli
 Project-URL: Issues, https://github.com/fegmorte/aws-ecs-exec-command-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3==1.26.13
+Requires-Dist: typer[all]==0.9.0
+Requires-Dist: pytest==6.2.4
+Requires-Dist: echoprompt==0.2.0
+Requires-Dist: deepdiff
 
 # aws-ecs-exec-command-cli
 
 AWS ECS Exec command cli tool is aimed to :
 
 - connect to your container instance running under ECS Fargate.
 - tail the log from cloudwatch logs (if you configure a logconfiguration in your task definition)
```

### Comparing `ecs_connect_cli-1.8.0/pyproject.toml` & `ecs_connect_cli-1.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 [project]
 name = "ecs_connect_cli"
 dynamic = ["version"]
+
+dependencies = [
+  "boto3==1.26.13",
+  "typer[all]==0.9.0",
+  "pytest==6.2.4",
+  "echoprompt==0.2.0",
+  "deepdiff",
+]
+
 authors = [
   { name="Frederic Egmorte", email="frederic.egmorte@gmail.com" },
 ]
+
 description = "AWS ECS Cli tool for connecting to ecs container and update secret manager"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -19,8 +29,8 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "setuptools-git-versioning<2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
-starting_version = "1.8.0"
+starting_version = "1.9.0"
```

