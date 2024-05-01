# Comparing `tmp/bambot-0.3.9.tar.gz` & `tmp/bambot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.9.tar", last modified: Mon Apr 29 21:48:58 2024, max compression
+gzip compressed data, was "bambot-0.4.0.tar", last modified: Wed May  1 05:22:48 2024, max compression
```

## Comparing `bambot-0.3.9.tar` & `bambot-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 21:48:58.452133 bambot-0.3.9/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 21:48:58.451583 bambot-0.3.9/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-29 19:41:11.000000 bambot-0.3.9/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 21:48:58.448153 bambot-0.3.9/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7498 2024-04-29 21:40:57.000000 bambot-0.3.9/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     4937 2024-04-29 21:41:40.000000 bambot-0.3.9/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      708 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/logger.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2016 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/remote_utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 21:48:58.450589 bambot-0.3.9/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1103 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/templates/Dockerfile.dashboard.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1020 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/templates/Dockerfile.lightweight.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/templates/Procfile.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/templates/agent_readme.md.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      352 2024-04-29 21:38:53.000000 bambot-0.3.9/bambot/templates/bot.py.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/templates/dashboard.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      214 2024-04-29 21:46:10.000000 bambot-0.3.9/bambot/templates/run.sh.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-29 19:41:11.000000 bambot-0.3.9/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 21:48:58.451315 bambot-0.3.9/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      602 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       27 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 21:48:58.000000 bambot-0.3.9/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 21:48:58.452185 bambot-0.3.9/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1296 2024-04-29 21:48:06.000000 bambot-0.3.9/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 21:48:58.450972 bambot-0.3.9/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-29 19:41:11.000000 bambot-0.3.9/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:22:48.433166 bambot-0.4.0/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2148 2024-05-01 05:22:48.432950 bambot-0.4.0/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1217 2024-05-01 05:21:22.000000 bambot-0.4.0/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:22:48.429320 bambot-0.4.0/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3948 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     3326 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/container.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1241 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      196 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/logging.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      254 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/metrics.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      446 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/prometheus.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1125 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/streamlit_dashboard.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:22:48.431073 bambot-0.4.0/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      319 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/templates/Dockerfile
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      485 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/templates/agent_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      525 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/templates/langchain_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      150 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/templates/main.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       55 2024-05-01 04:48:56.000000 bambot-0.4.0/bambot/templates/requirements.txt
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:22:48.432727 bambot-0.4.0/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2148 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      690 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-01 05:22:48.000000 bambot-0.4.0/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-01 05:22:48.433200 bambot-0.4.0/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1248 2024-05-01 05:18:19.000000 bambot-0.4.0/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:22:48.432520 bambot-0.4.0/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      394 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      389 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_container.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      381 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_docker.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_logging.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_metrics.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      258 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_prometheus.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      307 2024-05-01 04:49:02.000000 bambot-0.4.0/tests/test_streamlit_dashboard.py
```

### Comparing `bambot-0.3.9/bambot.egg-info/SOURCES.txt` & `bambot-0.4.0/bambot.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 README.md
 setup.py
 bambot/__init__.py
-bambot/agent.py
 bambot/cli.py
+bambot/container.py
 bambot/docker_utils.py
-bambot/log_utils.py
-bambot/logger.py
-bambot/remote_utils.py
-bambot/utils.py
+bambot/logging.py
+bambot/metrics.py
+bambot/prometheus.py
+bambot/streamlit_dashboard.py
 bambot.egg-info/PKG-INFO
 bambot.egg-info/SOURCES.txt
 bambot.egg-info/dependency_links.txt
 bambot.egg-info/entry_points.txt
 bambot.egg-info/requires.txt
 bambot.egg-info/top_level.txt
-bambot/templates/Dockerfile.dashboard.j2
-bambot/templates/Dockerfile.lightweight.j2
-bambot/templates/Procfile.j2
-bambot/templates/agent_readme.md.j2
-bambot/templates/bot.py.j2
-bambot/templates/dashboard.py
-bambot/templates/run.sh.j2
-tests/test_bambot.py
+bambot/templates/Dockerfile
+bambot/templates/agent_template.py
+bambot/templates/langchain_template.py
+bambot/templates/main.py
+bambot/templates/requirements.txt
+tests/test_cli.py
+tests/test_container.py
+tests/test_docker.py
+tests/test_logging.py
+tests/test_metrics.py
+tests/test_prometheus.py
+tests/test_streamlit_dashboard.py
```

### Comparing `bambot-0.3.9/setup.py` & `bambot-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.3.9",
+    version="0.4.0",
     author="Bam Corp",
     author_email="spencer@bam.bot",
-    description="Lightweight containers for AI agents",
+    description="Containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/BamCorp/bambot",
+    url="https://github.com/Bam-Corp/bambot",
     packages=find_packages(),
-    package_data={
-        "bambot": ["templates/*"],
-    },
-    install_requires=[
-        "click",
-        "jinja2",
-        "tqdm",
-        "requests"
-    ],
+    package_data={'bambot': ['templates/*']},
+    install_requires=["click", "docker", "prometheus-client", "streamlit", "tqdm", "python-dotenv"],
     entry_points={
-        "console_scripts": [
-            "bam=bambot.cli:cli",
-        ],
+        "console_scripts": ["bam=bambot.cli:main"]
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

