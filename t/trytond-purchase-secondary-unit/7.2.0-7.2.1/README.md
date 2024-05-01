# Comparing `tmp/trytond_purchase_secondary_unit-7.2.0.tar.gz` & `tmp/trytond_purchase_secondary_unit-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_secondary_unit-7.2.0.tar", last modified: Mon Apr 29 15:46:33 2024, max compression
+gzip compressed data, was "trytond_purchase_secondary_unit-7.2.1.tar", last modified: Wed May  1 11:32:48 2024, max compression
```

## Comparing `trytond_purchase_secondary_unit-7.2.0.tar` & `trytond_purchase_secondary_unit-7.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      998 2024-04-29 15:24:16.000000 trytond_purchase_secondary_unit-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:24:15.000000 trytond_purchase_secondary_unit-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      852 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1225 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.073167 trytond_purchase_secondary_unit-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_purchase_secondary_unit-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_secondary_unit-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6851 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6884 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6855 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6917 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6988 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6694 2024-03-17 11:01:36.000000 trytond_purchase_secondary_unit-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-02-04 18:51:26.000000 trytond_purchase_secondary_unit-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4750 2024-03-17 11:01:36.000000 trytond_purchase_secondary_unit-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_requisition_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3987 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_secondary_unit-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-29 15:24:11.000000 trytond_purchase_secondary_unit-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2186 2024-04-29 15:46:33.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/stock_move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.388610 trytond_purchase_secondary_unit-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1099 2024-05-01 11:32:45.000000 trytond_purchase_secondary_unit-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:32:44.000000 trytond_purchase_secondary_unit-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-05-01 11:32:48.388610 trytond_purchase_secondary_unit-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      852 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1225 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.381943 trytond_purchase_secondary_unit-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.385276 trytond_purchase_secondary_unit-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6827 2024-04-30 17:21:59.000000 trytond_purchase_secondary_unit-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6857 2024-04-30 17:21:59.000000 trytond_purchase_secondary_unit-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6828 2024-04-30 17:21:59.000000 trytond_purchase_secondary_unit-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6917 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-04-30 17:21:59.000000 trytond_purchase_secondary_unit-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6694 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:32:48.388610 trytond_purchase_secondary_unit-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4750 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.385276 trytond_purchase_secondary_unit-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_requisition_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3987 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-30 17:21:06.000000 trytond_purchase_secondary_unit-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.385276 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2186 2024-05-01 11:32:48.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:32:47.000000 trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:48.385276 trytond_purchase_secondary_unit-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      723 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond_purchase_secondary_unit-7.2.1/view/stock_move_list.xml
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/CHANGELOG` & `trytond_purchase_secondary_unit-7.2.1/CHANGELOG`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_purchase_secondary_unit-7.2.0/COPYRIGHT` & `trytond_purchase_secondary_unit-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/LICENSE` & `trytond_purchase_secondary_unit-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/PKG-INFO` & `trytond_purchase_secondary_unit-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_secondary_unit
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add a secondary unit on purchase line
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/__init__.py` & `trytond_purchase_secondary_unit-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/account.py` & `trytond_purchase_secondary_unit-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/doc/conf.py` & `trytond_purchase_secondary_unit-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/bg.po` & `trytond_purchase_secondary_unit-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/ca.po` & `trytond_purchase_secondary_unit-7.2.1/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Rati UdM de compra secundaria"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Categoria de la UdM secundaria del producte"
 
-#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "La unitat de mesura secundaria de les compres."
+msgstr "La unitat de mesura secundària de les compres."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "El coeficient de la formula:\n"
@@ -104,18 +103,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "El coeficient de la formula:\n"
 "coeficent (unitat_compra) = 1 (unitat_secundaria)"
 
-#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "La unitat de mesura secundaria de les compres."
+msgstr "La unitat de mesura secundària de les compres."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "El coeficient de la formula:\n"
@@ -145,18 +143,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "El rati de la unitat de mesura secundaria."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "La categoria de la unitat de mesura per defecte."
 
-#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "La unitat de mesura secundaria de les compres."
+msgstr "La unitat de mesura secundària de les compres."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "El coeficient de la formula:\n"
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/cs.po` & `trytond_purchase_secondary_unit-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/de.po` & `trytond_purchase_secondary_unit-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Einkauf Zweitmaßeinheit Kehrwert Faktor"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Artikel Zweitmaßeinheitenkategorie"
 
-#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
@@ -104,15 +103,14 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "Der Koeffizient für die Formel:\n"
 "Koeffizient(Einkaufseinheit) = 1 (Zweitmaßeinheit)"
 
-#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
@@ -145,15 +143,14 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "Der Kehrwert Faktor für die zweite Maßeinheit."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "Die Kategorie für die Standardmaßeinheit."
 
-#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/es.po` & `trytond_purchase_secondary_unit-7.2.1/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Ratio UdM compra secundaria"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Categoría de la UdM secundaria del producto"
 
-#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
@@ -104,15 +103,14 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "El coeficiente de la fórmula:\n"
 "coeficiente (unidad_compra) = 1 (unidad secundaria)"
 
-#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
@@ -145,15 +143,14 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "El ratio de la unidad de medida secundaria."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "La categoría de la unidad de medida por defecto."
 
-#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/es_419.po` & `trytond_purchase_secondary_unit-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/et.po` & `trytond_purchase_secondary_unit-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/fa.po` & `trytond_purchase_secondary_unit-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/fi.po` & `trytond_purchase_secondary_unit-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/fr.po` & `trytond_purchase_secondary_unit-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/hu.po` & `trytond_purchase_secondary_unit-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/id.po` & `trytond_purchase_secondary_unit-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/it.po` & `trytond_purchase_secondary_unit-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/lo.po` & `trytond_purchase_secondary_unit-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/lt.po` & `trytond_purchase_secondary_unit-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/nl.po` & `trytond_purchase_secondary_unit-7.2.1/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Inkoop secundaire maateenheid verhouding"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Product secundaire maateenheid categorie"
 
-#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "De tweede maateenheid voor inkopen."
+msgstr "De secundaire maateenheid voor inkopen."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "De coëfficiënt voor de formule:\n"
@@ -104,18 +103,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "De coëfficiënt voor de formule:\n"
 "coëfficiënt (inkoopeenheid) = 1 (secundaire eenheid)"
 
-#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "De tweede maateenheid voor inkopen."
+msgstr "De secundaire maateenheid voor inkopen."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "De coëfficiënt voor de formule:\n"
@@ -145,18 +143,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "De verhouding voor de secundaire maateenheid."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "De categorie van de standaard maateenheid."
 
-#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
 msgid "The secondary Unit of Measure for purchases."
-msgstr "De tweede maateenheid voor inkopen."
+msgstr "De secundaire maateenheid voor inkopen."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "De coëfficiënt voor de formule:\n"
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/pl.po` & `trytond_purchase_secondary_unit-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/pt.po` & `trytond_purchase_secondary_unit-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/ro.po` & `trytond_purchase_secondary_unit-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/ru.po` & `trytond_purchase_secondary_unit-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/sl.po` & `trytond_purchase_secondary_unit-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/tr.po` & `trytond_purchase_secondary_unit-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/uk.po` & `trytond_purchase_secondary_unit-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/locale/zh_CN.po` & `trytond_purchase_secondary_unit-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/product.py` & `trytond_purchase_secondary_unit-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/product.xml` & `trytond_purchase_secondary_unit-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/purchase.py` & `trytond_purchase_secondary_unit-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/purchase.xml` & `trytond_purchase_secondary_unit-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/setup.py` & `trytond_purchase_secondary_unit-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/stock.py` & `trytond_purchase_secondary_unit-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_blanket_agreement_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_requisition_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_requisition_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.1/tests/scenario_purchase_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/tox.ini` & `trytond_purchase_secondary_unit-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO` & `trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_secondary_unit
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add a secondary unit on purchase line
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt` & `trytond_purchase_secondary_unit-7.2.1/trytond_purchase_secondary_unit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/view/product_supplier_form.xml` & `trytond_purchase_secondary_unit-7.2.1/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/view/product_template_form.xml` & `trytond_purchase_secondary_unit-7.2.1/view/product_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.2.0/view/purchase_line_form.xml` & `trytond_purchase_secondary_unit-7.2.1/view/purchase_line_form.xml`

 * *Files identical despite different names*

