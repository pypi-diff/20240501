# Comparing `tmp/dummyML-0.9.4.dev0.tar.gz` & `tmp/dummyml-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummyML-0.9.4.dev0.tar", last modified: Tue Nov 29 02:08:41 2022, max compression
+gzip compressed data, was "dummyml-0.9.5.tar", last modified: Wed May  1 06:09:35 2024, max compression
```

## Comparing `dummyML-0.9.4.dev0.tar` & `dummyml-0.9.5.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1073 2021-08-31 02:36:50.000000 dummyML-0.9.4.dev0/LICENSE.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      183 2021-08-31 02:36:50.000000 dummyML-0.9.4.dev0/MANIFEST.in
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1699 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/PKG-INFO
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      977 2022-11-29 00:56:20.000000 dummyML-0.9.4.dev0/README.md
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2021-12-03 04:35:32.000000 dummyML-0.9.4.dev0/TODO.md
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      103 2021-08-31 02:36:50.000000 dummyML-0.9.4.dev0/pyproject.toml
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)       38 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/setup.cfg
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1419 2022-11-29 00:58:45.000000 dummyML-0.9.4.dev0/setup.py
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.637085 dummyML-0.9.4.dev0/src/
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.637085 dummyML-0.9.4.dev0/src/dummyML/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)       40 2022-11-24 05:03:26.000000 dummyML-0.9.4.dev0/src/dummyML/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    10219 2022-11-29 00:18:52.000000 dummyML-0.9.4.dev0/src/dummyML/automate_analysis.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11477 2022-11-28 22:39:56.000000 dummyML-0.9.4.dev0/src/dummyML/automate_modeling_evaluation.py
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/src/dummyML/evaluate_models/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyML-0.9.4.dev0/src/dummyML/evaluate_models/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8836 2022-11-25 04:29:13.000000 dummyML-0.9.4.dev0/src/dummyML/evaluate_models/classification_metrics.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8644 2022-11-28 21:06:48.000000 dummyML-0.9.4.dev0/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3458 2022-11-24 04:56:55.000000 dummyML-0.9.4.dev0/src/dummyML/evaluate_models/regression_metrics.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8673 2022-11-24 05:03:07.000000 dummyML-0.9.4.dev0/src/dummyML/preprocessing.py
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/src/dummyML/select_fit_models/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyML-0.9.4.dev0/src/dummyML/select_fit_models/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    29719 2022-11-24 05:03:54.000000 dummyML-0.9.4.dev0/src/dummyML/select_fit_models/classification_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11845 2022-11-24 05:05:42.000000 dummyML-0.9.4.dev0/src/dummyML/select_fit_models/imbalanced_classification_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    23287 2022-11-24 05:05:48.000000 dummyML-0.9.4.dev0/src/dummyML/select_fit_models/regression_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11534 2022-11-24 04:56:55.000000 dummyML-0.9.4.dev0/src/dummyML/utilities.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)       94 2022-11-24 05:03:34.000000 dummyML-0.9.4.dev0/src/dummyML/version.py
-drwxr-xr-x   0 yipeng    (1000) yipeng    (1000)        0 2022-11-29 02:08:41.640418 dummyML-0.9.4.dev0/src/dummyML.egg-info/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1699 2022-11-29 02:08:41.000000 dummyML-0.9.4.dev0/src/dummyML.egg-info/PKG-INFO
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      840 2022-11-29 02:08:41.000000 dummyML-0.9.4.dev0/src/dummyML.egg-info/SOURCES.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2022-11-29 02:08:41.000000 dummyML-0.9.4.dev0/src/dummyML.egg-info/dependency_links.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      127 2022-11-29 02:08:41.000000 dummyML-0.9.4.dev0/src/dummyML.egg-info/requires.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        8 2022-11-29 02:08:41.000000 dummyML-0.9.4.dev0/src/dummyML.egg-info/top_level.txt
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.409978 dummyml-0.9.5/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1073 2021-08-31 02:36:50.000000 dummyml-0.9.5/LICENSE.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      183 2021-08-31 02:36:50.000000 dummyml-0.9.5/MANIFEST.in
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1985 2024-05-01 06:09:35.409978 dummyml-0.9.5/PKG-INFO
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      975 2024-05-01 05:08:30.000000 dummyml-0.9.5/README.md
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2021-12-03 04:35:32.000000 dummyml-0.9.5/TODO.md
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      103 2021-08-31 02:36:50.000000 dummyml-0.9.5/pyproject.toml
+-rw-rw-r--   0 yipeng    (1000) yipeng    (1000)       38 2024-05-01 06:09:35.409978 dummyml-0.9.5/setup.cfg
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1469 2024-05-01 06:08:50.000000 dummyml-0.9.5/setup.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.405978 dummyml-0.9.5/src/
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.405978 dummyml-0.9.5/src/dummyML/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)       40 2022-11-24 05:03:26.000000 dummyml-0.9.5/src/dummyML/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    10219 2022-11-29 00:18:52.000000 dummyml-0.9.5/src/dummyML/automate_analysis.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11477 2022-11-28 22:39:56.000000 dummyml-0.9.5/src/dummyML/automate_modeling_evaluation.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.409978 dummyml-0.9.5/src/dummyML/evaluate_models/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.5/src/dummyML/evaluate_models/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8836 2022-11-25 04:29:13.000000 dummyml-0.9.5/src/dummyML/evaluate_models/classification_metrics.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8644 2022-11-28 21:06:48.000000 dummyml-0.9.5/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3458 2022-11-24 04:56:55.000000 dummyml-0.9.5/src/dummyML/evaluate_models/regression_metrics.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8673 2022-11-24 05:03:07.000000 dummyml-0.9.5/src/dummyML/preprocessing.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.409978 dummyml-0.9.5/src/dummyML/select_fit_models/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.5/src/dummyML/select_fit_models/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    29719 2022-11-24 05:03:54.000000 dummyml-0.9.5/src/dummyML/select_fit_models/classification_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11845 2022-11-24 05:05:42.000000 dummyml-0.9.5/src/dummyML/select_fit_models/imbalanced_classification_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    23287 2022-11-24 05:05:48.000000 dummyml-0.9.5/src/dummyML/select_fit_models/regression_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11534 2022-11-24 04:56:55.000000 dummyml-0.9.5/src/dummyML/utilities.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)       94 2022-11-24 05:03:34.000000 dummyml-0.9.5/src/dummyML/version.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.409978 dummyml-0.9.5/src/dummyML.egg-info/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1985 2024-05-01 06:09:35.000000 dummyml-0.9.5/src/dummyML.egg-info/PKG-INFO
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      924 2024-05-01 06:09:35.000000 dummyml-0.9.5/src/dummyML.egg-info/SOURCES.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2024-05-01 06:09:35.000000 dummyml-0.9.5/src/dummyML.egg-info/dependency_links.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      174 2024-05-01 06:09:35.000000 dummyml-0.9.5/src/dummyML.egg-info/requires.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        8 2024-05-01 06:09:35.000000 dummyml-0.9.5/src/dummyML.egg-info/top_level.txt
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:09:35.409978 dummyml-0.9.5/tests/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3918 2022-11-29 00:53:33.000000 dummyml-0.9.5/tests/test_automate_analysis.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1397 2022-11-29 00:54:22.000000 dummyml-0.9.5/tests/test_preprocessing.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1514 2022-11-29 00:54:36.000000 dummyml-0.9.5/tests/test_utilities.py
```

### Comparing `dummyML-0.9.4.dev0/LICENSE.txt` & `dummyml-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/PKG-INFO` & `dummyml-0.9.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: dummyML
-Version: 0.9.4.dev0
+Version: 0.9.5
 Summary: Automated data analysis pipelines on tabular data for data analyst
 Home-page: https://gitlab.com/YipengUva/dummyML_pkg
 Author: Yipeng Song
 Author-email: yipeng.song@hotmail.com
 Project-URL: Bug Tracker, https://gitlab.com/YipengUva/dummyML_pkg/issues
 Keywords: data analysis,machine learning,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy<=1.26,>=1.19
