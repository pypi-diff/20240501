# Comparing `tmp/qrawl-0.1.6.tar.gz` & `tmp/qrawl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.1.6.tar", max compression
+gzip compressed data, was "qrawl-0.1.7.tar", max compression
```

## Comparing `qrawl-0.1.6.tar` & `qrawl-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.6/LICENSE
--rw-r--r--   0        0        0      794 2024-05-01 06:29:45.830330 qrawl-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.6/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.6/qrawl/common.py
--rw-r--r--   0        0        0      352 2024-04-10 20:17:48.317729 qrawl-0.1.6/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.6/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.6/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.6/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.6/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.6/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.6/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.6/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.6/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.6/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.6/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     6682 2024-04-10 20:17:48.321751 qrawl-0.1.6/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     1769 2024-04-10 20:17:48.318749 qrawl-0.1.6/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.6/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.6/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.6/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.7/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-01 06:45:07.851742 qrawl-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.7/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.7/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.1.7/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.7/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.7/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.7/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.7/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.7/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.7/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.7/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.1.7/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.7/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.7/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     6682 2024-04-10 20:17:48.321751 qrawl-0.1.7/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     1667 2024-05-01 06:44:39.479457 qrawl-0.1.7/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    15799 2024-05-01 06:29:28.782685 qrawl-0.1.7/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.7/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.7/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.7/PKG-INFO
```

### Comparing `qrawl-0.1.6/LICENSE` & `qrawl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/pyproject.toml` & `qrawl-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.1.6/qrawl/common.py` & `qrawl-0.1.7/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/google_sheets/column.py` & `qrawl-0.1.7/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.1.7/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/playwright/async_api/common.py` & `qrawl-0.1.7/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/playwright/sync_api/common.py` & `qrawl-0.1.7/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.1.7/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.1.7/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/selenium/exceptions.py` & `qrawl-0.1.7/qrawl/selenium/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # BMP Exceptions
 class BrowsermobProxyNotInstalled(Exception):
     # Raise this when browsermob proxy path is missing
     def __init__(
         self,
-        message="<y>'browsermob-proxy' is not installed. Run 'pip install browsermob-proxy'.",
+        message="Module 'browsermob-proxy' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
 class MissingBrowsermobProxyPath(Exception):
     # Raise this when browsermob proxy path is missing
@@ -32,21 +32,21 @@
         super().__init__(self.message)
 
 
 class SeleniumWireNotInstalled(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>'seleniumwire' is not installed. Run 'pip install seleniumwire'.",
+        message="<y>Module 'seleniumwire' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
 
 
 class UndetectedChromedriverNotInstalled(Exception):
     # Raise this when undetected_chromedriver is not installed
     def __init__(
         self,
-        message="<y>'undetected_chromedriver' is not installed. Run 'pip install undetected_chromedriver'.",
+        message="<y>Module 'undetected_chromedriver' not installed.",
     ):
         self.message = ctext(message)
         super().__init__(self.message)
```

### Comparing `qrawl-0.1.6/qrawl/selenium/selenium.py` & `qrawl-0.1.7/qrawl/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.6/qrawl/xpath.py` & `qrawl-0.1.7/qrawl/xpath.py`

 * *Files identical despite different names*
