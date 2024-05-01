# Comparing `tmp/trytond_purchase-7.2.0.tar.gz` & `tmp/trytond_purchase-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-7.2.0.tar", last modified: Mon Apr 29 15:45:08 2024, max compression
+gzip compressed data, was "trytond_purchase-7.2.1.tar", last modified: Wed May  1 11:38:28 2024, max compression
```

## Comparing `trytond_purchase-7.2.0.tar` & `trytond_purchase-7.2.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     7140 2024-04-29 15:23:24.000000 trytond_purchase-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:23:23.000000 trytond_purchase-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3581 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2508 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:20.000000 trytond_purchase-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/prepurchase.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5036 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/returns.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5999 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1715 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37791 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37990 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32968 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38450 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38189 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32498 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34685 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39922 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32955 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38334 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37020 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33611 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36267 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37779 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35762 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38352 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34308 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36009 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38395 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38348 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37703 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32946 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31266 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36435 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4336 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3698 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1146 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20794 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    77247 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    87914 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31720 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11639 2024-03-17 11:01:36.000000 trytond_purchase-7.2.0/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23812 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8934 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4754 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.275385 trytond_purchase-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19177 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1678 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1285 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2509 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2448 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3040 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5169 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5595 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:20.000000 trytond_purchase-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-29 15:23:19.000000 trytond_purchase-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5171 2024-04-29 15:45:08.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3651 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      918 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2024-05-01 11:38:25.000000 trytond_purchase-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:38:25.000000 trytond_purchase-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2508 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.519714 trytond_purchase-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.519714 trytond_purchase-7.2.1/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/prepurchase.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5036 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.523047 trytond_purchase-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5999 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1715 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.523047 trytond_purchase-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37931 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38111 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33102 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38601 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38303 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32642 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34815 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40065 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33089 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38471 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37153 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33743 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36400 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37935 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35906 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38479 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34444 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36141 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38529 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38486 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37835 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33080 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31383 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36567 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4336 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3698 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1146 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    77247 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    87914 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31720 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11639 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23812 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8934 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4754 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.526380 trytond_purchase-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19177 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1678 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1285 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2509 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2448 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3040 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5169 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5595 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-30 17:21:06.000000 trytond_purchase-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5171 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3651 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      918 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/template_tree.xml
```

### Comparing `trytond_purchase-7.2.0/CHANGELOG` & `trytond_purchase-7.2.1/CHANGELOG`

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

### Comparing `trytond_purchase-7.2.0/COPYRIGHT` & `trytond_purchase-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/LICENSE` & `trytond_purchase-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/PKG-INFO` & `trytond_purchase-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.2.0/__init__.py` & `trytond_purchase-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/configuration.py` & `trytond_purchase-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/configuration.xml` & `trytond_purchase-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/doc/conf.py` & `trytond_purchase-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/doc/design.rst` & `trytond_purchase-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/doc/usage/prepurchase.inc.rst` & `trytond_purchase-7.2.1/doc/usage/prepurchase.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/doc/usage/process.inc.rst` & `trytond_purchase-7.2.1/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/doc/usage/returns.inc.rst` & `trytond_purchase-7.2.1/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/icons/LICENSE` & `trytond_purchase-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/invoice.py` & `trytond_purchase-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/invoice.xml` & `trytond_purchase-7.2.1/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/locale/bg.po` & `trytond_purchase-7.2.1/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -1458,19 +1458,28 @@
 msgid "Delivery Date:"
 msgstr "Дата на доставка"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Основен"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Фактура"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Бележки"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Данъци"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Друга информация"
```

### Comparing `trytond_purchase-7.2.0/locale/ca.po` & `trytond_purchase-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,17 @@
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
-#, fuzzy
 msgctxt "field:purchase.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Adreça de facturació"
+msgstr "Progrés de facturació"
 
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -809,15 +808,14 @@
 msgid "Done"
 msgstr "Finalitzada"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Pendent"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase unit of measure on which the purchase "
 "prices are based."
 msgstr ""
 "Esteu intentar modificar la unitat de mesura de compra en la que es basen "
 "els preus de compra."
@@ -859,16 +857,16 @@
 " esborrany la compra \"%(purchase)s\"."
 
 msgctxt "model:ir.message,text:msg_purchase_line_move_quantity"
 msgid ""
 "The purchase line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
-"La línia de compra \"%(line)s\" està movent %(extra)s més dels \"(quantity)s"
-" demanats."
+"La línia de compra \"%(line)s\" està movent %(extra)s a més dels "
+"%(quantity)s demanats."
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
 msgid "A tax can be added only once to a purchase line."
 msgstr "Un impost només es pot afegir una vegada a una línia de compra."
 
 msgctxt "model:ir.message,text:msg_purchase_missing_account_expense"
 msgid ""
