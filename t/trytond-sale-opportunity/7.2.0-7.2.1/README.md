# Comparing `tmp/trytond_sale_opportunity-7.2.0.tar.gz` & `tmp/trytond_sale_opportunity-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_opportunity-7.2.0.tar", last modified: Mon Apr 29 15:48:21 2024, max compression
+gzip compressed data, was "trytond_sale_opportunity-7.2.1.tar", last modified: Wed May  1 11:21:26 2024, max compression
```

## Comparing `trytond_sale_opportunity-7.2.0.tar` & `trytond_sale_opportunity-7.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     4109 2024-04-29 15:25:32.000000 trytond_sale_opportunity-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2024-04-29 15:25:32.000000 trytond_sale_opportunity-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1904 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3610 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-22 12:01:28.000000 trytond_sale_opportunity-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_opportunity-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/icons/tryton-sale-opportunity.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.810324 trytond_sale_opportunity-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    12891 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12228 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11501 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12374 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12280 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11446 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12197 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12515 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11492 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12565 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11867 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11126 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12268 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12598 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11648 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12136 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11856 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12278 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12548 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12808 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12307 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11483 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10451 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11600 2024-04-29 13:17:17.000000 trytond_sale_opportunity-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2938 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22612 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10404 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15523 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25162 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:21.816990 trytond_sale_opportunity-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4640 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5386 2024-04-22 12:14:36.000000 trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3919 2024-04-22 12:14:36.000000 trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_opportunity-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-29 15:25:28.000000 trytond_sale_opportunity-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4161 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:21.000000 trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:21.813657 trytond_sale_opportunity-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:21.000000 trytond_sale_opportunity-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2303 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      908 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/view/opportunity_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-27 16:30:39.000000 trytond_sale_opportunity-7.2.0/view/opportunity_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_employee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-01-27 09:58:52.000000 trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      781 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/opportunity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_opportunity-7.2.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:26.006457 trytond_sale_opportunity-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4210 2024-05-01 11:21:22.000000 trytond_sale_opportunity-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2024-05-01 11:21:22.000000 trytond_sale_opportunity-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-05-01 11:21:26.006457 trytond_sale_opportunity-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1904 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:25.996457 trytond_sale_opportunity-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3610 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:25.996457 trytond_sale_opportunity-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/icons/tryton-sale-opportunity.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:25.999790 trytond_sale_opportunity-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13368 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12861 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11953 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13000 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12908 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11898 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12666 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12982 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11944 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13081 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12336 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11596 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12740 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13098 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12100 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12767 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12321 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12750 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13018 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13285 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12772 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11935 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10903 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12067 2024-04-30 17:21:59.000000 trytond_sale_opportunity-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2938 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22612 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/opportunity.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10404 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/opportunity.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15523 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25162 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1280 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:21:26.006457 trytond_sale_opportunity-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4640 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:25.999790 trytond_sale_opportunity-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5386 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tests/scenario_sale_opportunity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3919 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tests/scenario_sale_opportunity_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-30 17:21:06.000000 trytond_sale_opportunity-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:26.003124 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3061 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4161 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:21:25.000000 trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:26.003124 trytond_sale_opportunity-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2303 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      908 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_employee_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_employee_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_employee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      781 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/opportunity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_sale_opportunity-7.2.1/view/party_form.xml
```

### Comparing `trytond_sale_opportunity-7.2.0/CHANGELOG` & `trytond_sale_opportunity-7.2.1/CHANGELOG`

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
 * Add description and note to opportunity line
 * Make product optional on opportunity line
 * Restrict convert button to sale group
```

### Comparing `trytond_sale_opportunity-7.2.0/COPYRIGHT` & `trytond_sale_opportunity-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/LICENSE` & `trytond_sale_opportunity-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/PKG-INFO` & `trytond_sale_opportunity-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_opportunity
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with leads and opportunities
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_opportunity-7.2.0/__init__.py` & `trytond_sale_opportunity-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/configuration.py` & `trytond_sale_opportunity-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/configuration.xml` & `trytond_sale_opportunity-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/doc/conf.py` & `trytond_sale_opportunity-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/doc/design.rst` & `trytond_sale_opportunity-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/icons/LICENSE` & `trytond_sale_opportunity-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/locale/bg.po` & `trytond_sale_opportunity-7.2.1/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -90,30 +90,47 @@
 msgid "Start Date"
 msgstr "Начална дата"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Състояние"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Описание"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Възможност"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Продукт"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Количество"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Единица"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -485,14 +502,22 @@
 msgstr "Месец"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Година"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/ca.po` & `trytond_sale_opportunity-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr "Data inicial"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Estat"
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Descripció"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr "Nota"
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Oportunitat"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Estat de l'oportunitat"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Producte"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr "Categoria UdM del producte"
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Quantitat"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr "Resum"
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Unitat"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -136,14 +152,16 @@
 msgstr "Empleat"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
