# Comparing `tmp/trytond_account_stock_eu-7.2.0.tar.gz` & `tmp/trytond_account_stock_eu-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_eu-7.2.0.tar", last modified: Mon Apr 29 15:36:38 2024, max compression
+gzip compressed data, was "trytond_account_stock_eu-7.2.1.tar", last modified: Wed May  1 12:12:34 2024, max compression
```

## Comparing `trytond_account_stock_eu-7.2.0.tar` & `trytond_account_stock_eu-7.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-29 15:16:40.000000 trytond_account_stock_eu-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:16:40.000000 trytond_account_stock_eu-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2119 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19525 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account_stock_eu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20839 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/account_stock_eu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      970 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1838 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/country.py
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/country.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/customs.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/customs.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.848709 trytond_account_stock_eu-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:01.000000 trytond_account_stock_eu-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.852042 trytond_account_stock_eu-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20067 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20753 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20327 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20322 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19903 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18290 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4770 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26402 2024-02-04 18:51:26.000000 trytond_account_stock_eu-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9898 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.852042 trytond_account_stock_eu-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9933 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_arrival.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10228 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_dispatch.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:01.000000 trytond_account_stock_eu-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-29 15:16:34.000000 trytond_account_stock_eu-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3277 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:16.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/account_fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/country_subdivision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/country_subdivision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/customs_tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list_incoterm.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transaction_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transaction_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transport_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transport_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_move_form_incoterm.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_shipment_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.580838 trytond_account_stock_eu-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-05-01 12:12:31.000000 trytond_account_stock_eu-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:12:30.000000 trytond_account_stock_eu-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-05-01 12:12:34.580838 trytond_account_stock_eu-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2119 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19525 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/account_stock_eu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20839 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/account_stock_eu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      970 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1838 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/country.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/country.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/customs.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/customs.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.574168 trytond_account_stock_eu-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      704 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.577503 trytond_account_stock_eu-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20067 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20753 2024-04-30 17:21:59.000000 trytond_account_stock_eu-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20327 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20322 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19903 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18290 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:12:34.580838 trytond_account_stock_eu-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4770 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26402 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9898 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.577503 trytond_account_stock_eu-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9933 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tests/scenario_account_stock_eu_arrival.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10228 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tests/scenario_account_stock_eu_dispatch.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-30 17:21:06.000000 trytond_account_stock_eu-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.580838 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3277 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:12:34.000000 trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:12:34.580838 trytond_account_stock_eu-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/account_fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/country_subdivision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/country_subdivision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/customs_tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_line_list_incoterm.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_declaration_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_transaction_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_transaction_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_transport_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/intrastat_transport_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/stock_move_form_incoterm.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-04-30 17:20:59.000000 trytond_account_stock_eu-7.2.1/view/stock_shipment_form.xml
```

### Comparing `trytond_account_stock_eu-7.2.0/COPYRIGHT` & `trytond_account_stock_eu-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/LICENSE` & `trytond_account_stock_eu-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/PKG-INFO` & `trytond_account_stock_eu-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_eu
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for european stock accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_eu-7.2.0/__init__.py` & `trytond_account_stock_eu-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/account_stock_eu.py` & `trytond_account_stock_eu-7.2.1/account_stock_eu.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/account_stock_eu.xml` & `trytond_account_stock_eu-7.2.1/account_stock_eu.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/company.py` & `trytond_account_stock_eu-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/country.py` & `trytond_account_stock_eu-7.2.1/country.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/country.xml` & `trytond_account_stock_eu-7.2.1/country.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/doc/conf.py` & `trytond_account_stock_eu-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/doc/design.rst` & `trytond_account_stock_eu-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/doc/usage.rst` & `trytond_account_stock_eu-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/bg.po` & `trytond_account_stock_eu-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/ca.po` & `trytond_account_stock_eu-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/cs.po` & `trytond_account_stock_eu-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/de.po` & `trytond_account_stock_eu-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
 
 msgctxt "model:ir.model.button,string:intrastat_declaration_export_button"
 msgid "Export"
 msgstr "Export"
 
 msgctxt "model:ir.rule.group,name:rule_group_intrastat_declaration_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_intrastat_declaration"
 msgid "Intrastat Declarations"
 msgstr "Intrastat-Meldungen"
 
 msgctxt "selection:account.stock.eu.intrastat.declaration,state:"
 msgid "Closed"
```

### Comparing `trytond_account_stock_eu-7.2.0/locale/es.po` & `trytond_account_stock_eu-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/es_419.po` & `trytond_account_stock_eu-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/et.po` & `trytond_account_stock_eu-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/fa.po` & `trytond_account_stock_eu-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/fi.po` & `trytond_account_stock_eu-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/fr.po` & `trytond_account_stock_eu-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/hu.po` & `trytond_account_stock_eu-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/id.po` & `trytond_account_stock_eu-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/it.po` & `trytond_account_stock_eu-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/lo.po` & `trytond_account_stock_eu-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/lt.po` & `trytond_account_stock_eu-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/nl.po` & `trytond_account_stock_eu-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/pl.po` & `trytond_account_stock_eu-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/pt.po` & `trytond_account_stock_eu-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/ro.po` & `trytond_account_stock_eu-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/ru.po` & `trytond_account_stock_eu-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/sl.po` & `trytond_account_stock_eu-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/tr.po` & `trytond_account_stock_eu-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/uk.po` & `trytond_account_stock_eu-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/locale/zh_CN.po` & `trytond_account_stock_eu-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/message.xml` & `trytond_account_stock_eu-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/setup.py` & `trytond_account_stock_eu-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/stock.py` & `trytond_account_stock_eu-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/stock.xml` & `trytond_account_stock_eu-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_arrival.rst` & `trytond_account_stock_eu-7.2.1/tests/scenario_account_stock_eu_arrival.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_dispatch.rst` & `trytond_account_stock_eu-7.2.1/tests/scenario_account_stock_eu_dispatch.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/tox.ini` & `trytond_account_stock_eu-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/PKG-INFO` & `trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_eu
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for european stock accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/SOURCES.txt` & `trytond_account_stock_eu-7.2.1/trytond_account_stock_eu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list.xml` & `trytond_account_stock_eu-7.2.1/view/intrastat_declaration_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/view/stock_move_form.xml` & `trytond_account_stock_eu-7.2.1/view/stock_move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.2.0/view/stock_shipment_form.xml` & `trytond_account_stock_eu-7.2.1/view/stock_shipment_form.xml`

 * *Files identical despite different names*

