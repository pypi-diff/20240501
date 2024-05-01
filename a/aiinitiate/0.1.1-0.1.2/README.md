# Comparing `tmp/aiinitiate-0.1.1.tar.gz` & `tmp/aiinitiate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiinitiate-0.1.1.tar", max compression
+gzip compressed data, was "aiinitiate-0.1.2.tar", max compression
```

## Comparing `aiinitiate-0.1.1.tar` & `aiinitiate-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-05-01 09:31:17.094915 aiinitiate-0.1.1/aiinitiate/__init__.py
--rw-r--r--   0        0        0     1159 2024-05-01 08:48:43.743703 aiinitiate-0.1.1/aiinitiate/cli.py
--rw-r--r--   0        0        0     2607 2024-05-01 08:05:05.053797 aiinitiate-0.1.1/aiinitiate/sysinfo.py
--rw-r--r--   0        0        0      282 2024-05-01 09:31:17.098914 aiinitiate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 aiinitiate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-01 10:06:12.647334 aiinitiate-0.1.2/aiinitiate/__init__.py
+-rw-r--r--   0        0        0     3636 2024-05-01 10:14:11.525955 aiinitiate-0.1.2/aiinitiate/cli.py
+-rw-r--r--   0        0        0     2608 2024-05-01 09:39:08.221584 aiinitiate-0.1.2/aiinitiate/sysinfo.py
+-rw-r--r--   0        0        0      342 2024-05-01 10:15:37.064994 aiinitiate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 aiinitiate-0.1.2/PKG-INFO
```

### Comparing `aiinitiate-0.1.1/aiinitiate/sysinfo.py` & `aiinitiate-0.1.2/aiinitiate/sysinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """
     获取设备mac地址
     :return:
     """
     return uuid.UUID(int=uuid.getnode()).hex[-12:]
 
 
-def get_device_info():
+def get_device_model():
     """
     获取设备型号信息
     :return:
     """
     system = platform.system()
     if system == 'Linux':  # For Linux systems
         try:
```

### Comparing `aiinitiate-0.1.1/PKG-INFO` & `aiinitiate-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aiinitiate
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: CachCheng
 Author-email: tkggpdc2007@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typer (==0.9.4)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
```