+"L'adreça predeterminada per a la factura i l'enviament.\n"
+"Deixeu-lo en blanc per utilitzar els valors predeterminats."
 
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Import estimat d'ingressos."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
@@ -434,14 +452,22 @@
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Any"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr "General"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr "Notes"
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/cs.po` & `trytond_sale_opportunity-7.2.1/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
 msgstr ""
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr ""
+msgstr "Adresas"
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr ""
+msgstr "Komentaras"
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
@@ -37,27 +37,27 @@
 #, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
 msgstr "Converted"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valiuta"
 
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Pabaigos data"
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
@@ -65,15 +65,15 @@
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr ""
+msgstr "Kontrahentas"
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
 msgstr ""
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
@@ -82,56 +82,75 @@
 #, fuzzy
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Pradžios data"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
+#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Pradžios data"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Pabaigos data"
 
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
@@ -224,15 +243,15 @@
 msgid "Opportunities"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr "Won"
+msgstr "Vonas"
 
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
@@ -294,15 +313,15 @@
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "Won"
+msgstr "Vonas"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
@@ -452,28 +471,36 @@
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "Won"
+msgstr "Vonas"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/de.po` & `trytond_sale_opportunity-7.2.1/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr "Startdatum"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Status"
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Beschreibung"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr "Notiz"
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Verkaufschance"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Status Verkaufschance"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Artikel"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr "Maßeinheitenkategorie"
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Menge"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr "Kurzbeschreibung"
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Einheit"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Unternehmen"
@@ -136,14 +152,16 @@
 msgstr "Mitarbeiter"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
+"Die Standardadresse für Rechnung und Lieferung.\n"
+"Leer lassen, um die Standardwerte zu verwenden."
 
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Geschätzter Ertrag."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
@@ -314,43 +332,43 @@
 
 msgctxt "model:ir.model.button,string:opportunity_opportunity_button"
 msgid "Convert to Opportunity"
 msgstr "In Verkaufschance umwandeln"
 
 msgctxt "model:ir.rule.group,name:rule_group_opportunity_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_conversion_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_employee_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_employee_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
 msgstr "Verkaufschance"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale_opportunity"
 msgid "Sale Opportunity"
@@ -437,14 +455,22 @@
 msgid "Month"
 msgstr "Monat"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Jahr"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr "Allgemein"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr "Notizen"
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/es.po` & `trytond_sale_opportunity-7.2.1/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr "Fecha inicial"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Estado"
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Descripción"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr "Nota"
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Oportunidad"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Estado de la oportunidad"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Producto"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr "Categoría UdM del producto"
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Cantidad"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr "Resumen"
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Unidad"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Empresa"
@@ -136,14 +152,16 @@
 msgstr "Empleado"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
+"La dirección por defecto para la factura y el albarán.\n"
+"Dejar en blanco para usar los valores por defecto."
 
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Importe estimado de ingresos."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
@@ -433,14 +451,22 @@
 msgid "Month"
 msgstr "Mes"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Año"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr "General"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr "Notas"
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/es_419.po` & `trytond_sale_opportunity-7.2.1/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -87,30 +87,46 @@
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
@@ -461,14 +477,22 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/et.po` & `trytond_sale_opportunity-7.2.1/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -87,30 +87,47 @@
 msgid "Start Date"
 msgstr "Alguskuupäev"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Olek"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Selgitus"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Võimalus"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Võimaluse olek"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Toode"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Kogus"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Ühik"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -476,14 +493,22 @@
 msgstr "Kuu"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Aasta"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/fa.po` & `trytond_sale_opportunity-7.2.1/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -87,30 +87,47 @@
 msgid "Start Date"
 msgstr "تاریخ شروع"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "وضعیت"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "شرح"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "فرصت"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "وضعیت فرصت"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "محصول"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "مقدار/تعداد"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "واحد"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -472,14 +489,22 @@
 msgstr "ماه"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "سال"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/fi.po` & `trytond_sale_opportunity-7.2.1/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 msgid "Converted By"
 msgstr "Converted"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
