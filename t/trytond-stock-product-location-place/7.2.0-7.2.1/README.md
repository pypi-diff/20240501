# Comparing `tmp/trytond_stock_product_location_place-7.2.0.tar.gz` & `tmp/trytond_stock_product_location_place-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_product_location_place-7.2.0.tar", last modified: Mon Apr 29 15:54:43 2024, max compression
+gzip compressed data, was "trytond_stock_product_location_place-7.2.1.tar", last modified: Wed May  1 09:55:19 2024, max compression
```

## Comparing `trytond_stock_product_location_place-7.2.0.tar` & `trytond_stock_product_location_place-7.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)       71 2024-04-29 15:30:26.000000 trytond_stock_product_location_place-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:26.000000 trytond_stock_product_location_place-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.767000 trytond_stock_product_location_place-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3091 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      932 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-29 13:17:17.000000 trytond_stock_product_location_place-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3284 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      486 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4769 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7307 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2153 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2368 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1542 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place_copy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place_modification.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      112 2024-04-29 15:30:22.000000 trytond_stock_product_location_place-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:43.000000 trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:43.770334 trytond_stock_product_location_place-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/view/stock_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/view/stock_product_location_place_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-27 16:30:39.000000 trytond_stock_product_location_place-7.2.0/view/stock_product_location_place_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.173182 trytond_stock_product_location_place-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-05-01 09:55:16.000000 trytond_stock_product_location_place-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:55:15.000000 trytond_stock_product_location_place-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-05-01 09:55:19.173182 trytond_stock_product_location_place-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.169849 trytond_stock_product_location_place-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3091 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      932 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.169849 trytond_stock_product_location_place-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1308 2024-04-30 17:21:59.000000 trytond_stock_product_location_place-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1308 2024-04-30 17:21:59.000000 trytond_stock_product_location_place-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1322 2024-04-30 17:21:59.000000 trytond_stock_product_location_place-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1352 2024-04-30 17:21:59.000000 trytond_stock_product_location_place-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1322 2024-04-30 17:21:59.000000 trytond_stock_product_location_place-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3284 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      486 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:55:19.173182 trytond_stock_product_location_place-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4769 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7307 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2153 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.169849 trytond_stock_product_location_place-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2368 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1542 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place_copy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place_modification.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      112 2024-04-30 17:21:06.000000 trytond_stock_product_location_place-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.173182 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-05-01 09:55:19.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:55:18.000000 trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:55:19.173182 trytond_stock_product_location_place-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/view/stock_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/view/stock_product_location_place_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond_stock_product_location_place-7.2.1/view/stock_product_location_place_list.xml
```

### Comparing `trytond_stock_product_location_place-7.2.0/COPYRIGHT` & `trytond_stock_product_location_place-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/LICENSE` & `trytond_stock_product_location_place-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/PKG-INFO` & `trytond_stock_product_location_place-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_product_location_place
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define a product place for each location
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_product_location_place-7.2.0/__init__.py` & `trytond_stock_product_location_place-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/doc/conf.py` & `trytond_stock_product_location_place-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/doc/design.rst` & `trytond_stock_product_location_place-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/bg.po` & `trytond_stock_product_location_place-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/ca.po` & `trytond_stock_product_location_place-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/cs.po` & `trytond_stock_product_location_place-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/de.po` & `trytond_stock_product_location_place-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/es.po` & `trytond_stock_product_location_place-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/es_419.po` & `trytond_stock_product_location_place-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/et.po` & `trytond_stock_product_location_place-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/fa.po` & `trytond_stock_product_location_place-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/fi.po` & `trytond_stock_product_location_place-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/fr.po` & `trytond_stock_product_location_place-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/hu.po` & `trytond_stock_product_location_place-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/id.po` & `trytond_stock_product_location_place-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/it.po` & `trytond_stock_product_location_place-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/lo.po` & `trytond_stock_product_location_place-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/lt.po` & `trytond_stock_product_location_place-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/nl.po` & `trytond_stock_product_location_place-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/pl.po` & `trytond_stock_product_location_place-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/pt.po` & `trytond_stock_product_location_place-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/ro.po` & `trytond_stock_product_location_place-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/locale/ru.po` & `trytond_stock_product_location_place-7.2.1/locale/de.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,location_places:"
 msgid "Places per Location"
-msgstr ""
+msgstr "Lagerplätze je Lagerort"
 
 msgctxt "field:product.template,location_places:"
 msgid "Places per Location"
-msgstr ""
+msgstr "Lagerplätze je Lagerort"
 
 msgctxt "field:stock.move,from_place:"
 msgid "From Place"
-msgstr ""
+msgstr "Von Lagerplatz"
 
 msgctxt "field:stock.move,to_place:"
 msgid "To Place"
-msgstr ""
+msgstr "Zu Lagerplatz"
 
 msgctxt "field:stock.product.location.place,location:"
 msgid "Storage Location"
-msgstr ""
+msgstr "Lagerort"
 
 msgctxt "field:stock.product.location.place,place:"
 msgid "Place"
-msgstr ""
+msgstr "Lagerplatz"
 
 msgctxt "field:stock.product.location.place,product:"
 msgid "Variant"
-msgstr ""
+msgstr "Variante"
 
 msgctxt "field:stock.product.location.place,template:"
 msgid "Product"
-msgstr ""
+msgstr "Artikel"
 
 msgctxt "help:stock.product.location.place,place:"
 msgid "The place where the product is always stored in the location."
-msgstr ""
+msgstr "Der Lagerplatz, an dem der Artikel immer gelagert wird."
 
 msgctxt "model:ir.message,text:msg_stock_product_location_unique"
 msgid "Only one product place can be defined per location."
-msgstr ""
+msgstr "Pro Lagerort kann nur ein Artikellagerplatz definiert werden."
 
 msgctxt "model:stock.product.location.place,name:"
 msgid "Product Location Place"
-msgstr ""
+msgstr "Artikel Lagerplatz"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_product_location_place-7.2.0/product.py` & `trytond_stock_product_location_place-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/setup.py` & `trytond_stock_product_location_place-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/stock.py` & `trytond_stock_product_location_place-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/stock.xml` & `trytond_stock_product_location_place-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place.rst` & `trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place_copy.rst` & `trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place_copy.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/tests/scenario_stock_product_location_place_modification.rst` & `trytond_stock_product_location_place-7.2.1/tests/scenario_stock_product_location_place_modification.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/tox.ini` & `trytond_stock_product_location_place-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/PKG-INFO` & `trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_product_location_place
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define a product place for each location
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_product_location_place-7.2.0/trytond_stock_product_location_place.egg-info/SOURCES.txt` & `trytond_stock_product_location_place-7.2.1/trytond_stock_product_location_place.egg-info/SOURCES.txt`

 * *Files identical despite different names*

