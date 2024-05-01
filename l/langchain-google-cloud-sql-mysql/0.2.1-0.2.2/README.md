# Comparing `tmp/langchain_google_cloud_sql_mysql-0.2.1-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_mysql-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29961 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/__init__.py
--rw-r--r--  2.0 unx     4636 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/chat_message_history.py
--rw-r--r--  2.0 unx    14907 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/engine.py
--rw-r--r--  2.0 unx     3430 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/indexes.py
--rw-r--r--  2.0 unx    11912 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/py.typed
--rw-r--r--  2.0 unx    29956 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/vectorstore.py
--rw-r--r--  2.0 unx      597 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    18482 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1326 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD
-13 files, 97880 bytes uncompressed, 27667 bytes compressed:  71.7%
+Zip file size: 30027 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1151 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/__init__.py
+-rw-r--r--  2.0 unx     4636 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/chat_message_history.py
+-rw-r--r--  2.0 unx    14879 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/engine.py
+-rw-r--r--  2.0 unx     3430 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/indexes.py
+-rw-r--r--  2.0 unx    11880 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/py.typed
+-rw-r--r--  2.0 unx    29732 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/vectorstore.py
+-rw-r--r--  2.0 unx      597 b- defN 24-May-01 21:09 langchain_google_cloud_sql_mysql/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 21:11 langchain_google_cloud_sql_mysql-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19948 b- defN 24-May-01 21:11 langchain_google_cloud_sql_mysql-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 21:11 langchain_google_cloud_sql_mysql-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-May-01 21:11 langchain_google_cloud_sql_mysql-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1326 b- defN 24-May-01 21:11 langchain_google_cloud_sql_mysql-0.2.2.dist-info/RECORD
+13 files, 99062 bytes uncompressed, 27733 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_cloud_sql_mysql/vectorstore.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_mysql/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_mysql-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA
+Filename: langchain_google_cloud_sql_mysql-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_mysql-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_mysql-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD
+Filename: langchain_google_cloud_sql_mysql-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_mysql/engine.py

```diff
@@ -249,30 +249,33 @@
             return result_fetch
 
     def init_chat_history_table(self, table_name: str) -> None:
         """Create table with schema required for MySQLChatMessageHistory class.
 
         Required schema is as follows:
 
+        ::
+
             CREATE TABLE {table_name} (
                 id INT AUTO_INCREMENT PRIMARY KEY,
                 session_id TEXT NOT NULL,
                 data JSON NOT NULL,
                 type TEXT NOT NULL
             )
 
         Args:
-            table_name (str): Name of database table to create for storing chat
-                message history.
+            table_name (str): The name of the table to create.
+
         """
+
         create_table_query = f"""CREATE TABLE IF NOT EXISTS `{table_name}` (
-          id INT AUTO_INCREMENT PRIMARY KEY,
-          session_id TEXT NOT NULL,
-          data JSON NOT NULL,
-          type TEXT NOT NULL
+            id INT AUTO_INCREMENT PRIMARY KEY,
+            session_id TEXT NOT NULL,
+            data JSON NOT NULL,
+            type TEXT NOT NULL
         );"""
 
         with self.engine.connect() as conn:
             conn.execute(sqlalchemy.text(create_table_query))
             conn.commit()
 
     def init_document_table(
```

## langchain_google_cloud_sql_mysql/loader.py

```diff
@@ -198,24 +198,22 @@
         table_name: str,
         content_column: Optional[str] = None,
         metadata_json_column: Optional[str] = None,
     ):
         """
         MySQLDocumentSaver allows for saving of langchain documents in a database. If the table
         doesn't exists, a table with default schema will be created. The default schema:
-            - page_content (type: text)
-            - langchain_metadata (type: JSON)
+        - page_content (type: text)
+        - langchain_metadata (type: JSON)
 
         Args:
           engine (MySQLEngine): MySQLEngine object to connect to the MySQL database.
           table_name (str): The name of table for saving documents.
-          content_column (str): The column to store document content.
-            Deafult: `page_content`. Optional.
-          metadata_json_column (str): The name of the JSON column to use as the metadata’s base
-            dictionary. Default: `langchain_metadata`. Optional.
+          content_column (str): The column to store document content. Deafult: `page_content`. Optional.
+          metadata_json_column (str): The name of the JSON column to use as the metadata’s base dictionary. Default: `langchain_metadata`. Optional.
         """
         self.engine = engine
         self.table_name = table_name
         self._table = self.engine._load_document_table(table_name)
 
         self.content_column = content_column or DEFAULT_CONTENT_COL
         if self.content_column not in self._table.columns.keys():
```