@@ -84,16 +85,26 @@
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
+msgstr "状态"
+
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "描述"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
@@ -101,29 +112,38 @@
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "写入日期"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
@@ -190,18 +210,19 @@
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Opportunities"
 msgstr "Opportunities"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
 msgstr "Cancelled"
 
 msgctxt ""
@@ -220,18 +241,19 @@
 msgstr "Lost"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_opportunities"
 msgid "Opportunities"
 msgstr "Opportunities"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr "Won"
+msgstr "圆"
 
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
@@ -293,15 +315,15 @@
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "Won"
+msgstr "圆"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
@@ -349,20 +371,20 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale_opportunity"
 msgid "Sale Opportunity"
@@ -451,28 +473,36 @@
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "Won"
+msgstr "圆"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/fr.po` & `trytond_sale_opportunity-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr "Date de début"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "État"
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Description"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr "Note"
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunité"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "État de l'opportunité"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Produit"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr "Catégorie d'UDM du produit"
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Quantité"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr "Résumé"
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Unité"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Société"
@@ -438,14 +454,22 @@
 msgid "Month"
 msgstr "Mois"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Année"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr "Général"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr "Notes"
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/hu.po` & `trytond_sale_opportunity-7.2.1/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -99,32 +99,49 @@
 
 #, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Állapot"
 
 #, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Leírás"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Termék"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Mennyiség"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Egység"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
@@ -487,14 +504,22 @@
 msgstr "Hónap"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Év"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/id.po` & `trytond_sale_opportunity-7.2.1/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -87,30 +87,47 @@
 msgid "Start Date"
 msgstr "Tanggal Awal"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Status"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Deskripsi"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Produk"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -454,14 +471,22 @@
 msgstr "Bulan"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Tahun"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/it.po` & `trytond_sale_opportunity-7.2.1/locale/sl.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,166 +1,182 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.configuration,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr "sequenza opportunity"
+msgstr "Številčna serija priložnosti"
 
-#, fuzzy
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr "sequenza opportunity"
+msgstr "Številčna serija priložnosti"
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr "Indirizzo"
+msgstr "Naslov"
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Znesek"
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr "Commento"
+msgstr "Opomba"
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Družba"
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
-msgstr "Probabilita di conversion"
+msgstr "Verjetnost pretvorbe"
 
 #, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
-msgstr "convertito"
+msgstr "Pretvorjeno"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Opis"
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Zaposlenec"
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
-msgstr "Data finale"
+msgstr "Končni datum"
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
-msgstr "Righe"
+msgstr "Postavke"
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
-msgstr "motivo della perdita"
+msgstr "Razlog za zapravljeno priložnost"
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
-msgstr "Numero"
+msgstr "Številka"
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr "Controparte"
+msgstr "Partner"
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
-msgstr "Termine di pagamento"
+msgstr "Pogoji plačila"
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
-msgstr "Riferimento"
+msgstr "Sklic"
 
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
-msgstr "Vendite"
+msgstr "Prodajni nalogi"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
-msgstr "Data iniziale"
+msgstr "Začetni datum"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
-msgstr "Stato"
+msgstr "Stanje"
+
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Opis"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
-msgstr "opportunity"
+msgstr "Priložnost"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
-msgstr "stato opportunity"
+msgstr "Stanje priložnosti"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "Izdelek"
+
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
-msgstr "Quantità"
+msgstr "Količina"
+
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
-msgstr "Unità"
+msgstr "Enota"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Družba"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Data iniziale"
+msgstr "Začetni datum"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
-msgstr "Data finale"
+msgstr "Končni datum"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Zaposlenec"
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Zaposlenec"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
-msgstr "Importo reddito stimato"
+msgstr "Ocenjen znesek prihodkov"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
-msgstr "percentuale fra 0 e 100"
+msgstr "Odstotek med 0 in 100"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_open_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
@@ -205,18 +221,19 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
 msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "Cancelled"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_converted"
 msgid "Converted"
 msgstr "Converted"
 
@@ -251,93 +268,93 @@
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Znesek"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount_trend"
 msgid "Amount Trend"
-msgstr "Importo"
+msgstr "Znesek"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
-msgstr "tasso di conversione"
+msgstr "Stopnja pretvorbe"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
 msgid "Conversion Trend"
