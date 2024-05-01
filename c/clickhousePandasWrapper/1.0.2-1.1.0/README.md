# Comparing `tmp/clickhousePandasWrapper-1.0.2.tar.gz` & `tmp/clickhousepandaswrapper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhousePandasWrapper-1.0.2.tar", last modified: Mon Feb 19 19:41:44 2024, max compression
+gzip compressed data, was "clickhousepandaswrapper-1.1.0.tar", last modified: Wed May  1 01:51:23 2024, max compression
```

## Comparing `clickhousePandasWrapper-1.0.2.tar` & `clickhousepandaswrapper-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:41:44.791204 clickhousePandasWrapper-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-19 19:41:36.000000 clickhousePandasWrapper-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-19 19:41:44.791204 clickhousePandasWrapper-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-19 19:41:36.000000 clickhousePandasWrapper-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:41:44.787204 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-19 19:41:36.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-02-19 19:41:36.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper/insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 19:41:44.791204 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-19 19:41:44.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-19 19:41:44.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 19:41:44.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-19 19:41:44.000000 clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-19 19:41:38.000000 clickhousePandasWrapper-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 19:41:44.791204 clickhousePandasWrapper-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-01 01:51:21.000000 clickhousepandaswrapper-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/setup.cfg
```

### Comparing `clickhousePandasWrapper-1.0.2/LICENSE` & `clickhousepandaswrapper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhousePandasWrapper-1.0.2/PKG-INFO` & `clickhousepandaswrapper-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhousePandasWrapper
-Version: 1.0.2
+Version: 1.1.0
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clickhousePandasWrapper-1.0.2/clickhousePandasWrapper/insert.py` & `clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ```
     insert data
 ```
 clickhouseInserter.insertDataInClickhouse(df=df,table='test')
 ```
     """
     def __init__(self, host='127.0.0.1', port=9000, db='default', columnTypeMap=columnTypeMap, logLevel=None):
-        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger = logging.getLogger(__name__)
         if logLevel:
             if re.match(r"^(warn|warning)$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.WARNING)
             elif re.match(r"^debug$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.DEBUG)
             else:
                 self.logger.setLevel(logging.INFO)
@@ -73,24 +73,25 @@
 
         defName = inspect.stack()[0][3]
         mapping = {
             'int32': 'Int32',
             'int64': 'Int64',
             'float32': 'Float32',
             'float64': 'Float64',
+            'bool': 'Bool',
             'object': 'String',
         }
         if columnName in self.columnTypeMap:
             # define type by column name
             return self.columnTypeMap.get(columnName)
         else:
             # define type by pandas types
             return mapping.get(str(pandasType), 'String')
 
-    def generateCreateTableQuery(self, df, db, table, partitionBy, orderBy):
+    def generateCreateTableQuery(self, df, db, table, engine = 'MergeTree', partitionBy = None, orderBy = None, primaryKey = None, settings = 'index_granularity = 8192'):
         """
         generate create table query
         """
 
         defName = inspect.stack()[0][3]
 
         self.logger.debug(f"{defName}: dtypes={df.dtypes}")
@@ -103,18 +104,31 @@
             if columnsStr:
                 columnsStr = columnsStr + '\n'
             columnsStr = columnsStr +'    `'+ columnName +'` '+ chType +','
         sql = f"""
 CREATE TABLE IF NOT EXISTS {db}.{table} (
 {columnsStr}
 )
-ENGINE MergeTree
+ENGINE {engine}
+"""
+        if primaryKey:
+            sql = sql + f"""
+PRIMARY KEY ({primaryKey})
+"""
+        if partitionBy:
+            sql = sql + f"""
 PARTITION BY ({partitionBy})
+"""
+        if orderBy:
+            sql = sql + f"""
 ORDER BY {orderBy}
-SETTINGS index_granularity = 8192
+"""
+        if settings:
+            sql = sql + f"""
+SETTINGS {settings}
 """
         self.logger.info(f"{defName}: create table sql='{sql}'")
         return sql
 
     def generateAlterQuery(self, df, table, db, partitionByTable, cleanDataWhereColumns=list()):
         """
         generate alter table query
@@ -183,16 +197,18 @@
 
     def insertDataInClickhouse(self,
             df,
             table,
             db=None,
             cleanDataInDateRange=True,
             cleanDataWhereColumns=list(),
+            cleanAllData=False,
             partitionByTable='date',
             partitionByFunction='toYYYYMM',
+            primaryKey=None,
             orderBy=None,
             retryCounter=0
         ):
         """
         insert dataframe in clickhouse
         cleanDataInDateRange - delete data in date range before insert
         partitionByTable - column name for partitioning
@@ -235,39 +251,47 @@
                     )
             else:
                 self.logger.error(f"{defName}: failed execute in clickhouse: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
                 return False
         # }}
         tableExists = any(tbl[0] == table for tbl in tables)
         if tableExists:
-            # clean exists data in table {{
-            if cleanDataInDateRange:
-                alterTable = self.generateAlterQuery(
-                    df = df,
-                    table = table,
-                    db = db,
-                    partitionByTable = partitionByTable,
-                    cleanDataWhereColumns = cleanDataWhereColumns,
-                )
+            # clean exists data in table
+            if cleanDataInDateRange or cleanAllData:
+                if cleanDataInDateRange:
+                    sql = self.generateAlterQuery(
+                        df = df,
+                        table = table,
+                        db = db,
+                        partitionByTable = partitionByTable,
+                        cleanDataWhereColumns = cleanDataWhereColumns,
+                    )
+                elif cleanAllData:
+                    sql = f"TRUNCATE TABLE IF EXISTS {db}.{table}"
                 # clean data
-                self.logger.debug(alterTable)
+                self.logger.debug(sql)
                 try:
-                    self.ch.execute(alterTable)
+                    self.ch.execute(sql)
                 except Exception as e:
                     self.logger.error(f"{defName}: failed execute in clickhouse: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
                     return False
-            # }}
+
         else:
             # create table if not exists
+            if partitionByFunction and partitionByTable:
+                partitionBy = partitionByFunction+'('+partitionByTable+')'
+            else:
+                partitionBy = None
             query = self.generateCreateTableQuery(
                 df = df,
                 db = db,
                 table = table,
-                partitionBy = partitionByFunction+'('+partitionByTable+')',
+                partitionBy = partitionBy,
                 orderBy = orderBy,
+                primaryKey = primaryKey,
             )
             try:
                 self.ch.execute(query)
             except Exception as e:
                 self.logger.error(f"{defName}: failed execute in clickhouse: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
                 return False
 
@@ -275,21 +299,27 @@
         columnsString = ''
         for column in df.columns.values.tolist():
             if columnsString:
                 columnsString = columnsString +","
             columnsString = columnsString +"`"+ column +"`"
         insertString = 'INSERT INTO %s.%s (%s) VALUES' % (db,table,columnsString)
         self.logger.debug(insertString)
+
+        # convert df type objects to string
+        objectColumns = df.select_dtypes(include=[object]).columns
+        df[objectColumns] = df[objectColumns].astype(str)
+
         try:
             self.ch.insert_dataframe(
                 insertString,
                 df,
                 settings={ "use_numpy": True },
             )
         except Exception as e:
+            self.logger.warning(f"{defName}: failed insert error={str(e)}")
             if e.code == 16: # NO_SUCH_COLUMN_IN_TABLE https://github.com/mymarilyn/clickhouse-driver/blob/master/clickhouse_driver/errors.py#L17
                 self.logger.warning(f"{defName}: schema in clickhouse table does not match df schema: host={self.host}, port={self.port}, db={db}, table={table}'")
                 self.syncTableSchema(df,table,db)
                 # retry
                 if retryCounter >= 1:
                     raise Exception(f"{defName}: failed insert_dataframe in clickhouse: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
                 else:
```

### Comparing `clickhousePandasWrapper-1.0.2/clickhousePandasWrapper.egg-info/PKG-INFO` & `clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhousePandasWrapper
-Version: 1.0.2
+Version: 1.1.0
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

