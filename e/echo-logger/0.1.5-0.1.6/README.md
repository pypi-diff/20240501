# Comparing `tmp/echo_logger-0.1.5.tar.gz` & `tmp/echo_logger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_logger-0.1.5.tar", last modified: Mon Mar 11 05:39:22 2024, max compression
+gzip compressed data, was "echo_logger-0.1.6.tar", last modified: Wed May  1 14:55:21 2024, max compression
```

## Comparing `echo_logger-0.1.5.tar` & `echo_logger-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 05:39:22.840267 echo_logger-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1989 2024-03-11 05:39:22.838218 echo_logger-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-05-29 07:57:45.000000 echo_logger-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 05:39:22.826727 echo_logger-0.1.5/echo_logger/
--rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.1.5/echo_logger/__init__.py
--rw-rw-rw-   0        0        0    14414 2024-03-11 05:38:39.000000 echo_logger-0.1.5/echo_logger/echo_logger.py
-drwxrwxrwx   0        0        0        0 2024-03-11 05:39:22.837218 echo_logger-0.1.5/echo_logger.egg-info/
--rw-rw-rw-   0        0        0     1989 2024-03-11 05:39:22.000000 echo_logger-0.1.5/echo_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-03-11 05:39:22.000000 echo_logger-0.1.5/echo_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 05:39:22.000000 echo_logger-0.1.5/echo_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-11 05:39:22.000000 echo_logger-0.1.5/echo_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 05:39:22.840267 echo_logger-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-03-11 05:39:05.000000 echo_logger-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 05:39:22.836218 echo_logger-0.1.5/test/
--rw-rw-rw-   0        0        0      116 2024-01-20 14:01:16.000000 echo_logger-0.1.5/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:55:21.611544 echo_logger-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 05:16:22.000000 echo_logger-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2037 2024-05-01 14:55:21.610544 echo_logger-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-05-29 07:57:45.000000 echo_logger-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 14:55:21.601693 echo_logger-0.1.6/echo_logger/
+-rw-rw-rw-   0        0        0       90 2023-04-28 05:21:08.000000 echo_logger-0.1.6/echo_logger/__init__.py
+-rw-rw-rw-   0        0        0    14671 2024-05-01 14:53:24.000000 echo_logger-0.1.6/echo_logger/echo_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:55:21.609544 echo_logger-0.1.6/echo_logger.egg-info/
+-rw-rw-rw-   0        0        0     2037 2024-05-01 14:55:21.000000 echo_logger-0.1.6/echo_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-01 14:55:21.000000 echo_logger-0.1.6/echo_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:55:21.000000 echo_logger-0.1.6/echo_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-01 14:55:21.000000 echo_logger-0.1.6/echo_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 14:55:21.000000 echo_logger-0.1.6/echo_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:55:21.611544 echo_logger-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-01 14:54:46.000000 echo_logger-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:55:21.608553 echo_logger-0.1.6/test/
+-rw-rw-rw-   0        0        0      133 2024-05-01 14:44:33.000000 echo_logger-0.1.6/test/test.py
```

### Comparing `echo_logger-0.1.5/LICENSE` & `echo_logger-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_logger-0.1.5/PKG-INFO` & `echo_logger-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: echo_logger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple logger for python, with color and time
 Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: loguru
 
 # Echo Logger
 
 pip repo is [here](https://pypi.org/project/echo-logger/).
 
 This is a simple echo logger for informative, warning and error messages.
```

### Comparing `echo_logger-0.1.5/README.md` & `echo_logger-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `echo_logger-0.1.5/echo_logger/echo_logger.py` & `echo_logger-0.1.6/echo_logger/echo_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #!/usr/bin/env python
 import functools
+import io
 import json
 import os
 import socket
 import time
 import warnings
 from pathlib import Path
 from typing import Callable, Any, Dict, Union
 
 import requests
+from loguru import logger
 
 # noinspection DuplicatedCode
 echo_logger_debug = True
+log_sink = io.StringIO()
+logger.add(log_sink, format="{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}", level="ERROR")
 
 
 # noinspection PyPep8Naming
 class _colors:
     def __init__(self):
         pass
 
@@ -372,15 +376,17 @@
             real_title_, real_content_ = None, None
             try:
                 result = func(*args, **kwargs)
                 real_title_ = f"Python Function {func.__name__}() Executed Successfully" if title_ok is None else title_ok
                 real_content_ = f"args: {args}\nkwargs: {kwargs}" if content_ok is None else content_ok
                 return result
             except Exception as e:
-                e_str = str(e)
+                # loguru print full traceback
+                logger.exception(e)
+                e_str = log_sink.getvalue()
                 real_title_ = f"Failed to Execute Python Function {func.__name__}()" if title_err is None else title_err
                 real_content_ = f"args: {args}\nkwargs: {kwargs}\nError: {e_str}" if content_err is None else content_err
             finally:
                 time_end = time.time()
                 time_str = calc_time(time_start, time_end)
                 # Your function has been executed successfully in xx:xx:xx.xx
                 msg = FeiShuMessage(real_title_, real_content_)
```

### Comparing `echo_logger-0.1.5/echo_logger.egg-info/PKG-INFO` & `echo_logger-0.1.6/echo_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: echo_logger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple logger for python, with color and time
 Home-page: https://github.com/void-echo/echo_logger/
 Author: Echo Void
 Author-email: void-echo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: loguru
 
 # Echo Logger
 
 pip repo is [here](https://pypi.org/project/echo-logger/).
 
 This is a simple echo logger for informative, warning and error messages.
```

### Comparing `echo_logger-0.1.5/setup.py` & `echo_logger-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="echo_logger",
-    version="0.1.5",
+    version="0.1.6",
     author="Echo Void",
     author_email="void-echo@outlook.com",
     description="A simple logger for python, with color and time",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/void-echo/echo_logger/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        ],
+    ],
+    install_requires=[
+        'requests',
+        'loguru',
+
+    ]
 )
```