+Requires-Dist: pandas<=1.5,>=1.1
+Requires-Dist: imbalanced-learn<=0.10,>=0.8
+Requires-Dist: scikit-learn<=1.2,>=1.0
+Requires-Dist: pandas-profiling<=3.3,>=2.9
+Requires-Dist: joblib<=1.2,>=1.0
+Requires-Dist: xgboost<=1.5,>=1.4
+Requires-Dist: optuna<=2.10,>=2.7
 
 # dummyML package
 
 The dummyML Python package is designed for data analysts to do automated data analysis on tabular data using machine learning algorithms. The package implemented all the components, data preprocessing, data splitting, model selection, model fitting and model evaluation, required for defining pipelines to automatically analyze tabular data. 
 
 ### Installation
 
@@ -26,13 +34,12 @@
 
 ```
 pip install dummyML
 ```
 
 on the command line of a Linux system or the Anaconda Prompt on a Windows system. If you don't have root privileges, sometimes you need to add `--user` after the above commands, then pip will install the package in your home directory.
 
-If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.3 by `pip install dummyML==0.9.3`. 
+If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.5 by `pip install dummyML==0.9.5`.
 
 ### User guide
 
 The user guide is available at https://dummyml.readthedocs.io/en/latest/.
-
```

### Comparing `dummyML-0.9.4.dev0/README.md` & `dummyml-0.9.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,12 @@
 
 ```
 pip install dummyML
 ```
 
 on the command line of a Linux system or the Anaconda Prompt on a Windows system. If you don't have root privileges, sometimes you need to add `--user` after the above commands, then pip will install the package in your home directory.
 
