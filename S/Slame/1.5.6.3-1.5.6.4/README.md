# Comparing `tmp/Slame-1.5.6.3.tar.gz` & `tmp/Slame-1.5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.5.6.3.tar", last modified: Wed May  1 15:41:05 2024, max compression
+gzip compressed data, was "Slame-1.5.6.4.tar", last modified: Wed May  1 15:47:42 2024, max compression
```

## Comparing `Slame-1.5.6.3.tar` & `Slame-1.5.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/
--rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:41:05.922961 Slame-1.5.6.3/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.3/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/Slame/
--rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.3/Slame/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)    12645 2024-05-01 15:39:32.000000 Slame-1.5.6.3/Slame/slame.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/Slame.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/top_level.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 15:41:05.922961 Slame-1.5.6.3/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 15:40:41.000000 Slame-1.5.6.3/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:47:42.941052 Slame-1.5.6.4/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:47:42.941052 Slame-1.5.6.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.4/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:47:42.941052 Slame-1.5.6.4/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.4/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    11621 2024-05-01 15:46:57.000000 Slame-1.5.6.4/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:47:42.941052 Slame-1.5.6.4/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:47:42.000000 Slame-1.5.6.4/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 15:47:42.000000 Slame-1.5.6.4/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 15:47:42.000000 Slame-1.5.6.4/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 15:47:42.000000 Slame-1.5.6.4/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 15:47:42.000000 Slame-1.5.6.4/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 15:47:42.941052 Slame-1.5.6.4/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 15:47:36.000000 Slame-1.5.6.4/setup.py
```

### Comparing `Slame-1.5.6.3/PKG-INFO` & `Slame-1.5.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.3
+Version: 1.5.6.4
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.3/README.md` & `Slame-1.5.6.4/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.5.6.3/Slame/slame.py` & `Slame-1.5.6.4/Slame/slame.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,110 +19,95 @@
 """
 class ZHRXX:
     def __init__(self, host, port):
         self.host = host
         self.port = port
         self.routes = {}
         self.middlewares = []
+        self.server_socket = None
 
     def route(self, path, methods=['GET']):
         def decorator(func):
             self.routes[path] = {
                 'methods': methods,
                 'handler': func
             }
             return func
         return decorator
 
+
     def use(self, middleware):
         self.middlewares.append(middleware)
 
     def start(self):
-        server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        server_socket.bind((self.host, self.port))
-        server_socket.listen(5)
+        self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
+        self.server_socket.bind((self.host, self.port))
+        self.server_socket.listen(5)
         print(f"Server is listening on {self.host}:{self.port}")
 
         while True:
-            client_socket, client_address = server_socket.accept()
+            client_socket, client_address = self.server_socket.accept()
             request_data = client_socket.recv(1024).decode('utf-8')
 
             if request_data:
                 request_lines = request_data.split('\n')
                 request_line = request_lines[0]
                 method, path, _ = request_line.split()
                 response = self.handle_request(method, path, request_data)
                 client_socket.send(response.encode('utf-8'))
                 client_socket.close()
 
     def handle_request(self, method, path, request_data):
-        # Execute middleware functions
         for middleware in self.middlewares:
             middleware()
 
-        # Check if the requested path matches any defined route
         if path in self.routes:
             route = self.routes[path]
-            # Check if the requested HTTP method is allowed for the route
             if method in route['methods']:
                 if method == 'POST':
-                    # Parse request data for POST requests
                     content_length = self.get_content_length(request_data)
                     data = self.parse_post_data(request_data, content_length)
-                    # Execute the handler function for the matched route with provided data
                     response = route['handler'](data)
                 else:
-                    # Execute the handler function for the matched route
                     response = route['handler']()
-                # Return a successful HTTP response with the response content
-                return f"HTTP/1.1 200 OK\n\n{response}"
+
+                response_headers = "HTTP/1.1 200 OK\n\n"
+                return response_headers.encode('utf-8') + response.encode('utf-8')
             else:
-                # Return a "Method Not Allowed" response if the method is not allowed for the route
-                return "HTTP/1.1 405 Method Not Allowed\n\n405 Method Not Allowed"
-        # Check if the requested path starts with '/static/', indicating a static file request
+                return "HTTP/1.1 405 Method Not Allowed\n\n405 Method Not Allowed".encode('utf-8')
         elif path.startswith('/static/'):
-            # Serve the requested static file
             return self.serve_static_file(path)
         else:
-            # Return a "Not Found" response for paths that don't match any route or static file
-            return "HTTP/1.1 404 Not Found\n\n404 Not Found"
-
-
+            return "HTTP/1.1 404 Not Found\n\n404 Not Found".encode('utf-8')
 
     def serve_static_file(self, path):
-        # Get the absolute path to the file based on the script's directory
         script_dir = os.path.dirname(os.path.abspath(__file__))
         abs_file_path = os.path.join(script_dir, "static", path[1:])
-        
-        print("Absolute file path:", abs_file_path)  # Debugging statement
-        
+
         try:
             with open(abs_file_path, 'rb') as file:
                 content = file.read()
-            response_header = "HTTP/1.1 200 OK\n\n"
-            return response_header.encode('utf-8') + content
+            response_headers = "HTTP/1.1 200 OK\n\n"
+            return response_headers.encode('utf-8') + content
         except FileNotFoundError:
-            print("File not found:", abs_file_path)  # Debugging statement
-            return b"HTTP/1.1 404 Not Found\n\n404 Not Found"
+            return "HTTP/1.1 404 Not Found\n\n404 Not Found".encode('utf-8')
 
     def get_content_length(self, request_data):
-        # Parse Content-Length header to determine data size
         for line in request_data.split('\n'):
             if line.startswith('Content-Length:'):
                 return int(line.split(':')[1])
         return 0
 
     def parse_post_data(self, request_data, content_length):
-        # Parse POST data from request body
         body = request_data.split('\n\n')[-1]
         post_data = parse_qs(body)
         return post_data
-
-    def close(self):  # Added close method to properly close the server socket
-        server_socket.close()
+    
+    def close(self):
+        self.server_socket.close() 
 
 """
 (c) ZHRXXgroup
 https://zhrxxgroup.com/+
 
 Version: 1.0.5
 """
```

### Comparing `Slame-1.5.6.3/Slame.egg-info/PKG-INFO` & `Slame-1.5.6.4/Slame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.3
+Version: 1.5.6.4
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.3/setup.py` & `Slame-1.5.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.5.6.3'
+version = '1.5.6.4'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```

