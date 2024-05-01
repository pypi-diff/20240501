# Comparing `tmp/trytond_product_measurements-7.2.0.tar.gz` & `tmp/trytond_product_measurements-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_measurements-7.2.0.tar", last modified: Mon Apr 29 15:43:27 2024, max compression
+gzip compressed data, was "trytond_product_measurements-7.2.1.tar", last modified: Wed May  1 11:49:56 2024, max compression
```

## Comparing `trytond_product_measurements-7.2.0.tar` & `trytond_product_measurements-7.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2183 2024-04-29 15:22:04.000000 trytond_product_measurements-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:22:04.000000 trytond_product_measurements-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.584685 trytond_product_measurements-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_product_measurements-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:16.000000 trytond_product_measurements-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4101 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4543 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4470 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4549 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4125 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3989 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3714 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3831 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4326 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4521 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4653 2024-04-29 13:17:17.000000 trytond_product_measurements-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3959 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3861 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3969 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3603 2024-04-27 16:43:25.000000 trytond_product_measurements-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4542 2024-02-04 18:51:26.000000 trytond_product_measurements-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_product_measurements-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2024-03-17 11:01:36.000000 trytond_product_measurements-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_product_measurements-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:16.000000 trytond_product_measurements-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:22:00.000000 trytond_product_measurements-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:27.000000 trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:27.588019 trytond_product_measurements-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1080 2024-02-04 18:51:26.000000 trytond_product_measurements-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.908376 trytond_product_measurements-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2024-05-01 11:49:53.000000 trytond_product_measurements-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-05-01 11:49:53.000000 trytond_product_measurements-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-05-01 11:49:56.908376 trytond_product_measurements-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.901710 trytond_product_measurements-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.905043 trytond_product_measurements-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4101 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4543 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4468 2024-04-30 17:21:59.000000 trytond_product_measurements-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4549 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4125 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3989 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3714 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3831 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4326 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4521 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4653 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3959 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3861 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3969 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3603 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4542 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:49:56.908376 trytond_product_measurements-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4334 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.905043 trytond_product_measurements-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_product_measurements-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-30 17:21:06.000000 trytond_product_measurements-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.905043 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:49:56.000000 trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:56.905043 trytond_product_measurements-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1080 2024-04-30 17:20:59.000000 trytond_product_measurements-7.2.1/view/template_form.xml
```

### Comparing `trytond_product_measurements-7.2.0/CHANGELOG` & `trytond_product_measurements-7.2.1/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.1 - 2024-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_product_measurements-7.2.0/COPYRIGHT` & `trytond_product_measurements-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/LICENSE` & `trytond_product_measurements-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/PKG-INFO` & `trytond_product_measurements-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_measurements
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add measurements to product
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_measurements-7.2.0/doc/conf.py` & `trytond_product_measurements-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/bg.po` & `trytond_product_measurements-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/ca.po` & `trytond_product_measurements-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/cs.po` & `trytond_product_measurements-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/de.po` & `trytond_product_measurements-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 msgctxt "field:product.product,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:product.product,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:product.product,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:product.product,weight_uom:"
 msgid "Weight UoM"
-msgstr "Maßeinheit Gewicht"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:product.product,width:"
 msgid "Width"
 msgstr "Breite"
 
 msgctxt "field:product.product,width_uom:"
 msgid "Width UoM"
@@ -60,23 +60,23 @@
 
 msgctxt "field:product.template,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:product.template,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:product.template,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:product.template,weight_uom:"
 msgid "Weight UoM"
-msgstr "Maßeinheit Gewicht"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:product.template,width:"
 msgid "Width"
 msgstr "Breite"
 
 msgctxt "field:product.template,width_uom:"
 msgid "Width UoM"
```

### Comparing `trytond_product_measurements-7.2.0/locale/es.po` & `trytond_product_measurements-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/es_419.po` & `trytond_product_measurements-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/et.po` & `trytond_product_measurements-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/fa.po` & `trytond_product_measurements-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/fi.po` & `trytond_product_measurements-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/fr.po` & `trytond_product_measurements-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/hu.po` & `trytond_product_measurements-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/id.po` & `trytond_product_measurements-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/it.po` & `trytond_product_measurements-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/lo.po` & `trytond_product_measurements-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/lt.po` & `trytond_product_measurements-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/nl.po` & `trytond_product_measurements-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/pl.po` & `trytond_product_measurements-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/pt.po` & `trytond_product_measurements-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/ro.po` & `trytond_product_measurements-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/ru.po` & `trytond_product_measurements-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/sl.po` & `trytond_product_measurements-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/tr.po` & `trytond_product_measurements-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/uk.po` & `trytond_product_measurements-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/locale/zh_CN.po` & `trytond_product_measurements-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/product.py` & `trytond_product_measurements-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/setup.py` & `trytond_product_measurements-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/tox.ini` & `trytond_product_measurements-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/PKG-INFO` & `trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_measurements
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add measurements to product
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_measurements-7.2.0/trytond_product_measurements.egg-info/SOURCES.txt` & `trytond_product_measurements-7.2.1/trytond_product_measurements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product_measurements-7.2.0/view/template_form.xml` & `trytond_product_measurements-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

