# Comparing `tmp/trytond_sale-7.2.0.tar.gz` & `tmp/trytond_sale-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-7.2.0.tar", last modified: Mon Apr 29 15:46:55 2024, max compression
+gzip compressed data, was "trytond_sale-7.2.1.tar", last modified: Wed May  1 11:28:15 2024, max compression
```

## Comparing `trytond_sale-7.2.0.tar` & `trytond_sale-7.2.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     6684 2024-04-29 15:24:31.000000 trytond_sale-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:24:31.000000 trytond_sale-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9121 2024-03-17 11:01:36.000000 trytond_sale-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_sale-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/presales.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4187 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/reporting.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/returns.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.535913 trytond_sale-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    41606 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42411 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36682 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43131 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42615 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34974 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39927 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    44661 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36643 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43010 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40949 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37869 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39224 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40656 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41015 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42496 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38125 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39436 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42533 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41687 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39131 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36634 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34410 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36942 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4617 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4595 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9027 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2740 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    76278 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    89113 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25512 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    55353 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7637 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.535913 trytond_sale-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1935 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_manual_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12959 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2524 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_sale-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-29 15:24:27.000000 trytond_sale-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5488 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale-7.2.0/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3954 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-09-26 14:46:01.000000 trytond_sale-7.2.0/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6785 2024-05-01 11:28:12.000000 trytond_sale-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:28:12.000000 trytond_sale-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.545745 trytond_sale-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9121 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/presales.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4187 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/reporting.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41783 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42532 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36808 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43272 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42730 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35108 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40072 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    44826 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36769 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43139 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41105 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37993 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39376 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40834 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41176 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42618 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38275 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39584 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42692 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41861 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39277 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36760 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34519 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37068 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4617 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9027 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2740 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76278 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    89113 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25512 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    55353 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7637 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.552412 trytond_sale-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1935 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_manual_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12959 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:21:06.000000 trytond_sale-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5488 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3954 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/template_tree.xml
```

### Comparing `trytond_sale-7.2.0/CHANGELOG` & `trytond_sale-7.2.1/CHANGELOG`

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
 * Permit to remove ignored invoices and stock moves
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_sale-7.2.0/COPYRIGHT` & `trytond_sale-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/LICENSE` & `trytond_sale-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/PKG-INFO` & `trytond_sale-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-7.2.0/__init__.py` & `trytond_sale-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/configuration.py` & `trytond_sale-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/configuration.xml` & `trytond_sale-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/conf.py` & `trytond_sale-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/design.rst` & `trytond_sale-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/usage/presales.inc.rst` & `trytond_sale-7.2.1/doc/usage/presales.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/usage/process.inc.rst` & `trytond_sale-7.2.1/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/usage/reporting.inc.rst` & `trytond_sale-7.2.1/doc/usage/reporting.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/doc/usage/returns.inc.rst` & `trytond_sale-7.2.1/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/icons/LICENSE` & `trytond_sale-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/invoice.py` & `trytond_sale-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/invoice.xml` & `trytond_sale-7.2.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/locale/bg.po` & `trytond_sale-7.2.1/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -1667,18 +1667,28 @@
 msgid "Choose move to recreate:"
 msgstr "Избор на движение за ново създаване"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Основен"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Фактура"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Бележки"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Състояние на пратка"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Данъци"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/ca.po` & `trytond_sale-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -210,18 +210,17 @@
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
-#, fuzzy
 msgctxt "field:sale.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Adreça de facturació"
+msgstr "Progrés de facturació"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -1584,18 +1583,26 @@
 msgstr "Seleccioneu els moviments a recrear:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Facturació"
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Enviament"
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Impostos"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Esteu segur de retornar aquestes comandes de venda?"
```

### Comparing `trytond_sale-7.2.0/locale/cs.po` & `trytond_sale-7.2.1/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -1626,19 +1626,28 @@
 msgid "Choose move to recreate:"
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/de.po` & `trytond_sale-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,18 +210,17 @@
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
-#, fuzzy
 msgctxt "field:sale.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Rechnungsadresse"
