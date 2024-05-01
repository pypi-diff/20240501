# Comparing `tmp/parameterframe-0.0.1.tar.gz` & `tmp/parameterframe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.0.1.tar", last modified: Sun Apr 21 22:44:11 2024, max compression
+gzip compressed data, was "parameterframe-0.0.2.tar", last modified: Wed May  1 00:04:14 2024, max compression
```

## Comparing `parameterframe-0.0.1.tar` & `parameterframe-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:11.404351 parameterframe-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-21 22:41:17.000000 parameterframe-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-04-21 22:44:11.404351 parameterframe-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-21 22:41:17.000000 parameterframe-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:11.404351 parameterframe-0.0.1/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 22:44:10.000000 parameterframe-0.0.1/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68147 2024-04-21 22:44:10.000000 parameterframe-0.0.1/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:11.404351 parameterframe-0.0.1/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 22:44:11.000000 parameterframe-0.0.1/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:44:11.404351 parameterframe-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-01 00:01:16.000000 parameterframe-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-05-01 00:04:14.798398 parameterframe-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-01 00:01:16.000000 parameterframe-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69559 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:14.798398 parameterframe-0.0.2/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 00:04:14.000000 parameterframe-0.0.2/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:04:14.798398 parameterframe-0.0.2/setup.cfg
```

### Comparing `parameterframe-0.0.1/LICENSE` & `parameterframe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.0.1/PKG-INFO` & `parameterframe-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `parameterframe-0.0.1/README.md` & `parameterframe-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 It provides a method to output various types of lines and headers, with customizable message and line lengths.
 The purpose is to be integrated into other classes that also use logger.
 
 [module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
 
 A tool to run experiments based on defined grid and function with single iteration.
 
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
 
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
@@ -44,15 +44,15 @@
 with a use of more expensive, slower or simply no-existant method.
 
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
-[module](python_modules/parameterframe.py) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -scema](docs/parameterframe-scema.png) | [drawio: -usage](docs/parameterframe-usage.png) - Parameter frame
+[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameter frame
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
```

### Comparing `parameterframe-0.0.1/parameterframe/parameterframe.py` & `parameterframe-0.0.2/parameterframe/parameterframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,123 @@
 
         db_remote_handler.insert_data(
             data = [d for _, d in self.db_handler.data.items()]
         )
 
         return True
 
+    def push_tables(self,
+                      solution_description : list,
+                      solution_parameter_set : list,
+                      parameter_set : list,
+                      parameter_set_description : list,
+                      parameter_description : list,
+                      parameter_attribute : list,
+                      attribute_values : list):
+
+        """
+        Pushes tables with database handler
+        """
+
+
+        self.add_entries(table_name = 'solution_description',
+                                            entries = solution_description)
+        self.add_entries(table_name = 'solution_parameter_set',
+                                            entries = solution_parameter_set)
+        self.add_entries(table_name = 'parameter_set',
+                                            entries = parameter_set)
+        self.add_entries(table_name = 'parameter_set_description',
+                                            entries = parameter_set_description)
+        self.add_entries(table_name = 'parameter_description',
+                                            entries = parameter_description)
+        self.add_entries(table_name = 'parameter_attribute',
+                                            entries = parameter_attribute)
+        self.add_entries(table_name = 'attribute_values',
+                                            entries = attribute_values)
+
+        self.commit()
+
+        return True
+
+    def pull_tables(self,
+                      solution_id : list = None,
+                      parameter_set_id : list = None):
+
+        """
+        Pulls commited tables from database for selected solutions
+        """
+
+        if solution_id is None:
+            raise ValueError("Provide solution_id!")
+
+        if parameter_set_id is None:
+            raise ValueError("Provide parameter_set_id!")
+
+        # fetch tables with solution and parameter_set_ids
+        self.fetch_entries(
+            filters={'table_name' : ['solution_description',
+                                          'solution_parameter_set',
+                                          'parameter_set',
+                                          'parameter_set_description'],
+                          'solution_id': [solution_id, None],
+                          'parameter_set_id' :[parameter_set_id, None]})
+
+        # get parameter_id for fetching next tables
+        dict_param_ids = self.get_entries(
+            table_name = 'parameter_set',
+            return_keys=['parameter_id'])
+
+        param_ids = [dict_param_id['parameter_id'] for dict_param_id in dict_param_ids]
+
+        # fetch tables with parameter_ids
+        self.fetch_entries(
+            filters={'table_name' : ['parameter_description',
+                                          'parameter_attribute'],
+                          'parameter_id': param_ids})
+
+        # get attribute_ids for fetching next tables
+        dict_attribute_ids = self.get_entries(
+            table_name = 'parameter_attribute',
+            return_keys=['attribute_id'])
+
+        attribute_ids = [dict_attribute_id['attribute_id'] \
+            for dict_attribute_id in dict_attribute_ids]
+
+        # fetch final tables
+        self.fetch_entries(
+            filters={'table_name' : 'attribute_values',
+                          'attribute_id': attribute_ids})
+
+        # get table lists from connector
+        solution_description = self.get_entries(
+    table_name = 'solution_description')
+        solution_parameter_sets = self.get_entries(
+    table_name = 'solution_parameter_set')
+        parameter_sets = self.get_entries(
+    table_name = 'parameter_set')
+        parameter_set_descriptions = self.get_entries(
+    table_name = 'parameter_set_description')
+        parameter_descriptions = self.get_entries(
+    table_name = 'parameter_description')
+        parameter_attributes = self.get_entries(
+    table_name = 'parameter_attribute')
+        attribute_values = self.get_entries(
+    table_name = 'attribute_values')
+
+        return (
+            solution_description,
+            solution_parameter_sets,
+            parameter_sets,
+            parameter_set_descriptions,
+            parameter_descriptions,
+            parameter_attributes,
+            attribute_values
+        )
+
+
 
 @attr.s
 class FileTypeHandler:
 
     """
     Handles raw files, processes them for storage
     and reconstructs when pulling from storage.
@@ -1408,30 +1517,23 @@
             parameter_description,
             parameter_attribute,
             attribute_values) = self._prep_tables_for_pushing(
                 solution_id = solution_id,
                 parameter_set_ids = parameter_set_ids
             )
 
-        self.database_connector.add_entries(table_name = 'solution_description',
-                                            entries = solution_description)
-        self.database_connector.add_entries(table_name = 'solution_parameter_set',
-                                            entries = solution_parameter_set)
-        self.database_connector.add_entries(table_name = 'parameter_set',
-                                            entries = parameter_set)
-        self.database_connector.add_entries(table_name = 'parameter_set_description',
-                                            entries = parameter_set_description)
-        self.database_connector.add_entries(table_name = 'parameter_description',
-                                            entries = parameter_description)
-        self.database_connector.add_entries(table_name = 'parameter_attribute',
-                                            entries = parameter_attribute)
-        self.database_connector.add_entries(table_name = 'attribute_values',
-                                            entries = attribute_values)
-
-        self.database_connector.commit()
+        self.database_connector.push_tables(
+            solution_description,
+            solution_parameter_set,
+            parameter_set,
+            parameter_set_description,
+            parameter_description,
+            parameter_attribute,
+            attribute_values
+        )
 
         return True
 
     def _rebuild_tables_from_pulled_data(self,
                                      solution_id: str,
                                      parameter_set_ids: list,
                                      solution_description,
@@ -1534,89 +1636,47 @@
 
 
     def pull_solution(self,
                       solution_id : list = None,
                       parameter_set_id : list = None):
 
         """
