# Comparing `tmp/deadline_cloud_for_maya-0.14.0.tar.gz` & `tmp/deadline_cloud_for_maya-0.14.1.tar.gz`

## Comparing `deadline_cloud_for_maya-0.14.0.tar` & `deadline_cloud_for_maya-0.14.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/_version.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/MayaAdaptor.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/__main__.py
--rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/py.typed
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/__init__.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/dir_map.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/maya_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/py.typed
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/arnold_handler.py
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/default_maya_handler.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/renderman_handler.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/vray_handler.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/_version.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/assets.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/cameras.py
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/data_classes.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/default_maya_job_template.yaml
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/file_path_editor.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/job_bundle_output_test_runner.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/logging.py
--rw-r--r--   0        0        0    28212 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/maya_render_submitter.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/mel_commands.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/render_layers.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/renderers.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/scene.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/shelf.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/NOTICE
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/README.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/hatch.toml
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/_version.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/MayaAdaptor.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/__main__.py
+-rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/py.typed
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/__init__.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/dir_map.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/maya_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/py.typed
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/arnold_handler.py
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/default_maya_handler.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/renderman_handler.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/vray_handler.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/_version.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/assets.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/cameras.py
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/data_classes.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/default_maya_job_template.yaml
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/file_path_editor.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/job_bundle_output_test_runner.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/logging.py
+-rw-r--r--   0        0        0    28212 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/maya_render_submitter.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/mel_commands.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/render_layers.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/renderers.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/scene.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/shelf.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/NOTICE
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/README.md
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/hatch.toml
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 deadline_cloud_for_maya-0.14.1/PKG-INFO
```

### Comparing `deadline_cloud_for_maya-0.14.0/hatch_custom_hook.py` & `deadline_cloud_for_maya-0.14.1/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/__main__.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/adaptor.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/dir_map.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/dir_map.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/maya_client.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/maya_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/__init__.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/arnold_handler.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/arnold_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/default_maya_handler.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/default_maya_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/renderman_handler.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/renderman_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_adaptor/MayaClient/render_handlers/vray_handler.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_adaptor/MayaClient/render_handlers/vray_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/assets.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/cameras.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/cameras.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/data_classes.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/default_maya_job_template.yaml` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/default_maya_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/file_path_editor.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/file_path_editor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/job_bundle_output_test_runner.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/job_bundle_output_test_runner.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/logging.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/logging.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/maya_render_submitter.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/maya_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/mel_commands.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/mel_commands.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/render_layers.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/render_layers.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/renderers.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/renderers.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/scene.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/scene.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/shelf.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/shelf.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/utils.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/src/deadline/maya_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_maya-0.14.1/src/deadline/maya_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/LICENSE` & `deadline_cloud_for_maya-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/README.md` & `deadline_cloud_for_maya-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/hatch.toml` & `deadline_cloud_for_maya-0.14.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_maya-0.14.0/pyproject.toml` & `deadline_cloud_for_maya-0.14.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Operating System :: MacOS",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop"
 ]
 
 dependencies = [
-    "deadline == 0.47.*",
+    "deadline == 0.48.*",
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-maya"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-maya"
```

### Comparing `deadline_cloud_for_maya-0.14.0/PKG-INFO` & `deadline_cloud_for_maya-0.14.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-maya
-Version: 0.14.0
+Version: 0.14.1
 Summary: AWS Deadline Cloud for Maya
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-maya
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-maya
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
 
 # AWS Deadline Cloud for Maya
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-maya.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-maya)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-maya.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-maya)
```

