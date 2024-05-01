# Comparing `tmp/trytond_sale_supply_drop_shipment-7.2.0.tar.gz` & `tmp/trytond_sale_supply_drop_shipment-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply_drop_shipment-7.2.0.tar", last modified: Mon Apr 29 15:50:20 2024, max compression
+gzip compressed data, was "trytond_sale_supply_drop_shipment-7.2.1.tar", last modified: Wed May  1 11:17:05 2024, max compression
```

## Comparing `trytond_sale_supply_drop_shipment-7.2.0.tar` & `trytond_sale_supply_drop_shipment-7.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2633 2024-04-29 15:27:08.000000 trytond_sale_supply_drop_shipment-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:27:08.000000 trytond_sale_supply_drop_shipment-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1282 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/icons/tryton-shipment-drop.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7058 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7751 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7801 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7721 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6547 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6500 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7872 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7880 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6790 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6470 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7164 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6980 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6710 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7745 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6912 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7279 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6290 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7096 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7083 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6273 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6653 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1156 2024-04-13 17:12:23.000000 trytond_sale_supply_drop_shipment-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8653 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4729 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4609 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24025 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13541 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10842 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4426 2024-04-22 12:14:36.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-04-22 12:14:36.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4188 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_split.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_supply_drop_shipment-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-29 15:27:04.000000 trytond_sale_supply_drop_shipment-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2892 2024-04-29 15:50:20.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_request_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_split_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/stock_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.842726 trytond_sale_supply_drop_shipment-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2734 2024-05-01 11:17:02.000000 trytond_sale_supply_drop_shipment-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:17:02.000000 trytond_sale_supply_drop_shipment-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-05-01 11:17:05.842726 trytond_sale_supply_drop_shipment-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1282 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.836056 trytond_sale_supply_drop_shipment-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.836056 trytond_sale_supply_drop_shipment-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/icons/tryton-shipment-drop.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.839391 trytond_sale_supply_drop_shipment-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7292 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8093 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6861 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8172 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8063 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6767 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6732 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8106 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6861 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8253 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7024 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6708 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7398 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7214 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6944 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8083 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7146 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7513 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6528 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7330 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7317 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6861 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6511 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6887 2024-04-30 17:21:59.000000 trytond_sale_supply_drop_shipment-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1156 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8653 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4729 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:17:05.842726 trytond_sale_supply_drop_shipment-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4609 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24025 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13541 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.839391 trytond_sale_supply_drop_shipment-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10842 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4426 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4188 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_split.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:21:06.000000 trytond_sale_supply_drop_shipment-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.842726 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2892 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:17:05.000000 trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:05.842726 trytond_sale_supply_drop_shipment-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/purchase_request_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/shipment_drop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/shipment_drop_split_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/shipment_drop_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/stock_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond_sale_supply_drop_shipment-7.2.1/view/stock_move_form.xml
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/CHANGELOG` & `trytond_sale_supply_drop_shipment-7.2.1/CHANGELOG`

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
 * Support splitting drop shipment
 * Split customer moves when splitting supplier moves
 * Rename 'done' button to 'do'
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/COPYRIGHT` & `trytond_sale_supply_drop_shipment-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/LICENSE` & `trytond_sale_supply_drop_shipment-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/PKG-INFO` & `trytond_sale_supply_drop_shipment-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_drop_shipment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale supply drop shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/README.rst` & `trytond_sale_supply_drop_shipment-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/__init__.py` & `trytond_sale_supply_drop_shipment-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/doc/conf.py` & `trytond_sale_supply_drop_shipment-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/doc/index.rst` & `trytond_sale_supply_drop_shipment-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/icons/LICENSE` & `trytond_sale_supply_drop_shipment-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/icons/tryton-shipment-drop.svg` & `trytond_sale_supply_drop_shipment-7.2.1/icons/tryton-shipment-drop.svg`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/bg.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -220,25 +224,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/ca.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/ca.po`

 * *Files 5% similar despite different names*

```diff
@@ -177,20 +177,26 @@
 
 msgctxt ""
 "model:ir.message,text:msg_delivery_address_required_quotation_purchase"
 msgid ""
 "To get a quotation for purchase \"%(purchase)s\" you must provide a delivery"
 " address."
 msgstr ""
