# Comparing `tmp/trytond_stock_lot_unit-7.2.0.tar.gz` & `tmp/trytond_stock_lot_unit-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot_unit-7.2.0.tar", last modified: Mon Apr 29 15:51:36 2024, max compression
+gzip compressed data, was "trytond_stock_lot_unit-7.2.1.tar", last modified: Wed May  1 10:04:14 2024, max compression
```

## Comparing `trytond_stock_lot_unit-7.2.0.tar` & `trytond_stock_lot_unit-7.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-29 15:28:05.000000 trytond_stock_lot_unit-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:28:04.000000 trytond_stock_lot_unit-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.048577 trytond_stock_lot_unit-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:33.000000 trytond_stock_lot_unit-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2347 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2270 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2672 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2395 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2435 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2024-03-17 11:01:36.000000 trytond_stock_lot_unit-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-22 12:01:28.000000 trytond_stock_lot_unit-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5551 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1924 2024-04-22 12:14:36.000000 trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:33.000000 trytond_stock_lot_unit-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:28:00.000000 trytond_stock_lot_unit-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1737 2024-04-29 15:51:36.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/view/lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-02-04 18:51:26.000000 trytond_stock_lot_unit-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1286 2024-05-01 10:04:11.000000 trytond_stock_lot_unit-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-05-01 10:04:11.000000 trytond_stock_lot_unit-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.492514 trytond_stock_lot_unit-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2307 2024-04-30 17:21:59.000000 trytond_stock_lot_unit-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2410 2024-04-30 17:21:59.000000 trytond_stock_lot_unit-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2310 2024-04-30 17:21:59.000000 trytond_stock_lot_unit-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2270 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2672 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2393 2024-04-30 17:21:59.000000 trytond_stock_lot_unit-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2401 2024-04-30 17:21:59.000000 trytond_stock_lot_unit-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5551 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tests/scenario_stock_lot_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1924 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tests/scenario_stock_lot_unit_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-30 17:21:06.000000 trytond_stock_lot_unit-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1737 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:04:14.000000 trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:14.495848 trytond_stock_lot_unit-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/view/lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_stock_lot_unit-7.2.1/view/template_form.xml
```

### Comparing `trytond_stock_lot_unit-7.2.0/CHANGELOG` & `trytond_stock_lot_unit-7.2.1/CHANGELOG`

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

### Comparing `trytond_stock_lot_unit-7.2.0/COPYRIGHT` & `trytond_stock_lot_unit-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/LICENSE` & `trytond_stock_lot_unit-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/PKG-INFO` & `trytond_stock_lot_unit-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot_unit
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define unit on stock lot
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_lot_unit-7.2.0/__init__.py` & `trytond_stock_lot_unit-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/doc/conf.py` & `trytond_stock_lot_unit-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/bg.po` & `trytond_stock_lot_unit-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/ca.po` & `trytond_stock_lot_unit-7.2.1/locale/ca.po`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,21 @@
 msgid "Unit"
 msgstr "Unitat"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Quantitat unitària"
 
-#, fuzzy
 msgctxt "help:product.product,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "La unitat de mesuera per defecte del lot."
+msgstr "La unitat per defecte del lot."
 
-#, fuzzy
 msgctxt "help:product.template,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "La unitat de mesuera per defecte del lot."
+msgstr "La unitat per defecte del lot."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La major unitat del lot."
 
 msgctxt "help:stock.lot,unit_quantity:"
 msgid "The maximal quantity for the lot."
```

### Comparing `trytond_stock_lot_unit-7.2.0/locale/cs.po` & `trytond_stock_lot_unit-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/de.po` & `trytond_stock_lot_unit-7.2.1/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,lot_uom:"
 msgid "Lot UoM"
-msgstr "Chargeneinheit"
+msgstr "Chargenmaßeinheit"
 
 msgctxt "field:product.template,lot_uom:"
 msgid "Lot UoM"
-msgstr "Chargeneinheit"
+msgstr "Chargenmaßeinheit"
 
 msgctxt "field:stock.lot,product_default_uom_category:"
 msgid "Default Product UoM Category"
 msgstr "Standardmaßeinheitenkategorie"
 
 msgctxt "field:stock.lot,unit:"
 msgid "Unit"
@@ -30,20 +30,18 @@
 msgid "Unit"
 msgstr "Einheit"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Maßeinheit Menge"
 
-#, fuzzy
 msgctxt "help:product.product,lot_uom:"
 msgid "The default unit of measure for lot."
 msgstr "Die Standardmaßeinheit für Chargen."
 
-#, fuzzy
 msgctxt "help:product.template,lot_uom:"
 msgid "The default unit of measure for lot."
 msgstr "Die Standardmaßeinheit für Chargen."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "Die größte Maßeinheit für die Charge."
