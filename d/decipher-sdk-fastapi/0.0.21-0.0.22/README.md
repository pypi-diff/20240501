# Comparing `tmp/decipher_sdk_fastapi-0.0.21.tar.gz` & `tmp/decipher_sdk_fastapi-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decipher_sdk_fastapi-0.0.21.tar", last modified: Thu Apr 25 19:55:07 2024, max compression
+gzip compressed data, was "decipher_sdk_fastapi-0.0.22.tar", last modified: Wed May  1 00:16:13 2024, max compression
```

## Comparing `decipher_sdk_fastapi-0.0.21.tar` & `decipher_sdk_fastapi-0.0.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:55:06.999017 decipher_sdk_fastapi-0.0.21/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      313 2024-04-25 19:55:06.998901 decipher_sdk_fastapi-0.0.21/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)       71 2024-04-25 19:54:53.000000 decipher_sdk_fastapi-0.0.21/README.md
--rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-04-25 19:55:06.999063 decipher_sdk_fastapi-0.0.21/setup.cfg
--rw-r--r--   0 mrosenfield   (501) staff       (20)      510 2024-04-25 19:55:03.000000 decipher_sdk_fastapi-0.0.21/setup.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:55:06.997100 decipher_sdk_fastapi-0.0.21/src/
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:55:06.997762 decipher_sdk_fastapi-0.0.21/src/decipher_sdk/
--rw-r--r--   0 mrosenfield   (501) staff       (20)       45 2024-04-14 18:23:34.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk/__init__.py
--rw-r--r--   0 mrosenfield   (501) staff       (20)     8205 2024-04-25 00:42:11.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk/decipher_sdk.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:55:06.998737 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      313 2024-04-25 19:55:06.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      319 2024-04-25 19:55:06.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-04-25 19:55:06.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       17 2024-04-25 19:55:06.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/requires.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-04-25 19:55:06.000000 decipher_sdk_fastapi-0.0.21/src/decipher_sdk_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-01 00:16:13.617539 decipher_sdk_fastapi-0.0.22/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      370 2024-05-01 00:16:13.617417 decipher_sdk_fastapi-0.0.22/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      128 2024-04-30 20:27:42.000000 decipher_sdk_fastapi-0.0.22/README.md
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-05-01 00:16:13.617590 decipher_sdk_fastapi-0.0.22/setup.cfg
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      510 2024-05-01 00:15:52.000000 decipher_sdk_fastapi-0.0.22/setup.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-01 00:16:13.615789 decipher_sdk_fastapi-0.0.22/src/
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-01 00:16:13.616493 decipher_sdk_fastapi-0.0.22/src/decipher_sdk/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       55 2024-04-30 23:04:45.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk/__init__.py
+-rw-r--r--   0 mrosenfield   (501) staff       (20)     8575 2024-05-01 00:16:00.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk/decipher_sdk.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-05-01 00:16:13.617220 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      370 2024-05-01 00:16:13.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      319 2024-05-01 00:16:13.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-05-01 00:16:13.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       17 2024-05-01 00:16:13.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/requires.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-05-01 00:16:13.000000 decipher_sdk_fastapi-0.0.22/src/decipher_sdk_fastapi.egg-info/top_level.txt
```

### Comparing `decipher_sdk_fastapi-0.0.21/src/decipher_sdk/decipher_sdk.py` & `decipher_sdk_fastapi-0.0.22/src/decipher_sdk/decipher_sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import asyncio
 import linecache
 from contextvars import ContextVar
 from fastapi import Request
 
 current_request = ContextVar("decipher_current_request")
 current_messages = ContextVar("current_messages", default=[])
+current_user = ContextVar("current_user", default=None)
 
 def safe_method(func):
     @functools.wraps(func)
     async def wrapper(*args, **kwargs):
         try:
             if asyncio.iscoroutinefunction(func):
                 return await func(*args, **kwargs)
@@ -39,26 +40,32 @@
         builtins.print = self.custom_print
 
     async def __call__(self, scope, receive, send):
         # Setup or any preparation before handling the request
         request = Request(scope, receive=receive)
         request_token = current_request.set(request)
         messages_token = current_messages.set([])
