# Comparing `tmp/pysparkify-0.26.2.tar.gz` & `tmp/pysparkify-0.26.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.26.2.tar", last modified: Sun Apr 28 08:50:21 2024, max compression
+gzip compressed data, was "pysparkify-0.26.3.tar", last modified: Wed May  1 15:48:49 2024, max compression
```

## Comparing `pysparkify-0.26.2.tar` & `pysparkify-0.26.3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.517237 pysparkify-0.26.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-28 08:50:21.517237 pysparkify-0.26.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-28 08:50:18.000000 pysparkify-0.26.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.513237 pysparkify-0.26.2/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.513237 pysparkify-0.26.2/lib/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.513237 pysparkify-0.26.2/lib/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.513237 pysparkify-0.26.2/lib/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-28 08:50:18.000000 pysparkify-0.26.2/lib/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.517237 pysparkify-0.26.2/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 08:50:21.000000 pysparkify-0.26.2/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 08:50:21.517237 pysparkify-0.26.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-28 08:50:18.000000 pysparkify-0.26.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:21.517237 pysparkify-0.26.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 08:50:18.000000 pysparkify-0.26.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 08:50:18.000000 pysparkify-0.26.2/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-01 15:48:49.817455 pysparkify-0.26.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-01 15:48:46.000000 pysparkify-0.26.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/redshift_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/s3_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/redshift_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/s3_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.813455 pysparkify-0.26.3/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-01 15:48:46.000000 pysparkify-0.26.3/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 15:48:49.000000 pysparkify-0.26.3/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:48:49.817455 pysparkify-0.26.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 15:48:46.000000 pysparkify-0.26.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:49.817455 pysparkify-0.26.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:48:46.000000 pysparkify-0.26.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 15:48:46.000000 pysparkify-0.26.3/tests/test_app.py
```

### Comparing `pysparkify-0.26.2/PKG-INFO` & `pysparkify-0.26.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.2
+Version: 0.26.3
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -91,22 +91,27 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify your_recipe.yml
+pysparkify 'path/to/recipe.yml'
 ```
 
 Or use it in your Python scripts:
 
 ```python
+
 from pysparkify.lib.app import run
-run('your_recipe.yml')
+run('path/to/recipe.yml') #this expects spark_config.conf file on path `config/spark_config.conf` path
+
+# or with optional spark configuration file
+run('path/to/recipe.yml', 'path/to/custom_spark_config.conf')
+
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.26.2/README.md` & `pysparkify-0.26.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -74,22 +74,27 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify your_recipe.yml
+pysparkify 'path/to/recipe.yml'
 ```
 
 Or use it in your Python scripts:
 
 ```python
+
 from pysparkify.lib.app import run
-run('your_recipe.yml')
+run('path/to/recipe.yml') #this expects spark_config.conf file on path `config/spark_config.conf` path
+
+# or with optional spark configuration file
+run('path/to/recipe.yml', 'path/to/custom_spark_config.conf')
+
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.26.2/lib/transformer/sql_transformer.py` & `pysparkify-0.26.3/lib/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.2/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.26.3/pysparkify.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.2
+Version: 0.26.3
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
@@ -91,22 +91,27 @@
 
 
 ### Usage
 
 This library can be run as a command line tool:
 
 ```bash
-pysparkify your_recipe.yml
+pysparkify 'path/to/recipe.yml'
 ```
 
 Or use it in your Python scripts:
 
 ```python
+
 from pysparkify.lib.app import run
-run('your_recipe.yml')
+run('path/to/recipe.yml') #this expects spark_config.conf file on path `config/spark_config.conf` path
+
+# or with optional spark configuration file
+run('path/to/recipe.yml', 'path/to/custom_spark_config.conf')
+
 ```
 
 
 ## Design
 
 The package is structured as follows:
```

### Comparing `pysparkify-0.26.2/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.26.3/pysparkify.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 setup.py
 lib/__init__.py
 lib/app.py
 lib/context_manager.py
 lib/logger.py
 lib/sink/__init__.py
 lib/sink/csv_sink.py
+lib/sink/redshift_sink.py
+lib/sink/s3_sink.py
 lib/sink/sink.py
 lib/sink/sink_factory.py
 lib/source/__init__.py
 lib/source/csv_source.py
+lib/source/redshift_source.py
+lib/source/s3_source.py
 lib/source/source.py
 lib/source/source_factory.py
 lib/transformer/__init__.py
 lib/transformer/sql_transformer.py
 lib/transformer/transformer.py
 lib/transformer/transformer_factory.py
 pysparkify.egg-info/PKG-INFO
```

### Comparing `pysparkify-0.26.2/setup.py` & `pysparkify-0.26.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.26.2',
+    version='0.26.3',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
```

### Comparing `pysparkify-0.26.2/tests/test_app.py` & `pysparkify-0.26.3/tests/test_app.py`

 * *Files identical despite different names*

