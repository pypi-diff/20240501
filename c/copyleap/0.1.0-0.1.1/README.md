# Comparing `tmp/copyleap-0.1.0.tar.gz` & `tmp/copyleap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyleap-0.1.0.tar", max compression
+gzip compressed data, was "copyleap-0.1.1.tar", max compression
```

## Comparing `copyleap-0.1.0.tar` & `copyleap-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-30 22:05:51.721255 copyleap-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 22:05:51.720909 copyleap-0.1.0/copyleap/__init__.py
--rw-r--r--   0        0        0      266 2024-04-30 22:06:58.744105 copyleap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 copyleap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-30 22:05:51.721255 copyleap-0.1.1/README.md
+-rw-r--r--   0        0        0       40 2024-04-30 23:40:21.033097 copyleap-0.1.1/copyleap/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-30 23:53:59.585691 copyleap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 copyleap-0.1.1/PKG-INFO
```

