# Comparing `tmp/trytond_sale_subscription-7.2.0.tar.gz` & `tmp/trytond_sale_subscription-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_subscription-7.2.0.tar", last modified: Mon Apr 29 15:49:59 2024, max compression
+gzip compressed data, was "trytond_sale_subscription-7.2.1.tar", last modified: Wed May  1 11:18:04 2024, max compression
```

## Comparing `trytond_sale_subscription-7.2.0.tar` & `trytond_sale_subscription-7.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2039 2024-04-29 15:26:53.000000 trytond_sale_subscription-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2024-04-29 15:26:53.000000 trytond_sale_subscription-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_subscription-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/icons/tryton-sale-subscription.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18247 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18369 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18386 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16241 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19172 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18505 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15286 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16546 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16524 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18167 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16783 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17696 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14978 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17598 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/recurrence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4499 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/recurrence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/service.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2384 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/service.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4488 2024-03-17 11:01:36.000000 trytond_sale_subscription-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    37697 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/subscription.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14027 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/subscription.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5489 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5298 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_advanced_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4643 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_new_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_subscription-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2024-04-29 15:26:49.000000 trytond_sale_subscription-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3482 2024-04-29 15:49:59.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/create_invoice_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/line_consumption_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/service_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/service_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_consumption_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_consumption_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.227044 trytond_sale_subscription-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2140 2024-05-01 11:18:01.000000 trytond_sale_subscription-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      686 2024-05-01 11:18:00.000000 trytond_sale_subscription-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-05-01 11:18:04.227044 trytond_sale_subscription-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1841 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.223709 trytond_sale_subscription-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.223709 trytond_sale_subscription-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/icons/tryton-sale-subscription.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.223709 trytond_sale_subscription-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18248 2024-04-30 17:21:59.000000 trytond_sale_subscription-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18369 2024-04-30 17:21:59.000000 trytond_sale_subscription-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18386 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16241 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19172 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18505 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15286 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16546 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16524 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18175 2024-04-30 17:21:59.000000 trytond_sale_subscription-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16783 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17696 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14978 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17598 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/recurrence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4499 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/recurrence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/service.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2384 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/service.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:18:04.227044 trytond_sale_subscription-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4488 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    37697 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/subscription.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14027 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/subscription.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.223709 trytond_sale_subscription-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5489 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5298 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription_advanced_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4643 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription_new_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2024-04-30 17:21:06.000000 trytond_sale_subscription-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.227044 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2024-05-01 11:18:04.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:18:03.000000 trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:18:04.227044 trytond_sale_subscription-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/create_invoice_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/line_consumption_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_set_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/recurrence_rule_set_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/service_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/service_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2120 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_line_consumption_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_line_consumption_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1246 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-04-30 17:21:00.000000 trytond_sale_subscription-7.2.1/view/subscription_list.xml
```

### Comparing `trytond_sale_subscription-7.2.0/CHANGELOG` & `trytond_sale_subscription-7.2.1/CHANGELOG`

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

### Comparing `trytond_sale_subscription-7.2.0/COPYRIGHT` & `trytond_sale_subscription-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/LICENSE` & `trytond_sale_subscription-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/PKG-INFO` & `trytond_sale_subscription-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_subscription
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for subscription
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_subscription-7.2.0/README.rst` & `trytond_sale_subscription-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/__init__.py` & `trytond_sale_subscription-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/configuration.py` & `trytond_sale_subscription-7.2.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/configuration.xml` & `trytond_sale_subscription-7.2.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/doc/conf.py` & `trytond_sale_subscription-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/doc/index.rst` & `trytond_sale_subscription-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/icons/LICENSE` & `trytond_sale_subscription-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/invoice.py` & `trytond_sale_subscription-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/ir.py` & `trytond_sale_subscription-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/bg.po` & `trytond_sale_subscription-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/ca.po` & `trytond_sale_subscription-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -447,16 +447,16 @@
 "genera cap ocurrència."
 
 msgctxt "model:ir.message,text:msg_recurrence_rule_invalid_by"
 msgid ""
 "Invalid \"%(field)s\" \"%(value)s\" in recurence rule "
 "\"%(recurrence_rule)s\" with exception \"%(exception)s\"."
 msgstr ""
-"Invalid \"%(fields)\" \"%(value)s\" a la regla de recurrència "
-"\"%(recurrence_rule)s\" amb l'excpeció \"%(exception)s\"."
+"Invàlid \"%(field)s\" \"%(value)s\" a la regla de recurrència "
+"\"%(recurrence_rule)s\" amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.model.button,string:subscription_cancel_button"
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:subscription_draft_button"
 msgid "Draft"
