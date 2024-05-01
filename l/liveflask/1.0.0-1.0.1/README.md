# Comparing `tmp/liveflask-1.0.0.tar.gz` & `tmp/liveflask-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.0.tar", last modified: Wed May  1 19:38:45 2024, max compression
+gzip compressed data, was "liveflask-1.0.1.tar", last modified: Wed May  1 20:13:02 2024, max compression
```

## Comparing `liveflask-1.0.0.tar` & `liveflask-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.111272 liveflask-1.0.0/
--rw-rw-rw-   0        0        0     1342 2024-05-01 19:38:45.110268 liveflask-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.068269 liveflask-1.0.0/liveflask/
--rw-rw-rw-   0        0        0     5758 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.078271 liveflask-1.0.0/liveflask/mvlive/
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.080273 liveflask-1.0.0/liveflask/mvlive/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.089270 liveflask-1.0.0/liveflask/mvlive/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/__init__.py
--rw-rw-rw-   0        0        0     2058 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/has_props.py
--rw-rw-rw-   0        0        0     2494 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/has_renders.py
--rw-rw-rw-   0        0        0     4114 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/mvlive/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.091270 liveflask-1.0.0/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.103270 liveflask-1.0.0/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0      872 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     8446 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.107268 liveflask-1.0.0/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      284 2024-05-01 18:57:08.000000 liveflask-1.0.0/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-01 19:38:45.075269 liveflask-1.0.0/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-01 19:38:45.000000 liveflask-1.0.0/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      895 2024-05-01 19:38:45.000000 liveflask-1.0.0/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:38:45.000000 liveflask-1.0.0/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 19:38:45.000000 liveflask-1.0.0/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 19:38:45.000000 liveflask-1.0.0/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 19:38:45.112270 liveflask-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-05-01 19:37:43.000000 liveflask-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.917877 liveflask-1.0.1/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 20:13:02.915878 liveflask-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.872877 liveflask-1.0.1/liveflask/
+-rw-rw-rw-   0        0        0     5778 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.883876 liveflask-1.0.1/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.884876 liveflask-1.0.1/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.898877 liveflask-1.0.1/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1566 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0      872 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     8446 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.902877 liveflask-1.0.1/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      284 2024-05-01 18:57:08.000000 liveflask-1.0.1/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.914877 liveflask-1.0.1/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/__init__.py
+-rw-rw-rw-   0        0        0     2042 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 20:12:56.000000 liveflask-1.0.1/liveflask/traits/has_snapshots.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:13:02.881876 liveflask-1.0.1/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 20:13:02.000000 liveflask-1.0.1/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:13:02.917877 liveflask-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-01 20:12:56.000000 liveflask-1.0.1/setup.py
```

### Comparing `liveflask-1.0.0/PKG-INFO` & `liveflask-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.0
+Version: 1.0.1
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.0/liveflask/__init__.py` & `liveflask-1.0.1/liveflask/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 import secrets
 
 from flask import Blueprint, render_template, Response
 from flask import request
 from markupsafe import Markup
 
-from .mvlive.traits.has_actions import HasActions
-from .mvlive.traits.has_props import HasProps
-from .mvlive.traits.has_renders import HasRenders
-from .mvlive.traits.has_snapshots import HasSnapshots
+from .traits.has_actions import HasActions
+from .traits.has_props import HasProps
+from .traits.has_renders import HasRenders
+from .traits.has_snapshots import HasSnapshots
 
 
 def parse_argument(arg):
     try:
         return ast.literal_eval(arg)
     except (SyntaxError, ValueError):
         # If the literal is not valid, return the string itself
@@ -79,20 +79,23 @@
             cls.mvlive__session = []
             cls.mvlive__url = []
 
     DecoratedClass.__name__ = cls.__name__
     return DecoratedClass
 
 
-class MVLive(HasRenders, HasProps, HasSnapshots, HasActions):
+class LiveFlask(HasRenders, HasProps, HasSnapshots, HasActions):
     pass
 
 
-def LiveFlask(app):
-    app.add_template_global(MVLive().inital_render, 'live')
+def LiveFlaskExt(app):
+    app.add_template_global(
+        LiveFlask().inital_render, 'live'
+    )
+
     package_dir = os.path.dirname(os.path.abspath(__file__))
     enduser_project_dir = os.getcwd()
     # check if the project directory has a templates folder
     if not os.path.exists(f"{enduser_project_dir}/templates"):
         os.makedirs(f"{enduser_project_dir}/templates")
 
     # check if the templates folder has a liveflask folder
