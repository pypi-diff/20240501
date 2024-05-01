# Comparing `tmp/haunts-0.7.1.tar.gz` & `tmp/haunts-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haunts-0.7.1.tar", last modified: Sat Apr 13 12:22:48 2024, max compression
+gzip compressed data, was "haunts-0.7.2.tar", last modified: Wed May  1 10:14:32 2024, max compression
```

## Comparing `haunts-0.7.1.tar` & `haunts-0.7.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.120260 haunts-0.7.1/
--rw-r--r--   0 keul       (501) staff       (20)      154 2024-04-13 12:22:47.000000 haunts-0.7.1/AUTHORS.rst
--rw-r--r--   0 keul       (501) staff       (20)     3512 2024-04-13 12:22:47.000000 haunts-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 keul       (501) staff       (20)     1766 2024-04-13 12:22:47.000000 haunts-0.7.1/HISTORY.rst
--rw-r--r--   0 keul       (501) staff       (20)     1520 2024-04-13 12:22:47.000000 haunts-0.7.1/LICENSE
--rw-r--r--   0 keul       (501) staff       (20)      262 2024-04-13 12:22:47.000000 haunts-0.7.1/MANIFEST.in
--rw-r--r--   0 keul       (501) staff       (20)    13450 2024-04-13 12:22:48.120184 haunts-0.7.1/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)    10653 2024-04-13 12:22:47.000000 haunts-0.7.1/README.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.117748 haunts-0.7.1/docs/
--rw-r--r--   0 keul       (501) staff       (20)      607 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/Makefile
--rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/authors.rst
--rwxr-xr-x   0 keul       (501) staff       (20)     4786 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/conf.py
--rw-r--r--   0 keul       (501) staff       (20)       33 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/contributing.rst
--rw-r--r--   0 keul       (501) staff       (20)    61680 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/fear-of-the-worklog.jpg
--rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/history.rst
--rw-r--r--   0 keul       (501) staff       (20)      309 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/index.rst
--rw-r--r--   0 keul       (501) staff       (20)     1108 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/installation.rst
--rw-r--r--   0 keul       (501) staff       (20)      768 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/make.bat
--rw-r--r--   0 keul       (501) staff       (20)    88743 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/pm.gif
--rw-r--r--   0 keul       (501) staff       (20)       27 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/readme.rst
--rw-r--r--   0 keul       (501) staff       (20)       73 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/usage.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.118788 haunts-0.7.1/haunts/
--rw-r--r--   0 keul       (501) staff       (20)      226 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      155 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/actions.py
--rw-r--r--   0 keul       (501) staff       (20)     4746 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/calendars.py
--rw-r--r--   0 keul       (501) staff       (20)     4017 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/cli.py
--rw-r--r--   0 keul       (501) staff       (20)     1664 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/credentials.py
--rw-r--r--   0 keul       (501) staff       (20)     4367 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/download.py
--rw-r--r--   0 keul       (501) staff       (20)     1268 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/ini.py
--rw-r--r--   0 keul       (501) staff       (20)     6877 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/report.py
--rw-r--r--   0 keul       (501) staff       (20)    13955 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/spreadsheet.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.119990 haunts-0.7.1/haunts.egg-info/
--rw-r--r--   0 keul       (501) staff       (20)    13450 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)      726 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/SOURCES.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/dependency_links.txt
--rw-r--r--   0 keul       (501) staff       (20)       43 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/entry_points.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/not-zip-safe
--rw-r--r--   0 keul       (501) staff       (20)      140 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/requires.txt
--rw-r--r--   0 keul       (501) staff       (20)        7 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/top_level.txt
--rw-r--r--   0 keul       (501) staff       (20)      863 2024-04-13 12:22:47.000000 haunts-0.7.1/pyproject.toml
--rw-r--r--   0 keul       (501) staff       (20)      378 2024-04-13 12:22:48.120514 haunts-0.7.1/setup.cfg
--rw-r--r--   0 keul       (501) staff       (20)     1588 2024-04-13 12:22:47.000000 haunts-0.7.1/setup.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.119824 haunts-0.7.1/tests/
--rw-r--r--   0 keul       (501) staff       (20)       36 2024-04-13 12:22:47.000000 haunts-0.7.1/tests/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      819 2024-04-13 12:22:47.000000 haunts-0.7.1/tests/test_haunts.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-05-01 10:14:32.055320 haunts-0.7.2/
+-rw-r--r--   0 keul       (501) staff       (20)      154 2024-05-01 10:14:31.000000 haunts-0.7.2/AUTHORS.rst
+-rw-r--r--   0 keul       (501) staff       (20)     3512 2024-05-01 10:14:31.000000 haunts-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1974 2024-05-01 10:14:31.000000 haunts-0.7.2/HISTORY.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1520 2024-05-01 10:14:31.000000 haunts-0.7.2/LICENSE
+-rw-r--r--   0 keul       (501) staff       (20)      262 2024-05-01 10:14:31.000000 haunts-0.7.2/MANIFEST.in
+-rw-r--r--   0 keul       (501) staff       (20)    13657 2024-05-01 10:14:32.055225 haunts-0.7.2/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)    10652 2024-05-01 10:14:31.000000 haunts-0.7.2/README.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-05-01 10:14:32.052940 haunts-0.7.2/docs/
+-rw-r--r--   0 keul       (501) staff       (20)      607 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/Makefile
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/authors.rst
+-rwxr-xr-x   0 keul       (501) staff       (20)     4786 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/conf.py
+-rw-r--r--   0 keul       (501) staff       (20)       33 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/contributing.rst
+-rw-r--r--   0 keul       (501) staff       (20)    61680 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/fear-of-the-worklog.jpg
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/history.rst
+-rw-r--r--   0 keul       (501) staff       (20)      309 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/index.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1108 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/installation.rst
+-rw-r--r--   0 keul       (501) staff       (20)      768 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/make.bat
+-rw-r--r--   0 keul       (501) staff       (20)    88743 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/pm.gif
+-rw-r--r--   0 keul       (501) staff       (20)       27 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/readme.rst
+-rw-r--r--   0 keul       (501) staff       (20)       73 2024-05-01 10:14:31.000000 haunts-0.7.2/docs/usage.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-05-01 10:14:32.053897 haunts-0.7.2/haunts/
+-rw-r--r--   0 keul       (501) staff       (20)      226 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      155 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/actions.py
+-rw-r--r--   0 keul       (501) staff       (20)     4746 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/calendars.py
+-rw-r--r--   0 keul       (501) staff       (20)     4017 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/cli.py
+-rw-r--r--   0 keul       (501) staff       (20)     1664 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/credentials.py
+-rw-r--r--   0 keul       (501) staff       (20)     5587 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/download.py
+-rw-r--r--   0 keul       (501) staff       (20)     1268 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/ini.py
+-rw-r--r--   0 keul       (501) staff       (20)     6877 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/report.py
+-rw-r--r--   0 keul       (501) staff       (20)    14684 2024-05-01 10:14:31.000000 haunts-0.7.2/haunts/spreadsheet.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-05-01 10:14:32.055015 haunts-0.7.2/haunts.egg-info/
+-rw-r--r--   0 keul       (501) staff       (20)    13657 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)      726 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/SOURCES.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/dependency_links.txt
+-rw-r--r--   0 keul       (501) staff       (20)       43 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/entry_points.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/not-zip-safe
+-rw-r--r--   0 keul       (501) staff       (20)      140 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/requires.txt
+-rw-r--r--   0 keul       (501) staff       (20)        7 2024-05-01 10:14:32.000000 haunts-0.7.2/haunts.egg-info/top_level.txt
+-rw-r--r--   0 keul       (501) staff       (20)      863 2024-05-01 10:14:31.000000 haunts-0.7.2/pyproject.toml
+-rw-r--r--   0 keul       (501) staff       (20)      378 2024-05-01 10:14:32.055607 haunts-0.7.2/setup.cfg
+-rw-r--r--   0 keul       (501) staff       (20)     1588 2024-05-01 10:14:31.000000 haunts-0.7.2/setup.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-05-01 10:14:32.054859 haunts-0.7.2/tests/
+-rw-r--r--   0 keul       (501) staff       (20)       36 2024-05-01 10:14:31.000000 haunts-0.7.2/tests/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      819 2024-05-01 10:14:31.000000 haunts-0.7.2/tests/test_haunts.py
```

### Comparing `haunts-0.7.1/CONTRIBUTING.rst` & `haunts-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/HISTORY.rst` & `haunts-0.7.2/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 History
 =======
 