+msgstr "Rechnungsfortschritt"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -1110,75 +1109,75 @@
 msgctxt "model:ir.model.button,string:sale_quote_button"
 msgid "Quote"
 msgstr "Angebot"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_country_subdivision_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_country_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_country_tree_companies"
 msgid "User in companies"
 msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_customer_category_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_customer_category_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_customer_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_customer_time_series_companies"
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
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_category_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_category_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_product_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sale_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_sale"
 msgid "Sale"
 msgstr "Verkauf"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale"
 msgid "Sale"
@@ -1589,18 +1588,26 @@
 msgstr "Warenbewegungen zur Neuerstellung auswählen:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Allgemein"
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Rechnungsfortschritt"
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notizen"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Lieferfortschritt"
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Steuern"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
 "Mit der Rücknahme dieses Verkaufs/dieser Verkäufe wirklich fortfahren?"
```

### Comparing `trytond_sale-7.2.0/locale/es.po` & `trytond_sale-7.2.1/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,18 +210,17 @@
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
-#, fuzzy
 msgctxt "field:sale.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Dirección de facturación"
+msgstr "Progreso de facturación"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -981,15 +980,15 @@
 " la venta \"%(sale)s\"."
 
 msgctxt "model:ir.message,text:msg_sale_line_move_quantity"
 msgid ""
 "The sale line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
-"La linea de venta \"%(line)s\" esta movimiendo %(extra)s a demas de los "
+"La linea de venta \"%(line)s\" está moviendo %(extra)s además de los "
 "\"%(quantity)s pedidos."
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
 msgid "A tax can be added only once to a sale line."
 msgstr "Un impuesto solo se puede agregar una vez a una línea de venta."
 
 msgctxt "model:ir.message,text:msg_sale_missing_account_revenue"
@@ -1583,18 +1582,26 @@
 msgstr "Seleccione los movimientos a recrear:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Facturación"
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notas"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Envío"
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Impuestos"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "¿Estás seguro de querer devolver este/os pedido/s de venta?"
```

### Comparing `trytond_sale-7.2.0/locale/es_419.po` & `trytond_sale-7.2.1/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -1553,17 +1553,26 @@
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Estado de envío"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/et.po` & `trytond_sale-7.2.1/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -1667,18 +1667,28 @@
 msgid "Choose move to recreate:"
 msgstr "Vali kanne taasloomiseks"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Üldine"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Arve"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Märkused"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Tarne kuupäev"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Maksud"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/fa.po` & `trytond_sale-7.2.1/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -1679,18 +1679,28 @@
 msgid "Choose move to recreate:"
 msgstr "انتخاب جابجایی برای ایجاد دوباره"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "عمومی"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "صورت حساب"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "یادداشت ها"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "تاریخ ارسال"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "مالیات ها"
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/fi.po` & `trytond_sale-7.2.1/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -1623,19 +1623,28 @@
 msgid "Choose move to recreate:"
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/fr.po` & `trytond_sale-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1583,18 +1583,26 @@
 msgstr "Choisissez les mouvements à recréer :"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Général"
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Facturation"
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Livraison"
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Taxes"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Êtes-vous sûr de retourner ces/cette vente(s) ?"
```

### Comparing `trytond_sale-7.2.0/locale/hu.po` & `trytond_sale-7.2.1/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -1637,18 +1637,28 @@
 msgid "Choose move to recreate:"
 msgstr "Válassza ki a készletmozgásokat, amiket újra létre szeretne hozni:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Általános"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Számla"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Jegyzetek"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Kiszállítás dátuma"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Adók"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Biztos, hogy vissza akarja vételezni ez(eke)t a rendelés(eke)t?"
