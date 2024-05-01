# Comparing `tmp/clichatapp-0.1.0.tar.gz` & `tmp/clichatapp-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clichatapp-0.1.0.tar", max compression
+gzip compressed data, was "clichatapp-0.1.10.tar", max compression
```

## Comparing `clichatapp-0.1.0.tar` & `clichatapp-0.1.10.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-23 23:37:07.730804 clichatapp-0.1.0/clichatapp/__init__.py
--rw-r--r--   0        0        0       46 2024-04-23 23:56:07.006643 clichatapp-0.1.0/clichatapp/__main__.py
--rw-r--r--   0        0        0     1319 2024-04-23 23:52:41.247724 clichatapp-0.1.0/clichatapp/main.py
--rw-r--r--   0        0        0      474 2024-04-23 23:45:48.378027 clichatapp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 23:37:07.730804 clichatapp-0.1.0/README.md
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 clichatapp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 23:37:07.730804 clichatapp-0.1.10/clichatapp/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-23 23:56:07.006643 clichatapp-0.1.10/clichatapp/__main__.py
+-rw-r--r--   0        0        0     1690 2024-05-01 00:33:23.033607 clichatapp-0.1.10/clichatapp/main.py
+-rw-r--r--   0        0        0      509 2024-05-01 00:42:06.465712 clichatapp-0.1.10/pyproject.toml
+-rw-r--r--   0        0        0      575 2024-04-24 02:16:34.863944 clichatapp-0.1.10/README.md
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 clichatapp-0.1.10/PKG-INFO
```