+0.7.2 (2024-05-01)
+------------------
+
+- Fixed a bug introduced when with using action sync
+- Read events: prevents creation of duplicates
+- Read events: now automatically read events from personal calendar
+
 0.7.1 (2024-04-13)
 ------------------
 
 - read event selection: if user is in invited list, add the event only if she/he accepted or not answered
 - read events: do not put event id (I action flag) when event cames from a linked calendar
```

### Comparing `haunts-0.7.1/LICENSE` & `haunts-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/PKG-INFO` & `haunts-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.7.1
+Version: 0.7.2
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
 Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
@@ -172,15 +172,15 @@
   If provided, the current event will start at given time. This will influence also events defined after this row
 
 **Spent**
   (number or empty)
   
   How long the event will last. Leave empty to create a full-day event.
   
-  When executiing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
+  When executing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
 
 **Project**
   (string)
   
   Project name as it's named in the *config* sheet (see below)
 
 **Activity**
@@ -360,14 +360,21 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.2 (2024-05-01)
+------------------
+
+- Fixed a bug introduced when with using action sync
+- Read events: prevents creation of duplicates
+- Read events: now automatically read events from personal calendar
+
 0.7.1 (2024-04-13)
 ------------------
 
 - read event selection: if user is in invited list, add the event only if she/he accepted or not answered
 - read events: do not put event id (I action flag) when event cames from a linked calendar
