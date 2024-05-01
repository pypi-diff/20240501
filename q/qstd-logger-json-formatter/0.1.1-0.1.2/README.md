# Comparing `tmp/qstd_logger_json_formatter-0.1.1.tar.gz` & `tmp/qstd_logger_json_formatter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_logger_json_formatter-0.1.1.tar", last modified: Fri Apr 19 15:13:28 2024, max compression
+gzip compressed data, was "qstd_logger_json_formatter-0.1.2.tar", last modified: Wed May  1 10:10:41 2024, max compression
```

## Comparing `qstd_logger_json_formatter-0.1.1.tar` & `qstd_logger_json_formatter-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_logger_json_formatter-0.1.1/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      744 2024-03-31 10:24:13.000000 qstd_logger_json_formatter-0.1.1/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3226 2024-04-19 15:00:03.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      275 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       27 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      624 2024-04-19 15:11:57.000000 qstd_logger_json_formatter-0.1.1/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 10:10:41.255810 qstd_logger_json_formatter-0.1.2/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_logger_json_formatter-0.1.2/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-05-01 10:10:41.255810 qstd_logger_json_formatter-0.1.2/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      744 2024-03-31 10:24:13.000000 qstd_logger_json_formatter-0.1.2/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 10:10:41.255810 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3376 2024-05-01 10:04:12.000000 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 10:10:41.255810 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-05-01 10:10:41.000000 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      275 2024-05-01 10:10:41.000000 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-01 10:10:41.000000 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       27 2024-05-01 10:10:41.000000 qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-01 10:10:41.255810 qstd_logger_json_formatter-0.1.2/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      624 2024-05-01 10:07:54.000000 qstd_logger_json_formatter-0.1.2/setup.py
```

### Comparing `qstd_logger_json_formatter-0.1.1/LICENSE` & `qstd_logger_json_formatter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_logger_json_formatter-0.1.1/PKG-INFO` & `qstd_logger_json_formatter-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd_logger_json_formatter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logging json formatter
 Home-page: https://github.com/QuisEgoSum/qstd-logger-json-formatter
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: logging json formatter
 Requires-Python: >=3.7
```

### Comparing `qstd_logger_json_formatter-0.1.1/README.md` & `qstd_logger_json_formatter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/__init__.py` & `qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 
 class JsonFormatter(logging.Formatter):
     datefmt = None
     default_time_format = "%Y-%m-%dT%H:%M:%S"
     msec_format = "%s.%03dZ"
 
+    json_dumps = dict(default=str)
+
     FORMATTERS: typing.Dict[str, typing.Callable[[LogRecord], dict]] = dict()
     ROOT_FORMATTERS: typing.Dict[str, typing.Callable[[LogRecord], dict]] = dict()
     PARSE_PAYLOAD_ROOT_LOGGER: typing.Set[str] = set()
 
     def __init__(self):
         super().__init__()
 
@@ -49,14 +51,19 @@
             message=record.message,
             label=record.name,
             pname=record.processName,
             pid=record.process,
             timestamp=record.asctime
         )
 
+    @classmethod
+    def set_json_dumps(cls, **kwargs):
+        cls.json_dumps = kwargs
+        return cls
+
     def format(self, record: LogRecord) -> str:
         root_name = record.name.split('.')[0]
         if root_name in self.PARSE_PAYLOAD_ROOT_LOGGER:
             record.message = record.msg
             if not record.args:
                 record.payload = None
             elif isinstance(record.args, tuple) and len(record.args) == 1:
@@ -81,15 +88,15 @@
         if record.exc_info:
             if not record.exc_text:
                 record.exc_text = self.formatException(record.exc_info)
         if record.exc_text:
             log_dict["exc_info"] = record.exc_text
         if record.stack_info:
             log_dict["stack_info"] = self.formatStack(record.stack_info)
-        return json.dumps(log_dict, default=str)
+        return json.dumps(log_dict, **self.json_dumps)
 
 
 def configure(formatter_cls: typing.Type[JsonFormatter]):
     handler = logging.StreamHandler(stream=sys.stdout)
     handler.setFormatter(formatter_cls())
     root_logger = logging.getLogger()
     root_logger.addHandler(handler)
```

### Comparing `qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/PKG-INFO` & `qstd_logger_json_formatter-0.1.2/qstd_logger_json_formatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd-logger-json-formatter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logging json formatter
 Home-page: https://github.com/QuisEgoSum/qstd-logger-json-formatter
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: logging json formatter
 Requires-Python: >=3.7
```

### Comparing `qstd_logger_json_formatter-0.1.1/setup.py` & `qstd_logger_json_formatter-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_logger_json_formatter',
-    version='0.1.1',
+    version='0.1.2',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Logging json formatter',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-logger-json-formatter',
     packages=find_packages(exclude=['tmp', 'example']),
```

