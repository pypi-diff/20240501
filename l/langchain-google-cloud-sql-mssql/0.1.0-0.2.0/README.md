# Comparing `tmp/langchain_google_cloud_sql_mssql-0.1.0-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_mssql-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20179 bytes, number of entries: 11
--rw-r--r--  2.0 unx      879 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/__init__.py
--rw-r--r--  2.0 unx     4641 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/chat_message_history.py
--rw-r--r--  2.0 unx     7715 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/engine.py
--rw-r--r--  2.0 unx    11243 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Feb-26 19:11 langchain_google_cloud_sql_mssql/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Feb-26 19:13 langchain_google_cloud_sql_mssql-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18318 b- defN 24-Feb-26 19:13 langchain_google_cloud_sql_mssql-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-26 19:13 langchain_google_cloud_sql_mssql-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Feb-26 19:13 langchain_google_cloud_sql_mssql-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1119 b- defN 24-Feb-26 19:13 langchain_google_cloud_sql_mssql-0.1.0.dist-info/RECORD
-11 files, 55995 bytes uncompressed, 18217 bytes compressed:  67.5%
+Zip file size: 20265 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      879 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/__init__.py
+-rw-r--r--  2.0 unx     4641 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/chat_message_history.py
+-rw-r--r--  2.0 unx     7727 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/engine.py
+-rw-r--r--  2.0 unx    11253 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/py.typed
+-rw-r--r--  2.0 unx      597 b- defN 24-May-01 21:29 langchain_google_cloud_sql_mssql/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 21:31 langchain_google_cloud_sql_mssql-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19294 b- defN 24-May-01 21:31 langchain_google_cloud_sql_mssql-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 21:31 langchain_google_cloud_sql_mssql-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-May-01 21:31 langchain_google_cloud_sql_mssql-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1119 b- defN 24-May-01 21:31 langchain_google_cloud_sql_mssql-0.2.0.dist-info/RECORD
+11 files, 56993 bytes uncompressed, 18303 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: langchain_google_cloud_sql_mssql/py.typed
 Comment: 
 
 Filename: langchain_google_cloud_sql_mssql/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_mssql-0.1.0.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_mssql-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_mssql-0.1.0.dist-info/METADATA
+Filename: langchain_google_cloud_sql_mssql-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_mssql-0.1.0.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_mssql-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_mssql-0.1.0.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_mssql-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_mssql-0.1.0.dist-info/RECORD
+Filename: langchain_google_cloud_sql_mssql-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_mssql/engine.py

```diff
@@ -124,14 +124,16 @@
         return self.engine.connect()
 
     def init_chat_history_table(self, table_name: str) -> None:
         """Create table with schema required for MSSQLChatMessageHistory class.
 
         Required schema is as follows:
 
+        ::
+
             CREATE TABLE {table_name} (
                 id INT IDENTITY(1,1) PRIMARY KEY,
                 session_id NVARCHAR(MAX) NOT NULL,
                 data NVARCHAR(MAX) NOT NULL,
                 type NVARCHAR(MAX) NOT NULL
             )
```

## langchain_google_cloud_sql_mssql/loader.py

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
-from collections.abc import Iterable
-from typing import Any, Dict, Iterator, List, Optional, Sequence, cast
+from typing import Any, Dict, Iterable, Iterator, List, Optional
 
 import sqlalchemy
 from langchain_community.document_loaders.base import BaseLoader
 from langchain_core.documents import Document
 
 from .engine import MSSQLEngine
 
