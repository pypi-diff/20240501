# Comparing `tmp/llama_index_vector_stores_postgres-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_postgres-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_postgres-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_postgres-0.1.6.tar", max compression
```

## Comparing `llama_index_vector_stores_postgres-0.1.5.tar` & `llama_index_vector_stores_postgres-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       49 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/README.md
--rw-r--r--   0        0        0       95 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/__init__.py
--rw-r--r--   0        0        0    25831 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/base.py
--rw-r--r--   0        0        0     1609 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 llama_index_vector_stores_postgres-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-01 19:44:03.289470 llama_index_vector_stores_postgres-0.1.6/README.md
+-rw-r--r--   0        0        0       95 2024-05-01 19:44:03.289470 llama_index_vector_stores_postgres-0.1.6/llama_index/vector_stores/postgres/__init__.py
+-rw-r--r--   0        0        0    26395 2024-05-01 19:44:03.289470 llama_index_vector_stores_postgres-0.1.6/llama_index/vector_stores/postgres/base.py
+-rw-r--r--   0        0        0     1609 2024-05-01 19:44:03.289470 llama_index_vector_stores_postgres-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 llama_index_vector_stores_postgres-0.1.6/PKG-INFO
```

### Comparing `llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/base.py` & `llama_index_vector_stores_postgres-0.1.6/llama_index/vector_stores/postgres/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,24 +281,28 @@
 
     def _create_schema_if_not_exists(self) -> None:
         with self._session() as session, session.begin():
             from sqlalchemy import text
 
             # Check if the specified schema exists with "CREATE" statement
             check_schema_statement = text(
-                f"SELECT schema_name FROM information_schema.schemata WHERE schema_name = '{self.schema_name}'"
+                f"SELECT schema_name FROM information_schema.schemata WHERE schema_name = :schema_name"
             )
-            result = session.execute(check_schema_statement).fetchone()
+            result = session.execute(
+                check_schema_statement, {"schema_name", self.schema_name}
+            ).fetchone()
 
             # If the schema does not exist, then create it
             if not result:
                 create_schema_statement = text(
-                    f"CREATE SCHEMA IF NOT EXISTS {self.schema_name}"
+                    f"CREATE SCHEMA IF NOT EXISTS :schema_name"
+                )
+                session.execute(
+                    create_schema_statement, {"schema_name": self.schema_name}
                 )
-                session.execute(create_schema_statement)
 
             session.commit()
 
     def _create_tables_if_not_exists(self) -> None:
         with self._session() as session, session.begin():
             self._base.metadata.create_all(session.connection())
 
@@ -474,20 +478,24 @@
         **kwargs: Any,
     ) -> List[DBEmbeddingRow]:
         stmt = self._build_query(embedding, limit, metadata_filters)
         with self._session() as session, session.begin():
             from sqlalchemy import text
 
             if kwargs.get("ivfflat_probes"):
+                ivfflat_probes = kwargs.get("ivfflat_probes")
                 session.execute(
-                    text(f"SET ivfflat.probes = {kwargs.get('ivfflat_probes')}")
+                    text(f"SET ivfflat.probes = :ivfflat_probes"),
+                    {"ivfflat_probes": ivfflat_probes},
                 )
             if kwargs.get("hnsw_ef_search"):
+                hnsw_ef_search = kwargs.get("hnsw_ef_search")
                 session.execute(
-                    text(f"SET hnsw.ef_search = {kwargs.get('hnsw_ef_search')}")
+                    text(f"SET hnsw.ef_search = :hnsw_ef_search"),
+                    {"hnsw_ef_search": hnsw_ef_search},
                 )
 
             res = session.execute(
                 stmt,
             )
             return [
                 DBEmbeddingRow(
@@ -507,20 +515,24 @@
         **kwargs: Any,
     ) -> List[DBEmbeddingRow]:
         stmt = self._build_query(embedding, limit, metadata_filters)
         async with self._async_session() as async_session, async_session.begin():
             from sqlalchemy import text
 
             if kwargs.get("hnsw_ef_search"):
+                hnsw_ef_search = kwargs.get("hnsw_ef_search")
                 await async_session.execute(
-                    text(f"SET hnsw.ef_search = {kwargs.get('hnsw_ef_search')}")
+                    text(f"SET hnsw.ef_search = :hnsw_ef_search"),
+                    {"hnsw_ef_search": hnsw_ef_search},
                 )
             if kwargs.get("ivfflat_probes"):
+                ivfflat_probes = kwargs.get("ivfflat_probes")
                 await async_session.execute(
-                    text(f"SET ivfflat.probes = {kwargs.get('ivfflat_probes')}")
+                    text(f"SET ivfflat.probes = :ivfflat_probes"),
+                    {"ivfflat_probes": ivfflat_probes},
                 )
 
             res = await async_session.execute(stmt)
             return [
                 DBEmbeddingRow(
                     node_id=item.node_id,
                     text=item.text,
@@ -740,18 +752,18 @@
     def delete(self, ref_doc_id: str, **delete_kwargs: Any) -> None:
         import sqlalchemy
 
         self._initialize()
         with self._session() as session, session.begin():
             stmt = sqlalchemy.text(
                 f"DELETE FROM {self.schema_name}.data_{self.table_name} where "
-                f"(metadata_->>'doc_id')::text = '{ref_doc_id}' "
+                f"(metadata_->>'doc_id')::text = :ref_doc_id"
             )
 
-            session.execute(stmt)
+            session.execute(stmt, {"ref_doc_id": ref_doc_id})
             session.commit()
 
 
 def _dedup_results(results: List[DBEmbeddingRow]) -> List[DBEmbeddingRow]:
     seen_ids = set()
     deduped_results = []
     for result in results:
```

### Comparing `llama_index_vector_stores_postgres-0.1.5/pyproject.toml` & `llama_index_vector_stores_postgres-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores postgres integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-postgres"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.20"
 pgvector = "^0.2.4"
 psycopg2-binary = "^2.9.9"
 asyncpg = "^0.29.0"
```

### Comparing `llama_index_vector_stores_postgres-0.1.5/PKG-INFO` & `llama_index_vector_stores_postgres-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-postgres
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index vector_stores postgres integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

