# Comparing `tmp/torch_model_manager-0.1.0.dev2.tar.gz` & `tmp/torch_model_manager-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev2.tar", last modified: Wed May  1 11:22:47 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev3.tar", last modified: Wed May  1 12:02:13 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev2.tar` & `torch_model_manager-0.1.0.dev3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 11:22:47.671007 torch_model_manager-0.1.0.dev2/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 11:22:41.000000 torch_model_manager-0.1.0.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.659007 torch_model_manager-0.1.0.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23321 2024-05-01 11:20:17.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev2/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 12:02:08.000000 torch_model_manager-0.1.0.dev3/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.662922 torch_model_manager-0.1.0.dev3/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.662922 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.666922 torch_model_manager-0.1.0.dev3/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.666922 torch_model_manager-0.1.0.dev3/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22993 2024-05-01 12:01:40.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev3/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 12:02:13.000000 torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 12:02:13.670922 torch_model_manager-0.1.0.dev3/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev3/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev3/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev2/PKG-INFO` & `torch_model_manager-0.1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev2/README.md` & `torch_model_manager-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev2/setup.py` & `torch_model_manager-0.1.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev2'
+version = '0.1.0.dev3'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev3/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev3/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev3/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,16 +257,14 @@
                 )
             
         
         def init_npt_logger(self, 
                             model: nn.Module,
                             base_namespace: str='training', 
                             log_model_diagram: bool=True, 
-                            log_gradients: bool=True, 
-                            log_parameters: bool=True, 
                             log_freq: int=1,
                             **kwargs):
             """
             Initialize the Neptune logger.
 
             Args:
                 model (nn.Module): The model to log.
@@ -277,32 +275,28 @@
                 log_freq (int, optional): The logging frequency. Defaults to 1.
             """
             self.npt_logger = NeptuneLogger(
                 run=self.run,
                 base_namespace=base_namespace,
                 model=model,
                 log_model_diagram=log_model_diagram,
-                log_gradients=log_gradients,
-                log_parameters=log_parameters,
                 log_freq=log_freq,
 
             )
             
-            # output = kwargs.get("output", None)
-            # show_attrs = kwargs.get("show_attrs", True)
-            # show_saved = kwargs.get("show_saved", True)
-            # render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
-            
-            # if output is not None:
-            #     make_dot(output, 
-            #         params=dict(model.named_parameters()), 
-            #         show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
-            #     self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
-                
-            print(Fore.GREEN+"The Neptune Logger is successfully initialized.", Fore.WHITE)
+            output = kwargs.get("output", None)
+            show_attrs = kwargs.get("show_attrs", True)
+            show_saved = kwargs.get("show_saved", True)
+            render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
+            
+            if output is not None:
+                make_dot(output, 
+                    params=dict(model.named_parameters()), 
+                    show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
+                self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
         
         def track_metric(self, 
                          model: nn.Module, 
                          metric: Union[float, int],
                          namespace: str, 
                          **kwargs):
             """
@@ -338,15 +332,15 @@
             Log hyperparameters.
 
             Args:
                 model (nn.Module): The model to log the hyperparameters for.
                 hyperparams (dict): The hyperparameters.
                 namespace (str, optional): The namespace to log the hyperparameters. Defaults to "hyperparams".
             """
-            self.init_npt_logger(model, kwargs)
+            self.init_npt_logger(model, **kwargs)
             self.run[self.npt_logger.base_namespace][namespace] = stringify_unsupported( 
                 hyperparams
             )
             
             print(Fore.GREEN+"The hyperparameters are successfully logged to Neptune.", Fore.WHITE)
             
         def log_figure(self,
```

### Comparing `torch_model_manager-0.1.0.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev3/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev3/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev2/utils/helpers.py` & `torch_model_manager-0.1.0.dev3/utils/helpers.py`

 * *Files identical despite different names*