```

### Comparing `trytond_stock_lot_unit-7.2.0/locale/es.po` & `trytond_stock_lot_unit-7.2.1/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,21 @@
 msgid "Unit"
 msgstr "Unidad"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Cantidad unitaria"
 
-#, fuzzy
 msgctxt "help:product.product,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "La unidad de medida por defecto del lote."
+msgstr "La unidad por defecto del lote."
 
-#, fuzzy
 msgctxt "help:product.template,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "La unidad de medida por defecto del lote."
+msgstr "La unidad por defecto del lote."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La mayor unidad del lote."
 
 msgctxt "help:stock.lot,unit_quantity:"
 msgid "The maximal quantity for the lot."
```

### Comparing `trytond_stock_lot_unit-7.2.0/locale/es_419.po` & `trytond_stock_lot_unit-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/et.po` & `trytond_stock_lot_unit-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/fa.po` & `trytond_stock_lot_unit-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/fi.po` & `trytond_stock_lot_unit-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/fr.po` & `trytond_stock_lot_unit-7.2.1/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,21 @@
 msgid "Unit"
 msgstr "Unité"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Quantité Unitaire"
 
-#, fuzzy
 msgctxt "help:product.product,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "L'unité par défaut pour les lots."
+msgstr "L'unité de mesure par défaut pour le lot."
 
-#, fuzzy
 msgctxt "help:product.template,lot_uom:"
 msgid "The default unit of measure for lot."
-msgstr "L'unité par défaut pour les lots."
+msgstr "L'unité de mesure par défaut pour le lot."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La plus grande unité pour le lot."
 
 msgctxt "help:stock.lot,unit_quantity:"
 msgid "The maximal quantity for the lot."
```

### Comparing `trytond_stock_lot_unit-7.2.0/locale/hu.po` & `trytond_stock_lot_unit-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/id.po` & `trytond_stock_lot_unit-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/it.po` & `trytond_stock_lot_unit-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/lo.po` & `trytond_stock_lot_unit-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/lt.po` & `trytond_stock_lot_unit-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/nl.po` & `trytond_stock_lot_unit-7.2.1/locale/nl.po`

 * *Files 9% similar despite different names*

```diff
@@ -30,20 +30,18 @@
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Eenheid Hoeveelheid"
 
-#, fuzzy
 msgctxt "help:product.product,lot_uom:"
 msgid "The default unit of measure for lot."
 msgstr "De standaard maateenheid voor een batch."
 
-#, fuzzy
 msgctxt "help:product.template,lot_uom:"
 msgid "The default unit of measure for lot."
 msgstr "De standaard maateenheid voor een batch."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "De grootste eenheid voor een batch."
@@ -72,9 +70,9 @@
 "wijzigen."
 
 msgctxt "model:ir.message,text:msg_lot_unit_quantity_greater"
 msgid ""
 "You cannot use more than %(quantity)s%(unit)s of lot \"%(lot)s\" in "
 "\"%(name)s\"."
 msgstr ""
-"U kunt niet meer dan %(quantity)s%(unit)s van batch \"%(lot)s\" in \"% "
-"(name)s\" gebruiken."
+"U kunt niet meer dan %(quantity)s%(unit)s van batch \"%(lot)s\" in "
+"\"%(name)s\" gebruiken."
```

### Comparing `trytond_stock_lot_unit-7.2.0/locale/pl.po` & `trytond_stock_lot_unit-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/pt.po` & `trytond_stock_lot_unit-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/ro.po` & `trytond_stock_lot_unit-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/ru.po` & `trytond_stock_lot_unit-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/sl.po` & `trytond_stock_lot_unit-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/tr.po` & `trytond_stock_lot_unit-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/uk.po` & `trytond_stock_lot_unit-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/locale/zh_CN.po` & `trytond_stock_lot_unit-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/message.xml` & `trytond_stock_lot_unit-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/product.py` & `trytond_stock_lot_unit-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/setup.py` & `trytond_stock_lot_unit-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/stock.py` & `trytond_stock_lot_unit-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/stock.xml` & `trytond_stock_lot_unit-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit.rst` & `trytond_stock_lot_unit-7.2.1/tests/scenario_stock_lot_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit_move_add.rst` & `trytond_stock_lot_unit-7.2.1/tests/scenario_stock_lot_unit_move_add.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/tox.ini` & `trytond_stock_lot_unit-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/PKG-INFO` & `trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot_unit
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define unit on stock lot
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/SOURCES.txt` & `trytond_stock_lot_unit-7.2.1/trytond_stock_lot_unit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

