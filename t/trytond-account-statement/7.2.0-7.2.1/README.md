# Comparing `tmp/trytond_account_statement-7.2.0.tar.gz` & `tmp/trytond_account_statement-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement-7.2.0.tar", last modified: Mon Apr 29 15:35:41 2024, max compression
+gzip compressed data, was "trytond_account_statement-7.2.1.tar", last modified: Wed May  1 12:16:15 2024, max compression
```

## Comparing `trytond_account_statement-7.2.0.tar` & `trytond_account_statement-7.2.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     5399 2024-04-29 15:15:49.000000 trytond_account_statement-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:15:49.000000 trytond_account_statement-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-03-17 11:01:36.000000 trytond_account_statement-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/bank.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_statement-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3680 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3104 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16002 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16529 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14452 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16967 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14608 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15240 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17386 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14426 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16728 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15409 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14586 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15204 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16521 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16889 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14408 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15437 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15067 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15872 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15199 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14638 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14654 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3474 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51356 2024-04-29 13:17:17.000000 trytond_account_statement-7.2.0/statement.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    47460 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18593 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.326880 trytond_account_statement-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14862 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2553 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/tests/scenario_account_statement_second_currency_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2992 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_statement_origin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-22 12:14:36.000000 trytond_account_statement-7.2.0/tests/scenario_statement_origin_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_statement-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-04-29 15:15:45.000000 trytond_account_statement-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2872 2024-04-29 15:35:41.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:40.000000 trytond_account_statement-7.2.0/trytond_account_statement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:41.330213 trytond_account_statement-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1732 2024-02-04 18:51:26.000000 trytond_account_statement-7.2.0/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_account_statement-7.2.0/view/statement_import_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-02-04 18:51:26.000000 trytond_account_statement-7.2.0/view/statement_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/view/statement_journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_line_tree_editable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_origin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-27 16:30:39.000000 trytond_account_statement-7.2.0/view/statement_origin_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_account_statement-7.2.0/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5500 2024-05-01 12:16:12.000000 trytond_account_statement-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:16:11.000000 trytond_account_statement-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/bank.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.434242 trytond_account_statement-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3680 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3104 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.434242 trytond_account_statement-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16002 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16795 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14452 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16837 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14608 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17386 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14426 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17016 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15409 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14586 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15204 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16521 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17151 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14408 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15437 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15067 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15872 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15199 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14638 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14654 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3474 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51356 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    47460 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18593 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14862 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2553 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement_second_currency_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2992 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_statement_origin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_statement_origin_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-04-30 17:21:06.000000 trytond_account_statement-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2872 2024-05-01 12:16:15.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1732 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_import_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_tree_editable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_origin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_origin_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_tree.xml
```

### Comparing `trytond_account_statement-7.2.0/CHANGELOG` & `trytond_account_statement-7.2.1/CHANGELOG`

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
 * Allow RPC on get_by_bank_account of statement journal
 * Search statement journal by bank account and currency
 * Support second currency on statement line
```

### Comparing `trytond_account_statement-7.2.0/COPYRIGHT` & `trytond_account_statement-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/LICENSE` & `trytond_account_statement-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/PKG-INFO` & `trytond_account_statement-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with account statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement-7.2.0/__init__.py` & `trytond_account_statement-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/account.py` & `trytond_account_statement-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/bank.py` & `trytond_account_statement-7.2.1/bank.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/doc/conf.py` & `trytond_account_statement-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/doc/configuration.rst` & `trytond_account_statement-7.2.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/doc/design.rst` & `trytond_account_statement-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/journal.py` & `trytond_account_statement-7.2.1/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/journal.xml` & `trytond_account_statement-7.2.1/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/bg.po` & `trytond_account_statement-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/ca.po` & `trytond_account_statement-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -120,24 +120,23 @@
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Import"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Empresa"
 
-#, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Tercer de l'empresa"
+msgstr "Moneda de l'empresa"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
@@ -167,18 +166,17 @@
 msgid "Party Required"
 msgstr "Tercer obligatori"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Relacionat amb"
 
-#, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Extracte"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
@@ -186,15 +184,15 @@
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Import"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
@@ -212,18 +210,17 @@
 msgid "Number"
 msgstr "Número"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Tercer"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Extracte"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
@@ -231,24 +228,23 @@
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Import"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Empresa"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Tercer de l'empresa"
+msgstr "Moneda de l'empresa"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -274,18 +270,17 @@
 msgid "Party"
 msgstr "Tercer"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Import pendent"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Extracte"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -395,14 +390,16 @@
 msgstr "Validat"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
+"La moneda del compte bancari \"%(bank_account)s\" ha de ser la mateixa que "
+"la del diari \"%(journal)s\" (%(currency)s)."
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Per importar l'extracte heu de crear un diari per al compte \"%(account)s\"."
 
@@ -424,35 +421,34 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "La validació dels extractes eliminarà de les línies dels extractes les "
 "factures ja pagades o cancel·lades."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
-"l'extracte \"%(statement)s\"."
+"Per eliminar la línia \"%(line)s\" heu de cancel·lar o restablir a esborrany"
+" l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
+"El signe de la moneda secundaria ha de ser el mateix que el del import."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
-"l'extracte \"%(statement)s\"."
+"Per eliminar l'origen \"%(origin)s\" heu de cancel·lar o restablir a "
+"esborrany l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "La validació dels extractes eliminarà les factures pagades en altres "
```

### Comparing `trytond_account_statement-7.2.0/locale/cs.po` & `trytond_account_statement-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/de.po` & `trytond_account_statement-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -120,24 +120,23 @@
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Fremdwährungsbetrag"
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
-#, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Unternehmen"
+msgstr "Unternehmenswährung"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
@@ -167,18 +166,17 @@
 msgid "Party Required"
 msgstr "Partei erforderlich"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Zugeordnet zu"
 
