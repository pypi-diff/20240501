# Comparing `tmp/trytond_account_asset-7.2.0.tar.gz` & `tmp/trytond_account_asset-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_asset-7.2.0.tar", last modified: Mon Apr 29 15:31:37 2024, max compression
+gzip compressed data, was "trytond_account_asset-7.2.1.tar", last modified: Wed May  1 12:25:13 2024, max compression
```

## Comparing `trytond_account_asset-7.2.0.tar` & `trytond_account_asset-7.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2024-04-29 15:12:43.000000 trytond_account_asset-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:12:43.000000 trytond_account_asset-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1351 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7220 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    43075 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/asset.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11392 2024-04-27 16:30:39.000000 trytond_account_asset-7.2.0/asset.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    61964 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/asset_table.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.363261 trytond_account_asset-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_account_asset-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account_asset-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.366594 trytond_account_asset-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    19721 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20940 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21368 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21049 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19616 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20298 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22250 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21098 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18853 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18548 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19852 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23118 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18567 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20824 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18955 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20787 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20474 2024-04-29 13:17:17.000000 trytond_account_asset-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19780 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19968 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19753 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17526 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18533 2024-04-27 16:43:20.000000 trytond_account_asset-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3101 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1766 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1751 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3519 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1111 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2024-03-17 11:01:36.000000 trytond_account_asset-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.366594 trytond_account_asset-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8424 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_account_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4517 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_account_asset_depreciated.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3701 2024-04-22 12:14:36.000000 trytond_account_asset-7.2.0/tests/scenario_purchase_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1645 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-01-27 09:58:52.000000 trytond_account_asset-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account_asset-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-29 15:12:39.000000 trytond_account_asset-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2024-04-29 15:31:37.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:36.000000 trytond_account_asset-7.2.0/trytond_account_asset.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:37.369927 trytond_account_asset-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_create_moves_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2342 2024-02-04 18:51:26.000000 trytond_account_asset-7.2.0/view/asset_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/asset_update_show_depreciation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/asset_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/print_depreciation_table_start.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:14.000000 trytond_account_asset-7.2.0/view/revision_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:20.000000 trytond_account_asset-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2630 2024-05-01 12:25:09.000000 trytond_account_asset-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-05-01 12:25:09.000000 trytond_account_asset-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7220 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1065 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    43075 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/asset.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11392 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/asset.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    61964 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/asset_table.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.193511 trytond_account_asset-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.193511 trytond_account_asset-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19721 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20940 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21357 2024-04-30 17:21:59.000000 trytond_account_asset-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21049 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19616 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20298 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22250 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21098 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18853 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18548 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19852 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23118 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18567 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20823 2024-04-30 17:21:59.000000 trytond_account_asset-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18955 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20787 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20474 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19780 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19968 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19753 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17526 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18533 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3101 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1766 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3519 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1111 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4505 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8424 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/scenario_account_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4517 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/scenario_account_asset_depreciated.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3701 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/scenario_purchase_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1645 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:21:06.000000 trytond_account_asset-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3611 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2024-05-01 12:25:13.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:25:12.000000 trytond_account_asset-7.2.1/trytond_account_asset.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:25:13.196844 trytond_account_asset-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_create_moves_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2342 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      532 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      617 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_update_show_depreciation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/asset_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/print_depreciation_table_start.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/revision_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:20:59.000000 trytond_account_asset-7.2.1/view/template_form.xml
```

### Comparing `trytond_account_asset-7.2.0/CHANGELOG` & `trytond_account_asset-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_asset-7.2.0/COPYRIGHT` & `trytond_account_asset-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/LICENSE` & `trytond_account_asset-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/PKG-INFO` & `trytond_account_asset-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_asset
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for assets management
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_asset-7.2.0/README.rst` & `trytond_account_asset-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/__init__.py` & `trytond_account_asset-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/account.py` & `trytond_account_asset-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/account.xml` & `trytond_account_asset-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/asset.py` & `trytond_account_asset-7.2.1/asset.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/asset.xml` & `trytond_account_asset-7.2.1/asset.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/asset_table.fodt` & `trytond_account_asset-7.2.1/asset_table.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/doc/conf.py` & `trytond_account_asset-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/doc/index.rst` & `trytond_account_asset-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/invoice.py` & `trytond_account_asset-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/bg.po` & `trytond_account_asset-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/ca.po` & `trytond_account_asset-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/cs.po` & `trytond_account_asset-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/de.po` & `trytond_account_asset-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 msgctxt "field:account.configuration,asset_bymonthday:"
 msgid "Day of the Month"
 msgstr "Tag des Monats"
 
 msgctxt "field:account.configuration,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr "Abschreibungsbuchungsfrequenz"
