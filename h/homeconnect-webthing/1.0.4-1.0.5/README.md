# Comparing `tmp/homeconnect_webthing-1.0.4.tar.gz` & `tmp/homeconnect_webthing-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeconnect_webthing-1.0.4.tar", last modified: Sun Jan 28 14:47:35 2024, max compression
+gzip compressed data, was "homeconnect_webthing-1.0.5.tar", last modified: Wed May  1 07:32:28 2024, max compression
```

## Comparing `homeconnect_webthing-1.0.4.tar` & `homeconnect_webthing-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:47:35.069898 homeconnect_webthing-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-28 14:47:35.069898 homeconnect_webthing-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:47:35.065898 homeconnect_webthing-1.0.4/homeconnect_webthing/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    35435 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/appliances.py
--rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/appliances_webthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/auth_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/homeconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/homeconnect_webthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:47:35.069898 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-28 14:47:35.000000 homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-28 14:47:25.000000 homeconnect_webthing-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-28 14:47:35.069898 homeconnect_webthing-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:32:28.003788 homeconnect_webthing-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 07:32:28.003788 homeconnect_webthing-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:32:28.003788 homeconnect_webthing-1.0.5/homeconnect_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35983 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/appliances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/appliances_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/auth_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/homeconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/homeconnect_webthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:32:28.003788 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 07:32:27.000000 homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 07:32:21.000000 homeconnect_webthing-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-01 07:32:28.003788 homeconnect_webthing-1.0.5/setup.cfg
```

### Comparing `homeconnect_webthing-1.0.4/LICENSE` & `homeconnect_webthing-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/PKG-INFO` & `homeconnect_webthing-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect_webthing
-Version: 1.0.4
+Version: 1.0.5
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sseclient-py>=1.7.2
```

### Comparing `homeconnect_webthing-1.0.4/README.md` & `homeconnect_webthing-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/__init__.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/app.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/app.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/appliances.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/appliances.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     def _perform_put(self, path:str, data: str, max_trials: int = 3, current_trial: int = 1, verbose: bool = False):
         uri = self._device_uri + path
         if verbose:
             logging.info("PUT " + uri + "\r\n" + json.dumps(data, indent=2))
         response = requests.put(uri, data=data, headers={"Content-Type": "application/json", "Authorization": "Bearer " + self._auth.access_token}, timeout=5000)
         if verbose:
-            logging.info(str(response.status_code) + "\r\n" + response.text)
+            logging.info("response code " + str(response.status_code) + "\r\n" + response.text)
         if not is_success(response.status_code):
             logging.warning("error occurred by calling PUT (" + str(current_trial) + ". trial) " + uri + " " + data)
             logging.warning("got " + str(response.status_code) + " " + str(response.text))
             if current_trial <= max_trials:
                 delay = 1 + current_trial
                 logging.warning("waiting " + str(delay) + " sec for retry")
                 sleep(delay)
@@ -416,28 +416,28 @@
 
     def __init__(self, start_date: str, program_duration_sec: int, remaining_secs_to_finish: int):
         self.start_date = start_date
         self.program_duration_sec = program_duration_sec
         self.remaining_secs_to_finish = remaining_secs_to_finish
 
     @staticmethod
+    def create(start_date: str, program_duration_sec: int, program_finish_in_relative_stepsize_sec: int, program_finish_in_relative_max_sec: int):
+        remaining_secs_to_finish = FinishDate.__compute_remaining_secs_to_finish(start_date, program_duration_sec, program_finish_in_relative_stepsize_sec)
+        return FinishDate(start_date, program_duration_sec, remaining_secs_to_finish)
+
+    @staticmethod
     def __compute_remaining_secs_to_finish(start_date: str, duration_sec: int, program_finish_in_relative_stepsize_sec: int) -> int:
         remaining_secs_to_finish = int((datetime.fromisoformat(start_date) - datetime.now()).total_seconds()) + duration_sec
         if remaining_secs_to_finish < 0:
             logging.info("remaining_secs_to_finish is < 0. set it with 0")
             remaining_secs_to_finish = 0
         if remaining_secs_to_finish > 0 and program_finish_in_relative_stepsize_sec > 0:
             remaining_secs_to_finish = int(remaining_secs_to_finish / program_finish_in_relative_stepsize_sec) * program_finish_in_relative_stepsize_sec
         return remaining_secs_to_finish
 