-#, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Währung"
+msgstr "Fremdwährung"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
@@ -186,15 +184,15 @@
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Fremdwährungsbetrag"
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
@@ -212,18 +210,17 @@
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Partei"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Währung"
+msgstr "Fremdwährung"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
@@ -231,24 +228,23 @@
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Fremdwährungsbetrag"
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Unternehmen"
+msgstr "Unternehmenswährung"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Währung"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -274,18 +270,17 @@
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Ausstehender Betrag"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Währung"
+msgstr "Fremdwährung"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Kontoauszug"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -395,14 +390,16 @@
 msgstr "Geprüft"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
+"Die Währung des Bankkontos \"%(bank_account)s\" muss mit der Währung "
+"\"%(currency)s\" des Journals \"%(journal)s\" übereinstimmen."
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Um den Kontoauszug importieren zu können, muss ein Journal für Konto "
 "\"%(account)s\" erstellt werden."
@@ -427,35 +424,37 @@
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
 "Die Validierung der Kontoauszüge wird bereits bezahlte oder stornierte "
 "Rechnungen von den Kontoauszugspositionen entfernen."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Damit der Buchungssatz \"%(move)s\" festgeschrieben werden kann, muss zuerst"
-" der Auszug \"%(statement)s\" festgeschrieben werden."
+"Um die Buchungsposition \"%(line)s\" löschen zu können, müssen Sie zuerst "
+"den Auszug \"%(statement)s\" annullieren oder in den Entwurfsstatus "
+"zurücksetzen."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
+"Sie müssen für den Fremdwährungsbetrag das gleiche Vorzeichen wie für den "
+"Betrag verwenden."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Damit der Buchungssatz \"%(move)s\" festgeschrieben werden kann, muss zuerst"
-" der Auszug \"%(statement)s\" festgeschrieben werden."
+"Um die Herkunft \"%(origin)s\" löschen zu können, muss zuerst der Auszug "
+"\"%(statement)s\" annulliert oder in den Entwurfsstatus zurückgesetzt "
+"werden."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
 "Die Validierung des Kontoauszugs wird bezahlte Rechnungen von anderen "
@@ -521,19 +520,19 @@
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
 msgstr "Prüfen"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
 msgstr "Positionengruppen"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
```

### Comparing `trytond_account_statement-7.2.0/locale/es.po` & `trytond_account_statement-7.2.1/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,648 +1,645 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr "Balance"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Date"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Saldo final"
+msgstr "Solde final"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Journal"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Lignes"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Número de líneas"
+msgstr "Nombre de lignes"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Archivo origen"
+msgstr "Fichier d'origine"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "Identificador archivo origen"
+msgstr "ID du fichier d'origine"
 
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Orígenes"
+msgstr "Origines"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Saldo inicial"
+msgstr "Solde initial"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "État"
 
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Por conciliar"
+msgstr "À réconcilier"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Importe total"
+msgstr "Montant total"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Validación"
+msgstr "Validation"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Archivo"
+msgstr "Fichier"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Formato del archivo"
+msgstr "Format du fichier"
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Cuenta bancaria"
+msgstr "Compte bancaire"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Tercero de la empresa"
+msgstr "Tiers de la société"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Journal"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Nom"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Tipo de validación"
+msgstr "Type de validation"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Montant"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Montant en devise secondaire"
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
-#, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Tercero de la empresa"
+msgstr "Devise de la société"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Date"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Description"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Asiento contable"
+msgstr "Mouvement comptable"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Numéro"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origen"
+msgstr "Origine"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tiers"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
-msgstr "Tercero obligatorio"
+msgstr "Tiers requis"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
-msgstr "Relacionado con"
+msgstr "Relative à"
 
