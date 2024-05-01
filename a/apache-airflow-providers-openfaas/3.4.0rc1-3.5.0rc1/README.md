# Comparing `tmp/apache_airflow_providers_openfaas-3.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_openfaas-3.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openfaas-3.4.0rc1.tar", last modified: Thu Dec  7 21:10:01 2023, max compression
+gzip compressed data, was "apache_airflow_providers_openfaas-3.5.0rc1.tar", last modified: Tue Apr 30 11:36:57 2024, max compression
```

## Comparing `apache_airflow_providers_openfaas-3.4.0rc1.tar` & `apache_airflow_providers_openfaas-3.5.0rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3031 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/LICENSE
--rw-r--r--   0        0        0     1583 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/__init__.py
--rw-r--r--   0        0        0     2104 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/get_provider_info.py
--rw-r--r--   0        0        0      787 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/hooks/__init__.py
--rw-r--r--   0        0        0     4890 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/hooks/openfaas.py
--rw-r--r--   0        0        0     2911 2023-12-07 21:10:01.000000 apache_airflow_providers_openfaas-3.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4652 1970-01-01 00:00:00.000000 apache_airflow_providers_openfaas-3.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3036 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/__init__.py
+-rw-r--r--   0        0        0     2123 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/hooks/__init__.py
+-rw-r--r--   0        0        0     4891 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/hooks/openfaas.py
+-rw-r--r--   0        0        0     2955 2024-04-30 11:36:57.000000 apache_airflow_providers_openfaas-3.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 apache_airflow_providers_openfaas-3.5.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/README.rst` & `apache_airflow_providers_openfaas-3.5.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,42 +38,42 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.4.0.rc1``
+Release: ``3.5.0.rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openfaas`` provider. All classes for this provider package
 are in ``airflow.providers.openfaas`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openfaas``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/LICENSE` & `apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/__init__.py` & `apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.6.0"
+    "2.7.0"
 ):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-openfaas:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-openfaas:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/get_provider_info.py` & `apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,32 +23,33 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openfaas",
         "name": "OpenFaaS",
         "description": "`OpenFaaS <https://www.openfaas.com/>`__\n",
-        "suspended": False,
-        "source-date-epoch": 1701983401,
+        "state": "ready",
+        "source-date-epoch": 1714477017,
         "versions": [
+            "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.1.1",
             "1.1.0",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0"],
+        "dependencies": ["apache-airflow>=2.7.0"],
         "integrations": [
             {
                 "integration-name": "OpenFaaS",
                 "external-doc-url": "https://www.openfaas.com/",
                 "logo": "/integration-logos/openfaas/OpenFaaS.png",
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/hooks/__init__.py` & `apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/airflow/providers/openfaas/hooks/openfaas.py` & `apache_airflow_providers_openfaas-3.5.0rc1/airflow/providers/openfaas/hooks/openfaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,26 @@
                 self.log.error("Response status %d", response.status_code)
                 self.log.error("Failed to deploy")
                 raise AirflowException("failed to deploy")
             else:
                 self.log.info("Function deployed %s", self.function_name)
 
     def invoke_async_function(self, body: dict[str, Any]) -> None:
-        """Invoking function asynchronously."""
+        """Invoke function asynchronously."""
         url = self.get_conn().host + self.INVOKE_ASYNC_FUNCTION + self.function_name
         self.log.info("Invoking function asynchronously %s", url)
         response = requests.post(url, body)
         if response.ok:
             self.log.info("Invoked %s", self.function_name)
         else:
             self.log.error("Response status %d", response.status_code)
             raise AirflowException("failed to invoke function")
 
     def invoke_function(self, body: dict[str, Any]) -> None:
-        """Invoking function synchronously, will block until function completes and returns."""
+        """Invoke function synchronously. This will block until function completes and returns."""
         url = self.get_conn().host + self.INVOKE_FUNCTION + self.function_name
         self.log.info("Invoking function synchronously %s", url)
         response = requests.post(url, body)
         if response.ok:
             self.log.info("Invoked %s", self.function_name)
             self.log.info("Response code %s", response.status_code)
             self.log.info("Response %s", response.text)
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/pyproject.toml` & `apache_airflow_providers_openfaas-3.5.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openfaas"
-version = "3.4.0.rc1"
+version = "3.5.0.rc1"
 description = "Provider package apache-airflow-providers-openfaas for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,24 +47,25 @@
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
+    "apache-airflow>=2.7.0rc0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_openfaas-3.4.0rc1/PKG-INFO` & `apache_airflow_providers_openfaas-3.5.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openfaas
-Version: 3.4.0rc1
+Version: 3.5.0rc1
 Summary: Provider package apache-airflow-providers-openfaas for Apache Airflow
 Keywords: airflow-provider,openfaas,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,20 @@
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
+Requires-Dist: apache-airflow>=2.7.0rc0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -69,42 +70,42 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.4.0.rc1``
+Release: ``3.5.0.rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openfaas`` provider. All classes for this provider package
 are in ``airflow.providers.openfaas`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openfaas``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.5.0/changelog.html>`_.
```

