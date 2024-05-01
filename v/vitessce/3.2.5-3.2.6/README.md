# Comparing `tmp/vitessce-3.2.5.tar.gz` & `tmp/vitessce-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitessce-3.2.5.tar", last modified: Tue Apr 16 20:21:46 2024, max compression
+gzip compressed data, was "vitessce-3.2.6.tar", last modified: Wed May  1 21:51:16 2024, max compression
```

## Comparing `vitessce-3.2.5.tar` & `vitessce-3.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.086568 vitessce-3.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 20:19:36.000000 vitessce-3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-16 20:19:36.000000 vitessce-3.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-16 20:21:46.086568 vitessce-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-16 20:19:36.000000 vitessce-3.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-16 20:19:36.000000 vitessce-3.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 20:21:46.086568 vitessce-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:19:36.000000 vitessce-3.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.078568 vitessce-3.2.5/vitessce/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75366 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/config_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.082568 vitessce-3.2.5/vitessce/data_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/multivec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/ome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    53910 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.082568 vitessce-3.2.5/vitessce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:51:16.640010 vitessce-3.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 21:49:25.000000 vitessce-3.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-01 21:49:25.000000 vitessce-3.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-01 21:51:16.640010 vitessce-3.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-01 21:49:25.000000 vitessce-3.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-01 21:49:25.000000 vitessce-3.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-01 21:51:16.640010 vitessce-3.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:49:25.000000 vitessce-3.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:51:16.632010 vitessce-3.2.6/vitessce/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75998 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:51:16.636010 vitessce-3.2.6/vitessce/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/data_utils/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/data_utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/data_utils/multivec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/data_utils/ome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56573 2024-05-01 21:49:25.000000 vitessce-3.2.6/vitessce/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:51:16.636010 vitessce-3.2.6/vitessce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-01 21:51:16.000000 vitessce-3.2.6/vitessce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-01 21:51:16.000000 vitessce-3.2.6/vitessce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:51:16.000000 vitessce-3.2.6/vitessce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 21:51:16.000000 vitessce-3.2.6/vitessce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:51:16.000000 vitessce-3.2.6/vitessce.egg-info/top_level.txt
```

### Comparing `vitessce-3.2.5/LICENSE` & `vitessce-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/PKG-INFO` & `vitessce-3.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.5
+Version: 3.2.6
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,15 +70,15 @@
 Requires-Dist: nbsphinx==0.8.8; extra == "docs"
 Requires-Dist: nbclean==0.3.2; extra == "docs"
 Requires-Dist: sqlalchemy==1.3.24; extra == "docs"
 Requires-Dist: nbconvert==5.6.1; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Provides-Extra: all
 Requires-Dist: jupyter-server-proxy>=1.5.2; extra == "all"
-Requires-Dist: anywidget>=0.9.3; extra == "all"
+Requires-Dist: anywidget>=0.9.10; extra == "all"
 Requires-Dist: uvicorn>=0.17.0; extra == "all"
 Requires-Dist: ujson>=4.0.1; extra == "all"
 Requires-Dist: starlette==0.14.0; extra == "all"
 Requires-Dist: generate-tiff-offsets>=0.1.7; extra == "all"
 Requires-Dist: aiofiles>=0.6.0; extra == "all"
 Provides-Extra: building
 Provides-Extra: testing
