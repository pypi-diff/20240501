# Comparing `tmp/extensilog-0.0.1.tar.gz` & `tmp/extensilog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extensilog-0.0.1.tar", last modified: Wed May  1 15:00:32 2024, max compression
+gzip compressed data, was "extensilog-0.0.2.tar", last modified: Wed May  1 18:04:08 2024, max compression
```

## Comparing `extensilog-0.0.1.tar` & `extensilog-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:00:32.803946 extensilog-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-01 15:00:28.000000 extensilog-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 15:00:28.000000 extensilog-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-01 15:00:32.803946 extensilog-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 15:00:28.000000 extensilog-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:00:32.799946 extensilog-0.0.1/extensilog/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:00:32.803946 extensilog-0.0.1/extensilog/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/base_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/extensible_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/local_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/mongo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/connectors/postgres_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/extensilog.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-01 15:00:28.000000 extensilog-0.0.1/extensilog/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:00:32.803946 extensilog-0.0.1/extensilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-01 15:00:32.000000 extensilog-0.0.1/extensilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-01 15:00:32.000000 extensilog-0.0.1/extensilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:00:32.000000 extensilog-0.0.1/extensilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 15:00:32.000000 extensilog-0.0.1/extensilog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 15:00:32.000000 extensilog-0.0.1/extensilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 15:00:28.000000 extensilog-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:00:32.803946 extensilog-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-01 15:00:28.000000 extensilog-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.395032 extensilog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-01 18:04:02.000000 extensilog-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 18:04:02.000000 extensilog-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 18:04:08.395032 extensilog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-01 18:04:02.000000 extensilog-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.391032 extensilog-0.0.2/extensilog/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.391032 extensilog-0.0.2/extensilog/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/extensible_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/local_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/mongo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/postgres_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/extensilog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.395032 extensilog-0.0.2/extensilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:04:02.000000 extensilog-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:04:08.395032 extensilog-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 18:04:02.000000 extensilog-0.0.2/setup.py
```

### Comparing `extensilog-0.0.1/LICENSE` & `extensilog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/connectors/extensible_connector.py` & `extensilog-0.0.2/extensilog/connectors/extensible_connector.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/connectors/local_connector.py` & `extensilog-0.0.2/extensilog/connectors/local_connector.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/connectors/mongo_connector.py` & `extensilog-0.0.2/extensilog/connectors/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/connectors/postgres_connector.py` & `extensilog-0.0.2/extensilog/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/extensilog.py` & `extensilog-0.0.2/extensilog/extensilog.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog/singleton.py` & `extensilog-0.0.2/extensilog/singleton.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/extensilog.egg-info/SOURCES.txt` & `extensilog-0.0.2/extensilog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.1/setup.py` & `extensilog-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,19 @@
     required = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='extensilog',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(include=['extensilog', 'extensilog.*']),
     install_requires=required,
     long_description=long_description,
+    long_description_content_type='text/markdown',
     license='Apache License 2.0',
     author='Parth Sareen, Omkaar Kamath',
     author_email='parth@extensible.dev, omkaar@extensible.dev',
     description='A logger for tracking your agent workflow',
     url='https://github.com/Extensible-AI/extensilog/',
     classifiers=[
         'Programming Language :: Python :: 3',
```

