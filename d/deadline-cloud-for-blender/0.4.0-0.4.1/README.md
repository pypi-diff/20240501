# Comparing `tmp/deadline_cloud_for_blender-0.4.0.tar.gz` & `tmp/deadline_cloud_for_blender-0.4.1.tar.gz`

## Comparing `deadline_cloud_for_blender-0.4.0.tar` & `deadline_cloud_for_blender-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/_version.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/BlenderAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py
--rw-r--r--   0        0        0    18486 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/py.typed
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/py.typed
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/cycles_blender_handler.py
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/workbench_blender_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/_version.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/_version.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py
--rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/NOTICE
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/README.md
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/hatch.toml
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/_version.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/BlenderAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py
+-rw-r--r--   0        0        0    18486 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/py.typed
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/blender_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/py.typed
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/cycles_blender_handler.py
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/workbench_blender_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/_version.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/_version.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/NOTICE
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/README.md
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/hatch.toml
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.1/PKG-INFO
```

### Comparing `deadline_cloud_for_blender-0.4.0/hatch_custom_hook.py` & `deadline_cloud_for_blender-0.4.1/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/blender_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py` & `deadline_cloud_for_blender-0.4.1/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/LICENSE` & `deadline_cloud_for_blender-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/README.md` & `deadline_cloud_for_blender-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/hatch.toml` & `deadline_cloud_for_blender-0.4.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.4.0/pyproject.toml` & `deadline_cloud_for_blender-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
 ]
 # Blender 3.1-4.0 uses Python version 3.10
 # Blender 4.1+ uses Python version 3.11
 
 dependencies = [
-    "deadline == 0.47.*", 
+    "deadline == 0.48.*", 
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-blender"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-blender"
```

### Comparing `deadline_cloud_for_blender-0.4.0/PKG-INFO` & `deadline_cloud_for_blender-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-blender
-Version: 0.4.0
+Version: 0.4.1
 Summary: AWS Deadline Cloud for Blender
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-blender
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-blender
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
-Requires-Dist: deadline==0.47.*
+Requires-Dist: deadline==0.48.*
 Requires-Dist: openjd-adaptor-runtime==0.7.*
 Description-Content-Type: text/markdown
 
 # AWS Deadline Cloud for Blender
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-blender.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-blender)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-blender.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-blender)
```

