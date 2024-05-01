# Comparing `tmp/trytond_sale_shipment_cost-7.0.4.tar.gz` & `tmp/trytond_sale_shipment_cost-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_cost-7.0.4.tar", last modified: Wed May  1 11:19:09 2024, max compression
+gzip compressed data, was "trytond_sale_shipment_cost-7.2.0.tar", last modified: Mon Apr 29 15:49:35 2024, max compression
```

## Comparing `trytond_sale_shipment_cost-7.0.4.tar` & `trytond_sale_shipment_cost-7.2.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.781426 trytond_sale_shipment_cost-7.0.4/
--rw-r--r--   0 ced       (1000) ced       (1000)     3723 2024-05-01 11:19:06.000000 trytond_sale_shipment_cost-7.0.4/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-05-01 11:19:06.000000 trytond_sale_shipment_cost-7.0.4/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3635 2024-05-01 11:19:09.781426 trytond_sale_shipment_cost-7.0.4/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.778091 trytond_sale_shipment_cost-7.0.4/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2797 2024-03-03 16:24:20.000000 trytond_sale_shipment_cost-7.0.4/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.778091 trytond_sale_shipment_cost-7.0.4/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4415 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4354 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4308 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3844 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4023 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4526 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4413 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3912 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3479 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4234 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3584 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3896 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3506 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3778 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3290 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1988 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18753 2024-04-27 05:19:51.000000 trytond_sale_shipment_cost-7.0.4/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:19:09.781426 trytond_sale_shipment_cost-7.0.4/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4584 2024-02-05 16:24:27.000000 trytond_sale_shipment_cost-7.0.4/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9051 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      797 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.778091 trytond_sale_shipment_cost-7.0.4/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8870 2024-04-27 05:19:48.000000 trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2024-02-05 16:24:27.000000 trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_modify_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3599 2024-02-05 16:24:27.000000 trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_promotion.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5180 2024-02-05 16:24:27.000000 trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2024-02-05 16:24:27.000000 trytond_sale_shipment_cost-7.0.4/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-03-03 12:19:24.000000 trytond_sale_shipment_cost-7.0.4/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.781426 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3635 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2277 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:10.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:19:09.000000 trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:19:09.781426 trytond_sale_shipment_cost-7.0.4/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_sale_shipment_cost-7.0.4/view/shipment_out_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.205071 trytond_sale_shipment_cost-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2024-04-29 15:26:33.000000 trytond_sale_shipment_cost-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:26:33.000000 trytond_sale_shipment_cost-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3708 2024-04-29 15:49:35.205071 trytond_sale_shipment_cost-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      869 2024-04-13 17:12:23.000000 trytond_sale_shipment_cost-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.198404 trytond_sale_shipment_cost-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:29.000000 trytond_sale_shipment_cost-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.201737 trytond_sale_shipment_cost-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4415 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4354 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4308 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3844 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4023 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4526 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4413 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3912 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3479 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4234 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3584 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3896 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3506 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3778 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3290 2024-04-27 16:43:26.000000 trytond_sale_shipment_cost-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2024-01-27 09:58:52.000000 trytond_sale_shipment_cost-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1988 2024-01-27 09:58:52.000000 trytond_sale_shipment_cost-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1179 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18953 2024-04-29 13:17:17.000000 trytond_sale_shipment_cost-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:35.205071 trytond_sale_shipment_cost-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4627 2024-04-22 12:14:36.000000 trytond_sale_shipment_cost-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9047 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.201737 trytond_sale_shipment_cost-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8937 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3193 2024-04-22 12:14:36.000000 trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_modify_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3413 2024-04-22 12:14:36.000000 trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_promotion.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5145 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-04-27 16:30:39.000000 trytond_sale_shipment_cost-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:29.000000 trytond_sale_shipment_cost-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-04-29 15:26:29.000000 trytond_sale_shipment_cost-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.201737 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3708 2024-04-29 15:49:34.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2024-04-29 15:49:35.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:34.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:49:34.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-29 15:49:34.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:34.000000 trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:35.201737 trytond_sale_shipment_cost-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-01-16 14:00:21.000000 trytond_sale_shipment_cost-7.2.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_sale_shipment_cost-7.2.0/view/shipment_out_form.xml
```

### Comparing `trytond_sale_shipment_cost-7.0.4/CHANGELOG` & `trytond_sale_shipment_cost-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,9 @@
 
