# Comparing `tmp/deadline_cloud_for_rhino-0.1.2.tar.gz` & `tmp/deadline_cloud_for_rhino-0.1.3.tar.gz`

## Comparing `deadline_cloud_for_rhino-0.1.2.tar` & `deadline_cloud_for_rhino-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/_version.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/_version.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/data_classes.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/default_rhino_job_template.yaml
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/rhino_render_submitter.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/.gitignore
--rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/NOTICE
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/hatch.toml
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/_version.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/_version.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/data_classes.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/default_rhino_job_template.yaml
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/rhino_render_submitter.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/.gitignore
+-rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/LICENSE
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/NOTICE
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/hatch.toml
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 deadline_cloud_for_rhino-0.1.3/PKG-INFO
```

### Comparing `deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/data_classes.py` & `deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/default_rhino_job_template.yaml` & `deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/default_rhino_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/rhino_render_submitter.py` & `deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/rhino_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_rhino-0.1.3/src/deadline/rhino_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/LICENSE` & `deadline_cloud_for_rhino-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/README.md` & `deadline_cloud_for_rhino-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/hatch.toml` & `deadline_cloud_for_rhino-0.1.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_rhino-0.1.2/pyproject.toml` & `deadline_cloud_for_rhino-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop"
 ]
 # Rhino 8 - 3.9
 
 dependencies = [
-    "deadline == 0.47.*",
+    "deadline == 0.48.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-rhino"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-rhino"
 
 [tool.hatch.build]
```

### Comparing `deadline_cloud_for_rhino-0.1.2/PKG-INFO` & `deadline_cloud_for_rhino-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-rhino
-Version: 0.1.2
+Version: 0.1.3
 Summary: AWS Deadline Cloud for Rhino
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-rhino
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-rhino
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
 Description-Content-Type: text/markdown
 
 # AWS Deadline Cloud for Rhino
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-rhino.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-rhino)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-rhino.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-rhino)
 [![license](https://img.shields.io/pypi/l/deadline-cloud-for-rhino.svg?style=flat)](https://github.com/aws-deadline/deadline-cloud-for-rhino/blob/mainline/LICENSE)
```

