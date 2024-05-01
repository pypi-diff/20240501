# Comparing `tmp/trytond_sale_shipment_tolerance-7.2.0.tar.gz` & `tmp/trytond_sale_shipment_tolerance-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_tolerance-7.2.0.tar", last modified: Mon Apr 29 15:49:47 2024, max compression
+gzip compressed data, was "trytond_sale_shipment_tolerance-7.2.1.tar", last modified: Wed May  1 11:18:29 2024, max compression
```

## Comparing `trytond_sale_shipment_tolerance-7.2.0.tar` & `trytond_sale_shipment_tolerance-7.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1322 2024-04-29 15:26:43.000000 trytond_sale_shipment_tolerance-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:26:43.000000 trytond_sale_shipment_tolerance-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2585 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:29.000000 trytond_sale_shipment_tolerance-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:26.000000 trytond_sale_shipment_tolerance-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-04-27 16:43:26.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2050 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2220 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2099 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2128 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2051 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2925 2024-02-04 18:51:26.000000 trytond_sale_shipment_tolerance-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4409 2024-03-17 11:01:36.000000 trytond_sale_shipment_tolerance-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3215 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_over_shipment_tolerance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2807 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_under_shipment_tolerance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:29.000000 trytond_sale_shipment_tolerance-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2024-04-29 15:26:39.000000 trytond_sale_shipment_tolerance-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1794 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1023 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/view/configuration_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.689104 trytond_sale_shipment_tolerance-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1423 2024-05-01 11:18:26.000000 trytond_sale_shipment_tolerance-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:18:26.000000 trytond_sale_shipment_tolerance-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-01 11:18:29.689104 trytond_sale_shipment_tolerance-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2585 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.685769 trytond_sale_shipment_tolerance-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.685769 trytond_sale_shipment_tolerance-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2130 2024-04-30 17:21:59.000000 trytond_sale_shipment_tolerance-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2050 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2220 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2099 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2128 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2051 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2925 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:18:29.689104 trytond_sale_shipment_tolerance-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4409 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.685769 trytond_sale_shipment_tolerance-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3215 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tests/scenario_sale_over_shipment_tolerance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2807 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tests/scenario_sale_under_shipment_tolerance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2024-04-30 17:21:06.000000 trytond_sale_shipment_tolerance-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.689104 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1794 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:18:29.000000 trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:29.689104 trytond_sale_shipment_tolerance-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1023 2024-04-30 17:21:00.000000 trytond_sale_shipment_tolerance-7.2.1/view/configuration_form.xml
```

### Comparing `trytond_sale_shipment_tolerance-7.2.0/CHANGELOG` & `trytond_sale_shipment_tolerance-7.2.1/CHANGELOG`

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

### Comparing `trytond_sale_shipment_tolerance-7.2.0/COPYRIGHT` & `trytond_sale_shipment_tolerance-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/LICENSE` & `trytond_sale_shipment_tolerance-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/PKG-INFO` & `trytond_sale_shipment_tolerance-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_tolerance
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define tolerance for sale shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_shipment_tolerance-7.2.0/configuration.py` & `trytond_sale_shipment_tolerance-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/doc/conf.py` & `trytond_sale_shipment_tolerance-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/bg.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/ca.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 msgstr "El percentatge de quantitat mínim a acceptar com a enviat."
 
 msgctxt "model:ir.message,text:msg_over_shipment"
 msgid ""
 "The sale line \"%(line)s\" exceeds the over shipment tolerance (%(shipped)s "
 "shipped > %(maximal)s )."
 msgstr ""
-"La línia de venda \"%s\" sobrepassa la tolerància d'enviament excessiu "
-"(%(shipped)s enviat > %(maximal)s )."
+"La línia de venda \"%(line)s\" sobrepassa la tolerància d'enviament excessiu"
+" (%(shipped)s enviat > %(maximal)s )."
 
 msgctxt "model:sale.configuration.shipment_tolerance,name:"
 msgid "Sale Configuration Shipment Tolerance"
 msgstr "Configuració de la tolerància d'enviament de venda"
 
 msgctxt "view:sale.configuration:"
 msgid "%"
```

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/cs.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/de.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/es.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/es_419.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/et.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/fa.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/fi.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/fr.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/hu.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/id.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/it.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/lo.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/lt.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/nl.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/pl.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/pt.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/ro.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/ru.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/sl.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/tr.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/uk.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/locale/zh_CN.po` & `trytond_sale_shipment_tolerance-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/sale.py` & `trytond_sale_shipment_tolerance-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/setup.py` & `trytond_sale_shipment_tolerance-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/stock.py` & `trytond_sale_shipment_tolerance-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_over_shipment_tolerance.rst` & `trytond_sale_shipment_tolerance-7.2.1/tests/scenario_sale_over_shipment_tolerance.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_under_shipment_tolerance.rst` & `trytond_sale_shipment_tolerance-7.2.1/tests/scenario_sale_under_shipment_tolerance.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/tox.ini` & `trytond_sale_shipment_tolerance-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO` & `trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_tolerance
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to define tolerance for sale shipment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt` & `trytond_sale_shipment_tolerance-7.2.1/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.2.0/view/configuration_form.xml` & `trytond_sale_shipment_tolerance-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

