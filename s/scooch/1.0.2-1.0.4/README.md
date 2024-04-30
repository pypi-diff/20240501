# Comparing `tmp/scooch-1.0.2.tar.gz` & `tmp/scooch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scooch-1.0.2.tar", last modified: Thu Feb  2 01:44:24 2023, max compression
+gzip compressed data, was "scooch-1.0.4.tar", last modified: Tue Apr 30 23:36:06 2024, max compression
```

## Comparing `scooch-1.0.2.tar` & `scooch-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-02-02 01:44:24.777916 scooch-1.0.2/
--rw-r--r--   0 mmccallum   (502) staff       (20)    11414 2022-08-15 23:24:09.000000 scooch-1.0.2/LICENSE
--rw-r--r--   0 mmccallum   (502) staff       (20)     3797 2023-02-02 01:44:24.777155 scooch-1.0.2/PKG-INFO
--rw-r--r--   0 mmccallum   (502) staff       (20)     6227 2022-11-29 20:47:36.000000 scooch-1.0.2/README.md
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-02-02 01:44:24.761698 scooch-1.0.2/scooch/
--rw-r--r--   0 mmccallum   (502) staff       (20)     1140 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/__init__.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-02-02 01:44:24.775486 scooch-1.0.2/scooch/cli/
--rw-r--r--   0 mmccallum   (502) staff       (20)      644 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/cli/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2676 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/cli/cli.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2205 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/cli/export.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1865 2022-11-29 20:47:36.000000 scooch-1.0.2/scooch/cli/options.py
--rw-r--r--   0 mmccallum   (502) staff       (20)    10657 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/config.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1344 2022-08-15 23:24:09.000000 scooch-1.0.2/scooch/config_collection.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     9227 2022-08-15 23:24:09.000000 scooch-1.0.2/scooch/config_factory.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1317 2022-08-15 23:24:09.000000 scooch-1.0.2/scooch/config_list.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     8217 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/configurable.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     5547 2022-12-03 11:23:20.000000 scooch-1.0.2/scooch/configurable_factory.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     7914 2023-01-04 05:39:40.000000 scooch-1.0.2/scooch/configurable_meta.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     4381 2023-01-04 06:33:39.000000 scooch-1.0.2/scooch/configurize_helper.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3835 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/generic.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3215 2022-09-20 00:26:18.000000 scooch-1.0.2/scooch/param.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-02-02 01:44:24.769877 scooch-1.0.2/scooch.egg-info/
--rw-r--r--   0 mmccallum   (502) staff       (20)     3797 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/PKG-INFO
--rw-r--r--   0 mmccallum   (502) staff       (20)      548 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/SOURCES.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)        1 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/dependency_links.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)       44 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/entry_points.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)       81 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/requires.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)        7 2023-02-02 01:44:24.000000 scooch-1.0.2/scooch.egg-info/top_level.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)       38 2023-02-02 01:44:24.778139 scooch-1.0.2/setup.cfg
--rw-r--r--   0 mmccallum   (502) staff       (20)     5271 2023-02-02 01:43:27.000000 scooch-1.0.2/setup.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-04-30 23:36:06.100643 scooch-1.0.4/
+-rw-r--r--   0 mmccallum   (502) staff       (20)    11414 2023-06-02 20:13:37.000000 scooch-1.0.4/LICENSE
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3606 2024-04-30 23:36:06.100389 scooch-1.0.4/PKG-INFO
+-rw-r--r--   0 mmccallum   (502) staff       (20)     6227 2023-06-02 20:13:37.000000 scooch-1.0.4/README.md
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-04-30 23:36:06.098407 scooch-1.0.4/scooch/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1176 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4134 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/alias_param.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-04-30 23:36:06.100061 scooch-1.0.4/scooch/cli/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      644 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/cli/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2676 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/cli/cli.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2205 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/cli/export.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1865 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/cli/options.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)    10657 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/config.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1344 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/config_collection.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     9227 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/config_factory.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1317 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/config_list.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     9436 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/configurable.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     5547 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/configurable_factory.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     9938 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/configurable_meta.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4640 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/configurize_helper.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3835 2023-06-02 20:13:37.000000 scooch-1.0.4/scooch/generic.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3393 2024-04-30 01:13:15.000000 scooch-1.0.4/scooch/param.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-04-30 23:36:06.099401 scooch-1.0.4/scooch.egg-info/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3606 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/PKG-INFO
+-rw-r--r--   0 mmccallum   (502) staff       (20)      570 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/SOURCES.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)        1 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/dependency_links.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)       43 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/entry_points.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)       79 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/requires.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)        7 2024-04-30 23:36:06.000000 scooch-1.0.4/scooch.egg-info/top_level.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)       38 2024-04-30 23:36:06.100698 scooch-1.0.4/setup.cfg
+-rw-r--r--   0 mmccallum   (502) staff       (20)     5269 2024-04-30 23:19:17.000000 scooch-1.0.4/setup.py
```

### Comparing `scooch-1.0.2/LICENSE` & `scooch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/PKG-INFO` & `scooch-1.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,19 @@
 Metadata-Version: 2.1
 Name: scooch
