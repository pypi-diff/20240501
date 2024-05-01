# Comparing `tmp/polyapi_python-0.2.4.dev9.tar.gz` & `tmp/polyapi_python-0.2.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.4.dev9.tar", last modified: Tue Apr 23 19:40:46 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.5.dev1.tar", last modified: Wed May  1 14:37:29 2024, max compression
```

## Comparing `polyapi_python-0.2.4.dev9.tar` & `polyapi_python-0.2.5.dev1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.485624 polyapi_python-0.2.4.dev9/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/poly_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:37:29.990818 polyapi_python-0.2.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-01 14:37:29.990818 polyapi_python-0.2.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:37:29.986818 polyapi_python-0.2.5.dev1/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:37:29.990818 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-01 14:37:29.000000 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-01 14:37:29.000000 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:37:29.000000 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-01 14:37:29.000000 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 14:37:29.000000 polyapi_python-0.2.5.dev1/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:37:29.990818 polyapi_python-0.2.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:37:29.986818 polyapi_python-0.2.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-01 14:37:23.000000 polyapi_python-0.2.5.dev1/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.4.dev9/LICENSE` & `polyapi_python-0.2.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/PKG-INFO` & `polyapi_python-0.2.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev9
+Version: 0.2.5.dev1
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev9/README.md` & `polyapi_python-0.2.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/api.py` & `polyapi_python-0.2.5.dev1/polyapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 ) -> {api_response_type}:
     \"""{function_description}
 
     Function ID: {function_id}
     \"""
     resp = execute("{function_type}", "{function_id}", {data})
     return {api_response_type}(resp.json())  # type: ignore
+
+
 """
 
 
 def render_api_function(
     function_type: str,
     function_name: str,
     function_id: str,
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/auth.py` & `polyapi_python-0.2.5.dev1/polyapi/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 """
 
 GET_TOKEN_TEMPLATE = """
 import asyncio
 
 
 class AuthFunctionResponse(TypedDict):
-  status: int
-  data: Any
-  headers: Dict[str, str]
+    status: int
+    data: Any
+    headers: Dict[str, str]
 
 
 async def getToken(clientId: str, clientSecret: str, scopes: List[str], callback, options: Optional[Dict[str, Any]] = None):
     \"""{description}
 
     Function ID: {function_id}
     \"""
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/cli.py` & `polyapi_python-0.2.5.dev1/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/config.py` & `polyapi_python-0.2.5.dev1/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/error_handler.py` & `polyapi_python-0.2.5.dev1/polyapi/error_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import copy
 import socketio  # type: ignore
+from socketio.exceptions import ConnectionError  # type: ignore
 from typing import Any, Callable, Dict, List, Optional
 
 from polyapi.config import get_api_key_and_url
 
 
 # all active webhook handlers, used by unregister_all to cleanup
 active_handlers: List[Dict[str, Any]] = []
@@ -24,34 +25,37 @@
     _, base_url = get_api_key_and_url()
     global client
     client = socketio.AsyncClient()
     await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
 
 
 async def unregister(data: Dict[str, Any]):
-    print(f"stopping error handler for '{data['path']}'...")
+    print(f"Stopping error handler for {data['path']}...")
     assert client
     await client.emit(
         "unregisterErrorHandler",
         data,
         "/events",
     )
 
 
 async def unregister_all():
     _, base_url = get_api_key_and_url()
     # need to reconnect because maybe socketio client disconnected after Ctrl+C?
-    await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
+    try:
+        await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
+    except ConnectionError:
+        pass
     await asyncio.gather(*[unregister(handler) for handler in active_handlers])
 
 
 async def on(
     path: str, callback: Callable, options: Optional[Dict[str, Any]] = None
 ) -> None:
-    print(f"starting error handler for {path}...")
+    print(f"Starting error handler for {path}...")
 
     if not client:
         raise Exception("Client not initialized. Abort!")
 
     api_key, _ = get_api_key_and_url()
     handler_id = None
     data = copy.deepcopy(options or {})
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/execute.py` & `polyapi_python-0.2.5.dev1/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/function_cli.py` & `polyapi_python-0.2.5.dev1/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/generate.py` & `polyapi_python-0.2.5.dev1/polyapi/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,22 @@
     for spec in specs:
         # this needs to stay in sync with logic in parse_specs
         if spec["type"] in SUPPORTED_TYPES:
             supported.append(spec)
 
     full_path = os.path.dirname(os.path.abspath(__file__))
     full_path = os.path.join(full_path, "poly")
-    if not os.path.exists(full_path):
-        os.makedirs(full_path)
-
-    with open(os.path.join(full_path, "specs.json"), "w") as f:
-        f.write(json.dumps(supported))
+    try:
+        if not os.path.exists(full_path):
+            os.makedirs(full_path)
+
+        with open(os.path.join(full_path, "specs.json"), "w") as f:
+            f.write(json.dumps(supported))
+    except Exception as e:
+        print("Failed to cache specs", e)
 
 
 def read_cached_specs() -> List[SpecificationDto]:
     full_path = os.path.dirname(os.path.abspath(__file__))
     full_path = os.path.join(full_path, "poly")
     with open(os.path.join(full_path, "specs.json"), "r") as f:
         return json.loads(f.read())
@@ -172,14 +175,15 @@
         assert resp.status_code == 201, (resp.text, resp.status_code)
 
 
 def render_spec(spec: SpecificationDto):
     function_type = spec["type"]
     function_description = spec["description"]
     function_name = spec["name"]
+    function_context = spec["context"]
     function_id = spec["id"]
 
     arguments: List[PropertySpecification] = []
     return_type = {}
     if spec["function"]:
         arguments = [
             arg for arg in spec["function"]["arguments"]
@@ -219,14 +223,15 @@
             function_description,
             arguments,
             return_type,
         )
     elif function_type == "webhookHandle":
         func_str, func_type_defs = render_webhook_handle(
             function_type,
+            function_context,
             function_name,
             function_id,
             function_description,
             arguments,
             return_type,
         )
     return func_str, func_type_defs
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/schema.py` & `polyapi_python-0.2.5.dev1/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/server.py` & `polyapi_python-0.2.5.dev1/polyapi/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Tuple
 
 from polyapi.typedefs import PropertySpecification
 from polyapi.utils import camelCase, add_type_import_path, parse_arguments, get_type_and_def
 
 SERVER_DEFS_TEMPLATE = """
-from typing import List, Dict, Any, TypedDict
+from typing import List, Dict, Any, TypedDict, Callable
 {args_def}
 {return_type_def}
 """
 
 SERVER_FUNCTION_TEMPLATE = """
 def {function_name}(
 {args}
@@ -18,14 +18,16 @@
     Function ID: {function_id}
     \"""
     resp = execute("{function_type}", "{function_id}", {data})
     try:
         return {return_action}
     except:
         return resp.text
+
+
 """
 
 
 def render_server_function(
     function_type: str,
     function_name: str,
     function_id: str,
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/typedefs.py` & `polyapi_python-0.2.5.dev1/polyapi/typedefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     required: bool
     nullable: NotRequired[bool]
     type: "PropertyType"
 
 
 class PropertyType(TypedDict):
     kind: Literal['void', 'primitive', 'array', 'object', 'function', 'plain']
+    spec: NotRequired[Dict]
     name: NotRequired[str]
     type: NotRequired[str]
     items: NotRequired['PropertyType']
     schema: NotRequired[Dict]
     properties: NotRequired[List[PropertySpecification]]
     typeName: NotRequired[str]
     value: NotRequired[str]
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/utils.py` & `polyapi_python-0.2.5.dev1/polyapi/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from polyapi.constants import BASIC_PYTHON_TYPES
 from polyapi.typedefs import PropertySpecification, PropertyType
 from polyapi.schema import generate_schema_types, clean_title, map_primitive_types
 
 
 # this string should be in every __init__ file.
 # it contains all the imports needed for the function or variable code to run
-CODE_IMPORTS = "from typing import List, Dict, Any, TypedDict, Optional\nimport requests\nimport socketio  # type: ignore\nfrom polyapi.config import get_api_key_and_url\nfrom polyapi.execute import execute, execute_post, variable_get, variable_update\n\n"
+CODE_IMPORTS = "from typing import List, Dict, Any, TypedDict, Optional, Callable\nimport logging\nimport requests\nimport socketio  # type: ignore\nfrom polyapi.config import get_api_key_and_url\nfrom polyapi.execute import execute, execute_post, variable_get, variable_update\n\n"
 
 
 def init_the_init(full_path: str) -> None:
     init_path = os.path.join(full_path, "__init__.py")
     if not os.path.exists(init_path):
         with open(init_path, "w") as f:
             f.write(CODE_IMPORTS)
@@ -57,14 +57,18 @@
 def print_red(s: str):
     print(Fore.RED + s + Style.RESET_ALL)
 
 
 def add_type_import_path(function_name: str, arg: str) -> str:
     """ if not basic type, coerce to camelCase and add the import path
     """
+    # for now, just treat Callables as basic types
+    if arg.startswith("Callable"):
+        return arg
+
     if arg in BASIC_PYTHON_TYPES:
         return arg
 
     if arg.startswith("List["):
         sub = arg[5:-1]
         if sub in BASIC_PYTHON_TYPES:
             return arg
@@ -138,14 +142,33 @@
                 except:
                     logging.exception(f"Error when generating schema type: {schema}")
                     return "List", ""
             else:
                 return "Any", ""
         else:
             return "Dict", ""
+    elif type_spec["kind"] == "function":
+        arg_types = []
+        arg_defs = []
+        if "spec" in type_spec:
+            return_type, _ = get_type_and_def(type_spec["spec"]["returnType"])
+            if return_type not in BASIC_PYTHON_TYPES:
+                # for now only Python only supports basic types as return types
+                return_type = "Any"
+
+            for argument in type_spec["spec"]["arguments"]:
+                arg_type, arg_def = get_type_and_def(argument["type"])
+                arg_types.append(arg_type)
+                if arg_def:
+                    arg_defs.append(arg_def)
+
+            final_arg_type = "Callable[[{}], {}]".format(", ".join(arg_types), return_type)
+            return final_arg_type, "\n".join(arg_defs)
+        else:
+            return "Callable", ""
     elif type_spec["kind"] == "any":
         return "Any", ""
     else:
         return "Any", ""
 
 
 def parse_arguments(function_name: str, arguments: List[PropertySpecification]) -> Tuple[str, str]:
@@ -161,8 +184,17 @@
         if description:
             if idx == len(arguments) - 1:
                 arg_string += f"  # {description}\n"
             else:
                 arg_string += f",  # {description}\n"
         else:
             arg_string += ",\n"
-    return arg_string.rstrip("\n"), "\n\n".join(args_def)
+    return arg_string.rstrip("\n"), "\n\n".join(args_def)
+
+
+def poly_full_path(context, name) -> str:
+    """get the functions path as it will be exposed in the poly library"""
+    if context:
+        path = context + "." + name
+    else:
+        path = name
+    return f"poly.{path}"
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi/variables.py` & `polyapi_python-0.2.5.dev1/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/polyapi/webhook.py` & `polyapi_python-0.2.5.dev1/polyapi/webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,33 +2,42 @@
 import socketio  # type: ignore
 from socketio.exceptions import ConnectionError  # type: ignore
 import uuid
 from typing import Any, Dict, List, Tuple
 
 from polyapi.config import get_api_key_and_url
 from polyapi.typedefs import PropertySpecification
+from polyapi.utils import parse_arguments, poly_full_path
 
 # all active webhook handlers, used by unregister_all to cleanup
 active_handlers: List[Dict[str, Any]] = []
 
 # global client shared by all webhooks, will be initialized by webhook.start
 client = None
 
 
+WEBHOOK_DEFS_TEMPLATE = """
+from typing import List, Dict, Any, TypedDict, Callable
+{function_args_def}
+"""
+
+
 WEBHOOK_TEMPLATE = """
 
 
-async def {function_name}(callback, options=None):
+async def {function_name}(
+{function_args}
+):
     \"""{description}
 
     Function ID: {function_id}
     \"""
     from polyapi.webhook import client, active_handlers
 
-    print("Starting webhook for {function_name}...")
+    print("Starting webhook handler for {function_path}...")
 
     if not client:
         raise Exception("Client not initialized. Abort!")
 
     options = options or {{}}
     eventsClientId = "{client_id}"
     function_id = "{function_id}"
@@ -62,27 +71,27 @@
     data = {{
         "clientID": eventsClientId,
         "webhookHandleID": function_id,
         "apiKey": api_key,
         "waitForResponse": options.get("waitForResponse"),
     }}
     await client.emit('registerWebhookEventHandler', data, namespace="/events", callback=registerCallback)
-    active_handlers.append({{"clientID": eventsClientId, "webhookHandleID": function_id, "apiKey": api_key}})
+    active_handlers.append({{"clientID": eventsClientId, "webhookHandleID": function_id, "apiKey": api_key, "path": "{function_path}"}})
 """
 
 
 async def get_client_and_connect():
     _, base_url = get_api_key_and_url()
     global client
     client = socketio.AsyncClient()
     await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
 
 
 async def unregister(data: Dict[str, Any]):
-    print(f"stopping webhook handler for '{data['webhookHandleID']}'...")
+    print(f"Stopping webhook handler for {data['path']}...")
     assert client
     await client.emit(
         "unregisterWebhookEventHandler",
         {
             "clientID": data["clientID"],
             "webhookHandleID": data["webhookHandleID"],
             "apiKey": data["apiKey"],
@@ -100,28 +109,37 @@
     except ConnectionError:
         pass
     await asyncio.gather(*[unregister(handler) for handler in active_handlers])
 
 
 def render_webhook_handle(
     function_type: str,
+    function_context: str,
     function_name: str,
     function_id: str,
     function_description: str,
     arguments: List[PropertySpecification],
     return_type: Dict[str, Any],
 ) -> Tuple[str, str]:
+    function_args, function_args_def = parse_arguments(function_name, arguments)
+
+    if "WebhookEventType" in function_args:
+        # let's add the function name import!
+        function_args = function_args.replace("WebhookEventType", f"_{function_name}.WebhookEventType")
+
     func_str = WEBHOOK_TEMPLATE.format(
         description=function_description,
         client_id=uuid.uuid4().hex,
         function_id=function_id,
         function_name=function_name,
+        function_args=function_args,
+        function_path=poly_full_path(function_context, function_name),
     )
-
-    return func_str, ""
+    func_defs = WEBHOOK_DEFS_TEMPLATE.format(function_args_def=function_args_def)
+    return func_str, func_defs
 
 
 def start(*args):
     loop = asyncio.get_event_loop()
     loop.run_until_complete(get_client_and_connect())
     asyncio.gather(*args)
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.5.dev1/polyapi_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev9
+Version: 0.2.5.dev1
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev9/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.5.dev1/polyapi_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 polyapi/config.py
 polyapi/constants.py
 polyapi/error_handler.py
 polyapi/exceptions.py
 polyapi/execute.py
 polyapi/function_cli.py
 polyapi/generate.py
-polyapi/poly_custom.py
 polyapi/py.typed
 polyapi/schema.py
 polyapi/server.py
 polyapi/typedefs.py
 polyapi/utils.py
 polyapi/variables.py
 polyapi/webhook.py
```

### Comparing `polyapi_python-0.2.4.dev9/pyproject.toml` & `polyapi_python-0.2.5.dev1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.4.dev9"
+version = "0.2.5.dev1"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.4.dev9/tests/test_api.py` & `polyapi_python-0.2.5.dev1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/tests/test_auth.py` & `polyapi_python-0.2.5.dev1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/tests/test_function_cli.py` & `polyapi_python-0.2.5.dev1/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/tests/test_server.py` & `polyapi_python-0.2.5.dev1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev9/tests/test_variables.py` & `polyapi_python-0.2.5.dev1/tests/test_variables.py`

 * *Files identical despite different names*

