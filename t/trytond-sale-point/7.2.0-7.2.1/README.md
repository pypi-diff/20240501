# Comparing `tmp/trytond_sale_point-7.2.0.tar.gz` & `tmp/trytond_sale_point-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_point-7.2.0.tar", last modified: Mon Apr 29 15:48:34 2024, max compression
+gzip compressed data, was "trytond_sale_point-7.2.1.tar", last modified: Wed May  1 11:20:26 2024, max compression
```

## Comparing `trytond_sale_point-7.2.0.tar` & `trytond_sale_point-7.2.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-29 15:25:42.000000 trytond_sale_point-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:25:42.000000 trytond_sale_point-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.273331 trytond_sale_point-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_point-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-09-24 17:12:47.000000 trytond_sale_point-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.276664 trytond_sale_point-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17180 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17599 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17213 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17447 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14481 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14168 2024-04-29 13:17:17.000000 trytond_sale_point-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17048 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14071 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14063 2024-04-27 16:43:26.000000 trytond_sale_point-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45634 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24271 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2024-03-17 11:01:36.000000 trytond_sale_point-7.2.0/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:30:39.000000 trytond_sale_point-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.276664 trytond_sale_point-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5830 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3643 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4447 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4928 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_session.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3900 2024-04-22 12:14:36.000000 trytond_sale_point-7.2.0/tests/scenario_sale_point_tax_excluded.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_point-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-29 15:25:38.000000 trytond_sale_point-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2919 2024-04-29 15:48:34.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:33.000000 trytond_sale_point-7.2.0/trytond_sale_point.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:34.279997 trytond_sale_point-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_session_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_session_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/view/cash_transfer_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/cash_transfer_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_form_wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/payment_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-02-04 18:51:26.000000 trytond_sale_point-7.2.0/view/point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-09-24 17:12:47.000000 trytond_sale_point-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/sale_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_sale_point-7.2.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.304335 trytond_sale_point-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      889 2024-05-01 11:20:23.000000 trytond_sale_point-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:20:23.000000 trytond_sale_point-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-05-01 11:20:26.304335 trytond_sale_point-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.297665 trytond_sale_point-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4049 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.301000 trytond_sale_point-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17180 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17599 2024-04-30 17:21:59.000000 trytond_sale_point-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17210 2024-04-30 17:21:59.000000 trytond_sale_point-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17447 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14481 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14168 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17048 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14071 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14042 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14063 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1870 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45634 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24271 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:20:26.304335 trytond_sale_point-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4575 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.301000 trytond_sale_point-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5830 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/scenario_sale_point.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3643 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/scenario_sale_point_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4447 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/scenario_sale_point_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4928 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/scenario_sale_point_session.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3900 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/scenario_sale_point_tax_excluded.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-30 17:21:06.000000 trytond_sale_point-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.304335 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2919 2024-05-01 11:20:26.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:20:25.000000 trytond_sale_point-7.2.1/trytond_sale_point.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:26.304335 trytond_sale_point-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_session_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_session_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_transfer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_transfer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_transfer_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/cash_transfer_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/payment_form_wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      276 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/payment_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      799 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1878 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/sale_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/sale_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:21:00.000000 trytond_sale_point-7.2.1/view/template_tree.xml
```

### Comparing `trytond_sale_point-7.2.0/CHANGELOG` & `trytond_sale_point-7.2.1/CHANGELOG`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_sale_point-7.2.0/COPYRIGHT` & `trytond_sale_point-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/LICENSE` & `trytond_sale_point-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/PKG-INFO` & `trytond_sale_point-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_point
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_point-7.2.0/__init__.py` & `trytond_sale_point-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/account.py` & `trytond_sale_point-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/doc/conf.py` & `trytond_sale_point-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/doc/design.rst` & `trytond_sale_point-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/bg.po` & `trytond_sale_point-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/ca.po` & `trytond_sale_point-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/cs.po` & `trytond_sale_point-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/de.po` & `trytond_sale_point-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -523,35 +523,35 @@
 
 msgctxt "model:ir.model.button,string:sale_process_button"
 msgid "Process"
 msgstr "Ausführen"
 
 msgctxt "model:ir.rule.group,name:rule_group_cash_session_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_cash_transfer_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_cash_transfer_type_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_method_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_point_sale_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sale_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_sale"
 msgid "POS"
 msgstr "Point of Sale"
 
 msgctxt "model:ir.ui.menu,name:menu_cash_session_form"
 msgid "POS Cash Sessions"
```

### Comparing `trytond_sale_point-7.2.0/locale/es.po` & `trytond_sale_point-7.2.1/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 msgctxt "field:sale.point,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:sale.point,customer_location:"
 msgid "To Location"
-msgstr "A la ubicación"
+msgstr "A ubicación"
 
 msgctxt "field:sale.point,journal:"
 msgid "Journal"
 msgstr "Diario"
 
 msgctxt "field:sale.point,name:"
 msgid "Name"
```

### Comparing `trytond_sale_point-7.2.0/locale/es_419.po` & `trytond_sale_point-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/et.po` & `trytond_sale_point-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/fa.po` & `trytond_sale_point-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/fi.po` & `trytond_sale_point-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/fr.po` & `trytond_sale_point-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/hu.po` & `trytond_sale_point-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/id.po` & `trytond_sale_point-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/it.po` & `trytond_sale_point-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/lo.po` & `trytond_sale_point-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/lt.po` & `trytond_sale_point-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/nl.po` & `trytond_sale_point-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/pl.po` & `trytond_sale_point-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/pt.po` & `trytond_sale_point-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/ro.po` & `trytond_sale_point-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/ru.po` & `trytond_sale_point-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/sl.po` & `trytond_sale_point-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/tr.po` & `trytond_sale_point-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/uk.po` & `trytond_sale_point-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/locale/zh_CN.po` & `trytond_sale_point-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/message.xml` & `trytond_sale_point-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/product.py` & `trytond_sale_point-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/product.xml` & `trytond_sale_point-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/sale.py` & `trytond_sale_point-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/sale.xml` & `trytond_sale_point-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/sale_reporting.py` & `trytond_sale_point-7.2.1/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/setup.py` & `trytond_sale_point-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tests/scenario_sale_point.rst` & `trytond_sale_point-7.2.1/tests/scenario_sale_point.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tests/scenario_sale_point_reporting.rst` & `trytond_sale_point-7.2.1/tests/scenario_sale_point_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tests/scenario_sale_point_return.rst` & `trytond_sale_point-7.2.1/tests/scenario_sale_point_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tests/scenario_sale_point_session.rst` & `trytond_sale_point-7.2.1/tests/scenario_sale_point_session.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tests/scenario_sale_point_tax_excluded.rst` & `trytond_sale_point-7.2.1/tests/scenario_sale_point_tax_excluded.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/tox.ini` & `trytond_sale_point-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/trytond_sale_point.egg-info/PKG-INFO` & `trytond_sale_point-7.2.1/trytond_sale_point.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_point
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_point-7.2.0/trytond_sale_point.egg-info/SOURCES.txt` & `trytond_sale_point-7.2.1/trytond_sale_point.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/view/cash_session_form.xml` & `trytond_sale_point-7.2.1/view/cash_session_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/view/cash_transfer_form.xml` & `trytond_sale_point-7.2.1/view/cash_transfer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/view/point_form.xml` & `trytond_sale_point-7.2.1/view/point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/view/sale_form.xml` & `trytond_sale_point-7.2.1/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-7.2.0/view/sale_line_form.xml` & `trytond_sale_point-7.2.1/view/sale_line_form.xml`

 * *Files identical despite different names*

