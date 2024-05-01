# Comparing `tmp/sqlalchemy_tx_context-0.2.0.tar.gz` & `tmp/sqlalchemy_tx_context-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_tx_context-0.2.0.tar", last modified: Wed Mar 27 20:59:33 2024, max compression
+gzip compressed data, was "sqlalchemy_tx_context-0.2.1.tar", last modified: Wed May  1 16:24:08 2024, max compression
```

## Comparing `sqlalchemy_tx_context-0.2.0.tar` & `sqlalchemy_tx_context-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-27 20:59:33.048507 sqlalchemy_tx_context-0.2.0/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 sqlalchemy_tx_context-0.2.0/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-03-27 20:59:33.048507 sqlalchemy_tx_context-0.2.0/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2512 2024-03-27 20:51:31.000000 sqlalchemy_tx_context-0.2.0/README.md
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-03-27 20:59:33.048507 sqlalchemy_tx_context-0.2.0/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      795 2024-03-27 20:59:02.000000 sqlalchemy_tx_context-0.2.0/setup.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-27 20:59:33.044507 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5009 2024-03-27 20:26:03.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       71 2024-03-22 08:33:51.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5591 2024-03-27 20:06:20.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/__init__.pyi
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-27 20:59:33.048507 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      767 2024-03-21 18:14:54.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/CompoundSelect.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4514 2024-03-24 14:14:37.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Delete.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      781 2024-03-24 14:09:36.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/ExecuteMixin.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-24 14:13:14.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Exists.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5507 2024-03-24 14:14:45.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Insert.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      701 2024-03-24 13:57:12.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Rowcount.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      185 2024-03-24 14:14:11.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Select.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4692 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Update.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2587 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/WithDataMixin.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      178 2024-03-21 18:36:38.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-03-27 20:59:33.044507 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-03-27 20:59:32.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      788 2024-03-27 20:59:32.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-03-27 20:59:32.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       51 2024-03-27 20:59:32.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-03-27 20:59:32.000000 sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/top_level.txt
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 16:24:08.572877 sqlalchemy_tx_context-0.2.1/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 sqlalchemy_tx_context-0.2.1/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-01 16:24:08.572877 sqlalchemy_tx_context-0.2.1/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2512 2024-03-27 21:02:21.000000 sqlalchemy_tx_context-0.2.1/README.md
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-01 16:24:08.572877 sqlalchemy_tx_context-0.2.1/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      795 2024-05-01 16:21:41.000000 sqlalchemy_tx_context-0.2.1/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 16:24:08.568877 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5241 2024-05-01 16:17:05.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       71 2024-03-22 08:33:51.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5575 2024-05-01 16:21:00.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/__init__.pyi
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 16:24:08.568877 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      767 2024-03-21 18:14:54.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/CompoundSelect.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4514 2024-03-24 14:14:37.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Delete.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      781 2024-03-24 14:09:36.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/ExecuteMixin.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      934 2024-03-24 14:13:14.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Exists.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5507 2024-03-24 14:14:45.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Insert.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      701 2024-03-24 13:57:12.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Rowcount.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      185 2024-03-24 14:14:11.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Select.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4692 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Update.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2587 2024-03-24 14:15:02.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/WithDataMixin.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      178 2024-03-21 18:36:38.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-01 16:24:08.568877 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2877 2024-05-01 16:24:08.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      788 2024-05-01 16:24:08.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-01 16:24:08.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       51 2024-05-01 16:24:08.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-05-01 16:24:08.000000 sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/top_level.txt
```

### Comparing `sqlalchemy_tx_context-0.2.0/LICENSE` & `sqlalchemy_tx_context-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/PKG-INFO` & `sqlalchemy_tx_context-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_tx_context
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension for sqlalchemy
 Home-page: https://github.com/QuisEgoSum/sqlalchemy-tx-context
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: sqlalchemy
 Platform: UNKNOWN
```

### Comparing `sqlalchemy_tx_context-0.2.0/README.md` & `sqlalchemy_tx_context-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/setup.py` & `sqlalchemy_tx_context-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sqlalchemy_tx_context',
-    version='0.2.0',
+    version='0.2.1',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='An extension for sqlalchemy',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/sqlalchemy-tx-context',
     packages=find_packages(exclude=['tmp', 'example']),
```

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/SQLAlchemyTransactionContext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import typing
 import contextvars
 from contextlib import asynccontextmanager
 
 import sqlalchemy
 from sqlalchemy.ext.asyncio import AsyncEngine, async_sessionmaker, AsyncSessionTransaction
 from sqlalchemy.ext.asyncio import AsyncSession
-
+from sqlalchemy.sql import roles
 
 FIELD_PROPERTIES = frozenset([
     'query',
     'context'
 ])
 
+IGNORE_PROPERTIES = frozenset([
+    'compile',
+    'alias',
+    'subquery'
+])
+
 EXECUTE_PROPERTIES = frozenset([
     'execute',
     'scalar',
     'scalars',
     'first',
     'all',
     'mapped_first',
@@ -74,14 +80,18 @@
 
     def __getattribute__(self, item):
         if item in FIELD_PROPERTIES:
             return object.__getattribute__(self, item)
         elif item in EXECUTE_PROPERTIES:
             return _execute_query(self.context, self.query, item)
         value = object.__getattribute__(self.query, item)
+        if item.startswith('_'):
+            return value
+        if item in IGNORE_PROPERTIES:
+            return value
         if not callable(value):
             return value
 
         def wrapper(*args, **kwargs):
             self.query = value(*args, **kwargs)
             return self
         return wrapper
```

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/__init__.pyi` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, overload, Any, Optional, Union, ContextManager, AsyncContextManager
+from typing import TYPE_CHECKING, overload, Any, Optional, Union, AsyncContextManager
 
 from sqlalchemy import ScalarSelect, SelectBase
 from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, AsyncSessionTransaction
 
 from .types import Insert, Select, Update, Delete, Exists, CompoundSelect
 
 if TYPE_CHECKING:
```

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/CompoundSelect.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/CompoundSelect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Delete.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Delete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/ExecuteMixin.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/ExecuteMixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Exists.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Exists.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Insert.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Insert.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Rowcount.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Rowcount.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/Update.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/Update.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context/types/WithDataMixin.py` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context/types/WithDataMixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/PKG-INFO` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-tx-context
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension for sqlalchemy
 Home-page: https://github.com/QuisEgoSum/sqlalchemy-tx-context
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: sqlalchemy
 Platform: UNKNOWN
```

### Comparing `sqlalchemy_tx_context-0.2.0/sqlalchemy_tx_context.egg-info/SOURCES.txt` & `sqlalchemy_tx_context-0.2.1/sqlalchemy_tx_context.egg-info/SOURCES.txt`

 * *Files identical despite different names*

