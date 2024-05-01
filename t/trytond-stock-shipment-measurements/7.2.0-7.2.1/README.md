# Comparing `tmp/trytond_stock_shipment_measurements-7.2.0.tar.gz` & `tmp/trytond_stock_shipment_measurements-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_shipment_measurements-7.2.0.tar", last modified: Mon Apr 29 15:53:05 2024, max compression
+gzip compressed data, was "trytond_stock_shipment_measurements-7.2.1.tar", last modified: Wed May  1 09:52:36 2024, max compression
```

## Comparing `trytond_stock_shipment_measurements-7.2.0.tar` & `trytond_stock_shipment_measurements-7.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.806229 trytond_stock_shipment_measurements-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1509 2024-04-29 15:29:10.000000 trytond_stock_shipment_measurements-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:29:10.000000 trytond_stock_shipment_measurements-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-04-29 15:53:05.802896 trytond_stock_shipment_measurements-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.796229 trytond_stock_shipment_measurements-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-27 16:30:39.000000 trytond_stock_shipment_measurements-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:36.000000 trytond_stock_shipment_measurements-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.799563 trytond_stock_shipment_measurements-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8441 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8734 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8619 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7832 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8481 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8598 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6837 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8665 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8152 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8065 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-27 16:43:28.000000 trytond_stock_shipment_measurements-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:05.806229 trytond_stock_shipment_measurements-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4438 2024-03-17 11:01:36.000000 trytond_stock_shipment_measurements-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17315 2024-02-04 18:51:27.000000 trytond_stock_shipment_measurements-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5104 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.799563 trytond_stock_shipment_measurements-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8184 2024-02-04 18:51:26.000000 trytond_stock_shipment_measurements-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:36.000000 trytond_stock_shipment_measurements-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-04-29 15:29:06.000000 trytond_stock_shipment_measurements-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.802896 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      173 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:05.000000 trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:05.802896 trytond_stock_shipment_measurements-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/package_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/shipment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/shipment_form_package.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/shipment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/shipment_list_package.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-7.2.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.347441 trytond_stock_shipment_measurements-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-05-01 09:52:33.000000 trytond_stock_shipment_measurements-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:52:33.000000 trytond_stock_shipment_measurements-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-05-01 09:52:36.344107 trytond_stock_shipment_measurements-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.340774 trytond_stock_shipment_measurements-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.344107 trytond_stock_shipment_measurements-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8441 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8745 2024-04-30 17:21:59.000000 trytond_stock_shipment_measurements-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8619 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7832 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8481 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8598 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6837 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8665 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8152 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8065 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:52:36.347441 trytond_stock_shipment_measurements-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4438 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17315 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5104 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.344107 trytond_stock_shipment_measurements-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8184 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-04-30 17:21:06.000000 trytond_stock_shipment_measurements-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.344107 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2713 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1864 2024-05-01 09:52:36.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:52:35.000000 trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:36.344107 trytond_stock_shipment_measurements-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/package_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/shipment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/shipment_form_package.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/shipment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/shipment_list_package.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_stock_shipment_measurements-7.2.1/view/stock_move_form.xml
```

### Comparing `trytond_stock_shipment_measurements-7.2.0/CHANGELOG` & `trytond_stock_shipment_measurements-7.2.1/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_stock_shipment_measurements-7.2.0/COPYRIGHT` & `trytond_stock_shipment_measurements-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/LICENSE` & `trytond_stock_shipment_measurements-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/PKG-INFO` & `trytond_stock_shipment_measurements-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_measurements
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add measurements to shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_shipment_measurements-7.2.0/__init__.py` & `trytond_stock_shipment_measurements-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/doc/conf.py` & `trytond_stock_shipment_measurements-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/bg.po` & `trytond_stock_shipment_measurements-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/ca.po` & `trytond_stock_shipment_measurements-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/cs.po` & `trytond_stock_shipment_measurements-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/de.po` & `trytond_stock_shipment_measurements-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.configuration,measurement_volume_uom:"
 msgid "Measurement Volume UoM"
-msgstr "Volumeneinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.configuration,measurement_weight_uom:"
 msgid "Measurement Weight UoM"
-msgstr "Gewichtseinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.configuration.measurement,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:stock.configuration.measurement,measurement_volume_uom:"
 msgid "Measurement Volume UoM"
