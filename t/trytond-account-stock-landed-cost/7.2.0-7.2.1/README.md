# Comparing `tmp/trytond_account_stock_landed_cost-7.2.0.tar.gz` & `tmp/trytond_account_stock_landed_cost-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_landed_cost-7.2.0.tar", last modified: Mon Apr 29 15:36:44 2024, max compression
+gzip compressed data, was "trytond_account_stock_landed_cost-7.2.1.tar", last modified: Wed May  1 12:12:10 2024, max compression
```

## Comparing `trytond_account_stock_landed_cost-7.2.0.tar` & `trytond_account_stock_landed_cost-7.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.988548 trytond_account_stock_landed_cost-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-29 15:16:47.000000 trytond_account_stock_landed_cost-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:16:46.000000 trytond_account_stock_landed_cost-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3468 2024-04-29 15:36:44.988548 trytond_account_stock_landed_cost-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19670 2024-01-27 09:58:52.000000 trytond_account_stock_landed_cost-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8761 2024-04-27 16:30:39.000000 trytond_account_stock_landed_cost-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.985215 trytond_account_stock_landed_cost-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_stock_landed_cost-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:01.000000 trytond_account_stock_landed_cost-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.985215 trytond_account_stock_landed_cost-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6516 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7044 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7007 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7101 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6263 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6610 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6658 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7255 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6744 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6551 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6582 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6259 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6811 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6280 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6631 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5811 2024-04-29 13:17:17.000000 trytond_account_stock_landed_cost-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6505 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6444 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5778 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6248 2024-04-27 16:43:22.000000 trytond_account_stock_landed_cost-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:44.988548 trytond_account_stock_landed_cost-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4515 2024-03-17 11:01:36.000000 trytond_account_stock_landed_cost-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1158 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.985215 trytond_account_stock_landed_cost-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6991 2024-04-22 12:14:36.000000 trytond_account_stock_landed_cost-7.2.0/tests/scenario_account_stock_landed_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:01.000000 trytond_account_stock_landed_cost-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-29 15:16:41.000000 trytond_account_stock_landed_cost-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.988548 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3468 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:44.000000 trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:44.988548 trytond_account_stock_landed_cost-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/view/landed_cost_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/view/landed_cost_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/view/landed_cost_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/view/landed_cost_show_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-7.2.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2085 2024-05-01 12:12:07.000000 trytond_account_stock_landed_cost-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:12:07.000000 trytond_account_stock_landed_cost-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3468 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      846 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19670 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8761 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.976325 trytond_account_stock_landed_cost-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6516 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7044 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7007 2024-04-30 17:21:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7101 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6263 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6610 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6658 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7255 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6744 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6551 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6582 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6259 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6810 2024-04-30 17:21:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6280 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6631 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5811 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6505 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6444 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5778 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6248 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      824 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4515 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1158 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6991 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/tests/scenario_account_stock_landed_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:06.000000 trytond_account_stock_landed_cost-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3468 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:12:10.000000 trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:10.979660 trytond_account_stock_landed_cost-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/landed_cost_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/landed_cost_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/landed_cost_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/landed_cost_show_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:20:59.000000 trytond_account_stock_landed_cost-7.2.1/view/template_form.xml
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/CHANGELOG` & `trytond_account_stock_landed_cost-7.2.1/CHANGELOG`

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
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/COPYRIGHT` & `trytond_account_stock_landed_cost-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/LICENSE` & `trytond_account_stock_landed_cost-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/PKG-INFO` & `trytond_account_stock_landed_cost-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_landed_cost
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for landed cost
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/README.rst` & `trytond_account_stock_landed_cost-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/__init__.py` & `trytond_account_stock_landed_cost-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/account.py` & `trytond_account_stock_landed_cost-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/account.xml` & `trytond_account_stock_landed_cost-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/doc/conf.py` & `trytond_account_stock_landed_cost-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/doc/index.rst` & `trytond_account_stock_landed_cost-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/bg.po` & `trytond_account_stock_landed_cost-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/ca.po` & `trytond_account_stock_landed_cost-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/cs.po` & `trytond_account_stock_landed_cost-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/de.po` & `trytond_account_stock_landed_cost-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
 msgctxt "model:ir.model.button,string:landed_cost_show_button"
 msgid "Show"
 msgstr "Anzeigen"
 
 msgctxt "model:ir.rule.group,name:rule_group_landed_cost_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_landed_cost"
 msgid "Landed Cost"
 msgstr "Einstandskosten"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_landed_cost"
 msgid "Landed Cost"
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/es.po` & `trytond_account_stock_landed_cost-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/es_419.po` & `trytond_account_stock_landed_cost-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/et.po` & `trytond_account_stock_landed_cost-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/fa.po` & `trytond_account_stock_landed_cost-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/fi.po` & `trytond_account_stock_landed_cost-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/fr.po` & `trytond_account_stock_landed_cost-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/hu.po` & `trytond_account_stock_landed_cost-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/id.po` & `trytond_account_stock_landed_cost-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/it.po` & `trytond_account_stock_landed_cost-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/lo.po` & `trytond_account_stock_landed_cost-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/lt.po` & `trytond_account_stock_landed_cost-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/nl.po` & `trytond_account_stock_landed_cost-7.2.1/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 msgstr ""
 "De categorie \"%(category)s\"op landed cost \"%(landed_cost)s\" is niet "
 "gebruikt."
 
 msgctxt "model:ir.message,text:msg_landed_cost_unused_product"
 msgid "The product \"%(product)s\" on landed cost \"%(landed_cost)s\" is not used."
 msgstr ""
-"De categorie \"%(category)s\"op landed cost \"%(landed_cost)s\" is niet "
+"Het product \"%(product)s\" op landed cost \"%(landed_cost)s\" is niet "
 "gebruikt."
 
 msgctxt "model:ir.model.button,string:landed_cost_cancel_button"
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgctxt "model:ir.model.button,string:landed_cost_draft_button"
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/pl.po` & `trytond_account_stock_landed_cost-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/pt.po` & `trytond_account_stock_landed_cost-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/ro.po` & `trytond_account_stock_landed_cost-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/ru.po` & `trytond_account_stock_landed_cost-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/sl.po` & `trytond_account_stock_landed_cost-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/tr.po` & `trytond_account_stock_landed_cost-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/uk.po` & `trytond_account_stock_landed_cost-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/locale/zh_CN.po` & `trytond_account_stock_landed_cost-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/message.xml` & `trytond_account_stock_landed_cost-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/product.py` & `trytond_account_stock_landed_cost-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/setup.py` & `trytond_account_stock_landed_cost-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/stock.py` & `trytond_account_stock_landed_cost-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/tests/scenario_account_stock_landed_cost.rst` & `trytond_account_stock_landed_cost-7.2.1/tests/scenario_account_stock_landed_cost.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/tox.ini` & `trytond_account_stock_landed_cost-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO` & `trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_landed_cost
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for landed cost
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_landed_cost-7.2.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt` & `trytond_account_stock_landed_cost-7.2.1/trytond_account_stock_landed_cost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-7.2.0/view/landed_cost_form.xml` & `trytond_account_stock_landed_cost-7.2.1/view/landed_cost_form.xml`

 * *Files identical despite different names*