+msgstr "Abschreibungsintervall"
 
 msgctxt "field:account.configuration,asset_sequence:"
 msgid "Asset Reference Sequence"
 msgstr "Nummernkreis Anlage"
 
 msgctxt "field:account.configuration.asset_date,asset_bymonth:"
 msgid "Month"
@@ -240,15 +240,15 @@
 
 msgctxt "field:account.configuration.asset_date,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.configuration.asset_frequency,asset_frequency:"
 msgid "Asset Depreciation Frequency"
-msgstr "Abschreibungsbuchungsfrequenz"
+msgstr "Abschreibungsintervall"
 
 msgctxt "field:account.configuration.asset_frequency,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:account.configuration.asset_sequence,asset_sequence:"
 msgid "Asset Reference Sequence"
@@ -272,19 +272,19 @@
 
 msgctxt "field:product.category,account_depreciation:"
 msgid "Account Depreciation"
 msgstr "Abschreibungskonto"
 
 msgctxt "field:product.category.account,account_asset:"
 msgid "Account Asset"
-msgstr "Anlagenkonto"
+msgstr "Bilanzkonto Sachanlagen"
 
 msgctxt "field:product.category.account,account_depreciation:"
 msgid "Account Depreciation"
-msgstr "Abschreibungskonto"
+msgstr "Bilanzkonto Abschreibungen"
 
 msgctxt "field:product.product,depreciable:"
 msgid "Depreciable"
 msgstr "Abschreibungsfähig"
 
 msgctxt "field:product.product,depreciation_duration:"
 msgid "Depreciation Duration"
@@ -407,15 +407,15 @@
 
 msgctxt "model:ir.action,name:wizard_create_moves"
 msgid "Create Assets Moves"
 msgstr "Buchungssätze für Abschreibungen erstellen"
 
 msgctxt "model:ir.action,name:wizard_print_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr "Entwicklung des Anlagevermögens drucken"
+msgstr "Entwicklung des Anlagevermögens"
 
 msgctxt "model:ir.action,name:wizard_update"
 msgid "Update Asset"
 msgstr "Anlage aktualisieren"
 
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_all"
 msgid "All"
@@ -501,15 +501,15 @@
 
 msgctxt "model:ir.model.button,string:asset_update_button"
 msgid "Update Asset"
 msgstr "Anlage aktualisieren"
 
 msgctxt "model:ir.rule.group,name:rule_group_asset_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_asset"
 msgid "Asset"
 msgstr "Anlage"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_asset"
 msgid "Asset"
@@ -521,15 +521,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_asset_form"
 msgid "Assets"
 msgstr "Anlagen"
 
 msgctxt "model:ir.ui.menu,name:menu_create_depreciation_table"
 msgid "Print Depreciation Table"
-msgstr "Entwicklung des Anlagevermögens drucken"
+msgstr "Entwicklung des Anlagevermögens"
 
 msgctxt "model:ir.ui.menu,name:menu_create_moves"
 msgid "Create Assets Moves"
 msgstr "Abschreibungsbuchungssätze erstellen"
 
 msgctxt "report:account.asset.depreciation_table:"
 msgid "("