-"Per obtenir un pressupost de la compra \"%(compra)s\" heu de proporcionar "
+"Per obtenir un pressupost de la compra \"%(purchase)s\" heu de proporcionar "
 "una direcció d'entrega."
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
-msgstr "Per eliminar l'enviament directe \"%(shipmetn)s\" heu de cancel·lar-lo."
+msgstr "Per eliminar l'enviament directe \"%(shipment)s\" heu de cancel·lar-lo."
+
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+"Heu d'utilitzar l'assistent de divisió per dividir els moviments de "
+"l'enviament directe."
 
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "No podeu restablir a esborrany el moviment \"%(move)s\" perquè ha estat "
@@ -205,25 +211,29 @@
 msgstr "Esteu segurs que voleu enviar l'albarà?"
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Finalitza"
+msgid "Complete"
+msgstr "Completa"
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Esborrany"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Envia"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr "Divideix"
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "En espera"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr "Usuari a les empreses"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/cs.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -205,25 +209,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/de.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,20 @@
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 "Damit die Direktlieferung \"%(shipment)s\" gelöscht werden kann, muss sie "
 "zuerst annulliert werden."
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+"Um eine Lagerbewegung einer Direktlieferung aufteilen zu können, muss der "
+"Aufteilungsassistent verwendet werden."
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "Die Warenbewegung \"%(move)s\" kann nicht in den Entwurfsstatus "
 "zurückgesetzt werden, weil sie automatisch aus einem Verkauf oder Einkauf "
@@ -208,32 +214,36 @@
 msgstr "Lieferung wirklich abschließen?"
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Annullieren"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Erledigt"
+msgid "Complete"
+msgstr "Fertigstellen"
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Versenden"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr "Aufteilen"
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Warten"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_shipment_drop"
 msgid "Drop Shipment"
 msgstr "Direktlieferung"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_shipment_drop"
 msgid "Drop Shipment"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/es.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -184,14 +184,20 @@
 "Para obtener un presupuesto para la compra \"%(purchase)s\" debe "
 "proporcionar una dirección de entrega."
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr "Para eliminar el envío directo \"%(shipment)s\" debe cancelarlo."
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+"Debéis utilizar el asistente de dividir para dividir los movimientos de un "
+"envío directo."
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "No puede restaurar a borrador el movimiento \"%(move)s\" porque fue generado"
 " por una venta o una compra."
@@ -205,25 +211,29 @@
 msgstr "¿Estás seguro que quieres enviar el albarán?"
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Finalizar"
+msgid "Complete"
+msgstr "Completar"
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Borrador"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Enviar"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr "Dividir"
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "En espera"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr "Usuario en las empresas"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/es_419.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -202,27 +206,30 @@
 msgid "Are you sure you want to ship the shipment?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Realizado"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr ""
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/et.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -203,25 +207,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Tehtud"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Mustand"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Tarni"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Oota"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/fa.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 "برای دریافت یک نقل قول برای خرید :\"%(purchase)s\" شما باید یک آدرس تحویل "
 "ارائه دهید."
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr "برای حذف حمل و نقل قطره :\"%(shipment)s\" شما باید ابتدا آنرا لغو کنید."
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "شما نمیتوانید جابجایی :\"%(move)s\"را به حالت پیش نویس بازنشانی کنید، چراکه "
 "آن توسط یک فروش یا خرید تولید شده است."
