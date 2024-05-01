# Comparing `tmp/bec_ipython_client-2.7.3.tar.gz` & `tmp/bec_ipython_client-2.9.3.tar.gz`

## Comparing `bec_ipython_client-2.7.3.tar` & `bec_ipython_client-2.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/demo.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/scan_progress.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/client_tests/test_scan_progress.py
--rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/.gitignore
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/pyproject.toml
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_ipython_client-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/demo.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/scan_progress.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/client_tests/test_scan_progress.py
+-rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/.gitignore
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/pyproject.toml
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_ipython_client-2.9.3/PKG-INFO
```

### Comparing `bec_ipython_client-2.7.3/demo.py` & `bec_ipython_client-2.9.3/demo.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/beamline_mixin.py` & `bec_ipython_client-2.9.3/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/bec_magics.py` & `bec_ipython_client-2.9.3/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/bec_startup.py` & `bec_ipython_client-2.9.3/bec_ipython_client/bec_startup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 logger = _bec_logger.logger
 
 bec = _BECIPythonClient(
     _main_dict["config"], _RedisConnector, wait_for_server=_main_dict["wait_for_server"]
 )
 _main_dict["bec"] = bec
 
-if not _main_dict["args"].nogui and _BECFigure is not None:
-    fig = bec.fig = _BECFigure()
-    fig.show()
-
 try:
     bec.start()
 except Exception:
     sys.excepthook(*sys.exc_info())
 else:
 
     dev = bec.device_manager.devices
     scans = bec.scans
 
+    if not _main_dict["args"].nogui and _BECFigure is not None:
+        fig = bec.fig = _BECFigure()
+        fig.show()
+
     _available_plugins = plugin_helper.get_ipython_client_startup_plugins(state="post")
     if _available_plugins:
         for name, plugin in _available_plugins.items():
             logger.success(f"Loading plugin: {plugin['source']}")
             base = os.path.dirname(plugin["module"].__file__)
             with open(os.path.join(base, "post_startup.py"), "r", encoding="utf-8") as file:
                 # pylint: disable=exec-used
```

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/main.py` & `bec_ipython_client-2.9.3/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/prettytable.py` & `bec_ipython_client-2.9.3/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/progressbar.py` & `bec_ipython_client-2.9.3/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/signals.py` & `bec_ipython_client-2.9.3/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-2.9.3/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/callbacks/live_table.py` & `bec_ipython_client-2.9.3/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/callbacks/move_device.py` & `bec_ipython_client-2.9.3/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/callbacks/scan_progress.py` & `bec_ipython_client-2.9.3/bec_ipython_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/callbacks/utils.py` & `bec_ipython_client-2.9.3/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/high_level_interfaces/bec_hli.py` & `bec_ipython_client-2.9.3/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/high_level_interfaces/spec_hli.py` & `bec_ipython_client-2.9.3/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/plugins/SLS/sls_info.py` & `bec_ipython_client-2.9.3/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-2.9.3/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `bec_ipython_client-2.9.3/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_beamline_mixins.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_bec_client.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_ipython_live_updates.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_live_table.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_move_callback.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/client_tests/test_scan_progress.py` & `bec_ipython_client-2.9.3/tests/client_tests/test_scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/end-2-end/test_scans_e2e.py` & `bec_ipython_client-2.9.3/tests/end-2-end/test_scans_e2e.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/tests/end-2-end/test_scans_lib_e2e.py` & `bec_ipython_client-2.9.3/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/.gitignore` & `bec_ipython_client-2.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.7.3/pyproject.toml` & `bec_ipython_client-2.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.7.3"
+version = "2.9.3"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_ipython_client-2.7.3/PKG-INFO` & `bec_ipython_client-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec_ipython_client
-Version: 2.7.3
+Version: 2.9.3
 Summary: BEC IPython client
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

