# Comparing `tmp/trytond_purchase_amendment-7.2.0.tar.gz` & `tmp/trytond_purchase_amendment-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_amendment-7.2.0.tar", last modified: Mon Apr 29 15:45:32 2024, max compression
+gzip compressed data, was "trytond_purchase_amendment-7.2.1.tar", last modified: Wed May  1 11:37:33 2024, max compression
```

## Comparing `trytond_purchase_amendment-7.2.0.tar` & `trytond_purchase_amendment-7.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1068 2024-04-29 15:23:29.000000 trytond_purchase_amendment-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:23:29.000000 trytond_purchase_amendment-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3300 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.318090 trytond_purchase_amendment-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_purchase_amendment-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:20.000000 trytond_purchase_amendment-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4457 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4493 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4486 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4507 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3962 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4468 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4524 2024-04-29 13:17:17.000000 trytond_purchase_amendment-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-27 16:43:25.000000 trytond_purchase_amendment-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14949 2024-04-27 16:30:39.000000 trytond_purchase_amendment-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6021 2024-04-27 16:30:39.000000 trytond_purchase_amendment-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4430 2024-03-17 11:01:36.000000 trytond_purchase_amendment-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4626 2024-04-22 12:14:36.000000 trytond_purchase_amendment-7.2.0/tests/scenario_purchase_amendment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:20.000000 trytond_purchase_amendment-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-04-29 15:23:24.000000 trytond_purchase_amendment-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3300 2024-04-29 15:45:31.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-29 15:45:32.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:31.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:45:31.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:45:31.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:31.000000 trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:32.321423 trytond_purchase_amendment-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-01-27 09:58:52.000000 trytond_purchase_amendment-7.2.0/view/purchase_amendment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1228 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/view/purchase_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/view/purchase_amendment_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/view/purchase_amendment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_purchase_amendment-7.2.0/view/purchase_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.444487 trytond_purchase_amendment-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1169 2024-05-01 11:37:30.000000 trytond_purchase_amendment-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 11:37:29.000000 trytond_purchase_amendment-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3300 2024-05-01 11:37:33.444487 trytond_purchase_amendment-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.441154 trytond_purchase_amendment-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.441154 trytond_purchase_amendment-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4459 2024-04-30 17:21:59.000000 trytond_purchase_amendment-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4493 2024-04-30 17:21:59.000000 trytond_purchase_amendment-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4486 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4507 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3962 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4468 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4524 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14949 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6021 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:37:33.444487 trytond_purchase_amendment-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4430 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.441154 trytond_purchase_amendment-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4626 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/tests/scenario_purchase_amendment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2024-04-30 17:21:06.000000 trytond_purchase_amendment-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.444487 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3300 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-05-01 11:37:33.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:37:32.000000 trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:37:33.444487 trytond_purchase_amendment-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/view/purchase_amendment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/view/purchase_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/view/purchase_amendment_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/view/purchase_amendment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_purchase_amendment-7.2.1/view/purchase_form.xml
```

### Comparing `trytond_purchase_amendment-7.2.0/CHANGELOG` & `trytond_purchase_amendment-7.2.1/CHANGELOG`

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

### Comparing `trytond_purchase_amendment-7.2.0/COPYRIGHT` & `trytond_purchase_amendment-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/LICENSE` & `trytond_purchase_amendment-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/PKG-INFO` & `trytond_purchase_amendment-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_amendment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to amend purchases
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_amendment-7.2.0/README.rst` & `trytond_purchase_amendment-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/doc/conf.py` & `trytond_purchase_amendment-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/doc/index.rst` & `trytond_purchase_amendment-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/bg.po` & `trytond_purchase_amendment-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/ca.po` & `trytond_purchase_amendment-7.2.1/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 msgctxt "model:ir.message,text:msg_one_purchase_at_time"
 msgid ""
 "You cannot validate more than one amendment at the same time for purchase "
 "\"%(purchase)s\"."
 msgstr ""
 "No es pot validar a la vegada més d'una correcció de la mateixa compra "
-"\"%(compra)s\"."
+"\"%(purchase)s\"."
 
 msgctxt ""
 "model:ir.model.button,confirm:purchase_amendment_validation_amendment_button"
 msgid "Are you sure you want to validate the amendements?"
 msgstr "Esteu segurs que voleu validar les correccions?"
 
 msgctxt ""
```

### Comparing `trytond_purchase_amendment-7.2.0/locale/cs.po` & `trytond_purchase_amendment-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/de.po` & `trytond_purchase_amendment-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Bestätigen"
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr "Änderungen"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
```

### Comparing `trytond_purchase_amendment-7.2.0/locale/es.po` & `trytond_purchase_amendment-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/es_419.po` & `trytond_purchase_amendment-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/et.po` & `trytond_purchase_amendment-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/fa.po` & `trytond_purchase_amendment-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/fi.po` & `trytond_purchase_amendment-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/fr.po` & `trytond_purchase_amendment-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/hu.po` & `trytond_purchase_amendment-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/id.po` & `trytond_purchase_amendment-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/it.po` & `trytond_purchase_amendment-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/lo.po` & `trytond_purchase_amendment-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/lt.po` & `trytond_purchase_amendment-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/nl.po` & `trytond_purchase_amendment-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/pl.po` & `trytond_purchase_amendment-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/pt.po` & `trytond_purchase_amendment-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/ro.po` & `trytond_purchase_amendment-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/ru.po` & `trytond_purchase_amendment-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/sl.po` & `trytond_purchase_amendment-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/tr.po` & `trytond_purchase_amendment-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/uk.po` & `trytond_purchase_amendment-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/locale/zh_CN.po` & `trytond_purchase_amendment-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/purchase.py` & `trytond_purchase_amendment-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/purchase.xml` & `trytond_purchase_amendment-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/setup.py` & `trytond_purchase_amendment-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/tests/scenario_purchase_amendment.rst` & `trytond_purchase_amendment-7.2.1/tests/scenario_purchase_amendment.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/tox.ini` & `trytond_purchase_amendment-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/PKG-INFO` & `trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_amendment
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to amend purchases
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_amendment-7.2.0/trytond_purchase_amendment.egg-info/SOURCES.txt` & `trytond_purchase_amendment-7.2.1/trytond_purchase_amendment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/view/purchase_amendment_form.xml` & `trytond_purchase_amendment-7.2.1/view/purchase_amendment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-7.2.0/view/purchase_amendment_line_form.xml` & `trytond_purchase_amendment-7.2.1/view/purchase_amendment_line_form.xml`

 * *Files identical despite different names*