```

### Comparing `trytond_sale-7.2.0/locale/id.po` & `trytond_sale-7.2.1/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -1625,19 +1625,28 @@
 msgid "Choose move to recreate:"
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Umum"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Faktur"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Catatan-Catatan"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Pajak-Pajak"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Apakah Anda yakin akan mengembalikan penjualan ini?"
```

### Comparing `trytond_sale-7.2.0/locale/it.po` & `trytond_sale-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -1659,18 +1659,28 @@
 msgid "Choose move to recreate:"
 msgstr "Scegliere i movimenti da ricreare:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Generale"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Fattura"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Note"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "data di spedizione"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Imposte"
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/lo.po` & `trytond_sale-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -1717,17 +1717,26 @@
 #, fuzzy
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "ທົ່ວໄປ"
 
 #, fuzzy
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "ໃບເກັບເງິນພາສີທີ່ດິນ"
+
+#, fuzzy
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "ໝາຍເຫດ"
 
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "ອາກອນ"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/lt.po` & `trytond_sale-7.2.1/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1666,18 +1666,28 @@
 msgid "Choose move to recreate:"
 msgstr "Pasirinkite operacijas atkūrimui"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Pagrindinis"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Sąskaita faktūra"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Pastabos"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Išsiuntimo data"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Mokesčiai"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/nl.po` & `trytond_sale-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,18 +210,17 @@
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuur regels"
 
-#, fuzzy
 msgctxt "field:sale.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Factuur adres"
+msgstr "Factuur voortgang"
 
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mutaties"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -923,15 +922,15 @@
 msgstr "In behandeling"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
-"U kunt de relatie \"% (party) s\" niet verwijderen terwijl ze facturen in "
+"U kunt relatie \"%(party)s\" niet verwijderen terwijl ze verkopen in "
 "behandeling hebben bij bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_sale_customer_location_required"
 msgid ""
 "To process sale \"%(sale)s\" you must set a customer location on party "
 "\"%(party)s\"."
 msgstr ""
@@ -982,16 +981,16 @@
 "annuleren of terug zetten naar concept."
 
 msgctxt "model:ir.message,text:msg_sale_line_move_quantity"
 msgid ""
 "The sale line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
-"De verkoopregel \"%(line)s\" verplaatst naast het bestelde aantal %(aantal)s"
-" nog %(extra)s."
+"De verkoopregel \"%(line)s\" verplaatst naast het bestelde aantal "
+"%(quantity)s nog %(extra)s."
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
 msgid "A tax can be added only once to a sale line."
 msgstr ""
 "Een belasting kan slechts eenmaal aan een verkoop regel worden toegevoegd."
 
 msgctxt "model:ir.message,text:msg_sale_missing_account_revenue"
@@ -1585,18 +1584,26 @@
 msgstr "Kies mutatie om opnieuw aan te maken:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Algemeen"
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Facturering"
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notities"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Verzending"
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Belastingen"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Weet u zeker dat u deze verko(o)p(en) wilt retourneren?"
```

### Comparing `trytond_sale-7.2.0/locale/pl.po` & `trytond_sale-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1235,15 +1235,15 @@
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Products"
 msgstr "Produkt"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Raportowanie"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting_sale"
 msgid "Sales"
 msgstr "Sales"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_sale"
@@ -1651,18 +1651,28 @@
 msgid "Choose move to recreate:"
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Ogólne"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Faktura"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notatki"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Data wysyłki"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Podatki"
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/pt.po` & `trytond_sale-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1663,18 +1663,28 @@
 msgid "Choose move to recreate:"
 msgstr "Escolha as movimentações a recriar"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Geral"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Fatura"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Observação"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Data da Remessa"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Impostos"
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/ro.po` & `trytond_sale-7.2.1/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -1581,18 +1581,28 @@
 msgid "Choose move to recreate:"
 msgstr "Alegeți mișarea pentru a recrea:"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "General"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Factura fiscala"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Notițe"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Data de expediere"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Impozite"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr "Sunteți sigur că veți returna aceste vânzări /această vânzare?"
