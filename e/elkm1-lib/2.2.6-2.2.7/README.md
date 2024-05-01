# Comparing `tmp/elkm1_lib-2.2.6.tar.gz` & `tmp/elkm1_lib-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkm1_lib-2.2.6.tar", max compression
+gzip compressed data, was "elkm1_lib-2.2.7.tar", max compression
```

## Comparing `elkm1_lib-2.2.6.tar` & `elkm1_lib-2.2.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     9610 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/CHANGELOG.md
--rw-r--r--   0        0        0     9289 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/README.md
--rw-r--r--   0        0        0    12509 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/bin/cmdr.py
--rwxr-xr-x   0        0        0     3088 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/bin/elk
--rwxr-xr-x   0        0        0     2165 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/bin/mkdoc
--rwxr-xr-x   0        0        0     1259 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/bin/simple
--rwxr-xr-x   0        0        0     2117 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/bin/test-serial
--rw-r--r--   0        0        0       41 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/elkm1_lib/__init__.py
--rw-r--r--   0        0        0     5127 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/elkm1_lib/areas.py
--rw-r--r--   0        0        0     7032 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/elkm1_lib/connection.py
--rw-r--r--   0        0        0    10373 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/elkm1_lib/const.py
--rw-r--r--   0        0        0     1424 2023-09-17 23:26:20.655312 elkm1_lib-2.2.6/elkm1_lib/counters.py
--rw-r--r--   0        0        0     5788 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/discovery.py
--rw-r--r--   0        0        0     5119 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/elements.py
--rw-r--r--   0        0        0     5183 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/elk.py
--rw-r--r--   0        0        0     3586 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/keypads.py
--rw-r--r--   0        0        0     1835 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/lights.py
--rw-r--r--   0        0        0    18619 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/message.py
--rw-r--r--   0        0        0     1478 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/notify.py
--rw-r--r--   0        0        0     1691 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/outputs.py
--rw-r--r--   0        0        0     4437 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/panel.py
--rw-r--r--   0        0        0        0 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/py.typed
--rw-r--r--   0        0        0     1848 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/settings.py
--rw-r--r--   0        0        0     1096 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/tasks.py
--rw-r--r--   0        0        0     3196 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/thermostats.py
--rw-r--r--   0        0        0      974 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/users.py
--rw-r--r--   0        0        0     2516 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/util.py
--rw-r--r--   0        0        0     4933 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/elkm1_lib/zones.py
--rw-r--r--   0        0        0     1943 2023-09-17 23:26:20.659312 elkm1_lib-2.2.6/pyproject.toml
--rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 elkm1_lib-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0     9610 2022-12-01 01:08:00.053248 elkm1_lib-2.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2021-11-11 16:09:20.666353 elkm1_lib-2.2.7/LICENCE
+-rw-r--r--   0        0        0     9289 2022-12-01 01:06:13.075080 elkm1_lib-2.2.7/README.md
+-rw-r--r--   0        0        0    12509 2022-05-12 13:50:09.033080 elkm1_lib-2.2.7/bin/cmdr.py
+-rwxr-xr-x   0        0        0     3088 2023-06-11 20:56:06.150889 elkm1_lib-2.2.7/bin/elk
+-rwxr-xr-x   0        0        0     2165 2022-05-12 13:50:09.033413 elkm1_lib-2.2.7/bin/mkdoc
+-rwxr-xr-x   0        0        0     1259 2022-11-27 23:42:10.746410 elkm1_lib-2.2.7/bin/simple
+-rwxr-xr-x   0        0        0     2117 2022-04-29 01:35:42.861060 elkm1_lib-2.2.7/bin/test-serial
+-rw-r--r--   0        0        0       41 2022-04-13 02:33:50.735783 elkm1_lib-2.2.7/elkm1_lib/__init__.py
+-rw-r--r--   0        0        0     5127 2022-11-30 23:38:54.629315 elkm1_lib-2.2.7/elkm1_lib/areas.py
+-rw-r--r--   0        0        0     7037 2024-05-01 19:57:06.020001 elkm1_lib-2.2.7/elkm1_lib/connection.py
+-rw-r--r--   0        0        0    10373 2022-11-30 23:38:54.630129 elkm1_lib-2.2.7/elkm1_lib/const.py
+-rw-r--r--   0        0        0     1424 2022-11-30 23:38:54.630391 elkm1_lib-2.2.7/elkm1_lib/counters.py
+-rw-r--r--   0        0        0     5788 2024-03-03 01:50:44.597475 elkm1_lib-2.2.7/elkm1_lib/discovery.py
+-rw-r--r--   0        0        0     5119 2022-11-30 23:38:54.630665 elkm1_lib-2.2.7/elkm1_lib/elements.py
+-rw-r--r--   0        0        0     5183 2024-02-10 04:39:48.822997 elkm1_lib-2.2.7/elkm1_lib/elk.py
+-rw-r--r--   0        0        0     3586 2022-11-30 23:38:54.631665 elkm1_lib-2.2.7/elkm1_lib/keypads.py
+-rw-r--r--   0        0        0     1835 2022-05-12 13:50:46.802719 elkm1_lib-2.2.7/elkm1_lib/lights.py
+-rw-r--r--   0        0        0    18619 2022-11-30 23:38:54.632014 elkm1_lib-2.2.7/elkm1_lib/message.py
+-rw-r--r--   0        0        0     1478 2022-11-18 00:06:47.611012 elkm1_lib-2.2.7/elkm1_lib/notify.py
+-rw-r--r--   0        0        0     1691 2022-05-12 13:50:46.803107 elkm1_lib-2.2.7/elkm1_lib/outputs.py
+-rw-r--r--   0        0        0     4437 2022-11-29 05:31:05.986969 elkm1_lib-2.2.7/elkm1_lib/panel.py
+-rw-r--r--   0        0        0        0 2022-04-18 19:22:30.371621 elkm1_lib-2.2.7/elkm1_lib/py.typed
+-rw-r--r--   0        0        0     1848 2022-05-12 13:50:46.803404 elkm1_lib-2.2.7/elkm1_lib/settings.py
+-rw-r--r--   0        0        0     1096 2022-05-12 13:50:46.803541 elkm1_lib-2.2.7/elkm1_lib/tasks.py
+-rw-r--r--   0        0        0     3196 2022-11-30 23:38:54.632317 elkm1_lib-2.2.7/elkm1_lib/thermostats.py
+-rw-r--r--   0        0        0      974 2022-05-12 13:50:46.803805 elkm1_lib-2.2.7/elkm1_lib/users.py
+-rw-r--r--   0        0        0     2516 2024-03-03 01:50:44.597858 elkm1_lib-2.2.7/elkm1_lib/util.py
+-rw-r--r--   0        0        0     4933 2022-11-29 05:31:05.993081 elkm1_lib-2.2.7/elkm1_lib/zones.py
+-rw-r--r--   0        0        0     1951 2024-05-01 19:59:02.492941 elkm1_lib-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 elkm1_lib-2.2.7/PKG-INFO
```

### Comparing `elkm1_lib-2.2.6/CHANGELOG.md` & `elkm1_lib-2.2.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/README.md` & `elkm1_lib-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/bin/cmdr.py` & `elkm1_lib-2.2.7/bin/cmdr.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/bin/elk` & `elkm1_lib-2.2.7/bin/elk`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/bin/mkdoc` & `elkm1_lib-2.2.7/bin/mkdoc`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/bin/simple` & `elkm1_lib-2.2.7/bin/simple`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/bin/test-serial` & `elkm1_lib-2.2.7/bin/test-serial`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/areas.py` & `elkm1_lib-2.2.7/elkm1_lib/areas.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/connection.py` & `elkm1_lib-2.2.7/elkm1_lib/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 import logging
 import sys
 from collections import deque
 from functools import reduce
 from typing import Any, NamedTuple
 