-Version 7.0.4 - 2024-05-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.3 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-11-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_shipment_cost-7.0.4/COPYRIGHT` & `trytond_sale_shipment_cost-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/LICENSE` & `trytond_sale_shipment_cost-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/PKG-INFO` & `trytond_sale_shipment_cost-7.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_cost
-Version: 7.0.4
+Version: 7.2.0
 Summary: Tryton module for sale shipment cost
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
@@ -49,28 +49,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_promotion<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_promotion<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_grouping<7.3,>=7.2; extra == "test"
 
 Sale Shipment Cost Module
 #########################
 
 The sale_shipment_cost module adds shipment cost for sale.
 
 Two new fields are added to *Sale* and *Sale Configuration*:
```

### Comparing `trytond_sale_shipment_cost-7.0.4/README.rst` & `trytond_sale_shipment_cost-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/__init__.py` & `trytond_sale_shipment_cost-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/doc/conf.py` & `trytond_sale_shipment_cost-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_shipment_cost-7.0.4/doc/index.rst` & `trytond_sale_shipment_cost-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/bg.po` & `trytond_sale_shipment_cost-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/ca.po` & `trytond_sale_shipment_cost-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/cs.po` & `trytond_sale_shipment_cost-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/de.po` & `trytond_sale_shipment_cost-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/es.po` & `trytond_sale_shipment_cost-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/es_419.po` & `trytond_sale_shipment_cost-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/et.po` & `trytond_sale_shipment_cost-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/fa.po` & `trytond_sale_shipment_cost-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/fi.po` & `trytond_sale_shipment_cost-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/fr.po` & `trytond_sale_shipment_cost-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/hu.po` & `trytond_sale_shipment_cost-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/id.po` & `trytond_sale_shipment_cost-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/it.po` & `trytond_sale_shipment_cost-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/lo.po` & `trytond_sale_shipment_cost-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/lt.po` & `trytond_sale_shipment_cost-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/nl.po` & `trytond_sale_shipment_cost-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/pl.po` & `trytond_sale_shipment_cost-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/pt.po` & `trytond_sale_shipment_cost-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/ro.po` & `trytond_sale_shipment_cost-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/ru.po` & `trytond_sale_shipment_cost-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/sl.po` & `trytond_sale_shipment_cost-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/tr.po` & `trytond_sale_shipment_cost-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/uk.po` & `trytond_sale_shipment_cost-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/locale/zh_CN.po` & `trytond_sale_shipment_cost-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/message.xml` & `trytond_sale_shipment_cost-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/party.py` & `trytond_sale_shipment_cost-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/party.xml` & `trytond_sale_shipment_cost-7.2.0/party.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond_sale_shipment_cost-7.0.4/party.xml` & `trytond_sale_shipment_cost-7.2.0/party.xml`

```diff
@@ -5,19 +5,21 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_shipment_cost_method">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_shipment_cost_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_shipment_cost_method</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_shipment_cost_method_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_shipment_cost_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_shipment_cost_method</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_shipment_cost-7.0.4/sale.py` & `trytond_sale_shipment_cost-7.2.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
         shipment_cost = round_price(cost)
         cost_line = SaleLine(
             sale=self,
             sequence=sequence,
             type='line',
             product=product,
-            quantity=1,  # XXX
+            quantity=1.,  # XXX
             unit=product.sale_uom,
             shipment_cost=shipment_cost,
             )
         cost_line.on_change_product()
         if unit_price is not None:
             cost_line.unit_price = round_price(unit_price)
         else:
@@ -367,17 +367,17 @@
         cost_line.amount = cost_line.on_change_with_amount()
         return cost_line
 
     def _get_shipment_grouping_fields(self, shipment):
         pool = Pool()
         ShipmentOut = pool.get('stock.shipment.out')
         fields = super()._get_shipment_grouping_fields(shipment)
-        fields.append('carrier')
+        fields.add('carrier')
         if isinstance(shipment, ShipmentOut):
-            fields.append('cost_method')
+            fields.add('cost_method')
         return fields
 
     @property
     def shipment_cost_amount(self):
         cost = Decimal(0)
         for line in self.lines:
             if line.type == 'line' and line.shipment_cost is not None:
@@ -432,14 +432,21 @@
                     invoice_line = shipment.get_cost_invoice_line(
                         self.sale._get_invoice_sale(), origin=self)
                     if invoice_line:
                         lines.append(invoice_line)
                         shipment_cost_invoiced.append(shipment.id)
         return lines
 
+    @property
+    def _invoice_remaining_quantity(self):
+        quantity = super()._invoice_remaining_quantity
+        if self.shipment_cost is not None:
+            quantity = 0
+        return quantity
+
     def _get_invoice_line_quantity(self):
         quantity = super()._get_invoice_line_quantity()
         if self.shipment_cost is not None:
             if self.sale.shipment_cost_method == 'shipment':
                 quantity = 0
             elif (self.sale.shipment_cost_method == 'order'
                     and self.sale.invoice_method == 'shipment'):
