# Comparing `tmp/youtubeuser-1.0.2.tar.gz` & `tmp/youtubeuser-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeuser-1.0.2.tar", last modified: Mon Apr 29 08:38:41 2024, max compression
+gzip compressed data, was "youtubeuser-1.2.2.tar", last modified: Wed May  1 11:36:36 2024, max compression
```

## Comparing `youtubeuser-1.0.2.tar` & `youtubeuser-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 08:38:41.870609 youtubeuser-1.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 08:38:41.870609 youtubeuser-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-29 08:38:19.000000 youtubeuser-1.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 08:38:41.870609 youtubeuser-1.0.2/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 08:38:41.000000 youtubeuser-1.0.2/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-04-29 08:38:41.000000 youtubeuser-1.0.2/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-29 08:38:41.000000 youtubeuser-1.0.2/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-29 08:38:41.000000 youtubeuser-1.0.2/YoutubeUser.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-29 08:38:41.000000 youtubeuser-1.0.2/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      649 2024-04-29 08:32:06.000000 youtubeuser-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-29 08:38:41.870609 youtubeuser-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      735 2024-04-29 08:36:32.000000 youtubeuser-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 08:38:41.870609 youtubeuser-1.0.2/youtubeuser/
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-29 01:30:46.000000 youtubeuser-1.0.2/youtubeuser/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      759 2024-04-29 08:32:19.000000 youtubeuser-1.0.2/youtubeuser/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 11:36:36.251626 youtubeuser-1.2.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-05-01 11:36:36.251626 youtubeuser-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-29 08:38:19.000000 youtubeuser-1.2.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 11:36:36.251626 youtubeuser-1.2.2/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-05-01 11:36:35.000000 youtubeuser-1.2.2/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-05-01 11:36:36.000000 youtubeuser-1.2.2/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-01 11:36:35.000000 youtubeuser-1.2.2/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-05-01 11:36:35.000000 youtubeuser-1.2.2/YoutubeUser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-05-01 11:36:35.000000 youtubeuser-1.2.2/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      649 2024-05-01 11:36:01.000000 youtubeuser-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-01 11:36:36.251626 youtubeuser-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      735 2024-05-01 11:36:07.000000 youtubeuser-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 11:36:36.251626 youtubeuser-1.2.2/youtubeuser/
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-29 01:30:46.000000 youtubeuser-1.2.2/youtubeuser/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      889 2024-05-01 11:35:37.000000 youtubeuser-1.2.2/youtubeuser/user.py
```

### Comparing `youtubeuser-1.0.2/pyproject.toml` & `youtubeuser-1.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YoutubeUser"
-version = "1.0.2"
+version = "1.2.2"
 description = "A Lib For Search Youtube Channels Or User"
 authors = ["R1TGAMING"]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12"
 requests = "^2.31.0"
 setuptools = "^69.5.1"
```

### Comparing `youtubeuser-1.0.2/setup.py` & `youtubeuser-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
   
 setup(
     name="YoutubeUser",
-    version='1.0.2',
+    version='1.2.2',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
     long_description=long_description,
     long_description_content_type='text/markdown',
    url='https://github.com/R1TGAMING/YoutubeUser',
     packages=["youtubeuser"],
```

