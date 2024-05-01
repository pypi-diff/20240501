# Comparing `tmp/trytond_party_siret-7.2.0.tar.gz` & `tmp/trytond_party_siret-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party_siret-7.2.0.tar", last modified: Mon Apr 29 15:42:15 2024, max compression
+gzip compressed data, was "trytond_party_siret-7.2.1.tar", last modified: Wed May  1 11:56:26 2024, max compression
```

## Comparing `trytond_party_siret-7.2.0.tar` & `trytond_party_siret-7.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.146580 trytond_party_siret-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2646 2024-04-29 15:21:08.000000 trytond_party_siret-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:21:08.000000 trytond_party_siret-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party_siret-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2480 2024-04-29 15:42:15.146580 trytond_party_siret-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-27 16:30:39.000000 trytond_party_siret-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3385 2024-01-27 09:58:52.000000 trytond_party_siret-7.2.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/address.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-27 16:30:39.000000 trytond_party_siret-7.2.0/company.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.143247 trytond_party_siret-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_party_siret-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:13.000000 trytond_party_siret-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.143247 trytond_party_siret-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-29 13:17:17.000000 trytond_party_siret-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      622 2024-04-27 16:30:39.000000 trytond_party_siret-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:15.146580 trytond_party_siret-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4256 2024-03-17 11:01:36.000000 trytond_party_siret-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.143247 trytond_party_siret-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:13.000000 trytond_party_siret-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      111 2024-04-29 15:21:03.000000 trytond_party_siret-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.146580 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2480 2024-04-29 15:42:14.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1442 2024-04-29 15:42:15.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:14.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:42:14.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2024-04-29 15:42:14.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:14.000000 trytond_party_siret-7.2.0/trytond_party_siret.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:15.143247 trytond_party_siret-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_party_siret-7.2.0/view/party_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.191528 trytond_party_siret-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2747 2024-05-01 11:56:22.000000 trytond_party_siret-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 11:56:22.000000 trytond_party_siret-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2480 2024-05-01 11:56:26.188195 trytond_party_siret-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3385 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/address.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/company.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.184862 trytond_party_siret-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.188195 trytond_party_siret-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:59.000000 trytond_party_siret-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:59.000000 trytond_party_siret-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:59.000000 trytond_party_siret-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:21:59.000000 trytond_party_siret-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      622 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:56:26.191528 trytond_party_siret-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4256 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.188195 trytond_party_siret-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      111 2024-04-30 17:21:06.000000 trytond_party_siret-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.188195 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2480 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1442 2024-05-01 11:56:26.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:56:25.000000 trytond_party_siret-7.2.1/trytond_party_siret.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:56:26.188195 trytond_party_siret-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:20:59.000000 trytond_party_siret-7.2.1/view/party_tree.xml
```

### Comparing `trytond_party_siret-7.2.0/CHANGELOG` & `trytond_party_siret-7.2.1/CHANGELOG`

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

### Comparing `trytond_party_siret-7.2.0/COPYRIGHT` & `trytond_party_siret-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/LICENSE` & `trytond_party_siret-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/PKG-INFO` & `trytond_party_siret-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_party_siret
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add SIRET/SIREN on parties
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party_siret-7.2.0/address.py` & `trytond_party_siret-7.2.1/address.py`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/company.py` & `trytond_party_siret-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/doc/conf.py` & `trytond_party_siret-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/party.py` & `trytond_party_siret-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/setup.py` & `trytond_party_siret-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/tox.ini` & `trytond_party_siret-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party_siret-7.2.0/trytond_party_siret.egg-info/PKG-INFO` & `trytond_party_siret-7.2.1/trytond_party_siret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_party_siret
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add SIRET/SIREN on parties
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party_siret-7.2.0/trytond_party_siret.egg-info/SOURCES.txt` & `trytond_party_siret-7.2.1/trytond_party_siret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

