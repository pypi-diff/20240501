# Comparing `tmp/trytond_purchase_blanket_agreement-7.2.0.tar.gz` & `tmp/trytond_purchase_blanket_agreement-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_blanket_agreement-7.2.0.tar", last modified: Mon Apr 29 15:45:40 2024, max compression
+gzip compressed data, was "trytond_purchase_blanket_agreement-7.2.1.tar", last modified: Wed May  1 11:36:50 2024, max compression
```

## Comparing `trytond_purchase_blanket_agreement-7.2.0.tar` & `trytond_purchase_blanket_agreement-7.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2024-04-29 15:23:34.000000 trytond_purchase_blanket_agreement-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-29 15:23:34.000000 trytond_purchase_blanket_agreement-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.261215 trytond_purchase_blanket_agreement-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:20.000000 trytond_purchase_blanket_agreement-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.261215 trytond_purchase_blanket_agreement-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7774 2024-04-27 16:43:26.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7827 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7838 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7784 2024-04-27 16:43:26.000000 trytond_purchase_blanket_agreement-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6718 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7900 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-27 16:43:25.000000 trytond_purchase_blanket_agreement-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32617 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11915 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4824 2024-04-27 16:30:39.000000 trytond_purchase_blanket_agreement-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5537 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/tests/scenario_purchase_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-22 12:14:36.000000 trytond_purchase_blanket_agreement-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:20.000000 trytond_purchase_blanket_agreement-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-29 15:23:30.000000 trytond_purchase_blanket_agreement-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2405 2024-04-29 15:45:40.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:39.000000 trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:40.264549 trytond_purchase_blanket_agreement-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_create_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_purchase_blanket_agreement-7.2.0/view/purchase_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-05-01 11:36:46.000000 trytond_purchase_blanket_agreement-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-05-01 11:36:46.000000 trytond_purchase_blanket_agreement-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7777 2024-04-30 17:21:59.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7827 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7838 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7784 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6718 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7900 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32617 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11915 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4824 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5537 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/scenario_purchase_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-30 17:21:06.000000 trytond_purchase_blanket_agreement-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2405 2024-05-01 11:36:50.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_create_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1608 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_line_list.xml
```

### Comparing `trytond_purchase_blanket_agreement-7.2.0/COPYRIGHT` & `trytond_purchase_blanket_agreement-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/LICENSE` & `trytond_purchase_blanket_agreement-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_blanket_agreement-7.2.0/__init__.py` & `trytond_purchase_blanket_agreement-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/doc/conf.py` & `trytond_purchase_blanket_agreement-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/doc/design.rst` & `trytond_purchase_blanket_agreement-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/bg.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/ca.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -178,16 +178,16 @@
 "compatible amb les línies de compra existents."
 
 msgctxt "model:ir.message,text:msg_quantity_greater_remaining"
 msgid ""
 "The quantity of line \"%(line)s\" is greater than the remaining quantity "
 "(%(remaining)s) of agreement \"%(agreement)s\"."
 msgstr ""
-"La quantitat de la línia \"%(line)s\" es superior a la quantitat restant "
-"(%remaining)s\" de l'acord \"%(agreement)s\"."
+"La quantitat de la línia \"%(line)s\" és superior a la quantitat restant "
+"(%(remaining)s\") de l'acord \"%(agreement)s\"."
 
 msgctxt ""
 "model:ir.model.button,string:purchase_blanket_agreement_cancel_button"
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgctxt "model:ir.model.button,string:purchase_blanket_agreement_close_button"
```

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/cs.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/de.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/es.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/es_419.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/et.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/fa.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/fi.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/fr.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/hu.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/id.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/it.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/lo.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/lt.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/nl.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/pl.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/pt.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/ro.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/ru.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/sl.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/tr.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/uk.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/locale/zh_CN.po` & `trytond_purchase_blanket_agreement-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/message.xml` & `trytond_purchase_blanket_agreement-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/product.xml` & `trytond_purchase_blanket_agreement-7.2.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/purchase.py` & `trytond_purchase_blanket_agreement-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/purchase.xml` & `trytond_purchase_blanket_agreement-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/setup.py` & `trytond_purchase_blanket_agreement-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/tests/scenario_purchase_blanket_agreement.rst` & `trytond_purchase_blanket_agreement-7.2.1/tests/scenario_purchase_blanket_agreement.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/tox.ini` & `trytond_purchase_blanket_agreement-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_blanket_agreement-7.2.0/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt` & `trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_form.xml` & `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_form.xml` & `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.0/view/purchase_blanket_agreement_line_list.xml` & `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_list.xml`

 * *Files identical despite different names*

