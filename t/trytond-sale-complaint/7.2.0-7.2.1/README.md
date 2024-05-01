# Comparing `tmp/trytond_sale_complaint-7.2.0.tar.gz` & `tmp/trytond_sale_complaint-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_complaint-7.2.0.tar", last modified: Mon Apr 29 15:47:30 2024, max compression
+gzip compressed data, was "trytond_sale_complaint-7.2.1.tar", last modified: Wed May  1 11:24:23 2024, max compression
```

## Comparing `trytond_sale_complaint-7.2.0.tar` & `trytond_sale_complaint-7.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2024-04-29 15:24:52.000000 trytond_sale_complaint-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:24:51.000000 trytond_sale_complaint-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28911 2024-04-22 12:14:36.000000 trytond_sale_complaint-7.2.0/complaint.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13169 2024-04-27 16:30:39.000000 trytond_sale_complaint-7.2.0/complaint.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.271671 trytond_sale_complaint-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_complaint-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:24.000000 trytond_sale_complaint-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.271671 trytond_sale_complaint-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/icons/tryton-sale-complaint.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9498 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9554 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8621 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9459 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9570 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8160 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9292 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9987 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9478 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9471 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8811 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9385 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9692 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8690 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9351 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8999 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9509 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9589 2024-04-29 13:17:17.000000 trytond_sale_complaint-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9503 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9231 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8049 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8782 2024-04-27 16:43:26.000000 trytond_sale_complaint-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-01-27 09:58:52.000000 trytond_sale_complaint-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2024-03-17 11:01:36.000000 trytond_sale_complaint-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8106 2024-04-22 12:14:36.000000 trytond_sale_complaint-7.2.0/tests/scenario_sale_complaint.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:24.000000 trytond_sale_complaint-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:24:47.000000 trytond_sale_complaint-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.278338 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2141 2024-04-29 15:47:30.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:29.000000 trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:30.275005 trytond_sale_complaint-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/action_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-01-27 09:58:52.000000 trytond_sale_complaint-7.2.0/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/complaint_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/complaint_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_sale_complaint-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_sale_complaint-7.2.0/view/type_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-05-01 11:24:20.000000 trytond_sale_complaint-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:24:20.000000 trytond_sale_complaint-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28911 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/complaint.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13169 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/complaint.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.851805 trytond_sale_complaint-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.851805 trytond_sale_complaint-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/icons/tryton-sale-complaint.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9498 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9554 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8621 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9459 2024-04-30 17:21:59.000000 trytond_sale_complaint-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9570 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8160 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9292 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9987 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9478 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9471 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8811 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9385 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9692 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8690 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9345 2024-04-30 17:21:59.000000 trytond_sale_complaint-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8999 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9509 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9589 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9503 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9231 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8608 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8049 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8782 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4460 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8106 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/tests/scenario_sale_complaint.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-30 17:21:06.000000 trytond_sale_complaint-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2141 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:24:23.000000 trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:24:23.855139 trytond_sale_complaint-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/action_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/action_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/complaint_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/complaint_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond_sale_complaint-7.2.1/view/type_list.xml
```

### Comparing `trytond_sale_complaint-7.2.0/CHANGELOG` & `trytond_sale_complaint-7.2.1/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_sale_complaint-7.2.0/COPYRIGHT` & `trytond_sale_complaint-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/LICENSE` & `trytond_sale_complaint-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/PKG-INFO` & `trytond_sale_complaint-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_complaint
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale complaint
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_complaint-7.2.0/README.rst` & `trytond_sale_complaint-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/__init__.py` & `trytond_sale_complaint-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/complaint.py` & `trytond_sale_complaint-7.2.1/complaint.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/complaint.xml` & `trytond_sale_complaint-7.2.1/complaint.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/doc/conf.py` & `trytond_sale_complaint-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/doc/index.rst` & `trytond_sale_complaint-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/icons/LICENSE` & `trytond_sale_complaint-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/bg.po` & `trytond_sale_complaint-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/ca.po` & `trytond_sale_complaint-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/cs.po` & `trytond_sale_complaint-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/de.po` & `trytond_sale_complaint-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
 msgctxt "model:ir.model.button,string:complaint_wait_button"
 msgid "Wait"
 msgstr "Warten"
 
 msgctxt "model:ir.rule.group,name:rule_group_complaint_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_complaint"
 msgid "Customer Complaint"
 msgstr "Kundenreklamation"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_complaint"
 msgid "Customer Complaint"
```

### Comparing `trytond_sale_complaint-7.2.0/locale/es.po` & `trytond_sale_complaint-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/es_419.po` & `trytond_sale_complaint-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/et.po` & `trytond_sale_complaint-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/fa.po` & `trytond_sale_complaint-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/fi.po` & `trytond_sale_complaint-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/fr.po` & `trytond_sale_complaint-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/hu.po` & `trytond_sale_complaint-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/id.po` & `trytond_sale_complaint-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/it.po` & `trytond_sale_complaint-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/lo.po` & `trytond_sale_complaint-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/lt.po` & `trytond_sale_complaint-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/nl.po` & `trytond_sale_complaint-7.2.1/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,16 @@
 msgid "You cannot delete action \"%(action)s\" because it has a result."
 msgstr ""
 "U kunt actie \"%(action)s\" niet verwijderen omdat deze een resultaat heeft."
 
 msgctxt "model:ir.message,text:msg_complaint_delete_draft"
 msgid "To delete complaint \"%(complaint)s\" you must reset it to draft state."
 msgstr ""
-"Om de klacht \"% (klacht) s\" te verwijderen, moet u deze tergugzetten naar "
-"conceptstatus."
+"Om de klacht \"%(complaint)s\" te verwijderen, moet u deze terugzetten naar "
+"concept."
 
 msgctxt "model:ir.model.button,string:complaint_approve_button"
 msgid "Approve"
 msgstr "Goedkeuren"
 
 msgctxt "model:ir.model.button,string:complaint_cancel_button"
 msgid "Cancel"
```

### Comparing `trytond_sale_complaint-7.2.0/locale/pl.po` & `trytond_sale_complaint-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/pt.po` & `trytond_sale_complaint-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/ro.po` & `trytond_sale_complaint-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/ru.po` & `trytond_sale_complaint-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/sl.po` & `trytond_sale_complaint-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/tr.po` & `trytond_sale_complaint-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/uk.po` & `trytond_sale_complaint-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/locale/zh_CN.po` & `trytond_sale_complaint-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/message.xml` & `trytond_sale_complaint-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/sale.py` & `trytond_sale_complaint-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/sale.xml` & `trytond_sale_complaint-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/setup.py` & `trytond_sale_complaint-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/tests/scenario_sale_complaint.rst` & `trytond_sale_complaint-7.2.1/tests/scenario_sale_complaint.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/tox.ini` & `trytond_sale_complaint-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/PKG-INFO` & `trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_complaint
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for sale complaint
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_complaint-7.2.0/trytond_sale_complaint.egg-info/SOURCES.txt` & `trytond_sale_complaint-7.2.1/trytond_sale_complaint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/view/action_form.xml` & `trytond_sale_complaint-7.2.1/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/view/complaint_form.xml` & `trytond_sale_complaint-7.2.1/view/complaint_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-7.2.0/view/complaint_list.xml` & `trytond_sale_complaint-7.2.1/view/complaint_list.xml`

 * *Files identical despite different names*

