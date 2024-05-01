# Comparing `tmp/bmsdna_sql_utils-0.12.3.tar.gz` & `tmp/bmsdna_sql_utils-0.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.12.3.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.4.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.12.3.tar` & `bmsdna_sql_utils-0.12.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      255 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/README.md
--rw-r--r--   0        0        0        0 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5388 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     6066 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    25911 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2116 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5178 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1481 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1856 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0     4184 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source_spark.py
--rw-r--r--   0        0        0      739 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    16626 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1132 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      199 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0      996 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      884 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1870 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.3/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2373 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5388 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6066 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    25911 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1856 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0     4676 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/source_spark.py
+-rw-r--r--   0        0        0      739 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    16626 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1132 2024-05-01 04:47:56.885531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      996 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1870 2024-05-01 04:47:56.889531 bmsdna_sql_utils-0.12.4/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.4/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source_spark.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/source_spark.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 if TYPE_CHECKING:
     import pyspark
     from pyspark.sql import DataFrame
 logger = logging.getLogger(__name__)
 
 
 class SourceSpark(ImportSource):
-    def __init__(self, df: "DataFrame", use_json_insert=False, change_date: datetime | None = None) -> None:
+    def __init__(
+        self,
+        df: "DataFrame",
+        use_json_insert=False,
+        change_date: datetime | None = None,
+    ) -> None:
         super().__init__()
 
         self._schema: list[SQLField] | None = None
         self.use_json_insert = use_json_insert
         self.df = df
         self.change_date = change_date
 
@@ -38,33 +43,49 @@
 
         p_df = self.df
         if partition_filters:
             from pyspark.sql.functions import col, lit
 
             for k, v in partition_filters.items():
                 p_df = p_df.filter(col(k) == lit(v))
-        tbl = pa.Table.from_pandas(p_df.toPandas())
-
-        record_batch_reader = pa.RecordBatchReader.from_batches(tbl.schema, tbl.to_batches())
         from lakeapi2sql.bulk_insert import insert_record_batch_to_sql
 
         table_str = target_table if isinstance(target_table, str) else target_table[0] + "." + target_table[1]
         connection_string_sql = build_connection_string(connection_string, odbc=False)
         if self.use_json_insert:
-            from .json_insert import insert_into_table_via_json_from_batches
+            from .json_insert import insert_into_table_via_json
+
+            iter = p_df.toJSON().toLocalIterator()
+
+            async def _to_batches():
+                ls = []
+                for row in iter:
+                    ls.append(row)
+                    if len(ls) > 1000:
+                        yield "[" + "\n, ".join(ls) + "]"
+                        ls = []
+                if ls:
+                    yield "[" + "\n, ".join(ls) + "]"
+
             import pyodbc
 
             with pyodbc.connect(build_connection_string(connection_string, odbc=True)) as con:
                 schema = self.get_schema()
                 filtered_schema = schema if not select else [f for f in schema if f.column_name in select]
-                await insert_into_table_via_json_from_batches(
-                    reader=record_batch_reader, table_name=target_table, connection=con, schema=filtered_schema
+                await insert_into_table_via_json(
+                    json_batches=_to_batches(),
+                    table_name=target_table,
+                    connection=con,
+                    schema=filtered_schema,
                 )
                 col_names = [f.column_name for f in filtered_schema]
         else:
+            tbl = pa.Table.from_pandas(p_df.toPandas())
+
+            record_batch_reader = pa.RecordBatchReader.from_batches(tbl.schema, tbl.to_batches())
             res = await insert_record_batch_to_sql(connection_string_sql, table_str, record_batch_reader, select)
             col_names = [f["name"] for f in res["fields"]]
         return WriteInfo(column_names=col_names, table_name=target_table)
 
     def get_partition_values(self) -> list[dict]:
         col_names = [f.column_name for f in self.get_schema()]
         if "_partition" in col_names:
```

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.4/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.3/pyproject.toml` & `bmsdna_sql_utils-0.12.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.12.3"
+version = "0.12.4"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bmsdna_sql_utils-0.12.3/PKG-INFO` & `bmsdna_sql_utils-0.12.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.12.3
+Version: 0.12.4
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

