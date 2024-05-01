# Comparing `tmp/mongodb_orm-0.0.129a1.tar.gz` & `tmp/mongodb_orm-0.0.129a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.129a1.tar", last modified: Wed May  1 09:46:48 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.129a2.tar", last modified: Wed May  1 10:28:58 2024, max compression
```

## Comparing `mongodb_orm-0.0.129a1.tar` & `mongodb_orm-0.0.129a2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:48.323901 mongodb_orm-0.0.129a1/
--rw-rw-rw-   0        0        0      348 2024-05-01 09:46:48.321903 mongodb_orm-0.0.129a1/PKG-INFO
--rw-rw-rw-   0        0        0      593 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.293918 mongodb_orm-0.0.129a1/mongodb_orm/
--rw-rw-rw-   0        0        0       95 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/__init__.py
--rw-rw-rw-   0        0        0      489 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.365462 mongodb_orm-0.0.129a1/mongodb_orm/custom_urls/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/custom_urls/__init__.py
--rw-rw-rw-   0        0        0     1543 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a1/mongodb_orm/custom_urls/bread_urls.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.418962 mongodb_orm-0.0.129a1/mongodb_orm/decorators/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/decorators/__init__.py
--rw-rw-rw-   0        0        0      483 2024-05-01 09:35:34.000000 mongodb_orm-0.0.129a1/mongodb_orm/decorators/chained.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.477841 mongodb_orm-0.0.129a1/mongodb_orm/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/exceptions/__init__.py
--rw-rw-rw-   0        0        0      142 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/exceptions/syntax_exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.657991 mongodb_orm-0.0.129a1/mongodb_orm/interfaces/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2671 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/interfaces/base_mongodb_model.py
--rw-rw-rw-   0        0        0     7730 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/interfaces/mongodb_model.py
--rw-rw-rw-   0        0        0      826 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/interfaces/mongodb_model_events.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.715686 mongodb_orm-0.0.129a1/mongodb_orm/management/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.723695 mongodb_orm-0.0.129a1/mongodb_orm/management/commands/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4650 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/management/commands/update_schema.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.789875 mongodb_orm-0.0.129a1/mongodb_orm/models/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.796873 mongodb_orm-0.0.129a1/mongodb_orm/singletons/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/singletons/__init__.py
--rw-rw-rw-   0        0        0      392 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:48.122089 mongodb_orm-0.0.129a1/mongodb_orm/types/
--rw-rw-rw-   0        0        0      530 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/Relation.py
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/__init__.py
--rw-rw-rw-   0        0        0      136 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/index.py
--rw-rw-rw-   0        0        0      440 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/logger_object.py
--rw-rw-rw-   0        0        0      481 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/model_schema.py
--rw-rw-rw-   0        0        0      382 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/types/options.py
--rw-rw-rw-   0        0        0      196 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a1/mongodb_orm/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:48.195058 mongodb_orm-0.0.129a1/mongodb_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/utils/__init__.py
--rw-rw-rw-   0        0        0     1196 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:48.259517 mongodb_orm-0.0.129a1/mongodb_orm/views/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/views/__init__.py
--rw-rw-rw-   0        0        0     3978 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a1/mongodb_orm/views/mongodb_api_model_view.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:46:47.358932 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/
--rw-rw-rw-   0        0        0      348 2024-05-01 09:46:46.000000 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2024-05-01 09:46:47.000000 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 09:46:46.000000 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-01 09:46:46.000000 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 09:46:46.000000 mongodb_orm-0.0.129a1/mongodb_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 09:46:48.323901 mongodb_orm-0.0.129a1/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-01 09:32:03.000000 mongodb_orm-0.0.129a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.875768 mongodb_orm-0.0.129a2/
+-rw-rw-rw-   0        0        0      348 2024-05-01 10:28:58.870766 mongodb_orm-0.0.129a2/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.698738 mongodb_orm-0.0.129a2/mongodb_orm/
+-rw-rw-rw-   0        0        0       95 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/__init__.py
+-rw-rw-rw-   0        0        0      489 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.729738 mongodb_orm-0.0.129a2/mongodb_orm/custom_urls/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/custom_urls/__init__.py
+-rw-rw-rw-   0        0        0     1543 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a2/mongodb_orm/custom_urls/bread_urls.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.738751 mongodb_orm-0.0.129a2/mongodb_orm/decorators/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/decorators/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-05-01 09:35:34.000000 mongodb_orm-0.0.129a2/mongodb_orm/decorators/chained.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.752743 mongodb_orm-0.0.129a2/mongodb_orm/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      142 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/exceptions/syntax_exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.773751 mongodb_orm-0.0.129a2/mongodb_orm/interfaces/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2671 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-rw-rw-   0        0        0     7736 2024-05-01 10:27:38.000000 mongodb_orm-0.0.129a2/mongodb_orm/interfaces/mongodb_model.py
+-rw-rw-rw-   0        0        0      826 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/interfaces/mongodb_model_events.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.779743 mongodb_orm-0.0.129a2/mongodb_orm/management/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.790733 mongodb_orm-0.0.129a2/mongodb_orm/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4650 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/management/commands/update_schema.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.796743 mongodb_orm-0.0.129a2/mongodb_orm/models/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.805737 mongodb_orm-0.0.129a2/mongodb_orm/singletons/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/singletons/__init__.py
+-rw-rw-rw-   0        0        0      392 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.842011 mongodb_orm-0.0.129a2/mongodb_orm/types/
+-rw-rw-rw-   0        0        0      530 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/Relation.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/__init__.py
+-rw-rw-rw-   0        0        0      136 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/index.py
+-rw-rw-rw-   0        0        0      440 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/logger_object.py
+-rw-rw-rw-   0        0        0      481 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/model_schema.py
+-rw-rw-rw-   0        0        0      382 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/types/options.py
+-rw-rw-rw-   0        0        0      196 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a2/mongodb_orm/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.855004 mongodb_orm-0.0.129a2/mongodb_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/utils/__init__.py
+-rw-rw-rw-   0        0        0     1196 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.866016 mongodb_orm-0.0.129a2/mongodb_orm/views/
+-rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/views/__init__.py
+-rw-rw-rw-   0        0        0     3978 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a2/mongodb_orm/views/mongodb_api_model_view.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:28:58.720939 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/
+-rw-rw-rw-   0        0        0      348 2024-05-01 10:28:58.000000 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2024-05-01 10:28:58.000000 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:28:58.000000 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-01 10:28:58.000000 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 10:28:58.000000 mongodb_orm-0.0.129a2/mongodb_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 10:28:58.875768 mongodb_orm-0.0.129a2/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-05-01 10:28:48.000000 mongodb_orm-0.0.129a2/setup.py
```

### Comparing `mongodb_orm-0.0.129a1/README.md` & `mongodb_orm-0.0.129a2/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.129a2/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.129a2/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.129a2/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self._result: Cursor | InsertOneResult | dict | None = None
         self.chained = True
 
     def query(self) -> 'MongoDBModel':
         self.chained = False
         return self
 
-    def json(self) -> List[dict] | dict:
+    def json(self) -> Union[List[dict], dict]:
         if self._result is None:
             raise ChainingError(message='you can not call json directly, it needs to be chained')
         if isinstance(self._result, Cursor):
             return [Helper.standardize_dict(item, underscore=True) for item in list(self._result)]
         else:
             return Helper.standardize_dict(self._result, underscore=True)
```

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.0.129a2/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.129a2/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/types/Relation.py` & `mongodb_orm-0.0.129a2/mongodb_orm/types/Relation.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.0.129a2/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.129a2/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.129a2/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.129a1/setup.py` & `mongodb_orm-0.0.129a2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.129-alpha.1",
+    version="0.0.129-alpha.2",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```
