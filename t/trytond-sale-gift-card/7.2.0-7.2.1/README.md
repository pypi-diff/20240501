# Comparing `tmp/trytond_sale_gift_card-7.2.0.tar.gz` & `tmp/trytond_sale_gift_card-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_gift_card-7.2.0.tar", last modified: Mon Apr 29 15:47:56 2024, max compression
+gzip compressed data, was "trytond_sale_gift_card-7.2.1.tar", last modified: Wed May  1 11:23:38 2024, max compression
```

## Comparing `trytond_sale_gift_card-7.2.0.tar` & `trytond_sale_gift_card-7.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-29 15:25:12.000000 trytond_sale_gift_card-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:25:12.000000 trytond_sale_gift_card-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.700980 trytond_sale_gift_card-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:25.000000 trytond_sale_gift_card-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1042 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      553 2024-02-04 18:51:26.000000 trytond_sale_gift_card-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30315 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/gift_card.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.704314 trytond_sale_gift_card-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7601 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7486 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7370 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5993 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5952 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7160 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5953 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-27 16:43:26.000000 trytond_sale_gift_card-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2024-02-04 18:51:26.000000 trytond_sale_gift_card-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2459 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18775 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7817 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4595 2024-03-17 11:01:36.000000 trytond_sale_gift_card-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.704314 trytond_sale_gift_card-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5320 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3655 2024-04-27 16:30:39.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card_goods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-22 12:14:36.000000 trytond_sale_gift_card-7.2.0/tests/scenario_sale_point_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:25.000000 trytond_sale_gift_card-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-29 15:25:07.000000 trytond_sale_gift_card-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:56.000000 trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:56.707647 trytond_sale_gift_card-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/account_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/gift_card_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/sale_point_sale_pay_gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-7.2.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.446326 trytond_sale_gift_card-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      955 2024-05-01 11:23:35.000000 trytond_sale_gift_card-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:23:34.000000 trytond_sale_gift_card-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-05-01 11:23:38.446326 trytond_sale_gift_card-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1081 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.442993 trytond_sale_gift_card-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1042 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      553 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30315 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/gift_card.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.442993 trytond_sale_gift_card-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7467 2024-04-30 17:21:59.000000 trytond_sale_gift_card-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7601 2024-04-30 17:21:59.000000 trytond_sale_gift_card-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7486 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7370 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5993 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5952 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7160 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5953 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5939 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2459 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18775 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7817 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:23:38.446326 trytond_sale_gift_card-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4595 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2009 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.442993 trytond_sale_gift_card-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5320 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/scenario_sale_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3655 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/scenario_sale_gift_card_goods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/scenario_sale_point_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-30 17:21:06.000000 trytond_sale_gift_card-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.446326 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2844 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-05-01 11:23:38.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:23:37.000000 trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:23:38.446326 trytond_sale_gift_card-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      509 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/account_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/gift_card_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/sale_point_sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/sale_point_sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/sale_point_sale_pay_gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_gift_card-7.2.1/view/template_form.xml
```

### Comparing `trytond_sale_gift_card-7.2.0/CHANGELOG` & `trytond_sale_gift_card-7.2.1/CHANGELOG`

 * *Files 15% similar despite different names*

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

### Comparing `trytond_sale_gift_card-7.2.0/COPYRIGHT` & `trytond_sale_gift_card-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/LICENSE` & `trytond_sale_gift_card-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/PKG-INFO` & `trytond_sale_gift_card-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_gift_card
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage gift cards
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_gift_card-7.2.0/__init__.py` & `trytond_sale_gift_card-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/account.py` & `trytond_sale_gift_card-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/account.xml` & `trytond_sale_gift_card-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/doc/conf.py` & `trytond_sale_gift_card-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/doc/design.rst` & `trytond_sale_gift_card-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/doc/usage.rst` & `trytond_sale_gift_card-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/email.html` & `trytond_sale_gift_card-7.2.1/email.html`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/exceptions.py` & `trytond_sale_gift_card-7.2.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/gift_card.fodt` & `trytond_sale_gift_card-7.2.1/gift_card.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/bg.po` & `trytond_sale_gift_card-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/ca.po` & `trytond_sale_gift_card-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
 msgctxt "report:sale.gift_card.email:"
 msgid "Here is your code:"
 msgstr "Aquí teniu el vostre codi:"
 
 msgctxt "report:sale.gift_card.email:"
 msgid "You received a gift card of %(value)s for %(company)s."
-msgstr "Heu rebut una targeta regal de %(valor)s de l'empresa %(company)s."
+msgstr "Heu rebut una targeta regal de %(value)s de l'empresa %(company)s."
 
 msgctxt "report:sale.gift_card:"
 msgid "Value:"
 msgstr "Valor:"
 
 msgctxt "view:account.configuration:"
 msgid "Gift Card"
```

