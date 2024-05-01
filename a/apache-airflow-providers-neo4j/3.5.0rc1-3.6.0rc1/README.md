# Comparing `tmp/apache_airflow_providers_neo4j-3.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_neo4j-3.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_neo4j-3.5.0rc1.tar", last modified: Thu Dec  7 21:09:58 2023, max compression
+gzip compressed data, was "apache_airflow_providers_neo4j-3.6.0rc1.tar", last modified: Tue Apr 30 11:35:06 2024, max compression
```

## Comparing `apache_airflow_providers_neo4j-3.5.0rc1.tar` & `apache_airflow_providers_neo4j-3.6.0rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3035 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/LICENSE
--rw-r--r--   0        0        0      779 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/README.md
--rw-r--r--   0        0        0     1580 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/__init__.py
--rw-r--r--   0        0        0     2504 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/get_provider_info.py
--rw-r--r--   0        0        0      787 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/hooks/__init__.py
--rw-r--r--   0        0        0     4351 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/hooks/neo4j.py
--rw-r--r--   0        0        0      787 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/operators/__init__.py
--rw-r--r--   0        0        0     2067 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/operators/neo4j.py
--rw-r--r--   0        0        0     2910 2023-12-07 21:09:58.000000 apache_airflow_providers_neo4j-3.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4669 1970-01-01 00:00:00.000000 apache_airflow_providers_neo4j-3.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3040 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/LICENSE
+-rw-r--r--   0        0        0      779 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/README.md
+-rw-r--r--   0        0        0     1580 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/__init__.py
+-rw-r--r--   0        0        0     2523 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/hooks/__init__.py
+-rw-r--r--   0        0        0     4313 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/hooks/neo4j.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/operators/__init__.py
+-rw-r--r--   0        0        0     2067 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/operators/neo4j.py
+-rw-r--r--   0        0        0     2954 2024-04-30 11:35:06.000000 apache_airflow_providers_neo4j-3.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4723 1970-01-01 00:00:00.000000 apache_airflow_providers_neo4j-3.6.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/README.rst` & `apache_airflow_providers_neo4j-3.6.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,43 +38,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.5.0.rc1``
+Release: ``3.6.0.rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``neo4j`` provider. All classes for this provider package
 are in ``airflow.providers.neo4j`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-neo4j``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``neo4j``           ``>=4.2.1``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/LICENSE` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/README.md` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/README.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/__init__.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.6.0"
+    "2.7.0"
 ):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-neo4j:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-neo4j:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/get_provider_info.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-neo4j",
         "name": "Neo4j",
         "description": "`Neo4j <https://neo4j.com/>`__\n",
-        "suspended": False,
-        "source-date-epoch": 1701983398,
+        "state": "ready",
+        "source-date-epoch": 1714476906,
         "versions": [
+            "3.6.0",
             "3.5.0",
             "3.4.0",
             "3.3.3",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
@@ -46,15 +47,15 @@
             "2.1.0",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "neo4j>=4.2.1"],
+        "dependencies": ["apache-airflow>=2.7.0", "neo4j>=4.2.1"],
         "integrations": [
             {
                 "integration-name": "Neo4j",
                 "external-doc-url": "https://neo4j.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-neo4j/operators/neo4j.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/hooks/__init__.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/hooks/neo4j.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/hooks/neo4j.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module allows to connect to a Neo4j database."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlsplit
 
 from neo4j import Driver, GraphDatabase
 
@@ -46,15 +47,15 @@
     def __init__(self, conn_id: str = default_conn_name, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.neo4j_conn_id = conn_id
         self.connection = kwargs.pop("connection", None)
         self.client: Driver | None = None
 
     def get_conn(self) -> Driver:
-        """Function that initiates a new Neo4j connection with username, password and database schema."""
+        """Initiate a new Neo4j connection with username, password and database schema."""
         if self.client is not None:
             return self.client
 
         self.connection = self.get_connection(self.neo4j_conn_id)
 
         uri = self.get_uri(self.connection)
         self.log.info("URI: %s", uri)
@@ -63,15 +64,15 @@
 
         self.client = self.get_client(self.connection, is_encrypted, uri)
 
         return self.client
 
     def get_client(self, conn: Connection, encrypted: bool, uri: str) -> Driver:
         """
-        Function to determine that relevant driver based on extras.
+        Determine that relevant driver based on extras.
 
         :param conn: Connection object.
         :param encrypted: boolean if encrypted connection or not.
         :param uri: uri string for connection.
         :return: Driver
         """
         parsed_uri = urlsplit(uri)
@@ -107,15 +108,15 @@
         elif trusted_ca:
             encryption_scheme = "+s"
 
         return f"{scheme}{encryption_scheme}://{conn.host}:{7687 if conn.port is None else conn.port}"
 
     def run(self, query) -> list[Any]:
         """
-        Function to create a neo4j session and execute the query in the session.
+        Create a neo4j session and execute the query in the session.
 
         :param query: Neo4j query
         :return: Result
         """
         driver = self.get_conn()
         if not self.connection.schema:
             with driver.session() as session:
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/operators/__init__.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/airflow/providers/neo4j/operators/neo4j.py` & `apache_airflow_providers_neo4j-3.6.0rc1/airflow/providers/neo4j/operators/neo4j.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/pyproject.toml` & `apache_airflow_providers_neo4j-3.6.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-neo4j"
-version = "3.5.0.rc1"
+version = "3.6.0.rc1"
 description = "Provider package apache-airflow-providers-neo4j for Apache Airflow"
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
+    "apache-airflow>=2.7.0rc0",
     "neo4j>=4.2.1",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_neo4j-3.5.0rc1/PKG-INFO` & `apache_airflow_providers_neo4j-3.6.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-neo4j
-Version: 3.5.0rc1
+Version: 3.6.0rc1
 Summary: Provider package apache-airflow-providers-neo4j for Apache Airflow
 Keywords: airflow-provider,neo4j,airflow,integration
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
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: neo4j>=4.2.1
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -70,43 +71,43 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.5.0.rc1``
+Release: ``3.6.0.rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``neo4j`` provider. All classes for this provider package
 are in ``airflow.providers.neo4j`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-neo4j``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``neo4j``           ``>=4.2.1``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.5.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.6.0/changelog.html>`_.
```