```

### Comparing `trytond_sale_shipment_cost-7.0.4/sale.xml` & `trytond_sale_shipment_cost-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/setup.py` & `trytond_sale_shipment_cost-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     ]
-for dep in ['account', 'party', 'stock', 'sale_promotion']:
+for dep in [
+        'account', 'party', 'stock', 'sale_promotion',
+        'sale_shipment_grouping']:
     tests_require.append(get_require_version('trytond_%s' % dep))
 
 setup(name=name,
     version=version,
     description='Tryton module for sale shipment cost',
     long_description=read('README.rst'),
     author='Tryton',
```

### Comparing `trytond_sale_shipment_cost-7.0.4/stock.py` & `trytond_sale_shipment_cost-7.2.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,20 +212,20 @@
         if invoice_line:
             invoice_line.cost_shipments = [self]
         return invoice_line
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, shipments):
+    def do(cls, shipments):
         for shipment in shipments:
             shipment.cost_sale = shipment.cost_sale_used
             shipment.cost_sale_currency = shipment.cost_sale_currency_used
         cls.save(shipments)
-        super().done(shipments)
+        super().do(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('cancelled')
     def cancel(cls, shipments):
         for shipment in shipments:
             shipment.cost = None
```

### Comparing `trytond_sale_shipment_cost-7.0.4/stock.xml` & `trytond_sale_shipment_cost-7.2.0/stock.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_sale_shipment_cost-7.0.4/stock.xml` & `trytond_sale_shipment_cost-7.2.0/stock.xml`

```diff
@@ -5,14 +5,9 @@
   <data>
     <record model="ir.ui.view" id="shipment_out_view_form">
       <field name="model">stock.shipment.out</field>
       <field name="type" eval="None"/>
       <field name="inherit" ref="stock.shipment_out_view_form"/>
       <field name="name">shipment_out_form</field>
     </record>
-    <record model="ir.ui.view" id="shipment_out_view_list">
-      <field name="model">stock.shipment.out</field>
-      <field name="inherit" ref="stock.shipment_out_view_tree"/>
-      <field name="name">shipment_out_list</field>
-    </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost.rst` & `trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Sale Shipment Cost Scenario
 ===========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_shipment_cost',
     ...         'sale',
     ...         'account_invoice',
@@ -118,83 +118,80 @@
     >>> sale.shipment_cost_method
     'shipment'
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 5.0
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('3.00')
+    >>> cost_line.invoice_progress
+    1.0
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
     'processing'
     >>> sale.untaxed_amount
     Decimal('103.00')
 
 Send products::
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipment, = sale.shipments
     >>> shipment.cost_method
     'shipment'
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
     >>> shipment.cost_used
     Decimal('2.0000')
     >>> shipment.cost_sale_used
     Decimal('3.0000')
-    >>> shipment.cost_sale_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_sale_currency_used, company.currency)
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 4
     >>> shipment.cost_sale_used
     Decimal('3.0000')
-    >>> shipment.cost_sale_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_sale_currency_used, company.currency)
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_force')
     >>> shipment.state
     'assigned'
     >>> shipment.click('pick')
     >>> shipment.state
     'picked'
     >>> shipment.click('pack')
     >>> shipment.state
     'packed'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> shipment.cost_invoice_line.amount
     Decimal('3.00')
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
-    >>> sorted([l.product.id for l in invoice.lines]) == \
-    ...     sorted([product.id, carrier_product.id])
-    True
+    >>> assertEqual({l.product for l in invoice.lines},
+    ...     {product, carrier_product})
     >>> invoice.untaxed_amount
     Decimal('83.00')
 
 Send missing products::
 
     >>> sale.reload()
     >>> shipment, = [s for s in sale.shipments if s.state == 'waiting']
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> sale.reload()
     >>> len(sale.invoices)
     2
     >>> new_invoice, = [i for i in sale.invoices if i != invoice]
     >>> new_invoice.untaxed_amount
     Decimal('23.00')
 
@@ -207,32 +204,32 @@
     >>> sale.invoice_method = 'order'
     >>> sale.shipment_cost_method = 'order'
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 3.0
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('3.00')
+    >>> cost_line.invoice_progress
+    1.0
     >>> sale.click('confirm')
     >>> sale.click('process')
     >>> sale.state
     'processing'
     >>> sale.untaxed_amount
     Decimal('63.00')
 
 Check customer shipment::
 
     >>> shipment, = sale.shipments
-    >>> shipment.carrier == carrier
-    True
+    >>> assertEqual(shipment.carrier, carrier)
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
     >>> invoice.untaxed_amount
     Decimal('63.00')
