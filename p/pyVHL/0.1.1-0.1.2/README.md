# Comparing `tmp/pyvhl-0.1.1.tar.gz` & `tmp/pyvhl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvhl-0.1.1.tar", max compression
+gzip compressed data, was "pyvhl-0.1.2.tar", max compression
```

## Comparing `pyvhl-0.1.1.tar` & `pyvhl-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       78 2024-04-30 20:11:14.442569 pyvhl-0.1.1/README.md
--rw-r--r--   0        0        0      465 2024-04-30 20:11:14.442569 pyvhl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    15513 2024-04-30 20:11:14.442569 pyvhl-0.1.1/pyvhl/mirror_clients.py
--rw-r--r--   0        0        0        0 2024-04-30 20:11:14.442569 pyvhl-0.1.1/pyvhl/model/__init__.py
--rw-r--r--   0        0        0      523 2024-04-30 20:11:14.442569 pyvhl-0.1.1/pyvhl/model/_model.py
--rw-r--r--   0        0        0     5681 2024-04-30 20:11:14.442569 pyvhl-0.1.1/pyvhl/pyvhl.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 pyvhl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-05-01 05:33:54.771494 pyvhl-0.1.2/README.md
+-rw-r--r--   0        0        0      465 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15513 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/mirror_clients.py
+-rw-r--r--   0        0        0        0 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/model/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/model/_model.py
+-rw-r--r--   0        0        0     5672 2024-05-01 05:33:54.771494 pyvhl-0.1.2/pyvhl/pyvhl.py
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 pyvhl-0.1.2/PKG-INFO
```

### Comparing `pyvhl-0.1.1/pyvhl/mirror_clients.py` & `pyvhl-0.1.2/pyvhl/mirror_clients.py`

 * *Files identical despite different names*

### Comparing `pyvhl-0.1.1/pyvhl/model/_model.py` & `pyvhl-0.1.2/pyvhl/model/_model.py`

 * *Files identical despite different names*

### Comparing `pyvhl-0.1.1/pyvhl/pyvhl.py` & `pyvhl-0.1.2/pyvhl/pyvhl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 
 class pyvhl:
     """
     Handles proccessing of mirroring videos from Reddit and Twitter.
     """
 
-    def __init__(self, catbox_) -> None:
+    def __init__(self) -> None:
         session = Session()
-        session.headers["User-Agent"] = "pyVHL/1.0.0"
+        session.headers["User-Agent"] = "pyVHL/0.1.2"
         self.client = Client(session=session)
         self.clients = {
             "streamable": self.client.streamable,
             "catbox": self.client.catbox,
         }
 
     @retry(delay=5, tries=5)
```

### Comparing `pyvhl-0.1.1/PKG-INFO` & `pyvhl-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVHL
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: problemxl
 Author-email: email@github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

