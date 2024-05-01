# Comparing `tmp/DE_DataBaseConnect-0.0.80.tar.gz` & `tmp/DE_DataBaseConnect-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.80.tar", last modified: Wed May  1 13:57:12 2024, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.81.tar", last modified: Wed May  1 14:22:42 2024, max compression
```

## Comparing `DE_DataBaseConnect-0.0.80.tar` & `DE_DataBaseConnect-0.0.81.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 13:57:12.366582 DE_DataBaseConnect-0.0.80/
--rw-rw-rw-   0        0        0    19082 2024-04-30 19:25:32.000000 DE_DataBaseConnect-0.0.80/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2024-05-01 13:57:12.354614 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0     1210 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 13:57:11.000000 DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.80/Licence.txt
--rw-rw-rw-   0        0        0     1210 2024-05-01 13:57:12.367580 DE_DataBaseConnect-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.80/README.md
--rw-rw-rw-   0        0        0      292 2024-04-30 19:05:16.000000 DE_DataBaseConnect-0.0.80/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 13:57:12.379546 DE_DataBaseConnect-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-05-01 13:57:07.000000 DE_DataBaseConnect-0.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:22:42.682434 DE_DataBaseConnect-0.0.81/
+-rw-rw-rw-   0        0        0    19082 2024-04-30 19:25:32.000000 DE_DataBaseConnect-0.0.81/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:22:42.670470 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0     1210 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.81/Licence.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-01 14:22:42.683432 DE_DataBaseConnect-0.0.81/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.81/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:22:42.693406 DE_DataBaseConnect-0.0.81/setup.cfg
+-rw-rw-rw-   0        0        0      690 2024-05-01 14:22:08.000000 DE_DataBaseConnect-0.0.81/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.80/DE_DataBase.py` & `DE_DataBaseConnect-0.0.81/DE_DataBase.py`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.80/DE_DataBaseConnect.egg-info/PKG-INFO` & `DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DE-DataBaseConnect
-Version: 0.0.80
+Version: 0.0.81
 Summary: Conector com varias base de dados
 Home-page: https://github.com/DE-DataEng/DE_DataBaseConnect.git
 Author: Almir J Gomes
 Author-email: almir.jg@hotmail.com
 License: MIT
 Keywords: Database connect
 Platform: UNKNOWN
```

### Comparing `DE_DataBaseConnect-0.0.80/Licence.txt` & `DE_DataBaseConnect-0.0.81/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.80/PKG-INFO` & `DE_DataBaseConnect-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DE_DataBaseConnect
-Version: 0.0.80
+Version: 0.0.81
 Summary: Conector com varias base de dados
 Home-page: https://github.com/DE-DataEng/DE_DataBaseConnect.git
 Author: Almir J Gomes
 Author-email: almir.jg@hotmail.com
 License: MIT
 Keywords: Database connect
 Platform: UNKNOWN
```

### Comparing `DE_DataBaseConnect-0.0.80/README.md` & `DE_DataBaseConnect-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.80/setup.py` & `DE_DataBaseConnect-0.0.81/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme= arq.read()
 
 setup(
     name='DE_DataBaseConnect',
-    version='0.0.80',
+    version='0.0.81',
     license="MIT",
     author='Almir J Gomes',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='almir.jg@hotmail.com',
     keywords="Database connect",
     description='Conector com varias base de dados',
-    packages=find_packages(),
+    #packages=find_packages(),
     url='https://github.com/DE-DataEng/DE_DataBaseConnect.git',
-    install_requires=["sqlalchemy", "cx_Oracle", "sqlite3", "psycopg2", "mysql.connector", "pymssql", "redshift_connector", "fdb", "jaydebeapi", "jpype"]
+    #install_requires=["sqlalchemy", "cx_Oracle", "sqlite3", "psycopg2", "mysql.connector", "pymssql", "redshift_connector", "fdb", "jaydebeapi", "jpype"]
 )
```