```

### Comparing `trytond_account_asset-7.2.0/locale/es.po` & `trytond_account_asset-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/es_419.po` & `trytond_account_asset-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/et.po` & `trytond_account_asset-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/fa.po` & `trytond_account_asset-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/fi.po` & `trytond_account_asset-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/fr.po` & `trytond_account_asset-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/hu.po` & `trytond_account_asset-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/id.po` & `trytond_account_asset-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/it.po` & `trytond_account_asset-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/lo.po` & `trytond_account_asset-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/lt.po` & `trytond_account_asset-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/nl.po` & `trytond_account_asset-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
 msgctxt "model:ir.action.act_window.domain,name:act_asset_form_domain_running"
 msgid "Running"
 msgstr "In uitvoering"
 
 msgctxt "model:ir.message,text:msg_asset_delete_draft"
 msgid "You cannot delete asset \"%(asset)s\" because it is not in \"draft\" state."
 msgstr ""
-"U kunt activa \"% (asset)s\" niet verwijderen omdat het niet in status "
+"U kunt activa \"%(asset)s\" niet verwijderen omdat het niet in status "
 "\"concept\" staat."
 
 msgctxt "model:ir.message,text:msg_asset_draft_lines"
 msgid "You cannot reset to draft asset \"%(asset)s\" because it has lines."
 msgstr ""
 "U kunt activa \"%(asset)s\" niet terugzetten naar concept omdat het regels "
 "heeft."
```

### Comparing `trytond_account_asset-7.2.0/locale/pl.po` & `trytond_account_asset-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/pt.po` & `trytond_account_asset-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/ro.po` & `trytond_account_asset-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/ru.po` & `trytond_account_asset-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/sl.po` & `trytond_account_asset-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/tr.po` & `trytond_account_asset-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/uk.po` & `trytond_account_asset-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/locale/zh_CN.po` & `trytond_account_asset-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/message.xml` & `trytond_account_asset-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart.xml` & `trytond_account_asset-7.2.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_bg.xml` & `trytond_account_asset-7.2.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_ca.xml` & `trytond_account_asset-7.2.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_de.xml` & `trytond_account_asset-7.2.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_en.xml` & `trytond_account_asset-7.2.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_es.xml` & `trytond_account_asset-7.2.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_fr.xml` & `trytond_account_asset-7.2.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_nl.xml` & `trytond_account_asset-7.2.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_pt.xml` & `trytond_account_asset-7.2.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_ru.xml` & `trytond_account_asset-7.2.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/minimal_chart_sl.xml` & `trytond_account_asset-7.2.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/product.py` & `trytond_account_asset-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/product.xml` & `trytond_account_asset-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/purchase.py` & `trytond_account_asset-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/setup.py` & `trytond_account_asset-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tests/scenario_account_asset.rst` & `trytond_account_asset-7.2.1/tests/scenario_account_asset.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tests/scenario_account_asset_depreciated.rst` & `trytond_account_asset-7.2.1/tests/scenario_account_asset_depreciated.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tests/scenario_purchase_asset.rst` & `trytond_account_asset-7.2.1/tests/scenario_purchase_asset.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tests/test_module.py` & `trytond_account_asset-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tests/tools.py` & `trytond_account_asset-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/tox.ini` & `trytond_account_asset-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/trytond_account_asset.egg-info/PKG-INFO` & `trytond_account_asset-7.2.1/trytond_account_asset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_asset
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for assets management
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_asset-7.2.0/trytond_account_asset.egg-info/SOURCES.txt` & `trytond_account_asset-7.2.1/trytond_account_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/asset_form.xml` & `trytond_account_asset-7.2.1/view/asset_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/asset_line_form.xml` & `trytond_account_asset-7.2.1/view/asset_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/asset_tree.xml` & `trytond_account_asset-7.2.1/view/asset_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/asset_update_show_depreciation_form.xml` & `trytond_account_asset-7.2.1/view/asset_update_show_depreciation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/asset_update_start_form.xml` & `trytond_account_asset-7.2.1/view/asset_update_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/configuration_form.xml` & `trytond_account_asset-7.2.1/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-7.2.0/view/template_form.xml` & `trytond_account_asset-7.2.1/view/template_form.xml`

 * *Files identical despite different names*

