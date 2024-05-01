# Comparing `tmp/Slame-1.5.6.2.tar.gz` & `tmp/Slame-1.5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.5.6.2.tar", last modified: Wed May  1 15:36:13 2024, max compression
+gzip compressed data, was "Slame-1.5.6.3.tar", last modified: Wed May  1 15:41:05 2024, max compression
```

## Comparing `Slame-1.5.6.2.tar` & `Slame-1.5.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:36:13.817652 Slame-1.5.6.2/
--rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:36:13.817652 Slame-1.5.6.2/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.2/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:36:13.817652 Slame-1.5.6.2/Slame/
--rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.2/Slame/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)    12669 2024-05-01 15:35:11.000000 Slame-1.5.6.2/Slame/slame.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:36:13.817652 Slame-1.5.6.2/Slame.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:36:13.000000 Slame-1.5.6.2/Slame.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 15:36:13.000000 Slame-1.5.6.2/Slame.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 15:36:13.000000 Slame-1.5.6.2/Slame.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 15:36:13.000000 Slame-1.5.6.2/Slame.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 15:36:13.000000 Slame-1.5.6.2/Slame.egg-info/top_level.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 15:36:13.817652 Slame-1.5.6.2/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 15:36:01.000000 Slame-1.5.6.2/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:41:05.922961 Slame-1.5.6.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.3/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.3/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    12645 2024-05-01 15:39:32.000000 Slame-1.5.6.3/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:41:05.922961 Slame-1.5.6.3/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 15:41:05.000000 Slame-1.5.6.3/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 15:41:05.922961 Slame-1.5.6.3/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 15:40:41.000000 Slame-1.5.6.3/setup.py
```

### Comparing `Slame-1.5.6.2/PKG-INFO` & `Slame-1.5.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.2
+Version: 1.5.6.3
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.2/README.md` & `Slame-1.5.6.3/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.5.6.2/Slame/slame.py` & `Slame-1.5.6.3/Slame/slame.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,20 +77,21 @@
                 return f"HTTP/1.1 200 OK\n\n{response}"
             else:
                 # Return a "Method Not Allowed" response if the method is not allowed for the route
                 return "HTTP/1.1 405 Method Not Allowed\n\n405 Method Not Allowed"
         # Check if the requested path starts with '/static/', indicating a static file request
         elif path.startswith('/static/'):
             # Serve the requested static file
-            return self.serve_static_file(path)  # Ensure self is passed
+            return self.serve_static_file(path)
         else:
             # Return a "Not Found" response for paths that don't match any route or static file
             return "HTTP/1.1 404 Not Found\n\n404 Not Found"
 
 
+
     def serve_static_file(self, path):
         # Get the absolute path to the file based on the script's directory
         script_dir = os.path.dirname(os.path.abspath(__file__))
         abs_file_path = os.path.join(script_dir, "static", path[1:])
         
         print("Absolute file path:", abs_file_path)  # Debugging statement
```

### Comparing `Slame-1.5.6.2/Slame.egg-info/PKG-INFO` & `Slame-1.5.6.3/Slame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.2
+Version: 1.5.6.3
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.2/setup.py` & `Slame-1.5.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.5.6.2'
+version = '1.5.6.3'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```