@@ -1382,18 +1380,26 @@
 msgstr "Data lliurament:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Facturació"
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr "Enviament"
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Impostos"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Informació addicional"
```

### Comparing `trytond_purchase-7.2.0/locale/cs.po` & `trytond_purchase-7.2.1/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -315,18 +315,17 @@
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.product_supplier,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,party:"
 msgid "Supplier"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.product_supplier,prices:"
@@ -1416,19 +1415,28 @@
 msgid "Delivery Date:"
 msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
```

### Comparing `trytond_purchase-7.2.0/locale/de.po` & `trytond_purchase-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,17 @@
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
-#, fuzzy
 msgctxt "field:purchase.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Rechnungsadresse"
+msgstr "Rechnungsfortschritt"
 
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -814,22 +813,21 @@
 msgid "Done"
 msgstr "Erledigt"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Ausstehend"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase unit of measure on which the purchase "
 "prices are based."
 msgstr ""
-"Sie versuchen die Einkaufsmaßeinheit zu ändern, auf der die Einkaufspreise "
-"basieren."
+"Sie versuchen die Einkaufsmaßeinheit zu ändern, auf der die "
+"Lieferanteneinkaufspreise basieren."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
 "Partei \"%(party)s\" kann nicht gelöscht werden, solange noch unerledigte "
@@ -990,46 +988,46 @@
 
 msgctxt "model:ir.model.button,string:purchase_quote_button"
 msgid "Quote"
 msgstr "Anfrage"
 
 msgctxt "model:ir.rule.group,name:rule_group_product_supplier_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_companies"
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
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_product_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_supplier_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_supplier_time_series_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_purchase"
 msgid "Purchase"
 msgstr "Einkauf"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase"
 msgid "Purchase"
@@ -1388,18 +1386,26 @@
 msgstr "Lieferdatum:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Allgemein"
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Rechnungsfortschritt"
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notizen"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr "Lieferfortschritt"
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Steuern"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Sonstiges"
```

### Comparing `trytond_purchase-7.2.0/locale/es.po` & `trytond_purchase-7.2.1/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,17 @@
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
-#, fuzzy
 msgctxt "field:purchase.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Dirección de facturación"
+msgstr "Progreso de facturación"
 
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -812,15 +811,14 @@
 msgid "Done"
 msgstr "Finalizada"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Pendiente"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase unit of measure on which the purchase "
 "prices are based."
 msgstr ""
 "Está intentando modificar la unidad media de compra en la que se basan los "
 "precios de compra."
@@ -862,15 +860,15 @@
 "la compra \"%(purchase)s\"."
 
 msgctxt "model:ir.message,text:msg_purchase_line_move_quantity"
 msgid ""
 "The purchase line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
-"La línea de compra \"%(line)s\" esta movimiendo %(extra)s además de los "
+"La línea de compra \"%(line)s\" está moviendo %(extra)s además de los "
 "%(quantity)s pedidos."
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
 msgid "A tax can be added only once to a purchase line."
 msgstr "Un impuesto solo se puede agregar una vez a una línea de compra."
 
 msgctxt "model:ir.message,text:msg_purchase_missing_account_expense"
@@ -1385,18 +1383,26 @@
 msgstr "Fecha de entrega:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Facturación"
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notas"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr "Envío"
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Impuestos"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Información adicional"
```

### Comparing `trytond_purchase-7.2.0/locale/es_419.po` & `trytond_purchase-7.2.1/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -1382,19 +1382,28 @@
 msgid "Delivery Date:"
 msgstr "Fecha de entrega"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Líneas de factura"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
```

### Comparing `trytond_purchase-7.2.0/locale/et.po` & `trytond_purchase-7.2.1/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -1429,19 +1429,28 @@
 msgid "Delivery Date:"
 msgstr "Tarne kuupäev"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Üldine"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Arve"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Märkused"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Maksud"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Muu info"
```

### Comparing `trytond_purchase-7.2.0/locale/fa.po` & `trytond_purchase-7.2.1/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -1452,19 +1452,28 @@
 msgid "Delivery Date:"
 msgstr "تاریخ تحویل"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "عمومی"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "صورت حساب"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "یادداشت ها"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "مالیات ها"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "سایر اطلاعات"
```

### Comparing `trytond_purchase-7.2.0/locale/fi.po` & `trytond_purchase-7.2.1/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1192,15 +1192,14 @@
 msgid "Purchase"
 msgstr "Purchase"
 
 msgctxt "model:res.group,name:group_purchase_admin"
 msgid "Purchase Administrator"
 msgstr "Purchase Administrator"
 
