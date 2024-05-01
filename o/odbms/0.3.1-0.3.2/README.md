# Comparing `tmp/odbms-0.3.1.tar.gz` & `tmp/odbms-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbms-0.3.1.tar", last modified: Thu Apr 18 18:44:42 2024, max compression
+gzip compressed data, was "odbms-0.3.2.tar", last modified: Wed May  1 15:03:19 2024, max compression
```

## Comparing `odbms-0.3.1.tar` & `odbms-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:44:42.362128 odbms-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 18:44:38.000000 odbms-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 18:44:38.000000 odbms-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 18:44:42.358128 odbms-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 18:44:38.000000 odbms-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:44:42.358128 odbms-0.3.1/odbms/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/dbms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:44:42.358128 odbms-0.3.1/odbms/orms/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/postgresqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-18 18:44:38.000000 odbms-0.3.1/odbms/orms/sqlitedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:44:42.358128 odbms-0.3.1/odbms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 18:44:42.000000 odbms-0.3.1/odbms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 18:44:42.000000 odbms-0.3.1/odbms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:44:42.000000 odbms-0.3.1/odbms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 18:44:42.000000 odbms-0.3.1/odbms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 18:44:42.000000 odbms-0.3.1/odbms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:44:42.362128 odbms-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-18 18:44:38.000000 odbms-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.969566 odbms-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-01 15:03:15.000000 odbms-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 15:03:15.000000 odbms-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 15:03:19.965566 odbms-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 15:03:15.000000 odbms-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/dbms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms/orms/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/postgresqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-01 15:03:15.000000 odbms-0.3.2/odbms/orms/sqlitedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:03:19.965566 odbms-0.3.2/odbms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:03:19.000000 odbms-0.3.2/odbms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:03:19.969566 odbms-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-01 15:03:15.000000 odbms-0.3.2/setup.py
```

### Comparing `odbms-0.3.1/LICENSE` & `odbms-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/PKG-INFO` & `odbms-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.3.1
+Version: 0.3.2
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.3.1/odbms/database.py` & `odbms-0.3.2/odbms/database.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/dbms.py` & `odbms-0.3.2/odbms/dbms.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/model.py` & `odbms-0.3.2/odbms/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             if not updated_at else updated_at
         self.id = ObjectId() if not id else str(id)
 
     
     @classmethod
     def create_table(cls):
         """
-        Create the database table for the model (Only for non-MongoDB databases).
+        Create the database table for the model (Only for relational databases).
         """
         if DBMS.Database.dbms != 'mongodb':
             excluded = ['created_at', 'updated_at', 'id']
             columns = []
             additional_columns = {
                 'sqlite': [
                     'created_at TEXT NOT NULL DEFAULT CURRENT_TIMESTAMP',
@@ -58,18 +58,18 @@
             all_parameters = init_parameters
             
             for param in all_parameters:
                 param_name = param.name
                 param_type = param.annotation
                 
                 column_type = cls.get_column_type(param_type)
-                if column_type:
-                    if param_name not in excluded:
-                        column_def = f"{param_name} {column_type}"
-                        columns.append(column_def)
+                
+                if param_name not in excluded:
+                    column_def = f"{param_name} {column_type}"
+                    columns.append(column_def)
                         
             columns += additional_columns.get(DBMS.Database.dbms, [])
             columns_str = ', '.join(columns)
             table_definition = f"CREATE TABLE IF NOT EXISTS {cls.TABLE_NAME} ({columns_str});"
             
             DBMS.Database.execute(table_definition)
             
@@ -99,18 +99,19 @@
         """
         
         type_mapping = {
             str: "TEXT",
             int: "INTEGER",
             float: "REAL",
             bool: "BOOLEAN",
-            list: "TEXT"
+            list: "TEXT",
+            dict: "TEXT"
             # Add more mappings as needed
         }
-        return type_mapping.get(attr_type, "")
+        return type_mapping.get(attr_type, "TEXT")
 
     def save(self):
         '''
         Instance Method for saving Model instance to database
 
         @params None
         @return None
@@ -123,15 +124,15 @@
             del data["created_at"]
             del data["updated_at"]
 
         if isinstance(self.id, ObjectId):
             return DBMS.Database.insert(self.TABLE_NAME, Model.normalise(data, 'params'))
         
         # Update the existing record in database
-        del data['password']
+        data.pop('id', None)
         return DBMS.Database.update(self.TABLE_NAME, self.normalise({'id': self.id}, 'params'), self.normalise(data, 'params'))
 
     @staticmethod
     def insert(document):
         '''
         Static Method for saving documents into database
 
@@ -323,15 +324,17 @@
         Class Method for retrieving one model
         imstance by provided parameters
 
         @param params
         @return List[Model]
         '''
 
-        return cls(**cls.normalise(DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise(params, 'params'), projection))) # type: ignore
+        result = cls.normalise(DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise(params, 'params'), projection))
+
+        return cls(**result) if len(result.keys()) else None
     
     @classmethod
     def query(cls, column: str, search: str):
         '''
         Class Method for retrieving products
         by their names
 
@@ -429,17 +432,19 @@
         Instance Method for converting Model Instance to Dict
 
         @paramas None
         @return dict() format of Function instance
         '''
         
         data = self.__dict__.copy()
+        
+        data['created_at'] = data['created_at'].strftime("%a %b %d %Y %H:%M:%S")
+        data['updated_at'] = data['updated_at'].strftime("%a %b %d %Y %H:%M:%S")
 
-        if 'password' in data.keys():
-            del data['password']
+        data.pop('password', None)
 
         return data
     
     @classmethod
     def normalise(cls, content: dict|None, optype: str = 'dbresult')-> dict:
         '''
         Static method of normalising database results\n
@@ -476,17 +481,36 @@
                         content[key] = '::'.join([str(v) for v in value])
                 normalized = content
             return normalized
         else:
             if optype == 'params':
                 if 'id' in content.keys():
                     content['id'] = str(content['id'])
-            for key, value in content.items():
-                if type(value) == list:
-                    content[key] = '::'.join([str(v) for v in value])
-
-                elif type(value) == datetime:
-                    content[key] = value.strftime("%a %b %d %Y %H:%M:%S")
-                elif type(value) == dict:
-                    content[key] = json.dumps(value) # type: ignore
+                for key, value in content.items():
+                    if type(value) == list:
+                        content[key] = '::'.join([str(v) for v in value])
+
+                    elif type(value) == datetime:
+                        content[key] = value.strftime("%a %b %d %Y %H:%M:%S")
+                    elif type(value) == dict:
+                        content[key] = json.dumps(value) # type: ignore
+            else:
+                init_signatures = inspect.signature(cls.__init__)
+            
+                init_parameters = [param for param in init_signatures.parameters.values()
+                                if param.name != 'self']
+                
+                all_parameters = init_parameters
+                type_mapping = [str, int, float, bool, list, dict]
+                for param in all_parameters:
+                    param_name = param.name
+                    param_type = param.annotation
+                    
+                    if param_type in type_mapping:
+                        if param_type is dict:
+                            content[param_name] = json.loads(content[param_name])
+                        elif param_type is list:
+                            content[param_name] = content[param_name].split('::')
+                        else:
+                            content[param_name] = param_type(content[param_name])
             
-        return content
+        return content
```

### Comparing `odbms-0.3.1/odbms/orms/base.py` & `odbms-0.3.2/odbms/orms/base.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/orms/mongodb.py` & `odbms-0.3.2/odbms/orms/mongodb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/orms/mysqldb.py` & `odbms-0.3.2/odbms/orms/mysqldb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/orms/postgresqldb.py` & `odbms-0.3.2/odbms/orms/postgresqldb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms/orms/sqlitedb.py` & `odbms-0.3.2/odbms/orms/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.3.1/odbms.egg-info/PKG-INFO` & `odbms-0.3.2/odbms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.3.1
+Version: 0.3.2
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.3.1/setup.py` & `odbms-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='odbms',
     version=VERSION,
```