```

### Comparing `vitessce-3.2.5/README.md` & `vitessce-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/pyproject.toml` & `vitessce-3.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel>=0.38.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vitessce"
-version = "3.2.5"
+version = "3.2.6"
 authors = [
   { name="Mark Keller", email="mark_keller@hms.harvard.edu" },
 ]
 description = "Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -69,15 +69,15 @@
   # nbconvert and jinja2 versions need to be pinned.
   # Reference: https://github.com/vitessce/vitessce-python/issues/152
   'nbconvert==5.6.1',
   'jinja2==3.0.3',
 ]
 all = [
   'jupyter-server-proxy>=1.5.2',
-  'anywidget>=0.9.3',
+  'anywidget>=0.9.10',
   'uvicorn>=0.17.0',
   'ujson>=4.0.1',
   'starlette==0.14.0',
   'generate-tiff-offsets>=0.1.7',
 
   # aiofiles is not explicitly referenced in our code,
   # but it is an implicit dependency of starlette==0.14.0.
```

### Comparing `vitessce-3.2.5/setup.cfg` & `vitessce-3.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/__init__.py` & `vitessce-3.2.6/vitessce/__init__.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/config.py` & `vitessce-3.2.6/vitessce/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,24 @@
     def get_routes(self):
         routes = []
         for obj in self.objs:
             routes += obj.get_routes()
 
         return routes
 
+    def get_stores(self, base_url=None):
+        stores = {}
+        for obj in self.objs:
+            stores = {
+                **stores,
+                **obj.get_stores(base_url)
+            }
+
+        return stores
+
 
 class VitessceConfigViewHConcat:
     """
     A class to represent a horizontal concatenation of view instances.
     """
 
     def __init__(self, views):
@@ -1485,14 +1495,29 @@
         :rtype: list[starlette.routing.Route]
         """
         routes = []
         for d in self.config["datasets"]:
             routes += d.get_routes()
         return routes
 
+    def get_stores(self, base_url=None):
+        """
+        Convert the routes for this view config from the datasets.
+
+        :returns: A list of server routes.
+        :rtype: list[starlette.routing.Route]
+        """
+        stores = {}
+        for d in self.config["datasets"]:
+            stores = {
+                **stores,
+                **d.get_stores(base_url)
+            }
+        return stores
+
     def to_python(self):
         """
         Convert the VitessceConfig instance to a one-line Python code snippet that can be used to generate it.
 
         :returns: (A list of classes from the vitessce package used in the code block, The formatted code block)
         :rtype: (list[str], str)
         """
```

### Comparing `vitessce-3.2.5/vitessce/config_converter.py` & `vitessce-3.2.6/vitessce/config_converter.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/constants.py` & `vitessce-3.2.6/vitessce/constants.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/data_utils/anndata.py` & `vitessce-3.2.6/vitessce/data_utils/anndata.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/data_utils/entities.py` & `vitessce-3.2.6/vitessce/data_utils/entities.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/data_utils/multivec.py` & `vitessce-3.2.6/vitessce/data_utils/multivec.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/data_utils/ome.py` & `vitessce-3.2.6/vitessce/data_utils/ome.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/export.py` & `vitessce-3.2.6/vitessce/export.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/repr.py` & `vitessce-3.2.6/vitessce/repr.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/routes.py` & `vitessce-3.2.6/vitessce/routes.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/utils.py` & `vitessce-3.2.6/vitessce/utils.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce/widget.py` & `vitessce-3.2.6/vitessce/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib.util
 from urllib.parse import quote_plus
 import json
 
 # Widget dependencies
 import anywidget
-from traitlets import Unicode, Dict, Int, Bool
+from traitlets import Unicode, Dict, List, Int, Bool
 import time
 import uuid
 
 # Server dependencies
 from uvicorn import Config, Server
 
 from starlette.applications import Starlette
@@ -197,14 +197,15 @@
 async function render(view) {
     const cssUid = view.model.get('uid');
     const jsDevMode = view.model.get('js_dev_mode');
     const jsPackageVersion = view.model.get('js_package_version');
     const customJsUrl = view.model.get('custom_js_url');
     const pluginEsm = view.model.get('plugin_esm');
     const remountOnUidChange = view.model.get('remount_on_uid_change');
+    const storeUrls = view.model.get('store_urls');
 
     const pkgName = (jsDevMode ? "@vitessce/dev" : "vitessce");
 
     importMap.imports["vitessce"] = (customJsUrl.length > 0
         ? customJsUrl
         : `https://unpkg.com/${pkgName}@${jsPackageVersion}`
     );
@@ -220,14 +221,27 @@
     } = await importWithMap("vitessce", importMap);
 
     let pluginViewTypes;
     let pluginCoordinationTypes;
     let pluginFileTypes;
     let pluginJointFileTypes;
 
+    const stores = Object.fromEntries(
+        storeUrls.map(storeUrl => ([
+            storeUrl,
+            {
+                async get(key) {
+                    const [data, buffers] = await view.experimental.invoke("_zarr_get", [storeUrl, key]);
+                    if (!data.success) return undefined;
+                    return buffers[0].buffer;
+                },
+            }
+        ])),
+    );
+
     try {
         const pluginEsmUrl = URL.createObjectURL(new Blob([pluginEsm], { type: "text/javascript" }));
         const pluginModule = (await import(pluginEsmUrl)).default;
         URL.revokeObjectURL(pluginEsmUrl);
 
         const pluginsObj = await pluginModule.createPlugins({
             React,
@@ -306,15 +320,15 @@
                 setConfig(newConfig);
             });
         }, []);
 
         const vitessceProps = {
             height, theme, config, onConfigChange, validateConfig,
             pluginViewTypes, pluginCoordinationTypes, pluginFileTypes, pluginJointFileTypes,
-            remountOnUidChange,
+            remountOnUidChange, stores,
         };
 
         return e('div', { ref: divRef, style: { height: height + 'px' } },
             e(React.Suspense, { fallback: e('div', {}, 'Loading...') },
                 e(React.StrictMode, {},
                     e(Vitessce, vitessceProps)
                 ),
@@ -379,21 +393,23 @@
     theme = Unicode('auto').tag(sync=True)
     proxy = Bool(False).tag(sync=True)
     uid = Unicode('').tag(sync=True)
     has_host_name = Bool(False).tag(sync=True)
 
     next_port = DEFAULT_PORT
 
-    js_package_version = Unicode('3.3.7').tag(sync=True)
+    js_package_version = Unicode('3.3.12').tag(sync=True)
     js_dev_mode = Bool(False).tag(sync=True)
     custom_js_url = Unicode('').tag(sync=True)
     plugin_esm = Unicode(DEFAULT_PLUGIN_ESM).tag(sync=True)
     remount_on_uid_change = Bool(True).tag(sync=True)
 
-    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='3.3.7', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
+    store_urls = List(trait=Unicode(''), default_value=[]).tag(sync=True)
+
+    def __init__(self, config, height=600, theme='auto', uid=None, port=None, proxy=False, js_package_version='3.3.12', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
         """
         Construct a new Vitessce widget.
 
         :param config: A view config instance.
         :type config: VitessceConfig
         :param str theme: The theme name, either "light" or "dark". By default, "auto", which selects light or dark based on operating system preferences.
         :param int height: The height of the widget, in pixels. By default, 600.
@@ -418,21 +434,23 @@
         base_url, use_port, VitessceWidget.next_port = get_base_url_and_port(
             port, VitessceWidget.next_port, proxy=proxy)
         self.config_obj = config
         self.port = use_port
         config_dict = config.to_dict(base_url=base_url)
         routes = config.get_routes()
 
+        self._stores = config.get_stores(base_url=base_url)
+
         uid_str = get_uid_str(uid)
 
         super(VitessceWidget, self).__init__(
             config=config_dict, height=height, theme=theme, proxy=proxy,
             js_package_version=js_package_version, js_dev_mode=js_dev_mode, custom_js_url=custom_js_url,
             plugin_esm=plugin_esm, remount_on_uid_change=remount_on_uid_change,
-            uid=uid_str,
+            uid=uid_str, store_urls=list(self._stores.keys())
         )
 
         serve_routes(config, routes, use_port)
 
     def _get_coordination_value(self, coordination_type, coordination_scope):
         obj = self.config['coordinationSpace'][coordination_type]
         obj_scopes = list(obj.keys())
@@ -456,18 +474,28 @@
     def get_cell_selection(self, scope=None):
         return self._get_coordination_value('cellSelection', scope)
 
     def close(self):
         self.config_obj.stop_server(self.port)
         super().close()
 
+    @anywidget.experimental.command
+    def _zarr_get(self, params, buffers):
+        [store_url, key] = params
+        store = self._stores[store_url]
+        try:
+            buffers = [store[key.lstrip("/")]]
+        except KeyError:
+            buffers = []
+        return {"success": len(buffers) == 1}, buffers
+
 # Launch Vitessce using plain HTML representation (no ipywidgets)
 
 
-def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='3.3.7', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
+def ipython_display(config, height=600, theme='auto', base_url=None, host_name=None, uid=None, port=None, proxy=False, js_package_version='3.3.12', js_dev_mode=False, custom_js_url='', plugin_esm=DEFAULT_PLUGIN_ESM, remount_on_uid_change=True):
     from IPython.display import display, HTML
     uid_str = "vitessce" + get_uid_str(uid)
 
     base_url, use_port, _ = get_base_url_and_port(
         port, DEFAULT_PORT, proxy=proxy, base_url=base_url, host_name=host_name)
     config_dict = config.to_dict(base_url=base_url)
     routes = config.get_routes()
@@ -481,14 +509,15 @@
         "plugin_esm": plugin_esm,
         "remount_on_uid_change": remount_on_uid_change,
         "proxy": proxy,
         "has_host_name": host_name is not None,
         "height": height,
         "theme": theme,
         "config": config_dict,
+        "store_urls": [],
     }
 
     # We need to clean up the React and DOM state in any case in which
     # .display() is being run in the same cell as a previous .display().
     # Otherwise, React tries to diff the virtual DOM,
     # causing the browser to become unresponsive.