-#, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Devise secondaire"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Estado del extracto"
+msgstr "État du relevé"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Montant"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Montant en devise secondaire"
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Date"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Journal"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Asiento"
+msgstr "Mouvement"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Numéro"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tiers"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Devise secondaire"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Compte"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Montant"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Montant en devise secondaire"
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Tercero de la empresa"
+msgstr "Devise de la société"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Date"
 
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Description"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Información"
+msgstr "Informations"
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Lignes"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Número"
+msgstr "Numéro"
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tiers"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Importe pendiente"
+msgstr "Montant en attente"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Moneda"
+msgstr "Devise secondaire"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "ID del Extracto"
+msgstr "ID du relevé"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Estado del extracto"
+msgstr "État du relevé"
 
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Extracto bancario"
+msgstr "Relevé comptable"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Inicio importación extracto"
+msgstr "Importer un relevé"
 
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Diario de extracto"
+msgstr "Journal de relevés"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Línea de extracto bancario"
+msgstr "Ligne de relevé comptable"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Grupo de líneas de extracto"
+msgstr "Groupe de lignes de relevé comptable"
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Origen extracto"
+msgstr "Origine de relevé comptable"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Información origen extracto"
+msgstr "Information de l'origine du relevé"
 
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Groupes de ligne"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Groupes de ligne"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Apuntes"
+msgstr "Lignes de mouvement"
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Asientos"
+msgstr "Mouvements"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Conciliar extractos"
+msgstr "Réconcilier les relevés"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Relevés"
 
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diarios de extracto"
+msgstr "Journaux de relevés"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Lignes de relevé"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Lignes de relevé"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Orígenes"
+msgstr "Origines"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Importar extracto"
+msgstr "Importer un relevé"
 
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Tous"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillons"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Contabilizado"
+msgstr "Comptabilisés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validés"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
+"La devise du compte bancaire « %(bank_account)s » doit être la même que "
+"celle « %(currency)s » du journal « %(journal)s »."
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
-"Para importar extractos, debe crear un diario para la cuenta "
-"\"%(account)s\"."
+"Pour importer le relevé, vous devez créer un journal pour le compte "
+"« %(account)s »."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr "Solo se permite un diario por cuenta bancaria."
+msgstr "Seulement un journal est permis par compte bancaire."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
-"Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
-"extracto \"%(statement)s\"."
+"Pour comptabiliser le mouvement « %(move)s », vous devez comptabiliser le "
+"relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
-msgstr "Para eliminar el extracto \"%(statement)s\" debe cancelarlo."
+msgstr "Pour supprimer le relevé « %(statement)s », vous devez l'annuler."
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
-"La validación de los extractos eliminará de las líneas de los extractos las "
-"facturas ya pagadas o canceladas."
+"La validation des relevés enlèvera les factures déjà payées ou annulées des "
+"lignes des relevés."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
-"extracto \"%(statement)s\"."
+"Pour supprimer la ligne « %(line)s », vous devez annuler ou réinitialiser à "
+"l'état brouillon le relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
+"Vous devez définir le même signe pour la deuxième devise que le montant."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
-"extracto \"%(statement)s\"."
+"Pour supprimer l'origine « %(origin)s », vous devez annuler ou réinitialiser"
+" à l'état brouillon le relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
-"La validación de los extractos eliminará las facturas pagadas en otros "
-"extractos."
+"La validation des relevés enlèvera les factures payées des autres relevés."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
-"Para contabilizar el extracto \"%(statement)s\" debe crear líneas por "
-"%(amount)s pendiente del origen \"%(origin)s\"."
+"Pour comptabiliser le relevé « %(statement)s », vous devez créer des lignes "
+"pour les %(amount)s en attente sur l'origine « %(origin)s »."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
-"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
-"tener un saldo final de %(end_balance)s en lugar de %(amount)s."
+"Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
+" avoir une balance finale de %(end_balance)s au lieu de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_add"
 msgid "To validate statement \"%(statement)s\" you must add %(n)s line(s)."
-msgstr "Para validar el extracto \"%(statement)s\" debe añadir %(n)s línea(s)."
+msgstr ""
+"Pour valider le relevé « %(statement)s », vous devez ajouter %(n)s ligne(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_remove"
 msgid "To validate statement \"%(statement)s\" you must remove %(n)s line(s)."
-msgstr "Para validar el extracto \"%(statement)s\" debe eliminar %(n)s línea(s)."
+msgstr ""
+"Pour valider le relevé « %(statement)s », vous devez enlever %(n)s ligne(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_total_amount"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
-"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
-"tener un importe total de %(total_amount)s en lugar de %(amount)s."
+"Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
+" avoir un montant total de %(total_amount)s au lieu de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "¿Estás seguro que quieres contabilizar el extracto?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser le relevé ?"
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Contabilizar"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Conciliar"
+msgstr "Réconcilier"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validar"
+msgstr "Valider"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Grupos de líneas"
+msgstr "Groupes de ligne"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Relevés"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Relevés"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Importar extracto"
+msgstr "Importer un relevé"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Diarios de extracto"
+msgstr "Journaux de relevés"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Extractos"
+msgstr "Relevés"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Montant"
 
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Annulé"
 
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Date"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Fecha:"
+msgstr "Date :"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Description"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Diario:"
+msgstr "Journal :"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Número"
+msgstr "Numéro"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tiers"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "report:account.statement:"
 msgid "Total"
 msgstr "Total"
 
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Extracto"
+msgstr "Relevé"
 
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Cancelado"
+msgstr "Annulé"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Contabilizado"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validé"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Montant"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr "Balance"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Número de líneas"
+msgstr "Nombre de lignes"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Información adicional"
+msgstr "Autre information"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Líneas de extracto"
+msgstr "Lignes de relevé"
 
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuler"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Importar"
+msgstr "Importer"
```

### Comparing `trytond_account_statement-7.2.0/locale/es_419.po` & `trytond_account_statement-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/et.po` & `trytond_account_statement-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/fa.po` & `trytond_account_statement-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/fi.po` & `trytond_account_statement-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/fr.po` & `trytond_account_statement-7.2.1/locale/sl.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,647 +1,672 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Balance"
+msgstr "Saldo"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Družba"
 
+#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Date"
+msgstr "Datum"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Solde final"
+msgstr "Končni saldo"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Journal"
+msgstr "Dnevnik"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr "Postavke"
 
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naziv"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Nombre de lignes"
+msgstr "Število postavk"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr "Fichier d'origine"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr "ID du fichier d'origine"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origines"
+msgstr "Origins"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Solde initial"
+msgstr "Začetni saldo"
 
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "État"
+msgstr "Stanje"
 
+#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "À réconcilier"
+msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Montant total"
+msgstr "Skupni znesek"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Validation"
+msgstr "Odobritev"
 
+#, fuzzy
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Družba"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr "Fichier"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr "Format du fichier"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Konto"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr "Compte bancaire"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Družba"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Tiers de la société"
+msgstr "Partner družbe"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Journal"
+msgstr "Dnevnik"
 
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Naziv"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Type de validation"
+msgstr "Vrsta odobritve"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Konto"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Znesek"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Družba"
 
 #, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Tiers de la société"