-msgstr "Volumeneinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.configuration.measurement,measurement_weight_uom:"
 msgid "Measurement Weight UoM"
-msgstr "Gewichtseinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.move,internal_volume:"
 msgid "Internal Volume"
 msgstr "Internes Volumen"
 
 msgctxt "field:stock.move,internal_weight:"
 msgid "Internal Weight"
@@ -48,39 +48,39 @@
 
 msgctxt "field:stock.package,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:stock.package,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.package,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:stock.package,weight_uom:"
 msgid "Weight UoM"
-msgstr "Gewicht Maßeinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.shipment.in,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:stock.shipment.in,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.shipment.in,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:stock.shipment.in,weight_uom:"
 msgid "Weight UoM"
-msgstr "Gewicht Maßeinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.shipment.in.return,packages_volume:"
 msgid "Packages Volume"
 msgstr "Paketvolumen"
 
 msgctxt "field:stock.shipment.in.return,packages_weight:"
 msgid "Packages Weight"
@@ -88,23 +88,23 @@
 
 msgctxt "field:stock.shipment.in.return,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:stock.shipment.in.return,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.shipment.in.return,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:stock.shipment.in.return,weight_uom:"
 msgid "Weight UoM"
-msgstr "Gewicht Maßeinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.shipment.out,packages_volume:"
 msgid "Packages Volume"
 msgstr "Paketvolumen"
 
 msgctxt "field:stock.shipment.out,packages_weight:"
 msgid "Packages Weight"
@@ -112,39 +112,39 @@
 
 msgctxt "field:stock.shipment.out,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:stock.shipment.out,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.shipment.out,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:stock.shipment.out,weight_uom:"
 msgid "Weight UoM"
-msgstr "Gewicht Maßeinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:stock.shipment.out.return,volume:"
 msgid "Volume"
 msgstr "Volumen"
 
 msgctxt "field:stock.shipment.out.return,volume_uom:"
 msgid "Volume UoM"
-msgstr "Volumen Maßeinheit"
+msgstr "Volumenmaßeinheit"
 
 msgctxt "field:stock.shipment.out.return,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:stock.shipment.out.return,weight_uom:"
 msgid "Weight UoM"
-msgstr "Gewicht Maßeinheit"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "help:stock.configuration,measurement_volume_uom:"
 msgid "The default Unit of Measure for volume."
 msgstr "Die Standardmaßeinheit für das Volumen."
 
 msgctxt "help:stock.configuration,measurement_weight_uom:"
 msgid "The default Unit of Measure for weight."
```

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/es.po` & `trytond_stock_shipment_measurements-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/es_419.po` & `trytond_stock_shipment_measurements-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/et.po` & `trytond_stock_shipment_measurements-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/fa.po` & `trytond_stock_shipment_measurements-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/fi.po` & `trytond_stock_shipment_measurements-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/fr.po` & `trytond_stock_shipment_measurements-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/hu.po` & `trytond_stock_shipment_measurements-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/id.po` & `trytond_stock_shipment_measurements-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/it.po` & `trytond_stock_shipment_measurements-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/lo.po` & `trytond_stock_shipment_measurements-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/lt.po` & `trytond_stock_shipment_measurements-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/nl.po` & `trytond_stock_shipment_measurements-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/pl.po` & `trytond_stock_shipment_measurements-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/pt.po` & `trytond_stock_shipment_measurements-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/ro.po` & `trytond_stock_shipment_measurements-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/ru.po` & `trytond_stock_shipment_measurements-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/sl.po` & `trytond_stock_shipment_measurements-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/tr.po` & `trytond_stock_shipment_measurements-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/uk.po` & `trytond_stock_shipment_measurements-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/locale/zh_CN.po` & `trytond_stock_shipment_measurements-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/setup.py` & `trytond_stock_shipment_measurements-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/stock.py` & `trytond_stock_shipment_measurements-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/stock.xml` & `trytond_stock_shipment_measurements-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/tests/test_module.py` & `trytond_stock_shipment_measurements-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/tox.ini` & `trytond_stock_shipment_measurements-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO` & `trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_measurements
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add measurements to shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_shipment_measurements-7.2.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt` & `trytond_stock_shipment_measurements-7.2.1/trytond_stock_shipment_measurements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-7.2.0/view/configuration_form.xml` & `trytond_stock_shipment_measurements-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

