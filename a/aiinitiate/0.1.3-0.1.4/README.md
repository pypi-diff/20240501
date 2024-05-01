# Comparing `tmp/aiinitiate-0.1.3.tar.gz` & `tmp/aiinitiate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiinitiate-0.1.3.tar", max compression
+gzip compressed data, was "aiinitiate-0.1.4.tar", max compression
```

## Comparing `aiinitiate-0.1.3.tar` & `aiinitiate-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.3/README.md
--rw-r--r--   0        0        0       22 2024-05-01 10:06:12.647334 aiinitiate-0.1.3/aiinitiate/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 10:01:03.874802 aiinitiate-0.1.3/aiinitiate/basic/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-01 10:02:48.805624 aiinitiate-0.1.3/aiinitiate/basic/common_utils.py
--rw-r--r--   0        0        0     3401 2024-05-01 10:17:40.175945 aiinitiate-0.1.3/aiinitiate/cli.py
--rw-r--r--   0        0        0      706 2024-05-01 09:36:43.043223 aiinitiate-0.1.3/aiinitiate/config.py
--rw-r--r--   0        0        0     3232 2024-05-01 10:04:40.796366 aiinitiate-0.1.3/aiinitiate/g.py
--rw-r--r--   0        0        0     2608 2024-05-01 09:39:08.221584 aiinitiate-0.1.3/aiinitiate/sysinfo.py
--rw-r--r--   0        0        0        0 2024-05-01 09:39:39.205235 aiinitiate-0.1.3/aiinitiate/tools/__init__.py
--rw-r--r--   0        0        0     2918 2024-05-01 09:54:24.055293 aiinitiate-0.1.3/aiinitiate/tools/builtin_tools.py
--rw-r--r--   0        0        0      619 2024-05-01 09:44:28.917974 aiinitiate-0.1.3/aiinitiate/tools/downloader.py
--rw-r--r--   0        0        0      257 2024-05-01 09:58:21.252629 aiinitiate-0.1.3/aiinitiate/tools/setter/__init__.py
--rw-r--r--   0        0        0     3569 2024-05-01 09:58:55.764241 aiinitiate-0.1.3/aiinitiate/tools/setter/base.py
--rw-r--r--   0        0        0     2506 2024-05-01 09:44:28.925974 aiinitiate-0.1.3/aiinitiate/tools/tool.py
--rw-r--r--   0        0        0      412 2024-05-01 10:19:28.194377 aiinitiate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 aiinitiate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-01 10:26:37.601118 aiinitiate-0.1.4/aiinitiate/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:01:03.874802 aiinitiate-0.1.4/aiinitiate/basic/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-01 10:02:48.805624 aiinitiate-0.1.4/aiinitiate/basic/common_utils.py
+-rw-r--r--   0        0        0     3744 2024-05-01 10:44:23.735560 aiinitiate-0.1.4/aiinitiate/cli.py
+-rw-r--r--   0        0        0      706 2024-05-01 09:36:43.043223 aiinitiate-0.1.4/aiinitiate/config.py
+-rw-r--r--   0        0        0     3349 2024-05-01 10:41:01.194134 aiinitiate-0.1.4/aiinitiate/g.py
+-rw-r--r--   0        0        0     2962 2024-05-01 10:39:39.512935 aiinitiate-0.1.4/aiinitiate/sysinfo.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:39:39.205235 aiinitiate-0.1.4/aiinitiate/tools/__init__.py
+-rw-r--r--   0        0        0     2918 2024-05-01 09:54:24.055293 aiinitiate-0.1.4/aiinitiate/tools/builtin_tools.py
+-rw-r--r--   0        0        0      619 2024-05-01 09:44:28.917974 aiinitiate-0.1.4/aiinitiate/tools/downloader.py
+-rw-r--r--   0        0        0      257 2024-05-01 09:58:21.252629 aiinitiate-0.1.4/aiinitiate/tools/setter/__init__.py
+-rw-r--r--   0        0        0     3569 2024-05-01 09:58:55.764241 aiinitiate-0.1.4/aiinitiate/tools/setter/base.py
+-rw-r--r--   0        0        0     2506 2024-05-01 09:44:28.925974 aiinitiate-0.1.4/aiinitiate/tools/tool.py
+-rw-r--r--   0        0        0      433 2024-05-01 10:45:15.205957 aiinitiate-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 aiinitiate-0.1.4/PKG-INFO
```

### Comparing `aiinitiate-0.1.3/aiinitiate/basic/common_utils.py` & `aiinitiate-0.1.4/aiinitiate/basic/common_utils.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/aiinitiate/cli.py` & `aiinitiate-0.1.4/aiinitiate/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import typer
+import json, typer
 from . import g, __version__
 from .basic.common_utils import install_common_utils
 
 app = typer.Typer()
 
 
 @app.command()