@@ -101,36 +104,36 @@
 
     liveflask_bp = Blueprint('live', __name__, static_folder='static',
                              template_folder='templates')
 
     @liveflask_bp.post('/')
     def live():
         req = request.json
-        _class: object = MVLive().from_snapshot(req)
+        _class: object = LiveFlask().from_snapshot(req)
 
         if req.get('method'):
             method = req.get('method')
             args = req.get('args')
             kwargs = req.get('kwargs') or {}
             if method == "emit":
-                component = MVLive().call_event_handler(_class, method, *return_arguments(args), **kwargs)
+                component = LiveFlask().call_event_handler(_class, method, *return_arguments(args), **kwargs)
             elif method == "emit_to":
-                component = MVLive().call_event_handler(_class, method, *return_arguments(args), **kwargs)
+                component = LiveFlask().call_event_handler(_class, method, *return_arguments(args), **kwargs)
             else:
-                component = MVLive().call_method(_class, method, *return_arguments(args))
+                component = LiveFlask().call_method(_class, method, *return_arguments(args))
 
         if req.get('update_property'):
             req_updated_prop = req.get('update_property')
-            MVLive().set_props(_class, req_updated_prop[0], req_updated_prop[1])
+            LiveFlask().set_props(_class, req_updated_prop[0], req_updated_prop[1])
             component = _class
 
-        MVLive().set_props(_class, 'emits', _class.emits)
+        LiveFlask().set_props(_class, 'emits', _class.emits)
         component = _class
 
-        html, snapshot = MVLive().to_snapshot(component)
+        html, snapshot = LiveFlask().to_snapshot(component)
         return {
             "html": html, "snapshot": snapshot
         }
 
     @liveflask_bp.route('/bundle.js')
     def bundle_js():
         js_files = [
```

### Comparing `liveflask-1.0.0/liveflask/mvlive/attributes/__init__.py` & `liveflask-1.0.1/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/mvlive/traits/has_actions.py` & `liveflask-1.0.1/liveflask/traits/has_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, NoReturn
 
 from flask import session
-from ...mvlive.traits.Bootable import Bootable
-from ...mvlive.utils import dict_diff_changed_values
+from ..traits.Bootable import Bootable
+from ..utils import dict_diff_changed_values
 
 
 class HasActions:
     def call_method(self, component: Any, method: str, *args) -> NoReturn:
         props = self.get_props(component)
         Bootable.init_bootable_hook(_class=component)
```

### Comparing `liveflask-1.0.0/liveflask/mvlive/traits/has_props.py` & `liveflask-1.0.1/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/mvlive/traits/has_renders.py` & `liveflask-1.0.1/liveflask/traits/has_renders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any
 
 from flask import render_template_string, session
 from flask import request as req
 from markupsafe import Markup
 
-from ...mvlive.utils import to_class
+from ..utils import to_class
 
 
 class HasRenders:
     def inital_render(self, component_name: str, *args, **kwargs):
         #print(f"Doing initial render {component_name}")
         # if key == "":
         #     key = f"mvlive_{component_name}_{secrets.token_urlsafe()}"
```

### Comparing `liveflask-1.0.0/liveflask/mvlive/traits/has_snapshots.py` & `liveflask-1.0.1/liveflask/traits/has_snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pprint
 import secrets
 from typing import Any
 
 from flask import render_template_string
 from markupsafe import Markup
 
-from ...mvlive.utils import to_class
+from ..utils import to_class
 
 
 class HasSnapshots:
     def from_snapshot(self, req_snapshot: dict[str, Any]):
         req_checksum: str = req_snapshot['snapshot']['checksum']
         del req_snapshot['snapshot']['checksum']
         if 'children' in req_snapshot['snapshot']:
```

### Comparing `liveflask-1.0.0/liveflask/static/liveflask/action.js` & `liveflask-1.0.1/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.1/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/static/liveflask/model.js` & `liveflask-1.0.1/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/static/liveflask/polling.js` & `liveflask-1.0.1/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/static/liveflask/utils.js` & `liveflask-1.0.1/liveflask/static/liveflask/utils.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask/static/lodash.min.js` & `liveflask-1.0.1/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.0/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.1/liveflask.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.0
+Version: 1.0.1
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.0/setup.py` & `liveflask-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.0",
+    version="1.0.1",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