```

### Comparing `trytond_sale-7.2.0/locale/ru.po` & `trytond_sale-7.2.1/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -1668,18 +1668,28 @@
 msgid "Choose move to recreate:"
 msgstr "Выберите проводки для пересоздания"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Основной"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Инвойс"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Комментарии"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Состояние доставки"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Налоги"
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/sl.po` & `trytond_sale-7.2.1/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1651,18 +1651,28 @@
 msgid "Choose move to recreate:"
 msgstr "Izbor prometa za ponovno izdelavo"
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "Splošno"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Račun"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "Zapiski"
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr "Datum odpreme"
+
 msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr "Davki"
 
 #, fuzzy
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
```

### Comparing `trytond_sale-7.2.0/locale/tr.po` & `trytond_sale-7.2.1/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1622,19 +1622,28 @@
 msgid "Choose move to recreate:"
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/uk.po` & `trytond_sale-7.2.1/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -1539,18 +1539,26 @@
 msgstr ""
 
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/locale/zh_CN.po` & `trytond_sale-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -1641,18 +1641,27 @@
 #, fuzzy
 msgctxt "view:sale.line:"
 msgid "General"
 msgstr "基本"
 
 #, fuzzy
 msgctxt "view:sale.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
+#, fuzzy
+msgctxt "view:sale.line:"
 msgid "Notes"
 msgstr "注释"
 
 msgctxt "view:sale.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:sale.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:sale.return_sale.start:"
 msgid "Are you sure to return these/this sale(s)?"
 msgstr ""
```

### Comparing `trytond_sale-7.2.0/message.xml` & `trytond_sale-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/party.py` & `trytond_sale-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/party.xml` & `trytond_sale-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/product.py` & `trytond_sale-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/product.xml` & `trytond_sale-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/sale.fodt` & `trytond_sale-7.2.1/sale.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/sale.py` & `trytond_sale-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/sale.xml` & `trytond_sale-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/sale_reporting.py` & `trytond_sale-7.2.1/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/sale_reporting.xml` & `trytond_sale-7.2.1/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/setup.py` & `trytond_sale-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/stock.py` & `trytond_sale-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/stock.xml` & `trytond_sale-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale.rst` & `trytond_sale-7.2.1/tests/scenario_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_default_methods.rst` & `trytond_sale-7.2.1/tests/scenario_sale_default_methods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_default_taxes.rst` & `trytond_sale-7.2.1/tests/scenario_sale_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_empty.rst` & `trytond_sale-7.2.1/tests/scenario_sale_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_line_cancelled.rst` & `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_invoice.rst` & `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_shipment.rst` & `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_manual_invoice.rst` & `trytond_sale-7.2.1/tests/scenario_sale_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_manual_shipment.rst` & `trytond_sale-7.2.1/tests/scenario_sale_manual_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_modify_header.rst` & `trytond_sale-7.2.1/tests/scenario_sale_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/scenario_sale_reporting.rst` & `trytond_sale-7.2.1/tests/scenario_sale_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tests/test_module.py` & `trytond_sale-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/tox.ini` & `trytond_sale-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-7.2.1/trytond_sale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-7.2.0/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-7.2.1/trytond_sale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/configuration_form.xml` & `trytond_sale-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/party_form.xml` & `trytond_sale-7.2.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/product_list_sale_line.xml` & `trytond_sale-7.2.1/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/product_sale_context_form.xml` & `trytond_sale-7.2.1/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_form.xml` & `trytond_sale-7.2.1/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_line_form.xml` & `trytond_sale-7.2.1/view/sale_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_line_tree.xml` & `trytond_sale-7.2.1/view/sale_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_line_tree_sequence.xml` & `trytond_sale-7.2.1/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_reporting_context_form.xml` & `trytond_sale-7.2.1/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_reporting_customer_category_list.xml` & `trytond_sale-7.2.1/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_reporting_product_category_list.xml` & `trytond_sale-7.2.1/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/sale_tree.xml` & `trytond_sale-7.2.1/view/sale_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.0/view/template_form.xml` & `trytond_sale-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

