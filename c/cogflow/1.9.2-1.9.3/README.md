# Comparing `tmp/cogflow-1.9.2.tar.gz` & `tmp/cogflow-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.2.tar", last modified: Mon Apr 29 17:02:42 2024, max compression
+gzip compressed data, was "cogflow-1.9.3.tar", last modified: Wed May  1 10:06:44 2024, max compression
```

## Comparing `cogflow-1.9.2.tar` & `cogflow-1.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:42.719732 cogflow-1.9.2/
--rw-rw-rw-   0        0        0     3230 2024-04-29 17:02:42.712428 cogflow-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:42.552347 cogflow-1.9.2/cogflow/
--rw-rw-rw-   0        0        0     5553 2024-04-29 16:03:16.000000 cogflow-1.9.2/cogflow/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.2/cogflow/cogflow_config.ini
--rw-rw-rw-   0        0        0     5530 2024-04-29 16:03:16.000000 cogflow-1.9.2/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.2/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    12888 2024-04-29 16:09:31.000000 cogflow-1.9.2/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.2/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.2/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.2/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.2/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:42.616279 cogflow-1.9.2/cogflow.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-04-29 17:02:42.000000 cogflow-1.9.2/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-04-29 17:02:42.000000 cogflow-1.9.2/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:02:42.000000 cogflow-1.9.2/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-29 17:02:42.000000 cogflow-1.9.2/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 17:02:42.000000 cogflow-1.9.2/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:02:42.720741 cogflow-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1947 2024-04-29 16:43:32.000000 cogflow-1.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:42.688039 cogflow-1.9.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.2/tests/__init__.py
--rw-rw-rw-   0        0        0    10088 2024-04-27 04:47:53.000000 cogflow-1.9.2/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     5377 2024-04-27 04:47:53.000000 cogflow-1.9.2/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    14187 2024-04-29 11:23:09.000000 cogflow-1.9.2/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     7877 2024-04-29 11:23:09.000000 cogflow-1.9.2/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.744648 cogflow-1.9.3/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 10:06:44.744648 cogflow-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.689027 cogflow-1.9.3/cogflow/
+-rw-rw-rw-   0        0        0     5465 2024-04-29 17:30:08.000000 cogflow-1.9.3/cogflow/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.3/cogflow/cogflow_config.ini
+-rw-rw-rw-   0        0        0     5530 2024-04-30 09:53:35.000000 cogflow-1.9.3/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.3/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    13679 2024-05-01 10:04:07.000000 cogflow-1.9.3/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.3/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.3/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.3/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.3/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.713905 cogflow-1.9.3/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:06:44.744648 cogflow-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2024-05-01 10:05:21.000000 cogflow-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.729211 cogflow-1.9.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9844 2024-04-30 10:56:28.000000 cogflow-1.9.3/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5018 2024-04-30 11:04:44.000000 cogflow-1.9.3/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14194 2024-04-30 11:12:49.000000 cogflow-1.9.3/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     4821 2024-04-30 11:27:24.000000 cogflow-1.9.3/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.2/PKG-INFO` & `cogflow-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.2
+Version: 1.9.3
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.2/README.md` & `cogflow-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow/__init__.py` & `cogflow-1.9.3/cogflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,19 @@
     COGFLOW_DB_PORT,
     COGFLOW_DB_NAME,
     MINIO_ENDPOINT_URL,
     MINIO_ACCESS_KEY,
     MINIO_SECRET_ACCESS_KEY,
 )
 
-# from .plugin_status import plugin_statuses
-# from .pluginerrors import PluginErrors
-from .pluginmanager import PluginManager
 
-from .mlflowplugin import MlflowPlugin
-from .kubeflowplugin import CogContainer, KubeflowPlugin
+from .pluginmanager import PluginManager
 from .dataset_plugin import DatasetPlugin
+from .kubeflowplugin import CogContainer, KubeflowPlugin
+from .mlflowplugin import MlflowPlugin
 
 
 delete_registered_model = MlflowPlugin().delete_registered_model
 search_registered_models = MlflowPlugin().search_registered_models
 load_model = MlflowPlugin().load_model
 register_model = MlflowPlugin().register_model
 autolog = MlflowPlugin().autolog
```

### Comparing `cogflow-1.9.2/cogflow/dataset_plugin.py` & `cogflow-1.9.3/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow/kubeflowplugin.py` & `cogflow-1.9.3/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow/mlflowplugin.py` & `cogflow-1.9.3/cogflow/mlflowplugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module provides functionality related to Mlflow.
 """
 
 import os
-from typing import Union
+from typing import Union, Any, Optional
 
 import mlflow as ml
 import numpy as np
 import pandas as pd
 import requests
 from mlflow.models.signature import ModelSignature
 from mlflow.tracking import MlflowClient
@@ -285,45 +285,53 @@
             Mlflow Run object
         """
         # Verify plugin activation
         PluginManager().verify_activation(MlflowPlugin().section)
 
         return self.mlflow.end_run()
 