## langchain_google_cloud_sql_mysql/vectorstore.py

```diff
@@ -51,40 +51,26 @@
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         query_options: QueryOptions = DEFAULT_QUERY_OPTIONS,
     ):
         """Constructor for MySQLVectorStore.
         Args:
-            engine (MySQLEngine): Connection pool engine for managing
-                connections to Cloud SQL for MySQL database.
+            engine (MySQLEngine): Connection pool engine for managing connections to Cloud SQL for MySQL database.
             embedding_service (Embeddings): Text embedding model to use.
             table_name (str): Name of an existing table or table to be created.
-            content_column (str): Column that represent a Document's
-                page_content. Defaults to "content".
-            embedding_column (str): Column for embedding vectors. The embedding
-                is generated from the document value. Defaults to "embedding".
+            content_column (str): Column that represent a Document's page_content. Defaults to "content".
+            embedding_column (str): Column for embedding vectors. The embedding is generated from the document value. Defaults to "embedding".
             metadata_columns (List[str]): Column(s) that represent a document's metadata.
-            ignore_metadata_columns (List[str]): Column(s) to ignore in
-                pre-existing tables for a document's metadata. Can not be used
-                with metadata_columns. Defaults to None.
-            id_column (str): Column that represents the Document's id.
-                Defaults to "langchain_id".
-            metadata_json_column (str): Column to store metadata as JSON.
-                Defaults to "langchain_metadata".
-            k (int): The number of documents to return as the final result of a
-                similarity search. Defaults to 4.
-            fetch_k (int): The number of documents to initially retrieve from
-                the database during a similarity search. These documents are
-                then re-ranked using MMR to select the final `k` documents.
-                Defaults to 20.
-            lambda_mult (float): The weight used to balance relevance and
-                diversity in the MMR algorithm. A higher value emphasizes
-                diversity more, while a lower value prioritizes relevance.
-                Defaults to 0.5.
+            ignore_metadata_columns (List[str]): Column(s) to ignore in pre-existing tables for a document's metadata. Can not be used with metadata_columns. Defaults to None.
+            id_column (str): Column that represents the Document's id. Defaults to "langchain_id".
+            metadata_json_column (str): Column to store metadata as JSON. Defaults to "langchain_metadata".
+            k (int): The number of documents to return as the final result of a similarity search. Defaults to 4.
+            fetch_k (int): The number of documents to initially retrieve from the database during a similarity search. These documents are then re-ranked using MMR to select the final `k` documents. Defaults to 20.
+            lambda_mult (float): The weight used to balance relevance and diversity in the MMR algorithm. A higher value emphasizes diversity more, while a lower value prioritizes relevance. Defaults to 0.5.
             query_options: Additional query options.
         """
         if metadata_columns and ignore_metadata_columns:
             raise ValueError(
                 "Can not use both metadata_columns and ignore_metadata_columns."
             )
         # Get field type information
```

## langchain_google_cloud_sql_mysql/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

## Comparing `langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE` & `langchain_google_cloud_sql_mysql-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA` & `langchain_google_cloud_sql_mysql-0.2.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-mysql
-Version: 0.2.1
+Version: 0.2.2
 Summary: LangChain integrations for Google Cloud SQL for MySQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,144 +206,191 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/CHANGELOG.md
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Requires-Dist: numpy <2.0.0,>=1.24.4
 Requires-Dist: SQLAlchemy <3.0.0,>=2.0.7
 Requires-Dist: cloud-sql-python-connector[pymysql] <2.0.0,>=1.7.0
 Provides-Extra: test
-Requires-Dist: black[jupyter] ==24.3.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==24.4.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.9.0 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
+Requires-Dist: mypy ==1.10.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.6 ; extra == 'test'
 Requires-Dist: pytest ==8.1.1 ; extra == 'test'
 
-# Cloud SQL for MySQL for LangChain
+Cloud SQL for MySQL for LangChain
+=================================
 
