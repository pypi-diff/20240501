# Comparing `tmp/trytond_quality-7.2.0.tar.gz` & `tmp/trytond_quality-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_quality-7.2.0.tar", last modified: Mon Apr 29 15:46:45 2024, max compression
+gzip compressed data, was "trytond_quality-7.2.1.tar", last modified: Wed May  1 11:32:21 2024, max compression
```

## Comparing `trytond_quality-7.2.0.tar` & `trytond_quality-7.2.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-29 15:24:26.000000 trytond_quality-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:24:26.000000 trytond_quality-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      979 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.949497 trytond_quality-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_quality-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.949497 trytond_quality-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/icons/tryton-quality.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12416 2024-04-29 13:17:17.000000 trytond_quality-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13164 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12447 2024-04-29 13:17:17.000000 trytond_quality-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12579 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12405 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10564 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10492 2024-04-27 16:43:26.000000 trytond_quality-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1624 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    29183 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/quality.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20163 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/quality.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:45.956164 trytond_quality-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6334 2024-04-27 16:30:39.000000 trytond_quality-7.2.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2444 2024-04-22 12:14:36.000000 trytond_quality-7.2.0/tests/scenario_quality_control_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2570 2024-04-22 12:14:36.000000 trytond_quality-7.2.0/tests/scenario_quality_inspection.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_quality-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-29 15:24:22.000000 trytond_quality-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/trytond_quality.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2350 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-08 12:43:26.000000 trytond_quality-7.2.0/trytond_quality.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:45.000000 trytond_quality-7.2.0/trytond_quality.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:45.952831 trytond_quality-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1177 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_alert_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_alert_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      816 2024-02-04 18:51:26.000000 trytond_quality-7.2.0/view/quality_control_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      709 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_control_point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1281 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_inspection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-01-27 09:58:52.000000 trytond_quality-7.2.0/view/quality_inspection_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.185988 trytond_quality-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-05-01 11:32:18.000000 trytond_quality-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-05-01 11:32:17.000000 trytond_quality-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-05-01 11:32:21.185988 trytond_quality-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      979 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.179321 trytond_quality-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.179321 trytond_quality-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/icons/tryton-quality.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.182654 trytond_quality-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12410 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13160 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12441 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12615 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12405 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10558 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10486 2024-04-30 17:21:59.000000 trytond_quality-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1624 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    29183 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/quality.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20163 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/quality.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:32:21.185988 trytond_quality-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6334 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.182654 trytond_quality-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2444 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tests/scenario_quality_control_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2570 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tests/scenario_quality_inspection.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-30 17:21:06.000000 trytond_quality-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.185988 trytond_quality-7.2.1/trytond_quality.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2771 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2350 2024-05-01 11:32:21.000000 trytond_quality-7.2.1/trytond_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:32:20.000000 trytond_quality-7.2.1/trytond_quality.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:32:21.185988 trytond_quality-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1177 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_alert_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_alert_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      816 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_control_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_control_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      709 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_control_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_control_point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1281 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_inspection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:21:00.000000 trytond_quality-7.2.1/view/quality_inspection_list.xml
```

### Comparing `trytond_quality-7.2.0/COPYRIGHT` & `trytond_quality-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/LICENSE` & `trytond_quality-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/PKG-INFO` & `trytond_quality-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_quality
-Version: 7.2.0
+Version: 7.2.1
 Summary: Quality Management
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_quality-7.2.0/__init__.py` & `trytond_quality-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/doc/conf.py` & `trytond_quality-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/doc/design.rst` & `trytond_quality-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/icons/LICENSE` & `trytond_quality-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/locale/bg.po` & `trytond_quality-7.2.1/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/ca.po` & `trytond_quality-7.2.1/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr "Inspecció finalitzada"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr "Ejecuta inspecció"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspecció finalitzada"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspecció recepció"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspecció finalitzada"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr "Inspecció enviament"
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr "Inspecció empaqueta"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr "Inspecció recull"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspecció finalitzada"
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspecció recepció"
```

### Comparing `trytond_quality-7.2.0/locale/cs.po` & `trytond_quality-7.2.1/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/de.po` & `trytond_quality-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -191,23 +191,23 @@
 msgid "Inspect Done"
 msgstr "Qualitätsprüfung für Status \"Erledigt\" durchführen"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr "Qualitätsprüfung für Status \"In Ausführung\" durchführen"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr "Qualitätsprüfung für Status \"Erledigt\" durchführen"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Qualitätsprüfung für Status \"Erhalten\" durchführen"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr "Qualitätsprüfung für Status \"Erledigt\" durchführen"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr "Qualitätsprüfung für Status \"Versendet\" durchführen"
 
@@ -215,17 +215,17 @@
 msgid "Inspect Pack"
 msgstr "Qualitätsprüfung für Status \"Gepackt\" durchführen"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr "Qualitätsprüfung für Status \"Kommissioniert\" durchführen"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
-msgstr "Qualitätsprüfung für Status \"Erledigt\" ausführen"
+msgstr "Qualitätsprüfung für Status \"Erledigt\" durchführen"
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Qualitätsprüfung für Status \"Erhalten\" durchführen"
 
 msgctxt ""
@@ -311,19 +311,19 @@
 
 msgctxt "model:ir.model.button,string:quality_inspection_process_button"
 msgid "Process"
 msgstr "Ausführen"
 
 msgctxt "model:ir.rule.group,name:rule_group_quality_control_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_quality_inspection_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.sequence,name:sequence_quality_alert"
 msgid "Quality Alert"
 msgstr "Qualitätswarnung"
 
 msgctxt "model:ir.sequence,name:sequence_quality_inspection"
 msgid "Quality Inspection"
