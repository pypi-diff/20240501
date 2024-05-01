# Comparing `tmp/trytond_account_tax_cash-7.0.1.tar.gz` & `tmp/trytond_account_tax_cash-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_tax_cash-7.0.1.tar", last modified: Wed May  1 12:10:06 2024, max compression
+gzip compressed data, was "trytond_account_tax_cash-7.2.0.tar", last modified: Mon Apr 29 15:37:17 2024, max compression
```

## Comparing `trytond_account_tax_cash-7.0.1.tar` & `trytond_account_tax_cash-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.016753 trytond_account_tax_cash-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1249 2024-05-01 12:10:02.000000 trytond_account_tax_cash-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:10:02.000000 trytond_account_tax_cash-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-05-01 12:10:06.016753 trytond_account_tax_cash-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12051 2024-04-27 05:19:51.000000 trytond_account_tax_cash-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.013419 trytond_account_tax_cash-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2795 2024-03-03 16:24:20.000000 trytond_account_tax_cash-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.013419 trytond_account_tax_cash-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2782 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3145 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2099 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2156 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2678 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2094 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:10:06.016753 trytond_account_tax_cash-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4329 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.013419 trytond_account_tax_cash-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2024-02-05 16:24:27.000000 trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3282 2024-02-05 16:24:27.000000 trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_period_close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4412 2024-02-05 16:24:27.000000 trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2490 2024-02-05 16:24:27.000000 trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-02-05 16:24:27.000000 trytond_account_tax_cash-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.016753 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2071 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:41.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:10:05.000000 trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:10:06.016753 trytond_account_tax_cash-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-10-30 17:06:38.000000 trytond_account_tax_cash-7.0.1/view/tax_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1249 2024-04-29 15:17:18.000000 trytond_account_tax_cash-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:17:18.000000 trytond_account_tax_cash-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12051 2024-04-29 13:17:17.000000 trytond_account_tax_cash-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.967686 trytond_account_tax_cash-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_account_tax_cash-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:02.000000 trytond_account_tax_cash-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.967686 trytond_account_tax_cash-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2782 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3145 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2099 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2678 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2343 2024-04-29 13:17:17.000000 trytond_account_tax_cash-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2024-04-27 16:43:22.000000 trytond_account_tax_cash-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_account_tax_cash-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2024-04-27 16:30:39.000000 trytond_account_tax_cash-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4329 2024-03-17 11:01:36.000000 trytond_account_tax_cash-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5035 2024-04-22 12:14:36.000000 trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3197 2024-04-22 12:14:36.000000 trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_period_close.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4393 2024-04-22 12:14:36.000000 trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2024-04-22 12:14:36.000000 trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_tax_cash-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:02.000000 trytond_account_tax_cash-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-04-29 15:17:13.000000 trytond_account_tax_cash-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2071 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:17.000000 trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:17.971019 trytond_account_tax_cash-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-01-16 14:00:20.000000 trytond_account_tax_cash-7.2.0/view/tax_line_form.xml
```

### Comparing `trytond_account_tax_cash-7.0.1/CHANGELOG` & `trytond_account_tax_cash-7.2.0/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-05-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_tax_cash-7.0.1/COPYRIGHT` & `trytond_account_tax_cash-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/LICENSE` & `trytond_account_tax_cash-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/PKG-INFO` & `trytond_account_tax_cash-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_cash
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to support tax report on cash basis
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -45,20 +45,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Tax Cash Module
 #######################
 
 The account_tax_cash module allows to make tax report on cash basis.
 
 The tax groups reported on cash basis are defined on the *Fiscal Year* and
