# Comparing `tmp/ext_message-1.0.0.tar.gz` & `tmp/ext_message-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext_message-1.0.0.tar", last modified: Wed May  1 00:31:15 2024, max compression
+gzip compressed data, was "ext_message-1.0.1.tar", last modified: Wed May  1 01:11:54 2024, max compression
```

## Comparing `ext_message-1.0.0.tar` & `ext_message-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:31:14.999902 ext_message-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 00:31:07.000000 ext_message-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 00:31:14.999902 ext_message-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 00:31:07.000000 ext_message-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:31:14.999902 ext_message-1.0.0/ext_message/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 00:31:07.000000 ext_message-1.0.0/ext_message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:31:14.999902 ext_message-1.0.0/ext_message.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 00:31:14.000000 ext_message-1.0.0/ext_message.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-01 00:31:14.000000 ext_message-1.0.0/ext_message.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:31:14.000000 ext_message-1.0.0/ext_message.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:31:14.000000 ext_message-1.0.0/ext_message.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 00:31:14.000000 ext_message-1.0.0/ext_message.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 00:31:14.999902 ext_message-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 00:31:07.000000 ext_message-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:11:54.714270 ext_message-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 01:11:50.000000 ext_message-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 01:11:54.714270 ext_message-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-01 01:11:50.000000 ext_message-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:11:54.710270 ext_message-1.0.1/ext_message/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 01:11:50.000000 ext_message-1.0.1/ext_message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:11:54.714270 ext_message-1.0.1/ext_message.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 01:11:54.000000 ext_message-1.0.1/ext_message.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-01 01:11:54.000000 ext_message-1.0.1/ext_message.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:11:54.000000 ext_message-1.0.1/ext_message.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 01:11:54.000000 ext_message-1.0.1/ext_message.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 01:11:54.000000 ext_message-1.0.1/ext_message.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 01:11:54.714270 ext_message-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 01:11:50.000000 ext_message-1.0.1/setup.py
```

### Comparing `ext_message-1.0.0/LICENSE` & `ext_message-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ext_message-1.0.0/ext_message/__init__.py` & `ext_message-1.0.1/ext_message/__init__.py`

 * *Files identical despite different names*