### Comparing `trytond_sale_gift_card-7.2.0/locale/cs.po` & `trytond_sale_gift_card-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/de.po` & `trytond_sale_gift_card-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 msgctxt "model:ir.message,text:msg_gift_card_number_unique"
 msgid "The numbers for each company's gift cards must be unique."
 msgstr ""
 "Die Nummer für jeden Geschenkgutschein des Unternehmens muss eindeutig sein."
 
 msgctxt "model:ir.rule.group,name:rule_group_gift_card_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_gift_card"
 msgid "Gift Card"
 msgstr "Geschenkgutschein"
 
 msgctxt "model:ir.ui.menu,name:menu_gift_card_form"
 msgid "Gift Cards"
```

### Comparing `trytond_sale_gift_card-7.2.0/locale/es.po` & `trytond_sale_gift_card-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/es_419.po` & `trytond_sale_gift_card-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/et.po` & `trytond_sale_gift_card-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/fa.po` & `trytond_sale_gift_card-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/fi.po` & `trytond_sale_gift_card-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/fr.po` & `trytond_sale_gift_card-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/hu.po` & `trytond_sale_gift_card-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/id.po` & `trytond_sale_gift_card-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/it.po` & `trytond_sale_gift_card-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/lo.po` & `trytond_sale_gift_card-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/lt.po` & `trytond_sale_gift_card-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/nl.po` & `trytond_sale_gift_card-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/pl.po` & `trytond_sale_gift_card-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/pt.po` & `trytond_sale_gift_card-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/ro.po` & `trytond_sale_gift_card-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/ru.po` & `trytond_sale_gift_card-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/sl.po` & `trytond_sale_gift_card-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/tr.po` & `trytond_sale_gift_card-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/uk.po` & `trytond_sale_gift_card-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/locale/zh_CN.po` & `trytond_sale_gift_card-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/message.xml` & `trytond_sale_gift_card-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/product.py` & `trytond_sale_gift_card-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/sale.py` & `trytond_sale_gift_card-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/sale.xml` & `trytond_sale_gift_card-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/setup.py` & `trytond_sale_gift_card-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/stock.py` & `trytond_sale_gift_card-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card.rst` & `trytond_sale_gift_card-7.2.1/tests/scenario_sale_gift_card.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/tests/scenario_sale_gift_card_goods.rst` & `trytond_sale_gift_card-7.2.1/tests/scenario_sale_gift_card_goods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/tests/scenario_sale_point_gift_card.rst` & `trytond_sale_gift_card-7.2.1/tests/scenario_sale_point_gift_card.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/tox.ini` & `trytond_sale_gift_card-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/PKG-INFO` & `trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_gift_card
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to manage gift cards
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_gift_card-7.2.0/trytond_sale_gift_card.egg-info/SOURCES.txt` & `trytond_sale_gift_card-7.2.1/trytond_sale_gift_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-7.2.0/view/gift_card_form.xml` & `trytond_sale_gift_card-7.2.1/view/gift_card_form.xml`

 * *Files identical despite different names*