```

### Comparing `vitessce-3.2.5/vitessce/wrappers.py` & `vitessce-3.2.6/vitessce/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from os.path import join
 import tempfile
 from uuid import uuid4
 from pathlib import PurePath, PurePosixPath
+import zarr
 
 from .constants import (
     norm_enum,
     ViewType as cm,
     FileType as ft,
     DataType as dt,
 )
@@ -37,17 +38,19 @@
 
         :param str out_dir: The path to a local directory used for data processing outputs. By default, uses a temp. directory.
         :param dict request_init: options to be passed along with every fetch request from the browser, like `{ "header": { "Authorization": "Bearer dsfjalsdfa1431" } }`
         """
         self.out_dir = kwargs['out_dir'] if 'out_dir' in kwargs else tempfile.mkdtemp(
         )
         self.routes = []
-        self.is_remote = False
+        self.is_remote = False  # TODO: change to needs_localhost_serving for clarity
+        self.is_store = False  # TODO: change to needs_store_registration for clarity
         self.file_def_creators = []
         self.base_dir = None
+        self.stores = {}
         self._request_init = kwargs['request_init'] if 'request_init' in kwargs else None
 
     def __repr__(self):
         return self._repr
 
     def convert_and_save(self, dataset_uid, obj_i, base_dir=None):
         """
