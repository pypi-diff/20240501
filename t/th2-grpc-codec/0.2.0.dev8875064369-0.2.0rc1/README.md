# Comparing `tmp/th2_grpc_codec-0.2.0.dev8875064369.tar.gz` & `tmp/th2_grpc_codec-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_codec-0.2.0.dev8875064369.tar", last modified: Mon Apr 29 07:47:59 2024, max compression
+gzip compressed data, was "dist/th2_grpc_codec-0.2.0rc1.tar", last modified: Wed May  1 07:17:22 2024, max compression
```

## Comparing `th2_grpc_codec-0.2.0.dev8875064369.tar` & `th2_grpc_codec-0.2.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-29 07:47:11.000000 th2_grpc_codec-0.2.0.dev8875064369/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 07:47:11.000000 th2_grpc_codec-0.2.0.dev8875064369/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-29 07:47:11.000000 th2_grpc_codec-0.2.0.dev8875064369/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-29 07:47:11.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-29 07:47:58.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 07:47:58.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 07:47:58.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 07:47:42.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_service.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 07:47:59.000000 th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-01 07:16:31.000000 th2_grpc_codec-0.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 07:16:31.000000 th2_grpc_codec-0.2.0rc1/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-01 07:16:31.000000 th2_grpc_codec-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-01 07:16:31.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-01 07:17:08.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 07:17:22.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 07:17:21.000000 th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/top_level.txt
```

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/PKG-INFO` & `th2_grpc_codec-0.2.0rc1/th2_grpc_codec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_codec
-Version: 0.2.0.dev8875064369
+Name: th2-grpc-codec
+Version: 0.2.0rc1
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC codec library (0.2.0)
```

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/README.md` & `th2_grpc_codec-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/setup.py` & `th2_grpc_codec-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec.proto` & `th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2.py` & `th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2.pyi` & `th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec/codec_pb2_grpc.py` & `th2_grpc_codec-0.2.0rc1/th2_grpc_codec/codec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8875064369/th2_grpc_codec.egg-info/PKG-INFO` & `th2_grpc_codec-0.2.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-codec
-Version: 0.2.0.dev8875064369
+Name: th2_grpc_codec
+Version: 0.2.0rc1
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC codec library (0.2.0)
```

