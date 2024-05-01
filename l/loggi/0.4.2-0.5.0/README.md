# Comparing `tmp/loggi-0.4.2.tar.gz` & `tmp/loggi-0.5.0.tar.gz`

## Comparing `loggi-0.4.2.tar` & `loggi-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 loggi-0.4.2/src/loggi/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 loggi-0.4.2/src/loggi/logger.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 loggi-0.4.2/src/loggi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 loggi-0.4.2/src/loggi/py.typed
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 loggi-0.4.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 loggi-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 loggi-0.4.2/README.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 loggi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 loggi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 loggi-0.5.0/src/loggi/__init__.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 loggi-0.5.0/src/loggi/logger.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 loggi-0.5.0/src/loggi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 loggi-0.5.0/src/loggi/py.typed
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 loggi-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 loggi-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 loggi-0.5.0/README.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 loggi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 loggi-0.5.0/PKG-INFO
```

### Comparing `loggi-0.4.2/src/loggi/__init__.py` & `loggi-0.5.0/src/loggi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import logging
 
 from .logger import (
     Logger,
+    LoggerMixin,
+    LogName,
     close,
     get_log,
     get_logpath,
     get_logpaths,
     getLogger,
     load_log,
 )
 from .models import Event, Log
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 __all__ = [
     "Logger",
     "close",
     "get_log",
     "get_logpath",
     "get_logpaths",
     "getLogger",
     "load_log",
     "Event",
     "Log",
     "logging",
+    "LoggerMixin",
+    "LogName",
 ]
 
 CRITICAL = logging.CRITICAL
 FATAL = CRITICAL
 ERROR = logging.ERROR
 WARNING = logging.WARNING
 WARN = WARNING
```

### Comparing `loggi-0.4.2/src/loggi/logger.py` & `loggi-0.5.0/src/loggi/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import inspect
 import logging
+from enum import Enum
 
 from pathier import Pathier, Pathish
 
 from loggi import models
 
 root = Pathier(__file__).parent
 
@@ -84,14 +86,55 @@
 
 
 def load_log(logpath: Pathish) -> models.Log:
     """Return a `loggi.models.Log` object for the log file at `logpath`."""
     return models.Log.load_log(Pathier(logpath))
 
 
+class LogName(Enum):
+    CLASSNAME = 1
+    FILENAME = 2
+
+
+class LoggerMixin:
+    """Inherit from this class and call `self.init_logger()` in your `__init__()` function.
+
+    The logger instance can then be accessed through `self.logger`."""
+
+    def init_logger(
+        self,
+        name: str | int | LogName = LogName.CLASSNAME,
+        log_dir: Pathish = "logs",
+        log_level: int | str = "INFO",
+    ):
+        """
+        Initialize the logger instance.
+
+        #### :params:
+        * `name`: The name for the logger. The log file will be named `{name}.log`.
+        If `LogName.CLASSNAME` is given, a lowercase version of the name of the inheriting class will be used.
+        If `LogName.FILENAME` is given, a lowercase version of the file stem the inheriting class is instantiated in will be used.
+        * `log_dir`: The directory the log file will be written to.
+        * `log_level`: The level for the logger.
+        """
+        log_dir = Pathier(log_dir)
+        if name == LogName.CLASSNAME:
+            name = self.__class__.__name__.lower()
+        elif name == LogName.FILENAME:
+            source_file = inspect.getsourcefile(type(self))
+            if source_file:
+                name = Pathier(source_file).stem
+            else:
+                name = Pathier(__file__).stem
+            name = name.lower()
+        name = str(name)
+        self.logger = getLogger(name, log_dir)
+        self.logger.setLevel(log_level)
+
+
 # |===================================================|
 # Backwards compatibility with previous loggi versions
 # |===================================================|
 
 
 def get_logpaths(logger: Logger | logging.Logger) -> list[Pathier]:
     """Loop through the handlers for `logger` and return a list of paths for any handler of type `FileHandler`."""
```

### Comparing `loggi-0.4.2/src/loggi/models.py` & `loggi-0.5.0/src/loggi/models.py`

 * *Files identical despite different names*

### Comparing `loggi-0.4.2/LICENSE.txt` & `loggi-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loggi-0.4.2/pyproject.toml` & `loggi-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "loggi"
 description = "logger boilerplate with dataclass models for parsing"
-version = "0.4.2"
+version = "0.5.0"
 dependencies = ["pathier", "typing_extensions", "younotyou"]
 readme = "README.md"
 keywords = ["log", "logger", "logging"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <3.12"
 
 [[project.authors]]
```

