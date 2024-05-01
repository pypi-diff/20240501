# Comparing `tmp/trytond_sale_amendment-7.2.0.tar.gz` & `tmp/trytond_sale_amendment-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_amendment-7.2.0.tar", last modified: Mon Apr 29 15:47:18 2024, max compression
+gzip compressed data, was "trytond_sale_amendment-7.2.1.tar", last modified: Wed May  1 11:27:13 2024, max compression
```

## Comparing `trytond_sale_amendment-7.2.0.tar` & `trytond_sale_amendment-7.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1068 2024-04-29 15:24:42.000000 trytond_sale_amendment-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:24:41.000000 trytond_sale_amendment-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.401982 trytond_sale_amendment-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_sale_amendment-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4347 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4360 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4382 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4398 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3870 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4395 2024-04-29 13:17:17.000000 trytond_sale_amendment-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4358 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4334 2024-04-29 13:17:17.000000 trytond_sale_amendment-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-27 16:43:26.000000 trytond_sale_amendment-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16693 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5788 2024-04-27 16:30:39.000000 trytond_sale_amendment-7.2.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2024-03-17 11:01:36.000000 trytond_sale_amendment-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4516 2024-04-22 12:14:36.000000 trytond_sale_amendment-7.2.0/tests/scenario_sale_amendment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_sale_amendment-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-04-29 15:24:37.000000 trytond_sale_amendment-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1771 2024-04-29 15:47:18.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:17.000000 trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:18.405315 trytond_sale_amendment-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      621 2024-01-27 09:58:52.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1305 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_amendment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_amendment-7.2.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1169 2024-05-01 11:27:10.000000 trytond_sale_amendment-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:27:10.000000 trytond_sale_amendment-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.827360 trytond_sale_amendment-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.827360 trytond_sale_amendment-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4347 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4360 2024-04-30 17:21:59.000000 trytond_sale_amendment-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4382 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4398 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3870 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4395 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4358 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4334 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16693 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5788 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4516 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/tests/scenario_sale_amendment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      129 2024-04-30 17:21:06.000000 trytond_sale_amendment-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3257 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:27:13.000000 trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:27:13.830693 trytond_sale_amendment-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      621 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/view/sale_amendment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1305 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/view/sale_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/view/sale_amendment_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/view/sale_amendment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_sale_amendment-7.2.1/view/sale_form.xml
```

### Comparing `trytond_sale_amendment-7.2.0/CHANGELOG` & `trytond_sale_amendment-7.2.1/CHANGELOG`

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

### Comparing `trytond_sale_amendment-7.2.0/COPYRIGHT` & `trytond_sale_amendment-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/LICENSE` & `trytond_sale_amendment-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/PKG-INFO` & `trytond_sale_amendment-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_amendment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to amend sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_amendment-7.2.0/README.rst` & `trytond_sale_amendment-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/doc/conf.py` & `trytond_sale_amendment-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/doc/index.rst` & `trytond_sale_amendment-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/bg.po` & `trytond_sale_amendment-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/ca.po` & `trytond_sale_amendment-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/cs.po` & `trytond_sale_amendment-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/de.po` & `trytond_sale_amendment-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Bestätigen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Änderungen"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
```

### Comparing `trytond_sale_amendment-7.2.0/locale/es.po` & `trytond_sale_amendment-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/es_419.po` & `trytond_sale_amendment-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/et.po` & `trytond_sale_amendment-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/fa.po` & `trytond_sale_amendment-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/fi.po` & `trytond_sale_amendment-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/fr.po` & `trytond_sale_amendment-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/hu.po` & `trytond_sale_amendment-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/id.po` & `trytond_sale_amendment-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/it.po` & `trytond_sale_amendment-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/lo.po` & `trytond_sale_amendment-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/lt.po` & `trytond_sale_amendment-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/nl.po` & `trytond_sale_amendment-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/pl.po` & `trytond_sale_amendment-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/pt.po` & `trytond_sale_amendment-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/ro.po` & `trytond_sale_amendment-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/ru.po` & `trytond_sale_amendment-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/sl.po` & `trytond_sale_amendment-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/tr.po` & `trytond_sale_amendment-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/uk.po` & `trytond_sale_amendment-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/locale/zh_CN.po` & `trytond_sale_amendment-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/sale.py` & `trytond_sale_amendment-7.2.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/sale.xml` & `trytond_sale_amendment-7.2.1/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/setup.py` & `trytond_sale_amendment-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/tests/scenario_sale_amendment.rst` & `trytond_sale_amendment-7.2.1/tests/scenario_sale_amendment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/tox.ini` & `trytond_sale_amendment-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/PKG-INFO` & `trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_amendment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to amend sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_amendment-7.2.0/trytond_sale_amendment.egg-info/SOURCES.txt` & `trytond_sale_amendment-7.2.1/trytond_sale_amendment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/view/sale_amendment_form.xml` & `trytond_sale_amendment-7.2.1/view/sale_amendment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-7.2.0/view/sale_amendment_line_form.xml` & `trytond_sale_amendment-7.2.1/view/sale_amendment_line_form.xml`

 * *Files identical despite different names*

