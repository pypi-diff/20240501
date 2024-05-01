# Comparing `tmp/trytond_production-7.2.0.tar.gz` & `tmp/trytond_production-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production-7.2.0.tar", last modified: Mon Apr 29 15:43:58 2024, max compression
+gzip compressed data, was "trytond_production-7.2.1.tar", last modified: Wed May  1 11:52:43 2024, max compression
```

## Comparing `trytond_production-7.2.0.tar` & `trytond_production-7.2.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     4169 2024-04-29 15:22:30.000000 trytond_production-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:22:30.000000 trytond_production-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-04-29 15:43:58.843868 trytond_production-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:30:39.000000 trytond_production-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-01-27 09:58:52.000000 trytond_production-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9434 2024-04-27 16:30:39.000000 trytond_production-7.2.0/bom.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6250 2024-04-27 16:30:39.000000 trytond_production-7.2.0/bom.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1826 2024-01-27 09:58:52.000000 trytond_production-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-27 16:30:39.000000 trytond_production-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.837201 trytond_production-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3141 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:17.000000 trytond_production-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-04-15 07:12:15.000000 trytond_production-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.837201 trytond_production-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-01-16 14:00:20.000000 trytond_production-7.2.0/icons/tryton-production.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      951 2024-04-27 16:30:39.000000 trytond_production-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.840535 trytond_production-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14569 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14348 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12671 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14334 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14215 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11823 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13229 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14373 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12658 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14272 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13334 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12270 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13882 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14285 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12731 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14089 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13274 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13811 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14032 2024-04-29 13:17:17.000000 trytond_production-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13667 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13554 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11806 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12726 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-04-15 07:12:15.000000 trytond_production-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4297 2024-01-27 09:58:52.000000 trytond_production-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4152 2024-04-27 16:30:39.000000 trytond_production-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32160 2024-04-27 16:30:39.000000 trytond_production-7.2.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12522 2024-04-27 16:30:39.000000 trytond_production-7.2.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:58.843868 trytond_production-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-04-27 16:30:39.000000 trytond_production-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2024-04-27 16:30:39.000000 trytond_production-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-27 16:30:39.000000 trytond_production-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.840535 trytond_production-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7298 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2722 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_by_product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2908 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_lot_trace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_no_list_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2454 2024-04-22 12:14:36.000000 trytond_production-7.2.0/tests/scenario_production_rounding.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3137 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_set_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_waste.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-02-04 18:51:26.000000 trytond_production-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:17.000000 trytond_production-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-29 15:22:25.000000 trytond_production-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/trytond_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_production-7.2.0/trytond_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_input_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_input_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_output_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_output_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_tree_open_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/bom_tree_open_tree_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_tree_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_production-7.2.0/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_production-7.2.0/view/product_bom_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-01-27 09:58:52.000000 trytond_production-7.2.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_calendar.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-27 16:30:39.000000 trytond_production-7.2.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.790678 trytond_production-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-05-01 11:52:40.000000 trytond_production-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:52:40.000000 trytond_production-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_production-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_production-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-01 11:52:43.790678 trytond_production-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond_production-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9434 2024-04-30 17:20:59.000000 trytond_production-7.2.1/bom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6250 2024-04-30 17:21:00.000000 trytond_production-7.2.1/bom.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1826 2024-04-30 17:21:00.000000 trytond_production-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond_production-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.780678 trytond_production-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond_production-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3141 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_production-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-30 17:21:00.000000 trytond_production-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.780678 trytond_production-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_production-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:21:00.000000 trytond_production-7.2.1/icons/tryton-production.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      951 2024-04-30 17:21:00.000000 trytond_production-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.784011 trytond_production-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14469 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14254 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12571 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14121 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11753 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13125 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14267 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12558 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14177 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13234 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12183 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13781 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14185 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12631 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14004 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13174 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13709 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13934 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14626 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13454 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11736 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12626 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2024-04-30 17:21:00.000000 trytond_production-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4297 2024-04-30 17:20:59.000000 trytond_production-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4152 2024-04-30 17:21:00.000000 trytond_production-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32160 2024-04-30 17:20:59.000000 trytond_production-7.2.1/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12522 2024-04-30 17:21:00.000000 trytond_production-7.2.1/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:52:43.790678 trytond_production-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-04-30 17:21:00.000000 trytond_production-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2024-04-30 17:21:00.000000 trytond_production-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-30 17:21:00.000000 trytond_production-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7298 2024-04-30 17:20:59.000000 trytond_production-7.2.1/tests/scenario_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2722 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_by_product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-30 17:20:59.000000 trytond_production-7.2.1/tests/scenario_production_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2908 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_lot_trace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_no_list_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_rounding.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3137 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_set_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_waste.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-30 17:21:06.000000 trytond_production-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/trytond_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_input_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_input_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_output_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_output_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_open_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_open_tree_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_calendar.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/template_list.xml
```

### Comparing `trytond_production-7.2.0/CHANGELOG` & `trytond_production-7.2.1/CHANGELOG`

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
 * Rename 'done' button to 'do'
 * Fill production number only in waiting state
 
 Version 7.0.0 - 2023-10-30
```

