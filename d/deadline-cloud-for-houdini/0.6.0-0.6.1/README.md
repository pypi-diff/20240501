# Comparing `tmp/deadline_cloud_for_houdini-0.6.0.tar.gz` & `tmp/deadline_cloud_for_houdini-0.6.1.tar.gz`

## Comparing `deadline_cloud_for_houdini-0.6.0.tar` & `deadline_cloud_for_houdini-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
--rw-r--r--   0        0        0    20756 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/_version.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
--rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
--rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
--rw-r--r--   0        0        0    28171 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/NOTICE
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/hatch.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
+-rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/_version.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
+-rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
+-rw-r--r--   0        0        0    28434 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/NOTICE
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/hatch.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/PKG-INFO
```

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,17 @@
 
         Returns:
             str: The value to set HOUDINI_PATHMAP to
         """
         path_mapping_rules: dict[str, str] = {}
 
         for rule in self._path_mapping_rules:
-            path_mapping_rules[rule.source_path] = rule.destination_path
+            path_mapping_rules[rule.source_path.replace("\\", "/")] = rule.destination_path.replace(
+                "\\", "/"
+            )
 
         if path_mapping_rules:
             return str(path_mapping_rules)
         return ""
 
     def on_start(self) -> None:
         """
```

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated`

 * *Files 27% similar despite different names*

```diff
@@ -9,8 +9,8 @@
     farm_response = deadline.get_farm(farmId=farm_id)
     node.parm('farm').set(farm_response['displayName'])
     queue_id = get_setting('defaults.queue_id')
     queue_response = deadline.get_queue(farmId=farm_id, queueId=queue_id)
     node.parm('queue').set(queue_response['displayName'])
     node.hdaModule().update_queue_parameters_callback(kwargs)
 except CredentialRetrievalError:
-    print('Expired credentials')
+    print('AWS Deadline Cloud credentials are expired.')
```

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py` & `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from deadline.job_attachments.models import JobAttachmentS3Settings
 
 from .queue_parameters import update_queue_parameters, get_queue_parameter_values_as_openjd
 from ._version import version
 
 import hou
 
-IGNORE_REF_VALUES = ("opdef:", "oplib:", "temp:")
+IGNORE_REF_VALUES = ("opdef:", "oplib:", "temp:", "op:")
 IGNORE_REF_PARMS = (
     "taskgraphfile",
     "pdg_workingdir",
     "soho_program",
     "BakeView_img_file_path",
     "OutputDeepWriter_file",
     "SettingsOutput_img_file_path",
@@ -44,27 +44,31 @@
 def _get_houdini_version() -> str:
     return hou.applicationVersionString()
 
 
 def _get_scene_asset_references(rop_node: hou.Node) -> AssetReferences:
     # collect input filenames
     asset_references = AssetReferences()
-    input_filenames: set[str] = set()
-    input_filenames.add(_get_hip_file())
+    asset_references.input_filenames.add(_get_hip_file())
+
     for parm, ref in hou.fileReferences():
-        if parm:
-            if parm.node() == rop_node:
-                continue
-            if ref.startswith(IGNORE_REF_VALUES):
-                continue
-            if parm.name() in IGNORE_REF_PARMS:
-                continue
-        if os.path.isdir(ref):
+        if (
+            (not parm)
+            or (parm.node() == rop_node)
+            or (ref.startswith(IGNORE_REF_VALUES))
+            or (parm.name() in IGNORE_REF_PARMS)
+        ):
             continue
-        input_filenames.add(ref)
+
+        path = parm.evalAsString()
+        if os.path.isdir(path):
+            asset_references.input_directories.add(path)
+        if os.path.isfile(path):
+            asset_references.input_filenames.add(path)
+
     rop_dir_map = {
         # Mantra/karma
         "Driver/ifd": "vm_picture",
         "Driver/karma": "picture",
         # Husk
         "Lop/usdrender_rop": _husk_outputs,
         # Arnold
@@ -80,27 +84,24 @@
         # Geo
         "Driver/geometry": "sopoutput",
         "Driver/alembic": "filename",
         "Sop/filecache": "file",
     }
     # collect output dirs for each ROP
     all_inputs = rop_node.inputAncestors()
-    output_directories: set[str] = set()
     for node in all_inputs:
         type_name = node.type().nameWithCategory()
         out_parm = rop_dir_map.get(type_name, None)
         if out_parm is not None:
             if callable(out_parm):
                 computed_dirs = out_parm(node)
-                output_directories.update(computed_dirs)
+                asset_references.output_directories.update(computed_dirs)
             else:
                 path = node.parm(out_parm).eval()
-                output_directories.add(os.path.dirname(path))
-    asset_references.input_filenames = input_filenames
-    asset_references.output_directories = output_directories
+                asset_references.output_directories.add(os.path.dirname(path))
     return asset_references
 
 
 def _get_wedge_render_node(node: hou.Node):
     """Return ROP set as input or parameter to a wedge node
 
     This ROP may have a network of input ROP nodes that will also be modified
@@ -249,24 +250,29 @@
 
 
 def _get_parameter_values(node: hou.Node) -> dict[str, Any]:
     priority = node.parm("priority").eval()
     initial_status = node.parm("initial_status").evalAsString()
     failed_tasks_limit = node.parm("failed_tasks_limit").eval()
     task_retry_limit = node.parm("task_retry_limit").eval()
-    return {
-        "parameterValues": [
-            {"name": "deadline:priority", "value": priority},
-            {"name": "deadline:targetTaskRunStatus", "value": initial_status},
-            {"name": "deadline:maxFailedTasksCount", "value": failed_tasks_limit},
-            {"name": "deadline:maxRetriesPerTask", "value": task_retry_limit},
-            {"name": "HipFile", "value": _get_hip_file()},
-            *get_queue_parameter_values_as_openjd(node),
-        ]
-    }
+    parameter_values = [
+        {"name": "deadline:priority", "value": priority},
+        {"name": "deadline:targetTaskRunStatus", "value": initial_status},
+        {"name": "deadline:maxFailedTasksCount", "value": failed_tasks_limit},
+        {"name": "deadline:maxRetriesPerTask", "value": task_retry_limit},
+        {"name": "HipFile", "value": _get_hip_file()},
+        *get_queue_parameter_values_as_openjd(node),
+    ]
+
+    if node.parm("include_adaptor_wheels").eval():
+        parameter_values.append(
+            {"name": "AdaptorWheels", "value": node.parm("adaptor_wheels").evalAsString()}
+        )
+
+    return {"parameterValues": parameter_values}
 
 
 def _is_node_locked(rop_path: str) -> bool:
     """Check rop path lineage for any locked nodes.
 
     Locked nodes can not be driven by the adaptor and must be unlocked before
     submission.
@@ -441,15 +447,14 @@
         adaptor_wheels = rop.parm("adaptor_wheels").evalAsString()
         if os.path.exists(adaptor_wheels):
             override_file = os.path.join(
                 os.path.dirname(__file__), "adaptor_override_environment.yaml"
             )
             with open(override_file) as yaml_file:
                 override_environment = yaml.safe_load(yaml_file)
-                override_environment["parameterDefinitions"][0]["default"] = str(adaptor_wheels)
                 job_template["parameterDefinitions"].extend(
                     override_environment["parameterDefinitions"]
                 )
                 if "jobEnvironments" not in job_template:
                     job_template["jobEnvironments"] = []
                 job_template["jobEnvironments"].append(override_environment["environment"])
     return job_template
@@ -639,14 +644,20 @@
         job_bundle_dir = create_job_history_bundle_dir("houdini", name)
         _create_job_bundle(node, job_bundle_dir, asset_references)
 
         farm_id = get_setting("defaults.farm_id")
         queue_id = get_setting("defaults.queue_id")
         storage_profile_id = get_setting("settings.storage_profile_id")
 
+        storage_profile = None
+        if storage_profile_id:
+            storage_profile = api.get_storage_profile_for_queue(
+                farm_id, queue_id, storage_profile_id, deadline
+            )
+
         queue = deadline.get_queue(farmId=farm_id, queueId=queue_id)
 
         queue_role_session = api.get_queue_user_boto3_session(
             deadline=deadline,
             farm_id=farm_id,
             queue_id=queue_id,
             queue_display_name=queue["displayName"],
@@ -659,15 +670,15 @@
             session=queue_role_session,
         )
 
         job_progress_dialog = SubmitJobProgressDialog(parent=hou.qt.mainWindow())
         job_progress_dialog.start_submission(
             farm_id,
             queue_id,
-            storage_profile_id,
+            storage_profile,
             job_bundle_dir,
             queue_parameters,
             asset_manager,
             deadline,
             auto_accept=str2bool(get_setting("settings.auto_accept")),
         )
     except Exception as exc:
```

### Comparing `deadline_cloud_for_houdini-0.6.0/LICENSE` & `deadline_cloud_for_houdini-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/README.md` & `deadline_cloud_for_houdini-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/hatch.toml` & `deadline_cloud_for_houdini-0.6.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.0/pyproject.toml` & `deadline_cloud_for_houdini-0.6.1/pyproject.toml`

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
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-houdini"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-houdini"
```

### Comparing `deadline_cloud_for_houdini-0.6.0/PKG-INFO` & `deadline_cloud_for_houdini-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-houdini
-Version: 0.6.0
+Version: 0.6.1
 Summary: AWS Deadline Cloud for Houdini
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-houdini
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
 
 # AWS Deadline Cloud for Houdini
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-houdini.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-houdini)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-houdini.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-houdini)
```