-msgstr "tasso di conversione"
+msgstr "Stopnja pretvorbe"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_converted"
 msgid "Converted"
-msgstr "convertito"
+msgstr "Pretvorjeno"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount"
 msgid "Converted Amount"
-msgstr "importo convertito"
+msgstr "Pretvorjen znesek"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount_trend"
 msgid "Converted Amount Trend"
-msgstr "importo convertito"
+msgstr "Pretvorjen znesek"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_lost"
 msgid "Lost"
-msgstr "Perso"
+msgstr "Zapravljeno"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_help"
 msgid "Number of opportunities"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_trend"
 msgid "Number Trend"
-msgstr "Numero"
+msgstr "Številka"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_rate"
 msgid "Winning Rate"
-msgstr "tasso di aggiudicazione"
+msgstr "Dobljeni delež"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
-msgstr "tasso di aggiudicazione"
+msgstr "Dobljeni delež"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "conseguito"
+msgstr "Dobljeno"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
-msgstr "importo conseguito"
+msgstr "Dobljeni znesek"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
 msgid "Won Amount Trend"
-msgstr "importo conseguito"
+msgstr "Dobljeni znesek"
 
 msgctxt "model:ir.model.button,string:opportunity_cancel_button"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:opportunity_convert_button"
 msgid "Convert to Sale"
 msgstr "Convert to Sale"
 
 msgctxt "model:ir.model.button,string:opportunity_lead_button"
 msgid "Set as Lead"
@@ -372,20 +389,20 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Uporabnik v družbah"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Uporabnik v družbah"
 
 #, fuzzy
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 #, fuzzy
@@ -406,93 +423,101 @@
 #, fuzzy
 msgctxt "model:res.group,name:group_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 msgctxt "model:sale.opportunity,name:"
 msgid "Sale Opportunity"
-msgstr "opportunity di vendita"
+msgstr "Prodajna priložnost"
 
 msgctxt "model:sale.opportunity.line,name:"
 msgid "Sale Opportunity Line"
-msgstr "riga opportunity di vendita"
+msgstr "Postavka prodajne priložnosti"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr "context opportunity di vendita per dipendente"
+msgstr "Kontekst prodajne priložnosti na zaposlenca"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "opportunity di vendita per mese"
+msgstr "Mesečna prodajna priložnost"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.employee,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "opportunity di vendita per dipendente"
+msgstr "Prodajna priložnost na zaposlenca"
 
 #, fuzzy
 msgctxt ""
 "model:sale.opportunity.reporting.conversion.employee.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "opportunity di vendita per dipendente"
+msgstr "Prodajna priložnost na zaposlenca"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "opportunity di vendita per mese"
+msgstr "Mesečna prodajna priložnost"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.main,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "riga opportunity di vendita"
+msgstr "Postavka prodajne priložnosti"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.main.time_series,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "riga opportunity di vendita"
+msgstr "Postavka prodajne priložnosti"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "Preklicano"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Converted"
-msgstr "convertito"
+msgstr "Pretvorjeno"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lead"
-msgstr "lead"
+msgstr "Sled"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lost"
-msgstr "Perso"
+msgstr "Zapravljeno"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
-msgstr "opportunity"
+msgstr "Priložnost"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "conseguito"
+msgstr "Dobljeno"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
-msgstr "Mese"
+msgstr "Mesec"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
-msgstr "Anno"
+msgstr "Leto"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
@@ -502,8 +527,8 @@
 
 msgctxt "view:sale.opportunity:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
-msgstr "lead / opportunity"
+msgstr "Sled/Priložnost"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/lo.po` & `trytond_sale_opportunity-7.2.1/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,32 +104,49 @@
 
 #, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "ສະຖານະ"
 
 #, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "ເນື້ອໃນລາຍການ"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "ຜະລິດຕະພັນ"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "ຈຳນວນ"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "ໜ່ວຍ"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
