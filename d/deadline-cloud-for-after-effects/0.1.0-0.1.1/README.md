# Comparing `tmp/deadline_cloud_for_after_effects-0.1.0.tar.gz` & `tmp/deadline_cloud_for_after_effects-0.1.1.tar.gz`

## Comparing `deadline_cloud_for_after_effects-0.1.0.tar` & `deadline_cloud_for_after_effects-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/_version.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/AEAdaptor.json
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/__init__.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/__main__.py
--rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/py.typed
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/__init__.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ae_client.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ae_handler.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ipc.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/NOTICE
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/hatch.toml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/_version.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/AEAdaptor.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__init__.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__main__.py
+-rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/py.typed
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/__init__.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_client.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_handler.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ipc.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/NOTICE
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/hatch.toml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 deadline_cloud_for_after_effects-0.1.1/PKG-INFO
```

### Comparing `deadline_cloud_for_after_effects-0.1.0/hatch_custom_hook.py` & `deadline_cloud_for_after_effects-0.1.1/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/__main__.py` & `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEAdaptor/adaptor.py` & `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ae_client.py` & `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ae_handler.py` & `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ae_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/src/deadline/ae_adaptor/AEClient/ipc.py` & `deadline_cloud_for_after_effects-0.1.1/src/deadline/ae_adaptor/AEClient/ipc.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/LICENSE` & `deadline_cloud_for_after_effects-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/README.md` & `deadline_cloud_for_after_effects-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/hatch.toml` & `deadline_cloud_for_after_effects-0.1.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_after_effects-0.1.0/pyproject.toml` & `deadline_cloud_for_after_effects-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Operating System :: MacOS",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
 ]
 
 dependencies = [
-  "deadline == 0.47.*",
+  "deadline == 0.48.*",
   "openjd-adaptor-runtime == 0.7.*"
 ]
 
 [project.scripts]
 afterfx-openjd = "deadline.ae_adaptor.AEAdaptor:main"
 
 [project.urls]
```

### Comparing `deadline_cloud_for_after_effects-0.1.0/PKG-INFO` & `deadline_cloud_for_after_effects-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-after-effects
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Deadline Cloud for After Effects
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-after-effects
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-after-effects
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -17,15 +17,15 @@
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
 
 # AWS Deadline Cloud for After Effects
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-after-effects.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-after-effects)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-after-effects.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-after-effects)
```

