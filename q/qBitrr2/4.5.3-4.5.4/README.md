# Comparing `tmp/qbitrr2-4.5.3.tar.gz` & `tmp/qbitrr2-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.5.3.tar", last modified: Wed May  1 10:50:11 2024, max compression
+gzip compressed data, was "qbitrr2-4.5.4.tar", last modified: Wed May  1 13:08:59 2024, max compression
```

## Comparing `qbitrr2-4.5.3.tar` & `qbitrr2-4.5.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:50:11.961832 qbitrr2-4.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 10:50:11.961832 qbitrr2-4.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:50:11.957832 qbitrr2-4.5.3/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226568 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:50:11.957832 qbitrr2-4.5.3/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 10:50:11.000000 qbitrr2-4.5.3/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-01 10:50:11.961832 qbitrr2-4.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:50:07.000000 qbitrr2-4.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:08:59.470295 qbitrr2-4.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 13:08:59.470295 qbitrr2-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:08:59.466294 qbitrr2-4.5.4/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226700 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26588 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:08:59.466294 qbitrr2-4.5.4/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 13:08:59.000000 qbitrr2-4.5.4/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-01 13:08:59.470295 qbitrr2-4.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:08:55.000000 qbitrr2-4.5.4/setup.py
```

### Comparing `qbitrr2-4.5.3/LICENSE` & `qbitrr2-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/PKG-INFO` & `qbitrr2-4.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.5.3
+Version: 4.5.4
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.5.3/README.md` & `qbitrr2-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/pyproject.toml` & `qbitrr2-4.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.5.3"
+version = "4.5.4"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.5.3/qBitrr/arss.py` & `qbitrr2-4.5.4/qBitrr/arss.py`

 * *Files 0% similar despite different names*

```diff
@@ -4820,14 +4820,16 @@
     def __init__(self, categories: set[str], manager: ArrManager):
         self._name = "FreeSpaceManager"
         self.categories = categories
         self.manager = manager
         self.pause = set()
         self.resume = set()
         self.expiring_bool = ExpiringSet(max_age_seconds=10)
+        self.timed_ignore_cache = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
+        self.needs_cleanup = False
         self._LOG_LEVEL = self.manager.qbit_manager.logger.level
         if ENABLE_LOGS:
             LOGS_FOLDER = HOME_PATH.joinpath("logs")
             LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
             LOGS_FOLDER.chmod(mode=0o777)
             logfile = LOGS_FOLDER.joinpath(self._name + ".log")
             if pathlib.Path(logfile).is_file():
```

### Comparing `qbitrr2-4.5.3/qBitrr/config.py` & `qbitrr2-4.5.4/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/env_config.py` & `qbitrr2-4.5.4/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/errors.py` & `qbitrr2-4.5.4/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/ffprobe.py` & `qbitrr2-4.5.4/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/gen_config.py` & `qbitrr2-4.5.4/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/home_path.py` & `qbitrr2-4.5.4/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/logger.py` & `qbitrr2-4.5.4/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/main.py` & `qbitrr2-4.5.4/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/tables.py` & `qbitrr2-4.5.4/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr/utils.py` & `qbitrr2-4.5.4/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.5.4/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.5.3
+Version: 4.5.4
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.5.3/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.5.4/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.5.3/setup.cfg` & `qbitrr2-4.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.5.3
+version = 4.5.4
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