-#, fuzzy
 msgctxt "report:purchase.purchase:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:purchase.purchase:"
 msgid "Amount"
 msgstr ""
@@ -1415,19 +1414,28 @@
 msgid "Delivery Date:"
 msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
```

### Comparing `trytond_purchase-7.2.0/locale/fr.po` & `trytond_purchase-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1383,18 +1383,26 @@
 msgstr "Date de livraison :"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Général"
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Facturation"
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notes"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr "Livraison"
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Taxes"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Autre information"
```

### Comparing `trytond_purchase-7.2.0/locale/hu.po` & `trytond_purchase-7.2.1/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -1418,19 +1418,28 @@
 msgid "Delivery Date:"
 msgstr "Leszállítás dátuma:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Általános"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Számla"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Jegyzetek"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Adók"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Egyéb info"
```

### Comparing `trytond_purchase-7.2.0/locale/id.po` & `trytond_purchase-7.2.1/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -1406,19 +1406,28 @@
 msgid "Delivery Date:"
 msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Umum"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Faktur"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Catatan-Catatan"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Pajak-Pajak"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Info Lain"
```

### Comparing `trytond_purchase-7.2.0/locale/it.po` & `trytond_purchase-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -1437,19 +1437,28 @@
 msgid "Delivery Date:"
 msgstr "Data di consegna:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Generale"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Fattura"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Note"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Imposte"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Altre informazioni"
```

### Comparing `trytond_purchase-7.2.0/locale/lo.po` & `trytond_purchase-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -1502,17 +1502,26 @@
 #, fuzzy
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "ທົ່ວໄປ"
 
 #, fuzzy
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "ໃບເກັບເງິນ"
+
+#, fuzzy
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "ໝາຍເຫດ"
 
+msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
 #, fuzzy
 msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "ອາກອນ"
 
 #, fuzzy
 msgctxt "view:purchase.purchase:"
```

### Comparing `trytond_purchase-7.2.0/locale/lt.po` & `trytond_purchase-7.2.1/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1433,19 +1433,28 @@
 msgid "Delivery Date:"
 msgstr "Pristatymo data"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Pagrindinis"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Sąskaita faktūra"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Pastabos"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Mokesčiai"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Kita informacija"
```

### Comparing `trytond_purchase-7.2.0/locale/nl.po` & `trytond_purchase-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,17 @@
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuurregels"
 
-#, fuzzy
 msgctxt "field:purchase.line,invoice_progress:"
 msgid "Invoice Progress"
-msgstr "Factuuradres"
+msgstr "Factuur voortgang"
 
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Voorraad bewegingen"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -814,15 +813,14 @@
 msgid "Done"
 msgstr "Afgerond"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "In behandeling"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
 "You are trying to change the purchase unit of measure on which the purchase "
 "prices are based."
 msgstr ""
 "U probeert de inkoop maateenheid waarop de inkoopprijzen zijn gebaseerd te "
 "wijzigen."
@@ -864,16 +862,16 @@
 " annuleren, resetten of terugzetten naar concept."
 
 msgctxt "model:ir.message,text:msg_purchase_line_move_quantity"
 msgid ""
 "The purchase line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
-"De inkoopregel \"%(line)s\" verplaatst naast het bestelde aantal %(aantal)s "
-"nog %(extra)s."
+"De inkoopregel \"%(line)s\" verplaatst naast het bestelde aantal "
+"%(quantity)s nog %(extra)s."
 
 msgctxt "model:ir.message,text:msg_purchase_line_tax_unique"
 msgid "A tax can be added only once to a purchase line."
 msgstr ""
 "Een belasting kan slechts één keer worden toegevoegd aan een inkoopregel."
 
 msgctxt "model:ir.message,text:msg_purchase_missing_account_expense"
@@ -1388,18 +1386,26 @@
 msgstr "Leverdatum:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Algemeen"
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Facturering"
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notities"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr "Verzending"
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Belastingen"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Overige informatie"
```

### Comparing `trytond_purchase-7.2.0/locale/pl.po` & `trytond_purchase-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -1092,15 +1092,15 @@
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_form"
 msgid "Purchases"
 msgstr "Purchases"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Raportowanie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_purchase"
 msgid "Purchases"
 msgstr "Zakupy"
 
 #, fuzzy
@@ -1446,19 +1446,28 @@
 msgid "Delivery Date:"
 msgstr "Data dostawy"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Ogólne"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Faktura"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notatki"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Podatki"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Inne informacje"