-        Pushes commited tables to database handler for selected solutions
+        Pulls commited tables from database for selected solutions
         """
 
         if solution_id is None:
             raise ValueError("Provide solution_id!")
 
         if parameter_set_id is None:
             raise ValueError("Provide parameter_set_id!")
 
-        # fetch tables with solution and parameter_set_ids
-        self.database_connector.fetch_entries(
-            filters={'table_name' : ['solution_description',
-                                          'solution_parameter_set',
-                                          'parameter_set',
-                                          'parameter_set_description'],
-                          'solution_id': [solution_id, None],
-                          'parameter_set_id' :[parameter_set_id, None]})
-
-        # get parameter_id for fetching next tables
-        dict_param_ids = self.database_connector.get_entries(
-            table_name = 'parameter_set',
-            return_keys=['parameter_id'])
-
-        param_ids = [dict_param_id['parameter_id'] for dict_param_id in dict_param_ids]
-
-        # fetch tables with parameter_ids
-        self.database_connector.fetch_entries(
-            filters={'table_name' : ['parameter_description',
-                                          'parameter_attribute'],
-                          'parameter_id': param_ids})
-
-        # get attribute_ids for fetching next tables
-        dict_attribute_ids = self.database_connector.get_entries(
-            table_name = 'parameter_attribute',
-            return_keys=['attribute_id'])
-
-        attribute_ids = [dict_attribute_id['attribute_id'] for dict_attribute_id in dict_attribute_ids]
-
-        # fetch final tables
-        self.database_connector.fetch_entries(
-            filters={'table_name' : 'attribute_values',
-                          'attribute_id': attribute_ids})
-
-        # get table lists from connector
-        solution_description = self.database_connector.get_entries(
-    table_name = 'solution_description')
-        solution_parameter_sets = self.database_connector.get_entries(
-    table_name = 'solution_parameter_set')
-        parameter_sets = self.database_connector.get_entries(
-    table_name = 'parameter_set')
-        parameter_set_descriptions = self.database_connector.get_entries(
-    table_name = 'parameter_set_description')
-        parameter_descriptions = self.database_connector.get_entries(
-    table_name = 'parameter_description')
-        parameter_attributes = self.database_connector.get_entries(
-    table_name = 'parameter_attribute')
-        attribute_values = self.database_connector.get_entries(
-    table_name = 'attribute_values')
+        (solution_description,
+         solution_parameter_sets,
+         parameter_sets,
+         parameter_set_descriptions,
+         parameter_descriptions,
+         parameter_attributes,
+         attribute_values) = self.database_connector.pull_tables(
+            solution_id = solution_id,
+            parameter_set_id = parameter_set_id
+        )
 
         # get table lists into commited
         self._rebuild_tables_from_pulled_data(
             solution_id = solution_id,
             parameter_set_ids = [parameter_set_id],
             solution_description = solution_description,
             solution_parameter_sets = solution_parameter_sets,
             parameter_sets = parameter_sets,
             parameter_set_descriptions = parameter_set_descriptions,
             parameter_descriptions = parameter_descriptions,
             parameter_attributes = parameter_attributes,
             attribute_values = attribute_values
         )
 
-
-
-
     def _change_deployment_status(self,
                                  deployment_status : str,
                                  solution_id : str = None,
                                 solution_name : str = None,
                                 parameter_set_id : str = None,
                                 parameter_set_name : str = None,
                                 remote : bool = False):
```

### Comparing `parameterframe-0.0.1/parameterframe/setup.py` & `parameterframe-0.0.2/parameterframe/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'mocker_db==0.1.1', 'dill', 'pyyaml', 'attrs'],
+    install_requires=['### parameterframe.py', 'attrs', 'mocker_db==0.1.1', 'pyyaml', 'dill'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.0.1"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.0.2"
 )
```

### Comparing `parameterframe-0.0.1/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.0.2/parameterframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