```

### Comparing `haunts-0.7.1/README.rst` & `haunts-0.7.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
   If provided, the current event will start at given time. This will influence also events defined after this row
 
 **Spent**
   (number or empty)
   
   How long the event will last. Leave empty to create a full-day event.
   
-  When executiing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
+  When executing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
 
 **Project**
   (string)
   
   Project name as it's named in the *config* sheet (see below)
 
 **Activity**
```

### Comparing `haunts-0.7.1/docs/Makefile` & `haunts-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/docs/conf.py` & `haunts-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/docs/fear-of-the-worklog.jpg` & `haunts-0.7.2/docs/fear-of-the-worklog.jpg`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/docs/installation.rst` & `haunts-0.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/docs/make.bat` & `haunts-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/docs/pm.gif` & `haunts-0.7.2/docs/pm.gif`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/calendars.py` & `haunts-0.7.2/haunts/calendars.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/cli.py` & `haunts-0.7.2/haunts/cli.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/credentials.py` & `haunts-0.7.2/haunts/credentials.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/download.py` & `haunts-0.7.2/haunts/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from googleapiclient.discovery import build
 from datetime import datetime, timedelta
 import click
+from colorama import Back, Fore, Style
 
 from .ini import get
 from .credentials import get_credentials
 from .spreadsheet import (
     append_line,
     get_calendars_names,
     get_calendars,
+    get_calendar_col_values,
 )
 from .spreadsheet import SCOPES as SPREADSHEET_SCOPES
 from .calendars import SCOPES as CALENDAR_SCOPES
 
 
 def filter_my_event(events):
     """
@@ -73,46 +75,74 @@
 
     events_service = calendar_service.events()
     sheet_service = spreadsheet_service.spreadsheets()
 
     configured_calendars = get_calendars(
         sheet_service, ignore_alias=True, use_read_col=True
     )
+    configured_calendars["???"] = get("USER_EMAIL")
     all_events = []
     # Get "my events" from all configured calendars in the selected date
     already_added_events = set()
     for calendar_id in configured_calendars.values():
         events = get_events_at(events_service, calendar_id, date_to_check)
         new_events = [
             e for e in filter_my_event(events) if e["id"] not in already_added_events
         ]
         already_added_events.update([e["id"] for e in new_events])
         all_events.extend(new_events)
 
     # Get calendar configurations
     calendar_names = get_calendars_names(sheet_service, flat=False)
+    calendar_names[get("USER_EMAIL")] = {"alias": "???", "is_linked": False}
+
+    # Get a list of all events ids already present in the sheet
+    # This to prevent adding the same event multiple times
+    all_sheet_events = get_calendar_col_values(sheet_service, sheet, "Event id")
+    all_sheet_event_urls = get_calendar_col_values(sheet_service, sheet, "Link")
 
     # Main operation loop
     for event in all_events:
         event_summary = event.get("summary", "No summary")
         start = event["start"].get("dateTime", event["start"].get("date"))
         end = event["end"].get("dateTime", event["end"].get("date"))
         project = calendar_names[event["calendar_id"]]["alias"]
         is_linked = calendar_names[event["calendar_id"]]["is_linked"]
 
         start_date = datetime.fromisoformat(start).date()
         start_time = datetime.fromisoformat(start).time()
         duration = datetime.fromisoformat(end) - datetime.fromisoformat(start)
+        event_id = event["id"] if not is_linked else ""
+        if event_id and event_id in all_sheet_events:
+            click.echo(
+                Back.YELLOW
+                + Fore.BLACK
+                + (f"Event {event_summary} already present in the sheet. Skipping…")
+                + Style.RESET_ALL
+            )
+            continue
+        event_link = event.get("htmlLink", "")
+        if event_link and event_link in all_sheet_event_urls:
+            click.echo(
+                Back.YELLOW
+                + Fore.BLACK
+                + (
+                    f"A link to event {event_summary} already present in the sheet ({event_link}). "
+                    f"Skipping…"
+                )
+                + Style.RESET_ALL
+            )
+            continue
         click.echo(f"Adding new event {event_summary} ({project}) to selected sheet")
         append_line(
             sheet_service,
             sheet,
             date_col=start_date,
             time_col=start_time,
             duration_col=duration,
             project_col=project,
             activity_col=event_summary,
             details_col=event.get("description", ""),
-            event_id_col=event["id"] if not is_linked else "",
-            link_col=event.get("htmlLink", ""),
+            event_id_col=event_id,
+            link_col=event_link,
             action_col="I" if not is_linked else "",
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `haunts-0.7.1/haunts/ini.py` & `haunts-0.7.2/haunts/ini.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/report.py` & `haunts-0.7.2/haunts/report.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/haunts/spreadsheet.py` & `haunts-0.7.2/haunts/spreadsheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,15 +242,19 @@
         .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
         .execute()
     )
     values = calendars.get("values", [])
     configured_calendars = {}
     for cols in values:
         if not use_read_col:
-            id, alias = cols
+            try:
+                id, alias = cols
+            except ValueError:
+                # not required alias column
+                id, alias, _ = cols
             read_from = None
         else:
             try:
                 id, alias, read_from = cols
             except ValueError:
                 # no linked_id
                 id, alias = cols
@@ -259,14 +263,30 @@
             id in configured_calendars or read_from in configured_calendars
         ):
             continue
         configured_calendars[alias] = read_from or id
     return configured_calendars
 
 
+def get_calendar_col_values(sheet, month, col_name):
+    """Get all events ids for a month."""
+    headers_ids = get_headers(sheet, month, indexes=True)
+    col_of_interest = headers_ids.get(col_name)
+    # transform a zero.based index to a capital letter
+    col_of_interest = string.ascii_uppercase[col_of_interest]
+    RANGE = f"{month}!{col_of_interest}2:{col_of_interest}"
+    events = (
+        sheet.values()
+        .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
+        .execute()
+    )
+    values = events.get("values", [])
+    return [e[0] for e in values if e]
+
+
 def get_calendars_names(sheet, flat=True):
     """Get all calendars names, giving precedence to alias defined in column "linked_calendar".
 
     If multiple aliases are found, the first one will be used
     """
     RANGE = f"{get('CONTROLLER_SHEET_NAME', 'config')}!A2:C"
     calendars = (
```

### Comparing `haunts-0.7.1/haunts.egg-info/PKG-INFO` & `haunts-0.7.2/haunts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.7.1
+Version: 0.7.2
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
 Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
@@ -172,15 +172,15 @@
   If provided, the current event will start at given time. This will influence also events defined after this row
 
 **Spent**
   (number or empty)
   
   How long the event will last. Leave empty to create a full-day event.
   
-  When executiing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
+  When executing the report, full day event length is influences by ``OVERTIME_FROM`` configuration option
 
 **Project**
   (string)
   
   Project name as it's named in the *config* sheet (see below)
 
 **Activity**
@@ -360,14 +360,21 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.2 (2024-05-01)
+------------------
+
+- Fixed a bug introduced when with using action sync
+- Read events: prevents creation of duplicates
+- Read events: now automatically read events from personal calendar
+
 0.7.1 (2024-04-13)
 ------------------
 
 - read event selection: if user is in invited list, add the event only if she/he accepted or not answered
 - read events: do not put event id (I action flag) when event cames from a linked calendar
```

### Comparing `haunts-0.7.1/haunts.egg-info/SOURCES.txt` & `haunts-0.7.2/haunts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/pyproject.toml` & `haunts-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haunts-0.7.1/setup.py` & `haunts-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords="google-calendar spreadsheet reports worklog",
     name="haunts",
     packages=find_packages(include=["haunts", "haunts.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/keul/haunts",
-    version="0.7.1",
+    version="0.7.2",
     zip_safe=False,
 )
```

### Comparing `haunts-0.7.1/tests/test_haunts.py` & `haunts-0.7.2/tests/test_haunts.py`

 * *Files identical despite different names*

