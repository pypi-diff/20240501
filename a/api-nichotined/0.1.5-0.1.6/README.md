# Comparing `tmp/api-nichotined-0.1.5.tar.gz` & `tmp/api-nichotined-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-nichotined-0.1.5.tar", last modified: Fri Apr 26 18:09:45 2024, max compression
+gzip compressed data, was "api-nichotined-0.1.6.tar", last modified: Wed May  1 15:40:59 2024, max compression
```

## Comparing `api-nichotined-0.1.5.tar` & `api-nichotined-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 18:09:45.913606 api-nichotined-0.1.5/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 18:09:45.913336 api-nichotined-0.1.5/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      648 2024-04-19 16:19:11.000000 api-nichotined-0.1.5/README.md
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 18:09:45.911028 api-nichotined-0.1.5/api_nichotined/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       65 2024-04-26 10:16:58.000000 api-nichotined-0.1.5/api_nichotined/__init__.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 18:09:45.912267 api-nichotined-0.1.5/api_nichotined/core/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.5/api_nichotined/core/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2065 2024-04-26 18:08:38.000000 api-nichotined-0.1.5/api_nichotined/core/core.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 18:09:45.913032 api-nichotined-0.1.5/api_nichotined.egg-info/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1112 2024-04-26 18:09:45.000000 api-nichotined-0.1.5/api_nichotined.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      324 2024-04-26 18:09:45.000000 api-nichotined-0.1.5/api_nichotined.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-04-26 18:09:45.000000 api-nichotined-0.1.5/api_nichotined.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       17 2024-04-26 18:09:45.000000 api-nichotined-0.1.5/api_nichotined.egg-info/requires.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-04-26 18:09:45.000000 api-nichotined-0.1.5/api_nichotined.egg-info/top_level.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-04-26 18:09:45.913661 api-nichotined-0.1.5/setup.cfg
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      718 2024-04-26 18:09:37.000000 api-nichotined-0.1.5/setup.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-26 18:09:45.912673 api-nichotined-0.1.5/test/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.5/test/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      451 2024-04-26 10:35:06.000000 api-nichotined-0.1.5/test/main.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.328382 api-nichotined-0.1.6/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-01 15:40:59.328137 api-nichotined-0.1.6/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      877 2024-05-01 15:39:36.000000 api-nichotined-0.1.6/README.md
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.324844 api-nichotined-0.1.6/api_nichotined/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      206 2024-05-01 15:37:42.000000 api-nichotined-0.1.6/api_nichotined/__init__.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.326315 api-nichotined-0.1.6/api_nichotined/core/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.6/api_nichotined/core/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2065 2024-04-26 18:28:12.000000 api-nichotined-0.1.6/api_nichotined/core/core.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       92 2024-04-26 18:28:45.000000 api-nichotined-0.1.6/api_nichotined/core/hook.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327091 api-nichotined-0.1.6/api_nichotined/utillity/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-27 13:10:31.000000 api-nichotined-0.1.6/api_nichotined/utillity/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1375 2024-05-01 12:24:28.000000 api-nichotined-0.1.6/api_nichotined/utillity/bq.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       53 2024-04-27 13:11:27.000000 api-nichotined-0.1.6/api_nichotined/utillity/pq.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327855 api-nichotined-0.1.6/api_nichotined.egg-info/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      448 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       39 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/requires.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/top_level.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-05-01 15:40:59.328441 api-nichotined-0.1.6/setup.cfg
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      750 2024-05-01 15:40:31.000000 api-nichotined-0.1.6/setup.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327511 api-nichotined-0.1.6/test/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.6/test/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      685 2024-05-01 15:39:33.000000 api-nichotined-0.1.6/test/main.py
```

### Comparing `api-nichotined-0.1.5/api_nichotined/core/core.py` & `api-nichotined-0.1.6/api_nichotined/core/core.py`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.5/setup.py` & `api-nichotined-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="api-nichotined",
-    version="0.1.5",
+    version="0.1.6",
     author="Nicholas Frederich",
     author_email="nicholas.frederich.lagaunne@gmail.com",
     description="Simple lib for testing rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nichotined/simple-api",
     packages=setuptools.find_packages(),
     install_requires=[
         'requests',
         'curlify',
+        'google-cloud-bigquery'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