-This package contains the [LangChain][langchain] integrations for Cloud SQL for MySQL.
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
+- `Client Library Documentation`_
+- `Product Documentation`_
 
-* [Documentation](docs/)
-* [API Reference]()
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://cloud.google.com/products#product-launch-stages
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-cloud-sql-mysql.svg
+   :target: https://pypi.org/project/langchain-google-cloud-sql-mysql/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-cloud-sql-mysql.svg
+   :target: https://pypi.org/project/langchain-google-cloud-sql-mysql/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-cloud-sql-mysql/latest
+.. _Product Documentation: https://cloud.google.com/sql/mysql
 
-## Getting Started
+Quick Start
+-----------
 
-In order to use this library, you first need to go through the following steps:
+In order to use this library, you first need to go through the following
+steps:
 
-1. [Select or create a Cloud Platform project.][project]
-2. [Enable billing for your project.][billing]
-3. [Enable the Google Cloud SQL API.][api]
-4. [Setup Authentication.][auth]
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Google Cloud SQL Admin API.`_
+4. `Setup Authentication.`_
 
-### Installation
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Google Cloud SQL Admin API.: https://console.cloud.google.com/flows/enableapi?apiid=sqladmin.googleapis.com
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv] is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Installation
+~~~~~~~~~~~~
 
-With [`virtualenv`][venv], it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. The basic problem it addresses is
+one of dependencies and versions, and indirectly permissions.
 
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-cloud-sql-mysql
-```
+With `virtualenv`_, it’s possible to install this library without needing system install permissions, and without clashing with the installed system dependencies.
 
