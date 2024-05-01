# Comparing `tmp/datagov_harvesting_logic-0.3.8.tar.gz` & `tmp/datagov_harvesting_logic-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.3.8.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.3.9.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.3.8.tar` & `datagov_harvesting_logic-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1878 2024-04-24 21:07:10.203062 datagov_harvesting_logic-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     5265 2024-04-24 21:07:10.203062 datagov_harvesting_logic-0.3.8/README.md
--rw-r--r--   0        0        0      162 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/__init__.py
--rw-r--r--   0        0        0     4489 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/ckan_utils.py
--rw-r--r--   0        0        0     4464 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/arm.data.json
--rw-r--r--   0        0        0     7830 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
--rw-r--r--   0        0        0    14027 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
--rw-r--r--   0        0        0     7454 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/geospatial.data.json
--rw-r--r--   0        0        0   310979 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/large-spatial.data.json
--rw-r--r--   0        0        0      918 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-catalog.data.json
--rw-r--r--   0        0        0     1059 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
--rw-r--r--   0        0        0     3259 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-identifier-title.data.json
--rw-r--r--   0        0        0     1292 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/numerical-title.data.json
--rw-r--r--   0        0        0     2520 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/ny.data.json
--rw-r--r--   0        0        0     1314 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/reserved-title.data.json
--rw-r--r--   0        0        0     9562 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/usda.gov.data.json
--rw-r--r--   0        0        0     1604 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/catalog.json
--rw-r--r--   0        0        0    23811 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/dataset.json
--rw-r--r--   0        0        0     2158 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/exceptions.py
--rw-r--r--   0        0        0    25444 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/logger_config.py
--rw-r--r--   0        0        0     3859 2024-04-24 21:07:10.211062 datagov_harvesting_logic-0.3.8/harvester/utils.py
--rw-r--r--   0        0        0     2241 2024-04-24 21:07:10.215062 datagov_harvesting_logic-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-04-25 20:32:25.177374 datagov_harvesting_logic-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     5265 2024-04-25 20:32:25.177374 datagov_harvesting_logic-0.3.9/README.md
+-rw-r--r--   0        0        0      162 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/__init__.py
+-rw-r--r--   0        0        0     4489 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     4464 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/arm.data.json
+-rw-r--r--   0        0        0     7830 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
+-rw-r--r--   0        0        0    14027 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
+-rw-r--r--   0        0        0     7454 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/geospatial.data.json
+-rw-r--r--   0        0        0   310979 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/large-spatial.data.json
+-rw-r--r--   0        0        0      918 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-catalog.data.json
+-rw-r--r--   0        0        0     1059 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
+-rw-r--r--   0        0        0     3259 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-identifier-title.data.json
+-rw-r--r--   0        0        0     1292 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/numerical-title.data.json
+-rw-r--r--   0        0        0     2520 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/ny.data.json
+-rw-r--r--   0        0        0     1314 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/reserved-title.data.json
+-rw-r--r--   0        0        0     9562 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/usda.gov.data.json
+-rw-r--r--   0        0        0     1604 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/catalog.json
+-rw-r--r--   0        0        0    23811 2024-04-25 20:32:25.181374 datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/dataset.json
+-rw-r--r--   0        0        0     2158 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/exceptions.py
+-rw-r--r--   0        0        0    25444 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/logger_config.py
+-rw-r--r--   0        0        0     3859 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/harvester/utils.py
+-rw-r--r--   0        0        0     2241 2024-04-25 20:32:25.185374 datagov_harvesting_logic-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.9/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.3.8/LICENSE.md` & `datagov_harvesting_logic-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/README.md` & `datagov_harvesting_logic-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.3.9/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/arm.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/arm.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/geospatial.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/geospatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/large-spatial.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/large-spatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-catalog.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-catalog.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-dataset-fields.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-dataset-fields.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/missing-identifier-title.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/missing-identifier-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/numerical-title.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/numerical-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/ny.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/ny.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/reserved-title.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/reserved-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/jsons/usda.gov.data.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/jsons/usda.gov.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/catalog.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/catalog.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/data/dcatus/schemas/dataset.json` & `datagov_harvesting_logic-0.3.9/harvester/data/dcatus/schemas/dataset.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/exceptions.py` & `datagov_harvesting_logic-0.3.9/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/harvest.py` & `datagov_harvesting_logic-0.3.9/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/logger_config.py` & `datagov_harvesting_logic-0.3.9/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/harvester/utils.py` & `datagov_harvesting_logic-0.3.9/harvester/utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.8/pyproject.toml` & `datagov_harvesting_logic-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
```

### Comparing `datagov_harvesting_logic-0.3.8/PKG-INFO` & `datagov_harvesting_logic-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

