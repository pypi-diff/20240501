# Comparing `tmp/apache_airflow_providers_openai-1.1.0rc1.tar.gz` & `tmp/apache_airflow_providers_openai-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openai-1.1.0rc1.tar", last modified: Thu Dec  7 21:10:00 2023, max compression
+gzip compressed data, was "apache_airflow_providers_openai-1.2.0rc1.tar", last modified: Tue Apr 30 11:36:12 2024, max compression
```

## Comparing `apache_airflow_providers_openai-1.1.0rc1.tar` & `apache_airflow_providers_openai-1.2.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3073 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/LICENSE
--rw-r--r--   0        0        0     1581 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/__init__.py
--rw-r--r--   0        0        0     2268 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/get_provider_info.py
--rw-r--r--   0        0        0      785 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/hooks/__init__.py
--rw-r--r--   0        0        0     3221 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/hooks/openai.py
--rw-r--r--   0        0        0      785 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/operators/__init__.py
--rw-r--r--   0        0        0     3200 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/operators/openai.py
--rw-r--r--   0        0        0     2925 2023-12-07 21:10:00.000000 apache_airflow_providers_openai-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 apache_airflow_providers_openai-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3079 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/LICENSE
+-rw-r--r--   0        0        0     1581 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/hooks/__init__.py
+-rw-r--r--   0        0        0    14796 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/hooks/openai.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/operators/__init__.py
+-rw-r--r--   0        0        0     3200 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/operators/openai.py
+-rw-r--r--   0        0        0     2970 2024-04-30 11:36:12.000000 apache_airflow_providers_openai-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 apache_airflow_providers_openai-1.2.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openai-1.1.0rc1/README.rst` & `apache_airflow_providers_openai-1.2.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,43 +38,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openai``
 
-Release: ``1.1.0.rc1``
+Release: ``1.2.0.rc1``
 
 
 `OpenAI <https://platform.openai.com/docs/introduction>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openai`` provider. All classes for this provider package
 are in ``airflow.providers.openai`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openai``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.6.0``
-``openai[datalib]``  ``>=1.0``
+``apache-airflow``   ``>=2.7.0``
+``openai[datalib]``  ``>=1.23``
 ===================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/LICENSE` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/__init__.py` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.6.0"
+    "2.7.0"
 ):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-openai:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-openai:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/get_provider_info.py` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/get_provider_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openai",
         "name": "OpenAI",
         "description": "`OpenAI <https://platform.openai.com/docs/introduction>`__\n",
-        "suspended": False,
-        "source-date-epoch": 1701983400,
-        "versions": ["1.1.0", "1.0.1", "1.0.0"],
+        "state": "ready",
+        "source-date-epoch": 1714476972,
+        "versions": ["1.2.0", "1.1.0", "1.0.1", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "OpenAI",
                 "external-doc-url": "https://platform.openai.com/docs/introduction",
                 "how-to-guide": ["/docs/apache-airflow-providers-openai/operators/openai.rst"],
                 "tags": ["software"],
             }
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "openai[datalib]>=1.0"],
+        "dependencies": ["apache-airflow>=2.7.0", "openai[datalib]>=1.23"],
         "hooks": [
             {"integration-name": "OpenAI", "python-modules": ["airflow.providers.openai.hooks.openai"]}
         ],
         "operators": [
             {"integration-name": "OpenAI", "python-modules": ["airflow.providers.openai.operators.openai"]}
         ],
         "connection-types": [
```

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/hooks/__init__.py` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/operators/__init__.py` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openai-1.1.0rc1/airflow/providers/openai/operators/openai.py` & `apache_airflow_providers_openai-1.2.0rc1/airflow/providers/openai/operators/openai.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openai-1.1.0rc1/pyproject.toml` & `apache_airflow_providers_openai-1.2.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openai"
-version = "1.1.0.rc1"
+version = "1.2.0.rc1"
 description = "Provider package apache-airflow-providers-openai for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,25 +47,26 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
-    "openai[datalib]>=1.0",
+    "apache-airflow>=2.7.0rc0",
+    "openai[datalib]>=1.23",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_openai-1.1.0rc1/PKG-INFO` & `apache_airflow_providers_openai-1.2.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openai
-Version: 1.1.0rc1
+Version: 1.2.0rc1
 Summary: Provider package apache-airflow-providers-openai for Apache Airflow
 Keywords: airflow-provider,openai,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,21 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
-Requires-Dist: openai[datalib]>=1.0
+Requires-Dist: apache-airflow>=2.7.0rc0
+Requires-Dist: openai[datalib]>=1.23
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -70,43 +71,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openai``
 
-Release: ``1.1.0.rc1``
+Release: ``1.2.0.rc1``
 
 
 `OpenAI <https://platform.openai.com/docs/introduction>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openai`` provider. All classes for this provider package
 are in ``airflow.providers.openai`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openai``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.6.0``
-``openai[datalib]``  ``>=1.0``
+``apache-airflow``   ``>=2.7.0``
+``openai[datalib]``  ``>=1.23``
 ===================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openai/1.2.0/changelog.html>`_.
```
