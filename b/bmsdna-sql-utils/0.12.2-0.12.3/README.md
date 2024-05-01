# Comparing `tmp/bmsdna_sql_utils-0.12.2.tar.gz` & `tmp/bmsdna_sql_utils-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.12.2.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.3.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.12.2.tar` & `bmsdna_sql_utils-0.12.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      255 2024-04-30 11:33:09.068932 bmsdna_sql_utils-0.12.2/README.md
--rw-r--r--   0        0        0        0 2024-04-30 11:33:09.068932 bmsdna_sql_utils-0.12.2/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5388 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     6066 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    25911 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2116 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5178 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1481 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1856 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0     3900 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source_spark.py
--rw-r--r--   0        0        0      739 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    16306 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1132 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      199 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0      822 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      884 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1805 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5388 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6066 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    25911 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1856 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0     4184 2024-04-30 13:39:25.406973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source_spark.py
+-rw-r--r--   0        0        0      739 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    16626 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1132 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      996 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1870 2024-04-30 13:39:25.410973 bmsdna_sql_utils-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.3/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source_spark.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/source_spark.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,18 @@
     def get_schema(self) -> list[SQLField]:
         fields = self.df.schema.fields
 
         def sqlglot_type(dtype):
             simple_str = str(dtype.simpleString())
             if simple_str == "timestamp_ntz":
                 return ex.DataType.build("datetime2", dialect="tsql")  # more or less
+            if simple_str.startswith("date32[") or simple_str == "date32":
+                return ex.DataType.build("date", dialect="tsql")
+            if simple_str.startswith("date64[") or simple_str == "date64":
+                return ex.DataType.build("date", dialect="tsql")
             return ex.DataType.build(simple_str, dialect="spark")
 
         return [SQLField(f.name, sqlglot_type(f.dataType)) for f in fields]
 
     def get_last_change_date(self):
         if self.change_date:
             return self.change_date
```

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,16 @@
     nullable=True,
     default: str | None = None,
     formula: str | None = None,
 ) -> str:
     if formula is not None:
         return sql_quote_name(field.column_name) + " AS " + formula
     sql_type = field.data_type.sql("tsql")
+    if sql_type.startswith("varchar") or sql_type.startswith("char"):
+        sql_type = "n" + sql_type  # see https://github.com/tobymao/sqlglot/issues/3381
     definit = sql_quote_name(field.column_name) + " " + sql_type + (" NOT NULL" if not nullable else "")
     if default is not None and default.lower() != "null":
         definit += " DEFAULT (" + default + ")"
     return definit
 
 
 def sql_quote_value_with_type(field: FieldWithType | SQLField, value: Any) -> str:
@@ -147,14 +149,16 @@
         if value == True:
             return f"CAST(1 as bit)"
         else:
             return f"CAST(0 as bit)"
     if value is not None and str(field.data_type.type).lower() in ["string", "int32", "varchar", "int"]:
         return sql_quote_value(value)  # string / int32 are defaults for sql server
     sql_type = field.data_type.sql("tsql")
+    if sql_type.startswith("varchar") or sql_type.startswith("char"):
+        sql_type = "n" + sql_type  # see https://github.com/tobymao/sqlglot/issues/3381
     if value is not None:
         return f"CAST({sql_quote_value(value)} as {sql_type})"
     else:
         return f"CAST(NULL AS {sql_type})"
 
 
 def get_sql_for_schema(
```

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 def recursive_get_type(t: "DataType", jsonify_complex: bool, dialect: str = "spark") -> ex.DataType:
     import pyarrow as pa
     import pyarrow.types as pat
 
     if pat.is_decimal(t):
         return ex.DataType.build(f"decimal({t.precision},{t.scale})", dialect="spark")
+    if pat.is_date(t):
+        return ex.DataType.build("date", dialect="tsql")
+    if pat.is_timestamp(t):
+        return ex.DataType.build("datetime2", dialect="tsql")
     if pat.is_null(t):
         return ex.DataType.build("null")
     is_complex = pa.types.is_nested(t)
     if is_complex and not jsonify_complex:
         return ex.DataType.build(str(t), dialect=dialect)
     if is_complex and jsonify_complex:
         return ex.DataType.build("string", dialect=dialect)
```

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.3/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.2/pyproject.toml` & `bmsdna_sql_utils-0.12.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.12.2"
+version = "0.12.3"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,15 +16,15 @@
 requests = ">=2.28.0"
 duckdb = { version = "^0.10.1", optional = true }
 lakeapi2sql = { version = ">=0.7.4", optional = true }
 deltalake = { version = ">=0.16.4", optional = true }
 python-dateutil = { version = "^2.8.2", python = "<3.11" }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake2db = ">=0.3.0"
-polars = { version = ">=0.20.21", optional = true }
+polars = {extras = ["chrono-tz"], version = ">=0.20.21", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.325"
 pyodbc = { version = ">=4.0.0" }
 aioodbc = { version = "^0.5.0" }
 python-tds = { version = "^1.13.0" }
 pydantic = ">=1.10.0"
@@ -40,14 +40,16 @@
 pytest = "^7.4.3"
 pytest-order = "^1.2.0"
 docker = "^7.0.0"
 pytest-cov = "^5.0.0"
 azure-identity = "^1.16.0"
 azure-storage-blob = "^12.19.1"
 python-dotenv = "^1.0.1"
+faker = "^25.0.0"
+deltalake = "^0.17.2"
 
 [pytest]
 log_cli = true
 
 [tool.poetry.extras]
 db-io = ["pyodbc", "lakeapi2sql"]
 delta = ["duckdb", "deltalake"]
```

### Comparing `bmsdna_sql_utils-0.12.2/PKG-INFO` & `bmsdna_sql_utils-0.12.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.12.2
+Version: 0.12.3
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,15 +16,15 @@
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aioodbc (>=0.5.0,<0.6.0)
 Requires-Dist: arrow-odbc (>=5.0.0,<6.0.0) ; extra == "db2delta"
 Requires-Dist: deltalake (>=0.16.4) ; extra == "delta" or extra == "db2delta"
 Requires-Dist: deltalake2db (>=0.3.0)
 Requires-Dist: duckdb (>=0.10.1,<0.11.0) ; extra == "delta" or extra == "db2delta"
 Requires-Dist: lakeapi2sql (>=0.7.4) ; extra == "db-io"
-Requires-Dist: polars (>=0.20.21) ; extra == "polars"
+Requires-Dist: polars[chrono-tz] (>=0.20.21) ; extra == "polars"
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pyodbc (>=5.0.1,<6.0.0) ; extra == "db-io"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) ; python_version < "3.11"
 Requires-Dist: python-tds (>=1.13.0,<2.0.0)
 Requires-Dist: requests (>=2.28.0)
 Description-Content-Type: text/markdown
```

