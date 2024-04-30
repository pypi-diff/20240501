# Comparing `tmp/nsj_sql_utils_lib-1.2.0.tar.gz` & `tmp/nsj_sql_utils_lib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_sql_utils_lib-1.2.0.tar", last modified: Tue Apr 30 22:26:15 2024, max compression
+gzip compressed data, was "nsj_sql_utils_lib-1.3.0.tar", last modified: Tue Apr 30 22:43:19 2024, max compression
```

## Comparing `nsj_sql_utils_lib-1.2.0.tar` & `nsj_sql_utils_lib-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.2.0/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dao_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6146 2024-04-18 18:01:51.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbadapter3.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      916 2024-04-30 22:23:54.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbconection_mysql_connector.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbconection_psycopg2.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/create_script.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/db_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/erp_database_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/vars.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-30 22:26:15.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      656 2024-04-30 22:26:15.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-30 22:26:15.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2024-04-30 22:26:15.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-30 22:26:15.000000 nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.2.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2024-04-30 22:26:15.400244 nsj_sql_utils_lib-1.2.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dao_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6146 2024-04-18 18:01:51.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbadapter3.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1736 2024-04-30 22:42:26.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbconection.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      916 2024-04-30 22:23:54.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbconection_mysql_connector.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1005 2024-04-30 22:30:45.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbconection_psycopg2.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/create_script.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/db_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/erp_database_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/vars.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-30 22:43:19.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      691 2024-04-30 22:43:19.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-30 22:43:19.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2024-04-30 22:43:19.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-30 22:43:19.000000 nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.3.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2024-04-30 22:43:19.483161 nsj_sql_utils_lib-1.3.0/setup.cfg
```

### Comparing `nsj_sql_utils_lib-1.2.0/PKG-INFO` & `nsj_sql_utils_lib-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.2.0
+Version: 1.3.0
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.2.0/README.md` & `nsj_sql_utils_lib-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dao_util.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dao_util.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbadapter3.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbadapter3.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbconection_mysql_connector.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbconection_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/dbconection_psycopg2.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/dbconection_psycopg2.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,37 @@
         self,
         host: str,
         port: int,
         database: str,
         user: str,
         password: str,
         timeout: int = 5,
+        auto_commit: bool = True,
     ):
         self.host = host
         self.port = port
         self.database = database
         self.user = user
         self.password = password
         self.conn = None
         self.timeout = timeout
+        self.auto_commit = auto_commit
 
     def __enter__(self):
         self.conn = psycopg2.connect(
             host=self.host,
             port=self.port,
             database=self.database,
             user=self.user,
             password=self.password,
             connect_timeout=self.timeout,
         )
 
-        self.conn.set_isolation_level(psycopg2.extensions.ISOLATION_LEVEL_AUTOCOMMIT)
+        if self.auto_commit:
+            self.conn.set_isolation_level(
+                psycopg2.extensions.ISOLATION_LEVEL_AUTOCOMMIT
+            )
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.conn.close()
```

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/create_script.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/create_script.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/db_updater.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/db_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib/updater/erp_database_updater.py` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib/updater/erp_database_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/PKG-INFO` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.2.0
+Version: 1.3.0
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.2.0/nsj_sql_utils_lib.egg-info/SOURCES.txt` & `nsj_sql_utils_lib-1.3.0/nsj_sql_utils_lib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 pyproject.toml
 setup.cfg
 ./nsj_sql_utils_lib/__init__.py
 ./nsj_sql_utils_lib/dao_util.py
 ./nsj_sql_utils_lib/dbadapter3.py
+./nsj_sql_utils_lib/dbconection.py
 ./nsj_sql_utils_lib/dbconection_mysql_connector.py
 ./nsj_sql_utils_lib/dbconection_psycopg2.py
 ./nsj_sql_utils_lib.egg-info/PKG-INFO
 ./nsj_sql_utils_lib.egg-info/SOURCES.txt
 ./nsj_sql_utils_lib.egg-info/dependency_links.txt
 ./nsj_sql_utils_lib.egg-info/requires.txt
 ./nsj_sql_utils_lib.egg-info/top_level.txt
```

### Comparing `nsj_sql_utils_lib-1.2.0/setup.cfg` & `nsj_sql_utils_lib-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_sql_utils_lib
-version = 1.2.0
+version = 1.3.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-sql-utils-lib
 project_urls =
```

