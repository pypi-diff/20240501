# Comparing `tmp/runware-0.1.2.tar.gz` & `tmp/runware-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runware-0.1.2.tar", last modified: Wed May  1 18:39:30 2024, max compression
+gzip compressed data, was "runware-0.1.3.tar", last modified: Wed May  1 18:40:15 2024, max compression
```

## Comparing `runware-0.1.2.tar` & `runware-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:30.130321 runware-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:26.000000 runware-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-01 18:39:30.130321 runware-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-01 18:39:26.000000 runware-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:30.126320 runware-0.1.2/runware/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-01 18:39:26.000000 runware-0.1.2/runware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-01 18:39:26.000000 runware-0.1.2/runware/async_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31484 2024-05-01 18:39:26.000000 runware-0.1.2/runware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-01 18:39:26.000000 runware-0.1.2/runware/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-01 18:39:26.000000 runware-0.1.2/runware/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-01 18:39:26.000000 runware-0.1.2/runware/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-05-01 18:39:26.000000 runware-0.1.2/runware/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:30.130321 runware-0.1.2/runware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-01 18:39:30.000000 runware-0.1.2/runware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-01 18:39:30.000000 runware-0.1.2/runware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:39:30.000000 runware-0.1.2/runware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 18:39:30.000000 runware-0.1.2/runware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 18:39:30.000000 runware-0.1.2/runware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:39:30.130321 runware-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-01 18:39:26.000000 runware-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:30.130321 runware-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:26.000000 runware-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:26.000000 runware-0.1.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:26.000000 runware-0.1.2/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-05-01 18:39:26.000000 runware-0.1.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-01 18:39:26.000000 runware-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:15.365671 runware-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:11.000000 runware-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-01 18:40:15.365671 runware-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-01 18:40:11.000000 runware-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:15.361672 runware-0.1.3/runware/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-01 18:40:11.000000 runware-0.1.3/runware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-01 18:40:11.000000 runware-0.1.3/runware/async_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31484 2024-05-01 18:40:11.000000 runware-0.1.3/runware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-01 18:40:11.000000 runware-0.1.3/runware/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-01 18:40:11.000000 runware-0.1.3/runware/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-01 18:40:11.000000 runware-0.1.3/runware/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-05-01 18:40:11.000000 runware-0.1.3/runware/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:15.365671 runware-0.1.3/runware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-01 18:40:15.000000 runware-0.1.3/runware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-01 18:40:15.000000 runware-0.1.3/runware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:40:15.000000 runware-0.1.3/runware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 18:40:15.000000 runware-0.1.3/runware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 18:40:15.000000 runware-0.1.3/runware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:40:15.365671 runware-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-01 18:40:11.000000 runware-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:15.365671 runware-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:11.000000 runware-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:11.000000 runware-0.1.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:11.000000 runware-0.1.3/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-05-01 18:40:11.000000 runware-0.1.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-01 18:40:11.000000 runware-0.1.3/tests/test_utils.py
```

### Comparing `runware-0.1.2/PKG-INFO` & `runware-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runware
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python Runware SDK is used to run image inference with the Runware API, powered by the RunWare inference platform. It can be used to generate imaged with text-to-image and image-to-image. It also allows the use of an existing gallery of models or selecting any model or LoRA from the CivitAI gallery. The API also supports upscaling, background removal, inpainting and outpainting, and a series of other ControlNet models.
 Home-page: https://github.com/runware/sdk-python
 Author: Runware Inc.
 Author-email: python.sdk@runware.ai
 License: MIT
 Project-URL: Documentation, https://docs.runware.ai/
 Project-URL: Changes, https://github.com/runware/sdk-python/releases
```

### Comparing `runware-0.1.2/README.md` & `runware-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/async_retry.py` & `runware-0.1.3/runware/async_retry.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/base.py` & `runware-0.1.3/runware/base.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/logging_config.py` & `runware-0.1.3/runware/logging_config.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/server.py` & `runware-0.1.3/runware/server.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/types.py` & `runware-0.1.3/runware/types.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware/utils.py` & `runware-0.1.3/runware/utils.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/runware.egg-info/PKG-INFO` & `runware-0.1.3/runware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runware
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python Runware SDK is used to run image inference with the Runware API, powered by the RunWare inference platform. It can be used to generate imaged with text-to-image and image-to-image. It also allows the use of an existing gallery of models or selecting any model or LoRA from the CivitAI gallery. The API also supports upscaling, background removal, inpainting and outpainting, and a series of other ControlNet models.
 Home-page: https://github.com/runware/sdk-python
 Author: Runware Inc.
 Author-email: python.sdk@runware.ai
 License: MIT
 Project-URL: Documentation, https://docs.runware.ai/
 Project-URL: Changes, https://github.com/runware/sdk-python/releases
```

### Comparing `runware-0.1.2/setup.py` & `runware-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="runware",
     license="MIT",
-    version="0.1.2",
+    version="0.1.3",
     author="Runware Inc.",
     author_email="python.sdk@runware.ai",
     description="The Python Runware SDK is used to run image inference with the Runware API, powered by the RunWare inference platform. It can be used to generate imaged with text-to-image and image-to-image. It also allows the use of an existing gallery of models or selecting any model or LoRA from the CivitAI gallery. The API also supports upscaling, background removal, inpainting and outpainting, and a series of other ControlNet models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["Runware", "stable diffusion", "text to image", "image to text"],
     url="https://github.com/runware/sdk-python",
```

### Comparing `runware-0.1.2/tests/test_types.py` & `runware-0.1.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `runware-0.1.2/tests/test_utils.py` & `runware-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