### Comparing `trytond_production-7.2.0/COPYRIGHT` & `trytond_production-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/LICENSE` & `trytond_production-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/PKG-INFO` & `trytond_production-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production-7.2.0/__init__.py` & `trytond_production-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/bom.py` & `trytond_production-7.2.1/bom.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/bom.xml` & `trytond_production-7.2.1/bom.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/configuration.py` & `trytond_production-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/configuration.xml` & `trytond_production-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/doc/conf.py` & `trytond_production-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/doc/design.rst` & `trytond_production-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/icons/LICENSE` & `trytond_production-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/ir.py` & `trytond_production-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/locale/bg.po` & `trytond_production-7.2.1/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -426,16 +426,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -550,19 +550,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Производства"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/ca.po` & `trytond_production-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -398,16 +398,16 @@
 msgstr "Reserva"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Finalitza"
+msgid "Complete"
+msgstr "Completa"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Esborrany"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -510,18 +510,14 @@
 msgstr "Administració de producció"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Producció"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Reserva les produccions"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Replanifica les produccions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Estableix cost a partir dels moviments"
```

### Comparing `trytond_production-7.2.0/locale/cs.po` & `trytond_production-7.2.1/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -413,16 +413,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -531,19 +531,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/de.po` & `trytond_production-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -400,16 +400,16 @@
 msgstr "Reservieren"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Annullieren"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Erledigt"
+msgid "Complete"
+msgstr "Fertigstellen"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -421,15 +421,15 @@
 
 msgctxt "model:ir.model.button,string:production_wait_button"
 msgid "Wait"
 msgstr "Warten"
 
 msgctxt "model:ir.rule.group,name:rule_group_production_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_production"
 msgid "Production"
 msgstr "Produktion"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_production"
 msgid "Production"
@@ -512,18 +512,14 @@
 msgstr "Produktion Administration"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Produktion"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Produktionsaufträge reservieren"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Produktionsaufträge neu planen"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Einstandspreis auf Warenbewegungen setzen"
```

### Comparing `trytond_production-7.2.0/locale/es.po` & `trytond_production-7.2.1/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -399,16 +399,16 @@
 msgstr "Reservar"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Finalizar"
+msgid "Complete"
+msgstr "Completar"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Borrador"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -511,18 +511,14 @@
 msgstr "Administración de producción"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Producción"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Reserva las producciones"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Replanificar las producciones"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Establecer el coste desde los movimientos"
```

### Comparing `trytond_production-7.2.0/locale/es_419.po` & `trytond_production-7.2.1/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Canel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
@@ -503,18 +503,14 @@
 msgstr ""
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr ""
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr ""
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/et.po` & `trytond_production-7.2.1/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -409,16 +409,16 @@
 msgstr "Omista"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Tühista"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Tehtud"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Mustand"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -525,19 +525,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Tootmine"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Tootmise omistamine"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Tootmised"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/fa.po` & `trytond_production-7.2.1/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -412,16 +412,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -527,19 +527,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "تولید"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "اختصاص تولید"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "تولیدات"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/fi.po` & `trytond_production-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,18 @@
 msgid "Reference"
 msgstr ""
 
 msgctxt "field:production,run_by:"
 msgid "Run By"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:production,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:production,uom_category:"
 msgid "UoM Category"
@@ -116,17 +117,18 @@
 msgid "Warehouse"
 msgstr ""
 
 msgctxt "field:production.bom,inputs:"
 msgid "Inputs"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.bom,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:production.bom,output_products:"
 msgid "Output Products"
 msgstr ""
 
 msgctxt "field:production.bom,outputs:"
 msgid "Outputs"
@@ -170,17 +172,18 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:production.bom.output,uom_category:"
 msgid "Uom Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:production.bom.tree,childs:"
 msgid "Childs"
-msgstr ""
+msgstr "子项"
 
 msgctxt "field:production.bom.tree,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:production.bom.tree,quantity:"
 msgid "Quantity"
@@ -323,15 +326,15 @@
 msgctxt "model:ir.action,name:act_production_calendar"
 msgid "Productions"
 msgstr "Productions"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_production_configuration_form"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "设置"
 
 msgctxt "model:ir.action,name:act_production_list"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:ir.action,name:wizard_bom_tree_open"
 msgid "BOM Tree"
