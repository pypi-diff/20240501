# Comparing `tmp/qrawl-0.1.7.tar.gz` & `tmp/qrawl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.1.7.tar", max compression
+gzip compressed data, was "qrawl-0.1.8.tar", max compression
```

## Comparing `qrawl-0.1.7.tar` & `qrawl-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.7/LICENSE
--rw-r--r--   0        0        0      794 2024-05-01 06:45:07.851742 qrawl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.7/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.7/qrawl/common.py
--rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.7/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.7/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.7/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.7/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.7/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.7/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.7/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.7/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.7/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.7/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.7/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     6682 2024-04-10 20:17:48.321751 qrawl-0.1.7/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     1667 2024-05-01 06:44:39.479457 qrawl-0.1.7/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.7/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.7/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.7/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.8/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-01 07:17:30.215877 qrawl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.8/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.8/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.8/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.8/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.8/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.8/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.8/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.8/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.8/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.8/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.8/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.8/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.8/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     6558 2024-05-01 07:17:11.664631 qrawl-0.1.8/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     1667 2024-05-01 06:44:39.479457 qrawl-0.1.8/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.8/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.8/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.8/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.8/PKG-INFO
```

### Comparing `qrawl-0.1.7/LICENSE` & `qrawl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/pyproject.toml` & `qrawl-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.1.7/qrawl/common.py` & `qrawl-0.1.8/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/google_sheets/column.py` & `qrawl-0.1.8/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.1.8/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/playwright/async_api/common.py` & `qrawl-0.1.8/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/playwright/sync_api/common.py` & `qrawl-0.1.8/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.1.8/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.1.8/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Standard Libraries
 from base64 import b64decode
 import json
 import time
 
 # Third-party Libraries
 from lytils import cprint
-from lytils.file import create_new_file, append_line
+from lytils.file import LyFile
 from lytils.regex import match
 from selenium.common.exceptions import TimeoutException
 
 # * OPTIONAL IMPORTS
 try:
     from browsermobproxy import Server
 except ModuleNotFoundError:
@@ -117,30 +117,30 @@
         poll_interval: int = 1,
         timeout: int = 10,
         debug: bool = False,
     ):
         """
         Either returns a response or raises a timeout exception.
         """
-        debug_path = "debug/BMP/wait_for_response.txt"
+        debug_file = LyFile("debug/BMP/wait_for_response.txt")
         if debug:
-            create_new_file(debug_path)
+            debug_file.create()
 
         start_time = time.time()  # Record start time for timeout
 
         while time.time() - start_time < timeout:
 
             for entry in self._client.har["log"]["entries"]:
 
                 if partial_request_url in json.dumps(entry["request"]["url"]):
 
                     if debug:
                         # Print request url and response
-                        append_line(debug_path, entry["request"]["url"])
-                        append_line(debug_path, json.dumps(entry["response"], indent=4))
+                        debug_file.append(entry["request"]["url"])
+                        debug_file.append_json(entry["response"])
 
                     content = entry["response"]["content"]
 
                     try:
                         # No decoding necessary
                         return self._get_response_from_content(content, debug=True)
 
@@ -151,52 +151,50 @@
             # ping requests against after interval has passed
             time.sleep(poll_interval)
 
         # If code reaches outside of loop, it is because of timeout.
 
         if debug:
             duration = time.time() - start_time
-            append_line(
-                debug_path, f"Timed out. Duration: {round(duration, 3)} seconds."
-            )
+            debug_file.append(f"Timed out. Duration: {round(duration, 3)} seconds.")
 
         raise TimeoutException
 
     # Troubleshoot request urls
     def get_request_urls(self):
         request_urls = []
         for entry in self._client.har["log"]["entries"]:
             request_urls.append(entry["request"]["url"])
         return request_urls
 
     def get_responses(self, partial_request_url: str, debug: bool = False):
-        debug_path = "debug/BMP/get_responses.txt"
+        debug_file = LyFile("debug/BMP/get_responses.txt")
         if debug:
-            create_new_file(debug_path)
+            debug_file.create()
 
         responses = []
         for entry in self._client.har["log"]["entries"]:
 
             if partial_request_url in entry["request"]["url"]:
 
                 if debug:
                     # Print request url and response
-                    append_line(debug_path, entry["request"]["url"])
-                    append_line(debug_path, json.dumps(entry["response"], indent=4))
+                    debug_file.append(entry["request"]["url"])
+                    debug_file.append_json(entry["response"])
 
                 content = entry["response"]["content"]
 
                 try:
                     response = self._get_response_from_content(content, debug=False)
                     responses.append(response)
 
                 except KeyError:
                     continue
 
         if debug and len(responses) == 0:
-            append_line(debug_path, f"url '{partial_request_url}' not found.")
+            debug_file.append(f"url '{partial_request_url}' not found.")
 
         return responses
 
     def close(self):
         self._client.close()
         self._server.stop()
```

### Comparing `qrawl-0.1.7/qrawl/selenium/exceptions.py` & `qrawl-0.1.8/qrawl/selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/selenium/selenium.py` & `qrawl-0.1.8/qrawl/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.7/qrawl/xpath.py` & `qrawl-0.1.8/qrawl/xpath.py`

 * *Files identical despite different names*

