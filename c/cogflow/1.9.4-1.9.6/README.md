# Comparing `tmp/cogflow-1.9.4.tar.gz` & `tmp/cogflow-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.4.tar", last modified: Wed May  1 11:09:17 2024, max compression
+gzip compressed data, was "cogflow-1.9.6.tar", last modified: Wed May  1 15:12:00 2024, max compression
```

## Comparing `cogflow-1.9.4.tar` & `cogflow-1.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.308159 cogflow-1.9.4/
--rw-rw-rw-   0        0        0     3230 2024-05-01 11:09:17.304159 cogflow-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.250096 cogflow-1.9.4/cogflow/
--rw-rw-rw-   0        0        0     5465 2024-04-29 17:30:08.000000 cogflow-1.9.4/cogflow/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.4/cogflow/cogflow_config.ini
--rw-rw-rw-   0        0        0     5530 2024-04-30 09:53:35.000000 cogflow-1.9.4/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.4/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    13755 2024-05-01 10:28:19.000000 cogflow-1.9.4/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.4/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.4/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.4/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.4/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.273088 cogflow-1.9.4/cogflow.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 11:09:17.309158 cogflow-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1940 2024-05-01 10:30:25.000000 cogflow-1.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.297960 cogflow-1.9.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.4/tests/__init__.py
--rw-rw-rw-   0        0        0     9844 2024-04-30 10:56:28.000000 cogflow-1.9.4/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     5018 2024-04-30 11:04:44.000000 cogflow-1.9.4/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    14194 2024-04-30 11:12:49.000000 cogflow-1.9.4/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     4821 2024-04-30 11:27:24.000000 cogflow-1.9.4/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:12:00.280140 cogflow-1.9.6/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 15:12:00.274945 cogflow-1.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 15:12:00.214286 cogflow-1.9.6/cogflow/
+-rw-rw-rw-   0        0        0     5465 2024-04-29 17:30:08.000000 cogflow-1.9.6/cogflow/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.6/cogflow/cogflow_config.ini
+-rw-rw-rw-   0        0        0     6159 2024-05-01 14:08:07.000000 cogflow-1.9.6/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.6/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    13755 2024-05-01 10:28:19.000000 cogflow-1.9.6/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3116 2024-05-01 15:11:24.000000 cogflow-1.9.6/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.6/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.6/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.6/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:12:00.239738 cogflow-1.9.6/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 15:11:59.000000 cogflow-1.9.6/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-05-01 15:12:00.000000 cogflow-1.9.6/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 15:11:59.000000 cogflow-1.9.6/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-01 15:11:59.000000 cogflow-1.9.6/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 15:11:59.000000 cogflow-1.9.6/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 15:12:00.280140 cogflow-1.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2024-05-01 15:11:57.000000 cogflow-1.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:12:00.267513 cogflow-1.9.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     9844 2024-04-30 10:56:28.000000 cogflow-1.9.6/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5018 2024-04-30 11:04:44.000000 cogflow-1.9.6/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14194 2024-04-30 11:12:49.000000 cogflow-1.9.6/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     4821 2024-04-30 11:27:24.000000 cogflow-1.9.6/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.4/PKG-INFO` & `cogflow-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.4
+Version: 1.9.6
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.4/README.md` & `cogflow-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow/__init__.py` & `cogflow-1.9.6/cogflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow/dataset_plugin.py` & `cogflow-1.9.6/cogflow/dataset_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 
     def __init__(self):
         """
         Initializes DatasetPlugin with environment variables.
         """
         # Retrieve MinIO connection details from environment variables
         self.minio_endpoint = os.getenv(plugin_config.MINIO_ENDPOINT_URL)
+        # Check if the environment variable exists and has a value
+        if self.minio_endpoint:
+            # Remove the http:// or https:// prefix using string manipulation
+            if self.minio_endpoint.startswith(('http://', 'https://')):
+                # Find the index where the protocol ends
+                protocol_end_index = self.minio_endpoint.find('//') + 2
+                # Get the remaining part of the URL (without the protocol)
+                self.minio_endpoint = self.minio_endpoint[protocol_end_index:]
+        else:
+            print("MINIO_ENDPOINT_URL environment variable is not set.")
         self.minio_access_key = os.getenv(plugin_config.MINIO_ACCESS_KEY)
         self.minio_secret_key = os.getenv(plugin_config.MINIO_SECRET_ACCESS_KEY)
         self.section = "dataset_plugin"
 
     def create_minio_client(self):
         """
         Creates a MinIO client object.
```

### Comparing `cogflow-1.9.4/cogflow/kubeflowplugin.py` & `cogflow-1.9.6/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow/mlflowplugin.py` & `cogflow-1.9.6/cogflow/mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow/plugin_config.py` & `cogflow-1.9.6/cogflow/plugin_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
      MINIO_ACCESS_KEY for secure access.
 """
 
 COGFLOW_CONFIG_FILE_PATH = "COGFLOW_CONFIG_FILE_PATH"
 
 TRACKING_URI = "MLFLOW_TRACKING_URI"
 S3_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
-ACCESS_KEY_ID = "ACCESS_KEY_ID"
-SECRET_ACCESS_KEY = "SECRET_ACCESS_KEY"
+ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
+SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
 TIMER_IN_SEC = 10
 ML_TOOL = "mlflow"
 
 ML_DB_USERNAME = "ML_DB_USERNAME"
 ML_DB_PASSWORD = "ML_DB_PASSWORD"
 ML_DB_HOST = "ML_DB_HOST"
 ML_DB_PORT = "ML_DB_PORT"
@@ -58,9 +58,9 @@
 COGFLOW_DB_USERNAME = "DB_USER"
 COGFLOW_DB_PASSWORD = "DB_PASSWORD"
 COGFLOW_DB_HOST = "DB_HOST"
 COGFLOW_DB_PORT = "DB_PORT"
 COGFLOW_DB_NAME = "DB_NAME"
 
 MINIO_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
-MINIO_ACCESS_KEY = "ACCESS_KEY_ID"
-MINIO_SECRET_ACCESS_KEY = "SECRET_ACCESS_KEY"
+MINIO_ACCESS_KEY = "AWS_ACCESS_KEY_ID"
+MINIO_SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
```

### Comparing `cogflow-1.9.4/cogflow/plugin_status.py` & `cogflow-1.9.6/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow/pluginmanager.py` & `cogflow-1.9.6/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/cogflow.egg-info/PKG-INFO` & `cogflow-1.9.6/cogflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.4
+Version: 1.9.6
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.4/cogflow.egg-info/SOURCES.txt` & `cogflow-1.9.6/cogflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/setup.py` & `cogflow-1.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cogflow",
-    version="1.9.4",
+    version="1.9.6",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `cogflow-1.9.4/tests/test_dataset_plugin.py` & `cogflow-1.9.6/tests/test_dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/tests/test_kubeflowplugin.py` & `cogflow-1.9.6/tests/test_kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/tests/test_mlflowplugin.py` & `cogflow-1.9.6/tests/test_mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.4/tests/test_plugin_manager.py` & `cogflow-1.9.6/tests/test_plugin_manager.py`

 * *Files identical despite different names*

