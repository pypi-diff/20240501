# Comparing `tmp/aiinitiate-0.1.2.tar.gz` & `tmp/aiinitiate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiinitiate-0.1.2.tar", max compression
+gzip compressed data, was "aiinitiate-0.1.3.tar", max compression
```

## Comparing `aiinitiate-0.1.2.tar` & `aiinitiate-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.2/README.md
--rw-r--r--   0        0        0       22 2024-05-01 10:06:12.647334 aiinitiate-0.1.2/aiinitiate/__init__.py
--rw-r--r--   0        0        0     3636 2024-05-01 10:14:11.525955 aiinitiate-0.1.2/aiinitiate/cli.py
--rw-r--r--   0        0        0     2608 2024-05-01 09:39:08.221584 aiinitiate-0.1.2/aiinitiate/sysinfo.py
--rw-r--r--   0        0        0      342 2024-05-01 10:15:37.064994 aiinitiate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 aiinitiate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 07:21:29.416720 aiinitiate-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-01 10:06:12.647334 aiinitiate-0.1.3/aiinitiate/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:01:03.874802 aiinitiate-0.1.3/aiinitiate/basic/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-01 10:02:48.805624 aiinitiate-0.1.3/aiinitiate/basic/common_utils.py
+-rw-r--r--   0        0        0     3401 2024-05-01 10:17:40.175945 aiinitiate-0.1.3/aiinitiate/cli.py
+-rw-r--r--   0        0        0      706 2024-05-01 09:36:43.043223 aiinitiate-0.1.3/aiinitiate/config.py
+-rw-r--r--   0        0        0     3232 2024-05-01 10:04:40.796366 aiinitiate-0.1.3/aiinitiate/g.py
+-rw-r--r--   0        0        0     2608 2024-05-01 09:39:08.221584 aiinitiate-0.1.3/aiinitiate/sysinfo.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:39:39.205235 aiinitiate-0.1.3/aiinitiate/tools/__init__.py
+-rw-r--r--   0        0        0     2918 2024-05-01 09:54:24.055293 aiinitiate-0.1.3/aiinitiate/tools/builtin_tools.py
+-rw-r--r--   0        0        0      619 2024-05-01 09:44:28.917974 aiinitiate-0.1.3/aiinitiate/tools/downloader.py
+-rw-r--r--   0        0        0      257 2024-05-01 09:58:21.252629 aiinitiate-0.1.3/aiinitiate/tools/setter/__init__.py
+-rw-r--r--   0        0        0     3569 2024-05-01 09:58:55.764241 aiinitiate-0.1.3/aiinitiate/tools/setter/base.py
+-rw-r--r--   0        0        0     2506 2024-05-01 09:44:28.925974 aiinitiate-0.1.3/aiinitiate/tools/tool.py
+-rw-r--r--   0        0        0      412 2024-05-01 10:19:28.194377 aiinitiate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 aiinitiate-0.1.3/PKG-INFO
```

### Comparing `aiinitiate-0.1.2/aiinitiate/cli.py` & `aiinitiate-0.1.3/aiinitiate/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
-# from . import g, __version__
-# from .basic.common_utils import install_common_utils
+from . import g, __version__
+from .basic.common_utils import install_common_utils
 
 app = typer.Typer()
 
 
 @app.command()
 def logo():
     logo = """
@@ -13,144 +13,144 @@
     ███████ ██ ███████ ██ ██ ██  ██ ██    ██    ██    ██ ██ ██ ██  ██ 
     ██   ██ ██      ██ ██ ██  ██ ██ ██    ██    ██    ██ ██ ██  ██ ██ 
     ██   ██ ██ ███████ ██ ██   ████ ██    ██     ██████  ██ ██   ████ 
     """
     typer.echo(logo)
 
 