@@ -348,18 +351,19 @@
 msgstr "As Inputs"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_output"
 msgid "As Outputs"
 msgstr "As Outputs"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_assigned"
 msgid "Assigned"
 msgstr "Assigned"
 
@@ -412,16 +416,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -449,29 +453,29 @@
 
 msgctxt "model:ir.ui.menu,name:menu_bom_list"
 msgid "BOMs"
 msgstr "BOMs"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "设置"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:ir.ui.menu,name:menu_production_calendar"
 msgid "Productions"
 msgstr "Productions"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "设置"
 
 msgctxt "model:ir.ui.menu,name:menu_production_list"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:product.product-production.bom,name:"
 msgid "Product - BOM"
@@ -530,19 +534,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
 
@@ -550,20 +549,20 @@
 msgctxt "selection:production,state:"
 msgid "Assigned"
 msgstr "Assign"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "取消"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Done"
-msgstr "Done"
+msgstr "完成"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Draft"
 msgstr "Draft"
 
 #, fuzzy
@@ -597,20 +596,22 @@
 msgctxt "view:production:"
 msgid "Other Info"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,start,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,start,tree:"
 msgid "OK"
-msgstr ""
+msgstr "确定"
 
+#, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,tree,end:"
 msgid "Close"
-msgstr ""
+msgstr "关闭"
 
 msgctxt "wizard_button:production.bom.tree.open,tree,start:"
 msgid "Change"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_production-7.2.0/locale/fr.po` & `trytond_production-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -401,16 +401,16 @@
 msgstr "Assigner"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Terminée"
+msgid "Complete"
+msgstr "Terminer"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -513,18 +513,14 @@
 msgstr "Administration de la production"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assigner les productions"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Reprogrammer les productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Établir les coûts des mouvements"
```

### Comparing `trytond_production-7.2.0/locale/hu.po` & `trytond_production-7.2.1/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -445,16 +445,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -570,19 +570,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Termelés"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Termelés"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/id.po` & `trytond_production-7.2.1/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Batal"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
@@ -513,19 +513,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Produksi"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Produksi"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Produksi"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/it.po` & `trytond_production-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -412,16 +412,16 @@
 msgstr "Assegna"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Annulla"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Fatto"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Bozza"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -528,19 +528,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Produzione"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/lo.po` & `trytond_production-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -436,16 +436,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -561,19 +561,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "ຜະລິດຕະພັນ"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "ຜະລິດຕະພັນ"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/lt.po` & `trytond_production-7.2.1/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -413,16 +413,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -531,19 +531,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/nl.po` & `trytond_production-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -398,16 +398,16 @@
 msgstr "Toewijzen"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Annuleer"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Gereed"
+msgid "Complete"
+msgstr "Voltooien"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Concept"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -510,18 +510,14 @@
 msgstr "Productie administratie"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Productie"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Wijs productie toe"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions opnieuw plannen"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Stel kosten vast aan de hand van voorraadbewegingen"
```

### Comparing `trytond_production-7.2.0/locale/pl.po` & `trytond_production-7.2.1/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -423,16 +423,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -546,19 +546,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/pt.po` & `trytond_production-7.2.1/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -412,16 +412,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -527,19 +527,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Produção"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Atribuir Produção"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Produções"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/ro.po` & `trytond_production-7.2.1/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -411,16 +411,16 @@
 msgstr "Alocare"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Terminat"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Ciornă"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -527,18 +527,14 @@
 msgstr "Administrare producție"
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Producţie"
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Atribuire Producţie"
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Reprogramare Producţie"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr "Setați costul din mișcări"
```

### Comparing `trytond_production-7.2.0/locale/ru.po` & `trytond_production-7.2.1/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -425,16 +425,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -549,19 +549,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Производства"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/sl.po` & `trytond_production-7.2.1/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -425,16 +425,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -547,19 +547,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/tr.po` & `trytond_production-7.2.1/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -425,16 +425,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -549,19 +549,14 @@
 #, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/uk.po` & `trytond_production-7.2.1/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
+msgid "Complete"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
@@ -503,18 +503,14 @@
 msgstr ""
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr ""
 
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr ""
-
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
```

### Comparing `trytond_production-7.2.0/locale/zh_CN.po` & `trytond_production-7.2.1/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -96,18 +96,17 @@
 msgid "Reference"
 msgstr ""
 
 msgctxt "field:production,run_by:"
 msgid "Run By"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:production,state:"
 msgid "State"
-msgstr "状态"
+msgstr ""
 
 msgctxt "field:production,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:production,uom_category:"
 msgid "UoM Category"
