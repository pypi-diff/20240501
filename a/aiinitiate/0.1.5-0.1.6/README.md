# Comparing `tmp/aiinitiate-0.1.5.tar.gz` & `tmp/aiinitiate-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiinitiate-0.1.5.tar", max compression
+gzip compressed data, was "aiinitiate-0.1.6.tar", max compression
```

## Comparing `aiinitiate-0.1.5.tar` & `aiinitiate-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.5/README.md
--rw-r--r--   0        0        0       22 2024-05-01 10:47:17.166244 aiinitiate-0.1.5/aiinitiate/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 10:01:03.874802 aiinitiate-0.1.5/aiinitiate/basic/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-01 10:02:48.805624 aiinitiate-0.1.5/aiinitiate/basic/common_utils.py
--rw-r--r--   0        0        0     3744 2024-05-01 10:44:23.735560 aiinitiate-0.1.5/aiinitiate/cli.py
--rw-r--r--   0        0        0      706 2024-05-01 09:36:43.043223 aiinitiate-0.1.5/aiinitiate/config.py
--rw-r--r--   0        0        0     3349 2024-05-01 10:41:01.194134 aiinitiate-0.1.5/aiinitiate/g.py
--rw-r--r--   0        0        0     2961 2024-05-01 10:47:08.142515 aiinitiate-0.1.5/aiinitiate/sysinfo.py
--rw-r--r--   0        0        0        0 2024-05-01 09:39:39.205235 aiinitiate-0.1.5/aiinitiate/tools/__init__.py
--rw-r--r--   0        0        0     2918 2024-05-01 09:54:24.055293 aiinitiate-0.1.5/aiinitiate/tools/builtin_tools.py
--rw-r--r--   0        0        0      619 2024-05-01 09:44:28.917974 aiinitiate-0.1.5/aiinitiate/tools/downloader.py
--rw-r--r--   0        0        0      257 2024-05-01 09:58:21.252629 aiinitiate-0.1.5/aiinitiate/tools/setter/__init__.py
--rw-r--r--   0        0        0     3569 2024-05-01 09:58:55.764241 aiinitiate-0.1.5/aiinitiate/tools/setter/base.py
--rw-r--r--   0        0        0     2506 2024-05-01 09:44:28.925974 aiinitiate-0.1.5/aiinitiate/tools/tool.py
--rw-r--r--   0        0        0      433 2024-05-01 10:47:23.306060 aiinitiate-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 aiinitiate-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-01 10:49:30.670293 aiinitiate-0.1.6/aiinitiate/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:01:03.874802 aiinitiate-0.1.6/aiinitiate/basic/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-01 10:02:48.805624 aiinitiate-0.1.6/aiinitiate/basic/common_utils.py
+-rw-r--r--   0        0        0     3744 2024-05-01 10:44:23.735560 aiinitiate-0.1.6/aiinitiate/cli.py
+-rw-r--r--   0        0        0      706 2024-05-01 09:36:43.043223 aiinitiate-0.1.6/aiinitiate/config.py
+-rw-r--r--   0        0        0     3349 2024-05-01 10:41:01.194134 aiinitiate-0.1.6/aiinitiate/g.py
+-rw-r--r--   0        0        0     2959 2024-05-01 10:48:31.192040 aiinitiate-0.1.6/aiinitiate/sysinfo.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:39:39.205235 aiinitiate-0.1.6/aiinitiate/tools/__init__.py
+-rw-r--r--   0        0        0     2918 2024-05-01 09:54:24.055293 aiinitiate-0.1.6/aiinitiate/tools/builtin_tools.py
+-rw-r--r--   0        0        0      619 2024-05-01 09:44:28.917974 aiinitiate-0.1.6/aiinitiate/tools/downloader.py
+-rw-r--r--   0        0        0      257 2024-05-01 09:58:21.252629 aiinitiate-0.1.6/aiinitiate/tools/setter/__init__.py
+-rw-r--r--   0        0        0     3569 2024-05-01 09:58:55.764241 aiinitiate-0.1.6/aiinitiate/tools/setter/base.py
+-rw-r--r--   0        0        0     2506 2024-05-01 09:44:28.925974 aiinitiate-0.1.6/aiinitiate/tools/tool.py
+-rw-r--r--   0        0        0      433 2024-05-01 10:49:41.177986 aiinitiate-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 aiinitiate-0.1.6/PKG-INFO
```

### Comparing `aiinitiate-0.1.5/aiinitiate/basic/common_utils.py` & `aiinitiate-0.1.6/aiinitiate/basic/common_utils.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/cli.py` & `aiinitiate-0.1.6/aiinitiate/cli.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/config.py` & `aiinitiate-0.1.6/aiinitiate/config.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/g.py` & `aiinitiate-0.1.6/aiinitiate/g.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/sysinfo.py` & `aiinitiate-0.1.6/aiinitiate/sysinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return uuid.UUID(int=uuid.getnode()).hex[-12:]
 
 
 def get_local_ip():
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.connect("8.8.8.8", 80)
-        ip = s.getsockname()()[0]
+        ip = s.getsockname()[0]
     finally:
         s.close()
     return ip
 
 
 def get_public_ip():
     response = requests.get('https://api.ipify.org')
```

### Comparing `aiinitiate-0.1.5/aiinitiate/tools/builtin_tools.py` & `aiinitiate-0.1.6/aiinitiate/tools/builtin_tools.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/tools/downloader.py` & `aiinitiate-0.1.6/aiinitiate/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/tools/setter/base.py` & `aiinitiate-0.1.6/aiinitiate/tools/setter/base.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/aiinitiate/tools/tool.py` & `aiinitiate-0.1.6/aiinitiate/tools/tool.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.5/PKG-INFO` & `aiinitiate-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiinitiate
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: CachCheng
 Author-email: tkggpdc2007@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

