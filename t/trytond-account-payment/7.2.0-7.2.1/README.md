# Comparing `tmp/trytond_account_payment-7.2.0.tar.gz` & `tmp/trytond_account_payment-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment-7.2.0.tar", last modified: Mon Apr 29 15:34:33 2024, max compression
+gzip compressed data, was "trytond_account_payment-7.2.1.tar", last modified: Wed May  1 12:20:27 2024, max compression
```

## Comparing `trytond_account_payment-7.2.0.tar` & `trytond_account_payment-7.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3876 2024-04-29 15:15:03.000000 trytond_account_payment-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:03.000000 trytond_account_payment-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27997 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7785 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3888 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:56.000000 trytond_account_payment-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/icons/tryton-payment.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    19645 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20283 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18078 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20834 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20160 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17490 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19288 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20582 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20610 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18536 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18312 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18642 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21580 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20382 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18381 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19170 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19873 2024-04-29 13:17:17.000000 trytond_account_payment-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19646 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19231 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16686 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18288 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2212 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    24371 2024-02-13 17:30:52.000000 trytond_account_payment-7.2.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26995 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4835 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5477 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2583 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_blocked_direct_debit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3138 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_direct_debit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3528 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_planning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2714 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4209 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_warnings.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:56.000000 trytond_account_payment-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:14:58.000000 trytond_account_payment-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3402 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/move_line_create_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-01-27 09:58:52.000000 trytond_account_payment-7.2.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      841 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-01-27 09:58:52.000000 trytond_account_payment-7.2.0/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/move_line_pay_ask_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/move_line_pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/view/party_reception_direct_debit_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1833 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1029 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.374319 trytond_account_payment-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3977 2024-05-01 12:20:23.000000 trytond_account_payment-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 12:20:23.000000 trytond_account_payment-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-05-01 12:20:27.374319 trytond_account_payment-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1421 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27997 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7785 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.367653 trytond_account_payment-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3888 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.367653 trytond_account_payment-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/icons/tryton-payment.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.370986 trytond_account_payment-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19645 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20283 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18078 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20834 2024-04-30 17:21:59.000000 trytond_account_payment-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20160 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17490 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19288 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20582 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20610 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18536 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18312 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18642 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21580 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20376 2024-04-30 17:21:59.000000 trytond_account_payment-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18381 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19170 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19873 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19646 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19231 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16686 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18288 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2212 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    24371 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26995 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:20:27.374319 trytond_account_payment-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4835 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.370986 trytond_account_payment-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5477 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2583 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_blocked_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3138 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3528 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_planning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2714 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4209 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/scenario_account_payment_warnings.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:06.000000 trytond_account_payment-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.374319 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3402 2024-05-01 12:20:27.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:20:26.000000 trytond_account_payment-7.2.1/trytond_account_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:27.374319 trytond_account_payment-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_create_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      841 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_pay_ask_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/move_line_pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/party_reception_direct_debit_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1029 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_payment-7.2.1/view/payment_list.xml
```

### Comparing `trytond_account_payment-7.2.0/CHANGELOG` & `trytond_account_payment-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_payment-7.2.0/COPYRIGHT` & `trytond_account_payment-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/LICENSE` & `trytond_account_payment-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/PKG-INFO` & `trytond_account_payment-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment-7.2.0/__init__.py` & `trytond_account_payment-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/account.py` & `trytond_account_payment-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/account.xml` & `trytond_account_payment-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/doc/conf.py` & `trytond_account_payment-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/doc/design.rst` & `trytond_account_payment-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/exceptions.py` & `trytond_account_payment-7.2.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/icons/LICENSE` & `trytond_account_payment-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/bg.po` & `trytond_account_payment-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/ca.po` & `trytond_account_payment-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/cs.po` & `trytond_account_payment-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/de.po` & `trytond_account_payment-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -576,27 +576,27 @@
 msgctxt "model:ir.model.button,string:payment_succeed_button"
 msgid "Succeed"
 msgstr "Erfolgreich markieren"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_party_reception_direct_debit_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_group_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_journal_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_account_payment_group"
 msgid "Default Account Payment Group"
 msgstr "Standard Zahlungslauf"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_account_payment_group"
 msgid "Account Payment Group"