-## Vector Store Usage
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
-Use a [vector store](https://python.langchain.com/docs/modules/data_connection/vectorstores/) to store
-embedded data and perform vector search.
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
-```python
-from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLVectorStore
-from langchain_google_vertexai import VertexAIEmbeddings
+Python >= 3.8
 
+Mac/Linux
+^^^^^^^^^
 
-engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
-engine.init_vectorstore_table(
-    table_name="my-table-name",
-    vector_size=768,  # Vector size for `VertexAIEmbeddings()`
-)
-vectorstore = MySQLVectorStore(
-    engine,
-    embedding_service=VertextAIEmbeddings(),
-    table_name="my-table-name",
-)
-```
+.. code-block:: console
 
-See the full [Vector Store][vectorstore] tutorial.
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-cloud-sql-mysql
 
-## Document Loader Usage
+Windows
+^^^^^^^
 
-Use a [document loader](https://python.langchain.com/docs/modules/data_connection/document_loaders/) to load data as LangChain `Document`s.
+.. code-block:: console
 
-```python
-from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLLoader
+   pip install virtualenv
+   virtualenv <your-env>
+   <your-env>\Scripts\activate
+   <your-env>\Scripts\pip.exe install langchain-google-cloud-sql-mysql
 
+Vector Store Usage
+~~~~~~~~~~~~~~~~~~~
 
-engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
-loader = MySQLLoader(
-    engine,
-    table_name="my-table-name"
-)
-docs = loader.lazy_load()
-```
+Use a vector store to store embedded data and perform vector search.
 
-See the full [Document Loader][loader] tutorial.
+.. code-block:: python
 
-## Chat Message History Usage
+   from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLVectorStore
+   from langchain_google_vertexai import VertexAIEmbeddings
 
-Use [ChatMessageHistory](https://python.langchain.com/docs/modules/memory/chat_messages/) to store messages and provide conversation history to LLMs.
+   engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
+   engine.init_vectorstore_table(
+       table_name="my-table-name",
+       vector_size=768
+   )
+   vectorstore = MySQLVectorStore(
+       engine,
+       embedding_service=VertexAIEmbeddings(model_name="textembedding-gecko@003"),
+       table_name="my-table-name"
+   )
 
-```python
-from langchain_google_cloud_sql_mysql import MySQLChatMessageHistory, MySQLEngine
+See the full `Vector Store`_ tutorial.
 
+.. _`Vector Store`: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/docs/vector_store.ipynb
 
-engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
-history = MySQLChatMessageHistory(
-    engine,
-    table_name="my-message-store",
-    session_id="my-session_id"
-)
-```
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
 
-See the full [Chat Message History][history] tutorial.
+Use a document loader to load data as LangChain ``Document``\ s.
 
-## Contributing
+.. code-block:: python
+
+   from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLLoader
+
+   engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
+   loader = MySQLLoader(
+       engine,
+       table_name="my-table-name"
+   )
+   docs = loader.lazy_load()
+
+See the full `Document Loader`_ tutorial.
+
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/docs/document_loader.ipynb
+
+Chat Message History Usage
+--------------------------
+
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
+
+.. code:: python
+
+   from langchain_google_cloud_sql_mysql import MySQLChatMessageHistory, MySQLEngine
+
+   engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
+   history = MySQLChatMessageHistory(
+       engine,
+       table_name="my-message-store",
+       session_id="my-session-id"
+   )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/docs/chat_message_history.ipynb
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING](CONTRIBUTING.md) for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct](CODE_OF_CONDUCT.md) for more
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/CODE_OF_CONDUCT.md
+
+License
+-------
 
-Apache 2.0 - See [LICENSE](LICENSE) for more information.
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/LICENSE>`_
+for more information.
 
-## Disclaimer
+Disclaimer
+----------
 
 This is not an officially supported Google product.
 
-[project]: https://console.cloud.google.com/project
-[billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-[api]: https://console.cloud.google.com/flows/enableapi?apiid=sqladmin.googleapis.com
-[auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
-[venv]: https://virtualenv.pypa.io/en/latest/
-[loader]: ./docs/document_loader.ipynb
-[history]: ./docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[vectorstore]: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/tree/main/docs/vector_store.ipynb
```

## Comparing `langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD` & `langchain_google_cloud_sql_mysql-0.2.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_cloud_sql_mysql/__init__.py,sha256=fH1Y3GlQnwHNFt16hPowLHtEULVMTv1MX-_91qot_rc,1151
 langchain_google_cloud_sql_mysql/chat_message_history.py,sha256=gx2o-QegU04V6fX8P-JfHpm_yVn2Et846pDrPGOevWk,4636
-langchain_google_cloud_sql_mysql/engine.py,sha256=zbr6TIr5jdOP6W21cDsIBwfvoXxAKPPwEpgDjWo6Twg,14907
+langchain_google_cloud_sql_mysql/engine.py,sha256=15zkbyLnz0HTOZqdslJnSOa9EcVTx6dyMKWqUUi9seI,14879
 langchain_google_cloud_sql_mysql/indexes.py,sha256=sv6co_H0v1j1OwEL3SGTOV9mNt6x-aM-qwNXE1UL9ag,3430
-langchain_google_cloud_sql_mysql/loader.py,sha256=LPYEyoTc-_98zvTN_rtXG-gZdIBd8o5qWxbRvek7Kgk,11912
+langchain_google_cloud_sql_mysql/loader.py,sha256=56p67QW5Lqf_5vnLZbhcoH37B74-9Pt6FLW7kUXDJ0c,11880
 langchain_google_cloud_sql_mysql/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_cloud_sql_mysql/vectorstore.py,sha256=Bkw4CpTxlpRWbDOp4-oQ5_En01ghwuNEhNjYzZrbPNk,29956
-langchain_google_cloud_sql_mysql/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
-langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA,sha256=u5FbLzIt79a1uzE04syXCOINl1SnZ2YXtcDSvbbh_4c,18482
-langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt,sha256=66mG3PXjFtwydGTUP8umus8EqCXttsD9B01ulc-Q67g,33
-langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD,,
+langchain_google_cloud_sql_mysql/vectorstore.py,sha256=IbsSYcOqEeCF_WV5DH4iXVp_Bpdnizc1yLfznRT_TIc,29732
+langchain_google_cloud_sql_mysql/version.py,sha256=r_E0O4zsO8RmFXO1jNldtopOU4jjOND4dKdlCCYS1rE,597
+langchain_google_cloud_sql_mysql-0.2.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_cloud_sql_mysql-0.2.2.dist-info/METADATA,sha256=E8eBfgBj-g0EAB_0KCLlP8CgXmtck5yguVqcHOmchEg,19948
+langchain_google_cloud_sql_mysql-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_cloud_sql_mysql-0.2.2.dist-info/top_level.txt,sha256=66mG3PXjFtwydGTUP8umus8EqCXttsD9B01ulc-Q67g,33
+langchain_google_cloud_sql_mysql-0.2.2.dist-info/RECORD,,
```