-Version: 1.0.2
+Version: 1.0.4
 Summary: A python module for configuring hierarchical class structures in yaml with defaults
 Home-page: http://www.mattcmccallum.com/scooch/docs
 Author: Matt C. McCallum
 Author-email: scooch@mattcmccallum.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.mattcmccallum.com/scooch/docs
 Project-URL: Bug Reports, https://github.com/PandoraMedia/scooch/issues
 Project-URL: Source, https://github.com/PandoraMedia/scooch
-Description: 
-        # Scooch
-        
-        Scooch is a recursive acronym for **S**cooch **C**onfigures **O**bject 
-        **O**riented **C**lass **H**ierarchies, and that's exactly what this package 
-        does. It is a configuration package for python codebases that simplifies the 
-        problem of configuring parameters in python code by translating YAML 
-        configuration files into object oriented class hierarchies.
-        
-        # Who needs Scooch?
-        
-        Scooch is useful for people who need an accessible interface to enable 
-        tweakability in their code. ML practitioners are a good example. They 
-        typically write code that is intended to be continuously experimented with and 
-        adjusted in response to observations from running the code. As such, it is useful 
-        to abstract these tweakable parameters from the code into a config file, providing 
-        three major benefits:
-        
-         - The config file provides a centralized location for adjustable parameters of 
-         interest in the code, improving iteration and workflow.
-         - Loading, saving and adjusting the configuration of your code is separated 
-         from the many other working variables and data structures that may exist in 
-         code.
-         - The configuration of any part of the code can be hashed, logged, and indexed, 
-         to provide a record of the code configuration at any one time.
-        
-        # Why use Scooch?
-        
-        There are many other projects out there that endeavor to translate config files 
-        into parameters in python code, for example:
-        
-         - [Gin](https://github.com/google/gin-config)
-         - [Sacred](https://sacred.readthedocs.io/en/stable/index.html)
-         - [Hydra](https://hydra.cc/)
-        
-        However, what makes Scooch different is that it not only translates config 
-        parameters into variables in your code, but into object oriented class 
-        hierarchies. This means configurations can benefit from object oriented concepts 
-        such as Inheretance, Encapsulation, Abstraction and Polymorphism.
-        
-        For more information about how to use, and why to use Scooch. Please refer to 
-        the [documentation](http://www.mattcmccallum.com/scooch/docs).
-        
 Keywords: scooch python configuration machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -68,7 +24,56 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: sphinx
+Requires-Dist: sphinx_rtd_theme==0.5.1
+Requires-Dist: ruamel.yaml==0.16.12
+Requires-Dist: click==8.1.7
+
+
+# Scooch
+
+Scooch is a recursive acronym for **S**cooch **C**onfigures **O**bject 
+**O**riented **C**lass **H**ierarchies, and that's exactly what this package 
+does. It is a configuration package for python codebases that simplifies the 
+problem of configuring parameters in python code by translating YAML 
+configuration files into object oriented class hierarchies.
+
+# Who needs Scooch?
+
+Scooch is useful for people who need an accessible interface to enable 
+tweakability in their code. ML practitioners are a good example. They 
+typically write code that is intended to be continuously experimented with and 
+adjusted in response to observations from running the code. As such, it is useful 
+to abstract these tweakable parameters from the code into a config file, providing 
+three major benefits:
+
+ - The config file provides a centralized location for adjustable parameters of 
+ interest in the code, improving iteration and workflow.
+ - Loading, saving and adjusting the configuration of your code is separated 
+ from the many other working variables and data structures that may exist in 
+ code.
+ - The configuration of any part of the code can be hashed, logged, and indexed, 
+ to provide a record of the code configuration at any one time.
+
+# Why use Scooch?
+
+There are many other projects out there that endeavor to translate config files 
+into parameters in python code, for example:
+
+ - [Gin](https://github.com/google/gin-config)
+ - [Sacred](https://sacred.readthedocs.io/en/stable/index.html)
+ - [Hydra](https://hydra.cc/)
+
+However, what makes Scooch different is that it not only translates config 
+parameters into variables in your code, but into object oriented class 
+hierarchies. This means configurations can benefit from object oriented concepts 
+such as Inheretance, Encapsulation, Abstraction and Polymorphism.
+
+For more information about how to use, and why to use Scooch. Please refer to 
+the [documentation](http://www.mattcmccallum.com/scooch/docs).
```

### Comparing `scooch-1.0.2/README.md` & `scooch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/__init__.py` & `scooch-1.0.4/scooch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2023 Pandora Media, LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,11 +22,12 @@
 
 from .config import *
 from .configurable import *
 from .config_list import *
 from .config_collection import *
 from .config_factory import *
 from .param import Param
+from .alias_param import AliasParam
 from .configurable_factory import ConfigurableFactory
 
 # TODO [matt.c.mccallum 01.05.21]: Remove the two below in favor of the config factory, once legacy codebases are updated.
 from .configurize_helper import configurize
```

### Comparing `scooch-1.0.2/scooch/cli/__init__.py` & `scooch-1.0.4/scooch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/cli/cli.py` & `scooch-1.0.4/scooch/cli/cli.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/cli/export.py` & `scooch-1.0.4/scooch/cli/export.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/cli/options.py` & `scooch-1.0.4/scooch/cli/options.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/config.py` & `scooch-1.0.4/scooch/config.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/config_collection.py` & `scooch-1.0.4/scooch/config_collection.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/config_factory.py` & `scooch-1.0.4/scooch/config_factory.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/config_list.py` & `scooch-1.0.4/scooch/config_list.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/configurable.py` & `scooch-1.0.4/scooch/configurable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2023 Pandora Media, LLC.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -43,29 +43,31 @@
     
     __PARAMS__ = {} # <= Parameters that can be specified in the class's configuration
 
     __CONFIGURABLES__ = {} # <= Parameters that are Scooch configurables and will be constructed according to the configuration dicts specified in the Config
 
     __PARAM_DEFAULTS__ = {} # <= Parameters that are optional, and if not provided, will assume default values
 
+    __PARAM_ALIASES__ = {} # <= Parameters that are not configurable, but are derived from other parameter values
+
     def __init__(self, cfg):
         """
         **Constructor.**
 
         Args:
             cfg: dict - An object providing the configuration parameters for this object.
         """
         # TODO [matt.c.mccallum 11.04.21]: Gracefully handle the error case that the top-level dictionary is not a single key value corresponding to a class...
         if not cfg[self.__class__.__name__]:
             self._cfg = {self.__class__.__name__: {}}
         else:
             # Save configuration dictionary
             self._cfg = cfg
 
-        required_config = list(self.__PARAMS__.keys())
+        required_config = [ky for ky in self.__PARAMS__.keys()]
 
         # Populate defaults
         self._populate_defaults_recurse(self._cfg[self.__class__.__name__], self.__PARAM_DEFAULTS__)
 
         # Verify configuration
         # NOTE [matt.c.mccallum 12.16.20]: Just do this for this configurable, all sub-configurables will be verified upon their construction, respectively.
         self._verify_config(self._cfg[self.__class__.__name__], required_config)
@@ -120,22 +122,45 @@
             if field not in cfg.keys():
                 cfg[field] = value
             elif isinstance(value, dict):
                 # Check the sub fields
                 cls._populate_defaults_recurse(cfg[field], value)
 
         # Populate the defaults of any Configurables that are also encapsulated within this configurable
-        for key, cfg in cfg.items():
+        for key, cfg_val in cfg.items():
             
             # NOTE [matt.c.mccallum 02.23.22]: Do not populate defaults if there is no class specified (e.g., cfg==None)
-            if key in cls.__CONFIGURABLES__ and cfg is not None:
+            if key in cls.__CONFIGURABLES__ and cfg_val is not None:
                 base_class = cls.__CONFIGURABLES__[key]
                 if inspect.isclass(base_class) and issubclass(base_class, Configurable):
-                    subcls = configurable_factory.get_class(base_class, cfg)
-                    subcls.populate_defaults(cfg)
+                    subcls = configurable_factory.get_class(base_class, cfg_val)
+                    subcls.populate_defaults(cfg_val)
+            
+        # Populate the defaults of any aliases that are also encapsulated within this configurable
+        for key in cls.__PARAM_ALIASES__:
+            cls._assign_aliases(cfg, key)
+
+    @classmethod
+    def _assign_aliases(cls, cfg, alias_name):
+        """
+        Populate the specified alias in the provided config dictionary for this class. Note that if
+        this depends on any other alias parameters, then these in turn will be populated also.
+
+        Args:
+            cfg: dict() - A config dictionary for this class to have aliases populated in.
+
+            alias_name: str - The name of the alias parameter to populate in the provided config 
+            dictionary, based on the parameters that already exist there.
+        """
+        param_transform, transform_args = cls.__PARAM_ALIASES__[alias_name]
+        for arg in transform_args:
+            if arg in cls.__PARAM_ALIASES__ and arg not in cfg:
+                cls._assign_aliases(cfg, arg)
+        args = [cfg[ky] for ky in transform_args]
+        cfg[alias_name] = param_transform(*args)
 
     def _verify_config(self, cfg, template):
         """
         Checks that all the required fields in the object configuration are there,
         and any fields that aren't in the object configuration, aren't there.
 
         Args:
```

### Comparing `scooch-1.0.2/scooch/configurable_factory.py` & `scooch-1.0.4/scooch/configurable_factory.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/configurize_helper.py` & `scooch-1.0.4/scooch/configurize_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Third party imports
 # None.
 
 # Local imports
 from .configurable import Configurable
 
 
-def configurize(cls=None, base_class=None, init_base_on_construction=True):
+def configurize(cls=None, base_class=None, name_prefix='Scooch', init_base_on_construction=True):
     """
     Takes a class and makes it scooch configurable. This will prepend "Conf" to the class name
     to distinguish it from the class definition. The returned / transformed class will be accessible
     via the name assigned in code, although it must be referred to as "Conf<original_class_name>" in
     scooch config files.
 
     Args:
@@ -38,28 +38,30 @@
         base_class: class - A python SCOOCH class that the newly minted scooch configurable class will inherit 
         from.
 
     Returns:
         class - The augmented Configurable class that may be configured via scooch.
     """
 
-    def configurize_impl(cls, base_cls=None, init_base_on_construction=True):
+    def configurize_impl(cls, base_cls=None, name_prefix='Scooch', init_base_on_construction=True):
 
         # TODO [matt.c.mccallum 11.08.21]: Check the class `cls` is not already `Configurable`
         # TODO [matt.c.mccallum 11.08.21]: Check that `base_cls`` is `Configurable`
         # TODO [matt.c.mccallum 11.08.21]: Inherit class documentation too
 
         if base_cls is None:
             base_cls = Configurable
 
         class DerivedConfigurable(base_cls, cls):
             """
             """
 
-            __SCOOCH_NAME__ = 'Scooch' + cls.__name__
+            __SCOOCH_NAME__ = name_prefix + cls.__name__
+
+            # TODO [matt.c.mccallum 11.29.23]: Add option to exclude / delete parameters here.
 
             # TODO [matt.c.mccallum 11.08.21]: Add type info here
             _BASE_PARAMS = {param: f'<> - Parameter derived by extending base class: {cls.__name__}' for param in inspect.signature(cls.__init__).parameters.keys()}
             _BASE_PARAM_DEFAULTS = {param: val.default for param, val in inspect.signature(cls.__init__).parameters.items() if hasattr(val, 'default') and val.default != val.empty}        
             _NAME = base_cls.__name__
 
             __PARAMS__ = {ky: val for ky, val in _BASE_PARAMS.items() if ky not in ['self', 'args', 'kwargs']}
@@ -93,14 +95,14 @@
                 cls.__init__(self, *self._star_args, **self._star_kwargs)
 
         return DerivedConfigurable
 
     if base_class is None and cls is None:
         return None
     if base_class is None:
-        return configurize_impl(cls)
+        return configurize_impl(cls, name_prefix=name_prefix, init_base_on_construction=init_base_on_construction)
     elif cls is None:
-        return functools.partial(configurize_impl, base_cls=base_class, init_base_on_construction=init_base_on_construction)
+        return functools.partial(configurize_impl, base_cls=base_class, name_prefix=name_prefix, init_base_on_construction=init_base_on_construction)
     else:
-        return configurize_impl(cls, base_class, init_base_on_construction)
+        return configurize_impl(cls, base_class, name_prefix, init_base_on_construction)
```

### Comparing `scooch-1.0.2/scooch/generic.py` & `scooch-1.0.4/scooch/generic.py`

 * *Files identical despite different names*

### Comparing `scooch-1.0.2/scooch/param.py` & `scooch-1.0.4/scooch/param.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         Args:
             instance: Configurable - The instance of the class that this Param is an 
             attribute of.
 
             owner: Configurable - The class that this Param is a Param of.
         """
         # TODO [matt.c.mccallum 11.04.21]: Make sure owner is of type Configurable
+
+        # If called on the class (i.e., no instance), then return the parameter itself
+        if instance is None:
+            return self
+        # Otherwise return the value
         return instance._config_instances[self._name]
 
     def __set__(self, instance, value):
         """
         Sets the value of a parameter, keeping this separated from the object's config that
         was provided upon construction.
```

### Comparing `scooch-1.0.2/scooch.egg-info/PKG-INFO` & `scooch-1.0.4/scooch.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,19 @@
 Metadata-Version: 2.1
 Name: scooch
-Version: 1.0.2
+Version: 1.0.4
 Summary: A python module for configuring hierarchical class structures in yaml with defaults
 Home-page: http://www.mattcmccallum.com/scooch/docs
 Author: Matt C. McCallum
 Author-email: scooch@mattcmccallum.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.mattcmccallum.com/scooch/docs
 Project-URL: Bug Reports, https://github.com/PandoraMedia/scooch/issues
 Project-URL: Source, https://github.com/PandoraMedia/scooch
-Description: 
-        # Scooch
-        
-        Scooch is a recursive acronym for **S**cooch **C**onfigures **O**bject 
-        **O**riented **C**lass **H**ierarchies, and that's exactly what this package 
-        does. It is a configuration package for python codebases that simplifies the 
-        problem of configuring parameters in python code by translating YAML 
-        configuration files into object oriented class hierarchies.
-        
-        # Who needs Scooch?
-        
-        Scooch is useful for people who need an accessible interface to enable 
-        tweakability in their code. ML practitioners are a good example. They 
-        typically write code that is intended to be continuously experimented with and 
-        adjusted in response to observations from running the code. As such, it is useful 
-        to abstract these tweakable parameters from the code into a config file, providing 
-        three major benefits:
-        
-         - The config file provides a centralized location for adjustable parameters of 
-         interest in the code, improving iteration and workflow.
-         - Loading, saving and adjusting the configuration of your code is separated 
-         from the many other working variables and data structures that may exist in 
-         code.
-         - The configuration of any part of the code can be hashed, logged, and indexed, 
-         to provide a record of the code configuration at any one time.
-        
-        # Why use Scooch?
-        
-        There are many other projects out there that endeavor to translate config files 
-        into parameters in python code, for example:
-        
-         - [Gin](https://github.com/google/gin-config)
-         - [Sacred](https://sacred.readthedocs.io/en/stable/index.html)
-         - [Hydra](https://hydra.cc/)
-        
-        However, what makes Scooch different is that it not only translates config 
-        parameters into variables in your code, but into object oriented class 
-        hierarchies. This means configurations can benefit from object oriented concepts 
-        such as Inheretance, Encapsulation, Abstraction and Polymorphism.
-        
-        For more information about how to use, and why to use Scooch. Please refer to 
-        the [documentation](http://www.mattcmccallum.com/scooch/docs).
-        
 Keywords: scooch python configuration machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -68,7 +24,56 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: sphinx
+Requires-Dist: sphinx_rtd_theme==0.5.1
+Requires-Dist: ruamel.yaml==0.16.12
+Requires-Dist: click==8.1.7
+
+
+# Scooch
+
+Scooch is a recursive acronym for **S**cooch **C**onfigures **O**bject 
+**O**riented **C**lass **H**ierarchies, and that's exactly what this package 
+does. It is a configuration package for python codebases that simplifies the 
+problem of configuring parameters in python code by translating YAML 
+configuration files into object oriented class hierarchies.
+
+# Who needs Scooch?
+
+Scooch is useful for people who need an accessible interface to enable 
+tweakability in their code. ML practitioners are a good example. They 
+typically write code that is intended to be continuously experimented with and 
+adjusted in response to observations from running the code. As such, it is useful 
+to abstract these tweakable parameters from the code into a config file, providing 
+three major benefits:
+
+ - The config file provides a centralized location for adjustable parameters of 
+ interest in the code, improving iteration and workflow.
+ - Loading, saving and adjusting the configuration of your code is separated 
+ from the many other working variables and data structures that may exist in 
+ code.
+ - The configuration of any part of the code can be hashed, logged, and indexed, 
+ to provide a record of the code configuration at any one time.
+
+# Why use Scooch?
+
+There are many other projects out there that endeavor to translate config files 
+into parameters in python code, for example:
+
+ - [Gin](https://github.com/google/gin-config)
+ - [Sacred](https://sacred.readthedocs.io/en/stable/index.html)
+ - [Hydra](https://hydra.cc/)
+
+However, what makes Scooch different is that it not only translates config 
+parameters into variables in your code, but into object oriented class 
+hierarchies. This means configurations can benefit from object oriented concepts 
+such as Inheretance, Encapsulation, Abstraction and Polymorphism.
+
+For more information about how to use, and why to use Scooch. Please refer to 
+the [documentation](http://www.mattcmccallum.com/scooch/docs).
```

### Comparing `scooch-1.0.2/scooch.egg-info/SOURCES.txt` & `scooch-1.0.4/scooch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 scooch/__init__.py
+scooch/alias_param.py
 scooch/config.py
 scooch/config_collection.py
 scooch/config_factory.py
 scooch/config_list.py
 scooch/configurable.py
 scooch/configurable_factory.py
 scooch/configurable_meta.py
```

### Comparing `scooch-1.0.2/setup.py` & `scooch-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 
 For more information about how to use, and why to use Scooch. Please refer to 
 the [documentation](http://www.mattcmccallum.com/scooch/docs).
 """
 
 
 REQUIRED_PACKAGES = [
-    'pyyaml==5.4.1',
+    'pyyaml==6.0.1',
     'sphinx',
     'sphinx_rtd_theme==0.5.1',
     'ruamel.yaml==0.16.12',
-    'click==8.0.0a1'
+    'click==8.1.7'
 ]
 
 class MakeReqsCommand(distutils.cmd.Command):
   """A custom command to export requirements to a requirements.txt file."""
 
   description = 'Export requirements to a requirements.txt file.'
   user_options = []
@@ -101,15 +101,15 @@
 
 
 setuptools.setup(
     cmdclass={
         'make_reqs': MakeReqsCommand
     },
     name='scooch',
-    version='1.0.2',
+    version='1.0.4',
     description='A python module for configuring hierarchical class structures in yaml with defaults',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.mattcmccallum.com/scooch/docs",
     author="Matt C. McCallum",
     author_email="scooch@mattcmccallum.com",
     classifiers=[
```