```

### Comparing `trytond_sale_subscription-7.2.0/locale/cs.po` & `trytond_sale_subscription-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/de.po` & `trytond_sale_subscription-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
 
 msgctxt "model:ir.model.button,string:subscription_run_button"
 msgid "Run"
 msgstr "Ausführen"
 
 msgctxt "model:ir.rule.group,name:rule_group_subscription_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_subscription"
 msgid "Subscription"
 msgstr "Abonnement"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_subscription"
 msgid "Subscription"
```

### Comparing `trytond_sale_subscription-7.2.0/locale/es.po` & `trytond_sale_subscription-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/es_419.po` & `trytond_sale_subscription-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/et.po` & `trytond_sale_subscription-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/fa.po` & `trytond_sale_subscription-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/fi.po` & `trytond_sale_subscription-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/fr.po` & `trytond_sale_subscription-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/hu.po` & `trytond_sale_subscription-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/id.po` & `trytond_sale_subscription-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/it.po` & `trytond_sale_subscription-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/lo.po` & `trytond_sale_subscription-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/lt.po` & `trytond_sale_subscription-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/nl.po` & `trytond_sale_subscription-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -413,16 +413,16 @@
 
 msgctxt ""
 "model:ir.message,text:msg_consumption_invoice_missing_account_revenue"
 msgid ""
 "To invoice consumptions you must define an account revenue for product "
 "\"%(product)s\"."
 msgstr ""
-"Om consumpties te factureren, moet u een omzetrekening definiëren voor "
-"product \"% (product) s\"."
+"Om consumpties te factureren, moet u een omzet grootboekrekening definiëren "
+"voor product \"%(product)s\"."
 
 msgctxt "model:ir.message,text:msg_consumption_modify_invoiced"
 msgid "You cannot modify invoiced consumption \"%(consumption)s\"."
 msgstr "U kunt het gefactureerde verbruik \"%(consumption)s\" niet wijzigen."
 
 msgctxt "model:ir.message,text:msg_consumption_recurrence_invalid"
 msgid ""
```

### Comparing `trytond_sale_subscription-7.2.0/locale/pl.po` & `trytond_sale_subscription-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/pt.po` & `trytond_sale_subscription-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/ro.po` & `trytond_sale_subscription-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/ru.po` & `trytond_sale_subscription-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/sl.po` & `trytond_sale_subscription-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/tr.po` & `trytond_sale_subscription-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/uk.po` & `trytond_sale_subscription-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/locale/zh_CN.po` & `trytond_sale_subscription-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/message.xml` & `trytond_sale_subscription-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/party.py` & `trytond_sale_subscription-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/product.py` & `trytond_sale_subscription-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/recurrence.py` & `trytond_sale_subscription-7.2.1/recurrence.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/recurrence.xml` & `trytond_sale_subscription-7.2.1/recurrence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/service.py` & `trytond_sale_subscription-7.2.1/service.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/service.xml` & `trytond_sale_subscription-7.2.1/service.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/setup.py` & `trytond_sale_subscription-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/subscription.py` & `trytond_sale_subscription-7.2.1/subscription.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/subscription.xml` & `trytond_sale_subscription-7.2.1/subscription.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription.rst` & `trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_advanced_invoice.rst` & `trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription_advanced_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_new_line.rst` & `trytond_sale_subscription-7.2.1/tests/scenario_sale_subscription_new_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/tox.ini` & `trytond_sale_subscription-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/PKG-INFO` & `trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_subscription
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for subscription
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/SOURCES.txt` & `trytond_sale_subscription-7.2.1/trytond_sale_subscription.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/recurrence_rule_form.xml` & `trytond_sale_subscription-7.2.1/view/recurrence_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/recurrence_rule_list.xml` & `trytond_sale_subscription-7.2.1/view/recurrence_rule_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/subscription_form.xml` & `trytond_sale_subscription-7.2.1/view/subscription_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/subscription_line_form.xml` & `trytond_sale_subscription-7.2.1/view/subscription_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/subscription_line_list.xml` & `trytond_sale_subscription-7.2.1/view/subscription_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/subscription_line_list_sequence.xml` & `trytond_sale_subscription-7.2.1/view/subscription_line_list_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.2.0/view/subscription_list.xml` & `trytond_sale_subscription-7.2.1/view/subscription_list.xml`

 * *Files identical despite different names*