@@ -496,14 +513,22 @@
 msgstr "ເດືອນ"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "ປີ"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/lt.po` & `trytond_sale_opportunity-7.2.1/locale/tr.po`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
 msgstr ""
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr "Adresas"
+msgstr ""
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr "Komentaras"
+msgstr ""
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
@@ -37,27 +37,27 @@
 #, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
 msgstr "Converted"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
-msgstr "Valiuta"
+msgstr ""
 
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
-msgstr "Pabaigos data"
+msgstr ""
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
@@ -65,15 +65,15 @@
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
 msgstr ""
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr "Kontrahentas"
+msgstr ""
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
 msgstr ""
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
@@ -82,59 +82,72 @@
 #, fuzzy
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
-msgstr "Pradžios data"
+msgstr ""
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Pradžios data"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
-msgstr "Pabaigos data"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
@@ -223,19 +236,18 @@
 msgstr "Lost"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_opportunities"
 msgid "Opportunities"
 msgstr "Opportunities"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr "Vonas"
+msgstr "Won"
 
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
@@ -297,15 +309,15 @@
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "Vonas"
+msgstr "Won"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
@@ -455,39 +467,46 @@
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "Vonas"
+msgstr "Won"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
 
-#, fuzzy
 msgctxt "view:sale.opportunity:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/nl.po` & `trytond_sale_opportunity-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr "Start datum"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Status"
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Omschrijving"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr "Notitie"
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Verkoopkans"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Status verkoopkans"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Product"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr "Product eenheidsmaat categorie"
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Hoeveelheid"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr "Samenvatting"
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Bedrijf"
@@ -136,14 +152,16 @@
 msgstr "Werknemer"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
+"Het standaard adres voor de factuur en zending.\n"
+"Laat leeg om de standaard waarden te gebruiken."
 
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
 msgstr "Geschat omzetbedrag."
 
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
@@ -435,14 +453,22 @@
 msgid "Month"
 msgstr "Maand"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Jaar"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr "Algemeen"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr "Notities"
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/pl.po` & `trytond_sale_opportunity-7.2.1/locale/pl.po`

 * *Files 3% similar despite different names*

