# Comparing `tmp/torch_model_manager-0.1.0.dev1.tar.gz` & `tmp/torch_model_manager-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev1.tar", last modified: Mon Apr 29 11:59:28 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev2.tar", last modified: Wed May  1 11:22:47 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev1.tar` & `torch_model_manager-0.1.0.dev2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-04-29 11:58:58.000000 torch_model_manager-0.1.0.dev1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.494263 torch_model_manager-0.1.0.dev1/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23303 2024-04-29 11:52:37.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.494263 torch_model_manager-0.1.0.dev1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 11:22:47.671007 torch_model_manager-0.1.0.dev2/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 11:22:41.000000 torch_model_manager-0.1.0.dev2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.659007 torch_model_manager-0.1.0.dev2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.663007 torch_model_manager-0.1.0.dev2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23321 2024-05-01 11:20:17.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev2/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 11:22:47.000000 torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 11:22:47.667007 torch_model_manager-0.1.0.dev2/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev2/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev1/PKG-INFO` & `torch_model_manager-0.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev1/README.md` & `torch_model_manager-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev1/setup.py` & `torch_model_manager-0.1.0.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev1'
+version = '0.1.0.dev2'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev2/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,24 +283,24 @@
                 log_model_diagram=log_model_diagram,
                 log_gradients=log_gradients,
                 log_parameters=log_parameters,
                 log_freq=log_freq,
 
             )
             
-            output = kwargs.get("output", None)
-            show_attrs = kwargs.get("show_attrs", True)
-            show_saved = kwargs.get("show_saved", True)
-            render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
+            # output = kwargs.get("output", None)
+            # show_attrs = kwargs.get("show_attrs", True)
+            # show_saved = kwargs.get("show_saved", True)
+            # render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
             
-            if output is not None:
-                make_dot(output, 
-                    params=dict(model.named_parameters()), 
-                    show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
-                self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
+            # if output is not None:
+            #     make_dot(output, 
+            #         params=dict(model.named_parameters()), 
+            #         show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
+            #     self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
                 
             print(Fore.GREEN+"The Neptune Logger is successfully initialized.", Fore.WHITE)
         
         def track_metric(self, 
                          model: nn.Module, 
                          metric: Union[float, int],
                          namespace: str,
```

### Comparing `torch_model_manager-0.1.0.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev1/utils/helpers.py` & `torch_model_manager-0.1.0.dev2/utils/helpers.py`

 * *Files identical despite different names*

