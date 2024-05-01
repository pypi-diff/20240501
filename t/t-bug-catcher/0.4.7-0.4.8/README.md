# Comparing `tmp/t_bug_catcher-0.4.7.tar.gz` & `tmp/t_bug_catcher-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-lv6u1_xl/t_bug_catcher-0.4.7.tar", last modified: Mon Apr 22 14:36:02 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-ovp05d25/t_bug_catcher-0.4.8.tar", last modified: Wed May  1 07:10:25 2024, max compression
```

## Comparing `t_bug_catcher-0.4.7.tar` & `t_bug_catcher-0.4.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    49984 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-22 14:36:02.000000 t_bug_catcher-0.4.7/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-22 14:36:02.607114 t_bug_catcher-0.4.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-22 14:35:33.000000 t_bug_catcher-0.4.7/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    50197 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4063 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.7/PKG-INFO` & `t_bug_catcher-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.7
+Version: 0.4.8
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.7/README.rst` & `t_bug_catcher-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.7/setup.py` & `t_bug_catcher-0.4.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.7",
+    version="0.4.8",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.8/t_bug_catcher/bug_catcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .bug_snag import BugSnag
 from .config import CONFIG
 from .jira import Jira
 from .stack_saver import StackSaver
 from .utils import logger
 from .utils.common import get_frames
+from .validation import PRE_RUN_VALIDATION
 
 
 class Configurator:
     """Configurer class for configuring the JiraPoster and BugSnag."""
 
     def __init__(self, jira: Jira, bugsnag: BugSnag):
         """Initializes the Configurer class."""
@@ -328,7 +329,10 @@
 configure = __bug_catcher.configure
 report_error = __bug_catcher.report_error
 attach_file_to_exception = __bug_catcher.attach_file_to_exception
 report_error_to_jira = __bug_catcher.report_error_to_jira
 report_error_to_bugsnag = __bug_catcher.report_error_to_bugsnag
 install_sys_hook = __bug_catcher.install_sys_hook
 uninstall_sys_hook = __bug_catcher.uninstall_sys_hook
+
+if CONFIG.STAGE.lower() == "delivery":
+    pre_run_validation = PRE_RUN_VALIDATION
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.8/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/config.py` & `t_bug_catcher-0.4.8/t_bug_catcher/config.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.8/t_bug_catcher/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -688,14 +688,18 @@
         """
         exc_info = f"{exc_type.__name__}: {exc_value}"
         frames = get_frames(exc_traceback)
         error_string: str = frames[-1].line
         exc_traceback_info: str = (
             f"Traceback (most recent call last):\n{''.join(traceback.format_tb(exc_traceback))}{exc_info}"
         )
+        if len(exc_traceback_info) > 30000:
+            exc_traceback_info: str = (
+                f"Traceback (most recent call last):\n{''.join(traceback.format_tb(exc_traceback)[-1])}{exc_info}"
+            )
 
         return {
             "version": 1,
             "type": "doc",
             "content": []
             + (self.__error_string_markup(error_string, exc_info) if error_string else [])
             + self.__bot_name_markup()
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.8/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.8/t_bug_catcher/stack_saver.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,36 +9,24 @@
 from types import FunctionType, ModuleType
 from typing import Optional
 
 import whispers
 
 from .config import CONFIG
 from .utils import logger
-from .utils.common import Encoder, convert_keys_to_primitives
+from .utils.common import Encoder, convert_keys_to_primitives, strip_path
 
 
 class StackSaver:
     """A class to save the stack trace."""
 
     def __init__(self):
         """Initializes the StackSaver class."""
         pass
 
-    @staticmethod
-    def strip_path(path: str):
-        """A static method to strip the current working directory path from the input.
-
-        Args:
-            path (str): The path from which to strip the current working directory path.
-
-        Returns:
-            str: The stripped path.
-        """
-        return path.replace(os.getcwd(), "").strip(os.sep)
-
     def serialize_frame_info(self, frame_info: dict) -> dict:
         """A static method to serialize the frame info.
 
         Args:
             frame_info (dict): The frame info to be serialized.
 
         Returns:
@@ -142,15 +130,15 @@
                     continue
                 frames.append(frame)
                 tb = tb.tb_next
             frames = frames[-CONFIG.LIMITS.STACK_SCOPE :]
 
             for frame in frames:
                 frame_info = {
-                    "filename": self.strip_path(frame.f_code.co_filename),
+                    "filename": strip_path(frame.f_code.co_filename),
                     "function_name": frame.f_code.co_name,
                     "line_number": frame.f_lineno,
                     "line": linecache.getline(frame.f_code.co_filename, frame.f_lineno).strip(),
                     "locals": self.filter_variables(frame.f_locals),
                     "args": self.filter_variables(inspect.getargvalues(frame)[3]),
                 }
                 stack_details_json.append(self.serialize_frame_info(frame_info))
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.4.8/t_bug_catcher/utils/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import os
 import traceback
 from datetime import date, datetime
 from json import JSONEncoder
 from pathlib import Path
 from types import TracebackType
 from typing import List
 
@@ -70,7 +71,19 @@
     new_dict = {}
     for key, value in data.items():
         if isinstance(value, dict):
             new_dict[str(key)] = convert_keys_to_primitives(value)
         else:
             new_dict[str(key)] = value
     return new_dict
+
+
+def strip_path(path: str):
+    """A function to strip the current working directory path from the input.
+
+    Args:
+        path (str): The path from which to strip the current working directory path.
+
+    Returns:
+        str: The stripped path.
+    """
+    return path.replace(os.getcwd(), "").strip(os.sep)
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.8/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.8/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.7
+Version: 0.4.8
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.7/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.8/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 t_bug_catcher/__init__.py
 t_bug_catcher/bug_catcher.py
 t_bug_catcher/bug_snag.py
 t_bug_catcher/config.py
 t_bug_catcher/exceptions.py
 t_bug_catcher/jira.py
 t_bug_catcher/stack_saver.py
+t_bug_catcher/validation.py
 t_bug_catcher/workitems.py
 t_bug_catcher.egg-info/PKG-INFO
 t_bug_catcher.egg-info/SOURCES.txt
 t_bug_catcher.egg-info/dependency_links.txt
 t_bug_catcher.egg-info/not-zip-safe
 t_bug_catcher.egg-info/requires.txt
 t_bug_catcher.egg-info/top_level.txt
```

### Comparing `t_bug_catcher-0.4.7/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.8/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