+msgstr "Partner družbe"
 
+#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Date"
+msgstr "Datum"
 
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Description"
+msgstr "Opis"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Mouvement comptable"
+msgstr "Knjižba"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Numéro"
+msgstr "Številka"
 
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr "Izvor"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Partner"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
-msgstr "Tiers requis"
+msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
-msgstr "Relative à"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "État du relevé"
+msgstr "Stanje izpiska"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Znesek"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Date"
+msgstr "Datum"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Journal"
+msgstr "Dnevnik"
 
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Mouvement"
+msgstr "Knjižba"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Numéro"
+msgstr "Številka"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Partner"
 
 #, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Konto"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Znesek"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Družba"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Tiers de la société"
+msgstr "Partner družbe"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Date"
+msgstr "Datum"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Description"
+msgstr "Opis"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr "Informations"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr "Postavke"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Numéro"
+msgstr "Številka"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Partner"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr "Montant en attente"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Devise"
+msgstr "Valuta"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "ID du relevé"
+msgstr "Izpisek"
 
+#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "État du relevé"
+msgstr "Stanje izpiska"
 
+#, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Relevé comptable"
+msgstr "Izpisek"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr "Importer un relevé"
+msgstr ""
 
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Journal de relevés"
+msgstr "Dnevnik izpiskov"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Ligne de relevé comptable"
+msgstr "Postavka izpiska"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Groupe de lignes de relevé comptable"
+msgstr "Skupina postavk izpiska"
 
+#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Origine de relevé comptable"
+msgstr "Postavka izpiska"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr "Information de l'origine du relevé"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Groupes de ligne"
+msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Groupes de ligne"
+msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Lignes de mouvement"
+msgstr "Move Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Mouvements"
+msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Réconcilier les relevés"
+msgstr "Reconcile Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Relevés"
+msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Journaux de relevés"
+msgstr "Statement Journals"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Lignes de relevé"
+msgstr "Statement Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Lignes de relevé"
+msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Origines"
+msgstr "Origins"
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Importer un relevé"
+msgstr "Import Statement"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "Tous"
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Brouillons"
+msgstr "Draft"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Comptabilisés"
+msgstr "Posted"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validés"
+msgstr "Validated"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
-"Pour importer le relevé, vous devez créer un journal pour le compte "
-"« %(account)s »."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr "Seulement un journal est permis par compte bancaire."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
-"Pour comptabiliser le mouvement « %(move)s », vous devez comptabiliser le "
-"relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
-msgstr "Pour supprimer le relevé « %(statement)s », vous devez l'annuler."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
-"La validation des relevés enlèvera les factures déjà payées ou annulées des "
-"lignes des relevés."
 
 msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Pour supprimer la ligne « %(line)s », vous devez annuler ou réinitialiser à "
-"l'état brouillon le relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
-"Pour supprimer l'origine « %(origin)s », vous devez annuler ou réinitialiser"
-" à l'état brouillon le relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
-"La validation des relevés enlèvera les factures payées des autres relevés."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
-"Pour comptabiliser le relevé « %(statement)s », vous devez créer des lignes "
-"pour les %(amount)s en attente sur l'origine « %(origin)s »."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
-"Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
-" avoir une balance finale de %(end_balance)s au lieu de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_add"
 msgid "To validate statement \"%(statement)s\" you must add %(n)s line(s)."
 msgstr ""
-"Pour valider le relevé « %(statement)s », vous devez ajouter %(n)s ligne(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_remove"
 msgid "To validate statement \"%(statement)s\" you must remove %(n)s line(s)."
 msgstr ""
-"Pour valider le relevé « %(statement)s », vous devez enlever %(n)s ligne(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_total_amount"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
-"Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
-" avoir un montant total de %(total_amount)s au lieu de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "Êtes-vous sûr de vouloir comptabiliser le relevé ?"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Comptabiliser"
+msgstr "Post"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Réconcilier"
+msgstr "Reconcile"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Valider"
+msgstr "Validate"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Groupes de ligne"
+msgstr "Line Groups"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Relevés"
+msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Relevés"
+msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Importer un relevé"
+msgstr "Import Statement"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Journaux de relevés"
+msgstr "Statement Journals"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Relevés"
+msgstr "Statements"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Znesek"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Annulé"
+msgstr "Preklicano"
 
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Date"
+msgstr "Datum"
 
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Date :"
+msgstr "Datum:"
 
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Description"
+msgstr "Opis"
 
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "V pripravi"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Journal :"
+msgstr "Dnevnik:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Numéro"
+msgstr "Številka"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Tiers"
+msgstr "Partner"
 
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Total"
+msgstr "Skupaj"
 
+#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Relevé"
+msgstr "Izpisek"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Annulé"
+msgstr "Preklicano"
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "V pripravi"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Comptabilisé"
+msgstr "Knjiženo"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validé"
+msgstr "Odobreno"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Znesek"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Balance"
+msgstr "Bilanca"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Nombre de lignes"
+msgstr "Število postavk"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Autre information"
+msgstr "Drugo"
 
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Lignes de relevé"
+msgstr "Postavke izpiska"
 
