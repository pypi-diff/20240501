# Comparing `tmp/trytond_stock_package_shipping-7.0.1.tar.gz` & `tmp/trytond_stock_package_shipping-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping-7.0.1.tar", last modified: Wed May  1 10:02:34 2024, max compression
+gzip compressed data, was "trytond_stock_package_shipping-7.2.0.tar", last modified: Mon Apr 29 15:51:52 2024, max compression
```

## Comparing `trytond_stock_package_shipping-7.0.1.tar` & `trytond_stock_package_shipping-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2144 2024-05-01 10:02:31.000000 trytond_stock_package_shipping-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-05-01 10:02:31.000000 trytond_stock_package_shipping-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4554 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      650 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.395132 trytond_stock_package_shipping-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2801 2024-03-03 16:24:20.000000 trytond_stock_package_shipping-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2887 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2868 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2787 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2965 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2481 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11553 2024-04-27 05:19:49.000000 trytond_stock_package_shipping-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4514 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-02-05 16:24:27.000000 trytond_stock_package_shipping-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4554 2024-05-01 10:02:33.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1934 2024-05-01 10:02:34.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:02:33.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 10:02:33.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:15.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-05-01 10:02:33.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:02:33.000000 trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:02:34.398466 trytond_stock_package_shipping-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/carrier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/shipment_in_return_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-10-30 17:06:38.000000 trytond_stock_package_shipping-7.0.1/view/shipment_out_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2144 2024-04-29 15:28:15.000000 trytond_stock_package_shipping-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-29 15:28:14.000000 trytond_stock_package_shipping-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4554 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      650 2024-01-27 09:58:52.000000 trytond_stock_package_shipping-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-01-16 14:00:21.000000 trytond_stock_package_shipping-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.351484 trytond_stock_package_shipping-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_stock_package_shipping-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:34.000000 trytond_stock_package_shipping-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.351484 trytond_stock_package_shipping-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2887 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2873 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2868 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2787 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2965 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2481 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2798 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2812 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2024-04-27 16:43:27.000000 trytond_stock_package_shipping-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      604 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-03-17 11:01:36.000000 trytond_stock_package_shipping-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11549 2024-04-27 16:30:39.000000 trytond_stock_package_shipping-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4429 2024-04-27 16:30:39.000000 trytond_stock_package_shipping-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:34.000000 trytond_stock_package_shipping-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-29 15:28:10.000000 trytond_stock_package_shipping-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4554 2024-04-29 15:51:51.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1934 2024-04-29 15:51:52.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:51.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:51:51.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-29 15:51:51.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:51.000000 trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:52.354817 trytond_stock_package_shipping-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/view/carrier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-01-27 09:58:52.000000 trytond_stock_package_shipping-7.2.0/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-7.2.0/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2024-02-04 18:51:26.000000 trytond_stock_package_shipping-7.2.0/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-02-04 18:51:26.000000 trytond_stock_package_shipping-7.2.0/view/shipment_in_return_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2024-02-04 18:51:26.000000 trytond_stock_package_shipping-7.2.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-02-04 18:51:26.000000 trytond_stock_package_shipping-7.2.0/view/shipment_out_list.xml
```

### Comparing `trytond_stock_package_shipping-7.0.1/CHANGELOG` & `trytond_stock_package_shipping-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-05-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_package_shipping-7.0.1/COPYRIGHT` & `trytond_stock_package_shipping-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/LICENSE` & `trytond_stock_package_shipping-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/PKG-INFO` & `trytond_stock_package_shipping-7.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping
-Version: 7.0.1
+Version: 7.2.0
 Summary: The package shipping module of the Tryton application platform.
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
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Package Shipping Module
 #############################
 
 This module is the base module required to interact with shipping service
 providers.