-If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.3 by `pip install dummyML==0.9.3`. 
+If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.5 by `pip install dummyML==0.9.5`.
 
 ### User guide
 
 The user guide is available at https://dummyml.readthedocs.io/en/latest/.
-
```

### Comparing `dummyML-0.9.4.dev0/src/dummyML/automate_analysis.py` & `dummyml-0.9.5/src/dummyML/automate_analysis.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/automate_modeling_evaluation.py` & `dummyml-0.9.5/src/dummyML/automate_modeling_evaluation.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/evaluate_models/classification_metrics.py` & `dummyml-0.9.5/src/dummyML/evaluate_models/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py` & `dummyml-0.9.5/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/evaluate_models/regression_metrics.py` & `dummyml-0.9.5/src/dummyML/evaluate_models/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/preprocessing.py` & `dummyml-0.9.5/src/dummyML/preprocessing.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/select_fit_models/classification_models.py` & `dummyml-0.9.5/src/dummyML/select_fit_models/classification_models.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/select_fit_models/imbalanced_classification_models.py` & `dummyml-0.9.5/src/dummyML/select_fit_models/imbalanced_classification_models.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/select_fit_models/regression_models.py` & `dummyml-0.9.5/src/dummyML/select_fit_models/regression_models.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML/utilities.py` & `dummyml-0.9.5/src/dummyML/utilities.py`

 * *Files identical despite different names*

### Comparing `dummyML-0.9.4.dev0/src/dummyML.egg-info/PKG-INFO` & `dummyml-0.9.5/src/dummyML.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: dummyML
-Version: 0.9.4.dev0
+Version: 0.9.5
 Summary: Automated data analysis pipelines on tabular data for data analyst
 Home-page: https://gitlab.com/YipengUva/dummyML_pkg
 Author: Yipeng Song
 Author-email: yipeng.song@hotmail.com
 Project-URL: Bug Tracker, https://gitlab.com/YipengUva/dummyML_pkg/issues
 Keywords: data analysis,machine learning,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy<=1.26,>=1.19
+Requires-Dist: pandas<=1.5,>=1.1
+Requires-Dist: imbalanced-learn<=0.10,>=0.8
+Requires-Dist: scikit-learn<=1.2,>=1.0
+Requires-Dist: pandas-profiling<=3.3,>=2.9
+Requires-Dist: joblib<=1.2,>=1.0
+Requires-Dist: xgboost<=1.5,>=1.4
+Requires-Dist: optuna<=2.10,>=2.7
 
 # dummyML package
 
 The dummyML Python package is designed for data analysts to do automated data analysis on tabular data using machine learning algorithms. The package implemented all the components, data preprocessing, data splitting, model selection, model fitting and model evaluation, required for defining pipelines to automatically analyze tabular data. 
 
 ### Installation
 
@@ -26,13 +34,12 @@
 
 ```
 pip install dummyML
 ```
 
 on the command line of a Linux system or the Anaconda Prompt on a Windows system. If you don't have root privileges, sometimes you need to add `--user` after the above commands, then pip will install the package in your home directory.
 
-If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.3 by `pip install dummyML==0.9.3`. 
+If you want to install a specific version, please visit https://pypi.org/project/dummyML/ to find the exact version number. For example, you can install version 0.9.5 by `pip install dummyML==0.9.5`.
 
 ### User guide
 
 The user guide is available at https://dummyml.readthedocs.io/en/latest/.
-
```

### Comparing `dummyML-0.9.4.dev0/src/dummyML.egg-info/SOURCES.txt` & `dummyml-0.9.5/src/dummyML.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 src/dummyML/evaluate_models/__init__.py
 src/dummyML/evaluate_models/classification_metrics.py
 src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py
 src/dummyML/evaluate_models/regression_metrics.py
 src/dummyML/select_fit_models/__init__.py
 src/dummyML/select_fit_models/classification_models.py
 src/dummyML/select_fit_models/imbalanced_classification_models.py
-src/dummyML/select_fit_models/regression_models.py
+src/dummyML/select_fit_models/regression_models.py
+tests/test_automate_analysis.py
+tests/test_preprocessing.py
+tests/test_utilities.py
```