-    @staticmethod
-    def create(start_date: str, program_duration_sec: int, program_finish_in_relative_stepsize_sec: int, program_finish_in_relative_max_sec: int):
-        remaining_secs_to_finish = FinishDate.__compute_remaining_secs_to_finish(start_date, program_duration_sec, program_finish_in_relative_stepsize_sec)
-        return FinishDate(start_date, program_duration_sec, remaining_secs_to_finish)
-
     def __str__(self):
         return "remaining seconds to finished " + str(self.remaining_secs_to_finish) + " (" + print_duration(self.remaining_secs_to_finish) + "). End time " + (datetime.fromisoformat(self.start_date) + timedelta(seconds=self.program_duration_sec)).strftime("%H:%M") + " (= start time " + datetime.fromisoformat(self.start_date).strftime("%H:%M") + " + " + print_duration(self.program_duration_sec) + " program duration)"
 
     def __repr__(self):
         return self.__str__()
 
 
@@ -516,25 +516,32 @@
         # ensure that current settings and selected program is loaded
         self._reload_status_and_settings()
         self._reload_selected_program()
 
         # when startable
         if self.state == self.STATE_STARTABLE:
             program_duration_sec = self.__program_duration_sec()
+            logging.info("program duration " + print_duration(program_duration_sec))
             finish_date = FinishDate.create(start_date, program_duration_sec, self.__program_finish_in_relative_stepsize_sec, self.__program_finish_in_relative_max_sec)
+            logging.info("finish date " + str(finish_date))
             if finish_date.remaining_secs_to_finish >= self.__program_finish_in_relative_max_sec:
                 logging.warning("remaining seconds to finished " + print_duration(finish_date.remaining_secs_to_finish) + " is larger than max supported value of " + print_duration(self.__program_finish_in_relative_max_sec) + ". Ignore setting start date")
             else:
+                # bug fix FinishInRelative seems to be interpreted as start in relativ?!
+                finish_in_relative = finish_date.remaining_secs_to_finish - program_duration_sec
+                if finish_in_relative < 60:
+                    logging.info("finish_in_relative " + str(finish_in_relative) + " is < 60 sec. using finish_in_relative=60")
+                    finish_in_relative = 60
                 try:
                     data = {
                         "data": {
                             "key": self._program_selected,
                             "options": [{
                                 "key": "BSH.Common.Option.FinishInRelative",
-                                "value": finish_date.remaining_secs_to_finish,
+                                "value": finish_in_relative,
                                 "unit": "seconds"
                             }]
                         }
                     }
                     self._perform_put("/programs/active", json.dumps(data, indent=2), max_trials=3, verbose=True)
                     logging.info(self.name + " program " + self.program_selected + " starts at " + start_date + " -> " + str(finish_date))
                 except Exception as e:
```

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/appliances_webthing.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/appliances_webthing.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/auth.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/auth.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/auth_manager.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/auth_manager.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/eventstream.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/eventstream.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing/homeconnect.py` & `homeconnect_webthing-1.0.5/homeconnect_webthing/homeconnect.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/PKG-INFO` & `homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect_webthing
-Version: 1.0.4
+Version: 1.0.5
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sseclient-py>=1.7.2
```

### Comparing `homeconnect_webthing-1.0.4/homeconnect_webthing.egg-info/SOURCES.txt` & `homeconnect_webthing-1.0.5/homeconnect_webthing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