```diff
@@ -88,30 +88,47 @@
 msgstr "Data rozpoczęcia"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Stan"
 
 #, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Opis"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Produkt"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Ilość"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Jednostka"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -482,14 +499,22 @@
 msgstr "Miesiąc"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Rok"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/pt.po` & `trytond_sale_opportunity-7.2.1/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -87,30 +87,47 @@
 msgid "Start Date"
 msgstr "Data de início"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Estado"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Descrição"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Oportunidade"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Estado da Oportunidade"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Produto"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Quantidade"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Unidade"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -485,14 +502,22 @@
 msgstr "Mês"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Ano"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/ro.po` & `trytond_sale_opportunity-7.2.1/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -88,31 +88,48 @@
 msgid "Start Date"
 msgstr "Data de Început"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Stare"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Descriere"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Oportunitate"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr "Starea oportunității"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Produs"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Cantitate"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Unitate"
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr "Companie"
@@ -460,14 +477,22 @@
 msgid "Month"
 msgstr "Lună"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "An"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/ru.po` & `trytond_sale_opportunity-7.2.1/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -90,30 +90,47 @@
 msgid "Start Date"
 msgstr "Дата начала"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr "Состояние"
 
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Описание"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Возможная продажа"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr "Продукт"
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr "Кол-во"
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr "Единица измерения"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
@@ -486,14 +503,22 @@
 msgstr "Месяц"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr "Год"
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/sl.po` & `trytond_sale_opportunity-7.2.1/locale/it.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,165 +1,183 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.configuration,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr "Številčna serija priložnosti"
+msgstr "sequenza opportunity"
 
+#, fuzzy
 msgctxt "field:sale.configuration.sequence,sale_opportunity_sequence:"
 msgid "Opportunity Sequence"
-msgstr "Številčna serija priložnosti"
+msgstr "sequenza opportunity"
 
 msgctxt "field:sale.opportunity,address:"
 msgid "Address"
-msgstr "Naslov"
+msgstr "Indirizzo"
 
 msgctxt "field:sale.opportunity,amount:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr "Importo"
 
 msgctxt "field:sale.opportunity,comment:"
 msgid "Comment"
-msgstr "Opomba"
+msgstr "Commento"
 
 msgctxt "field:sale.opportunity,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Azienda"
 
 msgctxt "field:sale.opportunity,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:sale.opportunity,conversion_probability:"
 msgid "Conversion Probability"
-msgstr "Verjetnost pretvorbe"
+msgstr "Probabilita di conversion"
 
 #, fuzzy
 msgctxt "field:sale.opportunity,converted_by:"
 msgid "Converted By"
-msgstr "Pretvorjeno"
+msgstr "convertito"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "Descrizione"
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Dipendente"
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
-msgstr "Končni datum"
+msgstr "Data finale"
 
 msgctxt "field:sale.opportunity,lines:"
 msgid "Lines"
-msgstr "Postavke"
+msgstr "Righe"
 
 msgctxt "field:sale.opportunity,lost_reason:"
 msgid "Reason for loss"
-msgstr "Razlog za zapravljeno priložnost"
+msgstr "motivo della perdita"
 
 msgctxt "field:sale.opportunity,number:"
 msgid "Number"
-msgstr "Številka"
+msgstr "Numero"
 
 msgctxt "field:sale.opportunity,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr "Controparte"
 
 msgctxt "field:sale.opportunity,payment_term:"
 msgid "Payment Term"
-msgstr "Pogoji plačila"
+msgstr "Termine di pagamento"
 
 msgctxt "field:sale.opportunity,reference:"
 msgid "Reference"
-msgstr "Sklic"
+msgstr "Riferimento"
 
 msgctxt "field:sale.opportunity,sales:"
 msgid "Sales"
-msgstr "Prodajni nalogi"
+msgstr "Vendite"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
-msgstr "Začetni datum"
+msgstr "Data iniziale"
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "Stato"
+
+#, fuzzy
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr "Descrizione"
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
-msgstr "Priložnost"
+msgstr "opportunity"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
-msgstr "Stanje priložnosti"
+msgstr "stato opportunity"
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
-msgstr "Izdelek"
+msgstr "Prodotto"
+
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
-msgstr "Količina"
+msgstr "Quantità"
+
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
 
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
-msgstr "Enota"
+msgstr "Unità"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Azienda"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr "Začetni datum"
+msgstr "Data iniziale"
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
-msgstr "Končni datum"
+msgstr "Data finale"
 
 #, fuzzy
 msgctxt "field:sale.opportunity.reporting.conversion.employee,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Dipendente"
 
 #, fuzzy
 msgctxt ""
 "field:sale.opportunity.reporting.conversion.employee.time_series,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Dipendente"
 
 msgctxt "help:sale.opportunity,address:"
 msgid ""
 "The default address for the invoice and shipment.\n"
 "Leave empty to use the default values."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:sale.opportunity,amount:"
 msgid "Estimated revenue amount."
-msgstr "Ocenjen znesek prihodkov"
+msgstr "Importo reddito stimato"
 
 #, fuzzy
 msgctxt "help:sale.opportunity,conversion_probability:"
 msgid "Percentage between 0 and 100."
-msgstr "Odstotek med 0 in 100"
+msgstr "percentuale fra 0 e 100"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_open_sale_form"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
@@ -204,19 +222,18 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
 msgstr "All"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
-msgstr "Cancelled"
+msgstr "Annullato"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_converted"
 msgid "Converted"
 msgstr "Converted"
 
@@ -251,93 +268,93 @@
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount"
 msgid "Amount"
-msgstr "Znesek"
+msgstr "Importo"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_amount_trend"
 msgid "Amount Trend"
-msgstr "Znesek"
+msgstr "Importo"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_conversion_rate"
 msgid "Conversion Rate"
-msgstr "Stopnja pretvorbe"
+msgstr "tasso di conversione"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_conversion_trend"
 msgid "Conversion Trend"
-msgstr "Stopnja pretvorbe"
+msgstr "tasso di conversione"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_converted"
 msgid "Converted"
-msgstr "Pretvorjeno"
+msgstr "convertito"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount"
 msgid "Converted Amount"
-msgstr "Pretvorjen znesek"
+msgstr "importo convertito"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_converted_amount_trend"
 msgid "Converted Amount Trend"
-msgstr "Pretvorjen znesek"
+msgstr "importo convertito"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_lost"
 msgid "Lost"
-msgstr "Zapravljeno"
+msgstr "Perso"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_help"
 msgid "Number of opportunities"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_number_trend"
 msgid "Number Trend"
-msgstr "Številka"
+msgstr "Numero"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_rate"
 msgid "Winning Rate"
-msgstr "Dobljeni delež"
+msgstr "tasso di aggiudicazione"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
-msgstr "Dobljeni delež"
+msgstr "tasso di aggiudicazione"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "Dobljeno"
+msgstr "conseguito"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
-msgstr "Dobljeni znesek"
+msgstr "importo conseguito"
 
 #, fuzzy
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
 msgid "Won Amount Trend"
-msgstr "Dobljeni znesek"
+msgstr "importo conseguito"
 
 msgctxt "model:ir.model.button,string:opportunity_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Annulla"
 
 msgctxt "model:ir.model.button,string:opportunity_convert_button"
 msgid "Convert to Sale"
 msgstr "Convert to Sale"
 
 msgctxt "model:ir.model.button,string:opportunity_lead_button"
 msgid "Set as Lead"
@@ -372,20 +389,20 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr "Uporabnik v družbah"
+msgstr ""
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr "Uporabnik v družbah"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 #, fuzzy
@@ -406,93 +423,101 @@
 #, fuzzy
 msgctxt "model:res.group,name:group_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 msgctxt "model:sale.opportunity,name:"
 msgid "Sale Opportunity"
-msgstr "Prodajna priložnost"
+msgstr "opportunity di vendita"
 
 msgctxt "model:sale.opportunity.line,name:"
 msgid "Sale Opportunity Line"
-msgstr "Postavka prodajne priložnosti"
+msgstr "riga opportunity di vendita"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.context,name:"
 msgid "Sale Opportunity Reporting Context"
-msgstr "Kontekst prodajne priložnosti na zaposlenca"
+msgstr "context opportunity di vendita per dipendente"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "Mesečna prodajna priložnost"
+msgstr "opportunity di vendita per mese"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.employee,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "Prodajna priložnost na zaposlenca"
+msgstr "opportunity di vendita per dipendente"
 
 #, fuzzy
 msgctxt ""
 "model:sale.opportunity.reporting.conversion.employee.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion per Employee"
-msgstr "Prodajna priložnost na zaposlenca"
+msgstr "opportunity di vendita per dipendente"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.conversion.time_series,name:"
 msgid "Sale Opportunity Reporting Conversion"
-msgstr "Mesečna prodajna priložnost"
+msgstr "opportunity di vendita per mese"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.main,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "Postavka prodajne priložnosti"
+msgstr "riga opportunity di vendita"
 
 #, fuzzy
 msgctxt "model:sale.opportunity.reporting.main.time_series,name:"
 msgid "Sale Opportunity Reporting"
-msgstr "Postavka prodajne priložnosti"
+msgstr "riga opportunity di vendita"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "Annullato"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Converted"
-msgstr "Pretvorjeno"
+msgstr "convertito"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lead"
-msgstr "Sled"
+msgstr "lead"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Lost"
-msgstr "Zapravljeno"
+msgstr "Perso"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
-msgstr "Priložnost"
+msgstr "opportunity"
 
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "Dobljeno"
+msgstr "conseguito"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
-msgstr "Mesec"
+msgstr "Mese"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
-msgstr "Leto"
+msgstr "Anno"
+
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
@@ -502,8 +527,8 @@
 
 msgctxt "view:sale.opportunity:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
-msgstr "Sled/Priložnost"
+msgstr "lead / opportunity"
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/tr.po` & `trytond_sale_opportunity-7.2.1/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -88,31 +88,47 @@
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
@@ -465,24 +481,33 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr "%"
 
+#, fuzzy
 msgctxt "view:sale.opportunity:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:sale.opportunity:"
 msgid "Lead/Opportunity"
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/uk.po` & `trytond_sale_opportunity-7.2.1/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -86,30 +86,46 @@
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
@@ -433,14 +449,22 @@
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr ""
 
 msgctxt "view:sale.opportunity.reporting.main:"
 msgid "%"
 msgstr ""
```