+#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Preklic"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr "Importer"
+msgstr ""
```

### Comparing `trytond_account_statement-7.2.0/locale/hu.po` & `trytond_account_statement-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/id.po` & `trytond_account_statement-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/it.po` & `trytond_account_statement-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/lo.po` & `trytond_account_statement-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/lt.po` & `trytond_account_statement-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/nl.po` & `trytond_account_statement-7.2.1/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -120,24 +120,23 @@
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Bedrag secundaire valuta"
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
-#, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Bedrijf relatie"
+msgstr "Bedrijfsvaluta"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
@@ -167,18 +166,17 @@
 msgid "Party Required"
 msgstr "Relatie verplicht"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr "Gerelateerd aan"
 
-#, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr "Secundaire valuta"
 
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
@@ -186,15 +184,15 @@
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Bedrag secundaire valuta"
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
@@ -212,18 +210,17 @@
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
 msgstr "Relatie"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr "Secundaire valuta"
 
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
@@ -231,24 +228,23 @@
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
 msgstr "Bedrag"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Bedrag secundaire valuta"
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Bedrijf relatie"
+msgstr "Bedrijfsvaluta"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
@@ -274,18 +270,17 @@
 msgid "Party"
 msgstr "Relatie"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr "Bedrag in afwachting"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr "Secundaire valuta"
 
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
 msgstr "Bankafschrift"
 
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
@@ -395,14 +390,16 @@
 msgstr "Gevalideerd"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
+"De valuta \"%(currency)s\" van bankrekening \"%(bank_account)s\" moet "
+"hetzelfde zijn als van het dagboek \"%(journal)s\"."
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
 "Om bankafschrift te importeren, moet u een dagboek aanmaken voor "
 "bankrekening \"%(account)s\"."
@@ -438,14 +435,15 @@
 msgstr ""
 "Om regel \"%(line)s\" te verwijderen moet u eerst het afschrift "
 "\"%(statement)s\" annuleren of resetten naar concept."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
+"U moet hetzelfde teken instellen voor de secundaire valuta dan het bedrag."
 
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
 "Om de bron \"%(origin)s\" te verwijderen moet u eerst het bankafschrift "
```

### Comparing `trytond_account_statement-7.2.0/locale/pl.po` & `trytond_account_statement-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/pt.po` & `trytond_account_statement-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/ro.po` & `trytond_account_statement-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/ru.po` & `trytond_account_statement-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/sl.po` & `trytond_account_statement-7.2.1/locale/zh_CN.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "日期格式"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr "Končni saldo"
+msgstr ""
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr "Dnevnik"
+msgstr ""
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr "Postavke"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "纳木"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr "Število postavk"
+msgstr ""
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
 msgstr ""
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
@@ -50,377 +51,360 @@
 #, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
 msgstr "Origins"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr "Začetni saldo"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr "状态"
 
 #, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
 msgstr "Reconcile"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr "Skupni znesek"
+msgstr ""
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr "Odobritev"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
 msgstr ""
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
 msgstr ""
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr "Partner družbe"
+msgstr ""
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr "Dnevnik"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "纳木"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr "Vrsta odobritve"
+msgstr ""
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr "Partner družbe"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "描述"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr "Knjižba"
+msgstr ""
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr "Številka"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Izvor"
+msgstr "Origins"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
 msgstr ""
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr "Stanje izpiska"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "日期格式"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr "Dnevnik"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Knjižba"
+msgstr "Moves"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr "Številka"
+msgstr ""
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr "Partner družbe"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "日期格式"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "描述"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr "Postavke"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr "Številka"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr "Valuta"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Izpisek"
+msgstr "Statement"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr "Stanje izpiska"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr "Izpisek"
+msgstr ""
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Dnevnik izpiskov"
+msgstr "Statement Journals"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr "Postavka izpiska"
+msgstr ""
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr "Skupina postavk izpiska"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr "Postavka izpiska"
+msgstr ""
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
 msgstr "Move Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
 msgstr "Moves"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
 msgstr "Reconcile Statements"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
 msgstr "Statement Lines"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
 msgstr "Origins"
 
-#, fuzzy
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
 msgstr "Statement"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
 msgstr "Posted"
 
 #, fuzzy
 msgctxt ""
@@ -538,135 +522,141 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
 msgstr "Line Groups"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
 msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
 msgstr "Statements"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
 msgstr "Import Statement"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
 msgstr "Statement Journals"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
 msgstr "Statements"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
 msgstr "Statement"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 #, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "取消"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "Datum"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "Datum:"
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "Opis"
+msgstr "描述"
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "V pripravi"
+msgstr "Draft"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr "Dnevnik:"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr "Številka"
+msgstr ""
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
+#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr "Skupaj"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Izpisek"
+msgstr "Statement"
 
 #, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "取消"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "V pripravi"
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Knjiženo"
+msgstr "Posted"
 
+#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Odobreno"
+msgstr "Validate"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr "Bilanca"
+msgstr ""
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr "Število postavk"
+msgstr ""
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr "Drugo"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Postavke izpiska"
+msgstr "Statement Lines"
 
 #, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "Preklic"
+msgstr "取消"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
 msgstr ""
```

### Comparing `trytond_account_statement-7.2.0/locale/tr.po` & `trytond_account_statement-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/uk.po` & `trytond_account_statement-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/locale/zh_CN.po` & `trytond_account_statement-7.2.1/locale/es.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,662 +1,644 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.statement,balance:"
 msgid "Balance"
-msgstr ""
+msgstr "Saldo"
 
 msgctxt "field:account.statement,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.statement,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.statement,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
 msgctxt "field:account.statement,end_balance:"
 msgid "End Balance"
-msgstr ""
+msgstr "Saldo final"
 
 msgctxt "field:account.statement,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Diario"
 
 msgctxt "field:account.statement,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Líneas"
 