@@ -277,15 +274,15 @@
 
 Send products::
 
     >>> shipment, = sale.shipments
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
@@ -321,15 +318,15 @@
     >>> shipment, = sale.shipments
     >>> shipment.cost_used
     Decimal('2.0000')
     >>> shipment.cost_sale_used
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check customer invoice::
 
     >>> sale.reload()
     >>> invoice, = sale.invoices
```

### Comparing `trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_modify_price.rst` & `trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_modify_price.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ========================================
 Sale Shipment Cost Modify Price Scenario
 ========================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_cost')
 
 Create company::
 
@@ -75,42 +75,39 @@
     >>> sale.party = customer
     >>> sale.carrier = carrier
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 5.0
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('3.00')
 
 Change the shipment cost price::
 
     >>> sale.click('draft')
     >>> cost_line = sale.lines[-1]
     >>> cost_line.unit_price = Decimal('2.00')
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('2.00')
 
 Change the carrier price reset the cost line::
 
     >>> carrier_template.list_price = Decimal('4')
     >>> carrier_template.save()
 
     >>> sale.click('draft')
     >>> sale.click('quote')
     >>> cost_line = sale.lines[-1]
-    >>> cost_line.product == carrier_product
-    True
+    >>> assertEqual(cost_line.product, carrier_product)
     >>> cost_line.quantity
     1.0
     >>> cost_line.amount
     Decimal('4.00')
```

### Comparing `trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_promotion.rst` & `trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_promotion.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 =====================================
 Sale Shipment Cost Promotion Scenario
 =====================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_shipment_cost',
     ...         'sale',
     ...         'sale_promotion',
```

### Comparing `trytond_sale_shipment_cost-7.0.4/tests/scenario_sale_shipment_cost_stock.rst` & `trytond_sale_shipment_cost-7.2.0/tests/scenario_sale_shipment_cost_stock.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 =================================
 Sale Shipment Cost Stock Scenario
 =================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_shipment_cost',
     ...         'sale',
     ...         ])
@@ -110,15 +109,15 @@
 
     >>> shipment, = sale.shipments
     >>> shipment.cost_used
     Decimal('5.0000')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.outgoing_moves
     >>> move.shipment_out_cost_price
     Decimal('5.0000')
 
 Sell product with cost on shipment::
@@ -142,15 +141,15 @@
     >>> shipment.cost_used
     Decimal('5.0000')
     >>> shipment.cost_sale_used
     Decimal('2.0000')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.outgoing_moves
     >>> move.shipment_out_cost_price
     Decimal('3.0000')
 
 Sell product with cost on order::
@@ -177,13 +176,13 @@
 
     >>> shipment, = sale.shipments
     >>> shipment.cost_used
     Decimal('5.0000')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.outgoing_moves
     >>> move.shipment_out_cost_price
     Decimal('2.0000')
```

### Comparing `trytond_sale_shipment_cost-7.0.4/tox.ini` & `trytond_sale_shipment_cost-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/PKG-INFO` & `trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_cost
-Version: 7.0.4
+Version: 7.2.0
 Summary: Tryton module for sale shipment cost
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
@@ -49,28 +49,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_promotion<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_promotion<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_grouping<7.3,>=7.2; extra == "test"
 
 Sale Shipment Cost Module
 #########################
 
 The sale_shipment_cost module adds shipment cost for sale.
 
 Two new fields are added to *Sale* and *Sale Configuration*:
```

### Comparing `trytond_sale_shipment_cost-7.0.4/trytond_sale_shipment_cost.egg-info/SOURCES.txt` & `trytond_sale_shipment_cost-7.2.0/trytond_sale_shipment_cost.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 ./tests/test_scenario.py
 ./view/configuration_form.xml
 ./view/party_form.xml
 ./view/promotion_form.xml
 ./view/sale_form.xml
 ./view/sale_line_tree_sequence.xml
 ./view/shipment_out_form.xml
-./view/shipment_out_list.xml
 doc/conf.py
 doc/index.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
@@ -107,9 +106,8 @@
 trytond_sale_shipment_cost.egg-info/requires.txt
 trytond_sale_shipment_cost.egg-info/top_level.txt
 view/configuration_form.xml
 view/party_form.xml
 view/promotion_form.xml
 view/sale_form.xml
 view/sale_line_tree_sequence.xml
-view/shipment_out_form.xml
-view/shipment_out_list.xml
+view/shipment_out_form.xml
```

### Comparing `trytond_sale_shipment_cost-7.0.4/view/sale_form.xml` & `trytond_sale_shipment_cost-7.2.0/view/sale_form.xml`

 * *Files identical despite different names*

