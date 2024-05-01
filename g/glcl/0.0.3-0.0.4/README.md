# Comparing `tmp/glcl-0.0.3.tar.gz` & `tmp/glcl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\glcl-0.0.3.tar", last modified: Tue Apr 30 23:59:09 2024, max compression
+gzip compressed data, was "dist\glcl-0.0.4.tar", last modified: Wed May  1 01:18:13 2024, max compression
```

## Comparing `glcl-0.0.3.tar` & `glcl-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.249532 glcl-0.0.3/
--rw-rw-rw-   0        0        0       86 2024-04-30 23:59:07.000000 glcl-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      840 2024-04-30 23:59:09.249532 glcl-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.124732 glcl-0.0.3/glcl/
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.140332 glcl-0.0.3/glcl/Win32/
--rw-rw-rw-   0        0        0  6138880 2024-04-30 23:13:37.000000 glcl-0.0.3/glcl/Win32/glcl.pyd
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.155932 glcl-0.0.3/glcl/Win64/
--rw-rw-rw-   0        0        0  9771520 2024-04-30 23:14:30.000000 glcl-0.0.3/glcl/Win64/glcl.pyd
--rw-rw-rw-   0        0        0     1793 2024-04-30 23:06:42.000000 glcl-0.0.3/glcl/__init__.py
--rw-rw-rw-   0        0        0  1888021 2024-04-30 21:40:10.000000 glcl-0.0.3/glcl/__init__.pyi
--rw-rw-rw-   0        0        0      282 2024-04-30 23:08:15.000000 glcl-0.0.3/glcl/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.233932 glcl-0.0.3/glcl/doc/
--rw-rw-rw-   0        0        0  1465315 2024-04-17 05:13:09.000000 glcl-0.0.3/glcl/doc/docs.xml
-drwxrwxrwx   0        0        0        0 2024-04-30 23:59:09.140332 glcl-0.0.3/glcl.egg-info/
--rw-rw-rw-   0        0        0      840 2024-04-30 23:59:09.000000 glcl-0.0.3/glcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-30 23:59:09.000000 glcl-0.0.3/glcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 23:59:09.000000 glcl-0.0.3/glcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-30 23:59:09.000000 glcl-0.0.3/glcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 23:59:09.249532 glcl-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1307 2024-04-30 23:54:49.000000 glcl-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/
+-rw-rw-rw-   0        0        0     1027 2024-05-01 01:18:13.677758 glcl-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/glcl/
+-rw-rw-rw-   0        0        0        0 2024-05-01 01:12:19.000000 glcl-0.0.4/glcl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 01:18:13.677758 glcl-0.0.4/glcl.egg-info/
+-rw-rw-rw-   0        0        0     1027 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 01:18:13.000000 glcl-0.0.4/glcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 01:18:13.677758 glcl-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2024-05-01 01:12:19.000000 glcl-0.0.4/setup.py
```