### Comparing `trytond_sale_opportunity-7.2.0/locale/zh_CN.po` & `trytond_sale_opportunity-7.2.1/locale/cs.po`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,17 @@
 msgid "Converted By"
 msgstr "Converted"
 
 msgctxt "field:sale.opportunity,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity,description:"
 msgid "Description"
-msgstr "描述"
+msgstr ""
 
 msgctxt "field:sale.opportunity,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:sale.opportunity,end_date:"
 msgid "End Date"
@@ -85,48 +84,62 @@
 msgid "Sales"
 msgstr "Sales"
 
 msgctxt "field:sale.opportunity,start_date:"
 msgid "Start Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity,state:"
 msgid "State"
-msgstr "状态"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,description:"
+msgid "Description"
+msgstr ""
+
+msgctxt "field:sale.opportunity.line,note:"
+msgid "Note"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.opportunity.line,opportunity:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 msgctxt "field:sale.opportunity.line,opportunity_state:"
 msgid "Opportunity State"
 msgstr ""
 
 msgctxt "field:sale.opportunity.line,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,product_uom_category:"
+msgid "Product UoM Category"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
+msgctxt "field:sale.opportunity.line,summary:"
+msgid "Summary"
+msgstr ""
+
 msgctxt "field:sale.opportunity.line,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.opportunity.reporting.context,from_date:"
 msgid "From Date"
