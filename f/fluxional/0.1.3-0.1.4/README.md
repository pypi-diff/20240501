# Comparing `tmp/fluxional-0.1.3.tar.gz` & `tmp/fluxional-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.3.tar", max compression
+gzip compressed data, was "fluxional-0.1.4.tar", max compression
```

## Comparing `fluxional-0.1.3.tar` & `fluxional-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1059 2024-02-02 01:48:46.163715 fluxional-0.1.3/LICENSE
--rw-r--r--   0        0        0     3464 2024-04-22 20:27:58.523354 fluxional-0.1.3/README.md
--rw-r--r--   0        0        0      398 2024-04-06 03:52:15.283626 fluxional-0.1.3/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-06 03:52:08.843621 fluxional-0.1.3/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21402 2024-04-28 00:09:22.534943 fluxional-0.1.3/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-08 20:56:52.652758 fluxional-0.1.3/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-05 19:49:43.040843 fluxional-0.1.3/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-08 20:56:56.662776 fluxional-0.1.3/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    19676 2024-04-28 00:09:59.214928 fluxional-0.1.3/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7699 2024-04-28 00:07:24.364991 fluxional-0.1.3/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9554 2024-04-28 00:08:07.284974 fluxional-0.1.3/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-07 16:02:37.282853 fluxional-0.1.3/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-08 20:56:58.162781 fluxional-0.1.3/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-09 17:45:40.573927 fluxional-0.1.3/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-08 20:57:01.432779 fluxional-0.1.3/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-06 03:51:27.790814 fluxional-0.1.3/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-02-02 02:20:07.747714 fluxional-0.1.3/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15256 2024-04-03 23:29:19.551745 fluxional-0.1.3/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-05 19:50:15.280830 fluxional-0.1.3/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-03 20:50:44.146193 fluxional-0.1.3/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-02-02 01:50:49.633706 fluxional-0.1.3/fluxional/utils.py
--rw-r--r--   0        0        0     1151 2024-04-28 00:19:41.426103 fluxional-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 fluxional-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.4/README.md
+-rw-r--r--   0        0        0      421 2024-04-30 22:07:55.223192 fluxional-0.1.4/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.4/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.4/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.4/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21402 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.4/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.4/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    19676 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.4/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.4/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/utils.py
+-rw-r--r--   0        0        0     1151 2024-04-30 22:08:15.593233 fluxional-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.4/PKG-INFO
```

### Comparing `fluxional-0.1.3/LICENSE` & `fluxional-0.1.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 tj
+Copyright (c) 2024 Fluxional
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fluxional-0.1.3/README.md` & `fluxional-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # 🚀 AWS Serverless Development All In Python 🐍
 
+#### This is a work in progress. If you have any questions or need help, please reach out to us.
+
+<u>Join our discord community and give us feedback or ask questions:</u>
+
+[![Discord Shield](https://discordapp.com/api/guilds/1234210853574807668/widget.png?style=shield)](https://discord.gg/x8W4h5rT)
+
 <b class="theme-primary-light">Fluxional</b> is designed to simplify the development and deployment of serverless applications on AWS with <u>minimal</u> configuration.<br>
 
 Key features:<br>
 
 - Simplified infrastructure syntax
 - Deployment only require credentials and docker
 - Live interaction with your cloud application as you code
 - Focused on developer experience with intuitive syntax and editor / type support
+  <br>
 
-<br>
+Get started with:
+
+```bash
+
+pip install fluxional
+
+```
 
 <div class="index-title">1) Infrastructure is <u>simplified</u> and <u>part</u> of your code</div><br>
 
 😎 Rest API
 
 ```python
 from fluxional import Fluxional, ApiEvent, LambdaContext
@@ -130,17 +143,20 @@
 ```
 
 </div>
 
 <br>
 
 <div class="index-title"> 3) <u>Live Development</u>- Interact with your microservice as you code </div>
+
 - Invoke your microservice locally 💻 and make live changes 🕘 without the need to mock your services or re-deploy.
 - Your code will be ran in a local container with the exact ✨ environment and behaviors your application will have in the cloud.
 
+\*\* Setting must be <u>enabled</u> and <u>deployed</u> before executing below <br>
+
 <div>
 
 ```bash
 $ fluxional dev app.handler
 ```
 
 </div>
