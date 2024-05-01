# Comparing `tmp/socketsecurity-0.0.39.tar.gz` & `tmp/socketsecurity-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.39.tar", last modified: Wed May  1 08:34:36 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.40.tar", last modified: Wed May  1 08:46:55 2024, max compression
```

## Comparing `socketsecurity-0.0.39.tar` & `socketsecurity-0.0.40.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:34:36.317931 socketsecurity-0.0.39/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:34:36.317629 socketsecurity-0.0.39/PKG-INFO
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:34:36.316653 socketsecurity-0.0.39/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    23060 2024-05-01 07:25:53.000000 socketsecurity-0.0.39/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     8053 2024-05-01 07:24:43.000000 socketsecurity-0.0.39/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-05-01 06:00:20.000000 socketsecurity-0.0.39/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11580 2024-05-01 06:39:19.000000 socketsecurity-0.0.39/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-01 08:34:36.317998 socketsecurity-0.0.39/setup.cfg
--rw-r--r--   0 douglascoburn   (501) staff       (20)      346 2024-05-01 08:34:06.000000 socketsecurity-0.0.39/setup.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:34:36.317363 socketsecurity-0.0.39/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      307 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       35 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        5 2024-05-01 08:34:36.000000 socketsecurity-0.0.39/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:46:55.144164 socketsecurity-0.0.40/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:46:55.144019 socketsecurity-0.0.40/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-01 08:46:55.144206 socketsecurity-0.0.40/setup.cfg
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      347 2024-05-01 08:46:48.000000 socketsecurity-0.0.40/setup.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:46:55.143859 socketsecurity-0.0.40/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      238 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       35 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-01 08:46:55.000000 socketsecurity-0.0.40/socketsecurity.egg-info/top_level.txt
```