-#, fuzzy
 msgctxt "field:account.statement,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nombre"
 
 msgctxt "field:account.statement,number_of_lines:"
 msgid "Number of Lines"
-msgstr ""
+msgstr "Número de líneas"
 
 msgctxt "field:account.statement,origin_file:"
 msgid "Origin File"
-msgstr ""
+msgstr "Archivo origen"
 
 msgctxt "field:account.statement,origin_file_id:"
 msgid "Origin File ID"
-msgstr ""
+msgstr "Identificador archivo origen"
 
-#, fuzzy
 msgctxt "field:account.statement,origins:"
 msgid "Origins"
-msgstr "Origins"
+msgstr "Orígenes"
 
 msgctxt "field:account.statement,start_balance:"
 msgid "Start Balance"
-msgstr ""
+msgstr "Saldo inicial"
 
-#, fuzzy
 msgctxt "field:account.statement,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Estado"
 
-#, fuzzy
 msgctxt "field:account.statement,to_reconcile:"
 msgid "To Reconcile"
-msgstr "Reconcile"
+msgstr "Por conciliar"
 
 msgctxt "field:account.statement,total_amount:"
 msgid "Total Amount"
-msgstr ""
+msgstr "Importe total"
 
 msgctxt "field:account.statement,validation:"
 msgid "Validation"
-msgstr ""
+msgstr "Validación"
 
 msgctxt "field:account.statement.import.start,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.statement.import.start,file_:"
 msgid "File"
-msgstr ""
+msgstr "Archivo"
 
 msgctxt "field:account.statement.import.start,file_format:"
 msgid "File Format"
-msgstr ""
+msgstr "Formato del archivo"
 
 msgctxt "field:account.statement.journal,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
 msgctxt "field:account.statement.journal,bank_account:"
 msgid "Bank Account"
-msgstr ""
+msgstr "Cuenta bancaria"
 
 msgctxt "field:account.statement.journal,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.statement.journal,company_party:"
 msgid "Company Party"
-msgstr ""
+msgstr "Tercero de la empresa"
 
 msgctxt "field:account.statement.journal,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.statement.journal,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Diario"
 
-#, fuzzy
 msgctxt "field:account.statement.journal,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nombre"
 
 msgctxt "field:account.statement.journal,validation:"
 msgid "Validation Type"
-msgstr ""
+msgstr "Tipo de validación"
 
 msgctxt "field:account.statement.line,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
 msgctxt "field:account.statement.line,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Importe"
 
 msgctxt "field:account.statement.line,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.statement.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.statement.line,company_currency:"
 msgid "Company Currency"
-msgstr ""
+msgstr "Moneda de la empresa"
 
 msgctxt "field:account.statement.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.statement.line,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
-#, fuzzy
 msgctxt "field:account.statement.line,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descripción"
 
 msgctxt "field:account.statement.line,move:"
 msgid "Account Move"
-msgstr ""
+msgstr "Asiento contable"
 
 msgctxt "field:account.statement.line,number:"
 msgid "Number"
-msgstr ""
+msgstr "Número"
 
-#, fuzzy
 msgctxt "field:account.statement.line,origin:"
 msgid "Origin"
-msgstr "Origins"
+msgstr "Origen"
 
 msgctxt "field:account.statement.line,party:"
 msgid "Party"
-msgstr ""
+msgstr "Tercero"
 
 msgctxt "field:account.statement.line,party_required:"
 msgid "Party Required"
-msgstr ""
+msgstr "Tercero obligatorio"
 
 msgctxt "field:account.statement.line,related_to:"
 msgid "Related To"
-msgstr ""
+msgstr "Relacionado con"
 
 msgctxt "field:account.statement.line,second_currency:"
 msgid "Second Currency"
-msgstr ""
+msgstr "Moneda secundaria"
 
-#, fuzzy
 msgctxt "field:account.statement.line,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
 msgctxt "field:account.statement.line,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Estado del extracto"
 
 msgctxt "field:account.statement.line.group,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Importe"
 
 msgctxt "field:account.statement.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.statement.line.group,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
 msgctxt "field:account.statement.line.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Diario"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,move:"
 msgid "Move"
-msgstr "Moves"
+msgstr "Asiento"
 
 msgctxt "field:account.statement.line.group,number:"
 msgid "Number"
-msgstr ""
+msgstr "Número"
 
 msgctxt "field:account.statement.line.group,party:"
 msgid "Party"
-msgstr ""
+msgstr "Tercero"
 
 msgctxt "field:account.statement.line.group,second_currency:"
 msgid "Second Currency"
-msgstr ""
+msgstr "Moneda secundaria"
 
-#, fuzzy
 msgctxt "field:account.statement.line.group,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
 msgctxt "field:account.statement.origin,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
 msgctxt "field:account.statement.origin,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Importe"
 
 msgctxt "field:account.statement.origin,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.statement.origin,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.statement.origin,company_currency:"
 msgid "Company Currency"
-msgstr ""
+msgstr "Moneda de la empresa"
 
 msgctxt "field:account.statement.origin,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descripción"
 
 msgctxt "field:account.statement.origin,information:"
 msgid "Information"
-msgstr ""
+msgstr "Información"
 
 msgctxt "field:account.statement.origin,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Líneas"
 
 msgctxt "field:account.statement.origin,number:"
 msgid "Number"
-msgstr ""
+msgstr "Número"
 
 msgctxt "field:account.statement.origin,party:"
 msgid "Party"
