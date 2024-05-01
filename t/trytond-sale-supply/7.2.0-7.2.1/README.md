# Comparing `tmp/trytond_sale_supply-7.2.0.tar.gz` & `tmp/trytond_sale_supply-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply-7.2.0.tar", last modified: Mon Apr 29 15:50:13 2024, max compression
+gzip compressed data, was "trytond_sale_supply-7.2.1.tar", last modified: Wed May  1 11:17:41 2024, max compression
```

## Comparing `trytond_sale_supply-7.2.0.tar` & `trytond_sale_supply-7.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2334 2024-04-29 15:27:03.000000 trytond_sale_supply-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:27:03.000000 trytond_sale_supply-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_supply-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1885 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1898 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1553 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1684 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1809 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1852 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1628 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1699 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1728 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-02-04 18:51:26.000000 trytond_sale_supply-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2069 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10362 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-03-17 11:01:36.000000 trytond_sale_supply-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2854 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7830 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4144 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_request_cancelled.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3809 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3333 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_stock_first.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_supply-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-04-29 15:26:59.000000 trytond_sale_supply-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1992 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2024-05-01 11:17:38.000000 trytond_sale_supply-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:17:37.000000 trytond_sale_supply-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.106094 trytond_sale_supply-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1901 2024-04-30 17:21:59.000000 trytond_sale_supply-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1885 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1898 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1852 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1628 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1728 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2069 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10362 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2854 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7830 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/scenario_sale_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/scenario_sale_supply_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4144 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/scenario_sale_supply_request_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3809 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/scenario_sale_supply_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3333 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/scenario_sale_supply_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-04-30 17:21:06.000000 trytond_sale_supply-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1992 2024-05-01 11:17:41.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:17:40.000000 trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:17:41.109429 trytond_sale_supply-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2024-04-30 17:21:00.000000 trytond_sale_supply-7.2.1/view/template_form.xml
```

### Comparing `trytond_sale_supply-7.2.0/CHANGELOG` & `trytond_sale_supply-7.2.1/CHANGELOG`

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

### Comparing `trytond_sale_supply-7.2.0/COPYRIGHT` & `trytond_sale_supply-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/LICENSE` & `trytond_sale_supply-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/PKG-INFO` & `trytond_sale_supply-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-7.2.0/README.rst` & `trytond_sale_supply-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/__init__.py` & `trytond_sale_supply-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/doc/conf.py` & `trytond_sale_supply-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/doc/index.rst` & `trytond_sale_supply-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/bg.po` & `trytond_sale_supply-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/ca.po` & `trytond_sale_supply-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
 msgid "The product \"%(product)s\" is supplied on sale."
 msgstr "El producte \"%(product)s\" es subministra a la venda."
 
 msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
 msgid "The product has purchase order points \"%(order_points)s\" defined."
 msgstr ""
-"El producte te regles d'aprovisionament de compra \"%(order_point)s\" "
+"El producte té regles d'aprovisionament de compra \"%(order_points)s\" "
 "definits."
 
 msgctxt "selection:product.product,supply_on_sale:"
 msgid "Always"
 msgstr "Sempre"
 
 msgctxt "selection:product.product,supply_on_sale:"
```

### Comparing `trytond_sale_supply-7.2.0/locale/cs.po` & `trytond_sale_supply-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/de.po` & `trytond_sale_supply-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/es.po` & `trytond_sale_supply-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/es_419.po` & `trytond_sale_supply-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/et.po` & `trytond_sale_supply-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/fa.po` & `trytond_sale_supply-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/fi.po` & `trytond_sale_supply-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/fr.po` & `trytond_sale_supply-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/hu.po` & `trytond_sale_supply-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/id.po` & `trytond_sale_supply-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/it.po` & `trytond_sale_supply-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/lo.po` & `trytond_sale_supply-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/lt.po` & `trytond_sale_supply-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/nl.po` & `trytond_sale_supply-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/pl.po` & `trytond_sale_supply-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/pt.po` & `trytond_sale_supply-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/ro.po` & `trytond_sale_supply-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/ru.po` & `trytond_sale_supply-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/sl.po` & `trytond_sale_supply-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/tr.po` & `trytond_sale_supply-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/uk.po` & `trytond_sale_supply-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/locale/zh_CN.po` & `trytond_sale_supply-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/message.xml` & `trytond_sale_supply-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/product.py` & `trytond_sale_supply-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/purchase.py` & `trytond_sale_supply-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/sale.py` & `trytond_sale_supply-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/sale.xml` & `trytond_sale_supply-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/setup.py` & `trytond_sale_supply-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/stock.py` & `trytond_sale_supply-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tests/scenario_sale_supply.rst` & `trytond_sale_supply-7.2.1/tests/scenario_sale_supply.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_notifications.rst` & `trytond_sale_supply-7.2.1/tests/scenario_sale_supply_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_request_cancelled.rst` & `trytond_sale_supply-7.2.1/tests/scenario_sale_supply_request_cancelled.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_shipment_on_invoice.rst` & `trytond_sale_supply-7.2.1/tests/scenario_sale_supply_shipment_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_stock_first.rst` & `trytond_sale_supply-7.2.1/tests/scenario_sale_supply_stock_first.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/tox.ini` & `trytond_sale_supply-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/PKG-INFO` & `trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/SOURCES.txt` & `trytond_sale_supply-7.2.1/trytond_sale_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