```

### Comparing `trytond_account_tax_cash-7.0.1/README.rst` & `trytond_account_tax_cash-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/__init__.py` & `trytond_account_tax_cash-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/account.py` & `trytond_account_tax_cash-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/account.xml` & `trytond_account_tax_cash-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/doc/conf.py` & `trytond_account_tax_cash-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_account_tax_cash-7.0.1/doc/index.rst` & `trytond_account_tax_cash-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/bg.po` & `trytond_account_tax_cash-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/ca.po` & `trytond_account_tax_cash-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/cs.po` & `trytond_account_tax_cash-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/de.po` & `trytond_account_tax_cash-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/es.po` & `trytond_account_tax_cash-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/es_419.po` & `trytond_account_tax_cash-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/et.po` & `trytond_account_tax_cash-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/fa.po` & `trytond_account_tax_cash-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/fi.po` & `trytond_account_tax_cash-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/fr.po` & `trytond_account_tax_cash-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/hu.po` & `trytond_account_tax_cash-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/id.po` & `trytond_account_tax_cash-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/it.po` & `trytond_account_tax_cash-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/lo.po` & `trytond_account_tax_cash-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/lt.po` & `trytond_account_tax_cash-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/nl.po` & `trytond_account_tax_cash-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/pl.po` & `trytond_account_tax_cash-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/pt.po` & `trytond_account_tax_cash-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/ro.po` & `trytond_account_tax_cash-7.2.0/locale/ru.po`

 * *Files 8% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 
 msgctxt "field:account.period,tax_group_on_cash_basis:"
 msgid "Tax Group On Cash Basis"
 msgstr ""
 
 msgctxt "field:account.tax.group.cash,fiscalyear:"
 msgid "Fiscal Year"
-msgstr "An Fiscal"
+msgstr ""
 
 msgctxt "field:account.tax.group.cash,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.tax.group.cash,period:"
 msgid "Period"
-msgstr "Perioadă"
+msgstr ""
 
 msgctxt "field:account.tax.group.cash,tax_group:"
 msgid "Tax Group"
 msgstr ""
 
 msgctxt "field:account.tax.line,on_cash_basis:"
 msgid "On Cash Basis"
 msgstr ""
 
 msgctxt "field:account.tax.line,period:"
 msgid "Period"
-msgstr "Perioadă"
+msgstr ""
 
 msgctxt "field:party.party,supplier_tax_group_on_cash_basis:"
 msgid "Supplier Tax Group On Cash Basis"
 msgstr ""
 
 msgctxt "help:account.fiscalyear,tax_group_on_cash_basis:"
 msgid "The tax group reported on cash basis for this fiscal year."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_tax_cash-7.0.1/locale/ru.po` & `trytond_account_tax_cash-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/sl.po` & `trytond_account_tax_cash-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/tr.po` & `trytond_account_tax_cash-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/uk.po` & `trytond_account_tax_cash-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/locale/zh_CN.po` & `trytond_account_tax_cash-7.2.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.fiscalyear,tax_group_on_cash_basis:"
 msgid "Tax Group On Cash Basis"
-msgstr ""
+msgstr "Grup fiscal pe bază de numerar"
 
+#, fuzzy
 msgctxt "field:account.invoice,tax_group_on_cash_basis:"
 msgid "Tax Group On Cash Basis"
-msgstr ""
+msgstr "Grup fiscal pe bază de numerar"
 
 msgctxt "field:account.invoice.tax.group.cash,invoice:"
 msgid "Invoice"
-msgstr ""
+msgstr "Factură"
 
+#, fuzzy
 msgctxt "field:account.invoice.tax.group.cash,tax_group:"
 msgid "Tax Group"
-msgstr ""
+msgstr "Grup Fiscal"
 
+#, fuzzy
 msgctxt "field:account.period,tax_group_on_cash_basis:"
 msgid "Tax Group On Cash Basis"
-msgstr ""
+msgstr "Grup fiscal pe bază de numerar"
 
 msgctxt "field:account.tax.group.cash,fiscalyear:"
 msgid "Fiscal Year"
-msgstr ""
+msgstr "An Fiscal"
 
 msgctxt "field:account.tax.group.cash,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:account.tax.group.cash,period:"
 msgid "Period"
-msgstr ""
+msgstr "Perioadă"
 
+#, fuzzy
 msgctxt "field:account.tax.group.cash,tax_group:"
 msgid "Tax Group"
-msgstr ""
+msgstr "Grup Fiscal"
 
 msgctxt "field:account.tax.line,on_cash_basis:"
 msgid "On Cash Basis"
-msgstr ""
+msgstr "Pe bază de numerar"
 
 msgctxt "field:account.tax.line,period:"
 msgid "Period"
-msgstr ""
+msgstr "Perioadă"
 
+#, fuzzy
 msgctxt "field:party.party,supplier_tax_group_on_cash_basis:"
 msgid "Supplier Tax Group On Cash Basis"
-msgstr ""
+msgstr "Grup de impozitare a furnizorilor pe bază de numerar"
 
 msgctxt "help:account.fiscalyear,tax_group_on_cash_basis:"
 msgid "The tax group reported on cash basis for this fiscal year."
 msgstr ""
 
 msgctxt "help:account.invoice,tax_group_on_cash_basis:"
 msgid "The tax group reported on cash basis for this invoice."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_tax_cash-7.0.1/party.py` & `trytond_account_tax_cash-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/party.xml` & `trytond_account_tax_cash-7.2.0/party.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_account_tax_cash-7.0.1/party.xml` & `trytond_account_tax_cash-7.2.0/party.xml`