@@ -67,14 +70,28 @@
         Obtain the routes that have been created for this wrapper class.
 
         :returns: A list of server routes.
         :rtype: list[starlette.routing.Route]
         """
         return self.routes
 
+    def get_stores(self, base_url):
+        """
+        Obtain the stores that have been created for this wrapper class.
+
+        :returns: A dictionary that maps file URLs to Zarr Store objects.
+        :rtype: dict[str, zarr.Store]
+        """
+        relative_stores = self.stores
+        absolute_stores = {}
+        for relative_url, store in relative_stores.items():
+            absolute_url = base_url + relative_url
+            absolute_stores[absolute_url] = store
+        return absolute_stores
+
     def get_file_defs(self, base_url):
         """
         Obtain the file definitions for this wrapper class.
 
         :param str base_url: A base URL to prepend to relative URLs.
 
         :returns: A list of file definitions.
@@ -107,14 +124,38 @@
         return []
 
     def get_local_dir_url(self, base_url, dataset_uid, obj_i, local_dir_path, local_dir_uid):
         if not self.is_remote and self.base_dir is not None:
             return self._get_url_simple(base_url, file_path_to_url_path(local_dir_path, prepend_slash=False))
         return self._get_url(base_url, dataset_uid, obj_i, local_dir_uid)
 
