# Comparing `tmp/interopt-0.1.1.tar.gz` & `tmp/interopt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interopt-0.1.1.tar", last modified: Wed Apr 17 00:19:05 2024, max compression
+gzip compressed data, was "interopt-0.1.2.tar", last modified: Wed May  1 03:27:33 2024, max compression
```

## Comparing `interopt-0.1.1.tar` & `interopt-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-04-17 00:19:05.528967 interopt-0.1.1/PKG-INFO
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:08:52.000000 interopt-0.1.1/README.md
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.525633 interopt-0.1.1/interopt/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       32 2024-02-27 12:30:04.000000 interopt-0.1.1/interopt/__init__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      856 2024-03-27 12:26:56.000000 interopt-0.1.1/interopt/__main__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      310 2024-02-26 09:45:20.000000 interopt-0.1.1/interopt/definition.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4581 2024-03-29 18:29:35.000000 interopt-0.1.1/interopt/parameter.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt/runner/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:52:11.000000 interopt-0.1.1/interopt/runner/__init__.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt/runner/grpc_runner/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       29 2024-02-25 07:25:19.000000 interopt-0.1.1/interopt/runner/grpc_runner/__init__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4705 2024-03-13 12:40:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     5201 2024-03-13 12:40:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.pyi
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4270 2024-03-13 12:41:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2_grpc.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     2705 2024-03-27 13:19:28.000000 interopt-0.1.1/interopt/runner/grpc_runner/main.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     3706 2024-03-13 11:15:32.000000 interopt-0.1.1/interopt/runner/grpc_runner/server.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4140 2024-04-05 20:08:17.000000 interopt-0.1.1/interopt/runner/model.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     1462 2024-03-27 12:36:55.000000 interopt-0.1.1/interopt/search_space.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)    12472 2024-04-05 20:36:54.000000 interopt-0.1.1/interopt/study.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt.egg-info/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/PKG-INFO
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      630 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/SOURCES.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        1 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/dependency_links.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       67 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/requires.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        9 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/top_level.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       38 2024-04-17 00:19:05.528967 interopt-0.1.1/setup.cfg
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      601 2024-04-17 00:16:53.000000 interopt-0.1.1/setup.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-05-01 03:27:33.156071 interopt-0.1.2/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-05-01 03:27:33.156071 interopt-0.1.2/PKG-INFO
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:08:52.000000 interopt-0.1.2/README.md
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-05-01 03:27:33.152737 interopt-0.1.2/interopt/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       32 2024-02-27 12:30:04.000000 interopt-0.1.2/interopt/__init__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      856 2024-03-27 12:26:56.000000 interopt-0.1.2/interopt/__main__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      310 2024-02-26 09:45:20.000000 interopt-0.1.2/interopt/definition.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     2849 2024-05-01 00:12:20.000000 interopt-0.1.2/interopt/parameter.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-05-01 03:27:33.152737 interopt-0.1.2/interopt/runner/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:52:11.000000 interopt-0.1.2/interopt/runner/__init__.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-05-01 03:27:33.156071 interopt-0.1.2/interopt/runner/grpc_runner/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       29 2024-02-25 07:25:19.000000 interopt-0.1.2/interopt/runner/grpc_runner/__init__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4705 2024-03-13 12:40:56.000000 interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     5201 2024-03-13 12:40:56.000000 interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2.pyi
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4270 2024-03-13 12:41:56.000000 interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2_grpc.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     2831 2024-05-01 03:23:07.000000 interopt-0.1.2/interopt/runner/grpc_runner/main.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     3332 2024-05-01 03:24:19.000000 interopt-0.1.2/interopt/runner/grpc_runner/server.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4140 2024-04-05 20:08:17.000000 interopt-0.1.2/interopt/runner/model.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     1462 2024-03-27 12:36:55.000000 interopt-0.1.2/interopt/search_space.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)    12615 2024-05-01 03:22:26.000000 interopt-0.1.2/interopt/study.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-05-01 03:27:33.156071 interopt-0.1.2/interopt.egg-info/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-05-01 03:27:33.000000 interopt-0.1.2/interopt.egg-info/PKG-INFO
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      630 2024-05-01 03:27:33.000000 interopt-0.1.2/interopt.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        1 2024-05-01 03:27:33.000000 interopt-0.1.2/interopt.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       67 2024-05-01 03:27:33.000000 interopt-0.1.2/interopt.egg-info/requires.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        9 2024-05-01 03:27:33.000000 interopt-0.1.2/interopt.egg-info/top_level.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       38 2024-05-01 03:27:33.156071 interopt-0.1.2/setup.cfg
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      601 2024-05-01 03:27:18.000000 interopt-0.1.2/setup.py
```

### Comparing `interopt-0.1.1/interopt/__main__.py` & `interopt-0.1.2/interopt/__main__.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.py` & `interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.pyi` & `interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2_grpc.py` & `interopt-0.1.2/interopt/runner/grpc_runner/config_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/runner/grpc_runner/main.py` & `interopt-0.1.2/interopt/runner/grpc_runner/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import ast
 #import grpc
 import grpc.aio
 