```diff
@@ -5,19 +5,21 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_tax_group_on_cash_basis">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_tax_group_on_cash_basis')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_tax_group_on_cash_basis</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_tax_group_on_cash_basis_account_party">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_tax_group_on_cash_basis')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_tax_group_on_cash_basis</field>
       <field name="group" ref="account.group_account_party"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_tax_cash-7.0.1/setup.py` & `trytond_account_tax_cash-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash.rst` & `trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =========================
 Account Tax Cash Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_tax_cash')
 
 Create company::
```

### Comparing `trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_period_close.rst` & `trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_period_close.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ===============================
 Account Tax Cash Closing Period
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_tax_cash')
 
 Create company::
 
@@ -94,23 +94,23 @@
     >>> line.account = receivable
     >>> line.party = party
     >>> line.credit = Decimal('10')
     >>> move.click('post')
 
 Can not close the period::
 
-    >>> period.click('close')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> period.click('close')
     Traceback (most recent call last):
         ...
     ClosePeriodWarning: ...
 
 Reconcile lines::
 
     >>> Line = Model.get('account.move.line')
     >>> lines = Line.find([('account', '=', receivable.id)])
     >>> reconcile_lines = Wizard('account.move.reconcile_lines', lines)
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
 
 Can close the period::
 
     >>> period.click('close')
```

### Comparing `trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_reconciliation.rst` & `trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_reconciliation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =======================================
 Account Tax Cash Reconsilition Scenario
 =======================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, create_tax_code, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax, create_tax_code
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_tax_cash')
 
 Create company::
 
@@ -128,16 +128,16 @@
 
     >>> payment_line, = [l for l in move.lines if l.account == receivable]
     >>> term1 = [l for l in invoice.move.lines if l.account == receivable][0]
 
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [payment_line, term1],
     ...     context={'payment_date': period.start_date})
-    >>> reconcile_lines.state == 'end'
-    True
+    >>> reconcile_lines.state
+    'end'
 
 Check tax codes::
 
     >>> with config.set_context(periods=[period.id]):
     ...     TaxCode(code_base_cash_basis.id).amount
     ...     TaxCode(code_tax_cash_basis.id).amount
     Decimal('50.00')
```

### Comparing `trytond_account_tax_cash-7.0.1/tests/scenario_account_tax_cash_supplier.rst` & `trytond_account_tax_cash-7.2.0/tests/scenario_account_tax_cash_supplier.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ==================================
 Account Tax Cash Supplier Scenario
 ==================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules('account_tax_cash')
 
 Create company::
```

### Comparing `trytond_account_tax_cash-7.0.1/tox.ini` & `trytond_account_tax_cash-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/PKG-INFO` & `trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_cash
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to support tax report on cash basis
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -45,20 +45,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Tax Cash Module
 #######################
 
 The account_tax_cash module allows to make tax report on cash basis.
 
 The tax groups reported on cash basis are defined on the *Fiscal Year* and
```

### Comparing `trytond_account_tax_cash-7.0.1/trytond_account_tax_cash.egg-info/SOURCES.txt` & `trytond_account_tax_cash-7.2.0/trytond_account_tax_cash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