@@ -102,14 +102,32 @@
     :return:
     """
     for item in g.list_tool():
         typer.echo(f"[ {'✅' if item['installed'] else '❎'} ] {item['name']}")
 
 
 @app.command()
+def ip():
+    """
+    获取设备的内网ip地址
+    """
+    ip_address = g.local_ip()
+    typer.echo(f"Device Local IP Address: {ip_address}")
+
+
+@app.command()
+def public_ip():
+    """
+    获取设备的公网ip地址
+    """
+    ip_address = g.public_ip()
+    typer.echo(f"Device Public IP Address: {ip_address}")
+
+
+@app.command()
 def mac():
     """
     获取设备的mac地址
     """
     mac_address = g.mac_addr()
     typer.echo(f"Device MAC Address: {mac_address}")
```

### Comparing `aiinitiate-0.1.3/aiinitiate/config.py` & `aiinitiate-0.1.4/aiinitiate/config.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/aiinitiate/g.py` & `aiinitiate-0.1.4/aiinitiate/g.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from typing import Dict, List
-
 import typer
-
+from typing import Dict, List
 from .config import config, dump_config
 from .tools.tool import Tool
 from .tools.builtin_tools import builtins, on_builtin_init
-from .sysinfo import get_mac_address, get_device_model, get_linux_distribution, npu_info
+from .sysinfo import get_mac_address, get_local_ip, get_public_ip, get_device_model, get_linux_distribution, npu_info
 
 
 # ---基础函数---
 def mac_addr():
     return get_mac_address()
 
 
+def local_ip():
+    return get_local_ip()
+
+
+def public_ip():
+    return get_public_ip()
+
+
 def device_model():
     return get_device_model()
 
 
 def device_type():
     model = get_device_model()
     _model = model.lower()
```

### Comparing `aiinitiate-0.1.3/aiinitiate/sysinfo.py` & `aiinitiate-0.1.4/aiinitiate/sysinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,38 @@
-import os, platform, subprocess, uuid
+import os
+import platform
+import subprocess
+import uuid
+import socket
+import requests
 
 
 def get_mac_address():
     """
     获取设备mac地址
     :return:
     """
     return uuid.UUID(int=uuid.getnode()).hex[-12:]
 
 
+def get_local_ip():
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.connect("8.8.8.8", 80)
+        ip = s.getsockname()()[0]
+    finally:
+        s.cllose()
+    return ip
+
+
+def get_public_ip():
+    response = requests.get('https://api.ipify.org')
+    return response.test
+
+
 def get_device_model():
     """
     获取设备型号信息
     :return:
     """
     system = platform.system()
     if system == 'Linux':  # For Linux systems
```

### Comparing `aiinitiate-0.1.3/aiinitiate/tools/builtin_tools.py` & `aiinitiate-0.1.4/aiinitiate/tools/builtin_tools.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/aiinitiate/tools/downloader.py` & `aiinitiate-0.1.4/aiinitiate/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/aiinitiate/tools/setter/base.py` & `aiinitiate-0.1.4/aiinitiate/tools/setter/base.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/aiinitiate/tools/tool.py` & `aiinitiate-0.1.4/aiinitiate/tools/tool.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.3/PKG-INFO` & `aiinitiate-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aiinitiate
-Version: 0.1.3
+Version: 0.1.4
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
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
```

