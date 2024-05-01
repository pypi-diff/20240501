# Comparing `tmp/trytond_currency-7.2.0.tar.gz` & `tmp/trytond_currency-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency-7.2.0.tar", last modified: Mon Apr 29 15:39:43 2024, max compression
+gzip compressed data, was "trytond_currency-7.2.1.tar", last modified: Wed May  1 11:59:21 2024, max compression
```

## Comparing `trytond_currency-7.2.0.tar` & `trytond_currency-7.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2024-04-29 15:19:11.000000 trytond_currency-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:19:10.000000 trytond_currency-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15628 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:08.000000 trytond_currency-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/ecb.py
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/icons/tryton-currency.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5977 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4810 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5914 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5185 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5949 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5901 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5480 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5615 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5369 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5853 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5806 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5594 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6453 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5508 2024-04-27 16:43:23.000000 trytond_currency-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/message.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2024-02-04 18:51:26.000000 trytond_currency-7.2.0/scripts/import_currencies.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4801 2024-04-27 16:30:39.000000 trytond_currency-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.983867 trytond_currency-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_compute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-22 12:14:36.000000 trytond_currency-7.2.0/tests/scenario_currency_rate_update.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14824 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:08.000000 trytond_currency-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-29 15:19:06.000000 trytond_currency-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/trytond_currency.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2309 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_currency-7.2.0/trytond_currency.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:43.000000 trytond_currency-7.2.0/trytond_currency.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:43.987200 trytond_currency-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-01-27 09:58:52.000000 trytond_currency-7.2.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:20.000000 trytond_currency-7.2.0/view/currency_rate_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/currency_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-15 07:12:15.000000 trytond_currency-7.2.0/view/currency_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4085 2024-05-01 11:59:18.000000 trytond_currency-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 11:59:18.000000 trytond_currency-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15628 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3150 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/ecb.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1364 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/icons/tryton-currency.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5012 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5977 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4810 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5914 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5185 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5949 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5901 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5480 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5615 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5369 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5853 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5791 2024-04-30 17:21:59.000000 trytond_currency-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5806 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5594 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6453 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5508 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/message.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/scripts/import_currencies.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4801 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_compute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_rate_update.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14824 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-30 17:21:06.000000 trytond_currency-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/trytond_currency.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2309 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_tree.xml
```

### Comparing `trytond_currency-7.2.0/CHANGELOG` & `trytond_currency-7.2.1/CHANGELOG`

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

### Comparing `trytond_currency-7.2.0/COPYRIGHT` & `trytond_currency-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/LICENSE` & `trytond_currency-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/PKG-INFO` & `trytond_currency-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-7.2.0/currency.py` & `trytond_currency-7.2.1/currency.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/currency.xml` & `trytond_currency-7.2.1/currency.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/doc/conf.py` & `trytond_currency-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/doc/configuration.rst` & `trytond_currency-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/doc/design.rst` & `trytond_currency-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/doc/usage.rst` & `trytond_currency-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/ecb.py` & `trytond_currency-7.2.1/ecb.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/fields.py` & `trytond_currency-7.2.1/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/icons/LICENSE` & `trytond_currency-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/ir.py` & `trytond_currency-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/bg.po` & `trytond_currency-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/ca.po` & `trytond_currency-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/cs.po` & `trytond_currency-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/de.po` & `trytond_currency-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/es.po` & `trytond_currency-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/es_419.po` & `trytond_currency-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/et.po` & `trytond_currency-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/fa.po` & `trytond_currency-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/fi.po` & `trytond_currency-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/fr.po` & `trytond_currency-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/hu.po` & `trytond_currency-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/id.po` & `trytond_currency-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/it.po` & `trytond_currency-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/lo.po` & `trytond_currency-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/lt.po` & `trytond_currency-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/nl.po` & `trytond_currency-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/pl.po` & `trytond_currency-7.2.1/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 msgctxt "field:currency.cron,weekday:"
 msgid "Day of Week"
 msgstr "Dzień tygodnia"
 
 msgctxt "field:currency.cron-currency.currency,cron:"
 msgid "Cron"
-msgstr "Cron"
+msgstr "Planista zadań"
 
 msgctxt "field:currency.cron-currency.currency,currency:"
 msgid "Currency"
 msgstr "Waluta"
 
 msgctxt "field:currency.currency,code:"
 msgid "Code"
@@ -178,15 +178,14 @@
 msgid "Run"
 msgstr "Uruchom"
 
 msgctxt "model:ir.ui.menu,name:menu_cron_form"
 msgid "Scheduled Rate Updates"
 msgstr "Zaplanowane aktualizacje walut"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_currency"
 msgid "Currencies"
 msgstr "Waluty"
 
 msgctxt "model:ir.ui.menu,name:menu_currency_form"
 msgid "Currencies"
 msgstr "Waluty"
@@ -205,15 +204,15 @@
 
 msgctxt "selection:currency.cron,frequency:"
 msgid "Weekly"
 msgstr "Tygodniowo"
 
 msgctxt "selection:currency.cron,source:"
 msgid "European Central Bank"
-msgstr ""
+msgstr "Europejski Bank Centralny"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Update Currency Rates"
 msgstr "Aktualizuj kursy walut"
 
 msgctxt "view:currency.currency:"
 msgid "Rates"
```

### Comparing `trytond_currency-7.2.0/locale/pt.po` & `trytond_currency-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/ro.po` & `trytond_currency-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/ru.po` & `trytond_currency-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/sl.po` & `trytond_currency-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/tr.po` & `trytond_currency-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/uk.po` & `trytond_currency-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/locale/zh_CN.po` & `trytond_currency-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/message.xml` & `trytond_currency-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/scripts/import_currencies.py` & `trytond_currency-7.2.1/scripts/import_currencies.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/setup.py` & `trytond_currency-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/tests/scenario_currency_compute.rst` & `trytond_currency-7.2.1/tests/scenario_currency_compute.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/tests/scenario_currency_rate_update.rst` & `trytond_currency-7.2.1/tests/scenario_currency_rate_update.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/tests/test_module.py` & `trytond_currency-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/tests/tools.py` & `trytond_currency-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/tox.ini` & `trytond_currency-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/trytond_currency.egg-info/PKG-INFO` & `trytond_currency-7.2.1/trytond_currency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-7.2.0/trytond_currency.egg-info/SOURCES.txt` & `trytond_currency-7.2.1/trytond_currency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/view/cron_form.xml` & `trytond_currency-7.2.1/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.0/view/currency_form.xml` & `trytond_currency-7.2.1/view/currency_form.xml`

 * *Files identical despite different names*

