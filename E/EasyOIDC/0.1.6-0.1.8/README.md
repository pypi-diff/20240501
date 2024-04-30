# Comparing `tmp/EasyOIDC-0.1.6.tar.gz` & `tmp/easyoidc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyOIDC-0.1.6.tar", last modified: Fri Feb  2 21:49:36 2024, max compression
+gzip compressed data, was "easyoidc-0.1.8.tar", last modified: Tue Apr 30 23:29:11 2024, max compression
```

## Comparing `EasyOIDC-0.1.6.tar` & `easyoidc-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:49:36.899678 EasyOIDC-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:49:36.895678 EasyOIDC-0.1.6/EasyOIDC/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:49:36.895678 EasyOIDC-0.1.6/EasyOIDC/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/frameworks/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/frameworks/nicegui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/frameworks/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/frameworks/taipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/EasyOIDC/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:49:36.895678 EasyOIDC-0.1.6/EasyOIDC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-02-02 21:49:36.000000 EasyOIDC-0.1.6/EasyOIDC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-02 21:49:36.000000 EasyOIDC-0.1.6/EasyOIDC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 21:49:36.000000 EasyOIDC-0.1.6/EasyOIDC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-02 21:49:36.000000 EasyOIDC-0.1.6/EasyOIDC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-02 21:49:36.000000 EasyOIDC-0.1.6/EasyOIDC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-02-02 21:49:36.899678 EasyOIDC-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 21:49:36.899678 EasyOIDC-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-02 21:49:26.000000 EasyOIDC-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/nicegui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/taipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 23:29:07.000000 easyoidc-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-30 23:29:11.141757 easyoidc-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-30 23:29:07.000000 easyoidc-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:29:11.141757 easyoidc-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-30 23:29:07.000000 easyoidc-0.1.8/setup.py
```

### Comparing `EasyOIDC-0.1.6/EasyOIDC/auth.py` & `easyoidc-0.1.8/EasyOIDC/auth.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/config.py` & `easyoidc-0.1.8/EasyOIDC/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,22 @@
         response = requests.get(url)
         if response.status_code == 200:
             data = json.loads(response.text)
             self.authorization_endpoint = data['authorization_endpoint']
             self.token_endpoint = data['token_endpoint']
             self.userinfo_endpoint = data['userinfo_endpoint']
             self.token_revoke_endpoint = data['revocation_endpoint']
-            self.scope = data['scopes_supported']
+            if not self.scope:
+                # If not defined, copy the scopes_supported from the server.
+                self.scope = data['scopes_supported']
+            else:
+                # Validate self.scope with the scopes_supported by the server.
+                for scope in self.scope:
+                    if scope not in data['scopes_supported']:
+                        raise Exception(f"Scope '{scope}' not supported by the server.")
         else:
             raise Exception(f'Error loading wellknown url: {wellknown_url}')
 
     def __str__(self):
         return self.dump_configuration()
 
     def __repr__(self):
```

### Comparing `EasyOIDC-0.1.6/EasyOIDC/frameworks/flask.py` & `easyoidc-0.1.8/EasyOIDC/frameworks/flask.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/frameworks/nicegui.py` & `easyoidc-0.1.8/EasyOIDC/frameworks/nicegui.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/frameworks/streamlit.py` & `easyoidc-0.1.8/EasyOIDC/frameworks/streamlit.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/frameworks/taipy.py` & `easyoidc-0.1.8/EasyOIDC/frameworks/taipy.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/session.py` & `easyoidc-0.1.8/EasyOIDC/session.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC/utils.py` & `easyoidc-0.1.8/EasyOIDC/utils.py`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/EasyOIDC.egg-info/PKG-INFO` & `easyoidc-0.1.8/EasyOIDC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyOIDC
-Version: 0.1.6
+Version: 0.1.8
 Summary: Easy integration with OIDC authentication servers
 Home-page: https://github.com/jpmanson/EasyOIDC
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EasyOIDC-0.1.6/LICENSE` & `easyoidc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/PKG-INFO` & `easyoidc-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyOIDC
-Version: 0.1.6
+Version: 0.1.8
 Summary: Easy integration with OIDC authentication servers
 Home-page: https://github.com/jpmanson/EasyOIDC
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EasyOIDC-0.1.6/README.md` & `easyoidc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `EasyOIDC-0.1.6/setup.py` & `easyoidc-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 
 README = (Path(__file__).parent/"README.md").read_text()
 
 setuptools.setup(
     name="EasyOIDC",
-    version="0.1.6",
+    version="0.1.8",
     author="Juan Pablo Manson",
     author_email="jpmanson@gmail.com",
     description="Easy integration with OIDC authentication servers",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jpmanson/EasyOIDC",
     packages=setuptools.find_packages(),
```

