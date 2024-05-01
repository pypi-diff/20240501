# Comparing `tmp/weld_deps-0.6.1.tar.gz` & `tmp/weld_deps-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.6.1.tar", max compression
+gzip compressed data, was "weld_deps-0.6.2.tar", max compression
```

## Comparing `weld_deps-0.6.1.tar` & `weld_deps-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-01 14:34:25.427387 weld_deps-0.6.1/LICENSE
--rw-r--r--   0        0        0      333 2024-05-01 14:34:43.491362 weld_deps-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/__init__.py
--rw-r--r--   0        0        0     5879 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/dep.py
--rw-r--r--   0        0        0      423 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0     1859 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/main.py
--rw-r--r--   0        0        0     4855 2024-05-01 14:34:25.431387 weld_deps-0.6.1/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-01 14:36:01.293494 weld_deps-0.6.2/LICENSE
+-rw-r--r--   0        0        0      333 2024-05-01 14:36:17.853628 weld_deps-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/__init__.py
+-rw-r--r--   0        0        0     5879 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/dep.py
+-rw-r--r--   0        0        0      423 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0     1858 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/main.py
+-rw-r--r--   0        0        0     4855 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/utils.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.2/PKG-INFO
```

### Comparing `weld_deps-0.6.1/LICENSE` & `weld_deps-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.1/weld_deps/dep.py` & `weld_deps-0.6.2/weld_deps/dep.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.1/weld_deps/main.py` & `weld_deps-0.6.2/weld_deps/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 
 
 def beet_default(ctx: Context):
 
     if "weld_deps" not in ctx.meta:
         return
-    if ctx.meta["weld_deps"].get("enabled", False) == False:
+    if ctx.meta["weld_deps"].get("enabled", True) == False:
         return
 
 
     enable_weld_merging = ctx.meta["weld_deps"].get("enable_weld_merging", True)
     clean_load_tag = ctx.meta["weld_deps"].get("clean_load_tag", True)
     include_prerelease = ctx.meta["weld_deps"].get("include_prerelease", False)
     params = {
```

### Comparing `weld_deps-0.6.1/weld_deps/utils.py` & `weld_deps-0.6.2/weld_deps/utils.py`

 * *Files identical despite different names*

