# Comparing `tmp/gitdata-lib-0.0.8.tar.gz` & `tmp/gitdata-lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitdata-lib-0.0.8.tar", last modified: Tue Nov 23 17:17:24 2021, max compression
+gzip compressed data, was "dist/gitdata-lib-0.0.9.tar", last modified: Tue Nov 23 19:44:54 2021, max compression
```

## Comparing `gitdata-lib-0.0.8.tar` & `gitdata-lib-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/
--rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-10-14 22:45:21.000000 gitdata-lib-0.0.8/CHANGELOG.md
--rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-10-14 22:45:33.000000 gitdata-lib-0.0.8/LICENSE
--rw-rw-r--   0 herb      (1000) herb      (1000)      226 2021-10-14 22:45:55.000000 gitdata-lib-0.0.8/MANIFEST.in
--rw-rw-r--   0 herb      (1000) herb      (1000)     1155 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/PKG-INFO
--rw-rw-r--   0 herb      (1000) herb      (1000)      238 2021-06-16 02:00:03.000000 gitdata-lib-0.0.8/README.md
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/
--rw-rw-r--   0 herb      (1000) herb      (1000)      484 2021-10-21 06:16:11.000000 gitdata-lib-0.0.8/gitdata/__init__.py
--rw-rw-r--   0 herb      (1000) herb      (1000)       21 2021-11-22 17:10:51.000000 gitdata-lib-0.0.8/gitdata/__version__.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/assets/
--rw-rw-r--   0 herb      (1000) herb      (1000)       16 2021-06-30 17:14:47.000000 gitdata-lib-0.0.8/gitdata/assets/README.md
--rw-r--r--   0 herb      (1000) herb      (1000)     3207 2021-08-06 15:30:58.000000 gitdata-lib-0.0.8/gitdata/buckets.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/cli/
--rw-rw-r--   0 herb      (1000) herb      (1000)      864 2021-10-11 15:34:16.000000 gitdata-lib-0.0.8/gitdata/cli/__init__.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     6045 2021-08-06 15:09:45.000000 gitdata-lib-0.0.8/gitdata/config.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/connectors/
--rw-r--r--   0 herb      (1000) herb      (1000)       61 2021-11-13 18:32:58.000000 gitdata-lib-0.0.8/gitdata/connectors/__init__.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     3179 2021-09-28 03:27:21.000000 gitdata-lib-0.0.8/gitdata/connectors/common.py
--rw-r--r--   0 herb      (1000) herb      (1000)      292 2021-08-12 16:25:14.000000 gitdata-lib-0.0.8/gitdata/connectors/console.py
--rw-r--r--   0 herb      (1000) herb      (1000)      533 2021-09-27 22:30:58.000000 gitdata-lib-0.0.8/gitdata/connectors/csv.py
--rw-r--r--   0 herb      (1000) herb      (1000)     1577 2021-08-25 16:17:20.000000 gitdata-lib-0.0.8/gitdata/connectors/gitlab.py
--rw-rw-r--   0 herb      (1000) herb      (1000)      405 2021-10-11 19:42:22.000000 gitdata-lib-0.0.8/gitdata/connectors/http.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     1532 2021-08-11 21:20:11.000000 gitdata-lib-0.0.8/gitdata/connectors/json.py
--rw-r--r--   0 herb      (1000) herb      (1000)      816 2021-08-11 18:42:51.000000 gitdata-lib-0.0.8/gitdata/connectors/local.py
--rw-r--r--   0 herb      (1000) herb      (1000)      783 2021-08-11 18:42:35.000000 gitdata-lib-0.0.8/gitdata/connectors/location.py
--rw-r--r--   0 herb      (1000) herb      (1000)      192 2021-08-11 21:20:11.000000 gitdata-lib-0.0.8/gitdata/connectors/rows.py
--rw-rw-r--   0 herb      (1000) herb      (1000)      447 2021-09-28 03:27:12.000000 gitdata-lib-0.0.8/gitdata/connectors/system.py
--rw-r--r--   0 herb      (1000) herb      (1000)      268 2021-08-11 18:47:03.000000 gitdata-lib-0.0.8/gitdata/connectors/zip.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/database/
--rw-rw-r--   0 herb      (1000) herb      (1000)     1970 2021-11-23 16:08:09.000000 gitdata-lib-0.0.8/gitdata/database/__init__.py
--rw-rw-r--   0 herb      (1000) herb      (1000)    12192 2021-11-23 17:09:01.000000 gitdata-lib-0.0.8/gitdata/database/common.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     2395 2021-10-10 23:23:51.000000 gitdata-lib-0.0.8/gitdata/database/mysql.py
--rw-rw-r--   0 herb      (1000) herb      (1000)      263 2021-07-06 14:15:29.000000 gitdata-lib-0.0.8/gitdata/database/mysql_setup_test_database.sql
--rw-rw-r--   0 herb      (1000) herb      (1000)     2235 2021-11-13 17:33:58.000000 gitdata-lib-0.0.8/gitdata/database/postgresql.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     2486 2021-10-23 17:08:35.000000 gitdata-lib-0.0.8/gitdata/database/sqlite3.py
--rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-07-05 05:19:19.000000 gitdata-lib-0.0.8/gitdata/database/sqlite3_setup.sql
--rw-rw-r--   0 herb      (1000) herb      (1000)      855 2021-07-05 05:21:27.000000 gitdata-lib-0.0.8/gitdata/database/sqlite3_setup_test_data.sql
--rw-rw-r--   0 herb      (1000) herb      (1000)     1857 2021-07-06 03:44:00.000000 gitdata-lib-0.0.8/gitdata/json.py
--rw-r--r--   0 herb      (1000) herb      (1000)    16796 2021-10-22 08:04:45.000000 gitdata-lib-0.0.8/gitdata/queues.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     4387 2021-08-12 16:29:48.000000 gitdata-lib-0.0.8/gitdata/solutions.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata/stores/
--rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-07-16 18:08:53.000000 gitdata-lib-0.0.8/gitdata/stores/__init__.py
--rw-rw-r--   0 herb      (1000) herb      (1000)     3690 2021-07-16 18:06:49.000000 gitdata-lib-0.0.8/gitdata/stores/common.py
--rw-rw-r--   0 herb      (1000) herb      (1000)    28846 2021-10-23 17:05:35.000000 gitdata-lib-0.0.8/gitdata/stores/entities.py
--rw-rw-r--   0 herb      (1000) herb      (1000)      694 2021-10-14 21:19:38.000000 gitdata-lib-0.0.8/gitdata/stores/entity_store.sql
--rw-rw-r--   0 herb      (1000) herb      (1000)    23238 2021-10-23 17:09:37.000000 gitdata-lib-0.0.8/gitdata/stores/records.py
--rw-rw-r--   0 herb      (1000) herb      (1000)    20613 2021-11-23 17:12:14.000000 gitdata-lib-0.0.8/gitdata/utils.py
-drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/
--rw-rw-r--   0 herb      (1000) herb      (1000)     1155 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 herb      (1000) herb      (1000)     1226 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)        1 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)       46 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/entry_points.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)      103 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/requires.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)        8 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/gitdata_lib.egg-info/top_level.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)      102 2021-11-05 21:06:47.000000 gitdata-lib-0.0.8/requirements.txt
--rw-rw-r--   0 herb      (1000) herb      (1000)       38 2021-11-23 17:17:24.000000 gitdata-lib-0.0.8/setup.cfg
--rw-r--r--   0 herb      (1000) herb      (1000)     1613 2021-10-14 22:59:26.000000 gitdata-lib-0.0.8/setup.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/
+-rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-10-14 22:45:21.000000 gitdata-lib-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-10-14 22:45:33.000000 gitdata-lib-0.0.9/LICENSE
+-rw-rw-r--   0 herb      (1000) herb      (1000)      226 2021-10-14 22:45:55.000000 gitdata-lib-0.0.9/MANIFEST.in
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1155 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/PKG-INFO
+-rw-rw-r--   0 herb      (1000) herb      (1000)      238 2021-06-16 02:00:03.000000 gitdata-lib-0.0.9/README.md
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/
+-rw-rw-r--   0 herb      (1000) herb      (1000)      484 2021-10-21 06:16:11.000000 gitdata-lib-0.0.9/gitdata/__init__.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)       21 2021-11-23 19:44:33.000000 gitdata-lib-0.0.9/gitdata/__version__.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/assets/
+-rw-rw-r--   0 herb      (1000) herb      (1000)       16 2021-06-30 17:14:47.000000 gitdata-lib-0.0.9/gitdata/assets/README.md
+-rw-r--r--   0 herb      (1000) herb      (1000)     3207 2021-08-06 15:30:58.000000 gitdata-lib-0.0.9/gitdata/buckets.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/cli/
+-rw-rw-r--   0 herb      (1000) herb      (1000)      864 2021-10-11 15:34:16.000000 gitdata-lib-0.0.9/gitdata/cli/__init__.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     6045 2021-08-06 15:09:45.000000 gitdata-lib-0.0.9/gitdata/config.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/connectors/
+-rw-r--r--   0 herb      (1000) herb      (1000)       61 2021-11-13 18:32:58.000000 gitdata-lib-0.0.9/gitdata/connectors/__init__.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     3179 2021-09-28 03:27:21.000000 gitdata-lib-0.0.9/gitdata/connectors/common.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      292 2021-08-12 16:25:14.000000 gitdata-lib-0.0.9/gitdata/connectors/console.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      533 2021-09-27 22:30:58.000000 gitdata-lib-0.0.9/gitdata/connectors/csv.py
+-rw-r--r--   0 herb      (1000) herb      (1000)     1577 2021-08-25 16:17:20.000000 gitdata-lib-0.0.9/gitdata/connectors/gitlab.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)      405 2021-10-11 19:42:22.000000 gitdata-lib-0.0.9/gitdata/connectors/http.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1532 2021-08-11 21:20:11.000000 gitdata-lib-0.0.9/gitdata/connectors/json.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      816 2021-08-11 18:42:51.000000 gitdata-lib-0.0.9/gitdata/connectors/local.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      783 2021-08-11 18:42:35.000000 gitdata-lib-0.0.9/gitdata/connectors/location.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      192 2021-08-11 21:20:11.000000 gitdata-lib-0.0.9/gitdata/connectors/rows.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)      447 2021-09-28 03:27:12.000000 gitdata-lib-0.0.9/gitdata/connectors/system.py
+-rw-r--r--   0 herb      (1000) herb      (1000)      268 2021-08-11 18:47:03.000000 gitdata-lib-0.0.9/gitdata/connectors/zip.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/database/
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1970 2021-11-23 16:08:09.000000 gitdata-lib-0.0.9/gitdata/database/__init__.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)    12284 2021-11-23 19:36:39.000000 gitdata-lib-0.0.9/gitdata/database/common.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     2395 2021-10-10 23:23:51.000000 gitdata-lib-0.0.9/gitdata/database/mysql.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)      263 2021-07-06 14:15:29.000000 gitdata-lib-0.0.9/gitdata/database/mysql_setup_test_database.sql
+-rw-rw-r--   0 herb      (1000) herb      (1000)     2235 2021-11-13 17:33:58.000000 gitdata-lib-0.0.9/gitdata/database/postgresql.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     2486 2021-10-23 17:08:35.000000 gitdata-lib-0.0.9/gitdata/database/sqlite3.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-07-05 05:19:19.000000 gitdata-lib-0.0.9/gitdata/database/sqlite3_setup.sql
+-rw-rw-r--   0 herb      (1000) herb      (1000)      855 2021-07-05 05:21:27.000000 gitdata-lib-0.0.9/gitdata/database/sqlite3_setup_test_data.sql
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1857 2021-07-06 03:44:00.000000 gitdata-lib-0.0.9/gitdata/json.py
+-rw-r--r--   0 herb      (1000) herb      (1000)    16796 2021-10-22 08:04:45.000000 gitdata-lib-0.0.9/gitdata/queues.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     4387 2021-08-12 16:29:48.000000 gitdata-lib-0.0.9/gitdata/solutions.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata/stores/
+-rw-rw-r--   0 herb      (1000) herb      (1000)        0 2021-07-16 18:08:53.000000 gitdata-lib-0.0.9/gitdata/stores/__init__.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)     3690 2021-07-16 18:06:49.000000 gitdata-lib-0.0.9/gitdata/stores/common.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)    28846 2021-10-23 17:05:35.000000 gitdata-lib-0.0.9/gitdata/stores/entities.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)      694 2021-10-14 21:19:38.000000 gitdata-lib-0.0.9/gitdata/stores/entity_store.sql
+-rw-rw-r--   0 herb      (1000) herb      (1000)    23238 2021-10-23 17:09:37.000000 gitdata-lib-0.0.9/gitdata/stores/records.py
+-rw-rw-r--   0 herb      (1000) herb      (1000)    20613 2021-11-23 17:12:14.000000 gitdata-lib-0.0.9/gitdata/utils.py
+drwxrwxr-x   0 herb      (1000) herb      (1000)        0 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1155 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 herb      (1000) herb      (1000)     1226 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)        1 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)       46 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)      103 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/requires.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)        8 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/gitdata_lib.egg-info/top_level.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)      102 2021-11-05 21:06:47.000000 gitdata-lib-0.0.9/requirements.txt
+-rw-rw-r--   0 herb      (1000) herb      (1000)       38 2021-11-23 19:44:54.000000 gitdata-lib-0.0.9/setup.cfg
+-rw-r--r--   0 herb      (1000) herb      (1000)     1613 2021-10-14 22:59:26.000000 gitdata-lib-0.0.9/setup.py
```

### Comparing `gitdata-lib-0.0.8/PKG-INFO` & `gitdata-lib-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitdata-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data extraction and analysis library
 Home-page: https://github.com/gitdata/gitdata-lib
 Author: DSI Labs
 Author-email: support@gitdata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `gitdata-lib-0.0.8/gitdata/buckets.py` & `gitdata-lib-0.0.9/gitdata/buckets.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/cli/__init__.py` & `gitdata-lib-0.0.9/gitdata/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/config.py` & `gitdata-lib-0.0.9/gitdata/config.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/common.py` & `gitdata-lib-0.0.9/gitdata/connectors/common.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/csv.py` & `gitdata-lib-0.0.9/gitdata/connectors/csv.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/gitlab.py` & `gitdata-lib-0.0.9/gitdata/connectors/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/json.py` & `gitdata-lib-0.0.9/gitdata/connectors/json.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/local.py` & `gitdata-lib-0.0.9/gitdata/connectors/local.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/connectors/location.py` & `gitdata-lib-0.0.9/gitdata/connectors/location.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/database/__init__.py` & `gitdata-lib-0.0.9/gitdata/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/database/common.py` & `gitdata-lib-0.0.9/gitdata/database/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
             )
 
         def format_arg(arg):
             if isinstance(arg, str) and len(arg) > 100:
                 return arg[:50] + '[{:,} chars]'.format(len(arg) - 100) + arg[-50:]
             elif isinstance(arg, bytes):
                 return '[{:,} bytes]'.format(len(arg))
+            elif isinstance(arg, tuple):
+                return tuple(map(format_arg, arg))
             else:
                 return arg
 
         start = timeit.default_timer()
         many = method == cursor.executemany
         command, params = self.translate(command, *args, many=many)
         try:
```

