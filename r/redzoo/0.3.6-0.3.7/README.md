# Comparing `tmp/redzoo-0.3.6.tar.gz` & `tmp/redzoo-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.3.6.tar", last modified: Tue Apr 30 06:41:22 2024, max compression
+gzip compressed data, was "redzoo-0.3.7.tar", last modified: Wed May  1 07:39:35 2024, max compression
```

## Comparing `redzoo-0.3.6.tar` & `redzoo-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.169626 redzoo-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 06:41:11.000000 redzoo-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:41:22.169626 redzoo-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:41:11.000000 redzoo-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 06:41:11.000000 redzoo-0.3.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.165626 redzoo-0.3.6/redzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.165626 redzoo-0.3.6/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.165626 redzoo-0.3.6/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.165626 redzoo-0.3.6/redzoo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-30 06:41:11.000000 redzoo-0.3.6/redzoo/metrics/consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.169626 redzoo-0.3.6/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:41:22.000000 redzoo-0.3.6/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 06:41:22.000000 redzoo-0.3.6/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:41:22.000000 redzoo-0.3.6/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 06:41:22.000000 redzoo-0.3.6/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:41:22.000000 redzoo-0.3.6/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:41:22.169626 redzoo-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:41:22.165626 redzoo-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 06:41:11.000000 redzoo-0.3.6/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 06:41:11.000000 redzoo-0.3.6/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 07:39:30.000000 redzoo-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 07:39:35.899268 redzoo-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 07:39:30.000000 redzoo-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 07:39:30.000000 redzoo-0.3.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/redzoo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-01 07:39:30.000000 redzoo-0.3.7/redzoo/metrics/consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 07:39:35.000000 redzoo-0.3.7/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 07:39:35.000000 redzoo-0.3.7/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:39:35.000000 redzoo-0.3.7/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 07:39:35.000000 redzoo-0.3.7/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 07:39:35.000000 redzoo-0.3.7/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-01 07:39:35.903268 redzoo-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:39:35.899268 redzoo-0.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 07:39:30.000000 redzoo-0.3.7/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-01 07:39:30.000000 redzoo-0.3.7/test/test_simpledb.py
```

### Comparing `redzoo-0.3.6/LICENSE` & `redzoo-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.6/redzoo/database/simple.py` & `redzoo-0.3.7/redzoo/database/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,18 @@
         self.__name = name
         if directory is None:
             self.__directory = site_data_dir("simpledb", appauthor=False)
         else:
             self.__directory = directory
         self.__data = self.__load()
         self.__last_time_stored = datetime.now() - timedelta(days=2)
-        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + formatted_size(os.stat(self.filename).st_size) + ")")
+        try:
+            logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + formatted_size(os.stat(self.filename).st_size) + ")")
+        except Exception as e:
+            logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries)")
 
     @property
     def filename(self):
         if not os.path.exists(self.__directory):
             logging.info("directory " + self.__directory + " does not exits. Creating it")
             os.makedirs(self.__directory)
         return os.path.join(self.__directory, self.__name + ".json.gz")
```

### Comparing `redzoo-0.3.6/redzoo/math/display.py` & `redzoo-0.3.7/redzoo/math/display.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.6/redzoo/metrics/consumption.py` & `redzoo-0.3.7/redzoo/metrics/consumption.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.6/test/test_simpledb.py` & `redzoo-0.3.7/test/test_simpledb.py`

 * *Files identical despite different names*

