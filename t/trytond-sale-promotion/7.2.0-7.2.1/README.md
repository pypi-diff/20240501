# Comparing `tmp/trytond_sale_promotion-7.2.0.tar.gz` & `tmp/trytond_sale_promotion-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_promotion-7.2.0.tar", last modified: Mon Apr 29 15:49:11 2024, max compression
+gzip compressed data, was "trytond_sale_promotion-7.2.1.tar", last modified: Wed May  1 11:20:05 2024, max compression
```

## Comparing `trytond_sale_promotion-7.2.0.tar` & `trytond_sale_promotion-7.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2024-04-29 15:26:13.000000 trytond_sale_promotion-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:26:12.000000 trytond_sale_promotion-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_promotion-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.439025 trytond_sale_promotion-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_promotion-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:28.000000 trytond_sale_promotion-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2970 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2916 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2525 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2953 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2680 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3168 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2960 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2486 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2928 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2627 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2868 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-04-29 13:17:17.000000 trytond_sale_promotion-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2779 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2396 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2527 2024-04-27 16:43:26.000000 trytond_sale_promotion-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11801 2024-03-17 11:01:36.000000 trytond_sale_promotion-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3871 2024-04-27 16:30:39.000000 trytond_sale_promotion-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:11.445692 trytond_sale_promotion-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4420 2024-03-17 11:01:36.000000 trytond_sale_promotion-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4546 2024-04-22 12:14:36.000000 trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2473 2024-04-22 12:14:36.000000 trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion_amount.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:28.000000 trytond_sale_promotion-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-29 15:26:08.000000 trytond_sale_promotion-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1655 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:11.000000 trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:11.442359 trytond_sale_promotion-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_promotion-7.2.0/view/promotion_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2007 2024-05-01 11:20:02.000000 trytond_sale_promotion-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:20:02.000000 trytond_sale_promotion-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.454460 trytond_sale_promotion-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2970 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2916 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2525 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-30 17:21:59.000000 trytond_sale_promotion-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2953 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2643 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2680 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3168 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2960 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2486 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2928 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2831 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2627 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2868 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2779 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2798 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2396 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2527 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11801 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3871 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4420 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4546 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tests/scenario_sale_promotion.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2473 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tests/scenario_sale_promotion_amount.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-30 17:21:06.000000 trytond_sale_promotion-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1655 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:20:05.000000 trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:20:05.457795 trytond_sale_promotion-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:21:00.000000 trytond_sale_promotion-7.2.1/view/promotion_list.xml
```

### Comparing `trytond_sale_promotion-7.2.0/CHANGELOG` & `trytond_sale_promotion-7.2.1/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_sale_promotion-7.2.0/COPYRIGHT` & `trytond_sale_promotion-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/LICENSE` & `trytond_sale_promotion-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/PKG-INFO` & `trytond_sale_promotion-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_promotion
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale promotion
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_promotion-7.2.0/README.rst` & `trytond_sale_promotion-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/doc/conf.py` & `trytond_sale_promotion-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/doc/index.rst` & `trytond_sale_promotion-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/bg.po` & `trytond_sale_promotion-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/ca.po` & `trytond_sale_promotion-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/cs.po` & `trytond_sale_promotion-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/de.po` & `trytond_sale_promotion-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 "exception \"%(exception)s\"."
 msgstr ""
 "Ungültige Formel \"%(formula)s\" in Verkaufsaktion \"%(promotion)s\" mit "
 "Fehler \"%(exception)s\"."
 
 msgctxt "model:ir.rule.group,name:rule_group_promotion_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_promotion"
 msgid "Promotions"
 msgstr "Verkaufsaktionen"
 
 msgctxt "model:sale.promotion,name:"
 msgid "Sale Promotion"
```

### Comparing `trytond_sale_promotion-7.2.0/locale/es.po` & `trytond_sale_promotion-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/es_419.po` & `trytond_sale_promotion-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/et.po` & `trytond_sale_promotion-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/fa.po` & `trytond_sale_promotion-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/fi.po` & `trytond_sale_promotion-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/fr.po` & `trytond_sale_promotion-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/hu.po` & `trytond_sale_promotion-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/id.po` & `trytond_sale_promotion-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/it.po` & `trytond_sale_promotion-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/lo.po` & `trytond_sale_promotion-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/lt.po` & `trytond_sale_promotion-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/nl.po` & `trytond_sale_promotion-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/pl.po` & `trytond_sale_promotion-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/pt.po` & `trytond_sale_promotion-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/ro.po` & `trytond_sale_promotion-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/ru.po` & `trytond_sale_promotion-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/sl.po` & `trytond_sale_promotion-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/tr.po` & `trytond_sale_promotion-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/uk.po` & `trytond_sale_promotion-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/locale/zh_CN.po` & `trytond_sale_promotion-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/sale.py` & `trytond_sale_promotion-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/sale.xml` & `trytond_sale_promotion-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/setup.py` & `trytond_sale_promotion-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion.rst` & `trytond_sale_promotion-7.2.1/tests/scenario_sale_promotion.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/tests/scenario_sale_promotion_amount.rst` & `trytond_sale_promotion-7.2.1/tests/scenario_sale_promotion_amount.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/tox.ini` & `trytond_sale_promotion-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/PKG-INFO` & `trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_promotion
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale promotion
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_promotion-7.2.0/trytond_sale_promotion.egg-info/SOURCES.txt` & `trytond_sale_promotion-7.2.1/trytond_sale_promotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-7.2.0/view/promotion_form.xml` & `trytond_sale_promotion-7.2.1/view/promotion_form.xml`

 * *Files identical despite different names*

