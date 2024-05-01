# Comparing `tmp/torch_model_manager-0.1.0.dev4.tar.gz` & `tmp/torch_model_manager-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev4.tar", last modified: Wed May  1 12:17:51 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev5.tar", last modified: Wed May  1 12:49:19 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev4.tar` & `torch_model_manager-0.1.0.dev5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 12:17:47.000000 torch_model_manager-0.1.0.dev4/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.332164 torch_model_manager-0.1.0.dev4/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.332164 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.336164 torch_model_manager-0.1.0.dev4/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.336164 torch_model_manager-0.1.0.dev4/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22737 2024-05-01 12:12:13.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev4/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.262430 torch_model_manager-0.1.0.dev5/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:49:19.262430 torch_model_manager-0.1.0.dev5/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 12:49:19.262430 torch_model_manager-0.1.0.dev5/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 12:33:32.000000 torch_model_manager-0.1.0.dev5/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.242430 torch_model_manager-0.1.0.dev5/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.246430 torch_model_manager-0.1.0.dev5/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.246430 torch_model_manager-0.1.0.dev5/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.254430 torch_model_manager-0.1.0.dev5/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22885 2024-05-01 12:48:18.000000 torch_model_manager-0.1.0.dev5/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev5/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.262430 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:49:19.000000 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 12:49:19.000000 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 12:49:19.000000 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 12:49:19.000000 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 12:49:19.000000 torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:49:19.262430 torch_model_manager-0.1.0.dev5/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev5/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev5/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev4/PKG-INFO` & `torch_model_manager-0.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev4/README.md` & `torch_model_manager-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev4/setup.py` & `torch_model_manager-0.1.0.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev4'
+version = '0.1.0.dev5'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev4/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev5/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev4/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev5/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,29 +304,30 @@
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
             self.run[namespace].append(metric)
 
-        def log_checkpoint(self, model, checkpoint_name):
-            """
-            Log a checkpoint.
-
-            Args:
-                model (nn.Module): The model to log the checkpoint for.
-                checkpoint_name (str): The name of the checkpoint.
-            """
+        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, **kwargs):
+            stat_dict = {
+                "model_state_dict": model.state_dict(),
+                "optimizer_state_dict": optimizer.state_dict(),
+                "loss": loss,
+                "epoch": epoch,
+                **kwargs
+            }
             
-            self.npt_logger.log_checkpoint(checkpoint_name)
+            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            torch.save(stat_dict, tmp_file.name)
+            self.log_files(namespace=namespace, from_path=tmp_file.name, extension='pth')
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
         def log_hyperparameters(self, 
-                               model: nn.Module, 
                                hyperparams: dict, 
                                namespace: str):  
             """
             Log hyperparameters.
 
             Args:
                 model (nn.Module): The model to log the hyperparameters for.
```

### Comparing `torch_model_manager-0.1.0.dev4/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev5/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev5/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev4/utils/helpers.py` & `torch_model_manager-0.1.0.dev5/utils/helpers.py`

 * *Files identical despite different names*