+        user_token = current_user.set(None)
+        
         try:
             # Pass control to the next application in the stack
             await self.app(scope, receive, send)
         except Exception as exc:
             # Handle the exception (e.g., logging, modifying response to client)
             await self.capture_error_with_exception(request, exc, isManual = False)
             raise exc from None
         finally:
             current_request.reset(request_token)
             current_messages.reset(messages_token)
+            current_user.reset(user_token)
             builtins.print = self.original_print
 
+    def set_user(self, user):
+        if all(key in ['id', 'username', 'email'] for key in user):
+            current_user.set(user)
 
     async def capture_error_with_response(self, request: Request, response: Response):
         try:
             data = await self.prepare_data(request, response=response)
             await self.send_to_decipher(data)
         except Exception as e:
             pass
@@ -67,21 +74,21 @@
         try:
             data = await self.prepare_data(request, exception=exception, isManual = isManual)
             await self.send_to_decipher(data)
         except Exception as e:
             pass
 
     async def prepare_data(self, request: Request, response=None, exception=None, isManual = False):
-        request_body = await request.body()
-        try:
-            request_body = json.loads(request_body.decode())
-        except json.JSONDecodeError:
-            request_body = request_body.decode()  # Use raw body if JSON parsing fails
+        # request_body = await request.body()
+        # try:
+        #     request_body = json.loads(request_body.decode())
+        # except json.JSONDecodeError:
+        #     request_body = request_body.decode()  # Use raw body if JSON parsing fails
 
-        # Initialize response data
+        # # Initialize response data
         response_body = {}
 
         if (isManual):
             status_code = 0
         else:
             status_code = 500  # Default to 500 unless a response object is provided
 
@@ -102,19 +109,20 @@
             "codebase_id": self.codebase_id,
             "customer_id": self.customer_id,
             "timestamp": self.get_timestamp(),
             "error_stack": stack_trace,
             "request_url": str(request.url),
             "request_endpoint": str(request.url.path),
             "request_headers": dict(request.headers),
-            "request_body": request_body,
+            "request_body": None,
             "response_body": response_body,
             "status_code": status_code,
             "is_uncaught_exception": exception is not None,
-            'messages': current_messages.get()
+            'messages': current_messages.get(),
+            'affected_user': current_user.get()
         }
 
         return data
     
     def get_timestamp(self):
         return datetime.utcnow().isoformat() + 'Z'
     
@@ -174,30 +182,27 @@
     def get_local_variables(self, frame):
         return {var: repr(value) for var, value in frame.f_locals.items()}
 
     async def send_to_decipher(self, data):
         try:
             await asyncio.to_thread(requests.post, self.endpoint, json=data)
         except requests.RequestException as e:
-            print(f"Failed to send error data: {str(e)}")
+            pass
 
 
     def custom_print(self, *args, **kwargs):
         messages = current_messages.get()
         message = ' '.join(str(arg) for arg in args)
         messages.append({
             "message": message,
             "level": "log",
             "timestamp": self.get_timestamp()
         })
         self.original_print(*args, **kwargs)
 
-    def get_timestamp(self):
-        return datetime.utcnow().isoformat() + 'Z'
-
     def clear_messages(self):
         self.messages = []
 
 _decipher_monitor_instance = None
 
 def init(app, codebase_id, customer_id):
     global _decipher_monitor_instance
@@ -208,8 +213,13 @@
     request = current_request.get()
     if request and _decipher_monitor_instance:
         try:
             if asyncio.get_event_loop().is_running():
                 # Asynchronous context: Use asyncio to handle it
                 asyncio.create_task(_decipher_monitor_instance.capture_error_with_exception(request, error, isManual = True))
         except Exception as e:
-            asyncio.run(_decipher_monitor_instance.capture_error_with_exception(request, error, isManual = True))
+            asyncio.run(_decipher_monitor_instance.capture_error_with_exception(request, error, isManual = True))
+
+def set_user(user):
+    request = current_request.get()
+    if request and _decipher_monitor_instance:
+        _decipher_monitor_instance.set_user(user)
```

