# Comparing `tmp/lytils-0.1.5.tar.gz` & `tmp/lytils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytils-0.1.5.tar", max compression
+gzip compressed data, was "lytils-0.1.6.tar", max compression
```

## Comparing `lytils-0.1.5.tar` & `lytils-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.5/LICENSE
--rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.5/lytils/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.5/lytils/app.py
--rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.5/lytils/classes/__init__.py
--rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.5/lytils/classes/Regex.py
--rw-r--r--   0        0        0     1220 2024-04-29 06:18:46.279205 lytils-0.1.5/lytils/common.py
--rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.5/lytils/discord/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.5/lytils/discord/DiscordBot.py
--rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.5/lytils/email/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.5/lytils/email/Email.py
--rw-r--r--   0        0        0     1829 2024-04-30 07:52:51.978200 lytils-0.1.5/lytils/file.py
--rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.5/lytils/google_sheets/__init__.py
--rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.5/lytils/google_sheets/Column.py
--rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.5/lytils/google_sheets/format.py
--rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.5/lytils/google_sheets/GoogleSheets.py
--rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.5/lytils/google_sheets/helpers.py
--rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.5/lytils/google_sheets/Sheet.py
--rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.5/lytils/google_sheets/Tab.py
--rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.5/lytils/input.py
--rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.5/lytils/logging.py
--rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.5/lytils/print.py
--rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.5/lytils/regex.py
--rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.5/lytils/surfshark.py
--rw-r--r--   0        0        0      318 2024-04-30 07:53:05.856827 lytils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.5/README.md
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.6/LICENSE
+-rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.6/lytils/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.6/lytils/app.py
+-rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.6/lytils/classes/__init__.py
+-rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.6/lytils/classes/Regex.py
+-rw-r--r--   0        0        0     1220 2024-04-29 06:18:46.279205 lytils-0.1.6/lytils/common.py
+-rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.6/lytils/discord/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.6/lytils/discord/DiscordBot.py
+-rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.6/lytils/email/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.6/lytils/email/Email.py
+-rw-r--r--   0        0        0     1829 2024-04-30 07:52:51.978200 lytils-0.1.6/lytils/file.py
+-rw-r--r--   0        0        0      127 2024-05-01 06:20:57.735715 lytils-0.1.6/lytils/google_sheets/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.6/lytils/google_sheets/Column.py
+-rw-r--r--   0        0        0      309 2024-05-01 06:46:26.825065 lytils-0.1.6/lytils/google_sheets/exceptions.py
+-rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.6/lytils/google_sheets/format.py
+-rw-r--r--   0        0        0      794 2024-05-01 06:48:18.909689 lytils-0.1.6/lytils/google_sheets/GoogleSheets.py
+-rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.6/lytils/google_sheets/helpers.py
+-rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.6/lytils/google_sheets/Sheet.py
+-rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.6/lytils/google_sheets/Tab.py
+-rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.6/lytils/input.py
+-rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.6/lytils/logging.py
+-rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.6/lytils/print.py
+-rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.6/lytils/regex.py
+-rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.6/lytils/surfshark.py
+-rw-r--r--   0        0        0      318 2024-05-01 06:49:41.012494 lytils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.6/README.md
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.6/PKG-INFO
```

### Comparing `lytils-0.1.5/LICENSE` & `lytils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/app.py` & `lytils-0.1.6/lytils/app.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/classes/Regex.py` & `lytils-0.1.6/lytils/classes/Regex.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/common.py` & `lytils-0.1.6/lytils/common.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/discord/DiscordBot.py` & `lytils-0.1.6/lytils/discord/DiscordBot.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/email/Email.py` & `lytils-0.1.6/lytils/email/Email.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/file.py` & `lytils-0.1.6/lytils/file.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/google_sheets/Column.py` & `lytils-0.1.6/lytils/google_sheets/Column.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/google_sheets/format.py` & `lytils-0.1.6/lytils/google_sheets/format.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/google_sheets/GoogleSheets.py` & `lytils-0.1.6/lytils/google_sheets/GoogleSheets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # Third-party Libraries
-import gspread as gs
+try:
+    import gspread as gs
+except ModuleNotFoundError:
+    gs = None
 
 # Local Libraries
-from .Sheet import Sheet
+from lytils.google_sheets.exceptions import GSpreadNotInstalled
+from lytils.google_sheets.Sheet import Sheet
 
 
 # src: https://practicaldatascience.co.uk/data-science/how-to-read-google-sheets-data-in-pandas-with-gspread
 class GoogleSheets:
     # Interface with GoogleSheet API to transform data
 
     def __init__(self, service_account: str):
+        if gs is None:
+            raise GSpreadNotInstalled
+
         # Authenticate with Google Sheets
         self.__service_account = gs.service_account(filename=service_account)
 
     def get_sheet(self, url) -> Sheet:
         sheet = self.__service_account.open_by_url(url)
         return Sheet(sheet=sheet)
```

### Comparing `lytils-0.1.5/lytils/google_sheets/Tab.py` & `lytils-0.1.6/lytils/google_sheets/Tab.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/input.py` & `lytils-0.1.6/lytils/input.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/logging.py` & `lytils-0.1.6/lytils/logging.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/print.py` & `lytils-0.1.6/lytils/print.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.5/lytils/surfshark.py` & `lytils-0.1.6/lytils/surfshark.py`

 * *Files identical despite different names*

