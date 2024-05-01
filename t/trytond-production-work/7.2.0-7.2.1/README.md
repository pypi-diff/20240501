# Comparing `tmp/trytond_production_work-7.2.0.tar.gz` & `tmp/trytond_production_work-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_work-7.2.0.tar", last modified: Mon Apr 29 15:44:27 2024, max compression
+gzip compressed data, was "trytond_production_work-7.2.1.tar", last modified: Wed May  1 11:51:48 2024, max compression
```

## Comparing `trytond_production_work-7.2.0.tar` & `trytond_production_work-7.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1716 2024-04-29 15:22:51.000000 trytond_production_work-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-04-29 15:22:50.000000 trytond_production_work-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.813110 trytond_production_work-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_work-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.816444 trytond_production_work-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7172 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6990 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7093 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7025 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6136 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6549 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6854 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6329 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7025 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6784 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6621 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7227 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6400 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6891 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6624 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6691 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7032 2024-04-29 13:17:17.000000 trytond_production_work-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6878 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6650 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5968 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6574 2024-04-27 16:43:25.000000 trytond_production_work-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)      734 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1139 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-03-17 11:01:36.000000 trytond_production_work-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.816444 trytond_production_work-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7987 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/tests/scenario_production_work.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_work-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-29 15:22:46.000000 trytond_production_work-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/trytond_production_work.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:27.000000 trytond_production_work-7.2.0/trytond_production_work.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:27.819777 trytond_production_work-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_center_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_center_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_center_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      690 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_cycle_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-01-16 14:00:21.000000 trytond_production_work-7.2.0/view/work_cycle_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_production_work-7.2.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/view/work_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14680 2024-02-04 18:51:26.000000 trytond_production_work-7.2.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14850 2024-04-27 16:30:39.000000 trytond_production_work-7.2.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.258797 trytond_production_work-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-05-01 11:51:45.000000 trytond_production_work-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2024-05-01 11:51:44.000000 trytond_production_work-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-05-01 11:51:48.255464 trytond_production_work-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.252131 trytond_production_work-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.255464 trytond_production_work-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7172 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6990 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7093 2024-04-30 17:21:59.000000 trytond_production_work-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7025 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6136 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6549 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6854 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6329 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7022 2024-04-30 17:21:59.000000 trytond_production_work-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6784 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6138 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6621 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7227 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6400 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6891 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6624 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6691 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7032 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6878 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6650 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5968 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6574 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      734 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1139 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:51:48.258797 trytond_production_work-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.255464 trytond_production_work-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7987 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/tests/scenario_production_work.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2024-04-30 17:21:06.000000 trytond_production_work-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.255464 trytond_production_work-7.2.1/trytond_production_work.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-05-01 11:51:48.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:51:47.000000 trytond_production_work-7.2.1/trytond_production_work.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:51:48.255464 trytond_production_work-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_center_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_center_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_center_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_center_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_center_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      690 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_cycle_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_cycle_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/view/work_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14680 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14850 2024-04-30 17:21:00.000000 trytond_production_work-7.2.1/work.xml
```

### Comparing `trytond_production_work-7.2.0/CHANGELOG` & `trytond_production_work-7.2.1/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_production_work-7.2.0/COPYRIGHT` & `trytond_production_work-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/LICENSE` & `trytond_production_work-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/PKG-INFO` & `trytond_production_work-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production_work
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for production work
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production_work-7.2.0/README.rst` & `trytond_production_work-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/doc/conf.py` & `trytond_production_work-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/doc/index.rst` & `trytond_production_work-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/bg.po` & `trytond_production_work-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/ca.po` & `trytond_production_work-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/cs.po` & `trytond_production_work-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/de.po` & `trytond_production_work-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -196,23 +196,23 @@
 
 msgctxt "model:ir.model.button,string:work_stop_button"
 msgid "Stop"
 msgstr "Stop"
 
 msgctxt "model:ir.rule.group,name:rule_group_work_center_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_work_cycle_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_category_list"
 msgid "Work Center Categories"
 msgstr "Arbeitsplatzkategorien"
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_list"
 msgid "Work Centers"
```

### Comparing `trytond_production_work-7.2.0/locale/es.po` & `trytond_production_work-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/es_419.po` & `trytond_production_work-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/et.po` & `trytond_production_work-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/fa.po` & `trytond_production_work-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/fi.po` & `trytond_production_work-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/fr.po` & `trytond_production_work-7.2.1/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 msgstr ""
 "Pour supprimer le travail « %(work)s », il doit être dans l'état « requête »"
 " ou « brouillon »."
 
 msgctxt "model:ir.message,text:msg_do_finished_work"
 msgid "To complete production \"%(production)s\", work \"%(work)s\" must be finished."
 msgstr ""
-"Pour terminer la production « %(production)s », le travail « %(travail)s » "
-"doit être terminé."
+"Pour terminer la production « %(production)s », le travail « %(work)s » doit"
+" être terminé."
 
 msgctxt "model:ir.message,text:msg_missing_work_center"
 msgid ""
 "Could not find a work center of category \"%(category)s\" under "
 "\"%(parent)s\"."
 msgstr ""
 "Impossible de trouver un poste de travail de la catégorie « %(category)s » "
```

### Comparing `trytond_production_work-7.2.0/locale/hu.po` & `trytond_production_work-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/id.po` & `trytond_production_work-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/it.po` & `trytond_production_work-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/lo.po` & `trytond_production_work-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/lt.po` & `trytond_production_work-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/nl.po` & `trytond_production_work-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/pl.po` & `trytond_production_work-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/pt.po` & `trytond_production_work-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/ro.po` & `trytond_production_work-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/ru.po` & `trytond_production_work-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/sl.po` & `trytond_production_work-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/tr.po` & `trytond_production_work-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/uk.po` & `trytond_production_work-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/locale/zh_CN.po` & `trytond_production_work-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/message.xml` & `trytond_production_work-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/production.py` & `trytond_production_work-7.2.1/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/production.xml` & `trytond_production_work-7.2.1/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/routing.py` & `trytond_production_work-7.2.1/routing.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/routing.xml` & `trytond_production_work-7.2.1/routing.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/setup.py` & `trytond_production_work-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/tests/scenario_production_work.rst` & `trytond_production_work-7.2.1/tests/scenario_production_work.rst`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/tox.ini` & `trytond_production_work-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/trytond_production_work.egg-info/PKG-INFO` & `trytond_production_work-7.2.1/trytond_production_work.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production_work
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for production work
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production_work-7.2.0/trytond_production_work.egg-info/SOURCES.txt` & `trytond_production_work-7.2.1/trytond_production_work.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/view/production_form.xml` & `trytond_production_work-7.2.1/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/view/work_center_form.xml` & `trytond_production_work-7.2.1/view/work_center_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/view/work_cycle_form.xml` & `trytond_production_work-7.2.1/view/work_cycle_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/view/work_form.xml` & `trytond_production_work-7.2.1/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/work.py` & `trytond_production_work-7.2.1/work.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-7.2.0/work.xml` & `trytond_production_work-7.2.1/work.xml`

 * *Files identical despite different names*

