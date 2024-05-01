# Comparing `tmp/stinky_noodle-0.0.8.tar.gz` & `tmp/stinky_noodle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stinky_noodle-0.0.8.tar", last modified: Fri Apr 26 20:44:08 2024, max compression
+gzip compressed data, was "stinky_noodle-0.0.9.tar", last modified: Fri Apr 26 20:54:15 2024, max compression
```

## Comparing `stinky_noodle-0.0.8.tar` & `stinky_noodle-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.833288 stinky_noodle-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:44:08.833288 stinky_noodle-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:44:08.833288 stinky_noodle-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.829288 stinky_noodle-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.829288 stinky_noodle-0.0.8/src/stinky/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.829288 stinky_noodle-0.0.8/src/stinky/noodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.833288 stinky_noodle-0.0.8/src/stinky/noodle/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/enforcer.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 20:44:04.000000 stinky_noodle-0.0.8/src/stinky/noodle/utils/ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:44:08.833288 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:44:08.000000 stinky_noodle-0.0.8/src/stinky_noodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.709714 stinky_noodle-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:54:15.709714 stinky_noodle-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:54:15.709714 stinky_noodle-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.705714 stinky_noodle-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.705714 stinky_noodle-0.0.9/src/stinky/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.705714 stinky_noodle-0.0.9/src/stinky/noodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.705714 stinky_noodle-0.0.9/src/stinky/noodle/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/enforcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 20:54:11.000000 stinky_noodle-0.0.9/src/stinky/noodle/utils/ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:54:15.709714 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:54:15.000000 stinky_noodle-0.0.9/src/stinky_noodle.egg-info/top_level.txt
```

### Comparing `stinky_noodle-0.0.8/PKG-INFO` & `stinky_noodle-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stinky-noodle
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets
 Author-email: Riccardo Tiebax <riccardo.t@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyjsonpath==1.2.3
 Provides-Extra: tests
```

### Comparing `stinky_noodle-0.0.8/README.md` & `stinky_noodle-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.8/pyproject.toml` & `stinky_noodle-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stinky-noodle"
-version = "0.0.8"
+version = "0.0.9"
 description = "Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets"
 authors = [
     { name = "Riccardo Tiebax", email = "riccardo.t@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "loguru==0.7.2",
@@ -36,15 +36,15 @@
 
 [tool.isort]
 profile = "black"
 known_third_party = ["pytest"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.8"
+version = "0.0.9"
 tag_format = "$version"
 changelog_incremental = true
 update_changelog_on_bump = true
 version_files = ["src/stinky/__init__.py:__version__", "pyproject.toml:^version"]
 bump_message = "release $current_version -> $new_version"
 
 [tool.deptry]
```

### Comparing `stinky_noodle-0.0.8/src/stinky/noodle/core.py` & `stinky_noodle-0.0.9/src/stinky/noodle/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     except Exception as exception:
         logger.error(f"Unknown issue occured trying to import {mod}: {str(exception)}")
         raise exception
 
 
 def entrypoint():
     """CLI entrypoint."""
-    parser = argparse.ArgumentParser(prog="openapi.py")
+    parser = argparse.ArgumentParser(prog="noodle")
     parser.add_argument(
         "spec_path",
         help="Path to the spec file",
         default=None,
     )
     parser.add_argument(
         "-c",
```

### Comparing `stinky_noodle-0.0.8/src/stinky/noodle/utils/builtins.py` & `stinky_noodle-0.0.9/src/stinky/noodle/utils/builtins.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.8/src/stinky/noodle/utils/enforcer.py` & `stinky_noodle-0.0.9/src/stinky/noodle/utils/enforcer.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.8/src/stinky/noodle/utils/ruleset.py` & `stinky_noodle-0.0.9/src/stinky/noodle/utils/ruleset.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.8/src/stinky_noodle.egg-info/PKG-INFO` & `stinky_noodle-0.0.9/src/stinky_noodle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stinky-noodle
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets
 Author-email: Riccardo Tiebax <riccardo.t@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyjsonpath==1.2.3
 Provides-Extra: tests
```

### Comparing `stinky_noodle-0.0.8/src/stinky_noodle.egg-info/SOURCES.txt` & `stinky_noodle-0.0.9/src/stinky_noodle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

