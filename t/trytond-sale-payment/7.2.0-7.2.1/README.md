# Comparing `tmp/trytond_sale_payment-7.2.0.tar.gz` & `tmp/trytond_sale_payment-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_payment-7.2.0.tar", last modified: Mon Apr 29 15:48:28 2024, max compression
+gzip compressed data, was "trytond_sale_payment-7.2.1.tar", last modified: Wed May  1 11:21:00 2024, max compression
```

## Comparing `trytond_sale_payment-7.2.0.tar` & `trytond_sale_payment-7.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1352 2024-04-29 15:25:37.000000 trytond_sale_payment-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-04-29 15:25:37.000000 trytond_sale_payment-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:21.000000 trytond_sale_payment-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6422 2024-04-27 16:30:39.000000 trytond_sale_payment-7.2.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.380152 trytond_sale_payment-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_sale_payment-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:26.000000 trytond_sale_payment-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      628 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      673 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      661 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-27 16:43:26.000000 trytond_sale_payment-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      594 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2927 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4526 2024-03-17 11:01:36.000000 trytond_sale_payment-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5413 2024-04-22 12:14:36.000000 trytond_sale_payment-7.2.0/tests/scenario_sale_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2886 2024-04-22 12:14:36.000000 trytond_sale_payment-7.2.0/tests/scenario_sale_payment_no_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:26.000000 trytond_sale_payment-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-29 15:25:33.000000 trytond_sale_payment-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-04-29 15:48:27.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-04-29 15:48:28.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:27.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:48:27.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2024-04-29 15:48:27.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:27.000000 trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:28.383485 trytond_sale_payment-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_sale_payment-7.2.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1453 2024-05-01 11:20:57.000000 trytond_sale_payment-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-05-01 11:20:57.000000 trytond_sale_payment-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35146 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6422 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.887114 trytond_sale_payment-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      628 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      673 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      661 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      691 2024-04-30 17:21:59.000000 trytond_sale_payment-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      594 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2927 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4526 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5413 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tests/scenario_sale_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2886 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tests/scenario_sale_payment_no_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-30 17:21:06.000000 trytond_sale_payment-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3100 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1577 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:21:00.000000 trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:21:00.890447 trytond_sale_payment-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_sale_payment-7.2.1/view/sale_form.xml
```

### Comparing `trytond_sale_payment-7.2.0/CHANGELOG` & `trytond_sale_payment-7.2.1/CHANGELOG`

 * *Files 14% similar despite different names*

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

### Comparing `trytond_sale_payment-7.2.0/COPYRIGHT` & `trytond_sale_payment-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/LICENSE` & `trytond_sale_payment-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/PKG-INFO` & `trytond_sale_payment-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_payment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that manage payments on sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_payment-7.2.0/account.py` & `trytond_sale_payment-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/doc/conf.py` & `trytond_sale_payment-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/ca.po` & `trytond_sale_payment-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/de.po` & `trytond_sale_payment-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/es.po` & `trytond_sale_payment-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/et.po` & `trytond_sale_payment-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/fa.po` & `trytond_sale_payment-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/fr.po` & `trytond_sale_payment-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/id.po` & `trytond_sale_payment-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/it.po` & `trytond_sale_payment-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/nl.po` & `trytond_sale_payment-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgctxt "model:ir.action,name:act_payments_relate"
 msgid "Payments"
 msgstr "Betalingen"
 
 msgctxt "model:ir.message,text:msg_sale_cancel_payment"
 msgid "You cannot cancel sale \"%(sale)s\" because it has payments."
 msgstr ""
-"U kunt de verkoop \"% (sale)s\" niet annuleren omdat deze een betalingen "
+"U kunt de verkoop \"%(sale)s\" niet annuleren omdat deze een betalingen "
 "heeft."
 
 msgctxt "model:ir.message,text:msg_sale_draft_payment"
 msgid "You cannot reset to draft sale \"%(sale)s\" because it has payments."
 msgstr ""
 "U kunt de verkoop \"%(sale)s\" niet terug zetten naar concept status omdat "
 "deze betalingen heeft."
```

### Comparing `trytond_sale_payment-7.2.0/locale/pl.po` & `trytond_sale_payment-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/pt.po` & `trytond_sale_payment-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/locale/ro.po` & `trytond_sale_payment-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/message.xml` & `trytond_sale_payment-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/sale.py` & `trytond_sale_payment-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/sale.xml` & `trytond_sale_payment-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/setup.py` & `trytond_sale_payment-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/tests/scenario_sale_payment.rst` & `trytond_sale_payment-7.2.1/tests/scenario_sale_payment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/tests/scenario_sale_payment_no_clearing.rst` & `trytond_sale_payment-7.2.1/tests/scenario_sale_payment_no_clearing.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/tox.ini` & `trytond_sale_payment-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/PKG-INFO` & `trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_payment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that manage payments on sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_payment-7.2.0/trytond_sale_payment.egg-info/SOURCES.txt` & `trytond_sale_payment-7.2.1/trytond_sale_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

