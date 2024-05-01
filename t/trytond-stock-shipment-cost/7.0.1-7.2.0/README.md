# Comparing `tmp/trytond_stock_shipment_cost-7.0.1.tar.gz` & `tmp/trytond_stock_shipment_cost-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_shipment_cost-7.0.1.tar", last modified: Wed May  1 09:53:07 2024, max compression
+gzip compressed data, was "trytond_stock_shipment_cost-7.2.0.tar", last modified: Mon Apr 29 15:52:53 2024, max compression
```

## Comparing `trytond_stock_shipment_cost-7.0.1.tar` & `trytond_stock_shipment_cost-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      809 2024-05-01 09:53:04.000000 trytond_stock_shipment_cost-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:53:03.000000 trytond_stock_shipment_cost-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2796 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.209967 trytond_stock_shipment_cost-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2024-03-03 16:24:20.000000 trytond_stock_shipment_cost-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2374 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2439 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2418 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2386 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4625 2024-03-03 16:24:03.000000 trytond_stock_shipment_cost-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8603 2024-04-26 15:19:32.000000 trytond_stock_shipment_cost-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1023 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1057 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/stock_reporting_margin.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2024-02-05 16:24:27.000000 trytond_stock_shipment_cost-7.0.1/tests/scenario_stock_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-02-05 16:24:27.000000 trytond_stock_shipment_cost-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2796 2024-05-01 09:53:06.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1858 2024-05-01 09:53:07.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:53:06.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-05-01 09:53:06.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:18.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-05-01 09:53:06.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:53:06.000000 trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:53:07.213300 trytond_stock_shipment_cost-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/view/reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-10-30 17:06:38.000000 trytond_stock_shipment_cost-7.0.1/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      809 2024-04-29 15:29:00.000000 trytond_stock_shipment_cost-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:29:00.000000 trytond_stock_shipment_cost-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2796 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      892 2024-04-13 17:12:23.000000 trytond_stock_shipment_cost-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.903207 trytond_stock_shipment_cost-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:36.000000 trytond_stock_shipment_cost-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2374 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2478 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2439 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2418 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2386 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4625 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8599 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1293 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1057 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/stock_reporting_margin.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3958 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/tests/scenario_stock_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-13 17:12:23.000000 trytond_stock_shipment_cost-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:36.000000 trytond_stock_shipment_cost-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2024-04-29 15:28:56.000000 trytond_stock_shipment_cost-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2796 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1914 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:53.000000 trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:53.906540 trytond_stock_shipment_cost-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/view/reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost-7.2.0/view/shipment_out_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-7.2.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_shipment_cost-7.0.1/CHANGELOG` & `trytond_stock_shipment_cost-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-05-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_shipment_cost-7.0.1/COPYRIGHT` & `trytond_stock_shipment_cost-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/LICENSE` & `trytond_stock_shipment_cost-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/PKG-INFO` & `trytond_stock_shipment_cost-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_cost
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for stock shipment cost
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-shipment-cost/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Stock Shipment Cost Module
 ##########################
 
 The *Stock Shipment Cost Module* adds a shipment cost on the outgoing moves
 which is calculated from the carrier purchase price.
```

### Comparing `trytond_stock_shipment_cost-7.0.1/__init__.py` & `trytond_stock_shipment_cost-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/carrier.py` & `trytond_stock_shipment_cost-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/doc/conf.py` & `trytond_stock_shipment_cost-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/bg.po` & `trytond_stock_shipment_cost-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/ca.po` & `trytond_stock_shipment_cost-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/cs.po` & `trytond_stock_shipment_cost-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/de.po` & `trytond_stock_shipment_cost-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/es.po` & `trytond_stock_shipment_cost-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/es_419.po` & `trytond_stock_shipment_cost-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/et.po` & `trytond_stock_shipment_cost-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/fa.po` & `trytond_stock_shipment_cost-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/fi.po` & `trytond_stock_shipment_cost-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/fr.po` & `trytond_stock_shipment_cost-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/hu.po` & `trytond_stock_shipment_cost-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/id.po` & `trytond_stock_shipment_cost-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/it.po` & `trytond_stock_shipment_cost-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/lo.po` & `trytond_stock_shipment_cost-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/lt.po` & `trytond_stock_shipment_cost-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/nl.po` & `trytond_stock_shipment_cost-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/pl.po` & `trytond_stock_shipment_cost-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/pt.po` & `trytond_stock_shipment_cost-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/ro.po` & `trytond_stock_shipment_cost-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/ru.po` & `trytond_stock_shipment_cost-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/sl.po` & `trytond_stock_shipment_cost-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/tr.po` & `trytond_stock_shipment_cost-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/uk.po` & `trytond_stock_shipment_cost-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/locale/zh_CN.po` & `trytond_stock_shipment_cost-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/setup.py` & `trytond_stock_shipment_cost-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/stock.py` & `trytond_stock_shipment_cost-7.2.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,20 +230,20 @@
                 move.shipment_out_cost_price = cost_price
                 moves.append(move)
         return moves
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, shipments):
+    def do(cls, shipments):
         for shipment in shipments:
             shipment.cost = shipment.cost_used
             shipment.cost_currency = shipment.cost_currency_used
         cls.save(shipments)