-msgstr ""
+msgstr "Tercero"
 
 msgctxt "field:account.statement.origin,pending_amount:"
 msgid "Pending Amount"
-msgstr ""
+msgstr "Importe pendiente"
 
 msgctxt "field:account.statement.origin,second_currency:"
 msgid "Second Currency"
-msgstr ""
+msgstr "Moneda secundaria"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
-#, fuzzy
 msgctxt "field:account.statement.origin,statement_id:"
 msgid "Statement ID"
-msgstr "Statement"
+msgstr "ID del Extracto"
 
 msgctxt "field:account.statement.origin,statement_state:"
 msgid "Statement State"
-msgstr ""
+msgstr "Estado del extracto"
 
-#, fuzzy
 msgctxt "model:account.journal,name:journal_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
 msgctxt "model:account.statement,name:"
 msgid "Account Statement"
-msgstr ""
+msgstr "Extracto bancario"
 
 msgctxt "model:account.statement.import.start,name:"
 msgid "Statement Import Start"
-msgstr ""
+msgstr "Inicio importación extracto"
 
-#, fuzzy
 msgctxt "model:account.statement.journal,name:"
 msgid "Statement Journal"
-msgstr "Statement Journals"
+msgstr "Diario de extracto"
 
 msgctxt "model:account.statement.line,name:"
 msgid "Account Statement Line"
-msgstr ""
+msgstr "Línea de extracto bancario"
 
 msgctxt "model:account.statement.line.group,name:"
 msgid "Account Statement Line Group"
-msgstr ""
+msgstr "Grupo de líneas de extracto"
 
 msgctxt "model:account.statement.origin,name:"
 msgid "Account Statement Origin"
-msgstr ""
+msgstr "Origen extracto"
 
 msgctxt "model:account.statement.origin.information,name:"
 msgid "Statement Origin Information"
-msgstr ""
+msgstr "Información origen extracto"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr "Grupos de líneas"
 
 msgctxt "model:ir.action,name:act_line_groups_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr "Grupos de líneas"
 
 msgctxt "model:ir.action,name:act_move_lines_form"
 msgid "Move Lines"
-msgstr "Move Lines"
+msgstr "Apuntes"
 
 msgctxt "model:ir.action,name:act_moves_form"
 msgid "Moves"
-msgstr "Moves"
+msgstr "Asientos"
 
 msgctxt "model:ir.action,name:act_reconcile"
 msgid "Reconcile Statements"
-msgstr "Reconcile Statements"
+msgstr "Conciliar extractos"
 
 msgctxt "model:ir.action,name:act_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Extractos"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Diarios de extracto"
 
 msgctxt "model:ir.action,name:act_statement_line_move"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de extracto"
 
 msgctxt "model:ir.action,name:act_statement_line_move_line"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de extracto"
 
 msgctxt "model:ir.action,name:act_statement_origin_form_statement"
 msgid "Origins"
-msgstr "Origins"
+msgstr "Orígenes"
 
 msgctxt "model:ir.action,name:report_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
 msgctxt "model:ir.action,name:wizard_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr "Importar extracto"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_statement_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Todo"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Borrador"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Posted"
+msgstr "Contabilizado"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
-msgstr "Validated"
+msgstr "Validado"
 
 msgctxt "model:ir.message,text:msg_bank_account_currency"
 msgid ""
 "The currency of bank account \"%(bank_account)s\" must be the same as "
 "\"%(currency)s\" of the journal \"%(journal)s\"."
 msgstr ""
+"La moneda de la cuenta bancaria \"%(bank_account)s\" debe ser la misma que "
+"la del diario \"%(journal)s\" (%(currency)s)."
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
 msgid ""
 "To import statement, you must create a journal for account \"%(account)s\"."
 msgstr ""
+"Para importar extractos, debe crear un diario para la cuenta "
+"\"%(account)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
-msgstr ""
+msgstr "Solo se permite un diario por cuenta bancaria."
 
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
+"Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
+"extracto \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
-msgstr ""
+msgstr "Para eliminar el extracto \"%(statement)s\" debe cancelarlo."
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
 "The validation of the statements will remove already paid or cancelled "
 "invoices from the statements' lines."
 msgstr ""
+"La validación de los extractos eliminará de las líneas de los extractos las "
+"facturas ya pagadas o canceladas."
 
 msgctxt "model:ir.message,text:msg_statement_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
+"Para eliminar la línea \"%(line)s\" teneis que cancelar o restaurar a "
+"borrador el extracto \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_line_second_currency_sign"
 msgid "You must set the same sign for second currency than amount."
 msgstr ""
+"El signo de la moneda secundaria debe ser el mismo que el del importe."
 
 msgctxt "model:ir.message,text:msg_statement_origin_delete_cancel_draft"
 msgid ""
 "To delete origin \"%(origin)s\" you must cancel or reset to draft statement "
 "\"%(statement)s\"."
 msgstr ""
+"Para eliminar el origen \"%(origin)s\" teneis que cancelar o restaurar a "
+"borrador el extracto \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_paid_invoice_draft"
 msgid ""
 "The validation of the statements will remove paid invoices from other "
 "statements."
 msgstr ""
+"La validación de los extractos eliminará las facturas pagadas en otros "
+"extractos."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
+"Para contabilizar el extracto \"%(statement)s\" debe crear líneas por "
+"%(amount)s pendiente del origen \"%(origin)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
+"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
+"tener un saldo final de %(end_balance)s en lugar de %(amount)s."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_add"
 msgid "To validate statement \"%(statement)s\" you must add %(n)s line(s)."
