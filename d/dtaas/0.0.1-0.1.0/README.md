# Comparing `tmp/dtaas-0.0.1.tar.gz` & `tmp/dtaas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtaas-0.0.1.tar", max compression
+gzip compressed data, was "dtaas-0.1.0.tar", max compression
```

## Comparing `dtaas-0.0.1.tar` & `dtaas-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    13794 2024-03-11 08:44:09.322934 dtaas-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      102 2024-03-11 09:15:12.725483 dtaas-0.0.1/README.md
--rw-r--r--   0        0        0      352 2024-03-11 09:16:39.316991 dtaas-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-11 08:35:17.648933 dtaas-0.0.1/src/dtaas/__init__.py
--rw-r--r--   0        0        0       85 2024-03-11 09:15:30.602213 dtaas-0.0.1/src/dtaas/main.py
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 dtaas-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3317 2024-05-01 16:20:25.983763 dtaas-0.1.0/README.md
+-rw-r--r--   0        0        0      504 2024-05-01 16:34:37.850569 dtaas-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 19:29:22.222017 dtaas-0.1.0/src/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-27 19:29:22.222017 dtaas-0.1.0/src/cmd.py
+-rw-r--r--   0        0        0     2819 2024-04-27 20:43:16.791160 dtaas-0.1.0/src/pkg/config.py
+-rw-r--r--   0        0        0     3888 2024-04-27 22:15:13.778512 dtaas-0.1.0/src/pkg/users.py
+-rw-r--r--   0        0        0     2424 2024-04-27 20:10:50.088341 dtaas-0.1.0/src/pkg/utils.py
+-rw-r--r--   0        0        0     4027 1970-01-01 00:00:00.000000 dtaas-0.1.0/PKG-INFO
```