-msgstr "写入日期"
+msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:sale.opportunity.reporting.context,to_date:"
 msgid "To Date"
@@ -193,19 +206,18 @@
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Opportunities"
 msgstr "Opportunities"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "All"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_cancelled"
 msgid "Cancelled"
 msgstr "Cancelled"
 
 msgctxt ""
@@ -228,15 +240,15 @@
 msgid "Opportunities"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_opportunity_form_domain_won"
 msgid "Won"
-msgstr "圆"
+msgstr "Won"
 
 msgctxt "model:ir.message,text:msg_modify_origin_opportunity"
 msgid "You cannot modify the opportunity origin of the sale \"%(sale)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_opportunity_delete_cancel"
 msgid "To delete opportunity \"%(opportunity)s\", you must cancel it."
@@ -298,15 +310,15 @@
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_winning_trend"
 msgid "Winning Trend"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won"
 msgid "Won"
-msgstr "圆"
+msgstr "Won"
 
 msgctxt "model:ir.message,text:msg_sale_opportunity_reporting_won_amount"
 msgid "Won Amount"
 msgstr ""
 
 msgctxt ""
 "model:ir.message,text:msg_sale_opportunity_reporting_won_amount_trend"
@@ -354,20 +366,20 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_conversion_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr ""
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_sale_opportunity"
 msgid "Sale Opportunity"
 msgstr "Sale Opportunity"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale_opportunity"
 msgid "Sale Opportunity"
@@ -456,28 +468,36 @@
 msgctxt "selection:sale.opportunity,state:"
 msgid "Opportunity"
 msgstr "Opportunities"
 
 #, fuzzy
 msgctxt "selection:sale.opportunity,state:"
 msgid "Won"
-msgstr "圆"
+msgstr "Won"
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Month"
 msgstr ""
 
 msgctxt "selection:sale.opportunity.reporting.context,period:"
 msgid "Year"
 msgstr ""
 
+msgctxt "view:sale.opportunity.line:"
+msgid "General"
+msgstr ""
+
+msgctxt "view:sale.opportunity.line:"
+msgid "Notes"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.conversion:"
 msgid "%"
 msgstr "%"
 
 #, fuzzy
 msgctxt "view:sale.opportunity.reporting.main:"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_opportunity-7.2.0/message.xml` & `trytond_sale_opportunity-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/opportunity.py` & `trytond_sale_opportunity-7.2.1/opportunity.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/opportunity.xml` & `trytond_sale_opportunity-7.2.1/opportunity.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/opportunity_reporting.py` & `trytond_sale_opportunity-7.2.1/opportunity_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/opportunity_reporting.xml` & `trytond_sale_opportunity-7.2.1/opportunity_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/party.py` & `trytond_sale_opportunity-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/party.xml` & `trytond_sale_opportunity-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/sale.py` & `trytond_sale_opportunity-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/setup.py` & `trytond_sale_opportunity-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity.rst` & `trytond_sale_opportunity-7.2.1/tests/scenario_sale_opportunity.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/tests/scenario_sale_opportunity_reporting.rst` & `trytond_sale_opportunity-7.2.1/tests/scenario_sale_opportunity_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/tox.ini` & `trytond_sale_opportunity-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/PKG-INFO` & `trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_opportunity
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with leads and opportunities
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_opportunity-7.2.0/trytond_sale_opportunity.egg-info/SOURCES.txt` & `trytond_sale_opportunity-7.2.1/trytond_sale_opportunity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/view/opportunity_form.xml` & `trytond_sale_opportunity-7.2.1/view/opportunity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/view/opportunity_line_form.xml` & `trytond_sale_opportunity-7.2.1/view/opportunity_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/view/opportunity_reporting_conversion_list.xml` & `trytond_sale_opportunity-7.2.1/view/opportunity_reporting_conversion_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/view/opportunity_reporting_main_list.xml` & `trytond_sale_opportunity-7.2.1/view/opportunity_reporting_main_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-7.2.0/view/opportunity_tree.xml` & `trytond_sale_opportunity-7.2.1/view/opportunity_tree.xml`

 * *Files identical despite different names*

