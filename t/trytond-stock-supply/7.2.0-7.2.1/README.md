# Comparing `tmp/trytond_stock_supply-7.2.0.tar.gz` & `tmp/trytond_stock_supply-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply-7.2.0.tar", last modified: Mon Apr 29 15:53:17 2024, max compression
+gzip compressed data, was "trytond_stock_supply-7.2.1.tar", last modified: Wed May  1 09:52:09 2024, max compression
```

## Comparing `trytond_stock_supply-7.2.0.tar` & `trytond_stock_supply-7.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3971 2024-04-29 15:29:20.000000 trytond_stock_supply-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-29 15:29:20.000000 trytond_stock_supply-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-01-27 09:58:52.000000 trytond_stock_supply-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.785916 trytond_stock_supply-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-01-27 09:58:52.000000 trytond_stock_supply-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:37.000000 trytond_stock_supply-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5635 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5981 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-29 13:17:17.000000 trytond_stock_supply-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4704 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6098 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6102 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5766 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4980 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5820 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5039 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5924 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4611 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5684 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5505 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8358 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/order_point.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3947 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/order_point.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14550 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2024-03-17 11:01:36.000000 trytond_stock_supply-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7697 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5751 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4298 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_lead_time.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4435 2024-04-22 12:14:36.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7452 2024-04-22 12:14:36.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_supply_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:37.000000 trytond_stock_supply-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:29:16.000000 trytond_stock_supply-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2365 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/order_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      486 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/view/order_point_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/supply_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.204817 trytond_stock_supply-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-05-01 09:52:06.000000 trytond_stock_supply-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-05-01 09:52:05.000000 trytond_stock_supply-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-05-01 09:52:09.204817 trytond_stock_supply-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.201484 trytond_stock_supply-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.201484 trytond_stock_supply-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5635 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5981 2024-04-30 17:21:59.000000 trytond_stock_supply-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4704 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4985 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6098 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6102 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5766 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4980 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4839 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5820 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5039 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5924 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4611 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5684 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5505 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8358 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/order_point.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3947 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/order_point.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14550 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:52:09.204817 trytond_stock_supply-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7697 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1279 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.201484 trytond_stock_supply-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5751 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4298 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply_lead_time.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4435 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7452 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/scenario_stock_supply_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6265 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:06.000000 trytond_stock_supply-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.204817 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2365 2024-05-01 09:52:09.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:52:08.000000 trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:52:09.204817 trytond_stock_supply-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1076 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/view/order_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      486 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/view/order_point_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond_stock_supply-7.2.1/view/supply_start_form.xml
```

### Comparing `trytond_stock_supply-7.2.0/CHANGELOG` & `trytond_stock_supply-7.2.1/CHANGELOG`

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

### Comparing `trytond_stock_supply-7.2.0/COPYRIGHT` & `trytond_stock_supply-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/LICENSE` & `trytond_stock_supply-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/PKG-INFO` & `trytond_stock_supply-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
```

### Comparing `trytond_stock_supply-7.2.0/README.rst` & `trytond_stock_supply-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/__init__.py` & `trytond_stock_supply-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/doc/conf.py` & `trytond_stock_supply-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/doc/index.rst` & `trytond_stock_supply-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/bg.po` & `trytond_stock_supply-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/ca.po` & `trytond_stock_supply-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/cs.po` & `trytond_stock_supply-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/de.po` & `trytond_stock_supply-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 msgid "Only one order point is allowed for each product-location pair."
 msgstr ""
 "Es ist nur ein Bestellpunkt für jede Paarung aus Artikel und Lagerort "
 "erlaubt."
 
 msgctxt "model:ir.rule.group,name:rule_group_order_point_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_order_point_form"
 msgid "Order Points"
 msgstr "Bestellpunkte"
 
 msgctxt "model:ir.ui.menu,name:menu_stock_supply"
 msgid "Supply Stock"
```

### Comparing `trytond_stock_supply-7.2.0/locale/es.po` & `trytond_stock_supply-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/es_419.po` & `trytond_stock_supply-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/et.po` & `trytond_stock_supply-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/fa.po` & `trytond_stock_supply-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/fi.po` & `trytond_stock_supply-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/fr.po` & `trytond_stock_supply-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/hu.po` & `trytond_stock_supply-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/id.po` & `trytond_stock_supply-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/it.po` & `trytond_stock_supply-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/lo.po` & `trytond_stock_supply-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/lt.po` & `trytond_stock_supply-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/nl.po` & `trytond_stock_supply-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/pl.po` & `trytond_stock_supply-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/pt.po` & `trytond_stock_supply-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/ro.po` & `trytond_stock_supply-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/ru.po` & `trytond_stock_supply-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/sl.po` & `trytond_stock_supply-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/tr.po` & `trytond_stock_supply-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/uk.po` & `trytond_stock_supply-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/locale/zh_CN.po` & `trytond_stock_supply-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/location.py` & `trytond_stock_supply-7.2.1/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/message.xml` & `trytond_stock_supply-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/order_point.py` & `trytond_stock_supply-7.2.1/order_point.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/order_point.xml` & `trytond_stock_supply-7.2.1/order_point.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/product.py` & `trytond_stock_supply-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/product.xml` & `trytond_stock_supply-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/purchase_request.py` & `trytond_stock_supply-7.2.1/purchase_request.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/purchase_request.xml` & `trytond_stock_supply-7.2.1/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/setup.py` & `trytond_stock_supply-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/shipment.py` & `trytond_stock_supply-7.2.1/shipment.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/stock.py` & `trytond_stock_supply-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/stock.xml` & `trytond_stock_supply-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply.rst` & `trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_lead_time.rst` & `trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply_lead_time.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_overflow.rst` & `trytond_stock_supply-7.2.1/tests/scenario_stock_internal_supply_overflow.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tests/scenario_stock_supply_purchase_request.rst` & `trytond_stock_supply-7.2.1/tests/scenario_stock_supply_purchase_request.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tests/test_module.py` & `trytond_stock_supply-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/tox.ini` & `trytond_stock_supply-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/PKG-INFO` & `trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
```

### Comparing `trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/SOURCES.txt` & `trytond_stock_supply-7.2.1/trytond_stock_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.2.0/view/order_point_form.xml` & `trytond_stock_supply-7.2.1/view/order_point_form.xml`

 * *Files identical despite different names*