-    def log_param(self, *args):
+    def log_param(self, key: str, value: Any, synchronous: bool = True) -> None:
         """
-        Log parameters to the Mlflow run.
+        Log a parameter to the Mlflow run.
 
         Args:
-            run: Mlflow Run object returned by start_mlflow_run method.
-            param: Containing parameters to log.
+            key (str): The key of the parameter to log.
+            value (Any): The value of the parameter to log.
+            synchronous (bool, optional): If True, logs the parameter synchronously.
+                Defaults to True.
 
         Returns:
             None
         """
         # Verify plugin activation
         PluginManager().verify_activation(MlflowPlugin().section)
 
-        return self.mlflow.log_param(*args)
+        return self.mlflow.log_param(key, value, synchronous)
 
-    def log_metric(self, *args):
+    def log_metric(self, key: str,value: float,step: Optional[int] = None,
+                   synchronous: Optional[bool] = None,timestamp: Optional[int] = None,
+                   run_id: Optional[str] = None) -> None:
         """
-        Log metrics to the Mlflow run.
+        Log a metric to the Mlflow run.
 
         Args:
-            run: Mlflow Run object returned by start_mlflow_run method.
-            metric: Containing metrics to log.
+            key (str): The name of the metric to log.
+            value (float): The value of the metric to log.
+            step (Optional[int], optional): Step to log the metric at. Defaults to None.
+            synchronous (Optional[bool], optional): Whether to log synchronously. Defaults to True.
+            timestamp (Optional[int], optional): The timestamp of the metric. Defaults to None.
+            run_id (Optional[str], optional): The run ID. Defaults to None.
 
         Returns:
             None
         """
         # Verify plugin activation
         PluginManager().verify_activation(MlflowPlugin().section)
 
-        return self.mlflow.log_metric(*args)
+        return self.mlflow.log_metric(key, value, step, synchronous, timestamp, run_id)
 
     def log_model(
         self,
         sk_model,
         artifact_path,
         conda_env=None,
         code_paths=None,
```

### Comparing `cogflow-1.9.2/cogflow/plugin_config.py` & `cogflow-1.9.3/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow/plugin_status.py` & `cogflow-1.9.3/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow/pluginmanager.py` & `cogflow-1.9.3/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/cogflow.egg-info/PKG-INFO` & `cogflow-1.9.3/cogflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.2
+Version: 1.9.3
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.2/cogflow.egg-info/SOURCES.txt` & `cogflow-1.9.3/cogflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.2/setup.py` & `cogflow-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cogflow",
-    version="1.9.2",
+    version="1.9.3",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
@@ -52,10 +52,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     package_data={
-            'cogflow': ['cogflow_config.ini'],
-        }
+        "cogflow": ["cogflow_config.ini"],
+    },
 )
```

### Comparing `cogflow-1.9.2/tests/test_dataset_plugin.py` & `cogflow-1.9.3/tests/test_dataset_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from unittest.mock import patch, MagicMock
 
 import minio
 import requests
 
-from cogflow.cogflow.plugins.dataset_plugin import DatasetPlugin
+from cogflow.cogflow.dataset_plugin import DatasetPlugin
 
 
 class TestDatasetPlugin(unittest.TestCase):
     @patch("requests.get")
     @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.save_to_minio")
     def test_query_endpoint_and_download_file_success(
         self, mock_save_to_minio, mock_requests_get
@@ -73,17 +73,17 @@
     @patch("os.getenv")
     def test_save_to_minio_success(self, mock_getenv, mock_create_minio_client):
 
         # Arrange
         mock_minio_client = MagicMock()
         mock_create_minio_client.return_value = mock_minio_client
         mock_getenv.side_effect = lambda x: {
-            "MINIO_ENDPOINT_URL": "localhost:9000",
-            "MINIO_ACCESS_KEY": "minio",
-            "MINIO_SECRET_ACCESS_KEY": "minio123",
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "ACCESS_KEY_ID": "minio",
+            "SECRET_ACCESS_KEY": "minio123",
         }[x]
 
         dataset_plugin = DatasetPlugin()
         file_content = b"Test dataset content"
         output_file = "dataset.csv"
 
         mock_minio_instance = MagicMock()
@@ -109,17 +109,17 @@
         mock_getenv,
         mock_create_minio_client,
     ):
         # Arrange
         mock_minio_client = MagicMock()
         mock_create_minio_client.return_value = mock_minio_client
         mock_getenv.side_effect = lambda x: {
-            "MINIO_ENDPOINT_URL": "localhost:9000",
-            "MINIO_ACCESS_KEY": "minio",
-            "MINIO_SECRET_ACCESS_KEY": "minio123",
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "ACCESS_KEY_ID": "minio",
+            "SECRET_ACCESS_KEY": "minio123",
         }[x]
 
         dataset_plugin = DatasetPlugin()
         file_content = b"Test dataset content"
         output_file = "dataset.csv"
 
         mock_minio_client.bucket_exists.return_value = False
