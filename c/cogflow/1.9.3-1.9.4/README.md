# Comparing `tmp/cogflow-1.9.3.tar.gz` & `tmp/cogflow-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.3.tar", last modified: Wed May  1 10:06:44 2024, max compression
+gzip compressed data, was "cogflow-1.9.4.tar", last modified: Wed May  1 11:09:17 2024, max compression
```

## Comparing `cogflow-1.9.3.tar` & `cogflow-1.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.744648 cogflow-1.9.3/
--rw-rw-rw-   0        0        0     3230 2024-05-01 10:06:44.744648 cogflow-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.689027 cogflow-1.9.3/cogflow/
--rw-rw-rw-   0        0        0     5465 2024-04-29 17:30:08.000000 cogflow-1.9.3/cogflow/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.3/cogflow/cogflow_config.ini
--rw-rw-rw-   0        0        0     5530 2024-04-30 09:53:35.000000 cogflow-1.9.3/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.3/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    13679 2024-05-01 10:04:07.000000 cogflow-1.9.3/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.3/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.3/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.3/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.3/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.713905 cogflow-1.9.3/cogflow.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 10:06:44.000000 cogflow-1.9.3/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 10:06:44.744648 cogflow-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1940 2024-05-01 10:05:21.000000 cogflow-1.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 10:06:44.729211 cogflow-1.9.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.3/tests/__init__.py
--rw-rw-rw-   0        0        0     9844 2024-04-30 10:56:28.000000 cogflow-1.9.3/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     5018 2024-04-30 11:04:44.000000 cogflow-1.9.3/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    14194 2024-04-30 11:12:49.000000 cogflow-1.9.3/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     4821 2024-04-30 11:27:24.000000 cogflow-1.9.3/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.308159 cogflow-1.9.4/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 11:09:17.304159 cogflow-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.250096 cogflow-1.9.4/cogflow/
+-rw-rw-rw-   0        0        0     5465 2024-04-29 17:30:08.000000 cogflow-1.9.4/cogflow/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.4/cogflow/cogflow_config.ini
+-rw-rw-rw-   0        0        0     5530 2024-04-30 09:53:35.000000 cogflow-1.9.4/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.4/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    13755 2024-05-01 10:28:19.000000 cogflow-1.9.4/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.4/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.4/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.4/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.4/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.273088 cogflow-1.9.4/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 11:09:17.000000 cogflow-1.9.4/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:09:17.309158 cogflow-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2024-05-01 10:30:25.000000 cogflow-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:09:17.297960 cogflow-1.9.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     9844 2024-04-30 10:56:28.000000 cogflow-1.9.4/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5018 2024-04-30 11:04:44.000000 cogflow-1.9.4/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14194 2024-04-30 11:12:49.000000 cogflow-1.9.4/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     4821 2024-04-30 11:27:24.000000 cogflow-1.9.4/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.3/PKG-INFO` & `cogflow-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.3
+Version: 1.9.4
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.3/README.md` & `cogflow-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/__init__.py` & `cogflow-1.9.4/cogflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/dataset_plugin.py` & `cogflow-1.9.4/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/kubeflowplugin.py` & `cogflow-1.9.4/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/mlflowplugin.py` & `cogflow-1.9.4/cogflow/mlflowplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,16 @@
             None
         """
         # Verify plugin activation
         PluginManager().verify_activation(MlflowPlugin().section)
 
         return self.mlflow.log_param(key, value, synchronous)
 
-    def log_metric(self, key: str,value: float,step: Optional[int] = None,
-                   synchronous: Optional[bool] = None,timestamp: Optional[int] = None,
+    def log_metric(self, key: str, value: float, step: Optional[int] = None,
+                   synchronous: Optional[bool] = None, timestamp: Optional[int] = None,
                    run_id: Optional[str] = None) -> None:
         """
         Log a metric to the Mlflow run.
 
         Args:
             key (str): The name of the metric to log.
             value (float): The value of the metric to log.
@@ -323,15 +323,16 @@
 
         Returns:
             None
         """
         # Verify plugin activation
         PluginManager().verify_activation(MlflowPlugin().section)
 
-        return self.mlflow.log_metric(key, value, step, synchronous, timestamp, run_id)
+        return self.mlflow.log_metric(key, value, step=step, synchronous=synchronous,
+                                      timestamp=timestamp, run_id=run_id)
 
     def log_model(
         self,
         sk_model,
         artifact_path,
         conda_env=None,
         code_paths=None,
```

### Comparing `cogflow-1.9.3/cogflow/plugin_config.py` & `cogflow-1.9.4/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/plugin_status.py` & `cogflow-1.9.4/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow/pluginmanager.py` & `cogflow-1.9.4/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/cogflow.egg-info/PKG-INFO` & `cogflow-1.9.4/cogflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.3
+Version: 1.9.4
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.3/cogflow.egg-info/SOURCES.txt` & `cogflow-1.9.4/cogflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/setup.py` & `cogflow-1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cogflow",
-    version="1.9.3",
+    version="1.9.4",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `cogflow-1.9.3/tests/test_dataset_plugin.py` & `cogflow-1.9.4/tests/test_dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/tests/test_kubeflowplugin.py` & `cogflow-1.9.4/tests/test_kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/tests/test_mlflowplugin.py` & `cogflow-1.9.4/tests/test_mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.3/tests/test_plugin_manager.py` & `cogflow-1.9.4/tests/test_plugin_manager.py`

 * *Files identical despite different names*