```

### Comparing `trytond_quality-7.2.0/locale/es.po` & `trytond_quality-7.2.1/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr "Inspeccion finalizada"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr "Ejecutar inspección"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspeccion finalizada"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspección recepción"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspeccion finalizada"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr "Inspección envío"
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr "Inspección empaquetar"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr "Inspección recoger"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr "Inspeccion finalizada"
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspección recepción"
```

### Comparing `trytond_quality-7.2.0/locale/es_419.po` & `trytond_quality-7.2.1/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/et.po` & `trytond_quality-7.2.1/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/fa.po` & `trytond_quality-7.2.1/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/fi.po` & `trytond_quality-7.2.1/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/fr.po` & `trytond_quality-7.2.1/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -184,47 +184,47 @@
 
 msgctxt "model:ir.action,name:act_quality_inspection_form_relate"
 msgid "Quality Inspections"
 msgstr "Inspections de qualité"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_done"
 msgid "Inspect Done"
-msgstr "Inspecter terminé"
+msgstr "Inspecter l'achèvement"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
-msgstr "Inspecter Lancer"
+msgstr "Inspecter l'exécution"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspecter terminé"
+msgstr "Inspecter l'achèvement"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspecter la réception"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspecter terminé"
+msgstr "Inspecter l'achèvement"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
-msgstr "Inspecter Livrer"
+msgstr "Inspecter la livraison"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pack"
 msgid "Inspect Pack"
-msgstr "Inspecter Emballer"
+msgstr "Inspecter l'emballage"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
-msgstr "Inspecter Prélever"
+msgstr "Inspecter le prélèvement"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspecter terminé"
+msgstr "Inspecter l'achèvement"
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspecter la réception"
 
 msgctxt ""
```

### Comparing `trytond_quality-7.2.0/locale/hu.po` & `trytond_quality-7.2.1/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/id.po` & `trytond_quality-7.2.1/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/it.po` & `trytond_quality-7.2.1/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/lo.po` & `trytond_quality-7.2.1/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/lt.po` & `trytond_quality-7.2.1/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/nl.po` & `trytond_quality-7.2.1/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -190,41 +190,41 @@
 msgid "Inspect Done"
 msgstr "Inspectie Gereed"
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr "Inspectie Uitvoeren"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspectie Gereed"
+msgstr "Inspectie afronden"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspectie Levering"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspectie Gereed"
+msgstr "Inspectie afronden"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr "Inspectie Zending"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pack"
 msgid "Inspect Pack"
 msgstr "Inspectie Pakket"
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr "Inspectie Picking"
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
-msgstr "Inspectie Gereed"
+msgstr "Inspectie afronden"
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr "Inspectie Levering"
 
 msgctxt ""
```

### Comparing `trytond_quality-7.2.0/locale/pl.po` & `trytond_quality-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/pt.po` & `trytond_quality-7.2.1/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/ro.po` & `trytond_quality-7.2.1/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/ru.po` & `trytond_quality-7.2.1/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/sl.po` & `trytond_quality-7.2.1/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/tr.po` & `trytond_quality-7.2.1/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/uk.po` & `trytond_quality-7.2.1/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/locale/zh_CN.po` & `trytond_quality-7.2.1/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -190,23 +190,23 @@
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_production_inspect_run"
 msgid "Inspect Run"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_in_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_internal_inspect_ship"
 msgid "Inspect Ship"
 msgstr ""
 
@@ -214,15 +214,15 @@
 msgid "Inspect Pack"
 msgstr ""
 
 msgctxt "model:ir.action,name:wizard_stock_shipment_out_inspect_pick"
 msgid "Inspect Pick"
 msgstr ""
 
-msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_done"
+msgctxt "model:ir.action,name:wizard_stock_shipment_out_return_inspect_do"
 msgid "Inspect Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action,name:wizard_stock_shipment_out_return_inspect_receive"
 msgid "Inspect Reception"
 msgstr ""
```

### Comparing `trytond_quality-7.2.0/message.xml` & `trytond_quality-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/production.py` & `trytond_quality-7.2.1/production.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/production.xml` & `trytond_quality-7.2.1/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/quality.py` & `trytond_quality-7.2.1/quality.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/quality.xml` & `trytond_quality-7.2.1/quality.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/setup.py` & `trytond_quality-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/stock.py` & `trytond_quality-7.2.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/stock.xml` & `trytond_quality-7.2.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/tests/scenario_quality_control_shipment.rst` & `trytond_quality-7.2.1/tests/scenario_quality_control_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/tests/scenario_quality_inspection.rst` & `trytond_quality-7.2.1/tests/scenario_quality_inspection.rst`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/tox.ini` & `trytond_quality-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/trytond_quality.egg-info/PKG-INFO` & `trytond_quality-7.2.1/trytond_quality.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_quality
-Version: 7.2.0
+Version: 7.2.1
 Summary: Quality Management
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_quality-7.2.0/trytond_quality.egg-info/SOURCES.txt` & `trytond_quality-7.2.1/trytond_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/view/quality_alert_form.xml` & `trytond_quality-7.2.1/view/quality_alert_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/view/quality_control_form.xml` & `trytond_quality-7.2.1/view/quality_control_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/view/quality_control_list.xml` & `trytond_quality-7.2.1/view/quality_control_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/view/quality_control_point_form.xml` & `trytond_quality-7.2.1/view/quality_control_point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_quality-7.2.0/view/quality_inspection_form.xml` & `trytond_quality-7.2.1/view/quality_inspection_form.xml`

 * *Files identical despite different names*

