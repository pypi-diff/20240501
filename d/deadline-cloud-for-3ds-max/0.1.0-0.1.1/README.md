# Comparing `tmp/deadline_cloud_for_3ds_max-0.1.0.tar.gz` & `tmp/deadline_cloud_for_3ds_max-0.1.1.tar.gz`

## Comparing `deadline_cloud_for_3ds_max-0.1.0.tar` & `deadline_cloud_for_3ds_max-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/_version.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/MaxAdaptor.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/__main__.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/py.typed
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/__init__.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/max_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/py.typed
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/art_handler.py
--rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/default_max_handler.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/_version.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0    16741 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/create_job_bundle.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/data_classes.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/data_const.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/default_max_job_template.yaml
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/job_bundle_output_test_runner.py
--rw-r--r--   0        0        0    13847 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/max_render_submitter.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/run_ui.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/sanity_checks.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/ui/__init__.py
--rw-r--r--   0        0        0    21998 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/ui/scene_settings_tab.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/ui/submit_dialog.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/__init__.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/log_utils.py
--rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/max_utils.py
--rw-r--r--   0        0        0    18819 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/submission_utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/NOTICE
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/README.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/hatch.toml
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/_version.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/MaxAdaptor.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/__main__.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/py.typed
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/__init__.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/max_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/py.typed
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/art_handler.py
+-rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/default_max_handler.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/_version.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0    16741 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/create_job_bundle.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/data_classes.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/data_const.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/default_max_job_template.yaml
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/job_bundle_output_test_runner.py
+-rw-r--r--   0        0        0    13847 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/max_render_submitter.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/run_ui.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/sanity_checks.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/ui/__init__.py
+-rw-r--r--   0        0        0    21998 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/ui/scene_settings_tab.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/ui/submit_dialog.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/__init__.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/log_utils.py
+-rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/max_utils.py
+-rw-r--r--   0        0        0    18819 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/submission_utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/NOTICE
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/README.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/hatch.toml
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 deadline_cloud_for_3ds_max-0.1.1/PKG-INFO
```

### Comparing `deadline_cloud_for_3ds_max-0.1.0/hatch_custom_hook.py` & `deadline_cloud_for_3ds_max-0.1.1/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/__main__.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/adaptor.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/max_client.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/max_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/__init__.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/art_handler.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/art_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_adaptor/MaxClient/render_handlers/default_max_handler.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_adaptor/MaxClient/render_handlers/default_max_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/create_job_bundle.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/create_job_bundle.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/data_classes.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/data_const.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/data_const.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/default_max_job_template.yaml` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/default_max_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/job_bundle_output_test_runner.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/job_bundle_output_test_runner.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/max_render_submitter.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/max_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/run_ui.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/run_ui.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/sanity_checks.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/ui/scene_settings_tab.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/ui/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/ui/submit_dialog.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/ui/submit_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/log_utils.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/log_utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/max_utils.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/max_utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/src/deadline/max_submitter/utilities/submission_utils.py` & `deadline_cloud_for_3ds_max-0.1.1/src/deadline/max_submitter/utilities/submission_utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/LICENSE` & `deadline_cloud_for_3ds_max-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/README.md` & `deadline_cloud_for_3ds_max-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/hatch.toml` & `deadline_cloud_for_3ds_max-0.1.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_3ds_max-0.1.0/pyproject.toml` & `deadline_cloud_for_3ds_max-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Intended Audience :: End Users/Desktop",
 ]
 # Python versions:
 # 2023 - 3.9: https://help.autodesk.com/view/MAXDEV/2023/ENU/?guid=MAXDEV_Python_about_the_3ds_max_python_api_html
 # 2024 - 3.9: https://help.autodesk.com/view/MAXDEV/2024/ENU/?guid=MAXDEV_Python_about_the_3ds_max_python_api_html
 
 dependencies = [
-    "deadline == 0.47.*", 
+    "deadline == 0.48.*",
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-3ds-max"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-3ds-max"
```

### Comparing `deadline_cloud_for_3ds_max-0.1.0/PKG-INFO` & `deadline_cloud_for_3ds_max-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-3ds-max
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Deadline Cloud for 3ds Max
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-3ds-max
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-3ds-max
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -16,15 +16,15 @@
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
 
 # AWS Deadline Cloud for 3ds Max
 
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-3ds-max.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-3ds-max)
```

