# Comparing `tmp/de_databaseconnect-0.0.77.tar.gz` & `tmp/DE_DataBaseConnect-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de_databaseconnect-0.0.77.tar", max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.80.tar", last modified: Wed May  1 13:57:12 2024, max compression
```

## Comparing `de_databaseconnect-0.0.77.tar` & `DE_DataBaseConnect-0.0.80.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0        0 2024-04-30 18:24:30.466226 de_databaseconnect-0.0.77/DE_DataBaseConnect/de_databaseconnect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 18:24:30.473208 de_databaseconnect-0.0.77/DE_DataBaseConnect/README.md
--rw-r--r--   0        0        0        0 2024-04-30 18:24:30.479194 de_databaseconnect-0.0.77/DE_DataBaseConnect/tests/__init__.py
--rw-r--r--   0        0        0     1088 2022-08-23 21:32:43.000000 de_databaseconnect-0.0.77/Licence.txt
--rw-r--r--   0        0        0      292 2024-04-30 18:51:21.273282 de_databaseconnect-0.0.77/pyproject.toml
--rw-r--r--   0        0        0      829 2022-08-23 21:32:43.000000 de_databaseconnect-0.0.77/README.md
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 de_databaseconnect-0.0.77/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 13:57:12.366582 DE_DataBaseConnect-0.0.80/
+-rw-rw-rw-   0        0        0    19082 2024-04-30 19:25:32.000000 DE_DataBaseConnect-0.0.80/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:57:12.354614 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0     1210 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.80/Licence.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-01 13:57:12.367580 DE_DataBaseConnect-0.0.80/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.80/README.md
+-rw-rw-rw-   0        0        0      292 2024-04-30 19:05:16.000000 DE_DataBaseConnect-0.0.80/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 13:57:12.379546 DE_DataBaseConnect-0.0.80/setup.cfg
+-rw-rw-rw-   0        0        0      688 2024-05-01 13:57:07.000000 DE_DataBaseConnect-0.0.80/setup.py
```

### Comparing `de_databaseconnect-0.0.77/Licence.txt` & `DE_DataBaseConnect-0.0.80/Licence.txt`

 * *Files identical despite different names*

### Comparing `de_databaseconnect-0.0.77/README.md` & `DE_DataBaseConnect-0.0.80/README.md`

 * *Files identical despite different names*

