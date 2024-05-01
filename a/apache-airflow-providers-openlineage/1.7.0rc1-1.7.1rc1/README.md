# Comparing `tmp/apache_airflow_providers_openlineage-1.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_openlineage-1.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openlineage-1.7.0rc1.tar", last modified: Tue Apr  9 12:37:27 2024, max compression
+gzip compressed data, was "apache_airflow_providers_openlineage-1.7.1rc1.tar", last modified: Tue Apr 30 11:37:38 2024, max compression
```

## Comparing `apache_airflow_providers_openlineage-1.7.0rc1.tar` & `apache_airflow_providers_openlineage-1.7.1rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4410 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE
--rw-r--r--   0        0        0     1586 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py
--rw-r--r--   0        0        0     3398 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/conf.py
--rw-r--r--   0        0        0     1081 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0        0        0     5070 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0        0        0     2412 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0        0        0     9996 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0        0        0     2999 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0        0        0     6605 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0        0        0    14634 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0        0        0     2644 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0        0        0    11624 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0        0        0     3076 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0        0        0     1625 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0        0        0    13806 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py
--rw-r--r--   0        0        0      785 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/selective_enable.py
--rw-r--r--   0        0        0     9366 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0        0        0    13115 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py
--rw-r--r--   0        0        0     3355 2024-04-09 12:37:27.000000 apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4410 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/LICENSE
+-rw-r--r--   0        0        0     1586 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/__init__.py
+-rw-r--r--   0        0        0     3398 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/conf.py
+-rw-r--r--   0        0        0     1081 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0        0        0     5070 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0        0        0     2412 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0        0        0     9996 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0        0        0     2999 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0        0        0     6626 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0        0        0    14634 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0        0        0     2644 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0        0        0    11624 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0        0        0     3076 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0        0        0     1625 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0        0        0    15308 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/sqlparser.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/selective_enable.py
+-rw-r--r--   0        0        0     9366 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0        0        0    13285 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/utils.py
+-rw-r--r--   0        0        0     3355 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/README.rst` & `apache_airflow_providers_openlineage-1.7.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.0.rc1``
+Release: ``1.7.1.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
@@ -95,8 +95,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/LICENSE` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/__init__.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/conf.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/conf.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/__init__.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/base.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/bash.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/manager.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/extractors/python.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/get_provider_info.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openlineage",
         "name": "OpenLineage Airflow",
         "description": "`OpenLineage <https://openlineage.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1712666247,
+        "source-date-epoch": 1714477058,
         "versions": [
+            "1.7.1",
             "1.7.0",
             "1.6.0",
             "1.5.0",
             "1.4.0",
             "1.3.1",
             "1.3.0",
             "1.2.1",
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/__init__.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/adapter.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/facets.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/listener.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/macros.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/plugins/openlineage.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/sqlparser.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     ColumnLineageDatasetFacet,
     ColumnLineageDatasetFacetFieldsAdditional,
     ColumnLineageDatasetFacetFieldsAdditionalInputFields,
     ExtractionError,
     ExtractionErrorRunFacet,
     SqlJobFacet,
 )
+from openlineage.client.run import Dataset
 from openlineage.common.sql import DbTableMeta, SqlMeta, parse
 
 from airflow.providers.openlineage.extractors.base import OperatorLineage
 from airflow.providers.openlineage.utils.sql import (
     TablesHierarchy,
     create_information_schema_query,
     get_table_schemas,
 )
 from airflow.typing_compat import TypedDict
 
 if TYPE_CHECKING:
-    from openlineage.client.run import Dataset
     from sqlalchemy.engine import Engine
 
     from airflow.hooks.base import BaseHook
 
 DEFAULT_NAMESPACE = "default"
 DEFAULT_INFORMATION_SCHEMA_COLUMNS = [
     "table_schema",
@@ -100,28 +100,40 @@
     information_schema_table_name: str = DEFAULT_INFORMATION_SCHEMA_TABLE_NAME
     use_flat_cross_db_query: bool = False
     is_information_schema_cross_db: bool = False
     is_uppercase_names: bool = False
     normalize_name_method: Callable[[str], str] = default_normalize_name_method
 
 
+def from_table_meta(
+    table_meta: DbTableMeta, database: str | None, namespace: str, is_uppercase: bool
+) -> Dataset:
+    if table_meta.database:
+        name = table_meta.qualified_name
+    elif database:
+        name = f"{database}.{table_meta.schema}.{table_meta.name}"
+    else:
+        name = f"{table_meta.schema}.{table_meta.name}"
+    return Dataset(namespace=namespace, name=name if not is_uppercase else name.upper())
+
+
 class SQLParser:
     """Interface for openlineage-sql.
 
     :param dialect: dialect specific to the database
     :param default_schema: schema applied to each table with no schema parsed
     """
 
     def __init__(self, dialect: str | None = None, default_schema: str | None = None) -> None:
         self.dialect = dialect
         self.default_schema = default_schema
 
     def parse(self, sql: list[str] | str) -> SqlMeta | None:
         """Parse a single or a list of SQL statements."""
-        return parse(sql=sql, dialect=self.dialect)
+        return parse(sql=sql, dialect=self.dialect, default_schema=self.default_schema)
 
     def parse_table_schemas(
         self,
         hook: BaseHook,
         inputs: list[DbTableMeta],
         outputs: list[DbTableMeta],
         database_info: DatabaseInfo,
@@ -152,14 +164,31 @@
             self.create_information_schema_query(
                 tables=outputs, sqlalchemy_engine=sqlalchemy_engine, **database_kwargs
             )
             if outputs
             else None,
         )
 
+    def get_metadata_from_parser(
+        self,
+        inputs: list[DbTableMeta],
+        outputs: list[DbTableMeta],
+        database_info: DatabaseInfo,
+        namespace: str = DEFAULT_NAMESPACE,
+        database: str | None = None,
+    ) -> tuple[list[Dataset], ...]:
+        database = database if database else database_info.database
+        return [
+            from_table_meta(dataset, database, namespace, database_info.is_uppercase_names)
+            for dataset in inputs
+        ], [
+            from_table_meta(dataset, database, namespace, database_info.is_uppercase_names)
+            for dataset in outputs
+        ]
+
     def attach_column_lineage(
         self, datasets: list[Dataset], database: str | None, parse_result: SqlMeta
     ) -> None:
         """
         Attaches column lineage facet to the list of datasets.
 
         Note that currently each dataset has the same column lineage information set.
@@ -200,14 +229,15 @@
     def generate_openlineage_metadata_from_sql(
         self,
         sql: list[str] | str,
         hook: BaseHook,
         database_info: DatabaseInfo,
         database: str | None = None,
         sqlalchemy_engine: Engine | None = None,
+        use_connection: bool = True,
     ) -> OperatorLineage:
         """Parse SQL statement(s) and generate OpenLineage metadata.
 
         Generated OpenLineage metadata contains:
 
         * input tables with schemas parsed
         * output tables with schemas parsed
@@ -238,23 +268,32 @@
                         taskNumber=error.index,
                     )
                     for error in parse_result.errors
                 ],
             )
 
         namespace = self.create_namespace(database_info=database_info)
-        inputs, outputs = self.parse_table_schemas(
-            hook=hook,
-            inputs=parse_result.in_tables,
-            outputs=parse_result.out_tables,
-            namespace=namespace,
-            database=database,
-            database_info=database_info,
-            sqlalchemy_engine=sqlalchemy_engine,
-        )
+        if use_connection:
+            inputs, outputs = self.parse_table_schemas(
+                hook=hook,
+                inputs=parse_result.in_tables,
+                outputs=parse_result.out_tables,
+                namespace=namespace,
+                database=database,
+                database_info=database_info,
+                sqlalchemy_engine=sqlalchemy_engine,
+            )
+        else:
+            inputs, outputs = self.get_metadata_from_parser(
+                inputs=parse_result.in_tables,
+                outputs=parse_result.out_tables,
+                namespace=namespace,
+                database=database,
+                database_info=database_info,
+            )
 
         self.attach_column_lineage(outputs, database or database_info.database, parse_result)
 
         return OperatorLineage(
             inputs=inputs,
             outputs=outputs,
             run_facets=run_facets,
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/__init__.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/selective_enable.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/selective_enable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/sql.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/airflow/providers/openlineage/utils/utils.py` & `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,7 +380,12 @@
 
 
 def normalize_sql(sql: str | Iterable[str]):
     if isinstance(sql, str):
         sql = [stmt for stmt in sql.split(";") if stmt != ""]
     sql = [obj for stmt in sql for obj in stmt.split(";") if obj != ""]
     return ";\n".join(sql)
+
+
+def should_use_external_connection(hook) -> bool:
+    # TODO: Add checking overrides
+    return hook.__class__.__name__ not in ["SnowflakeHook", "SnowflakeSqlApiHook"]
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/pyproject.toml` & `apache_airflow_providers_openlineage-1.7.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openlineage"
-version = "1.7.0.rc1"
+version = "1.7.1.rc1"
 description = "Provider package apache-airflow-providers-openlineage for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -60,16 +60,16 @@
     "apache-airflow>=2.7.0rc0",
     "attrs>=22.2",
     "openlineage-integration-common>=0.28.0",
     "openlineage-python>=0.28.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_openlineage-1.7.0rc1/PKG-INFO` & `apache_airflow_providers_openlineage-1.7.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.7.0rc1
+Version: 1.7.1rc1
 Summary: Provider package apache-airflow-providers-openlineage for Apache Airflow
 Keywords: airflow-provider,openlineage,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Requires-Dist: apache-airflow-providers-common-sql>=1.6.0rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: attrs>=22.2
 Requires-Dist: openlineage-integration-common>=0.28.0
 Requires-Dist: openlineage-python>=0.28.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -76,28 +76,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.0.rc1``
+Release: ``1.7.1.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
@@ -133,8 +133,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html>`_.
```

