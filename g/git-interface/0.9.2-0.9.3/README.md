# Comparing `tmp/git-interface-0.9.2.tar.gz` & `tmp/git-interface-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-interface-0.9.2.tar", last modified: Mon Sep  5 20:42:28 2022, max compression
+gzip compressed data, was "git-interface-0.9.3.tar", last modified: Mon Nov 14 23:22:56 2022, max compression
```

## Comparing `git-interface-0.9.2.tar` & `git-interface-0.9.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 20:42:28.684141 git-interface-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-05 20:42:17.000000 git-interface-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-09-05 20:42:28.684141 git-interface-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-09-05 20:42:17.000000 git-interface-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 20:42:28.680141 git-interface-0.9.2/git_interface/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/cat_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/ls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/pack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/rev_list.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/show.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 20:42:28.684141 git-interface-0.9.2/git_interface/smart_http/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/smart_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/smart_http/quart.py
--rw-r--r--   0 runner    (1001) docker     (121)     5611 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/smart_http/ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/symbolic_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2022-09-05 20:42:17.000000 git-interface-0.9.2/git_interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 20:42:28.684141 git-interface-0.9.2/git_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-09-05 20:42:28.000000 git-interface-0.9.2/git_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-05 20:42:28.000000 git-interface-0.9.2/git_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 20:42:28.000000 git-interface-0.9.2/git_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 20:42:28.000000 git-interface-0.9.2/git_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-05 20:42:28.000000 git-interface-0.9.2/git_interface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-05 20:42:17.000000 git-interface-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-09-05 20:42:28.684141 git-interface-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-05 20:42:17.000000 git-interface-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 23:22:56.869589 git-interface-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-14 23:22:44.000000 git-interface-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-11-14 23:22:56.869589 git-interface-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-14 23:22:44.000000 git-interface-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 23:22:56.865589 git-interface-0.9.3/git_interface/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/cat_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/ls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/pack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/rev_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/shared.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/show.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 23:22:56.869589 git-interface-0.9.3/git_interface/smart_http/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/smart_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/smart_http/quart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5611 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/smart_http/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/symbolic_ref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5409 2022-11-14 23:22:44.000000 git-interface-0.9.3/git_interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 23:22:56.865589 git-interface-0.9.3/git_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-11-14 23:22:56.000000 git-interface-0.9.3/git_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-11-14 23:22:56.000000 git-interface-0.9.3/git_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 23:22:56.000000 git-interface-0.9.3/git_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-14 23:22:56.000000 git-interface-0.9.3/git_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-14 23:22:56.000000 git-interface-0.9.3/git_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-14 23:22:44.000000 git-interface-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-11-14 23:22:56.869589 git-interface-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-14 23:22:44.000000 git-interface-0.9.3/setup.py
```

### Comparing `git-interface-0.9.2/LICENSE` & `git-interface-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/PKG-INFO` & `git-interface-0.9.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: git-interface
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use the git cli from Python
 Home-page: https://github.com/enchant97/python-git-interface
 Author: Leo Spratt
 Author-email: "contact@enchantedcode.co.uk"
 License: MIT
 Project-URL: Change Log, https://github.com/enchant97/python-git-interface/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://python-git-interface.readthedocs.io/en/latest/
+Project-URL: Documentation, https://python-git-interface.readthedocs.io/en/stable/
 Keywords: git scm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
```

### Comparing `git-interface-0.9.2/README.md` & `git-interface-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/archive.py` & `git-interface-0.9.3/git_interface/archive.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/branch.py` & `git-interface-0.9.3/git_interface/branch.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/cat_file.py` & `git-interface-0.9.3/git_interface/cat_file.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/constants.py` & `git-interface-0.9.3/git_interface/constants.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/datatypes.py` & `git-interface-0.9.3/git_interface/datatypes.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/exceptions.py` & `git-interface-0.9.3/git_interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/helpers.py` & `git-interface-0.9.3/git_interface/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from subprocess import CompletedProcess
 from typing import Any, Union
 
 from .constants import DEFAULT_BUFFER_SIZE
 from .exceptions import BufferedProcessError
 
 __all__ = [
-    "ensure_path", "subprocess_run",
-    "subprocess_run_buffered",
+    "ensure_path", "chunk_yielder",
+    "subprocess_run", "subprocess_run_buffered",
 ]
 
 
 def ensure_path(path_or_str: Union[Path, str]) -> Path:
     """
     Ensures that given value is a pathlib.Path object.
```

### Comparing `git-interface-0.9.2/git_interface/log.py` & `git-interface-0.9.3/git_interface/log.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/ls.py` & `git-interface-0.9.3/git_interface/ls.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/pack.py` & `git-interface-0.9.3/git_interface/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .exceptions import BufferedProcessError
 from .helpers import chunk_yielder
 from .shared import logger
 
 __all__ = [
     "UPLOAD_PACK_TYPE", "RECEIVE_PACK_TYPE",
     "ALLOWED_PACK_TYPES", "exchange_pack",
-    "advertise_pack",
+    "advertise_pack", "ssh_pack_exchange",
 ]
 
 
 def _create_advertisement(pack_type) -> bytes:
     """
     Service type prefixed with the total line length
     """
```

### Comparing `git-interface-0.9.2/git_interface/rev_list.py` & `git-interface-0.9.3/git_interface/rev_list.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/show.py` & `git-interface-0.9.3/git_interface/show.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/smart_http/quart.py` & `git-interface-0.9.3/git_interface/smart_http/quart.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/smart_http/ssh.py` & `git-interface-0.9.3/git_interface/smart_http/ssh.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/symbolic_ref.py` & `git-interface-0.9.3/git_interface/symbolic_ref.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/tag.py` & `git-interface-0.9.3/git_interface/tag.py`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/git_interface/utils.py` & `git-interface-0.9.3/git_interface/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .exceptions import AlreadyExistsException, GitException
 from .helpers import ensure_path, subprocess_run
 
 __all__ = [
     "get_version", "init_repo",
     "clone_repo", "get_description",
     "set_description", "run_maintenance",
+    "add_to_staged", "commit_staged",
 ]
 
 
 async def get_version() -> Coroutine[Any, Any, str]:
     """
     Gets the git version
```

### Comparing `git-interface-0.9.2/git_interface.egg-info/PKG-INFO` & `git-interface-0.9.3/git_interface.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: git-interface
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use the git cli from Python
 Home-page: https://github.com/enchant97/python-git-interface
 Author: Leo Spratt
 Author-email: "contact@enchantedcode.co.uk"
 License: MIT
 Project-URL: Change Log, https://github.com/enchant97/python-git-interface/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://python-git-interface.readthedocs.io/en/latest/
+Project-URL: Documentation, https://python-git-interface.readthedocs.io/en/stable/
 Keywords: git scm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
```

### Comparing `git-interface-0.9.2/git_interface.egg-info/SOURCES.txt` & `git-interface-0.9.3/git_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-interface-0.9.2/setup.cfg` & `git-interface-0.9.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 author_email = "contact@enchantedcode.co.uk"
 description = Use the git cli from Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/enchant97/python-git-interface
 project_urls = 
 	Change Log = https://github.com/enchant97/python-git-interface/blob/main/CHANGELOG.md
-	Documentation = https://python-git-interface.readthedocs.io/en/latest/
+	Documentation = https://python-git-interface.readthedocs.io/en/stable/
 license = MIT
 keywords = git scm
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
```