@@ -136,17 +136,17 @@
         mock_getenv,
         mock_create_minio_client,
     ):
         # Arrange
         mock_minio_client = MagicMock()
         mock_create_minio_client.return_value = mock_minio_client
         mock_getenv.side_effect = lambda x: {
-            "MINIO_ENDPOINT_URL": "localhost:9000",
-            "MINIO_ACCESS_KEY": "minio",
-            "MINIO_SECRET_ACCESS_KEY": "minio123",
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "ACCESS_KEY_ID": "minio",
+            "SECRET_ACCESS_KEY": "minio123",
         }[x]
 
         dataset_plugin = DatasetPlugin()
         file_content = b"Test dataset content"
         output_file = "dataset.csv"
 
         mock_minio_client.bucket_exists.return_value = False
@@ -163,17 +163,17 @@
     @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
     @patch("os.getenv")
     def test_save_to_exception(self, mock_getenv, mock_create_minio_client):
         # Arrange
         mock_minio_client = MagicMock()
         mock_create_minio_client.return_value = mock_minio_client
         mock_getenv.side_effect = lambda x: {
-            "MINIO_ENDPOINT_URL": "localhost:9000",
-            "MINIO_ACCESS_KEY": "minio",
-            "MINIO_SECRET_ACCESS_KEY": "minio123",
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "ACCESS_KEY_ID": "minio",
+            "SECRET_ACCESS_KEY": "minio123",
         }[x]
 
         dataset_plugin = DatasetPlugin()
         file_content = b"Test dataset content"
         output_file = "dataset.csv"
 
         # mock_minio_client.bucket_exists.return_value = False
@@ -238,28 +238,21 @@
         # Act
         result = dataset_plugin.delete_from_minio(object_name, bucket_name)
 
         # Assert
         self.assertFalse(result)
         mock_minio_instance.remove_object.assert_not_called()
 
-    def test_version(self):
-        self.assertIsNone(DatasetPlugin.version())
-
-    def test_is_alive(self):
-        dataset_plugin = DatasetPlugin()
-        self.assertIsNone(dataset_plugin.is_alive())
-
     @patch("os.getenv")
     def test_create_minio_client(self, mock_getenv):
         # Define test parameters
         mock_getenv.side_effect = lambda x: {
-            "MINIO_ENDPOINT_URL": "localhost:9000",
-            "MINIO_ACCESS_KEY": "minio",
-            "MINIO_SECRET_ACCESS_KEY": "minio123",
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "ACCESS_KEY_ID": "minio",
+            "SECRET_ACCESS_KEY": "minio123",
         }[x]
 
         # Create the MinioClient object
         dataset_plugin = DatasetPlugin()
         minio_client = dataset_plugin.create_minio_client()
 
         # Assert that the MinioClient object is created correctly
```

### Comparing `cogflow-1.9.2/tests/test_kubeflowplugin.py` & `cogflow-1.9.3/tests/test_kubeflowplugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 from unittest.mock import patch, MagicMock
 
 from kubernetes.client.models import V1EnvVar
 
-from cogflow.cogflow.plugins.kubeflowplugin import KubeflowPlugin, CogContainer
+from cogflow.cogflow.kubeflowplugin import KubeflowPlugin, CogContainer
 from cogflow.cogflow import plugin_config
 
 
 class TestKubeflowPlugin(unittest.TestCase):
     def setUp(self):
         self.kfp_plugin = KubeflowPlugin()
 
@@ -127,20 +127,10 @@
     def test_get_model_url(self):
         model_name = "test_model"
 
         with self.assertRaises(Exception):
             # Call the method you're testing here
             self.kfp_plugin.get_model_url(model_name)
 
-    @patch("kfp.__version__", "1.8.22")  # Mocking the kfp.__version__ attribute
-    def test_version(self):
-        result = self.kfp_plugin.version()
-
-        # Assert that the result matches the mocked version
-        self.assertEqual(result, "1.8.22")
-
-    def test_is_alive(self):
-        self.assertIsNone(self.kfp_plugin.is_alive())
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cogflow-1.9.2/tests/test_mlflowplugin.py` & `cogflow-1.9.3/tests/test_mlflowplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Test module for cases related to mlflow_plugin
 """
 
 import unittest
 from unittest.mock import patch, MagicMock
 from mlflow.exceptions import MlflowException
-from cogflow.cogflow.model import MlflowPlugin
+from cogflow.cogflow.mlflowplugin import MlflowPlugin
 
 
 class TestMlflowPlugin(unittest.TestCase):
     """
     Test Class for cases related to mlflow_plugin
     """
 
@@ -146,15 +146,15 @@
         # Define the exception to be raised
         exception_to_raise = MlflowException("API request failed")
 
         # Mocking the client method to raise the exception
         mock_client.return_value.create_registered_model.side_effect = (
             exception_to_raise
         )
-        self.mlflow_plugin.create_registered_model("model_name_1")
+        self.mlflow_plugin.create_registered_model("model_name_2")
 
     @patch("mlflow.tracking.client.MlflowClient.create_registered_model")
     def test_create_registered_model(self, mock_client):
         """
             test case for create_registered_model
         :param mock_client:
         :return:
```

