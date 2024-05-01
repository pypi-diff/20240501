# Comparing `tmp/sqlgrep-0.0.8.tar.gz` & `tmp/sqlgrep-0.0.9.tar.gz`

## Comparing `sqlgrep-0.0.8.tar` & `sqlgrep-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     3456 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/sqlgrep/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/LICENSE
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/README.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 sqlgrep-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     3462 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/sqlgrep/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/README.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 sqlgrep-0.0.9/PKG-INFO
```

### Comparing `sqlgrep-0.0.8/sqlgrep/__init__.py` & `sqlgrep-0.0.9/sqlgrep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from sqlalchemy import create_engine, inspect, or_, cast, String, Integer, Float
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.orm import sessionmaker
 import sqlalchemy as sa
 
 
-__version__='0.0.8'
+__version__='0.0.9'
 
 def get_args():
 
 
     parser = argparse.ArgumentParser(description='database search (SQL grep), version: {}'.format(__version__))
   
     parser.add_argument('db', metavar='DB URL', default=None, help='example: mysql://user:password@host/db_name')
@@ -69,15 +69,15 @@
         if count:
             print(f"{column}: {count} rows matched")
         return
     
     try:
         result = query.all()
     except (Exception, TypeError) as e:
-        print(f"Table: {table}, column: {column} EXCEPTION: {e}")
+        print(f"Table: {table}, column: {column} EXCEPTION: {type(e)}")
         return
 
     # Print the results
     for row in result:
         value = getattr(row, column.key)
         if args.all:
             rprint(row.__dict__)
```

### Comparing `sqlgrep-0.0.8/.gitignore` & `sqlgrep-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlgrep-0.0.8/LICENSE` & `sqlgrep-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlgrep-0.0.8/README.md` & `sqlgrep-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlgrep-0.0.8/pyproject.toml` & `sqlgrep-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlgrep-0.0.8/PKG-INFO` & `sqlgrep-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlgrep
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple OpenSSL for humans: fetch/validate/show/save SSL certificates and warn about soon expiration
 Project-URL: Homepage, https://github.com/yaroslaff/sqlgrep
 Project-URL: Issues, https://github.com/yaroslaff/sqlgrep/issues
 Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