### Comparing `gitdata-lib-0.0.8/gitdata/database/mysql.py` & `gitdata-lib-0.0.9/gitdata/database/mysql.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/database/postgresql.py` & `gitdata-lib-0.0.9/gitdata/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/database/sqlite3.py` & `gitdata-lib-0.0.9/gitdata/database/sqlite3.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/database/sqlite3_setup_test_data.sql` & `gitdata-lib-0.0.9/gitdata/database/sqlite3_setup_test_data.sql`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/json.py` & `gitdata-lib-0.0.9/gitdata/json.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/queues.py` & `gitdata-lib-0.0.9/gitdata/queues.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/solutions.py` & `gitdata-lib-0.0.9/gitdata/solutions.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/stores/common.py` & `gitdata-lib-0.0.9/gitdata/stores/common.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/stores/entities.py` & `gitdata-lib-0.0.9/gitdata/stores/entities.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/stores/entity_store.sql` & `gitdata-lib-0.0.9/gitdata/stores/entity_store.sql`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/stores/records.py` & `gitdata-lib-0.0.9/gitdata/stores/records.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata/utils.py` & `gitdata-lib-0.0.9/gitdata/utils.py`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/gitdata_lib.egg-info/PKG-INFO` & `gitdata-lib-0.0.9/gitdata_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitdata-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data extraction and analysis library
 Home-page: https://github.com/gitdata/gitdata-lib
 Author: DSI Labs
 Author-email: support@gitdata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `gitdata-lib-0.0.8/gitdata_lib.egg-info/SOURCES.txt` & `gitdata-lib-0.0.9/gitdata_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitdata-lib-0.0.8/setup.py` & `gitdata-lib-0.0.9/setup.py`

 * *Files identical despite different names*