+    def register_zarr_store(self, dataset_uid, obj_i, store_or_local_dir_path, local_dir_uid):
+        if not self.is_remote and self.is_store:
+            # Set up `store` and `local_dir_path` variables.
+            if isinstance(store_or_local_dir_path, str):
+                # TODO: use zarr.FSStore if fsspec is installed?
+                store = zarr.DirectoryStore(store_or_local_dir_path)
+                local_dir_path = store_or_local_dir_path
+            else:
+                # TODO: check that store_or_local_dir_path is a zarr.Store or StoreLike?
+                store = store_or_local_dir_path
+                # A store instance was passed directly, so there is no local directory path.
+                # Instead we just make one up using _get_route_str but it could be any string.
+                local_dir_path = self._get_route_str(dataset_uid, obj_i, local_dir_uid)
+
+            # Register the store on the same route path
+            # that will be used for the "url" field in the file definition.
+            if self.base_dir is None:
+                route_path = self._get_route_str(dataset_uid, obj_i, local_dir_uid)
+            else:
+                route_path = file_path_to_url_path(local_dir_path)
+                local_dir_path = join(self.base_dir, local_dir_path)
+
+            self.stores[route_path] = store
+
     def get_local_dir_route(self, dataset_uid, obj_i, local_dir_path, local_dir_uid):
         """
         Obtain the Mount for some local directory
 
         :param str dataset_uid: A dataset unique identifier for the Mount
         :param str obj_i: A index of the current vitessce.wrappers.AbstractWrapper among all other wrappers in the view config
         :param str local_dir_path: The path to the local directory to serve.
@@ -892,20 +933,22 @@
                 file_def["coordinationValues"] = self._coordination_values
             return file_def
 
         return image_file_def_creator
 
 
 class AnnDataWrapper(AbstractWrapper):
-    def __init__(self, adata_path=None, adata_url=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, obs_spots_path=None, obs_points_path=None, feature_labels_path=None, obs_labels_path=None, convert_to_dense=True, coordination_values=None, obs_labels_paths=None, obs_labels_names=None, **kwargs):
+    def __init__(self, adata_path=None, adata_url=None, adata_store=None, obs_feature_matrix_path=None, feature_filter_path=None, initial_feature_filter_path=None, obs_set_paths=None, obs_set_names=None, obs_locations_path=None, obs_segmentations_path=None, obs_embedding_paths=None, obs_embedding_names=None, obs_embedding_dims=None, obs_spots_path=None, obs_points_path=None, feature_labels_path=None, obs_labels_path=None, convert_to_dense=True, coordination_values=None, obs_labels_paths=None, obs_labels_names=None, **kwargs):
         """
         Wrap an AnnData object by creating an instance of the ``AnnDataWrapper`` class.
 
         :param str adata_path: A path to an AnnData object written to a Zarr store containing single-cell experiment data.
         :param str adata_url: A remote url pointing to a zarr-backed AnnData store.
+        :param adata_store: A path to pass to zarr.FSStore, or an existing store instance.
+        :type adata_store: str or zarr.Storage
         :param str obs_feature_matrix_path: Location of the expression (cell x gene) matrix, like `X` or `obsm/highly_variable_genes_subset`
         :param str feature_filter_path: A string like `var/highly_variable` used in conjunction with `obs_feature_matrix_path` if obs_feature_matrix_path points to a subset of `X` of the full `var` list.
         :param str initial_feature_filter_path: A string like `var/highly_variable` used in conjunction with `obs_feature_matrix_path` if obs_feature_matrix_path points to a subset of `X` of the full `var` list.
         :param list[str] obs_set_paths: Column names like `['obs/louvain', 'obs/cellType']` for showing cell sets
         :param list[str] obs_set_names: Names to display in place of those in `obs_set_paths`, like `['Louvain', 'Cell Type']`
         :param str obs_locations_path: Column name in `obsm` that contains centroid coordinates for displaying centroids in the spatial viewer
         :param str obs_segmentations_path: Column name in `obsm` that contains polygonal coordinates for displaying outlines in the spatial viewer
