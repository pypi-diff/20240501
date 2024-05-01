# Comparing `tmp/trytond_carrier_weight-7.2.0.tar.gz` & `tmp/trytond_carrier_weight-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_weight-7.2.0.tar", last modified: Mon Apr 29 15:39:00 2024, max compression
+gzip compressed data, was "trytond_carrier_weight-7.2.1.tar", last modified: Wed May  1 12:03:13 2024, max compression
```

## Comparing `trytond_carrier_weight-7.2.0.tar` & `trytond_carrier_weight-7.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2278 2024-04-29 15:18:40.000000 trytond_carrier_weight-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:18:40.000000 trytond_carrier_weight-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4519 2024-02-04 18:51:26.000000 trytond_carrier_weight-7.2.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-02-04 18:51:26.000000 trytond_carrier_weight-7.2.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.441672 trytond_carrier_weight-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_carrier_weight-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:06.000000 trytond_carrier_weight-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2157 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2257 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2174 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1731 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2225 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2201 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2085 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1706 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2061 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1842 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2181 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1739 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1819 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2024-04-29 13:17:17.000000 trytond_carrier_weight-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-27 16:43:22.000000 trytond_carrier_weight-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4590 2024-03-17 11:01:36.000000 trytond_carrier_weight-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-08-20 10:47:27.000000 trytond_carrier_weight-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7465 2024-04-27 16:30:39.000000 trytond_carrier_weight-7.2.0/tests/scenario_carrier_weight.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3683 2024-01-27 09:58:52.000000 trytond_carrier_weight-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_weight-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:06.000000 trytond_carrier_weight-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-29 15:18:36.000000 trytond_carrier_weight-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1665 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:39:00.000000 trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:39:00.445006 trytond_carrier_weight-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/weight_price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-01-16 14:00:20.000000 trytond_carrier_weight-7.2.0/view/weight_price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.420877 trytond_carrier_weight-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-05-01 12:03:10.000000 trytond_carrier_weight-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-05-01 12:03:09.000000 trytond_carrier_weight-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-05-01 12:03:13.420877 trytond_carrier_weight-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4519 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.414211 trytond_carrier_weight-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.417544 trytond_carrier_weight-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2157 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2257 2024-04-30 17:21:59.000000 trytond_carrier_weight-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2174 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1731 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2225 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2201 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2085 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1706 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2061 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1842 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2181 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1739 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1819 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1674 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:03:13.420877 trytond_carrier_weight-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4590 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2768 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.417544 trytond_carrier_weight-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7465 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/tests/scenario_carrier_weight.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3683 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-30 17:21:06.000000 trytond_carrier_weight-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.417544 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3034 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1665 2024-05-01 12:03:13.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:03:12.000000 trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:03:13.417544 trytond_carrier_weight-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/view/weight_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:20:59.000000 trytond_carrier_weight-7.2.1/view/weight_price_list_tree.xml
```

### Comparing `trytond_carrier_weight-7.2.0/CHANGELOG` & `trytond_carrier_weight-7.2.1/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_carrier_weight-7.2.0/COPYRIGHT` & `trytond_carrier_weight-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/LICENSE` & `trytond_carrier_weight-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/PKG-INFO` & `trytond_carrier_weight-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_weight
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add cost method "on weight" on carrier
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_carrier_weight-7.2.0/__init__.py` & `trytond_carrier_weight-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/carrier.py` & `trytond_carrier_weight-7.2.1/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/carrier.xml` & `trytond_carrier_weight-7.2.1/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/common.py` & `trytond_carrier_weight-7.2.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/doc/conf.py` & `trytond_carrier_weight-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/bg.po` & `trytond_carrier_weight-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/ca.po` & `trytond_carrier_weight-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/cs.po` & `trytond_carrier_weight-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/de.po` & `trytond_carrier_weight-7.2.1/locale/de.po`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
 msgstr "Preisliste"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight UoM"
-msgstr "Maßeinheit Gewicht"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
 msgstr "Versanddienstleister"
 
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
@@ -28,15 +28,15 @@
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
 msgstr "Gewicht"
 
 msgctxt "field:carrier.weight_price_list,weight_uom:"
 msgid "Weight UoM"
-msgstr "Maßeinheit Gewicht"
+msgstr "Gewichtsmaßeinheit"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr "Die Währung des Preises."
 
 msgctxt "help:carrier,weight_price_list:"
 msgid ""
```

### Comparing `trytond_carrier_weight-7.2.0/locale/es.po` & `trytond_carrier_weight-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/es_419.po` & `trytond_carrier_weight-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/et.po` & `trytond_carrier_weight-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/fa.po` & `trytond_carrier_weight-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/fi.po` & `trytond_carrier_weight-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/fr.po` & `trytond_carrier_weight-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/hu.po` & `trytond_carrier_weight-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/id.po` & `trytond_carrier_weight-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/it.po` & `trytond_carrier_weight-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/lo.po` & `trytond_carrier_weight-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/lt.po` & `trytond_carrier_weight-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/nl.po` & `trytond_carrier_weight-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/pl.po` & `trytond_carrier_weight-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/pt.po` & `trytond_carrier_weight-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/ro.po` & `trytond_carrier_weight-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/ru.po` & `trytond_carrier_weight-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/sl.po` & `trytond_carrier_weight-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/tr.po` & `trytond_carrier_weight-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/uk.po` & `trytond_carrier_weight-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/locale/zh_CN.po` & `trytond_carrier_weight-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/sale.py` & `trytond_carrier_weight-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/setup.py` & `trytond_carrier_weight-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/stock.py` & `trytond_carrier_weight-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/tests/scenario_carrier_weight.rst` & `trytond_carrier_weight-7.2.1/tests/scenario_carrier_weight.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/tests/test_module.py` & `trytond_carrier_weight-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/tox.ini` & `trytond_carrier_weight-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/PKG-INFO` & `trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_weight
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add cost method "on weight" on carrier
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_carrier_weight-7.2.0/trytond_carrier_weight.egg-info/SOURCES.txt` & `trytond_carrier_weight-7.2.1/trytond_carrier_weight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

