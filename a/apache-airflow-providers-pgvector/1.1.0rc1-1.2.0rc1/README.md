# Comparing `tmp/apache_airflow_providers_pgvector-1.1.0rc1.tar.gz` & `tmp/apache_airflow_providers_pgvector-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_pgvector-1.1.0rc1.tar", last modified: Thu Dec  7 21:10:06 2023, max compression
+gzip compressed data, was "apache_airflow_providers_pgvector-1.2.0rc1.tar", last modified: Tue Apr 30 11:39:52 2024, max compression
```

## Comparing `apache_airflow_providers_pgvector-1.1.0rc1.tar` & `apache_airflow_providers_pgvector-1.2.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4396 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/LICENSE
--rw-r--r--   0        0        0     1583 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/__init__.py
--rw-r--r--   0        0        0     2197 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/get_provider_info.py
--rw-r--r--   0        0        0     1053 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/hooks/__init__.py
--rw-r--r--   0        0        0     3367 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/hooks/pgvector.py
--rw-r--r--   0        0        0     1053 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/operators/__init__.py
--rw-r--r--   0        0        0     1876 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/operators/pgvector.py
--rw-r--r--   0        0        0     3139 2023-12-07 21:10:06.000000 apache_airflow_providers_pgvector-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 apache_airflow_providers_pgvector-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4401 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/__init__.py
+-rw-r--r--   0        0        0     2204 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/get_provider_info.py
+-rw-r--r--   0        0        0     1053 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/hooks/__init__.py
+-rw-r--r--   0        0        0     3367 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/hooks/pgvector.py
+-rw-r--r--   0        0        0     1053 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/operators/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/operators/pgvector.py
+-rw-r--r--   0        0        0     3181 2024-04-30 11:39:52.000000 apache_airflow_providers_pgvector-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 apache_airflow_providers_pgvector-1.2.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/README.rst` & `apache_airflow_providers_pgvector-1.2.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -38,45 +38,45 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pgvector``
 
-Release: ``1.1.0.rc1``
+Release: ``1.2.0.rc1``
 
 
 `pgvector <https://github.com/pgvector/pgvector>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pgvector`` provider. All classes for this provider package
 are in ``airflow.providers.pgvector`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pgvector``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================================  ==================
 PIP package                            Version required
 =====================================  ==================
-``apache-airflow``                     ``>=2.6.0``
+``apache-airflow``                     ``>=2.7.0``
 ``apache-airflow-providers-postgres``  ``>=5.7.1``
 ``pgvector``                           ``>=0.2.3``
 =====================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -94,8 +94,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-postgres <https://airflow.apache.org/docs/apache-airflow-providers-postgres>`_      ``postgres``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/LICENSE` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/__init__.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/__init__.py`

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
-        f"The package `apache-airflow-providers-pgvector:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-pgvector:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/get_provider_info.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pgvector",
         "name": "pgvector",
         "description": "`pgvector <https://github.com/pgvector/pgvector>`__\n",
-        "suspended": False,
-        "source-date-epoch": 1701983406,
-        "versions": ["1.1.0", "1.0.0"],
+        "state": "ready",
+        "source-date-epoch": 1714477192,
+        "versions": ["1.2.0", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "pgvector",
                 "external-doc-url": "https://github.com/pgvector/pgvector",
                 "how-to-guide": ["/docs/apache-airflow-providers-pgvector/operators/pgvector.rst"],
                 "tags": ["software"],
             }
         ],
         "dependencies": [
-            "apache-airflow>=2.6.0",
+            "apache-airflow>=2.7.0",
             "apache-airflow-providers-postgres>=5.7.1",
             "pgvector>=0.2.3",
         ],
         "hooks": [
             {"integration-name": "pgvector", "python-modules": ["airflow.providers.pgvector.hooks.pgvector"]}
         ],
         "operators": [
```

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/hooks/__init__.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/hooks/pgvector.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/hooks/pgvector.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/operators/__init__.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/airflow/providers/pgvector/operators/pgvector.py` & `apache_airflow_providers_pgvector-1.2.0rc1/airflow/providers/pgvector/operators/pgvector.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/pyproject.toml` & `apache_airflow_providers_pgvector-1.2.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-pgvector"
-version = "1.1.0.rc1"
+version = "1.2.0.rc1"
 description = "Provider package apache-airflow-providers-pgvector for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,26 +47,27 @@
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
-    "apache-airflow-providers-postgres>=5.7.1.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-postgres>=5.7.1rc0",
+    "apache-airflow>=2.7.0rc0",
     "pgvector>=0.2.3",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_pgvector-1.1.0rc1/PKG-INFO` & `apache_airflow_providers_pgvector-1.2.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pgvector
-Version: 1.1.0rc1
+Version: 1.2.0rc1
 Summary: Provider package apache-airflow-providers-pgvector for Apache Airflow
 Keywords: airflow-provider,pgvector,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,23 +15,24 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-postgres>=5.7.1.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-postgres>=5.7.1rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pgvector>=0.2.3
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-postgres ; extra == "postgres"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 Provides-Extra: postgres
 
@@ -75,45 +76,45 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pgvector``
 
-Release: ``1.1.0.rc1``
+Release: ``1.2.0.rc1``
 
 
 `pgvector <https://github.com/pgvector/pgvector>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pgvector`` provider. All classes for this provider package
 are in ``airflow.providers.pgvector`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pgvector``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================================  ==================
 PIP package                            Version required
 =====================================  ==================
-``apache-airflow``                     ``>=2.6.0``
+``apache-airflow``                     ``>=2.7.0``
 ``apache-airflow-providers-postgres``  ``>=5.7.1``
 ``pgvector``                           ``>=0.2.3``
 =====================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,8 +132,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-postgres <https://airflow.apache.org/docs/apache-airflow-providers-postgres>`_      ``postgres``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.1.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pgvector/1.2.0/changelog.html>`_.
```

