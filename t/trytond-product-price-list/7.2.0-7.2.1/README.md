# Comparing `tmp/trytond_product_price_list-7.2.0.tar.gz` & `tmp/trytond_product_price_list-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list-7.2.0.tar", last modified: Mon Apr 29 15:43:34 2024, max compression
+gzip compressed data, was "trytond_product_price_list-7.2.1.tar", last modified: Wed May  1 11:49:09 2024, max compression
```

## Comparing `trytond_product_price_list-7.2.0.tar` & `trytond_product_price_list-7.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3015 2024-04-29 15:22:09.000000 trytond_product_price_list-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:22:09.000000 trytond_product_price_list-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_product_price_list-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:16.000000 trytond_product_price_list-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3465 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3165 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4190 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4122 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3456 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3360 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4225 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3154 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3177 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4155 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3357 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3921 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4169 2024-04-29 13:17:17.000000 trytond_product_price_list-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3399 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3891 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3167 2024-04-27 16:43:25.000000 trytond_product_price_list-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7283 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/price_list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3854 2024-04-27 16:30:39.000000 trytond_product_price_list-7.2.0/price_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4291 2024-03-17 11:01:36.000000 trytond_product_price_list-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.441173 trytond_product_price_list-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8440 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:16.000000 trytond_product_price_list-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-29 15:22:05.000000 trytond_product_price_list-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1713 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:34.000000 trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:34.444506 trytond_product_price_list-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-02-04 18:51:26.000000 trytond_product_price_list-7.2.0/view/price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      615 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_product_price_list-7.2.0/view/price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3116 2024-05-01 11:49:06.000000 trytond_product_price_list-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 11:49:05.000000 trytond_product_price_list-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.326287 trytond_product_price_list-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3465 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3165 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4190 2024-04-30 17:21:59.000000 trytond_product_price_list-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4122 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3456 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3360 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4225 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3154 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3218 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3177 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4155 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3357 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3921 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4169 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3399 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3891 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3167 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7283 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/price_list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3854 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/price_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4291 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8440 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:06.000000 trytond_product_price_list-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2561 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1713 2024-05-01 11:49:09.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:49:08.000000 trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:49:09.329620 trytond_product_price_list-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/view/price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      615 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/view/price_list_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:20:59.000000 trytond_product_price_list-7.2.1/view/price_list_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/view/price_list_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:21:00.000000 trytond_product_price_list-7.2.1/view/price_list_tree.xml
```

### Comparing `trytond_product_price_list-7.2.0/CHANGELOG` & `trytond_product_price_list-7.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_product_price_list-7.2.0/COPYRIGHT` & `trytond_product_price_list-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/LICENSE` & `trytond_product_price_list-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/PKG-INFO` & `trytond_product_price_list-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with price list
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_price_list-7.2.0/doc/conf.py` & `trytond_product_price_list-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/bg.po` & `trytond_product_price_list-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/ca.po` & `trytond_product_price_list-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/cs.po` & `trytond_product_price_list-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/de.po` & `trytond_product_price_list-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 "exception \"%(exception)s\"."
 msgstr ""
 "Ungültige Formel \"%(formula)s\" in Preislistenposition \"%(line)s\" mit "
 "Fehlermeldung \"%(exception)s\"."
 
 msgctxt "model:ir.rule.group,name:rule_group_price_list_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_price_list"
 msgid "Price Lists"
 msgstr "Preislisten"
 
 msgctxt "model:product.price_list,name:"
 msgid "Price List"
```

### Comparing `trytond_product_price_list-7.2.0/locale/es.po` & `trytond_product_price_list-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/es_419.po` & `trytond_product_price_list-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/et.po` & `trytond_product_price_list-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/fa.po` & `trytond_product_price_list-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/fi.po` & `trytond_product_price_list-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/fr.po` & `trytond_product_price_list-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/hu.po` & `trytond_product_price_list-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/id.po` & `trytond_product_price_list-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/it.po` & `trytond_product_price_list-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/lo.po` & `trytond_product_price_list-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/lt.po` & `trytond_product_price_list-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/nl.po` & `trytond_product_price_list-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/pl.po` & `trytond_product_price_list-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/pt.po` & `trytond_product_price_list-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/ro.po` & `trytond_product_price_list-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/ru.po` & `trytond_product_price_list-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/sl.po` & `trytond_product_price_list-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/tr.po` & `trytond_product_price_list-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/uk.po` & `trytond_product_price_list-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/locale/zh_CN.po` & `trytond_product_price_list-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/price_list.py` & `trytond_product_price_list-7.2.1/price_list.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/price_list.xml` & `trytond_product_price_list-7.2.1/price_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/setup.py` & `trytond_product_price_list-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/tests/test_module.py` & `trytond_product_price_list-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/tox.ini` & `trytond_product_price_list-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/PKG-INFO` & `trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with price list
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_price_list-7.2.0/trytond_product_price_list.egg-info/SOURCES.txt` & `trytond_product_price_list-7.2.1/trytond_product_price_list.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/view/price_list_form.xml` & `trytond_product_price_list-7.2.1/view/price_list_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-7.2.0/view/price_list_line_form.xml` & `trytond_product_price_list-7.2.1/view/price_list_line_form.xml`

 * *Files identical despite different names*