@@ -168,15 +167,18 @@
                 for column in column_names:
                     value = getattr(row, column)
                     if column == metadata_json_column:
                         row_data[column] = json.loads(value)
                     else:
                         row_data[column] = value
                 yield _parse_doc_from_row(
-                    content_columns, metadata_columns, row_data, metadata_json_column
+                    content_columns,
+                    metadata_columns,
+                    row_data,
+                    metadata_json_column,
                 )
 
 
 class MSSQLDocumentSaver:
     """A class for saving langchain documents into a Cloud SQL MSSQL database table."""
 
     def __init__(
@@ -185,16 +187,16 @@
         table_name: str,
         content_column: Optional[str] = None,
         metadata_json_column: Optional[str] = None,
     ):
         """
         MSSQLDocumentSaver allows for saving of langchain documents in a database. If the table
         doesn't exists, a table with default schema will be created. The default schema:
-            - page_content (type: text)
-            - langchain_metadata (type: JSON)
+        - page_content (type: text)
+        - langchain_metadata (type: JSON)
 
         Args:
           engine: MSSQLEngine object to connect to the MSSQL database.
           table_name: The name of table for saving documents.
           content_column (str): The column to store document content.
             Deafult: `page_content`. Optional.
           metadata_json_column (str): The name of the JSON column to use as the metadata’s base
```

## langchain_google_cloud_sql_mssql/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## Comparing `langchain_google_cloud_sql_mssql-0.1.0.dist-info/LICENSE` & `langchain_google_cloud_sql_mssql-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_mssql-0.1.0.dist-info/METADATA` & `langchain_google_cloud_sql_mssql-0.2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-mssql
-Version: 0.1.0
+Version: 0.2.0
 Summary: LangChain integrations for Google Cloud SQL for SQL Server
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,125 +206,169 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-cloud-sql-mssql-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-cloud-sql-mssql-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/CHANGELOG.md
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
 Requires-Dist: langchain-core <1.0.0,>=0.1.25
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Requires-Dist: SQLAlchemy <3.0.0,>=2.0.7
 Requires-Dist: sqlalchemy-pytds <2.0.0,>=1.0.0
 Requires-Dist: cloud-sql-python-connector[pytds] <2.0.0,>=1.7.0
 Provides-Extra: test
-Requires-Dist: black[jupyter] ==23.12.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: langchain ==0.1.8 ; extra == 'test'
-Requires-Dist: mypy ==1.7.1 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.0 ; extra == 'test'
+Requires-Dist: langchain ==0.1.12 ; extra == 'test'
+Requires-Dist: mypy ==1.9.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
-# Cloud SQL for SQL Server for LangChain
+Cloud SQL for SQL Server for LangChain
+======================================
 
-This package contains the [LangChain][langchain] integrations for Cloud SQL for SQL Server.
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
+- `Client Library Documentation`_
+- `Product Documentation`_
 
-* [Documentation][docs]
-* [API Reference]()
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://cloud.google.com/products#product-launch-stages
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-cloud-sql-mssql.svg
+   :target: https://pypi.org/project/langchain-google-cloud-sql-mssql/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-cloud-sql-mssql.svg
+   :target: https://pypi.org/project/langchain-google-cloud-sql-mssql/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-cloud-sql-mssql/latest
+.. _Product Documentation: https://cloud.google.com/sql/sqlserver
 
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
-<your-env>/bin/pip install langchain-google-cloud-sql-mssql
-```
+With `virtualenv`_, it’s possible to install this library without needing system install permissions, and without clashing with the installed system dependencies.
 
-## Document Loader Usage
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Use a [document loader](https://python.langchain.com/docs/modules/data_connection/document_loaders/) to load data as LangChain `Document`s.
+Python >= 3.8
 
-```python
-from langchain_google_cloud_sql_mssql import MSSQLEngine, MSSQLLoader
+Mac/Linux
+^^^^^^^^^
 
+.. code-block:: console
 
-engine = MSSQLEngine.from_instance("project-id", "region", "my-instance", "my-database", "db_user", "db_pass")
-loader = MSSQLLoader(
-    engine,
-    table_name="my-table-name"
-)
-docs = loader.lazy_load()
-```
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-cloud-sql-mssql
 
-See the full [Document Loader][loader] tutorial.
+Windows
+^^^^^^^
 
-## Chat Message History Usage
+.. code-block:: console
 
-Use [`ChatMessageHistory`](https://python.langchain.com/docs/modules/memory/chat_messages/) to store messages and provide conversation history to LLMs.
+   pip install virtualenv
+   virtualenv <your-env>
+   <your-env>\Scripts\activate
+   <your-env>\Scripts\pip.exe install langchain-google-cloud-sql-mssql
 
-```python
-from langchain_google_cloud_sql_mssql import MSSQLChatMessageHistory, MSSQLEngine
 
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
 
-engine = MSSQLEngine.from_instance("project-id", "region", "my-instance", "my-database", "db_user", "db_pass")
-history = MSSQLChatMessageHistory(
-    engine,
-    table_name="my-message-store",
-    session_id="my-session_id"
-)
-```
+Use a document loader to load data as LangChain ``Document``\ s.
 
-See the full [Chat Message History][history] tutorial.
+.. code-block:: python
 
-## Contributing
+    from langchain_google_cloud_sql_mssql import MSSQLEngine, MSSQLLoader
+
+    engine = MSSQLEngine.from_instance("project-id", "region", "my-instance", "my-database", "db_user", "db_pass")
+    loader = MSSQLLoader(
+        engine,
+        table_name="my-table-name"
+    )
+    docs = loader.lazy_load()
+
+See the full `Document Loader`_ tutorial.
+
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/docs/document_loader.ipynb
+
+Chat Message History Usage
+--------------------------
+
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
+
+.. code:: python
+
+    from langchain_google_cloud_sql_mssql import MSSQLChatMessageHistory, MSSQLEngine
+
+    engine = MSSQLEngine.from_instance("project-id", "region", "my-instance", "my-database", "db_user", "db_pass")
+    history = MSSQLChatMessageHistory(
+        engine,
+        table_name="my-message-store",
+        session_id="my-session_id"
+    )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/docs/chat_message_history.ipynb
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING][contributing] for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct][coc] for more
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/CODE_OF_CONDUCT.md
+
+
+License
+-------
 
-Apache 2.0 - See [LICENSE][license] for more information.
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/blob/main/LICENSE>`_
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
-[loader]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/docs/document_loader.ipynb
-[history]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[docs]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/docs
-[license]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/LICENSE
-[contributing]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/CONTRIBUTING.md
-[coc]: https://github.com/googleapis/langchain-google-cloud-sql-mssql-python/tree/main/CODE_OF_CONDUCT.md
```

## Comparing `langchain_google_cloud_sql_mssql-0.1.0.dist-info/RECORD` & `langchain_google_cloud_sql_mssql-0.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 langchain_google_cloud_sql_mssql/__init__.py,sha256=fTr4QKWQH9ZoEmvLThfz7eskNmWcNoev2axCeRO8Xns,879
 langchain_google_cloud_sql_mssql/chat_message_history.py,sha256=tD3yRy_GO4CHXld4dM-GZN0c3TObbsJ6nWN0dtgsFa8,4641
-langchain_google_cloud_sql_mssql/engine.py,sha256=Z_d-QSdsrvJXkCAy20jC_0LfGCxIt-O7GJAqSu0LgtA,7715
-langchain_google_cloud_sql_mssql/loader.py,sha256=cut-LWyQAtSgjiPOLgKYfVXP_kMXdsAJ92vUqLLcx-k,11243
+langchain_google_cloud_sql_mssql/engine.py,sha256=scpUdei-d1H97qt8HUjhtq5o09enibBdPMMhJXu5agI,7727
+langchain_google_cloud_sql_mssql/loader.py,sha256=UGcUT9zr9CHSO_UG9hHIMt0EFHILffxLULHepob_T-k,11253
 langchain_google_cloud_sql_mssql/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_cloud_sql_mssql/version.py,sha256=RuXdOB4FN_GOqGKFzaNfTuwuWOqyoQLC1DkG2RBXgGw,597
-langchain_google_cloud_sql_mssql-0.1.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_cloud_sql_mssql-0.1.0.dist-info/METADATA,sha256=oG3KrnRbm3KdESJZN4DylWvf99grdXoZ2gphabnBJEE,18318
-langchain_google_cloud_sql_mssql-0.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-langchain_google_cloud_sql_mssql-0.1.0.dist-info/top_level.txt,sha256=usQ5y0MkucRrezlQq53jf42wz750dTSX9Tq2A_TYADM,33
-langchain_google_cloud_sql_mssql-0.1.0.dist-info/RECORD,,
+langchain_google_cloud_sql_mssql/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
+langchain_google_cloud_sql_mssql-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_cloud_sql_mssql-0.2.0.dist-info/METADATA,sha256=NGrdKc6lm8T_vkKq4yMlcmIXdW_F4ibBWVnXRChjTOI,19294
+langchain_google_cloud_sql_mssql-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_cloud_sql_mssql-0.2.0.dist-info/top_level.txt,sha256=usQ5y0MkucRrezlQq53jf42wz750dTSX9Tq2A_TYADM,33
+langchain_google_cloud_sql_mssql-0.2.0.dist-info/RECORD,,
```

