# Comparing `tmp/pm2-0.0.4.tar.gz` & `tmp/pm2-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm2-0.0.4.tar", last modified: Tue Apr 30 09:31:04 2024, max compression
+gzip compressed data, was "pm2-0.0.4.1.tar", last modified: Wed May  1 14:20:00 2024, max compression
```

## Comparing `pm2-0.0.4.tar` & `pm2-0.0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.151445 pm2-0.0.4/
--rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4840 2024-04-30 09:31:04.097407 pm2-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.047449 pm2-0.0.4/pm2/
--rw-rw-rw-   0        0        0    10307 2024-04-30 09:23:19.000000 pm2-0.0.4/pm2/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4/pm2/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.091451 pm2-0.0.4/pm2.egg-info/
--rw-rw-rw-   0        0        0     4840 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-30 09:28:40.000000 pm2-0.0.4/pm2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 09:31:04.152408 pm2-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:20:00.008778 pm2-0.0.4.1/
+-rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4842 2024-05-01 14:19:59.905794 pm2-0.0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 14:19:59.718485 pm2-0.0.4.1/pm2/
+-rw-rw-rw-   0        0        0    10004 2024-05-01 14:19:13.000000 pm2-0.0.4.1/pm2/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4.1/pm2/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 14:19:59.889637 pm2-0.0.4.1/pm2.egg-info/
+-rw-rw-rw-   0        0        0     4842 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-01 14:19:59.000000 pm2-0.0.4.1/pm2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 14:20:00.030134 pm2-0.0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4.1/setup.py
```

### Comparing `pm2-0.0.4/LICENSE` & `pm2-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4/PKG-INFO` & `pm2-0.0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4/README.md` & `pm2-0.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4/pm2/__init__.py` & `pm2-0.0.4.1/pm2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from typing import Any, List, Optional
 
 import aiofiles
 from aylak.rich.console import Console
 
 console = Console()
 
-__version__ = "0.0.4"
+__version__ = "0.0.4.1"
 
 
 class PathIsFolderError(Exception):
     pass
 
 
 class PM2Process:
@@ -128,30 +128,27 @@
         pid: int = None,
         pm_id: int = None,
         name: str = None,
     ) -> PM2Process:
         processes = await self.list()
         for process in processes:
             if (
-                (pid and process.pid == pid)
-                or (pm_id and process.pm_id == pm_id)
-                or (name and process.name == name)
+                (pid is not None and process.pid == pid)
+                or (pm_id is not None and process.pm_id == pm_id)
+                or (name is not None and process.name == name)
             ):
                 return process
         return None
 
     async def start(
         self, path: str, name: str = None, extra_args: List[str] = None
     ) -> Optional[PM2Process]:
         extra_args = extra_args or []
         if os.path.isdir(path):
-            if "__main__.py" in os.listdir(path):
-                path = os.path.join(path, "__main__.py")
-            else:
-                raise PathIsFolderError("Path is a folder; a file is expected.")
+            raise PathIsFolderError("Path is a folder; a file is expected.")
         cmd = (
             self.COMMAND
             + ["start", path]
             + (["--name", name] if name else [])
             + extra_args
         )
         await self.execute_command(cmd)
@@ -230,32 +227,28 @@
         pid: int = None,
         pm_id: int = None,
         name: str = None,
     ) -> PM2Process:
         processes = self.list()
         for process in processes:
             if (
-                (pid and process.pid == pid)
-                or (pm_id and process.pm_id == pm_id)
-                or (name and process.name == name)
+                (pid is not None and process.pid == pid)
+                or (pm_id is not None and process.pm_id == pm_id)
+                or (name is not None and process.name == name)
             ):
                 return process
         return None
 
     def start(
         self, path: str, name: str = None, extra_args: List[str] = None
     ) -> Optional[PM2Process]:
         extra_args = extra_args or []
         if os.path.isdir(path):
-            if "__main__.py" in os.listdir(
-                path
-            ):  # TODO: Folder initialization for languages ​​other than Python will be added
-                path = os.path.join(path, "__main__.py")
-            else:
-                raise PathIsFolderError("Path is a folder; a file is expected.")
+
+            raise PathIsFolderError("Path is a folder; a file is expected.")
         cmd = (
             self.COMMAND
             + ["start", path]
             + (["--name", name] if name else [])
             + extra_args
         )
         self.execute_command(cmd)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pm2-0.0.4/pm2.egg-info/PKG-INFO` & `pm2-0.0.4.1/pm2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4/setup.py` & `pm2-0.0.4.1/setup.py`

 * *Files identical despite different names*