```

### Comparing `trytond_stock_package_shipping-7.0.1/README.rst` & `trytond_stock_package_shipping-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/__init__.py` & `trytond_stock_package_shipping-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/carrier.xml` & `trytond_stock_package_shipping-7.2.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/doc/conf.py` & `trytond_stock_package_shipping-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping-7.0.1/doc/configuration.rst` & `trytond_stock_package_shipping-7.2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/doc/index.rst` & `trytond_stock_package_shipping-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/bg.po` & `trytond_stock_package_shipping-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/ca.po` & `trytond_stock_package_shipping-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/cs.po` & `trytond_stock_package_shipping-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/de.po` & `trytond_stock_package_shipping-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/es.po` & `trytond_stock_package_shipping-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/es_419.po` & `trytond_stock_package_shipping-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/et.po` & `trytond_stock_package_shipping-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/fa.po` & `trytond_stock_package_shipping-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/fi.po` & `trytond_stock_package_shipping-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/fr.po` & `trytond_stock_package_shipping-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/hu.po` & `trytond_stock_package_shipping-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/id.po` & `trytond_stock_package_shipping-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/it.po` & `trytond_stock_package_shipping-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/lo.po` & `trytond_stock_package_shipping-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/lt.po` & `trytond_stock_package_shipping-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/nl.po` & `trytond_stock_package_shipping-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/pl.po` & `trytond_stock_package_shipping-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/pt.po` & `trytond_stock_package_shipping-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/ro.po` & `trytond_stock_package_shipping-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/ru.po` & `trytond_stock_package_shipping-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/sl.po` & `trytond_stock_package_shipping-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/tr.po` & `trytond_stock_package_shipping-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/uk.po` & `trytond_stock_package_shipping-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/locale/zh_CN.po` & `trytond_stock_package_shipping-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/message.xml` & `trytond_stock_package_shipping-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/setup.py` & `trytond_stock_package_shipping-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/stock.py` & `trytond_stock_package_shipping-7.2.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,16 +285,16 @@
         states={
             'readonly': ~Eval('state').in_(['draft', 'waiting', 'assigned']),
             })
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, shipments):
-        super().done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
         cls.check_no_carrier(shipments)
 
     @property
     def shipping_allowed(self):
         return {'assigned', 'done'}
 
     @property
```

### Comparing `trytond_stock_package_shipping-7.0.1/stock.xml` & `trytond_stock_package_shipping-7.2.0/stock.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_stock_package_shipping-7.0.1/stock.xml` & `trytond_stock_package_shipping-7.2.0/stock.xml`

```diff
@@ -10,47 +10,47 @@
     </record>
     <record model="ir.ui.view" id="package_view_tree">
       <field name="model">stock.package</field>
       <field name="inherit" ref="stock_package.package_view_tree"/>
       <field name="name">package_list</field>
     </record>
     <record model="ir.model.button" id="package_print_shipping_label_button">
+      <field name="model">stock.package</field>
       <field name="name">print_shipping_label</field>
       <field name="string">Shipping Label</field>
-      <field name="model" search="[('model', '=', 'stock.package')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_out_view_form">
       <field name="model">stock.shipment.out</field>
       <field name="inherit" ref="stock.shipment_out_view_form"/>
       <field name="name">shipment_out_form</field>
     </record>
     <record model="ir.ui.view" id="shipment_out_view_list">
       <field name="model">stock.shipment.out</field>
       <field name="inherit" ref="stock.shipment_out_view_tree"/>
       <field name="name">shipment_out_list</field>
     </record>
     <record model="ir.model.button" id="shipment_out_create_shipping_button">
+      <field name="model">stock.shipment.out</field>
       <field name="name">create_shipping</field>
       <field name="string">Create Shipping for Packages</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.out')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_in_return_view_form">
       <field name="model">stock.shipment.in.return</field>
       <field name="inherit" ref="stock.shipment_in_return_view_form"/>
       <field name="name">shipment_in_return_form</field>
     </record>
     <record model="ir.ui.view" id="shipment_in_return_view_list">
       <field name="model">stock.shipment.in.return</field>
       <field name="inherit" ref="stock.shipment_in_return_view_tree"/>
       <field name="name">shipment_in_return_list</field>
     </record>
     <record model="ir.model.button" id="shipment_in_return_create_shipping_button">
+      <field name="model">stock.shipment.in.return</field>
       <field name="name">create_shipping</field>
       <field name="string">Create Shipping for Packages</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
     </record>
     <record model="ir.action.wizard" id="act_create_shipping_wizard">
       <field name="name">Create Shipping</field>
       <field name="wiz_name">stock.shipment.create_shipping</field>
     </record>
     <record model="ir.action.report" id="report_shipping_label">
       <field name="name">Shipping Label</field>
```

### Comparing `trytond_stock_package_shipping-7.0.1/tox.ini` & `trytond_stock_package_shipping-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/PKG-INFO` & `trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping
-Version: 7.0.1
+Version: 7.2.0
 Summary: The package shipping module of the Tryton application platform.
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
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Package Shipping Module
 #############################
 
 This module is the base module required to interact with shipping service
 providers.
```

### Comparing `trytond_stock_package_shipping-7.0.1/trytond_stock_package_shipping.egg-info/SOURCES.txt` & `trytond_stock_package_shipping-7.2.0/trytond_stock_package_shipping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/view/package_form.xml` & `trytond_stock_package_shipping-7.2.0/view/package_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/view/shipment_in_return_form.xml` & `trytond_stock_package_shipping-7.2.0/view/shipment_in_return_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-7.0.1/view/shipment_out_form.xml` & `trytond_stock_package_shipping-7.2.0/view/shipment_out_form.xml`

 * *Files identical despite different names*