-msgstr ""
+msgstr "Para validar el extracto \"%(statement)s\" debe añadir %(n)s línea(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_number_of_lines_remove"
 msgid "To validate statement \"%(statement)s\" you must remove %(n)s line(s)."
-msgstr ""
+msgstr "Para validar el extracto \"%(statement)s\" debe eliminar %(n)s línea(s)."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_total_amount"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have total "
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
+"Para validar el extracto \"%(statement)s\" debe modificar las líneas para "
+"tener un importe total de %(total_amount)s en lugar de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr ""
+msgstr "¿Estás seguro que quieres contabilizar el extracto?"
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Cancelar"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Borrador"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Post"
+msgstr "Contabilizar"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
-msgstr "Reconcile"
+msgstr "Conciliar"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
-msgstr "Validate"
+msgstr "Validar"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_statement_journal_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_group_form"
 msgid "Line Groups"
-msgstr "Line Groups"
+msgstr "Grupos de líneas"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_configuration"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Extractos"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_form"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Extractos"
 
 msgctxt "model:ir.ui.menu,name:menu_statement_import"
 msgid "Import Statement"
-msgstr "Import Statement"
+msgstr "Importar extracto"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_statement_journal_form"
 msgid "Statement Journals"
-msgstr "Statement Journals"
+msgstr "Diarios de extracto"
 
 msgctxt "model:ir.ui.menu,name:menu_statements"
 msgid "Statements"
-msgstr "Statements"
+msgstr "Extractos"
 
 msgctxt "model:res.group,name:group_statement"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "#"
 msgstr "#"
 
 msgctxt "report:account.statement:"
 msgid "Amount"
-msgstr ""
+msgstr "Importe"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Cancelled"
-msgstr "取消"
+msgstr "Cancelado"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Date:"
-msgstr "日期格式"
+msgstr "Fecha:"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descripción"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Borrador"
 
 msgctxt "report:account.statement:"
 msgid "Journal:"
-msgstr ""
+msgstr "Diario:"
 
 msgctxt "report:account.statement:"
 msgid "Number"
-msgstr ""
+msgstr "Número"
 
 msgctxt "report:account.statement:"
 msgid "Party"
-msgstr ""
+msgstr "Tercero"
 
-#, fuzzy
 msgctxt "report:account.statement:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
 msgctxt "report:account.statement:"
 msgid "Total"
-msgstr ""
+msgstr "Total"
 
-#, fuzzy
 msgctxt "selection:account.journal,type:"
 msgid "Statement"
-msgstr "Statement"
+msgstr "Extracto"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Cancelled"
-msgstr "取消"
+msgstr "Cancelado"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Borrador"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Posted"
+msgstr "Contabilizado"
 
-#, fuzzy
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
-msgstr "Validate"
+msgstr "Validado"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
-msgstr ""
+msgstr "Importe"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Balance"
-msgstr ""
+msgstr "Saldo"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Number of Lines"
-msgstr ""
+msgstr "Número de líneas"
 
 msgctxt "view:account.statement:"
 msgid "Other Info"
-msgstr ""
+msgstr "Información adicional"
 
-#, fuzzy
 msgctxt "view:account.statement:"
 msgid "Statement Lines"
-msgstr "Statement Lines"
+msgstr "Líneas de extracto"
 
-#, fuzzy
 msgctxt "wizard_button:account.statement.import,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Cancelar"
 
 msgctxt "wizard_button:account.statement.import,start,import_:"
 msgid "Import"
-msgstr ""
+msgstr "Importar"
```

### Comparing `trytond_account_statement-7.2.0/message.xml` & `trytond_account_statement-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/setup.py` & `trytond_account_statement-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/statement.fodt` & `trytond_account_statement-7.2.1/statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/statement.py` & `trytond_account_statement-7.2.1/statement.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/statement.xml` & `trytond_account_statement-7.2.1/statement.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tests/scenario_account_statement.rst` & `trytond_account_statement-7.2.1/tests/scenario_account_statement.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tests/scenario_account_statement_bank_account.rst` & `trytond_account_statement-7.2.1/tests/scenario_account_statement_bank_account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tests/scenario_account_statement_second_currency_invoice.rst` & `trytond_account_statement-7.2.1/tests/scenario_account_statement_second_currency_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tests/scenario_statement_origin.rst` & `trytond_account_statement-7.2.1/tests/scenario_statement_origin.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tests/scenario_statement_origin_invoices.rst` & `trytond_account_statement-7.2.1/tests/scenario_statement_origin_invoices.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/tox.ini` & `trytond_account_statement-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/trytond_account_statement.egg-info/PKG-INFO` & `trytond_account_statement-7.2.1/trytond_account_statement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with account statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement-7.2.0/trytond_account_statement.egg-info/SOURCES.txt` & `trytond_account_statement-7.2.1/trytond_account_statement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/line_group_form.xml` & `trytond_account_statement-7.2.1/view/line_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_form.xml` & `trytond_account_statement-7.2.1/view/statement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_journal_form.xml` & `trytond_account_statement-7.2.1/view/statement_journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_line_form.xml` & `trytond_account_statement-7.2.1/view/statement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_line_tree.xml` & `trytond_account_statement-7.2.1/view/statement_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_line_tree_editable.xml` & `trytond_account_statement-7.2.1/view/statement_line_tree_editable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_origin_form.xml` & `trytond_account_statement-7.2.1/view/statement_origin_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.0/view/statement_origin_tree.xml` & `trytond_account_statement-7.2.1/view/statement_origin_tree.xml`

 * *Files identical despite different names*