@@ -207,25 +211,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/fi.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -205,25 +209,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/fr.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/fr.po`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 msgctxt ""
 "field:purchase.configuration.purchase_drop_location,purchase_drop_location:"
 msgid "Purchase Drop Location"
 msgstr "Emplacement de livraison directe d'achat"
 
 msgctxt "field:purchase.product_supplier,drop_shipment:"
 msgid "Drop Shipment"
-msgstr "Livraison directe"
+msgstr "Expédition directe"
 
 msgctxt "field:purchase.product_supplier,drop_shipment_available:"
 msgid "Drop Shipment Available"
-msgstr "Livraison directe disponible"
+msgstr "Expédition directe disponible"
 
 msgctxt "field:purchase.purchase,customer:"
 msgid "Customer"
 msgstr "Client"
 
 msgctxt "field:purchase.purchase,delivery_address:"
 msgid "Delivery Address"
@@ -29,15 +29,15 @@
 
 msgctxt "field:purchase.purchase,drop_location:"
 msgid "Drop Location"
 msgstr "Emplacement de livraison directe"
 
 msgctxt "field:purchase.purchase,drop_shipments:"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "field:purchase.request,customer:"
 msgid "Customer"
 msgstr "Client"
 
 msgctxt "field:purchase.request,delivery_address:"
 msgid "Delivery Address"
@@ -53,23 +53,23 @@
 
 msgctxt "field:sale.sale,drop_location:"
 msgid "Drop Location"
 msgstr "Emplacement de livraison directe"
 
 msgctxt "field:sale.sale,drop_shipments:"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "field:stock.configuration,shipment_drop_sequence:"
 msgid "Drop Shipment Sequence"
-msgstr "Séquence de livraison directe"
+msgstr "Séquence d'expédition directe"
 
 msgctxt "field:stock.configuration.sequence,shipment_drop_sequence:"
 msgid "Drop Shipment Sequence"
-msgstr "Séquence de livraison directe"
+msgstr "Séquence d'expédition directe"
 
 msgctxt "field:stock.move,customer_drop:"
 msgid "Drop Customer"
 msgstr "Livraison directe cliente"
 
 msgctxt "field:stock.move,moves_drop:"
 msgid "Drop Moves"
@@ -129,35 +129,35 @@
 
 msgctxt "help:stock.shipment.drop,reference:"
 msgid "The external identifier for the shipment."
 msgstr "L'identifiant externe de l'expédition."
 
 msgctxt "model:ir.action,name:act_purchase_drop_shipment_form"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "model:ir.action,name:act_purchase_shipments_relate"
 msgid "Purchases"
 msgstr "Achats"
 
 msgctxt "model:ir.action,name:act_sale_drop_shipment_form"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "model:ir.action,name:act_sale_shipments_relate"
 msgid "Sales"
 msgstr "Ventes"
 
 msgctxt "model:ir.action,name:act_shipment_drop_form"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "model:ir.action,name:act_shipment_drop_relate_party"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_shipment_drop_form_domain_all"
 msgid "All"
 msgstr "Toutes"
 
 msgctxt ""
@@ -183,15 +183,21 @@
 msgstr ""
 "Pour avoir un devis de l'achat « %(purchase)s », vous devez fournir une "
 "adresse de livraison."
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
-"Pour supprimer la livraison directes « %(shipment)s », vous devez l'annuler."
+"Pour supprimer l’expédiions directes « %(shipment)s », vous devez l'annuler."
+
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+"Pour diviser un mouvement d'expédition directe, vous devez utiliser "
+"l'assistant de division.."
 
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "Vous ne pouvez pas réinitialiser à l'état brouillon le mouvement "
@@ -206,44 +212,48 @@
 msgstr "Êtes-vous sûr de vouloir livrer l'expédition ?"
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Effectuée"
+msgid "Complete"
+msgstr "Terminer"
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Livrer"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr "Diviser"
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Attendre"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.sequence,name:sequence_shipment_drop"
 msgid "Drop Shipment"
-msgstr "Livraison directe"
+msgstr "Expédition directe"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_shipment_drop"
 msgid "Drop Shipment"
-msgstr "Livraison directe"
+msgstr "Expédition directe"
 
 msgctxt "model:ir.ui.menu,name:menu_shipment_drop_form"
 msgid "Drop Shipments"
-msgstr "Livraisons directes"
+msgstr "Expéditions directes"
 
 msgctxt "model:purchase.configuration.purchase_drop_location,name:"
 msgid "Purchase Configuration Purchase Drop Location"
 msgstr "Configuration d'achat Emplacement de livraison directe d'achat"
 
 msgctxt "model:sale.configuration.sale_drop_location,name:"
 msgid "Sale Configuration Sale Drop Location"
@@ -251,15 +261,15 @@
 
 msgctxt "model:stock.location,name:location_drop"
 msgid "Drop"
 msgstr "Livraison directe"
 
 msgctxt "model:stock.shipment.drop,name:"
 msgid "Drop Shipment"
-msgstr "Livraison directe"
+msgstr "Expédition directe"
 
 msgctxt "selection:stock.shipment.drop,state:"
 msgid "Cancelled"
 msgstr "Annulée"
 
 msgctxt "selection:stock.shipment.drop,state:"
 msgid "Done"
@@ -275,8 +285,8 @@
 
 msgctxt "selection:stock.shipment.drop,state:"
 msgid "Waiting"
 msgstr "En attente"
 
 msgctxt "view:stock.configuration:"
 msgid "Drop Shipment Sequence"
-msgstr "Séquence de livraison directe"
+msgstr "Séquence d'expédition directe"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/hu.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -214,25 +218,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/id.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -202,25 +206,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Batal"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr ""
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/it.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -213,25 +217,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Annulla"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/lo.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -213,25 +217,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/lt.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 msgctxt "field:purchase.purchase,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:purchase.purchase,delivery_address:"
 msgid "Delivery Address"
-msgstr "Siuntimo adresas"
+msgstr ""
 
 msgctxt "field:purchase.purchase,drop_location:"
 msgid "Drop Location"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.purchase,drop_shipments:"
@@ -39,15 +39,15 @@
 
 msgctxt "field:purchase.request,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:purchase.request,delivery_address:"
 msgid "Delivery Address"
-msgstr "Siuntimo adresas"
+msgstr ""
 
 msgctxt "field:sale.configuration,sale_drop_location:"
 msgid "Sale Drop Location"
 msgstr ""
 
 msgctxt "field:sale.configuration.sale_drop_location,sale_drop_location:"
 msgid "Sale Drop Location"
@@ -80,31 +80,31 @@
 
 msgctxt "field:stock.move,origin_drop:"
 msgid "Drop Origin"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:stock.shipment.drop,contact_address:"
 msgid "Contact Address"
-msgstr "Kontaktinis adresas"
+msgstr ""
 
 msgctxt "field:stock.shipment.drop,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,customer_moves:"
 msgid "Customer Moves"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,delivery_address:"
 msgid "Delivery Address"
-msgstr "Siuntimo adresas"
+msgstr ""
 
 msgctxt "field:stock.shipment.drop,moves:"
 msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,number:"
 msgid "Number"
@@ -136,23 +136,23 @@
 
 msgctxt "model:ir.action,name:act_purchase_drop_shipment_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 msgctxt "model:ir.action,name:act_purchase_shipments_relate"
 msgid "Purchases"
-msgstr "Pirkimai"
+msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_sale_drop_shipment_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 msgctxt "model:ir.action,name:act_sale_shipments_relate"
 msgid "Sales"
-msgstr "Pardavimai"
+msgstr "Sales"
 
 msgctxt "model:ir.action,name:act_shipment_drop_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_drop_relate_party"
@@ -186,14 +186,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -205,25 +209,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/nl.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/nl.po`

 * *Files 6% similar despite different names*

