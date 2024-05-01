# Comparing `tmp/trytond_purchase_requisition-7.2.0.tar.gz` & `tmp/trytond_purchase_requisition-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_requisition-7.2.0.tar", last modified: Mon Apr 29 15:46:26 2024, max compression
+gzip compressed data, was "trytond_purchase_requisition-7.2.1.tar", last modified: Wed May  1 11:33:37 2024, max compression
```

## Comparing `trytond_purchase_requisition-7.2.0.tar` & `trytond_purchase_requisition-7.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1965 2024-04-29 15:24:10.000000 trytond_purchase_requisition-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-29 15:24:10.000000 trytond_purchase_requisition-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2024-02-04 18:51:26.000000 trytond_purchase_requisition-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.080017 trytond_purchase_requisition-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_purchase_requisition-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_requisition-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      822 2024-04-29 13:17:17.000000 trytond_purchase_requisition-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.080017 trytond_purchase_requisition-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6834 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6970 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6840 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6555 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7142 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7009 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6139 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6823 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6522 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6907 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6687 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6871 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6364 2024-04-29 13:17:17.000000 trytond_purchase_requisition-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6785 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5890 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-27 16:43:26.000000 trytond_purchase_requisition-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    25975 2024-04-22 12:14:36.000000 trytond_purchase_requisition-7.2.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15423 2024-04-27 16:30:39.000000 trytond_purchase_requisition-7.2.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4533 2024-03-17 11:01:36.000000 trytond_purchase_requisition-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11285 2024-04-22 12:14:36.000000 trytond_purchase_requisition-7.2.0/tests/scenario_purchase_requisition.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_requisition-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-29 15:24:06.000000 trytond_purchase_requisition-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1991 2024-04-29 15:46:26.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:25.000000 trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:26.083350 trytond_purchase_requisition-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:21.000000 trytond_purchase_requisition-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1837 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_purchase_requisition-7.2.0/view/purchase_requisition_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2066 2024-05-01 11:33:34.000000 trytond_purchase_requisition-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-05-01 11:33:34.000000 trytond_purchase_requisition-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.680654 trytond_purchase_requisition-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6834 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6970 2024-04-30 17:21:59.000000 trytond_purchase_requisition-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6840 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6555 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7142 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7009 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6139 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6823 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6522 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6907 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6687 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6871 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6364 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6785 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5890 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    25975 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15423 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4533 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11285 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/tests/scenario_purchase_requisition.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-30 17:21:06.000000 trytond_purchase_requisition-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1991 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:33:37.000000 trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:33:37.683987 trytond_purchase_requisition-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1837 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/purchase_requisition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/purchase_requisition_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/purchase_requisition_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/purchase_requisition_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2024-04-30 17:21:00.000000 trytond_purchase_requisition-7.2.1/view/purchase_requisition_tree.xml
```

### Comparing `trytond_purchase_requisition-7.2.0/CHANGELOG` & `trytond_purchase_requisition-7.2.1/CHANGELOG`

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

### Comparing `trytond_purchase_requisition-7.2.0/COPYRIGHT` & `trytond_purchase_requisition-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/LICENSE` & `trytond_purchase_requisition-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/PKG-INFO` & `trytond_purchase_requisition-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_requisition
-Version: 7.2.0
+Version: 7.2.1
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_requisition-7.2.0/README.rst` & `trytond_purchase_requisition-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/__init__.py` & `trytond_purchase_requisition-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/doc/conf.py` & `trytond_purchase_requisition-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/doc/index.rst` & `trytond_purchase_requisition-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/ir.py` & `trytond_purchase_requisition-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/bg.po` & `trytond_purchase_requisition-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/ca.po` & `trytond_purchase_requisition-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/cs.po` & `trytond_purchase_requisition-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/de.po` & `trytond_purchase_requisition-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_admin"
 msgid "Any requisition"
 msgstr "Alle Bestellanforderungen"
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_requisition_employees"
 msgid "Own requisition"
 msgstr "Eigene Bestellanforderungen"
 
 msgctxt "model:ir.sequence,name:sequence_purchase_requisition"
 msgid "Purchase Requisition"
```

### Comparing `trytond_purchase_requisition-7.2.0/locale/es.po` & `trytond_purchase_requisition-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/es_419.po` & `trytond_purchase_requisition-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/et.po` & `trytond_purchase_requisition-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/fa.po` & `trytond_purchase_requisition-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/fi.po` & `trytond_purchase_requisition-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/fr.po` & `trytond_purchase_requisition-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/hu.po` & `trytond_purchase_requisition-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/id.po` & `trytond_purchase_requisition-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/it.po` & `trytond_purchase_requisition-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/lo.po` & `trytond_purchase_requisition-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/lt.po` & `trytond_purchase_requisition-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/nl.po` & `trytond_purchase_requisition-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/pl.po` & `trytond_purchase_requisition-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/pt.po` & `trytond_purchase_requisition-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/ro.po` & `trytond_purchase_requisition-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/ru.po` & `trytond_purchase_requisition-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/sl.po` & `trytond_purchase_requisition-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/tr.po` & `trytond_purchase_requisition-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/uk.po` & `trytond_purchase_requisition-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/locale/zh_CN.po` & `trytond_purchase_requisition-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/message.xml` & `trytond_purchase_requisition-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/purchase.py` & `trytond_purchase_requisition-7.2.1/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/purchase.xml` & `trytond_purchase_requisition-7.2.1/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/setup.py` & `trytond_purchase_requisition-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/tests/scenario_purchase_requisition.rst` & `trytond_purchase_requisition-7.2.1/tests/scenario_purchase_requisition.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/tox.ini` & `trytond_purchase_requisition-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/PKG-INFO` & `trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_requisition
-Version: 7.2.0
+Version: 7.2.1
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_requisition-7.2.0/trytond_purchase_requisition.egg-info/SOURCES.txt` & `trytond_purchase_requisition-7.2.1/trytond_purchase_requisition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/view/purchase_requisition_form.xml` & `trytond_purchase_requisition-7.2.1/view/purchase_requisition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-7.2.0/view/purchase_requisition_line_form.xml` & `trytond_purchase_requisition-7.2.1/view/purchase_requisition_line_form.xml`

 * *Files identical despite different names*