+import logging
+
 # Import param enum type
 from interopt.parameter import ParamType, Param
 
 import interopt.runner.grpc_runner.config_service_pb2 as cs
 import interopt.runner.grpc_runner.config_service_pb2_grpc as cs_grpc
 
 def value_to_param(value, param_type: ParamType):
@@ -47,17 +49,19 @@
 
     async with grpc.aio.insecure_channel(grpc_url) as channel:
         stub = cs_grpc.ConfigurationServiceStub(channel)
         request = cs.ConfigurationRequest(
             configurations=config,
             output_data_file="test"
         )
+        logging.info(f"Sending request: {request}")
         try:
             response = await stub.RunConfigurationsClientServer(request)
-            #print(f"Received response: {response}")
+            logging.info(f"Received response: {response}")
+            print(f"Received response: {response}")
             for metric in response.metrics:
                 result[metric.name] = metric.values
             #print(f"Received result: {result}")
         except grpc.aio.AioRpcError as e:
             print(e.with_traceback(None))
             # Extracting the status code
             status_code = e.code()
```

### Comparing `interopt-0.1.1/interopt/runner/grpc_runner/server.py` & `interopt-0.1.2/interopt/runner/grpc_runner/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import grpc
 import asyncio
+import logging
 
 import interopt.runner.grpc_runner.config_service_pb2 as cs
 import interopt.runner.grpc_runner.config_service_pb2_grpc as cs_grpc
 
 from interopt.study import Study
 
+# Configure logging
+#logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class ConfigurationServiceServicer(cs_grpc.ConfigurationServiceServicer):
     def __init__ (self, study: Study):
         self.study = study
 
     async def RunConfigurationsClientServer(self, request, context):
-        #print(f"Received request: {request}")
-        #print(f"Received configs: {request.configurations.parameters}")
-        #print(f"Received request: {request}")
+        logging.info(f"Received request: {request}")
         query = await self.convert_request(request)
-        #print(f"Converted request: {query}")
         # Sort the query to ensure consistent ordering
         parameter_names = self.study.get_parameter_names()
         query = {name: query[name] for name in parameter_names}
-        #print(f"Sorted converted request: {query}")
+        logging.info(f"Converted request: {query}")
 
-        #print(f"Converted request: {query}")
         result = await self.study.query_async(query)
 
-        #print(f"Results 2: {result}")
+        logging.info(f"Results: {result}")
         result = await self.convert_response(result)
-        #print(f"Converted response: {result}")
+        logging.info(f"Converted response: {result}")
         return result
 
     async def Shutdown(self, request, context):
         if request.shutdown:
-            print("Shutdown requested")
+            logging.warning("Shutdown requested")
             # Add async shutdown logic here if necessary
             return cs.ShutdownResponse(success=True)
         return cs.ShutdownResponse(success=False)
 
 
     async def convert_request(self, request):
         query = {}
@@ -55,25 +54,17 @@
             elif param.HasField('permutation_param'):
                 vals = param.permutation_param.values
                 query[key] = str(tuple(vals))
             # Add additional elif blocks for other parameter types as needed
         return query
 
     async def convert_response(self, result):
-        #print(f"Metrics: {result}")
-        #print(f"Metrics: {cs.Metric(values=[result['compute_time']])}")
-        #metrics = [
-        #    cs.Metric(values=metric)
-        #    for metric in result
-        #]
         metrics = []
         for obj in self.study.enabled_objectives:
             metrics.append(cs.Metric(name=obj, values=[result[obj]]))
-        #metrics = [cs.Metric(values=[result['compute_time']])]
-        #print(f"Metrics: {metrics}")
         return cs.ConfigurationResponse(
             metrics=metrics,
             timestamps=cs.Timestamp(timestamp=int()),
             feasible=cs.Feasible(value=True)
         )
 
 class Server():
```

### Comparing `interopt-0.1.1/interopt/runner/model.py` & `interopt-0.1.2/interopt/runner/model.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/search_space.py` & `interopt-0.1.2/interopt/search_space.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/interopt/study.py` & `interopt-0.1.2/interopt/study.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import pandas as pd
 import numpy as np
 
 from interopt.runner.grpc_runner import run_config
 from interopt.runner.model import load_models
 from interopt.definition import ProblemDefinition
 
+import logging
+
+logging.basicConfig(filename='app.log', level=logging.DEBUG, filemode='w', format='%(asctime)s - %(levelname)s - %(message)s')
 class TabularDataset:
     def __init__(self, benchmark_name, dataset, parameter_names, objectives, enable_download):
         self.objectives = objectives
         self.tab = None
         self.parameter_names = parameter_names
         self.tab_path = f'datasets/{benchmark_name}_{dataset}.csv'
         if os.path.exists(self.tab_path):
```

### Comparing `interopt-0.1.1/interopt.egg-info/SOURCES.txt` & `interopt-0.1.2/interopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interopt-0.1.1/setup.py` & `interopt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='interopt',
-    version='0.1.1',
+    version='0.1.2',
     author='Jacob Odgård Tørring',
     author_email='jacob.torring@ntnu.no',
     packages=find_packages(),
     license='LICENSE',
     description='An interoperability layer for black-box optimization',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