```diff
@@ -177,22 +177,28 @@
 
 msgctxt ""
 "model:ir.message,text:msg_delivery_address_required_quotation_purchase"
 msgid ""
 "To get a quotation for purchase \"%(purchase)s\" you must provide a delivery"
 " address."
 msgstr ""
-"Om een offerte te krijgen voor aankoop \"% (purchase) s\" moet u een "
+"Om een offerte te krijgen voor aankoop \"%(purchase) s\" moet u een "
 "afleveradres opgeven."
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 "Om spoed-verzending \"%(shipment)s\" te verwijderen, moet u deze annuleren."
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+"Om een voorraadboeking van een dropverzending te maken, moet u de wizard "
+"gebruiken."
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 "U kunt de beweging \"%(move)s\" niet terugzetten naar concept omdat deze is "
 "gegenereerd door een verkoop of een aankoop."
@@ -206,25 +212,29 @@
 msgstr "Weet u zeker dat u de zending wilt verzenden?"
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Klaar"
+msgid "Complete"
+msgstr "Voltooien"
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Concept"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "verzenden"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr "Splitsen"
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "wachten"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr "Gebruiker in het bedrijf"
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/pl.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/pl.po`

 * *Files 4% similar despite different names*

```diff
@@ -191,14 +191,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -210,25 +214,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/pt.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -210,25 +214,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/ro.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -182,14 +182,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -201,25 +205,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr ""
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/ru.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -221,25 +225,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/sl.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -210,25 +214,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/tr.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 msgctxt "field:purchase.purchase,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:purchase.purchase,delivery_address:"
 msgid "Delivery Address"
-msgstr ""
+msgstr "Siuntimo adresas"
 
 msgctxt "field:purchase.purchase,drop_location:"
 msgid "Drop Location"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.purchase,drop_shipments:"
@@ -39,15 +39,15 @@
 
 msgctxt "field:purchase.request,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:purchase.request,delivery_address:"
 msgid "Delivery Address"
-msgstr ""
+msgstr "Siuntimo adresas"
 
 msgctxt "field:sale.configuration,sale_drop_location:"
 msgid "Sale Drop Location"
 msgstr ""
 
 msgctxt "field:sale.configuration.sale_drop_location,sale_drop_location:"
 msgid "Sale Drop Location"
@@ -80,31 +80,31 @@
 
 msgctxt "field:stock.move,origin_drop:"
 msgid "Drop Origin"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:stock.shipment.drop,contact_address:"
 msgid "Contact Address"
-msgstr ""
+msgstr "Kontaktinis adresas"
 
 msgctxt "field:stock.shipment.drop,customer:"
 msgid "Customer"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,customer_moves:"
 msgid "Customer Moves"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,delivery_address:"
 msgid "Delivery Address"
-msgstr ""
+msgstr "Siuntimo adresas"
 
 msgctxt "field:stock.shipment.drop,moves:"
 msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.shipment.drop,number:"
 msgid "Number"
@@ -136,23 +136,23 @@
 
 msgctxt "model:ir.action,name:act_purchase_drop_shipment_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 msgctxt "model:ir.action,name:act_purchase_shipments_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr "Pirkimai"
 
 msgctxt "model:ir.action,name:act_sale_drop_shipment_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 msgctxt "model:ir.action,name:act_sale_shipments_relate"
 msgid "Sales"
-msgstr "Sales"
+msgstr "Pardavimai"
 
 msgctxt "model:ir.action,name:act_shipment_drop_form"
 msgid "Drop Shipments"
 msgstr "Drop Shipments"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_shipment_drop_relate_party"
@@ -186,14 +186,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -205,25 +209,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/uk.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/uk.po`

 * *Files 4% similar despite different names*

