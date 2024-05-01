# Comparing `tmp/torch_model_manager-0.1.0.dev3.tar.gz` & `tmp/torch_model_manager-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev3.tar", last modified: Wed May  1 12:02:13 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev4.tar", last modified: Wed May  1 12:17:51 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev3.tar` & `torch_model_manager-0.1.0.dev4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 12:02:08.000000 torch_model_manager-0.1.0.dev3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.662922 torch_model_manager-0.1.0.dev3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.662922 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.666922 torch_model_manager-0.1.0.dev3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.666922 torch_model_manager-0.1.0.dev3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22993 2024-05-01 12:01:40.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev3/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 12:17:47.000000 torch_model_manager-0.1.0.dev4/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.332164 torch_model_manager-0.1.0.dev4/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.332164 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.336164 torch_model_manager-0.1.0.dev4/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.336164 torch_model_manager-0.1.0.dev4/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22737 2024-05-01 12:12:13.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev4/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 12:17:51.000000 torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:17:51.340164 torch_model_manager-0.1.0.dev4/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev4/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev4/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev3/PKG-INFO` & `torch_model_manager-0.1.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev3/README.md` & `torch_model_manager-0.1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev3/setup.py` & `torch_model_manager-0.1.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev3'
+version = '0.1.0.dev4'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev3/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev3/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev4/torch_model_manager/neptune_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,15 +153,14 @@
                         **kwargs
                     ) 
                     # Retrieve the id of the run and store it in the file with its associated name
                     self.run_id = self.run["sys/id"].fetch()
                     helpers.add_to_json_file(NeptuneManager.run_ids_path, name, self.run_id)
             except:
                 print(Fore.RED+"The JSON file is not found. Please check the path."+Fore.WHITE)
-            self.npt_logger = None
             
         def log_tensors(self, 
                         tensors, 
                         descriptions: List[str] = None, 
                         names: List[str] = None, 
                         paths: List[str] = None, 
                         namespace: str = None, 
@@ -253,95 +252,92 @@
                 profile = ProfileReport(dataframe, title=profile_report_title, **profile_report_kwargs)
                 
                 self.run[namespace][profile_report_name].upload(
                     File.from_content(profile.to_html(), extension="html")
                 )
             
         
-        def init_npt_logger(self, 
-                            model: nn.Module,
-                            base_namespace: str='training', 
-                            log_model_diagram: bool=True, 
-                            log_freq: int=1,
-                            **kwargs):
-            """
-            Initialize the Neptune logger.
-
-            Args:
-                model (nn.Module): The model to log.
-                base_namespace (str, optional): The base namespace for logging. Defaults to 'training'.
-                log_model_diagram (bool, optional): Whether to log the model diagram. Defaults to True.
-                log_gradients (bool, optional): Whether to log the gradients. Defaults to True.
-                log_parameters (bool, optional): Whether to log the parameters. Defaults to True.
-                log_freq (int, optional): The logging frequency. Defaults to 1.
-            """
-            self.npt_logger = NeptuneLogger(
-                run=self.run,
-                base_namespace=base_namespace,
-                model=model,
-                log_model_diagram=log_model_diagram,
-                log_freq=log_freq,
-
-            )
-            
-            output = kwargs.get("output", None)
-            show_attrs = kwargs.get("show_attrs", True)
-            show_saved = kwargs.get("show_saved", True)
-            render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
-            
-            if output is not None:
-                make_dot(output, 
-                    params=dict(model.named_parameters()), 
-                    show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
-                self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
+        # def init_npt_logger(self, 
+        #                     model: nn.Module,
+        #                     base_namespace: str='training', 
+        #                     log_model_diagram: bool=True, 
+        #                     log_freq: int=1,
+        #                     **kwargs):
+        #     """
+        #     Initialize the Neptune logger.
+
+        #     Args:
+        #         model (nn.Module): The model to log.
+        #         base_namespace (str, optional): The base namespace for logging. Defaults to 'training'.
+        #         log_model_diagram (bool, optional): Whether to log the model diagram. Defaults to True.
+        #         log_gradients (bool, optional): Whether to log the gradients. Defaults to True.
+        #         log_parameters (bool, optional): Whether to log the parameters. Defaults to True.
+        #         log_freq (int, optional): The logging frequency. Defaults to 1.
+        #     """
+        #     self.npt_logger = NeptuneLogger(
+        #         run=self.run,
+        #         base_namespace=base_namespace,
+        #         model=model,
+        #         log_model_diagram=log_model_diagram,
+        #         log_freq=log_freq,
+
+        #     )
+            
+        #     output = kwargs.get("output", None)
+        #     show_attrs = kwargs.get("show_attrs", True)
+        #     show_saved = kwargs.get("show_saved", True)
+        #     render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
+            
+        #     if output is not None:
+        #         make_dot(output, 
+        #             params=dict(model.named_parameters()), 
+        #             show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
+        #         self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
+                
         
         def track_metric(self, 
                          model: nn.Module, 
                          metric: Union[float, int],
-                         namespace: str, 
-                         **kwargs):
+                         namespace: str):
             """
             Track a metric.
 
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
-            self.init_npt_logger(model, **kwargs)
-            self.run[self.npt_logger.base_namespace][namespace].append(metric)
+            self.run[namespace].append(metric)
 
-        def log_checkpoint(self, model, checkpoint_name, **kwargs):
+        def log_checkpoint(self, model, checkpoint_name):
             """
             Log a checkpoint.
 
             Args:
                 model (nn.Module): The model to log the checkpoint for.
                 checkpoint_name (str): The name of the checkpoint.
             """
-            self.init_npt_logger(model, **kwargs)
+            
             self.npt_logger.log_checkpoint(checkpoint_name)
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
         def log_hyperparameters(self, 
                                model: nn.Module, 
                                hyperparams: dict, 
-                               namespace: str="hyperparams",
-                               **kwargs):  
+                               namespace: str):  
             """
             Log hyperparameters.
 
             Args:
                 model (nn.Module): The model to log the hyperparameters for.
                 hyperparams (dict): The hyperparameters.
                 namespace (str, optional): The namespace to log the hyperparameters. Defaults to "hyperparams".
             """
-            self.init_npt_logger(model, **kwargs)
-            self.run[self.npt_logger.base_namespace][namespace] = stringify_unsupported( 
+            self.run[namespace] = stringify_unsupported( 
                 hyperparams
             )
             
             print(Fore.GREEN+"The hyperparameters are successfully logged to Neptune.", Fore.WHITE)
             
         def log_figure(self, 
                        figure,
```

### Comparing `torch_model_manager-0.1.0.dev3/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev4/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev4/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev3/utils/helpers.py` & `torch_model_manager-0.1.0.dev4/utils/helpers.py`

 * *Files identical despite different names*

