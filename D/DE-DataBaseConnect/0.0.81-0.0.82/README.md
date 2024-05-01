# Comparing `tmp/DE_DataBaseConnect-0.0.81.tar.gz` & `tmp/DE_DataBaseConnect-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.81.tar", last modified: Wed May  1 14:22:42 2024, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.82.tar", last modified: Wed May  1 14:31:59 2024, max compression
```

## Comparing `DE_DataBaseConnect-0.0.81.tar` & `DE_DataBaseConnect-0.0.82.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:22:42.682434 DE_DataBaseConnect-0.0.81/
--rw-rw-rw-   0        0        0    19082 2024-04-30 19:25:32.000000 DE_DataBaseConnect-0.0.81/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:22:42.670470 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0     1210 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:22:41.000000 DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.81/Licence.txt
--rw-rw-rw-   0        0        0     1210 2024-05-01 14:22:42.683432 DE_DataBaseConnect-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.81/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 14:22:42.693406 DE_DataBaseConnect-0.0.81/setup.cfg
--rw-rw-rw-   0        0        0      690 2024-05-01 14:22:08.000000 DE_DataBaseConnect-0.0.81/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:31:59.278070 DE_DataBaseConnect-0.0.82/
+-rw-rw-rw-   0        0        0    19082 2024-04-30 19:25:32.000000 DE_DataBaseConnect-0.0.82/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:31:59.263111 DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0     1210 2024-05-01 14:31:58.000000 DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-01 14:31:58.000000 DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:31:58.000000 DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:31:58.000000 DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.82/Licence.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-01 14:31:59.279070 DE_DataBaseConnect-0.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.82/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:31:59.291172 DE_DataBaseConnect-0.0.82/setup.cfg
+-rw-rw-rw-   0        0        0      690 2024-05-01 14:31:51.000000 DE_DataBaseConnect-0.0.82/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.81/DE_DataBase.py` & `DE_DataBaseConnect-0.0.82/DE_DataBase.py`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.81/DE_DataBaseConnect.egg-info/PKG-INFO` & `DE_DataBaseConnect-0.0.82/DE_DataBaseConnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DE-DataBaseConnect
-Version: 0.0.81
+Version: 0.0.82
 Summary: Conector com varias base de dados
 Home-page: https://github.com/DE-DataEng/DE_DataBaseConnect.git
 Author: Almir J Gomes
 Author-email: almir.jg@hotmail.com
 License: MIT
 Keywords: Database connect
 Platform: UNKNOWN
```

### Comparing `DE_DataBaseConnect-0.0.81/Licence.txt` & `DE_DataBaseConnect-0.0.82/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.81/PKG-INFO` & `DE_DataBaseConnect-0.0.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DE_DataBaseConnect
-Version: 0.0.81
+Version: 0.0.82
 Summary: Conector com varias base de dados
 Home-page: https://github.com/DE-DataEng/DE_DataBaseConnect.git
 Author: Almir J Gomes
 Author-email: almir.jg@hotmail.com
 License: MIT
 Keywords: Database connect
 Platform: UNKNOWN
```

### Comparing `DE_DataBaseConnect-0.0.81/README.md` & `DE_DataBaseConnect-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.81/setup.py` & `DE_DataBaseConnect-0.0.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme= arq.read()
 
 setup(
     name='DE_DataBaseConnect',
-    version='0.0.81',
+    version='0.0.82',
     license="MIT",
     author='Almir J Gomes',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='almir.jg@hotmail.com',
     keywords="Database connect",
     description='Conector com varias base de dados',
```

