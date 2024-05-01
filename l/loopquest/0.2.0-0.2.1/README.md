# Comparing `tmp/loopquest-0.2.0.tar.gz` & `tmp/loopquest-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.0.tar", last modified: Mon Apr 29 07:03:08 2024, max compression
+gzip compressed data, was "loopquest-0.2.1.tar", last modified: Wed May  1 06:20:38 2024, max compression
```

## Comparing `loopquest-0.2.0.tar` & `loopquest-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.0/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     5944 2024-04-29 07:03:08.142345 loopquest-0.2.0/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     3360 2024-04-19 04:42:45.000000 loopquest-0.2.0/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.0/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.0/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9075 2024-04-28 15:10:40.000000 loopquest-0.2.0/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/datasets.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.0/loopquest/eval.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1994 2024-04-24 04:19:39.000000 loopquest-0.2.0/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.0/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.0/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4216 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     5944 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      459 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1175 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-04-29 07:03:08.142345 loopquest-0.2.0/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      946 2024-04-29 07:01:19.000000 loopquest-0.2.0/setup.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/tests/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1397 2024-04-19 04:43:26.000000 loopquest-0.2.0/tests/test_datasets.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4677 2024-04-19 04:42:45.000000 loopquest-0.2.0/tests/test_performance.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      832 2024-04-19 04:42:45.000000 loopquest-0.2.0/tests/test_wrappers.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.614737 loopquest-0.2.1/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.1/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-01 06:20:38.614737 loopquest-0.2.1/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.1/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.1/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.1/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9075 2024-04-28 15:10:40.000000 loopquest-0.2.1/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.1/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4217 2024-04-29 05:10:05.000000 loopquest-0.2.1/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5767 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.1/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      173 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1994 2024-04-24 04:19:39.000000 loopquest-0.2.1/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.1/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.1/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4216 2024-04-19 04:43:26.000000 loopquest-0.2.1/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 06:20:38.610737 loopquest-0.2.1/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-01 06:20:38.000000 loopquest-0.2.1/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-01 06:20:38.614737 loopquest-0.2.1/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-01 06:20:16.000000 loopquest-0.2.1/setup.py
```

### Comparing `loopquest-0.2.0/LICENSE` & `loopquest-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/api.py` & `loopquest-0.2.1/loopquest/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/crud.py` & `loopquest-0.2.1/loopquest/crud.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/datasets.py` & `loopquest-0.2.1/loopquest/datasets.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/eval.py` & `loopquest-0.2.1/loopquest/eval.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/private_api.py` & `loopquest-0.2.1/loopquest/private_api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/schema.py` & `loopquest-0.2.1/loopquest/schema.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/loopquest/utils.py` & `loopquest-0.2.1/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.0/setup.py` & `loopquest-0.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 
-def parse_requirements(filename):
-    """Load requirements from a pip requirements file."""
-    with open(filename) as f:
-        lineiter = (line.strip() for line in f)
-        return [line for line in lineiter if line and not line.startswith("#")]
-
-
-reqs = parse_requirements("requirements.txt")
-
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.0",
+    version="0.2.1",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
-    packages=["loopquest"],
-    install_requires=reqs,
+    packages=find_packages(),
+    install_requires=[
+        "gymnasium>=0.29.0",
+        "huggingface-hub>=0.16.4",
+        "datasets>=2.14.4",
+        "python-dotenv>=1.0.0",
+        "stable-baselines3>=2.2.1",
+        "huggingface-sb3>=3.0",
+        "pydantic>=2.1.1",
+    ],
+    extras_require={
+        "dev": ["pytest", "twine"],
+        "rl": ["ale_py>=0.8", "box2d-py==2.3.5", "pygame>=2.1.3", "swig==4.*"],
+        "mujoco-py": ["mujoco-py>=2.1,<2.2", "cython<3"],
+        "mujoco": ["mujoco>=2.1.5", "imageio>=2.14.1"],
+    },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

