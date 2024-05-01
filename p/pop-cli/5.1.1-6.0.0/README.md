# Comparing `tmp/pop_cli-5.1.1.tar.gz` & `tmp/pop_cli-6.0.0.tar.gz`

## Comparing `pop_cli-5.1.1.tar` & `pop_cli-6.0.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-5.1.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      906 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/__main__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/config.yaml
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/cli.py
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/completer.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/config.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/console.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/init.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-5.1.1/src/hub/state.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-5.1.1/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-5.1.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-5.1.1/README.rst
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pop_cli-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pop_cli-6.0.0/setup.py
+-rwxr-xr-x   0        0        0      906 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/hub/__main__.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/config.yaml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/cli.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/completer.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/config.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/console.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/init.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-6.0.0/src/pop_cli/plugin/state.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-6.0.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-6.0.0/README.rst
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pop_cli-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-6.0.0/PKG-INFO
```

### Comparing `pop_cli-5.1.1/.pre-commit-config.yaml` & `pop_cli-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/src/__main__.py` & `pop_cli-6.0.0/src/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/src/config.yaml` & `pop_cli-6.0.0/src/pop_cli/config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     hub_state:
       help: The location of a pickle file that has a re-usable hub object
     history_file:
       help: The location of the history file for the interactive console
 
 dyne:
   cli:
-    - hub
+    - plugin
 
 # python imports to put on the hub for this plugin
 import:
   - aioconsole
   - aioconsole.console
   - aioconsole.server
   - aiopath
```

### Comparing `pop_cli-5.1.1/src/hub/cli.py` & `pop_cli-6.0.0/src/pop_cli/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/src/hub/completer.py` & `pop_cli-6.0.0/src/pop_cli/plugin/completer.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             self._cursor_position = document._cursor_position
             self._selection = document._selection
             self._cache = document._cache
 
         def __hash__(self):
             return hash(
                 (self._text, self._cursor_position, self._selection, self._cache)
-            
+
             )
 
     class HubCompleter(hub.lib.prompt_toolkit.completion.Completer):
         def get_completions(self, document, complete_event):
             return _get_completions(HashableDocument(document))
 
     completer = HubCompleter()
```

### Comparing `pop_cli-5.1.1/src/hub/config.py` & `pop_cli-6.0.0/src/pop_cli/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/src/hub/console.py` & `pop_cli-6.0.0/src/pop_cli/plugin/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/src/hub/init.py` & `pop_cli-6.0.0/src/pop_cli/plugin/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # Try to restore the hub state
     hub_state_file = await hub.cli.state.restore(opt)
 
     call_help = False
     if (opt.cli.cli != cli) and (
         opt.cli.cli
         or (
-            (cli in hub._dynamic.config.cli_config)
+            (cli in hub._dynamic.config.cli_config or cli in hub._dynamic.config.config)
             and (cli not in opt.get("pop", {}).get("global_clis", ()))
         )
     ):
         await hub.log.debug(f"Loading cli: {cli}")
         # Reload hub.OPT with the cli arguments not consumed by the initial hub
         await hub.cli.config.override(cli, opt)
         args = []
```

### Comparing `pop_cli-5.1.1/src/hub/ref.py` & `pop_cli-6.0.0/src/pop_cli/plugin/ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,20 @@
     As a last resort just return the plain object as is.
 
     Args:
         hub (pop.hub.Hub): The global namespace
         ref (object): An object found on the hub
     """
     try:
-        if hub.lib.asyncio.iscoroutinefunction(ref) or isinstance(
-            ref, (hub.lib.typing.Callable, hub.lib.cpop.contract.Contracted)
+        if (
+            hub.lib.asyncio.iscoroutinefunction(ref)
+            or isinstance(
+                ref, hub.lib.typing.Callable | hub.lib.cpop.contract.Contracted
+            )
+            or callable(ref)
         ):
             # Call the named reference on the hub
             ret = ref(*args, **kwargs)
             # If the return was an Async Generator, then yield all the results
             if hub.lib.inspect.isasyncgen(ret):
                 ret = [_ async for _ in ret]
             # If the return was a coroutine then await it
```

### Comparing `pop_cli-5.1.1/src/hub/state.py` & `pop_cli-6.0.0/src/pop_cli/plugin/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/conftest.py` & `pop_cli-6.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_cli.py` & `pop_cli-6.0.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_config.py` & `pop_cli-6.0.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_console.py` & `pop_cli-6.0.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_init.py` & `pop_cli-6.0.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_ref.py` & `pop_cli-6.0.0/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/tests/integration/test_state.py` & `pop_cli-6.0.0/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/.gitignore` & `pop_cli-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/README.rst` & `pop_cli-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-5.1.1/pyproject.toml` & `pop_cli-6.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "setuptools"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "5.1.1"
+version = "6.0.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -34,19 +34,19 @@
     "pytest",
     "pytest-asyncio",
 ]
 
 [project.scripts]
 hub = "hub.__main__:main"
 
-[tool.hatch.build.targets.wheel.sources]
-"src" = "hub"
-
 [tool.hatch.build.targets.wheel]
-include = ["src/**"]
+packages = [
+  "src/hub",
+  "src/pop_cli",
+]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = "--tb native --full-trace --color=yes -vv"
 asyncio_mode = "auto"
```

### Comparing `pop_cli-5.1.1/PKG-INFO` & `pop_cli-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 5.1.1
+Version: 6.0.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

