# Comparing `tmp/Slame-1.5.6.5.tar.gz` & `tmp/Slame-1.5.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.5.6.5.tar", last modified: Wed May  1 15:52:38 2024, max compression
+gzip compressed data, was "Slame-1.5.6.6.tar", last modified: Wed May  1 16:09:46 2024, max compression
```

## Comparing `Slame-1.5.6.5.tar` & `Slame-1.5.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:52:38.761919 Slame-1.5.6.5/
--rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:52:38.761919 Slame-1.5.6.5/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.5/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:52:38.761919 Slame-1.5.6.5/Slame/
--rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.5/Slame/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)    11605 2024-05-01 15:52:01.000000 Slame-1.5.6.5/Slame/slame.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 15:52:38.761919 Slame-1.5.6.5/Slame.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 15:52:38.000000 Slame-1.5.6.5/Slame.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 15:52:38.000000 Slame-1.5.6.5/Slame.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 15:52:38.000000 Slame-1.5.6.5/Slame.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 15:52:38.000000 Slame-1.5.6.5/Slame.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 15:52:38.000000 Slame-1.5.6.5/Slame.egg-info/top_level.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 15:52:38.761919 Slame-1.5.6.5/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 15:52:30.000000 Slame-1.5.6.5/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 16:09:46.072793 Slame-1.5.6.6/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-01 16:09:46.072793 Slame-1.5.6.6/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.6.6/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 16:09:46.072793 Slame-1.5.6.6/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.6.6/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    11573 2024-05-01 15:55:25.000000 Slame-1.5.6.6/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-01 16:09:46.072793 Slame-1.5.6.6/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-01 16:09:46.000000 Slame-1.5.6.6/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-01 16:09:46.000000 Slame-1.5.6.6/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-01 16:09:46.000000 Slame-1.5.6.6/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-01 16:09:46.000000 Slame-1.5.6.6/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-01 16:09:46.000000 Slame-1.5.6.6/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-01 16:09:46.072793 Slame-1.5.6.6/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-01 16:09:29.000000 Slame-1.5.6.6/setup.py
```

### Comparing `Slame-1.5.6.5/PKG-INFO` & `Slame-1.5.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.5
+Version: 1.5.6.6
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.5/README.md` & `Slame-1.5.6.6/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.5.6.5/Slame/slame.py` & `Slame-1.5.6.6/Slame/slame.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     content_length = self.get_content_length(request_data)
                     data = self.parse_post_data(request_data, content_length)
                     response = route['handler'](data)
                 else:
                     response = route['handler']()
 
                 response_headers = "HTTP/1.1 200 OK\n\n"
-                return response_headers.encode('utf-8') + response.encode('utf-8')
+                return response_headers + response
             else:
                 return "HTTP/1.1 405 Method Not Allowed\n\n405 Method Not Allowed".encode('utf-8')
         elif path.startswith('/static/'):
             return self.serve_static_file(path)
         else:
             return "HTTP/1.1 404 Not Found\n\n404 Not Found".encode('utf-8')
```

### Comparing `Slame-1.5.6.5/Slame.egg-info/PKG-INFO` & `Slame-1.5.6.6/Slame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.6.5
+Version: 1.5.6.6
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.6.5/setup.py` & `Slame-1.5.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.5.6.5'
+version = '1.5.6.6'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```