```

### Comparing `trytond_purchase-7.2.0/locale/pt.po` & `trytond_purchase-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -1457,19 +1457,28 @@
 msgid "Delivery Date:"
 msgstr "Data de entrega"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Geral"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Fatura"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Observações"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Impostos"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Outras Informações"
```

### Comparing `trytond_purchase-7.2.0/locale/ro.po` & `trytond_purchase-7.2.1/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -1414,19 +1414,28 @@
 msgid "Delivery Date:"
 msgstr "Data de livrare:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "General"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Factură"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Notiţe"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Taxe"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Alte Informații"
```

### Comparing `trytond_purchase-7.2.0/locale/ru.po` & `trytond_purchase-7.2.1/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -1463,19 +1463,28 @@
 msgid "Delivery Date:"
 msgstr "Дата доставки"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Основной"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Инвойс"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Комментарии"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Налоги"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Другая информация"
```

### Comparing `trytond_purchase-7.2.0/locale/sl.po` & `trytond_purchase-7.2.1/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -1393,19 +1393,28 @@
 msgid "Delivery Date:"
 msgstr "Datum dostave:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "Splošno"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Račun"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "Zapiski"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "Davki"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "Drugo"
```

### Comparing `trytond_purchase-7.2.0/locale/tr.po` & `trytond_purchase-7.2.1/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,18 @@
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.product_supplier,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:purchase.product_supplier,party:"
 msgid "Supplier"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.product_supplier,prices:"
@@ -1192,14 +1193,15 @@
 msgid "Purchase"
 msgstr "Purchase"
 
 msgctxt "model:res.group,name:group_purchase_admin"
 msgid "Purchase Administrator"
 msgstr "Purchase Administrator"
 
+#, fuzzy
 msgctxt "report:purchase.purchase:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:purchase.purchase:"
 msgid "Amount"
 msgstr ""
@@ -1414,19 +1416,28 @@
 msgid "Delivery Date:"
 msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr ""
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "Invoices"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
```

### Comparing `trytond_purchase-7.2.0/locale/uk.po` & `trytond_purchase-7.2.1/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -1352,18 +1352,26 @@
 msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr ""
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
```

### Comparing `trytond_purchase-7.2.0/locale/zh_CN.po` & `trytond_purchase-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -1356,19 +1356,28 @@
 msgid "Delivery Date:"
 msgstr "交货日期:"
 
 msgctxt "view:purchase.line:"
 msgid "General"
 msgstr "基本情况"
 
+#, fuzzy
+msgctxt "view:purchase.line:"
+msgid "Invoicing"
+msgstr "发票"
+
 msgctxt "view:purchase.line:"
 msgid "Notes"
 msgstr "备注"
 
 msgctxt "view:purchase.line:"
+msgid "Shipping"
+msgstr ""
+
+msgctxt "view:purchase.line:"
 msgid "Taxes"
 msgstr "税"
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr "其它信息"
```

### Comparing `trytond_purchase-7.2.0/message.xml` & `trytond_purchase-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/party.py` & `trytond_purchase-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/party.xml` & `trytond_purchase-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/product.py` & `trytond_purchase-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/product.xml` & `trytond_purchase-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/purchase.fodt` & `trytond_purchase-7.2.1/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/purchase.py` & `trytond_purchase-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/purchase.xml` & `trytond_purchase-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/purchase_reporting.py` & `trytond_purchase-7.2.1/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/purchase_reporting.xml` & `trytond_purchase-7.2.1/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/setup.py` & `trytond_purchase-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/stock.py` & `trytond_purchase-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/stock.xml` & `trytond_purchase-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_default_taxes.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_empty.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled_on_shipment.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled_on_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_manual_invoice.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_reporting.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-7.2.1/tests/scenario_purchase_return_wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tests/test_module.py` & `trytond_purchase-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/tox.ini` & `trytond_purchase-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-7.2.1/trytond_purchase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.2.0/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-7.2.1/trytond_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/party_form.xml` & `trytond_purchase-7.2.1/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/product_supplier_form.xml` & `trytond_purchase-7.2.1/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_form.xml` & `trytond_purchase-7.2.1/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_line_form.xml` & `trytond_purchase-7.2.1/view/purchase_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_line_tree.xml` & `trytond_purchase-7.2.1/view/purchase_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_line_tree_sequence.xml` & `trytond_purchase-7.2.1/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_reporting_context_form.xml` & `trytond_purchase-7.2.1/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/purchase_tree.xml` & `trytond_purchase-7.2.1/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.0/view/template_form.xml` & `trytond_purchase-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

