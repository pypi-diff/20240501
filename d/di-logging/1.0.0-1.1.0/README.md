# Comparing `tmp/di_logging-1.0.0.tar.gz` & `tmp/di_logging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "di_logging-1.0.0.tar", max compression
+gzip compressed data, was "di_logging-1.1.0.tar", max compression
```

## Comparing `di_logging-1.0.0.tar` & `di_logging-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-02-08 17:41:28.539949 di_logging-1.0.0/LICENSE
--rw-r--r--   0        0        0     2419 2024-02-08 17:41:28.539949 di_logging-1.0.0/README.md
--rw-r--r--   0        0        0     2754 2024-02-08 17:41:28.539949 di_logging-1.0.0/di_logging/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 17:41:28.539949 di_logging-1.0.0/di_logging/py.typed
--rw-r--r--   0        0        0     2744 2024-02-08 17:41:38.096048 di_logging-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       94 2024-02-08 17:41:28.539949 di_logging-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      486 2024-02-08 17:41:28.539949 di_logging-1.0.0/tests/test_logging.py
--rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 di_logging-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-01 15:53:43.887674 di_logging-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2419 2024-05-01 15:53:43.887674 di_logging-1.1.0/README.md
+-rw-r--r--   0        0        0     3163 2024-05-01 15:53:43.887674 di_logging-1.1.0/di_logging/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:53:43.887674 di_logging-1.1.0/di_logging/py.typed
+-rw-r--r--   0        0        0     2744 2024-05-01 15:53:52.559857 di_logging-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-05-01 15:53:43.891674 di_logging-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      486 2024-05-01 15:53:43.891674 di_logging-1.1.0/tests/test_logging.py
+-rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 di_logging-1.1.0/PKG-INFO
```

### Comparing `di_logging-1.0.0/LICENSE` & `di_logging-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `di_logging-1.0.0/README.md` & `di_logging-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `di_logging-1.0.0/di_logging/__init__.py` & `di_logging-1.1.0/di_logging/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,38 +66,49 @@
 
 def configure_logging(file_path: Optional[str] = None):
     """
     Configure the logging for a system/application.
 
     This method needs to be called in the entry point of an application.
     It will configure the loguru logger and also intercept python logging and redirect
-    it to the loguru logger.
+    it to the loguru logger. It serialises logs in the production
+    environment.
 
     Usage:
     main.py
         from di_logging import configure_logging
 
         if __name__ == "__main__":
             configure_logging()
             run_my_awesome_app()
     """
     level = os.environ.get("LOG_LEVEL", "DEBUG")
+    environment = os.environ.get("ENVIRONMENT", "development")
     logger.remove()
-    logger.add(
-        sys.stdout,
-        enqueue=True,
-        backtrace=True,
-        level=level.upper(),
-        format=LOGGER_FORMAT,
-    )
-    if file_path:
+    if environment == "development":
         logger.add(
-            file_path,
-            rotation="500 MB",
-            compression="zip",
-            level=level.upper(),
+            sys.stdout,
+            enqueue=True,
             backtrace=True,
+            level=level.upper(),
             format=LOGGER_FORMAT,
         )
+        if file_path is not None:
+            logger.add(
+                file_path,
+                rotation="500 MB",
+                compression="zip",
+                level=level.upper(),
+                backtrace=True,
+                format=LOGGER_FORMAT,
+            )
+    else:
+        logger.add(
+            sys.stdout,
+            enqueue=True,
+            backtrace=True,
+            level=level.upper(),
+            serialize=True,
+        )
 
     # add an intercept handler to the standard python logging so we get all logs to our logger
     logging.basicConfig(handlers=[_InterceptHandler()], level=0)
```

### Comparing `di_logging-1.0.0/pyproject.toml` & `di_logging-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "di-logging"
-version = "1.0.0"
+version = "1.1.0"
 description = "Standard logging library for product"
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://deeperinsights.com"
 repository = "https://github.com/skimit/di-logging"
 include = [
```

### Comparing `di_logging-1.0.0/PKG-INFO` & `di_logging-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: di-logging
-Version: 1.0.0
+Version: 1.1.0
 Summary: Standard logging library for product
 Home-page: https://deeperinsights.com
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