```

### Comparing `trytond_account_payment-7.2.0/locale/es.po` & `trytond_account_payment-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/es_419.po` & `trytond_account_payment-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/et.po` & `trytond_account_payment-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/fa.po` & `trytond_account_payment-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/fi.po` & `trytond_account_payment-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/fr.po` & `trytond_account_payment-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/hu.po` & `trytond_account_payment-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/id.po` & `trytond_account_payment-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/it.po` & `trytond_account_payment-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/lo.po` & `trytond_account_payment-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/lt.po` & `trytond_account_payment-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/nl.po` & `trytond_account_payment-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -454,16 +454,16 @@
 msgstr "In behandeling"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
-"U kunt de relatie \"% (party) s\" niet verwijderen terwijl ze facturen in "
-"behandeling hebben bij bedrijf \"%(company)s\"."
+"U kunt relatie \"%(party)s\" niet verwijderen terwijl ze betalingen open "
+"hebben staan bij bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_move_cancel_payments"
 msgid ""
 "The moves \"%(moves)s\" contain lines with payments, you may want to cancel "
 "them before cancelling."
 msgstr ""
 "De boekingen \"%(moves)s\" bevatten regels met betalingen, mogelijk wilt u "
@@ -498,16 +498,16 @@
 msgstr "Regel \"%(line)s\" is geblokkeerd voor betaling."
 
 msgctxt "model:ir.message,text:msg_pay_line_group"
 msgid ""
 "The lines \"%(names)s\" for %(party)s could be grouped with the line "
 "\"%(line)s\"."
 msgstr ""
-"De lijnen \"%(names)s\" voor %(party)s kunnen worden gegroepeerd met de lijn"
-" \"%(line s\"."
+"De regels \"%(names)s\" voor %(party)s kunnen worden gegroepeerd met de "
+"regel \"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_payment_delete_draft"
 msgid "To delete payment \"%(payment)s\" you must reset it to draft state."
 msgstr ""
 "Om betaling \"%(payment)s\" te verwijderen, moet u het terugzetten naar de "
 "conceptstatus."
```

### Comparing `trytond_account_payment-7.2.0/locale/pl.po` & `trytond_account_payment-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/pt.po` & `trytond_account_payment-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/ro.po` & `trytond_account_payment-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/ru.po` & `trytond_account_payment-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/sl.po` & `trytond_account_payment-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/tr.po` & `trytond_account_payment-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/uk.po` & `trytond_account_payment-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/locale/zh_CN.po` & `trytond_account_payment-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/message.xml` & `trytond_account_payment-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/party.py` & `trytond_account_payment-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/party.xml` & `trytond_account_payment-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/payment.py` & `trytond_account_payment-7.2.1/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/payment.xml` & `trytond_account_payment-7.2.1/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/setup.py` & `trytond_account_payment-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_blocked_direct_debit.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_blocked_direct_debit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_direct_debit.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_direct_debit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_dunning.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_dunning.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_invoice.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_planning.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_planning.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_statement.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_statement.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/scenario_account_payment_warnings.rst` & `trytond_account_payment-7.2.1/tests/scenario_account_payment_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tests/test_module.py` & `trytond_account_payment-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/tox.ini` & `trytond_account_payment-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/trytond_account_payment.egg-info/PKG-INFO` & `trytond_account_payment-7.2.1/trytond_account_payment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for payment
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_payment-7.2.0/trytond_account_payment.egg-info/SOURCES.txt` & `trytond_account_payment-7.2.1/trytond_account_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/view/move_line_form.xml` & `trytond_account_payment-7.2.1/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/view/move_line_list.xml` & `trytond_account_payment-7.2.1/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/view/payment_form.xml` & `trytond_account_payment-7.2.1/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/view/payment_group_form.xml` & `trytond_account_payment-7.2.1/view/payment_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.2.0/view/payment_list.xml` & `trytond_account_payment-7.2.1/view/payment_list.xml`

 * *Files identical despite different names*

