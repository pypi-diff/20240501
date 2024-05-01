# Comparing `tmp/supabase-2.4.3.tar.gz` & `tmp/supabase-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-2.4.3.tar", max compression
+gzip compressed data, was "supabase-2.4.4.tar", max compression
```

## Comparing `supabase-2.4.3.tar` & `supabase-2.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-04-17 14:07:12.395553 supabase-2.4.3/LICENSE
--rw-r--r--   0        0        0     8244 2024-04-17 14:07:12.395553 supabase-2.4.3/README.md
--rw-r--r--   0        0        0     1892 2024-04-17 14:07:18.427550 supabase-2.4.3/pyproject.toml
--rw-r--r--   0        0        0      751 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/__init__.py
--rw-r--r--   0        0        0       22 2024-04-17 14:07:18.427550 supabase-2.4.3/supabase/__version__.py
--rw-r--r--   0        0        0       35 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/__init__.py
--rw-r--r--   0        0        0     1130 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/auth_client.py
--rw-r--r--   0        0        0    10127 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/client.py
--rw-r--r--   0        0        0       35 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/auth_client.py
--rw-r--r--   0        0        0    10088 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/client.py
--rw-r--r--   0        0        0      772 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/client.py
--rw-r--r--   0        0        0      127 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0        0 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/py.typed
--rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-01 18:20:12.455018 supabase-2.4.4/LICENSE
+-rw-r--r--   0        0        0     8244 2024-05-01 18:20:12.455018 supabase-2.4.4/README.md
+-rw-r--r--   0        0        0     1892 2024-05-01 18:20:18.731041 supabase-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1224 2024-05-01 18:20:12.455018 supabase-2.4.4/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-01 18:20:18.731041 supabase-2.4.4/supabase/__version__.py
+-rw-r--r--   0        0        0       35 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_async/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_async/auth_client.py
+-rw-r--r--   0        0        0    10127 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_async/client.py
+-rw-r--r--   0        0        0       35 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_sync/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_sync/auth_client.py
+-rw-r--r--   0        0        0    10088 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/_sync/client.py
+-rw-r--r--   0        0        0     1172 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/client.py
+-rw-r--r--   0        0        0      127 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:20:12.459018 supabase-2.4.4/supabase/py.typed
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.4/PKG-INFO
```

### Comparing `supabase-2.4.3/LICENSE` & `supabase-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/README.md` & `supabase-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/pyproject.toml` & `supabase-2.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "2.4.3"
+version = "2.4.4"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
@@ -22,20 +22,20 @@
 httpx = ">=0.24,<0.28"
 storage3 = ">=0.5.3,<0.8.0"
 supafunc = ">=0.3.1,<0.5.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.5.0"
 black = "^24.4"
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 pytest-cov = "^5.0.0"
-commitizen = "^3.22.0"
-python-semantic-release = "^9.4.1"
+commitizen = "^3.24.0"
+python-semantic-release = "^9.6.0"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.scripts]
 tests = 'poetry_scripts:run_tests'
 
 [tool.poetry.group.dev.dependencies]
 unasync-cli = "^0.0.9"
```

### Comparing `supabase-2.4.3/supabase/_async/auth_client.py` & `supabase-2.4.4/supabase/_async/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/supabase/_async/client.py` & `supabase-2.4.4/supabase/_async/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/supabase/_sync/auth_client.py` & `supabase-2.4.4/supabase/_sync/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/supabase/_sync/client.py` & `supabase-2.4.4/supabase/_sync/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/supabase/client.py` & `supabase-2.4.4/supabase/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 from postgrest import APIError as PostgrestAPIError
 from postgrest import APIResponse as PostgrestAPIResponse
 from storage3.utils import StorageException
 
+# Version
 from .__version__ import __version__
+
+# Async Client
+from ._async.auth_client import AsyncSupabaseAuthClient
+from ._async.client import AsyncClient
+from ._async.client import AsyncStorageClient as AsyncSupabaseStorageClient
+from ._async.client import create_client as create_async_client
+
+# Sync Client
 from ._sync.auth_client import SyncSupabaseAuthClient as SupabaseAuthClient
-from ._sync.client import ClientOptions
 from ._sync.client import SyncClient as Client
 from ._sync.client import SyncStorageClient as SupabaseStorageClient
 from ._sync.client import create_client
+
+# Lib
+from .lib.client_options import ClientOptions
 from .lib.realtime_client import SupabaseRealtimeClient
 
 __all__ = [
-    "PostgrestAPIError",
-    "PostgrestAPIResponse",
-    "StorageException",
+    "AsyncSupabaseAuthClient",
+    "create_async_client",
+    "AsyncClient",
+    "AsyncSupabaseStorageClient",
     "SupabaseAuthClient",
-    "__version__",
     "create_client",
     "Client",
     "ClientOptions",
     "SupabaseStorageClient",
     "SupabaseRealtimeClient",
+    "PostgrestAPIError",
+    "PostgrestAPIResponse",
+    "StorageException",
+    "__version__",
 ]
```

### Comparing `supabase-2.4.3/supabase/lib/client_options.py` & `supabase-2.4.4/supabase/lib/client_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     storage: SyncSupportedStorage = field(default_factory=SyncMemoryStorage)
     """A storage provider. Used to store the logged in session."""
 
     realtime: Optional[Dict[str, Any]] = None
     """Options passed to the realtime-py instance"""
 
-    postgrest_client_timeout: Union[
-        int, float, Timeout
-    ] = DEFAULT_POSTGREST_CLIENT_TIMEOUT
+    postgrest_client_timeout: Union[int, float, Timeout] = (
+        DEFAULT_POSTGREST_CLIENT_TIMEOUT
+    )
     """Timeout passed to the SyncPostgrestClient instance."""
 
     storage_client_timeout: Union[int, float, Timeout] = DEFAULT_STORAGE_CLIENT_TIMEOUT
     """Timeout passed to the SyncStorageClient instance"""
 
     flow_type: AuthFlowType = "implicit"
     """flow type to use for authentication"""
```

### Comparing `supabase-2.4.3/supabase/lib/realtime_client.py` & `supabase-2.4.4/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.3/PKG-INFO` & `supabase-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supabase
-Version: 2.4.3
+Version: 2.4.4
 Summary: Supabase client for Python.
 Home-page: https://github.com/supabase-community/supabase-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

