# Comparing `tmp/trytond_stock_package-7.2.0.tar.gz` & `tmp/trytond_stock_package-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package-7.2.0.tar", last modified: Mon Apr 29 15:51:44 2024, max compression
+gzip compressed data, was "trytond_stock_package-7.2.1.tar", last modified: Wed May  1 10:03:48 2024, max compression
```

## Comparing `trytond_stock_package-7.2.0.tar` & `trytond_stock_package-7.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2243 2024-04-29 15:28:10.000000 trytond_stock_package-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:28:09.000000 trytond_stock_package-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2883 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_stock_package-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.861680 trytond_stock_package-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-27 16:30:39.000000 trytond_stock_package-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_stock_package-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:33.000000 trytond_stock_package-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6359 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7565 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6237 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7766 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7647 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6269 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6579 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6835 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6224 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7787 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6659 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6174 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6284 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6362 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6237 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7790 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6605 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6637 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6167 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6381 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6607 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6224 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6128 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6290 2024-04-27 16:43:27.000000 trytond_stock_package-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4398 2024-03-17 11:01:36.000000 trytond_stock_package-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16619 2024-04-27 16:30:39.000000 trytond_stock_package-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6400 2024-04-27 16:30:39.000000 trytond_stock_package-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3738 2024-04-22 12:14:36.000000 trytond_stock_package-7.2.0/tests/scenario_stock_package.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:33.000000 trytond_stock_package-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2024-04-29 15:28:05.000000 trytond_stock_package-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2883 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1950 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:44.000000 trytond_stock_package-7.2.0/trytond_stock_package.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:44.865013 trytond_stock_package-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2024-02-04 18:51:26.000000 trytond_stock_package-7.2.0/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/view/package_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-01-27 09:58:52.000000 trytond_stock_package-7.2.0/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/view/package_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:21.000000 trytond_stock_package-7.2.0/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:21.000000 trytond_stock_package-7.2.0/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_stock_package-7.2.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.109871 trytond_stock_package-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-05-01 10:03:45.000000 trytond_stock_package-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 10:03:44.000000 trytond_stock_package-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2883 2024-05-01 10:03:48.109871 trytond_stock_package-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.103205 trytond_stock_package-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3076 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.106538 trytond_stock_package-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6359 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7565 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6237 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7764 2024-04-30 17:21:59.000000 trytond_stock_package-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7647 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6269 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6579 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6835 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6224 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7787 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6659 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6174 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6284 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6362 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6237 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7790 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6605 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6637 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6167 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6381 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6607 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6224 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6128 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6290 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:03:48.109871 trytond_stock_package-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4398 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16619 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6400 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.106538 trytond_stock_package-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3738 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/tests/scenario_stock_package.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2024-04-30 17:21:06.000000 trytond_stock_package-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.106538 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2883 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1950 2024-05-01 10:03:48.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:03:47.000000 trytond_stock_package-7.2.1/trytond_stock_package.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:03:48.106538 trytond_stock_package-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1538 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/package_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/package_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/package_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:21:00.000000 trytond_stock_package-7.2.1/view/stock_move_form.xml
```

### Comparing `trytond_stock_package-7.2.0/CHANGELOG` & `trytond_stock_package-7.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_stock_package-7.2.0/COPYRIGHT` & `trytond_stock_package-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/LICENSE` & `trytond_stock_package-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/PKG-INFO` & `trytond_stock_package-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for stock packaging
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_package-7.2.0/doc/conf.py` & `trytond_stock_package-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/bg.po` & `trytond_stock_package-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/ca.po` & `trytond_stock_package-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/cs.po` & `trytond_stock_package-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/de.po` & `trytond_stock_package-7.2.1/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Verpackungsvolumen"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UoM"
-msgstr "Maßeinheit Verpackungsvolumen"
+msgstr "Volumenmaßeinheit Verpackung"
 
 msgctxt "field:stock.package,packaging_weight:"
 msgid "Packaging Weight"
 msgstr "Verpackungsgewicht"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UoM"
-msgstr "Maßeinheit Verpackungsgewicht"
+msgstr "Gewichtsmaßeinheit Verpackung"
 
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Übergeordnet (Paket)"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
@@ -108,23 +108,23 @@
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Verpackungsvolumen"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UoM"
-msgstr "Maßeinheit Verpackungsvolumen"
+msgstr "Volumenmaßeinheit Verpackung"
 
 msgctxt "field:stock.package.type,packaging_weight:"
 msgid "Packaging Weight"
 msgstr "Verpackungsgewicht"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UoM"
-msgstr "Maßeinheit Verpackungsgewicht"
+msgstr "Gewichtsmaßeinheit Verpackung"
 
 msgctxt "field:stock.package.type,width:"
 msgid "Width"
 msgstr "Breite"
 
 msgctxt "field:stock.package.type,width_uom:"
 msgid "Width UoM"
@@ -243,15 +243,15 @@
 msgstr ""
 "Das Volumen (%(volume)s) des Pakets \"%(package)s\" ist zu niedrig im "
 "Vergleich zum aufsummierten Volumen (%(children_volume)s) der "
 "untergeordneten Pakete."
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
 msgstr "Lager Paket"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
```

### Comparing `trytond_stock_package-7.2.0/locale/es.po` & `trytond_stock_package-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/es_419.po` & `trytond_stock_package-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/et.po` & `trytond_stock_package-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/fa.po` & `trytond_stock_package-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/fi.po` & `trytond_stock_package-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/fr.po` & `trytond_stock_package-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/hu.po` & `trytond_stock_package-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/id.po` & `trytond_stock_package-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/it.po` & `trytond_stock_package-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/lo.po` & `trytond_stock_package-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/lt.po` & `trytond_stock_package-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/nl.po` & `trytond_stock_package-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/pl.po` & `trytond_stock_package-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/pt.po` & `trytond_stock_package-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/ro.po` & `trytond_stock_package-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/ru.po` & `trytond_stock_package-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/sl.po` & `trytond_stock_package-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/tr.po` & `trytond_stock_package-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/uk.po` & `trytond_stock_package-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/locale/zh_CN.po` & `trytond_stock_package-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/message.xml` & `trytond_stock_package-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/setup.py` & `trytond_stock_package-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/stock.py` & `trytond_stock_package-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/stock.xml` & `trytond_stock_package-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/tests/scenario_stock_package.rst` & `trytond_stock_package-7.2.1/tests/scenario_stock_package.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/tox.ini` & `trytond_stock_package-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/trytond_stock_package.egg-info/PKG-INFO` & `trytond_stock_package-7.2.1/trytond_stock_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for stock packaging
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_package-7.2.0/trytond_stock_package.egg-info/SOURCES.txt` & `trytond_stock_package-7.2.1/trytond_stock_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/view/package_form.xml` & `trytond_stock_package-7.2.1/view/package_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-7.2.0/view/package_type_form.xml` & `trytond_stock_package-7.2.1/view/package_type_form.xml`

 * *Files identical despite different names*