@@ -117,18 +116,17 @@
 msgid "Warehouse"
 msgstr ""
 
 msgctxt "field:production.bom,inputs:"
 msgid "Inputs"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:production.bom,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr ""
 
 msgctxt "field:production.bom,output_products:"
 msgid "Output Products"
 msgstr ""
 
 msgctxt "field:production.bom,outputs:"
 msgid "Outputs"
@@ -172,18 +170,17 @@
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:production.bom.output,uom_category:"
 msgid "Uom Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:production.bom.tree,childs:"
 msgid "Childs"
-msgstr "子项"
+msgstr ""
 
 msgctxt "field:production.bom.tree,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:production.bom.tree,quantity:"
 msgid "Quantity"
@@ -326,15 +323,15 @@
 msgctxt "model:ir.action,name:act_production_calendar"
 msgid "Productions"
 msgstr "Productions"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_production_configuration_form"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_production_list"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:ir.action,name:wizard_bom_tree_open"
 msgid "BOM Tree"
@@ -351,19 +348,18 @@
 msgstr "As Inputs"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_output"
 msgid "As Outputs"
 msgstr "As Outputs"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "All"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_assigned"
 msgid "Assigned"
 msgstr "Assigned"
 
@@ -416,16 +412,16 @@
 msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
-msgid "Done"
-msgstr "Done"
+msgid "Complete"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
@@ -453,29 +449,29 @@
 
 msgctxt "model:ir.ui.menu,name:menu_bom_list"
 msgid "BOMs"
 msgstr "BOMs"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:ir.ui.menu,name:menu_production_calendar"
 msgid "Productions"
 msgstr "Productions"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Configuration"
 
 msgctxt "model:ir.ui.menu,name:menu_production_list"
 msgid "Productions"
 msgstr "Productions"
 
 msgctxt "model:product.product-production.bom,name:"
 msgid "Product - BOM"
@@ -534,19 +530,14 @@
 
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
 msgstr "Production"
 
 #, fuzzy
 msgctxt "selection:ir.cron,method:"
-msgid "Assign Productions"
-msgstr "Assign Production"
-
-#, fuzzy
-msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
 msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
 
@@ -554,20 +545,20 @@
 msgctxt "selection:production,state:"
 msgid "Assigned"
 msgstr "Assign"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Cancelled"
-msgstr "取消"
+msgstr "Cancel"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Done"
-msgstr "完成"
+msgstr "Done"
 
 #, fuzzy
 msgctxt "selection:production,state:"
 msgid "Draft"
 msgstr "Draft"
 
 #, fuzzy
@@ -601,22 +592,20 @@
 msgctxt "view:production:"
 msgid "Other Info"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Cancel"
 
-#, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,start,tree:"
 msgid "OK"
-msgstr "确定"
+msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:production.bom.tree.open,tree,end:"
 msgid "Close"
-msgstr "关闭"
+msgstr ""
 
 msgctxt "wizard_button:production.bom.tree.open,tree,start:"
 msgid "Change"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_production-7.2.0/message.xml` & `trytond_production-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/product.py` & `trytond_production-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/product.xml` & `trytond_production-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/production.py` & `trytond_production-7.2.1/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/production.xml` & `trytond_production-7.2.1/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/setup.py` & `trytond_production-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/stock.py` & `trytond_production-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/stock.xml` & `trytond_production-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production.rst` & `trytond_production-7.2.1/tests/scenario_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_by_product.rst` & `trytond_production-7.2.1/tests/scenario_production_by_product.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_lot_number.rst` & `trytond_production-7.2.1/tests/scenario_production_lot_number.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_lot_trace.rst` & `trytond_production-7.2.1/tests/scenario_production_lot_trace.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_no_list_price.rst` & `trytond_production-7.2.1/tests/scenario_production_no_list_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_rounding.rst` & `trytond_production-7.2.1/tests/scenario_production_rounding.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_set_cost.rst` & `trytond_production-7.2.1/tests/scenario_production_set_cost.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/scenario_production_waste.rst` & `trytond_production-7.2.1/tests/scenario_production_waste.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tests/test_module.py` & `trytond_production-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/tox.ini` & `trytond_production-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/trytond_production.egg-info/PKG-INFO` & `trytond_production-7.2.1/trytond_production.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production-7.2.0/trytond_production.egg-info/SOURCES.txt` & `trytond_production-7.2.1/trytond_production.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/view/location_form.xml` & `trytond_production-7.2.1/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/view/production_form.xml` & `trytond_production-7.2.1/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/view/production_list.xml` & `trytond_production-7.2.1/view/production_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.0/view/template_form.xml` & `trytond_production-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