-# @app.command()
-# def version():
-#     """
-#     版本信息
-#     """
-#     typer.echo(f"{__version__}")
-#
-#
-# @app.command()
-# def setup():
-#     """
-#     自动安装各种内置工具
-#     """
-#     install_common_utils()
-#
-#     init_tools = ["filebrowser", "coral-gateway"]
-#     for name in init_tools:
-#         # 加载对应工具
-#         g.add_builtin_tool(name)
-#         # 启动对应工具
-#         g.start_tool(name)
-#
-#
-# @app.command()
-# def add_tool(name: str):
-#     """
-#     下载基础工具到本地
-#     """
-#     g.add_builtin_tool(name)
-#
-#
-# @app.command()
-# def start_tool(name: str):
-#     """
-#     启动工具
-#     """
-#     g.start_tool(name)
-#
-#
-# @app.command()
-# def stop_tool(name: str):
-#     """
-#     停止工具
-#     """
-#     g.stop_tool(name)
-#
-#
-# @app.command()
-# def restart_tool(name: str):
-#     """
-#     重启工具
-#     """
-#     g.restart_tool(name)
-#
-#
-# @app.command()
-# def remove_tool(name: str):
-#     """
-#     删除工具
-#     """
-#     g.remove_tool(name)
-#
-#
-# @app.command()
-# def handle_tool_action(name: str, action: str, params: str = "{}"):
-#     tool = g.get_tool(name)
-#     tool.handle_action(action, json.loads(params))
-#
-#
-# @app.command()
-# def list_tool_action(name):
-#     """
-#     列出工具支持的操作
-#     """
-#     tool = g.get_tool(name)
-#     tool.list_action()
-#
-#
-# @app.command()
-# def list_tool():
-#     """
-#     查看工具列表
-#     :return:
-#     """
-#     for item in g.list_tool():
-#         typer.echo(f"[ {'✅' if item['installed'] else '❎'} ] {item['name']}")
-#
-#
-# @app.command()
-# def mac():
-#     """
-#     获取设备的mac地址
-#     """
-#     mac_address = g.mac_addr()
-#     typer.echo(f"Device MAC Address: {mac_address}")
-#
-#
-# @app.command()
-# def dist():
-#     """
-#     输出系统版本信息
-#     """
-#     dist_name = g.distribution_name()
-#     dist_id = g.distribution_id()
-#     typer.echo(f"dist id: {dist_id}")
-#     typer.echo(f"dist name: {dist_name}")
-#
-#
-# @app.command()
-# def npu():
-#     """
-#     npu信息[仅RK设备支持此命令]
-#     """
-#     typer.echo(g.npu())
-#
-#
-# @app.command()
-# def device_model():
-#     """
-#     获取设备详细型号信息
-#     """
-#     typer.echo(g.device_model())
-#
-#
-# @app.command()
-# def device_type():
-#     """
-#     获取设备类型信息
-#     """
-#     typer.echo(g.device_type())
+@app.command()
+def version():
+    """
+    版本信息
+    """
+    typer.echo(f"{__version__}")
+
+
+@app.command()
+def setup():
+    """
+    自动安装各种内置工具
+    """
+    install_common_utils()
+
+    init_tools = ["filebrowser", "coral-gateway"]
+    for name in init_tools:
+        # 加载对应工具
+        g.add_builtin_tool(name)
+        # 启动对应工具
+        g.start_tool(name)
+
+
+@app.command()
+def add_tool(name: str):
+    """
+    下载基础工具到本地
+    """
+    g.add_builtin_tool(name)
+
+
+@app.command()
+def start_tool(name: str):
+    """
+    启动工具
+    """
+    g.start_tool(name)
+
+
+@app.command()
+def stop_tool(name: str):
+    """
+    停止工具
+    """
+    g.stop_tool(name)
+
+
+@app.command()
+def restart_tool(name: str):
+    """
+    重启工具
+    """
+    g.restart_tool(name)
+
+
+@app.command()
+def remove_tool(name: str):
+    """
+    删除工具
+    """
+    g.remove_tool(name)
+
+
+@app.command()
+def handle_tool_action(name: str, action: str, params: str = "{}"):
+    tool = g.get_tool(name)
+    tool.handle_action(action, json.loads(params))
+
+
+@app.command()
+def list_tool_action(name):
+    """
+    列出工具支持的操作
+    """
+    tool = g.get_tool(name)
+    tool.list_action()
+
+
+@app.command()
+def list_tool():
+    """
+    查看工具列表
+    :return:
+    """
+    for item in g.list_tool():
+        typer.echo(f"[ {'✅' if item['installed'] else '❎'} ] {item['name']}")
+
+
+@app.command()
+def mac():
+    """
+    获取设备的mac地址
+    """
+    mac_address = g.mac_addr()
+    typer.echo(f"Device MAC Address: {mac_address}")
+
+
+@app.command()
+def dist():
+    """
+    输出系统版本信息
+    """
+    dist_name = g.distribution_name()
+    dist_id = g.distribution_id()
+    typer.echo(f"dist id: {dist_id}")
+    typer.echo(f"dist name: {dist_name}")
+
+
+@app.command()
+def npu():
+    """
+    npu信息[仅RK设备支持此命令]
+    """
+    typer.echo(g.npu())
+
+
+@app.command()
+def device_model():
+    """
+    获取设备详细型号信息
+    """
+    typer.echo(g.device_model())
+
+
+@app.command()
+def device_type():
+    """
+    获取设备类型信息
+    """
+    typer.echo(g.device_type())
 
 
 @app.command()
 def main():
     logo()
     typer.echo("Welcome to AIInitiate command!")
```

### Comparing `aiinitiate-0.1.2/aiinitiate/sysinfo.py` & `aiinitiate-0.1.3/aiinitiate/sysinfo.py`

 * *Files identical despite different names*

### Comparing `aiinitiate-0.1.2/PKG-INFO` & `aiinitiate-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: aiinitiate
-Version: 0.1.2
+Version: 0.1.3
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
+Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
```

