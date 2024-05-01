# Comparing `tmp/trytond_incoterm-7.2.0.tar.gz` & `tmp/trytond_incoterm-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_incoterm-7.2.0.tar", last modified: Mon Apr 29 15:41:07 2024, max compression
+gzip compressed data, was "trytond_incoterm-7.2.1.tar", last modified: Wed May  1 11:58:27 2024, max compression
```

## Comparing `trytond_incoterm-7.2.0.tar` & `trytond_incoterm-7.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      855 2024-04-29 15:20:17.000000 trytond_incoterm-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:20:17.000000 trytond_incoterm-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1636 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6269 2024-01-27 09:58:52.000000 trytond_incoterm-7.2.0/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.938338 trytond_incoterm-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:11.000000 trytond_incoterm-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3169 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/incoterm.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11251 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/incoterm.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.941671 trytond_incoterm-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5670 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5744 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5717 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5743 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4510 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5607 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:24.000000 trytond_incoterm-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1055 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3971 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2326 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3730 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5068 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1499 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1404 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.941671 trytond_incoterm-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6119 2024-04-22 12:14:36.000000 trytond_incoterm-7.2.0/tests/scenario_incoterm.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1200 2024-04-27 16:30:39.000000 trytond_incoterm-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:11.000000 trytond_incoterm-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-29 15:20:12.000000 trytond_incoterm-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2769 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:41:07.000000 trytond_incoterm-7.2.0/trytond_incoterm.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:41:07.945004 trytond_incoterm-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/carrier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_form_purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_form_sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/party_incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/sale_opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-7.2.0/view/stock_shipment_out_return_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.551687 trytond_incoterm-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      956 2024-05-01 11:58:24.000000 trytond_incoterm-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 11:58:24.000000 trytond_incoterm-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-05-01 11:58:27.551687 trytond_incoterm-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1636 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6269 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.548354 trytond_incoterm-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3169 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/incoterm.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11251 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/incoterm.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.548354 trytond_incoterm-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5670 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5744 2024-04-30 17:21:59.000000 trytond_incoterm-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5717 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5743 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4575 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4510 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5607 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1055 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3971 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2326 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3730 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:58:27.551687 trytond_incoterm-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5068 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1499 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1404 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.548354 trytond_incoterm-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6119 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/tests/scenario_incoterm.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1200 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-30 17:21:06.000000 trytond_incoterm-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.551687 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2769 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:58:27.000000 trytond_incoterm-7.2.1/trytond_incoterm.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:58:27.551687 trytond_incoterm-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/carrier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/party_form_purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/party_form_sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/party_incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/party_incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/sale_opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/stock_shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/stock_shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/stock_shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_incoterm-7.2.1/view/stock_shipment_out_return_form.xml
```

### Comparing `trytond_incoterm-7.2.0/CHANGELOG` & `trytond_incoterm-7.2.1/CHANGELOG`

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

### Comparing `trytond_incoterm-7.2.0/COPYRIGHT` & `trytond_incoterm-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/LICENSE` & `trytond_incoterm-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/PKG-INFO` & `trytond_incoterm-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_incoterm
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_incoterm-7.2.0/__init__.py` & `trytond_incoterm-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/account.py` & `trytond_incoterm-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/carrier.xml` & `trytond_incoterm-7.2.1/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/common.py` & `trytond_incoterm-7.2.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/doc/conf.py` & `trytond_incoterm-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/incoterm.py` & `trytond_incoterm-7.2.1/incoterm.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/incoterm.xml` & `trytond_incoterm-7.2.1/incoterm.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/bg.po` & `trytond_incoterm-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/ca.po` & `trytond_incoterm-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/cs.po` & `trytond_incoterm-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/de.po` & `trytond_incoterm-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 msgid "To get a quote for sale \"%(sale)s\" you must enter an incoterm."
 msgstr ""
 "Um ein Angebot für Verkauf \"%(sale)s\" erstellen zu können, muss ein "
 "Incoterm erfasst werden."
 
 msgctxt "model:ir.rule.group,name:rule_group_party_incoterm_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_incoterm"
 msgid "Incoterms"
 msgstr "Incoterms"
 
 msgctxt "model:party.incoterm,name:"
 msgid "Party Incoterm"
```

### Comparing `trytond_incoterm-7.2.0/locale/es.po` & `trytond_incoterm-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/es_419.po` & `trytond_incoterm-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/et.po` & `trytond_incoterm-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/fa.po` & `trytond_incoterm-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/fi.po` & `trytond_incoterm-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/fr.po` & `trytond_incoterm-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/hu.po` & `trytond_incoterm-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/id.po` & `trytond_incoterm-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/it.po` & `trytond_incoterm-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/lo.po` & `trytond_incoterm-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/lt.po` & `trytond_incoterm-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/nl.po` & `trytond_incoterm-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/pl.po` & `trytond_incoterm-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/pt.po` & `trytond_incoterm-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/ro.po` & `trytond_incoterm-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/ru.po` & `trytond_incoterm-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/sl.po` & `trytond_incoterm-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/tr.po` & `trytond_incoterm-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/uk.po` & `trytond_incoterm-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/locale/zh_CN.po` & `trytond_incoterm-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/message.xml` & `trytond_incoterm-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/party.py` & `trytond_incoterm-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/party.xml` & `trytond_incoterm-7.2.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/purchase.py` & `trytond_incoterm-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/purchase.xml` & `trytond_incoterm-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/sale.py` & `trytond_incoterm-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/sale.xml` & `trytond_incoterm-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/setup.py` & `trytond_incoterm-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/stock.py` & `trytond_incoterm-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/stock.xml` & `trytond_incoterm-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/tests/scenario_incoterm.rst` & `trytond_incoterm-7.2.1/tests/scenario_incoterm.rst`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/tests/test_module.py` & `trytond_incoterm-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/tox.ini` & `trytond_incoterm-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/trytond_incoterm.egg-info/PKG-INFO` & `trytond_incoterm-7.2.1/trytond_incoterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_incoterm
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_incoterm-7.2.0/trytond_incoterm.egg-info/SOURCES.txt` & `trytond_incoterm-7.2.1/trytond_incoterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/view/incoterm_form.xml` & `trytond_incoterm-7.2.1/view/incoterm_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-7.2.0/view/party_incoterm_form.xml` & `trytond_incoterm-7.2.1/view/party_incoterm_form.xml`

 * *Files identical despite different names*