-        super().done(shipments)
+        super().do(shipments)
         cls.set_shipment_cost(shipments)
 
 
 class ShipmentOut(ShipmentOutCostMixin, metaclass=PoolMeta):
     __name__ = 'stock.shipment.out'
 
     @property
```

### Comparing `trytond_stock_shipment_cost-7.0.1/stock.xml` & `trytond_stock_shipment_cost-7.2.0/stock.xml`

 * *Files 17% similar despite different names*

#### Comparing `trytond_stock_shipment_cost-7.0.1/stock.xml` & `trytond_stock_shipment_cost-7.2.0/stock.xml`

```diff
@@ -4,14 +4,19 @@
 <tryton>
   <data>
     <record model="ir.ui.view" id="stock_move_view_form">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_form"/>
       <field name="name">stock_move_form</field>
     </record>
+    <record model="ir.ui.view" id="shipment_out_view_list">
+      <field name="model">stock.shipment.out</field>
+      <field name="inherit" ref="stock.shipment_out_view_tree"/>
+      <field name="name">shipment_out_list</field>
+    </record>
     <record model="ir.ui.view" id="shipment_out_view_form">
       <field name="model">stock.shipment.out</field>
       <field name="inherit" ref="stock.shipment_out_view_form"/>
       <field name="name">shipment_out_form</field>
     </record>
     <record model="ir.ui.view" id="shipment_out_return_view_form">
       <field name="model">stock.shipment.out.return</field>
```

### Comparing `trytond_stock_shipment_cost-7.0.1/stock_reporting_margin.py` & `trytond_stock_shipment_cost-7.2.0/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/stock_reporting_margin.xml` & `trytond_stock_shipment_cost-7.2.0/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/tests/scenario_stock_shipment_cost.rst` & `trytond_stock_shipment_cost-7.2.0/tests/scenario_stock_shipment_cost.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Shipment Cost Scenario
 ============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_shipment_cost')
@@ -84,15 +84,15 @@
     >>> shipment.click('wait')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.cost_edit = True
     >>> shipment.cost_used = Decimal('5')
     >>> shipment.cost_currency_used = company.currency
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check move costs::
 
     >>> sorted([
     ...         (m.cost_price, m.shipment_out_cost_price)
@@ -110,18 +110,18 @@
     ...     'period': 'day',
     ...     }
     >>> with config.set_context(context=context):
     ...     reports = MarginProduct.find([])
     ...     time_series = MarginProductTimeseries.find([])
     >>> len(reports)
     2
-    >>> sorted([r.cost for r in reports]) == [Decimal('10.0000'), Decimal('40.0000')]
-    True
+    >>> sorted([r.cost for r in reports])
+    [Decimal('10.00'), Decimal('40.00')]
 
     >>> context['include_shipment_cost'] = True
     >>> with config.set_context(context=context):
     ...     reports = MarginProduct.find([])
     ...     time_series = MarginProductTimeseries.find([])
     >>> len(reports)
     2
-    >>> sorted([r.cost for r in reports]) == [Decimal('11.0000'), Decimal('44.0000')]
-    True
+    >>> sorted([r.cost for r in reports])
+    [Decimal('11.00'), Decimal('44.00')]
```

### Comparing `trytond_stock_shipment_cost-7.0.1/tox.ini` & `trytond_stock_shipment_cost-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/PKG-INFO` & `trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_cost
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for stock shipment cost
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-stock-shipment-cost/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##########################
 Stock Shipment Cost Module
 ##########################
 
 The *Stock Shipment Cost Module* adds a shipment cost on the outgoing moves
 which is calculated from the carrier purchase price.
```

### Comparing `trytond_stock_shipment_cost-7.0.1/trytond_stock_shipment_cost.egg-info/SOURCES.txt` & `trytond_stock_shipment_cost-7.2.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 ./tests/__init__.py
 ./tests/scenario_stock_shipment_cost.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
 ./view/reporting_margin_context_form.xml
 ./view/shipment_out_form.xml
+./view/shipment_out_list.xml
 ./view/stock_move_form.xml
 doc/conf.py
 doc/index.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
@@ -90,8 +91,9 @@
 trytond_stock_shipment_cost.egg-info/entry_points.txt
 trytond_stock_shipment_cost.egg-info/not-zip-safe
 trytond_stock_shipment_cost.egg-info/requires.txt
 trytond_stock_shipment_cost.egg-info/top_level.txt
 view/carrier_form.xml
 view/reporting_margin_context_form.xml
 view/shipment_out_form.xml
+view/shipment_out_list.xml
 view/stock_move_form.xml
```

### Comparing `trytond_stock_shipment_cost-7.0.1/view/shipment_out_form.xml` & `trytond_stock_shipment_cost-7.2.0/view/shipment_out_form.xml`

 * *Files identical despite different names*

