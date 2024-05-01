# Comparing `tmp/edgegap_logging-1.1.0.tar.gz` & `tmp/edgegap_logging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_logging-1.2.0.tar", max compression
```

## Comparing `edgegap_logging-1.1.0.tar` & `edgegap_logging-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/LICENSE
--rw-r--r--   0        0        0     2216 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/edgegap_logging/BUILD
--rw-r--r--   0        0        0      221 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      417 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/edgegap_logging/_format.py
--rw-r--r--   0        0        0     4077 2024-04-30 16:04:37.495396 edgegap_logging-1.1.0/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      494 2024-04-30 16:04:50.699508 edgegap_logging-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2216 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/BUILD
+-rw-r--r--   0        0        0      222 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     4058 2024-05-01 17:52:18.963014 edgegap_logging-1.2.0/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      644 2024-05-01 17:52:27.963235 edgegap_logging-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.2.0/PKG-INFO
```

### Comparing `edgegap_logging-1.1.0/LICENSE` & `edgegap_logging-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.1.0/README.md` & `edgegap_logging-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.1.0/edgegap_logging/_logging.py` & `edgegap_logging-1.2.0/edgegap_logging/_logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import click
 
 TRACE_LOG_LEVEL = 5
 
 
 class ColoredFormatter(logging.Formatter):
     level_name_colors = {
-        TRACE_LOG_LEVEL: lambda level_name: click.style(str(level_name), fg="blue"),
-        logging.DEBUG: lambda level_name: click.style(str(level_name), fg="cyan"),
-        logging.INFO: lambda level_name: click.style(str(level_name), fg="green"),
-        logging.WARNING: lambda level_name: click.style(str(level_name), fg="yellow"),
-        logging.ERROR: lambda level_name: click.style(str(level_name), fg="red"),
-        logging.CRITICAL: lambda level_name: click.style(str(level_name), fg="bright_red"),
+        TRACE_LOG_LEVEL: lambda level_name: click.style(str(level_name), fg='blue'),
+        logging.DEBUG: lambda level_name: click.style(str(level_name), fg='cyan'),
+        logging.INFO: lambda level_name: click.style(str(level_name), fg='green'),
+        logging.WARNING: lambda level_name: click.style(str(level_name), fg='yellow'),
+        logging.ERROR: lambda level_name: click.style(str(level_name), fg='red'),
+        logging.CRITICAL: lambda level_name: click.style(str(level_name), fg='bright_red'),
     }
-    default_fmt = "%(asctime)s | %(levelname)s | %(name)s | %(message)s"
+    default_fmt = '%(asctime)s | %(levelname)s | %(name)s | %(message)s'
 
     def __init__(
-            self,
-            fmt: str | None = default_fmt,
-            datefmt: str | None = None,
-            style: Literal["%", "{", "$"] = "%",
-            use_colors: bool | None = None,
+        self,
+        fmt: str | None = default_fmt,
+        datefmt: str | None = None,
+        style: Literal['%', '{', '$'] = '%',
+        use_colors: bool | None = None,
     ):
         if use_colors in (True, False):
             self.use_colors = use_colors
         else:
             self.use_colors = sys.stdout.isatty()
 
         super().__init__(fmt=fmt, datefmt=datefmt, style=style)
@@ -45,51 +45,51 @@
         return True  # pragma: no cover
 
     def formatMessage(self, record: logging.LogRecord) -> str:
         recordcopy = copy(record)
         levelname = recordcopy.levelname
 
         if self.use_colors:
-
             levelname = self.color_level_name(levelname, recordcopy.levelno)
 
-            if "color_message" in recordcopy.__dict__:
-                recordcopy.msg = recordcopy.__dict__["color_message"]
-                recordcopy.__dict__["message"] = recordcopy.getMessage()
+            if 'color_message' in recordcopy.__dict__:
+                recordcopy.msg = recordcopy.__dict__['color_message']
+                recordcopy.__dict__['message'] = recordcopy.getMessage()
 
-        recordcopy.__dict__["levelname"] = levelname
+        recordcopy.__dict__['levelname'] = levelname
 
         return super().formatMessage(recordcopy)
 
 
 class DefaultFormatter(ColoredFormatter):
     def should_use_colors(self) -> bool:
         return sys.stderr.isatty()  # pragma: no cover
 
 
 class AccessFormatter(ColoredFormatter):
     status_code_colours = {
-        1: lambda code: click.style(str(code), fg="bright_white"),
-        2: lambda code: click.style(str(code), fg="green"),
-        3: lambda code: click.style(str(code), fg="yellow"),
-        4: lambda code: click.style(str(code), fg="red"),
-        5: lambda code: click.style(str(code), fg="bright_red"),
+        1: lambda code: click.style(str(code), fg='bright_white'),
+        2: lambda code: click.style(str(code), fg='green'),
+        3: lambda code: click.style(str(code), fg='yellow'),
+        4: lambda code: click.style(str(code), fg='red'),
+        5: lambda code: click.style(str(code), fg='bright_red'),
     }
 
-    default_fmt = "%(asctime)s | %(levelname)s | %(name)s | %(client_addr)s - [%(request_line)s] %(status_code)s"
+    default_fmt = '%(asctime)s | %(levelname)s | %(name)s | %(client_addr)s - [%(request_line)s] %(status_code)s'
 
     def get_status_code(self, status_code: int) -> str:
         try:
             status_phrase = http.HTTPStatus(status_code).phrase
         except ValueError:
-            status_phrase = ""
+            status_phrase = ''
 
-        status_and_phrase = f"{status_code} {status_phrase}"
+        status_and_phrase = f'{status_code} {status_phrase}'
 
         if self.use_colors:
+
             def default(code: int) -> str:
                 return status_and_phrase  # pragma: no cover
 
             func = self.status_code_colours.get(status_code // 100, default)
 
             return func(status_and_phrase)
 
@@ -101,18 +101,18 @@
             client_addr,
             method,
             full_path,
             http_version,
             status_code,
         ) = recordcopy.args  # type: ignore[misc]
         status_code = self.get_status_code(int(status_code))  # type: ignore[arg-type]
-        request_line = f"{method} {full_path} HTTP/{http_version}"
+        request_line = f'{method} {full_path} HTTP/{http_version}'
         if self.use_colors:
             request_line = click.style(request_line, bold=True)
         recordcopy.__dict__.update(
             {
-                "client_addr": client_addr,
-                "request_line": request_line,
-                "status_code": status_code,
-            }
+                'client_addr': client_addr,
+                'request_line': request_line,
+                'status_code': status_code,
+            },
         )
         return super().formatMessage(recordcopy)
```

### Comparing `edgegap_logging-1.1.0/PKG-INFO` & `edgegap_logging-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

