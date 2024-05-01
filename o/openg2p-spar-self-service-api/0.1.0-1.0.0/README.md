# Comparing `tmp/openg2p_spar_self_service_api-0.1.0.tar.gz` & `tmp/openg2p_spar_self_service_api-1.0.0.tar.gz`

## Comparing `openg2p_spar_self_service_api-0.1.0.tar` & `openg2p_spar_self_service_api-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/app.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/config.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/controllers/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/controllers/dfsp_controller.py
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/controllers/selfservice_controller.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/helpers/__init__.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/helpers/response_helper.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/helpers/strategy_helper.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/__init__.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/dfsp.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/login_provider.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/strategy.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/dfsp.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/mapper.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/request.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/tests/test_placeholder.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/.gitignore
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/app.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/config.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/controllers/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/controllers/dfsp_controller.py
+-rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/controllers/selfservice_controller.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/helpers/__init__.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/helpers/response_helper.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/helpers/strategy_helper.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/__init__.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/dfsp.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/login_provider.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/strategy.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/dfsp.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/mapper.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/request.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/tests/test_placeholder.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/.gitignore
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 openg2p_spar_self_service_api-1.0.0/PKG-INFO
```

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/app.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/app.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/config.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/config.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/controllers/dfsp_controller.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/controllers/dfsp_controller.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/controllers/selfservice_controller.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/controllers/selfservice_controller.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/helpers/response_helper.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/helpers/strategy_helper.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/helpers/strategy_helper.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/dfsp.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/dfsp.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/models/strategy.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/models/strategy.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/__init__.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/dfsp.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/dfsp.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/mapper.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/mapper.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/src/openg2p_spar_self_service_api/schemas/response.py` & `openg2p_spar_self_service_api-1.0.0/src/openg2p_spar_self_service_api/schemas/response.py`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/.gitignore` & `openg2p_spar_self_service_api-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/README.md` & `openg2p_spar_self_service_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/pyproject.toml` & `openg2p_spar_self_service_api-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openg2p_spar_self_service_api-0.1.0/PKG-INFO` & `openg2p_spar_self_service_api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openg2p-spar-self-service-api
-Version: 0.1.0
+Version: 1.0.0
 Summary: OpenG2P SPAR Self Service API
 Project-URL: Homepage, https://openg2p.org
 Project-URL: Documentation, https://docs.openg2p.org/
 Project-URL: Repository, https://github.com/OpenG2P/openg2p-spar-self-service
 Project-URL: Source, https://github.com/OpenG2P/openg2p-spar-self-service
 Author-email: OpenG2P <info@openg2p.org>
 License-File: LICENSE
```