```diff
@@ -182,14 +182,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -201,25 +205,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr ""
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/locale/zh_CN.po` & `trytond_sale_supply_drop_shipment-7.2.1/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,18 @@
 " address."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_drop_shipment_delete_cancel"
 msgid "To delete drop shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_move_split_drop"
+msgid "To split move from drop shipment, you must use the split wizard."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_reset_move"
 msgid ""
 "You cannot reset move \"%(move)s\" to draft because it was generated by a "
 "sale or a purchase."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:shipment_drop_done_button"
@@ -207,25 +211,29 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:shipment_drop_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:shipment_drop_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:shipment_drop_ship_button"
 msgid "Ship"
 msgstr "Ship"
 
+msgctxt "model:ir.model.button,string:shipment_drop_split_wizard_button"
+msgid "Split"
+msgstr ""
+
 msgctxt "model:ir.model.button,string:shipment_drop_wait_button"
 msgid "Wait"
 msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_drop_companies"
 msgid "User in companies"
 msgstr ""
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/message.xml` & `trytond_sale_supply_drop_shipment-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/party.py` & `trytond_sale_supply_drop_shipment-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/product.py` & `trytond_sale_supply_drop_shipment-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/purchase.py` & `trytond_sale_supply_drop_shipment-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/purchase.xml` & `trytond_sale_supply_drop_shipment-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/sale.py` & `trytond_sale_supply_drop_shipment-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/sale.xml` & `trytond_sale_supply_drop_shipment-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/setup.py` & `trytond_sale_supply_drop_shipment-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/stock.py` & `trytond_sale_supply_drop_shipment-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/stock.xml` & `trytond_sale_supply_drop_shipment-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment.rst` & `trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst` & `trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst` & `trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_split.rst` & `trytond_sale_supply_drop_shipment-7.2.1/tests/scenario_sale_supply_drop_shipment_split.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tests/test_module.py` & `trytond_sale_supply_drop_shipment-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/tox.ini` & `trytond_sale_supply_drop_shipment-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO` & `trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_drop_shipment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale supply drop shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt` & `trytond_sale_supply_drop_shipment-7.2.1/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/view/purchase_form.xml` & `trytond_sale_supply_drop_shipment-7.2.1/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/view/sale_form.xml` & `trytond_sale_supply_drop_shipment-7.2.1/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_form.xml` & `trytond_sale_supply_drop_shipment-7.2.1/view/shipment_drop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_tree.xml` & `trytond_sale_supply_drop_shipment-7.2.1/view/shipment_drop_tree.xml`

 * *Files identical despite different names*

