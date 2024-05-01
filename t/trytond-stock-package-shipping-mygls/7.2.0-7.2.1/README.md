# Comparing `tmp/trytond_stock_package_shipping_mygls-7.2.0.tar.gz` & `tmp/trytond_stock_package_shipping_mygls-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_mygls-7.2.0.tar", last modified: Mon Apr 29 15:52:06 2024, max compression
+gzip compressed data, was "trytond_stock_package_shipping_mygls-7.2.1.tar", last modified: Wed May  1 10:02:07 2024, max compression
```

## Comparing `trytond_stock_package_shipping_mygls-7.2.0.tar` & `trytond_stock_package_shipping_mygls-7.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      765 2024-04-29 15:28:25.000000 trytond_stock_package_shipping_mygls-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:28:25.000000 trytond_stock_package_shipping_mygls-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/api.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4021 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3091 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_mygls-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6819 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6950 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6900 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6988 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5164 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5264 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6778 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6817 2024-04-29 13:17:17.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-27 16:43:28.000000 trytond_stock_package_shipping_mygls-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2010 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_mygls-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4853 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_mygls-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_mygls-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.491114 trytond_stock_package_shipping_mygls-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6596 2024-04-22 12:14:36.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/scenario_stock_package_shipping_mygls.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_mygls-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-29 15:28:21.000000 trytond_stock_package_shipping_mygls-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1849 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:06.000000 trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:06.494447 trytond_stock_package_shipping_mygls-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-7.2.0/view/credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2024-05-01 10:02:04.000000 trytond_stock_package_shipping_mygls-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 10:02:04.000000 trytond_stock_package_shipping_mygls-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/api.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4021 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2688 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.629166 trytond_stock_package_shipping_mygls-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3091 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6819 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-30 17:21:59.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6900 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6987 2024-04-30 17:21:59.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5164 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5264 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6778 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6817 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5139 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2010 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4853 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6596 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/tests/scenario_stock_package_shipping_mygls.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-30 17:21:06.000000 trytond_stock_package_shipping_mygls-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3039 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1849 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:02:07.000000 trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:07.632499 trytond_stock_package_shipping_mygls-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/view/credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:21:00.000000 trytond_stock_package_shipping_mygls-7.2.1/view/credential_list.xml
```

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/CHANGELOG` & `trytond_stock_package_shipping_mygls-7.2.1/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/COPYRIGHT` & `trytond_stock_package_shipping_mygls-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/LICENSE` & `trytond_stock_package_shipping_mygls-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/PKG-INFO` & `trytond_stock_package_shipping_mygls-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_mygls
-Version: 7.2.0
+Version: 7.2.1
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/__init__.py` & `trytond_stock_package_shipping_mygls-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/api.py` & `trytond_stock_package_shipping_mygls-7.2.1/api.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/carrier.py` & `trytond_stock_package_shipping_mygls-7.2.1/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/carrier.xml` & `trytond_stock_package_shipping_mygls-7.2.1/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/doc/conf.py` & `trytond_stock_package_shipping_mygls-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/doc/design.rst` & `trytond_stock_package_shipping_mygls-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/bg.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/ca.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/cs.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/de.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 msgstr "MyGLS Anmeldedaten"
 
 msgctxt "model:ir.message,text:msg_email_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add an email for address "
 "\"%(address)s\"."
 msgstr ""
-"Damit die Lieferung \"%(shipment)s\" validiert werden kann muss eine E-Mail-"
-"Adresse für Adresse \"%(address)s\" erfasst werden."
+"Damit die Lieferung \"%(shipment)s\" validiert werden kann, muss eine "
+"E-Mail-Adresse für Adresse \"%(address)s\" erfasst werden."
 
 msgctxt "model:ir.message,text:msg_mobile_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a mobile number for "
 "address \"%(address)s\"."
 msgstr ""
 "Damit die Lieferung \"%(shipment)s\" validiert werden kann, muss eine "
```

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/es.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/es_419.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/et.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/fa.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/fi.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/fr.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 msgctxt "model:ir.message,text:msg_mygls_api_error"
 msgid ""
 "MyGLS API call failed with the following error message:\n"
 "%(message)s"
 msgstr ""
 "L'appel de l'API MyGLS a échoué avec le message d'erreur suivant :\n"
-"%(messages)s"
+"%(message)s"
 
 msgctxt "model:ir.message,text:msg_phone_mobile_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a phone or mobile number "
 "for address \"%(address)s\"."
 msgstr ""
 "Pour valider l'expédition « %(shipment)s », vous devez ajouter un numéro de "
```

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/hu.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/id.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/it.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/lo.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/lt.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/nl.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/pl.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/pt.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/ro.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/ru.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/sl.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/tr.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/uk.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/locale/zh_CN.po` & `trytond_stock_package_shipping_mygls-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/message.xml` & `trytond_stock_package_shipping_mygls-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/setup.py` & `trytond_stock_package_shipping_mygls-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/stock.py` & `trytond_stock_package_shipping_mygls-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/tests/scenario_stock_package_shipping_mygls.rst` & `trytond_stock_package_shipping_mygls-7.2.1/tests/scenario_stock_package_shipping_mygls.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/tox.ini` & `trytond_stock_package_shipping_mygls-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO` & `trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_mygls
-Version: 7.2.0
+Version: 7.2.1
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_mygls-7.2.1/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/view/carrier_form.xml` & `trytond_stock_package_shipping_mygls-7.2.1/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-7.2.0/view/credential_form.xml` & `trytond_stock_package_shipping_mygls-7.2.1/view/credential_form.xml`

 * *Files identical despite different names*

