# Comparing `tmp/trytond_project_invoice-7.2.0.tar.gz` & `tmp/trytond_project_invoice-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_invoice-7.2.0.tar", last modified: Mon Apr 29 15:44:48 2024, max compression
+gzip compressed data, was "trytond_project_invoice-7.2.1.tar", last modified: Wed May  1 11:45:15 2024, max compression
```

## Comparing `trytond_project_invoice-7.2.0.tar` & `trytond_project_invoice-7.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2335 2024-04-29 15:23:08.000000 trytond_project_invoice-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:23:08.000000 trytond_project_invoice-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_invoice-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.342573 trytond_project_invoice-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project_invoice-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4804 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.342573 trytond_project_invoice-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4615 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5770 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5557 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4397 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4628 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5020 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5658 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4313 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4275 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4981 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4569 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5452 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4331 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4709 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4563 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2235 2024-02-04 18:51:26.000000 trytond_project_invoice-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    26656 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/project.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3160 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-03-17 11:01:36.000000 trytond_project_invoice-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_effort.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3272 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_multiple_party.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6024 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_progress.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6908 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-02-04 18:51:26.000000 trytond_project_invoice-7.2.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1515 2024-01-27 09:58:52.000000 trytond_project_invoice-7.2.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project_invoice-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-29 15:23:03.000000 trytond_project_invoice-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2164 2024-04-29 15:44:48.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-01-27 09:58:52.000000 trytond_project_invoice-7.2.0/view/timesheet_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_invoiced_progress_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_invoiced_progress_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.425738 trytond_project_invoice-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2436 2024-05-01 11:45:12.000000 trytond_project_invoice-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:45:11.000000 trytond_project_invoice-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-05-01 11:45:15.425738 trytond_project_invoice-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.419072 trytond_project_invoice-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4804 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.422405 trytond_project_invoice-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4615 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5770 2024-04-30 17:21:59.000000 trytond_project_invoice-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5557 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4397 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4628 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5020 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5658 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4313 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4275 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4981 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4569 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5452 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4331 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4709 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4563 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2235 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26656 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/project.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3160 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:45:15.425738 trytond_project_invoice-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.422405 trytond_project_invoice-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/scenario_project_invoice_effort.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3272 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/scenario_project_invoice_multiple_party.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6024 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/scenario_project_invoice_progress.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6908 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/scenario_project_invoice_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1515 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-30 17:21:06.000000 trytond_project_invoice-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.422405 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2164 2024-05-01 11:45:15.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:45:14.000000 trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:45:15.422405 trytond_project_invoice-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/view/timesheet_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/view/work_invoiced_progress_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/view/work_invoiced_progress_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:21:00.000000 trytond_project_invoice-7.2.1/view/work_list.xml
```

### Comparing `trytond_project_invoice-7.2.0/CHANGELOG` & `trytond_project_invoice-7.2.1/CHANGELOG`

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

### Comparing `trytond_project_invoice-7.2.0/COPYRIGHT` & `trytond_project_invoice-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/LICENSE` & `trytond_project_invoice-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/PKG-INFO` & `trytond_project_invoice-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_project_invoice
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to invoice projects
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_project_invoice-7.2.0/__init__.py` & `trytond_project_invoice-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/doc/conf.py` & `trytond_project_invoice-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/invoice.py` & `trytond_project_invoice-7.2.1/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/bg.po` & `trytond_project_invoice-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/ca.po` & `trytond_project_invoice-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/cs.po` & `trytond_project_invoice-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/de.po` & `trytond_project_invoice-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 msgstr ""
 "Die Aufgabe von Zeiterfassungsposition \"%(line)s\" kann nicht mehr geändert"
 " werden, weil diese bereits in Rechnung gestellt ist."
 
 msgctxt "model:ir.message,text:msg_invoiced_work_delete"
 msgid "You cannot delete work \"%(work)s\" because it has been invoiced."
 msgstr ""
-"Die Projektaufgabe \"%(line)s\" kann nicht mehr gelöscht werden, weil diese "
+"Die Projektaufgabe \"%(work)s\" kann nicht mehr gelöscht werden, weil diese "
 "bereits in Rechnung gestellt ist."
 
 msgctxt "model:ir.message,text:msg_invoiced_work_modify_effort"
 msgid ""
 "You cannot modify the effort of work \"%(work)s\" because it has been "
 "invoiced."
 msgstr ""
```

### Comparing `trytond_project_invoice-7.2.0/locale/es.po` & `trytond_project_invoice-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/es_419.po` & `trytond_project_invoice-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/et.po` & `trytond_project_invoice-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/fa.po` & `trytond_project_invoice-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/fi.po` & `trytond_project_invoice-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/fr.po` & `trytond_project_invoice-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/hu.po` & `trytond_project_invoice-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/id.po` & `trytond_project_invoice-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/it.po` & `trytond_project_invoice-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/lo.po` & `trytond_project_invoice-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/lt.po` & `trytond_project_invoice-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/nl.po` & `trytond_project_invoice-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/pl.po` & `trytond_project_invoice-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/pt.po` & `trytond_project_invoice-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/ro.po` & `trytond_project_invoice-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/ru.po` & `trytond_project_invoice-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/sl.po` & `trytond_project_invoice-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/tr.po` & `trytond_project_invoice-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/uk.po` & `trytond_project_invoice-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/locale/zh_CN.po` & `trytond_project_invoice-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/message.xml` & `trytond_project_invoice-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/project.py` & `trytond_project_invoice-7.2.1/project.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/project.xml` & `trytond_project_invoice-7.2.1/project.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/setup.py` & `trytond_project_invoice-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_effort.rst` & `trytond_project_invoice-7.2.1/tests/scenario_project_invoice_effort.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_multiple_party.rst` & `trytond_project_invoice-7.2.1/tests/scenario_project_invoice_multiple_party.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_progress.rst` & `trytond_project_invoice-7.2.1/tests/scenario_project_invoice_progress.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_timesheet.rst` & `trytond_project_invoice-7.2.1/tests/scenario_project_invoice_timesheet.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/timesheet.py` & `trytond_project_invoice-7.2.1/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/timesheet.xml` & `trytond_project_invoice-7.2.1/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/tox.ini` & `trytond_project_invoice-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/PKG-INFO` & `trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_project_invoice
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to invoice projects
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/SOURCES.txt` & `trytond_project_invoice-7.2.1/trytond_project_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/view/work_form.xml` & `trytond_project_invoice-7.2.1/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.2.0/view/work_invoiced_progress_form.xml` & `trytond_project_invoice-7.2.1/view/work_invoiced_progress_form.xml`

 * *Files identical despite different names*