@@ -923,26 +966,38 @@
         :type coordination_values: dict or None
         :param \\*\\*kwargs: Keyword arguments inherited from :class:`~vitessce.wrappers.AbstractWrapper`
         """
         super().__init__(**kwargs)
         self._repr = make_repr(locals())
         self._adata_path = adata_path
         self._adata_url = adata_url
-        if adata_url is not None and (adata_path is not None):
+        self._adata_store = adata_store
+
+        num_inputs = sum([1 for x in [adata_path, adata_url, adata_store] if x is not None])
+        if num_inputs > 1:
             raise ValueError(
-                "Did not expect adata_url to be provided with adata_path")
-        if adata_url is None and (adata_path is None):
+                "Expected only one of adata_path, adata_url, or adata_store to be provided")
+        if num_inputs == 0:
             raise ValueError(
-                "Expected either adata_url or adata_path to be provided")
+                "Expected one of adata_path, adata_url, or adata_store to be provided")
+
         if adata_path is not None:
             self.is_remote = False
+            self.is_store = False
             self.zarr_folder = 'anndata.zarr'
-        else:
+        elif adata_url is not None:
             self.is_remote = True
+            self.is_store = False
             self.zarr_folder = None
+        else:
+            # Store case
+            self.is_remote = False
+            self.is_store = True
+            self.zarr_folder = None
+
         self.local_dir_uid = make_unique_filename(".adata.zarr")
         self._expression_matrix = obs_feature_matrix_path
         self._cell_set_obs_names = obs_set_names
         self._mappings_obsm_names = obs_embedding_names
         self._gene_var_filter = feature_filter_path
         self._matrix_gene_var_filter = initial_feature_filter_path
         self._cell_set_obs = obs_set_paths
@@ -974,14 +1029,17 @@
 
         self.file_def_creators.append(file_def_creator)
         self.routes += routes
 
     def make_anndata_routes(self, dataset_uid, obj_i):
         if self.is_remote:
             return []
+        elif self.is_store:
+            self.register_zarr_store(dataset_uid, obj_i, self._adata_store, self.local_dir_uid)
+            return []
         else:
             return self.get_local_dir_route(dataset_uid, obj_i, self._adata_path, self.local_dir_uid)
 
     def get_zarr_url(self, base_url="", dataset_uid="", obj_i=""):
         if self.is_remote:
             return self._adata_url
         else:
```

### Comparing `vitessce-3.2.5/vitessce.egg-info/PKG-INFO` & `vitessce-3.2.6/vitessce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.5
+Version: 3.2.6
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,15 +70,15 @@
 Requires-Dist: nbsphinx==0.8.8; extra == "docs"
 Requires-Dist: nbclean==0.3.2; extra == "docs"
 Requires-Dist: sqlalchemy==1.3.24; extra == "docs"
 Requires-Dist: nbconvert==5.6.1; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Provides-Extra: all
 Requires-Dist: jupyter-server-proxy>=1.5.2; extra == "all"
-Requires-Dist: anywidget>=0.9.3; extra == "all"
+Requires-Dist: anywidget>=0.9.10; extra == "all"
 Requires-Dist: uvicorn>=0.17.0; extra == "all"
 Requires-Dist: ujson>=4.0.1; extra == "all"
 Requires-Dist: starlette==0.14.0; extra == "all"
 Requires-Dist: generate-tiff-offsets>=0.1.7; extra == "all"
 Requires-Dist: aiofiles>=0.6.0; extra == "all"
 Provides-Extra: building
 Provides-Extra: testing
```

### Comparing `vitessce-3.2.5/vitessce.egg-info/SOURCES.txt` & `vitessce-3.2.6/vitessce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.5/vitessce.egg-info/requires.txt` & `vitessce-3.2.6/vitessce.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ome-zarr==0.8.3
 tifffile>=2020.10.1
 jsonschema>=3.2
 tqdm>=4.1.0
 
 [all]
 jupyter-server-proxy>=1.5.2
-anywidget>=0.9.3
+anywidget>=0.9.10
 uvicorn>=0.17.0
 ujson>=4.0.1
 starlette==0.14.0
 generate-tiff-offsets>=0.1.7
 aiofiles>=0.6.0
 
 [building]
```

