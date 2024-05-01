# Comparing `tmp/SparkleLogging-1.0.0.tar.gz` & `tmp/SparkleLogging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.0.tar", last modified: Wed May  1 05:45:49 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.1.tar", last modified: Wed May  1 06:02:19 2024, max compression
```

## Comparing `SparkleLogging-1.0.0.tar` & `SparkleLogging-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 05:45:49.684551 SparkleLogging-1.0.0/
--rw-rw-rw-   0        0        0     2112 2024-05-01 05:45:49.682555 SparkleLogging-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 05:45:49.679563 SparkleLogging-1.0.0/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-05-01 05:45:48.000000 SparkleLogging-1.0.0/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-05-01 05:45:49.000000 SparkleLogging-1.0.0/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 05:45:48.000000 SparkleLogging-1.0.0/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-01 05:45:48.000000 SparkleLogging-1.0.0/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 05:45:48.000000 SparkleLogging-1.0.0/SparkleLogging.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 05:45:49.668592 SparkleLogging-1.0.0/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.0/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.0/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.0/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.0/plugins/websocketHander.py
--rw-rw-rw-   0        0        0       42 2024-05-01 05:45:49.685547 SparkleLogging-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      715 2024-05-01 05:45:31.000000 SparkleLogging-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:45:49.672580 SparkleLogging-1.0.0/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.0/utils/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.0/utils/core.py
--rw-rw-rw-   0        0        0     4761 2024-05-01 05:44:46.000000 SparkleLogging-1.0.0/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.0/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.144002 SparkleLogging-1.0.1/
+-rw-rw-rw-   0        0        0     2136 2024-05-01 06:02:19.143005 SparkleLogging-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.142008 SparkleLogging-1.0.1/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     2136 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.113927 SparkleLogging-1.0.1/plugins/
+-rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.1/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.1/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.1/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.1/plugins/websocketHander.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 06:02:19.144002 SparkleLogging-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-01 06:02:05.000000 SparkleLogging-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.140014 SparkleLogging-1.0.1/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.1/utils/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.1/utils/core.py
+-rw-rw-rw-   0        0        0     4761 2024-05-01 05:44:46.000000 SparkleLogging-1.0.1/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.1/utils/plugins_for_core.py
```

### Comparing `SparkleLogging-1.0.0/PKG-INFO` & `SparkleLogging-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging library for Python
-Home-page: https://github.com/KOKOMI12345/Log4p
+Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
@@ -22,15 +22,15 @@
 这是一个可以支持异步记录日志,发送到HTTP,websocket服务器,同时配置简单,它还实现了识别代码异步和同步的环境
 以支持不同环境下的日志记录,当然了,理论上,这个日志如果2个模式都启用(websocket,http),那么会分别的往2个地方发送日志
 
 ### 示例用法
 
 ```python
 #from core import *
-from Log4p.core import LogManager
+from SparkleLogging.utils.core import LogManager
 from logging import Formatter
 
 logger = LogManager().GetLogger(
     log_name='example',
     out_to_console=True,
     web_log_mode=True,
     WSpost_url='ws://localhost:8765',
```

### Comparing `SparkleLogging-1.0.0/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.1/SparkleLogging.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging library for Python
-Home-page: https://github.com/KOKOMI12345/Log4p
+Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
@@ -22,15 +22,15 @@
 这是一个可以支持异步记录日志,发送到HTTP,websocket服务器,同时配置简单,它还实现了识别代码异步和同步的环境
 以支持不同环境下的日志记录,当然了,理论上,这个日志如果2个模式都启用(websocket,http),那么会分别的往2个地方发送日志
 
 ### 示例用法
 
 ```python
 #from core import *
-from Log4p.core import LogManager
+from SparkleLogging.utils.core import LogManager
 from logging import Formatter
 
 logger = LogManager().GetLogger(
     log_name='example',
     out_to_console=True,
     web_log_mode=True,
     WSpost_url='ws://localhost:8765',
```

### Comparing `SparkleLogging-1.0.0/plugins/HttpHander.py` & `SparkleLogging-1.0.1/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.0/plugins/websocketHander.py` & `SparkleLogging-1.0.1/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.0/setup.py` & `SparkleLogging-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/KOKOMI12345/Log4p',
+    url='https://github.com/KOKOMI12345/SparkleLogging',
     install_requires=[
         'requests',
         'websockets',
         'colorlog',
         'httpx',
     ],
     classifiers=[
```

### Comparing `SparkleLogging-1.0.0/utils/getLog.py` & `SparkleLogging-1.0.1/utils/getLog.py`

 * *Files identical despite different names*