```

### Comparing `fluxional-0.1.3/fluxional/cli/__init__.py` & `fluxional-0.1.4/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/app.py` & `fluxional-0.1.4/fluxional/core/app.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/core.py` & `fluxional-0.1.4/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/events.py` & `fluxional-0.1.4/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/handlers.py` & `fluxional-0.1.4/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/infrastructure/base.py` & `fluxional-0.1.4/fluxional/core/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.4/fluxional/core/infrastructure/cdk.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.4/fluxional/core/infrastructure/resources.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/infrastructure/types.py` & `fluxional-0.1.4/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/logic.py` & `fluxional-0.1.4/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/settings.py` & `fluxional-0.1.4/fluxional/core/settings.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/tools.py` & `fluxional-0.1.4/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/core/types.py` & `fluxional-0.1.4/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/deployment/constants.py` & `fluxional-0.1.4/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/deployment/engine.py` & `fluxional-0.1.4/fluxional/deployment/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     default_aws_region,
     default_aws_secret_access_key,
     default_aws_access_key_id,
 )
 from rich.console import Console
 from rich import print as rp
 from typing import Any, Literal
+from fluxional import __version__
 import re
 
+
 load_dotenv()
 
 # Fix that will avoid using fileobject which does not allow
 # Context - IE: Imposible to copy files from host to container
 docker.api.build.process_dockerfile = lambda file, _: (
     "Dockerfile",
     file,
@@ -333,14 +335,20 @@
 
         if requirements_file:
             dockerfile += (
                 f"\nRUN pip install -r {requirements_file}"
                 # Needs to be escaped once for the echo cmd
                 + r' --target "\${LAMBDA_TASK_ROOT}"'
             )
+        else:
+            # We will always need fluxional installed
+            dockerfile += (
+                f"\nRUN pip install fluxional=={__version__}"
+                + r' --target "\${LAMBDA_TASK_ROOT}"'
+            )
 
         if include_otel:
             dockerfile += self.get_otel_steps()
 
         if include_fte:
             dockerfile += self.get_fte_steps()
```

### Comparing `fluxional-0.1.3/fluxional/dev/__init__.py` & `fluxional-0.1.4/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/dev/client.py` & `fluxional-0.1.4/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/dev/runner.py` & `fluxional-0.1.4/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/fluxional/utils.py` & `fluxional-0.1.4/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.3/pyproject.toml` & `fluxional-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
```

### Comparing `fluxional-0.1.3/PKG-INFO` & `fluxional-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -21,24 +21,37 @@
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # 🚀 AWS Serverless Development All In Python 🐍
 
+#### This is a work in progress. If you have any questions or need help, please reach out to us.
+
+<u>Join our discord community and give us feedback or ask questions:</u>
+
+[![Discord Shield](https://discordapp.com/api/guilds/1234210853574807668/widget.png?style=shield)](https://discord.gg/x8W4h5rT)
+
 <b class="theme-primary-light">Fluxional</b> is designed to simplify the development and deployment of serverless applications on AWS with <u>minimal</u> configuration.<br>
 
 Key features:<br>
 
 - Simplified infrastructure syntax
 - Deployment only require credentials and docker
 - Live interaction with your cloud application as you code
 - Focused on developer experience with intuitive syntax and editor / type support
+  <br>
 
-<br>
+Get started with:
+
+```bash
+
+pip install fluxional
+
+```
 
 <div class="index-title">1) Infrastructure is <u>simplified</u> and <u>part</u> of your code</div><br>
 
 😎 Rest API
 
 ```python
 from fluxional import Fluxional, ApiEvent, LambdaContext
@@ -155,17 +168,20 @@
 ```
 
 </div>
 
 <br>
 
 <div class="index-title"> 3) <u>Live Development</u>- Interact with your microservice as you code </div>
+
 - Invoke your microservice locally 💻 and make live changes 🕘 without the need to mock your services or re-deploy.
 - Your code will be ran in a local container with the exact ✨ environment and behaviors your application will have in the cloud.
 
+\*\* Setting must be <u>enabled</u> and <u>deployed</u> before executing below <br>
+
 <div>
 
 ```bash
 $ fluxional dev app.handler
 ```
 
 </div>
```

