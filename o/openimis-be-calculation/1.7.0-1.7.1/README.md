# Comparing `tmp/openimis_be_calculation-1.7.0.tar.gz` & `tmp/openimis_be_calculation-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis_be_calculation-1.7.0.tar", last modified: Tue Apr 30 09:06:12 2024, max compression
+gzip compressed data, was "openimis_be_calculation-1.7.1.tar", last modified: Wed May  1 05:26:01 2024, max compression
```

## Comparing `openimis_be_calculation-1.7.0.tar` & `openimis_be_calculation-1.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.095028 openimis_be_calculation-1.7.0/calculation/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.095028 openimis_be_calculation-1.7.0/calculation/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0002_auto_20210118_1426.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0003_add_calculation_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0004_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/calculation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-30 09:06:11.000000 openimis_be_calculation-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:01.613072 openimis_be_calculation-1.7.1/calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/calculation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/migrations/0002_auto_20210118_1426.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/migrations/0003_add_calculation_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/migrations/0004_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/calculation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/tests/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:25:52.000000 openimis_be_calculation-1.7.1/calculation/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:26:01.617072 openimis_be_calculation-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-01 05:26:01.000000 openimis_be_calculation-1.7.1/setup.py
```

### Comparing `openimis_be_calculation-1.7.0/LICENSE.md` & `openimis_be_calculation-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/PKG-INFO` & `openimis_be_calculation-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.7.0
+Version: 1.7.1
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis_be_calculation-1.7.0/README.md` & `openimis_be_calculation-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/apps.py` & `openimis_be_calculation-1.7.1/calculation/apps.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/calculation_rule.py` & `openimis_be_calculation-1.7.1/calculation/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/config.py` & `openimis_be_calculation-1.7.1/calculation/config.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/migrations/0001_initial.py` & `openimis_be_calculation-1.7.1/calculation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/migrations/0002_auto_20210118_1426.py` & `openimis_be_calculation-1.7.1/calculation/migrations/0002_auto_20210118_1426.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/migrations/0004_auto_20230126_0903.py` & `openimis_be_calculation-1.7.1/calculation/migrations/0004_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/schema.py` & `openimis_be_calculation-1.7.1/calculation/schema.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/calculation/services.py` & `openimis_be_calculation-1.7.1/calculation/services.py`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/PKG-INFO` & `openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.7.0
+Version: 1.7.1
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/SOURCES.txt` & `openimis_be_calculation-1.7.1/openimis_be_calculation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis_be_calculation-1.7.0/setup.py` & `openimis_be_calculation-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calculation',
-    version='v1.7.0',
+    version='v1.7.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Calculation reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