-from serial_asyncio import open_serial_connection
+from serial_asyncio_fast import open_serial_connection
 
 from .message import MessageEncode, decode, get_elk_command
 from .notify import Notifier
 from .util import parse_url
 
 if sys.version_info[:2] < (3, 11):
     from async_timeout import timeout as asyncio_timeout  # pyright: ignore
```

### Comparing `elkm1_lib-2.2.6/elkm1_lib/const.py` & `elkm1_lib-2.2.7/elkm1_lib/const.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/counters.py` & `elkm1_lib-2.2.7/elkm1_lib/counters.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/discovery.py` & `elkm1_lib-2.2.7/elkm1_lib/discovery.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/elements.py` & `elkm1_lib-2.2.7/elkm1_lib/elements.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/elk.py` & `elkm1_lib-2.2.7/elkm1_lib/elk.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/keypads.py` & `elkm1_lib-2.2.7/elkm1_lib/keypads.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/lights.py` & `elkm1_lib-2.2.7/elkm1_lib/lights.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/message.py` & `elkm1_lib-2.2.7/elkm1_lib/message.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/notify.py` & `elkm1_lib-2.2.7/elkm1_lib/notify.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/outputs.py` & `elkm1_lib-2.2.7/elkm1_lib/outputs.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/panel.py` & `elkm1_lib-2.2.7/elkm1_lib/panel.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/settings.py` & `elkm1_lib-2.2.7/elkm1_lib/settings.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/tasks.py` & `elkm1_lib-2.2.7/elkm1_lib/tasks.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/thermostats.py` & `elkm1_lib-2.2.7/elkm1_lib/thermostats.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/users.py` & `elkm1_lib-2.2.7/elkm1_lib/users.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/util.py` & `elkm1_lib-2.2.7/elkm1_lib/util.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/elkm1_lib/zones.py` & `elkm1_lib-2.2.7/elkm1_lib/zones.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.6/pyproject.toml` & `elkm1_lib-2.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "elkm1-lib"
-version = "2.2.6"
+version = "2.2.7"
 description = "Library for interacting with ElkM1 alarm/automation panel."
 homepage = "https://github.com/gwww/elkm1"
 authors = ["Glenn Waters <gwwaters+elkm1@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
 ]
 include = ["CHANGELOG.md", "bin/**/*"]
 exclude = ["test"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pyserial-asyncio = ">= 0.5"
+python = "^3.11"
+pyserial-asyncio-fast = ">= 0.11"
 async-timeout = "^4.0"
 
 [tool.poetry.group.dev.dependencies]
 attrs = ">=21.2"
-black = ">= 22.3"
+black = ">= 24.3"
 colorlog = ">= 4.0"
 isort = ">= 5.10"
 mypy = ">= 0.9"
 pylint = ">= 2"
 urwid = ">= 2.0"
 
 [tool.poetry.group.test.dependencies]
@@ -35,15 +35,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.pyright]
-pythonVersion = "3.9"
+pythonVersion = "3.11"
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "format",  # Handled by black
     "abstract-method",  # With intro of async there are always methods missing
     "cyclic-import",  # Doesn't test if both import on load
     "duplicate-code",  # Unavoidable
```

### Comparing `elkm1_lib-2.2.6/PKG-INFO` & `elkm1_lib-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: elkm1-lib
-Version: 2.2.6
+Version: 2.2.7
 Summary: Library for interacting with ElkM1 alarm/automation panel.
 Home-page: https://github.com/gwww/elkm1
 License: MIT
 Author: Glenn Waters
 Author-email: gwwaters+elkm1@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: async-timeout (>=4.0,<5.0)
-Requires-Dist: pyserial-asyncio (>=0.5)
+Requires-Dist: pyserial-asyncio-fast (>=0.11)
 Description-Content-Type: text/markdown
 
 # Python ElkM1 library
 
 [![PyPI version](https://badge.fury.io/py/elkm1-lib.svg)](https://badge.fury.io/py/elkm1-lib)
 [![CI](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml/badge.svg)](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml)
 [![Downloads](https://pepy.tech/badge/elkm1-lib)](https://pepy.tech/project/elkm1-lib)
```

