# Comparing `tmp/trytond_account_stock_shipment_cost-7.2.0.tar.gz` & `tmp/trytond_account_stock_shipment_cost-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_shipment_cost-7.2.0.tar", last modified: Mon Apr 29 15:36:57 2024, max compression
+gzip compressed data, was "trytond_account_stock_shipment_cost-7.2.1.tar", last modified: Wed May  1 12:11:41 2024, max compression
```

## Comparing `trytond_account_stock_shipment_cost-7.2.0.tar` & `trytond_account_stock_shipment_cost-7.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2024-04-29 15:17:00.000000 trytond_account_stock_shipment_cost-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:16:59.000000 trytond_account_stock_shipment_cost-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15600 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9364 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7039 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7192 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5878 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6857 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5887 2024-04-29 13:17:17.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5879 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4809 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      709 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7193 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/tests/scenario_account_stock_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-29 15:16:54.000000 trytond_account_stock_shipment_cost-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-04-29 15:36:57.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_show_shipment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2024-05-01 12:11:37.000000 trytond_account_stock_shipment_cost-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:11:37.000000 trytond_account_stock_shipment_cost-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15600 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9364 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.154265 trytond_account_stock_shipment_cost-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7039 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-30 17:21:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7192 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5878 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6857 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5887 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5879 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4809 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      709 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7193 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/tests/scenario_account_stock_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-30 17:21:06.000000 trytond_account_stock_shipment_cost-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-05-01 12:11:41.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:11:40.000000 trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:11:41.157598 trytond_account_stock_shipment_cost-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/shipment_cost_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/shipment_cost_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/shipment_cost_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/shipment_cost_show_shipment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_account_stock_shipment_cost-7.2.1/view/template_form.xml
```

### Comparing `trytond_account_stock_shipment_cost-7.2.0/CHANGELOG` & `trytond_account_stock_shipment_cost-7.2.1/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_account_stock_shipment_cost-7.2.0/COPYRIGHT` & `trytond_account_stock_shipment_cost-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/LICENSE` & `trytond_account_stock_shipment_cost-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/PKG-INFO` & `trytond_account_stock_shipment_cost-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_shipment_cost
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_shipment_cost-7.2.0/__init__.py` & `trytond_account_stock_shipment_cost-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/account.py` & `trytond_account_stock_shipment_cost-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/account.xml` & `trytond_account_stock_shipment_cost-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/doc/conf.py` & `trytond_account_stock_shipment_cost-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/doc/design.rst` & `trytond_account_stock_shipment_cost-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/bg.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/ca.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/cs.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/de.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
 msgctxt "model:ir.model.button,string:shipment_cost_show_button"
 msgid "Show"
 msgstr "Anzeigen"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_cost_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_shipment_cost"
 msgid "Shipment Cost"
 msgstr "Lieferkosten"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_shipment_cost"
 msgid "Shipment Cost"
```

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/es.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/es_419.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/et.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/fa.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/fi.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/fr.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/hu.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/id.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/it.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/lo.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/lt.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/nl.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/pl.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/pt.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/ro.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/ru.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/sl.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/tr.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/uk.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/locale/zh_CN.po` & `trytond_account_stock_shipment_cost-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/message.xml` & `trytond_account_stock_shipment_cost-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/product.py` & `trytond_account_stock_shipment_cost-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/setup.py` & `trytond_account_stock_shipment_cost-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/stock.py` & `trytond_account_stock_shipment_cost-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/tests/scenario_account_stock_shipment_cost.rst` & `trytond_account_stock_shipment_cost-7.2.1/tests/scenario_account_stock_shipment_cost.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/tox.ini` & `trytond_account_stock_shipment_cost-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO` & `trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_shipment_cost
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt` & `trytond_account_stock_shipment_cost-7.2.1/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_form.xml` & `trytond_account_stock_shipment_cost-7.2.1/view/shipment_cost_form.xml`

 * *Files identical despite different names*

