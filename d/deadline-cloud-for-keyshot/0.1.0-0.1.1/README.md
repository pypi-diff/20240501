# Comparing `tmp/deadline_cloud_for_keyshot-0.1.0.tar.gz` & `tmp/deadline_cloud_for_keyshot-0.1.1.tar.gz`

## Comparing `deadline_cloud_for_keyshot-0.1.0.tar` & `deadline_cloud_for_keyshot-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/KeyShotAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py
--rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotClient/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/_version.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/data_classes.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/keyshot_render_submitter.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/NOTICE
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/hatch.toml
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/KeyShotAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py
+-rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/_version.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/data_classes.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/keyshot_render_submitter.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/NOTICE
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/hatch.toml
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/PKG-INFO
```

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/__main__.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 import sys
 import os
 
 # Retrieve the value of the environment variable DEADLINE_KEYSHOT that was
-# passed as part of subprocess.run() in DeadlineCloudSubmitter.py
+# passed as part of subprocess.run() in "Submit to AWS Deadline Cloud.py"
 deadline_keyshot = sys.argv[-2]
 
 if not deadline_keyshot:
     raise Exception("deadline submitter not found")
 
 deadline_keyshot_path = os.path.dirname(deadline_keyshot)
 if deadline_keyshot_path not in sys.path:
@@ -16,9 +16,9 @@
 
 if __name__ == "__main__":
     from keyshot_submitter.keyshot_render_submitter import (  #  type: ignore
         show_submitter,
     )
 
     # Launch the submitter using the info file passed from the call to
-    # subprocess.run() in DeadlineCloudSubmitter.py
+    # subprocess.run() in "Submit to AWS Deadline Cloud.py"
     show_submitter(sys.argv[-1])
```

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/data_classes.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/keyshot_render_submitter.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/keyshot_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/LICENSE` & `deadline_cloud_for_keyshot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/README.md` & `deadline_cloud_for_keyshot-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ## Submitter
 
 This package provides a KeyShot plugin script that creates jobs for AWS Deadline Cloud using the [AWS Deadline Cloud client library][deadline-cloud-client]. Based on the loaded scene it determines the files required, allows the user to specify render options with KeyShot's render interface, and builds an [OpenJD template][openjd] that defines the workflow.
 
 ### Using the KeyShot Submitter
 
 1. Install deadline-cloud and PySide2
-2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/DeadlineCloudSubmitter.py` to the KeyShot scripts folder.
+2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/Submit to AWS Deadline Cloud.py` to the KeyShot scripts folder.
     - e.g. On Windows `C:/Users/<USER>/Documents/KeyShot 12/Scripts`
 3. Set the following environment variables
     - Set the environment variable `DEADLINE_PYTHON` as the path to the Python installation where deadline-cloud and PySide2 were installed in step 1.
       - e.g. On Windows if using Python 3.10 it might be `set DEADLINE_PYTHON=C:/Users/<USER>/AppData/Local/Programs/Python/Python310/python`
     - Set the environment variable `DEADLINE_KEYSHOT` as the path to the `<PATH TO>/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter` folder
       - e.g. On Windows if the source was on the user's desktop it might be  `set DEADLINE_KEYSHOT=C:/Users/<USER>/Desktop/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter`
 4. Launch KeyShot with the environment variables from step 3. set.
```

### Comparing `deadline_cloud_for_keyshot-0.1.0/hatch.toml` & `deadline_cloud_for_keyshot-0.1.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.0/pyproject.toml` & `deadline_cloud_for_keyshot-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
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
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-keyshot"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-keyshot"
```

### Comparing `deadline_cloud_for_keyshot-0.1.0/PKG-INFO` & `deadline_cloud_for_keyshot-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-keyshot
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Deadline Cloud for KeyShot
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-keyshot
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-keyshot
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
 
 # AWS Deadline Cloud for KeyShot
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-keyshot.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-keyshot)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-keyshot.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-keyshot)
@@ -49,15 +49,15 @@
 ## Submitter
 
 This package provides a KeyShot plugin script that creates jobs for AWS Deadline Cloud using the [AWS Deadline Cloud client library][deadline-cloud-client]. Based on the loaded scene it determines the files required, allows the user to specify render options with KeyShot's render interface, and builds an [OpenJD template][openjd] that defines the workflow.
 
 ### Using the KeyShot Submitter
 
 1. Install deadline-cloud and PySide2
-2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/DeadlineCloudSubmitter.py` to the KeyShot scripts folder.
+2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/Submit to AWS Deadline Cloud.py` to the KeyShot scripts folder.
     - e.g. On Windows `C:/Users/<USER>/Documents/KeyShot 12/Scripts`
 3. Set the following environment variables
     - Set the environment variable `DEADLINE_PYTHON` as the path to the Python installation where deadline-cloud and PySide2 were installed in step 1.
       - e.g. On Windows if using Python 3.10 it might be `set DEADLINE_PYTHON=C:/Users/<USER>/AppData/Local/Programs/Python/Python310/python`
     - Set the environment variable `DEADLINE_KEYSHOT` as the path to the `<PATH TO>/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter` folder
       - e.g. On Windows if the source was on the user's desktop it might be  `set DEADLINE_KEYSHOT=C:/Users/<USER>/Desktop/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter`
 4. Launch KeyShot with the environment variables from step 3. set.
```

