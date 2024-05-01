# Comparing `tmp/signal_export-2.3.0.tar.gz` & `tmp/signal_export-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_export-2.3.0.tar", last modified: Sat Apr 27 16:27:44 2024, max compression
+gzip compressed data, was "signal_export-2.3.1.tar", last modified: Wed May  1 07:52:25 2024, max compression
```

## Comparing `signal_export-2.3.0.tar` & `signal_export-2.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1170 2024-04-27 16:27:41.496862 signal_export-2.3.0/LICENSE
--rw-r--r--   0        0        0     6921 2024-04-27 16:27:41.496862 signal_export-2.3.0/README.md
--rw-r--r--   0        0        0     2006 2024-04-27 16:27:44.832870 signal_export-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-27 16:27:41.496862 signal_export-2.3.0/sigexport/__init__.py
--rw-r--r--   0        0        0       69 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/__main__.py
--rw-r--r--   0        0        0     3157 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/create.py
--rw-r--r--   0        0        0     2956 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/data.py
--rw-r--r--   0        0        0     3209 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/files.py
--rw-r--r--   0        0        0     3451 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/html.py
--rw-r--r--   0        0        0      144 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/logging.py
--rwxr-xr-x   0        0        0     8356 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/main.py
--rw-r--r--   0        0        0     2722 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/merge.py
--rw-r--r--   0        0        0     4310 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/models.py
--rw-r--r--   0        0        0     1846 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/style.css
--rw-r--r--   0        0        0     1271 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/templates.py
--rw-r--r--   0        0        0     2467 2024-04-27 16:27:41.500862 signal_export-2.3.0/sigexport/utils.py
--rw-r--r--   0        0        0     2546 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/attachments.noindex/image.jpeg
--rw-r--r--   0        0        0    17641 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/attachments.noindex/voicenote.m4a
--rw-r--r--   0        0        0       22 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/config.json
--rw-r--r--   0        0        0    16384 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/data/sql/db.sqlite
--rw-r--r--   0        0        0     5125 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/test_integration.py
--rw-r--r--   0        0        0       86 2024-04-27 16:27:41.500862 signal_export-2.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1170 2024-05-01 07:52:22.194915 signal_export-2.3.1/LICENSE
+-rw-r--r--   0        0        0     6921 2024-05-01 07:52:22.194915 signal_export-2.3.1/README.md
+-rw-r--r--   0        0        0     2006 2024-05-01 07:52:25.314926 signal_export-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/__init__.py
+-rw-r--r--   0        0        0       69 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/__main__.py
+-rw-r--r--   0        0        0     3173 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/create.py
+-rw-r--r--   0        0        0     2956 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/data.py
+-rw-r--r--   0        0        0     3209 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/files.py
+-rw-r--r--   0        0        0     3451 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/html.py
+-rw-r--r--   0        0        0      144 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/logging.py
+-rwxr-xr-x   0        0        0     8356 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/main.py
+-rw-r--r--   0        0        0     2722 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/merge.py
+-rw-r--r--   0        0        0     4310 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/models.py
+-rw-r--r--   0        0        0     1846 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/style.css
+-rw-r--r--   0        0        0     1271 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/templates.py
+-rw-r--r--   0        0        0     2467 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/utils.py
+-rw-r--r--   0        0        0     2546 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/attachments.noindex/image.jpeg
+-rw-r--r--   0        0        0    17641 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/attachments.noindex/voicenote.m4a
+-rw-r--r--   0        0        0       22 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/config.json
+-rw-r--r--   0        0        0    16384 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/sql/db.sqlite
+-rw-r--r--   0        0        0     5125 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/test_integration.py
+-rw-r--r--   0        0        0       86 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.1/PKG-INFO
```

### Comparing `signal_export-2.3.0/LICENSE` & `signal_export-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/README.md` & `signal_export-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/pyproject.toml` & `signal_export-2.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.11",
     "emoji ~= 2.0",
     "Markdown ~= 3.4",
     "typer[all] ~= 0.7",
 ]
-version = "2.3.0"
+version = "2.3.1"
 
 [project.license]
 text = "MIT License"
 
 [project.optional-dependencies]
 sql = [
     "pysqlcipher3 == 1.1.0; python_version <  \"3.11\"",
```

### Comparing `signal_export-2.3.0/sigexport/create.py` & `signal_export-2.3.1/sigexport/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     quote = ""
     if msg.quote:
         try:
             quote = msg.quote["text"].rstrip("\n")
             quote = quote.replace("\n", "\n> ")
             quote = f"\n\n> {quote}\n\n"
-        except (KeyError, TypeError):
+        except (AttributeError, KeyError, TypeError):
             pass
 
     return models.Message(
         date=date,
         sender=sender,
         body=body,
         quote=quote,
```

### Comparing `signal_export-2.3.0/sigexport/data.py` & `signal_export-2.3.1/sigexport/data.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/files.py` & `signal_export-2.3.1/sigexport/files.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/html.py` & `signal_export-2.3.1/sigexport/html.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/main.py` & `signal_export-2.3.1/sigexport/main.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/merge.py` & `signal_export-2.3.1/sigexport/merge.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/models.py` & `signal_export-2.3.1/sigexport/models.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/style.css` & `signal_export-2.3.1/sigexport/style.css`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/templates.py` & `signal_export-2.3.1/sigexport/templates.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/sigexport/utils.py` & `signal_export-2.3.1/sigexport/utils.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/tests/data/attachments.noindex/image.jpeg` & `signal_export-2.3.1/tests/data/attachments.noindex/image.jpeg`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/tests/data/attachments.noindex/voicenote.m4a` & `signal_export-2.3.1/tests/data/attachments.noindex/voicenote.m4a`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/tests/data/sql/db.sqlite` & `signal_export-2.3.1/tests/data/sql/db.sqlite`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/tests/test_integration.py` & `signal_export-2.3.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.0/PKG-INFO` & `signal_export-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-export
-Version: 2.3.0
+Version: 2.3.1
 Summary: Export Signal conversations to Markdown and HTML
 Keywords: backup,chat,export
 Home-page: https://github.com/carderne/signal-export
 Author-Email: Chris Arderne <chris@rdrn.me>
 License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

