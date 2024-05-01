# Comparing `tmp/trytond_sale_blanket_agreement-7.2.0.tar.gz` & `tmp/trytond_sale_blanket_agreement-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_blanket_agreement-7.2.0.tar", last modified: Mon Apr 29 15:47:24 2024, max compression
+gzip compressed data, was "trytond_sale_blanket_agreement-7.2.1.tar", last modified: Wed May  1 11:25:20 2024, max compression
```

## Comparing `trytond_sale_blanket_agreement-7.2.0.tar` & `trytond_sale_blanket_agreement-7.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:24:47.000000 trytond_sale_blanket_agreement-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-29 15:24:46.000000 trytond_sale_blanket_agreement-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.511822 trytond_sale_blanket_agreement-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:24.000000 trytond_sale_blanket_agreement-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7252 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7340 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7328 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7290 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6186 2024-04-29 13:17:17.000000 trytond_sale_blanket_agreement-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7397 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-27 16:43:26.000000 trytond_sale_blanket_agreement-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    29320 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11419 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:24.518489 trytond_sale_blanket_agreement-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4732 2024-04-27 16:30:39.000000 trytond_sale_blanket_agreement-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5183 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/tests/scenario_sale_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-22 12:14:36.000000 trytond_sale_blanket_agreement-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:24.000000 trytond_sale_blanket_agreement-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:24:42.000000 trytond_sale_blanket_agreement-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2281 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:24.000000 trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:24.515155 trytond_sale_blanket_agreement-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_create_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-7.2.0/view/sale_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.383660 trytond_sale_blanket_agreement-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-05-01 11:25:17.000000 trytond_sale_blanket_agreement-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-05-01 11:25:16.000000 trytond_sale_blanket_agreement-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-05-01 11:25:20.383660 trytond_sale_blanket_agreement-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.376994 trytond_sale_blanket_agreement-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.380327 trytond_sale_blanket_agreement-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7255 2024-04-30 17:21:59.000000 trytond_sale_blanket_agreement-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7340 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7328 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7290 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6186 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7397 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6148 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    29320 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11419 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:25:20.383660 trytond_sale_blanket_agreement-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4732 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.380327 trytond_sale_blanket_agreement-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/tests/scenario_sale_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-30 17:21:06.000000 trytond_sale_blanket_agreement-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.380327 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2709 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2281 2024-05-01 11:25:20.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:25:19.000000 trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:25:20.380327 trytond_sale_blanket_agreement-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_create_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond_sale_blanket_agreement-7.2.1/view/sale_line_list.xml
```

### Comparing `trytond_sale_blanket_agreement-7.2.0/COPYRIGHT` & `trytond_sale_blanket_agreement-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/LICENSE` & `trytond_sale_blanket_agreement-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/PKG-INFO` & `trytond_sale_blanket_agreement-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_blanket_agreement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_blanket_agreement-7.2.0/__init__.py` & `trytond_sale_blanket_agreement-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/doc/conf.py` & `trytond_sale_blanket_agreement-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/doc/design.rst` & `trytond_sale_blanket_agreement-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/bg.po` & `trytond_sale_blanket_agreement-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/ca.po` & `trytond_sale_blanket_agreement-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,16 @@
 "compatible amb les línies de venda existents."
 
 msgctxt "model:ir.message,text:msg_quantity_greater_remaining"
 msgid ""
 "The quantity of line \"%(line)s\" is greater than the remaining quantity "
 "(%(remaining)s) of agreement \"%(agreement)s\"."
 msgstr ""
-"La quantitat de la línia \"%(line)s\" es superior a la quantitat restant "
-"(%remaining)s\" de l'acord \"%(agreement)s\"."
+"La quantitat de la línia \"%(line)s\" és superior a la quantitat restant "
+"(%(remaining)s\") de l'acord \"%(agreement)s\"."
 
 msgctxt "model:ir.model.button,string:sale_blanket_agreement_cancel_button"
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:sale_blanket_agreement_close_button"
 msgid "Close"
```

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/cs.po` & `trytond_sale_blanket_agreement-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/de.po` & `trytond_sale_blanket_agreement-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/es.po` & `trytond_sale_blanket_agreement-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/es_419.po` & `trytond_sale_blanket_agreement-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/et.po` & `trytond_sale_blanket_agreement-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/fa.po` & `trytond_sale_blanket_agreement-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/fi.po` & `trytond_sale_blanket_agreement-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/fr.po` & `trytond_sale_blanket_agreement-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/hu.po` & `trytond_sale_blanket_agreement-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/id.po` & `trytond_sale_blanket_agreement-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/it.po` & `trytond_sale_blanket_agreement-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/lo.po` & `trytond_sale_blanket_agreement-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/lt.po` & `trytond_sale_blanket_agreement-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/nl.po` & `trytond_sale_blanket_agreement-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/pl.po` & `trytond_sale_blanket_agreement-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/pt.po` & `trytond_sale_blanket_agreement-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/ro.po` & `trytond_sale_blanket_agreement-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/ru.po` & `trytond_sale_blanket_agreement-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/sl.po` & `trytond_sale_blanket_agreement-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/tr.po` & `trytond_sale_blanket_agreement-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/uk.po` & `trytond_sale_blanket_agreement-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/locale/zh_CN.po` & `trytond_sale_blanket_agreement-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/message.xml` & `trytond_sale_blanket_agreement-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/product.xml` & `trytond_sale_blanket_agreement-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/sale.py` & `trytond_sale_blanket_agreement-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/sale.xml` & `trytond_sale_blanket_agreement-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/setup.py` & `trytond_sale_blanket_agreement-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/tests/scenario_sale_blanket_agreement.rst` & `trytond_sale_blanket_agreement-7.2.1/tests/scenario_sale_blanket_agreement.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/tox.ini` & `trytond_sale_blanket_agreement-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO` & `trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_blanket_agreement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_blanket_agreement-7.2.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt` & `trytond_sale_blanket_agreement-7.2.1/trytond_sale_blanket_agreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_form.xml` & `trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-7.2.0/view/sale_blanket_agreement_line_form.xml` & `trytond_sale_blanket_agreement-7.2.1/view/sale_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

