# Comparing `tmp/decipher-sdk-0.0.13.tar.gz` & `tmp/decipher-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decipher-sdk-0.0.13.tar", last modified: Mon Mar  4 02:36:05 2024, max compression
+gzip compressed data, was "decipher-sdk-0.0.2.tar", last modified: Tue Apr 30 22:15:10 2024, max compression
```

## Comparing `decipher-sdk-0.0.13.tar` & `decipher-sdk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-03-04 02:36:05.359166 decipher-sdk-0.0.13/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      324 2024-03-04 02:36:05.359060 decipher-sdk-0.0.13/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      126 2024-03-04 00:15:41.000000 decipher-sdk-0.0.13/README.md
--rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-03-04 02:36:05.359209 decipher-sdk-0.0.13/setup.cfg
--rw-r--r--   0 mrosenfield   (501) staff       (20)      456 2024-03-04 02:36:02.000000 decipher-sdk-0.0.13/setup.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-03-04 02:36:05.357668 decipher-sdk-0.0.13/src/
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-03-04 02:36:05.358192 decipher-sdk-0.0.13/src/decipher_sdk/
--rw-r--r--   0 mrosenfield   (501) staff       (20)       30 2024-03-04 02:34:29.000000 decipher-sdk-0.0.13/src/decipher_sdk/__init__.py
--rw-r--r--   0 mrosenfield   (501) staff       (20)     8124 2024-03-04 00:26:29.000000 decipher-sdk-0.0.13/src/decipher_sdk/decipher_sdk.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-03-04 02:36:05.358904 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      324 2024-03-04 02:36:05.000000 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      279 2024-03-04 02:36:05.000000 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-03-04 02:36:05.000000 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       15 2024-03-04 02:36:05.000000 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/requires.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-03-04 02:36:05.000000 decipher-sdk-0.0.13/src/decipher_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.675422 decipher-sdk-0.0.2/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      322 2024-04-30 22:15:10.675294 decipher-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      126 2024-04-12 14:51:10.000000 decipher-sdk-0.0.2/README.md
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-04-30 22:15:10.675508 decipher-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      454 2024-04-30 22:15:06.000000 decipher-sdk-0.0.2/setup.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.672561 decipher-sdk-0.0.2/src/
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.673637 decipher-sdk-0.0.2/src/decipher_sdk/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       55 2024-04-30 21:56:25.000000 decipher-sdk-0.0.2/src/decipher_sdk/__init__.py
+-rw-r--r--   0 mrosenfield   (501) staff       (20)     9020 2024-04-30 22:13:01.000000 decipher-sdk-0.0.2/src/decipher_sdk/decipher_sdk.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-30 22:15:10.675046 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      322 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      279 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       15 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/requires.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-04-30 22:15:10.000000 decipher-sdk-0.0.2/src/decipher_sdk.egg-info/top_level.txt
```

### Comparing `decipher-sdk-0.0.13/src/decipher_sdk/decipher_sdk.py` & `decipher-sdk-0.0.2/src/decipher_sdk/decipher_sdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 class DecipherMonitor:
     @safe_method
     def __init__(self, codebase_id, customer_id):
         self.codebase_id = codebase_id
         self.customer_id = customer_id
         self.endpoint = "https://prod.getdecipher.com/api/exception_upload"
-        #self.endpoint = "http://localhost:3005/api/exception_upload"
+        #self.endpoint = "http://localhost:3000/api/exception_upload"
         self.messages = []  # Initialize the messages list
+        self.user = None
         self.exception_occurred = False  # Flag to indicate an exception has occurred
         self.connect_to_signals()
 
     @safe_method
     def connect_to_signals(self):
         # Connect to Flask signals
         request_started.connect(self.before_request_handler)
@@ -44,14 +45,15 @@
 
     @safe_method
     def teardown_request_handler(self, sender, response, **extra):
         if has_request_context():
             self.restore_print()
             if not self.exception_occurred and response.status_code != 200:
                 self.capture_error_with_response(response)
+            self.user = None
             self.clear_messages()
 
     @safe_method
     def capture_error_with_response(self, response):
         data = self.prepare_data(response)
         self.send_to_decipher(data)
 
@@ -188,15 +190,16 @@
             "request_url": request.url,
             "request_endpoint": request.endpoint,
             "request_headers": self.get_headers(request.headers),
             "request_body": request_body,
             "response_body": response_body,
             "status_code": status_code,
             "is_uncaught_exception": exception is not None,
-            'messages': self.messages
+            'messages': self.messages,
+            'affected_user': self.user
         }
         return data
 
     @safe_method
     def get_timestamp(self):
         # To Do confirm this is right time format
         return datetime.utcnow().isoformat() + 'Z'
@@ -213,18 +216,44 @@
     def send_to_decipher(self, data):
         try:
             requests.post(self.endpoint, json=data)
         except requests.RequestException as e:
             pass
 
     @safe_method
+    def capture_error(self, error):
+        if has_request_context():
+            self.capture_error_with_exception(request._get_current_object(), error)
+        else:
+            # Handle cases where there is no Flask request context
+            pass
+
+    @safe_method
     def safe_stringify(self, obj, indent=2):
         try:
             return json.dumps(obj, indent=indent, default=str)
         except TypeError:
             return str(obj)
+
+    def set_user(self, user):
+        if all(key in ['id', 'username', 'email'] for key in user):
+            self.user = user
         
 _decipher_monitor_instance = None
 
 def init(codebase_id, customer_id):
     global _decipher_monitor_instance
-    _decipher_monitor_instance = DecipherMonitor(codebase_id, customer_id)
+    _decipher_monitor_instance = DecipherMonitor(codebase_id, customer_id)
+
+def capture_error(error):
+    if _decipher_monitor_instance:
+        _decipher_monitor_instance.capture_error(error)
+    else:
+        # Handle the case where DecipherMonitor is not initialized
+        pass
+
+def set_user(user):
+    if _decipher_monitor_instance:
+        _decipher_monitor_instance.set_user(user)
+    else:
+        # Handle the case where DecipherMonitor is not initialized
+        pass
```

