# Comparing `tmp/trytond_web_shop_shopify-7.2.0.tar.gz` & `tmp/trytond_web_shop_shopify-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_shopify-7.2.0.tar", last modified: Mon Apr 29 15:54:10 2024, max compression
+gzip compressed data, was "trytond_web_shop_shopify-7.2.1.tar", last modified: Wed May  1 09:50:34 2024, max compression
```

## Comparing `trytond_web_shop_shopify-7.2.0.tar` & `trytond_web_shop_shopify-7.2.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2024-04-29 15:30:01.000000 trytond_web_shop_shopify-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:01.000000 trytond_web_shop_shopify-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5698 2024-03-17 11:01:36.000000 trytond_web_shop_shopify-7.2.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.944526 trytond_web_shop_shopify-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:39.000000 trytond_web_shop_shopify-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1194 2024-04-22 12:14:37.000000 trytond_web_shop_shopify-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10401 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10685 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7596 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7584 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10331 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4150 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21497 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17230 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5034 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/shopify_retry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6221 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19751 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7351 2024-04-22 12:14:37.000000 trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:39.000000 trytond_web_shop_shopify-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-29 15:29:57.000000 trytond_web_shop_shopify-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/product_attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_stock_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_stock_location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/stock_shipment_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/stock_shipment_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28233 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4327 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.457295 trytond_web_shop_shopify-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1015 2024-05-01 09:50:31.000000 trytond_web_shop_shopify-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:50:31.000000 trytond_web_shop_shopify-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-05-01 09:50:34.457295 trytond_web_shop_shopify-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5112 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5698 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.453962 trytond_web_shop_shopify-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1194 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.453962 trytond_web_shop_shopify-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10401 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10685 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7596 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7584 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10332 2024-04-30 17:21:59.000000 trytond_web_shop_shopify-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4150 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4339 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21497 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      790 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17230 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:50:34.457295 trytond_web_shop_shopify-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5034 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/shopify_retry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6221 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2806 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.453962 trytond_web_shop_shopify-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19751 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tests/scenario_web_shop_shopify.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7351 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tests/scenario_web_shop_shopify_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:21:06.000000 trytond_web_shop_shopify-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.457295 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:50:34.000000 trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:34.457295 trytond_web_shop_shopify-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/product_attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_shopify_payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_shopify_payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_stock_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/shop_stock_location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/stock_shipment_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/view/stock_shipment_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    28233 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4327 2024-04-30 17:21:00.000000 trytond_web_shop_shopify-7.2.1/web.xml
```

### Comparing `trytond_web_shop_shopify-7.2.0/CHANGELOG` & `trytond_web_shop_shopify-7.2.1/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_web_shop_shopify-7.2.0/COPYRIGHT` & `trytond_web_shop_shopify-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/LICENSE` & `trytond_web_shop_shopify-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/PKG-INFO` & `trytond_web_shop_shopify-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 7.2.0
+Version: 7.2.1
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_shopify-7.2.0/__init__.py` & `trytond_web_shop_shopify-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/account.py` & `trytond_web_shop_shopify-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/common.py` & `trytond_web_shop_shopify-7.2.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/doc/conf.py` & `trytond_web_shop_shopify-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/doc/design.rst` & `trytond_web_shop_shopify-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/doc/usage.rst` & `trytond_web_shop_shopify-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/ir.py` & `trytond_web_shop_shopify-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/ir.xml` & `trytond_web_shop_shopify-7.2.1/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/bg.po` & `trytond_web_shop_shopify-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/ca.po` & `trytond_web_shop_shopify-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/cs.po` & `trytond_web_shop_shopify-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/de.po` & `trytond_web_shop_shopify-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/es.po` & `trytond_web_shop_shopify-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/es_419.po` & `trytond_web_shop_shopify-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/et.po` & `trytond_web_shop_shopify-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/fa.po` & `trytond_web_shop_shopify-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/fi.po` & `trytond_web_shop_shopify-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/fr.po` & `trytond_web_shop_shopify-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/hu.po` & `trytond_web_shop_shopify-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/id.po` & `trytond_web_shop_shopify-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/it.po` & `trytond_web_shop_shopify-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/lo.po` & `trytond_web_shop_shopify-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/lt.po` & `trytond_web_shop_shopify-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/nl.po` & `trytond_web_shop_shopify-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 msgstr "Elke Shopify-locatie kan slechts aan één magazijn worden gekoppeld."
 
 msgctxt "model:ir.message,text:msg_product_change_template"
 msgid ""
 "To change the template of product \"%(product)s\" you must unpublish it from"
 " the Shopify web shops."
 msgstr ""
-"Om het sjabloon van het artikel \"%(product)\" te kunnen bewerken, moet de "
+"Om het sjabloon van het artikel \"%(product)s\" te kunnen bewerken, moet de "
 "publicatie in de Shopfiy webshop eerst worden ingetrokken."
 
 msgctxt "model:ir.message,text:msg_product_fail"
 msgid ""
 "Failed to save product \"%(template)s\" with error:\n"
 "%(error)s"
 msgstr ""
```

### Comparing `trytond_web_shop_shopify-7.2.0/locale/pl.po` & `trytond_web_shop_shopify-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/pt.po` & `trytond_web_shop_shopify-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/ro.po` & `trytond_web_shop_shopify-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/ru.po` & `trytond_web_shop_shopify-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/sl.po` & `trytond_web_shop_shopify-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/tr.po` & `trytond_web_shop_shopify-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/uk.po` & `trytond_web_shop_shopify-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/locale/zh_CN.po` & `trytond_web_shop_shopify-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/message.xml` & `trytond_web_shop_shopify-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/party.py` & `trytond_web_shop_shopify-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/product.py` & `trytond_web_shop_shopify-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/product.xml` & `trytond_web_shop_shopify-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/routes.py` & `trytond_web_shop_shopify-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/sale.py` & `trytond_web_shop_shopify-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/setup.py` & `trytond_web_shop_shopify-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/shopify_retry.py` & `trytond_web_shop_shopify-7.2.1/shopify_retry.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/stock.py` & `trytond_web_shop_shopify-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/stock.xml` & `trytond_web_shop_shopify-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify.rst` & `trytond_web_shop_shopify-7.2.1/tests/scenario_web_shop_shopify.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify_secondary_unit.rst` & `trytond_web_shop_shopify-7.2.1/tests/scenario_web_shop_shopify_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/tox.ini` & `trytond_web_shop_shopify-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/PKG-INFO` & `trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 7.2.0
+Version: 7.2.1
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/SOURCES.txt` & `trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/requires.txt` & `trytond_web_shop_shopify-7.2.1/trytond_web_shop_shopify.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/view/shop_form.xml` & `trytond_web_shop_shopify-7.2.1/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/web.py` & `trytond_web_shop_shopify-7.2.1/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.2.0/web.xml` & `trytond_web_shop_shopify-7.2.1/web.xml`

 * *Files identical despite different names*

