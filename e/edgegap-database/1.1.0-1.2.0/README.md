# Comparing `tmp/edgegap_database-1.1.0.tar.gz` & `tmp/edgegap_database-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_database-1.2.0.tar", max compression
```

## Comparing `edgegap_database-1.1.0.tar` & `edgegap_database-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/BUILD
--rw-r--r--   0        0        0      386 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/__init__.py
--rw-r--r--   0        0        0      624 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_base.py
--rw-r--r--   0        0        0      452 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1004 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_engine.py
--rw-r--r--   0        0        0      885 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_factory.py
--rw-r--r--   0        0        0      253 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_model.py
--rw-r--r--   0        0        0     2555 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/_session.py
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/errors/BUILD
--rw-r--r--   0        0        0      325 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-04-30 16:04:37.495396 edgegap_database-1.1.0/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      542 2024-04-30 16:05:08.755659 edgegap_database-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/BUILD
+-rw-r--r--   0        0        0      387 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_base.py
+-rw-r--r--   0        0        0      452 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1005 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      885 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      253 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2555 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/_session.py
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/BUILD
+-rw-r--r--   0        0        0      327 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-01 17:52:18.963014 edgegap_database-1.2.0/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      743 2024-05-01 17:52:42.971603 edgegap_database-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.2.0/PKG-INFO
```

### Comparing `edgegap_database-1.1.0/LICENSE` & `edgegap_database-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.1.0/README.md` & `edgegap_database-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.1.0/edgegap_database/_base.py` & `edgegap_database-1.2.0/edgegap_database/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
 
 import sqlalchemy as sa
-from sqlmodel import SQLModel, Field
+from sqlmodel import Field, SQLModel
 
 
 class BaseModel(SQLModel, table=False):
     id: int | None = Field(default=None, primary_key=True)
     created_at: datetime | None = Field(
         default=None,
         sa_type=sa.DateTime(timezone=True),
-        sa_column_kwargs={"server_default": sa.func.now()},
+        sa_column_kwargs={'server_default': sa.func.now()},
         nullable=False,
     )
     updated_at: datetime | None = Field(
         default=None,
         sa_type=sa.DateTime(timezone=True),
         sa_column_kwargs={
-            "onupdate": sa.func.now(),
-            "server_default": sa.func.now()
+            'onupdate': sa.func.now(),
+            'server_default': sa.func.now(),
         },
     )
```

### Comparing `edgegap_database-1.1.0/edgegap_database/_engine.py` & `edgegap_database-1.2.0/edgegap_database/_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     __instance: '__Engine'
 
     class __Engine:
         def __init__(self, configuration: DatabaseConfiguration):
             self.__configuration = configuration
             self.__engine = create_engine(
                 url=str(self.__configuration.uri),
-                connect_args=self.__configuration.args or {}
+                connect_args=self.__configuration.args or {},
             )
 
         def get_engine(self):
             return self.__engine
 
     def __init__(self, configuration: DatabaseConfiguration):
         key = configuration.application
```

### Comparing `edgegap_database-1.1.0/edgegap_database/_factory.py` & `edgegap_database-1.2.0/edgegap_database/_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 from ._configuration import DatabaseConfiguration
 from ._model import SQLiteDsn
 
 logger = logging.getLogger(__name__)
 
 
 class DatabaseConfigurationFactory:
-
     @staticmethod
     def __parse(conf: DatabaseConfiguration) -> DatabaseConfiguration:
         if conf.application is None:
-            conf.application = "DefaultApplicationName"
+            conf.application = 'DefaultApplicationName'
 
         if not isinstance(conf.args, dict):
             conf.args = {}
 
         conf.args.update({
-            "application_name": conf.application,
-            "options": "-c timezone=utc"
+            'application_name': conf.application,
+            'options': '-c timezone=utc',
         })
 
         return conf
 
     def from_uri(self, uri: str | MultiHostUrl | PostgresDsn | SQLiteDsn, name: str) -> DatabaseConfiguration:
         configuration = DatabaseConfiguration(uri=str(uri), application=name)
```

### Comparing `edgegap_database-1.1.0/edgegap_database/_operator.py` & `edgegap_database-1.2.0/edgegap_database/_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from datetime import datetime, timezone
 from typing import Any
 
-from sqlalchemy.engine import TupleResult, ScalarResult
-from sqlmodel import SQLModel, Session
+from sqlalchemy.engine import ScalarResult, TupleResult
+from sqlmodel import Session, SQLModel
 from sqlmodel.sql import expression
 
 from .errors import DatabaseExceptionFactory
 
 logger = logging.getLogger(__name__)
```

### Comparing `edgegap_database-1.1.0/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.2.0/edgegap_database/errors/_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from sqlalchemy.exc import DBAPIError
 
 
 class DatabaseException(Exception):
-    default_message = "Database Exception"
+    default_message = 'Database Exception'
 
     def __init__(self, message: str | None = None, exception: type(DBAPIError) = None):
         default_message = str(exception) if exception is not None else self.default_message
         self.message = message or default_message
         self.db_exception = exception
 
 
 class DatabaseConfigurationExceptions(DatabaseException):
-    default_message = "Database Configuration Exception, please verify your configuration"
+    default_message = 'Database Configuration Exception, please verify your configuration'
 
 
 class DatabaseUniqueViolationExceptions(DatabaseException):
-    default_message = "Database Unique Violation Exception, please verify your Unique Violation"
+    default_message = 'Database Unique Violation Exception, please verify your Unique Violation'
```

### Comparing `edgegap_database-1.1.0/pyproject.toml` & `edgegap_database-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.1.0"
+version = "1.2.0"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
 psycopg2 = "^2.9.9"
 sqlmodel = "^0.0.16"
 alembic = "^1.13.1"
 pydantic = "^2.7.1"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
+ruff = "^0.4.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+extend = "../../../3rdparty/ruff/ruff.toml"
```

### Comparing `edgegap_database-1.1.0/PKG-INFO` & `edgegap_database-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

