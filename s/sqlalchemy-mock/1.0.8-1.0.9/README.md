# Comparing `tmp/sqlalchemy_mock-1.0.8.tar.gz` & `tmp/sqlalchemy_mock-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.8.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.9.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.8.tar` & `sqlalchemy_mock-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.8/README.md
--rw-r--r--   0        0        0      448 2023-08-22 22:07:07.481536 sqlalchemy_mock-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.8/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.8/sqlalchemy_mock/async_session.py
--rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.8/sqlalchemy_mock/execute.py
--rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.8/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     3508 2023-07-03 19:53:53.223210 sqlalchemy_mock-1.0.8/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     5228 2023-08-22 22:06:54.266005 sqlalchemy_mock-1.0.8/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.9/README.md
+-rw-r--r--   0        0        0      448 2024-05-01 16:51:12.107527 sqlalchemy_mock-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.9/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.9/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.9/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.9/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3508 2023-07-03 19:53:53.223210 sqlalchemy_mock-1.0.9/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     5363 2024-05-01 16:48:06.921740 sqlalchemy_mock-1.0.9/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.9/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.8/README.md` & `sqlalchemy_mock-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.8/sqlalchemy_mock/execute.py` & `sqlalchemy_mock-1.0.9/sqlalchemy_mock/execute.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.8/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.9/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.8/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.9/sqlalchemy_mock/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.8/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.9/sqlalchemy_mock/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         "utcnow": datetime.datetime.utcnow
     }
 
     for column in record.__class__.__table__._columns:
         if column.default and not getattr(record, column.name, None):
             value = column.default.arg
             if isinstance(column.default.arg, FunctionType):
+                value_wrapped = getattr(value, "__wrapped__", None)
+                value = value_wrapped if value_wrapped else value
+
                 value = functions.get(column.default.arg.__name__, value)()
             setattr(record, column.name, value)
 
 
 def mock_sessions_methods(session: object):
     db_mock_methods = {method: unittest.mock.MagicMock(side_effect=getattr(session, method)) for method in ("query", "add", "add_all", "commit", "refresh", "execute", "bulk_insert_mappings")}
     return unittest.mock.patch.multiple(sqlalchemy.orm.Session, **db_mock_methods)
```

### Comparing `sqlalchemy_mock-1.0.8/PKG-INFO` & `sqlalchemy_mock-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.8
+Version: 1.0.9
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

