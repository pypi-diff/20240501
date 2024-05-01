# Comparing `tmp/trytond_timesheet-7.2.0.tar.gz` & `tmp/trytond_timesheet-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_timesheet-7.2.0.tar", last modified: Mon Apr 29 15:53:44 2024, max compression
+gzip compressed data, was "trytond_timesheet-7.2.1.tar", last modified: Wed May  1 09:51:46 2024, max compression
```

## Comparing `trytond_timesheet-7.2.0.tar` & `trytond_timesheet-7.2.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3216 2024-04-29 15:29:41.000000 trytond_timesheet-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:29:40.000000 trytond_timesheet-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2024-02-04 18:51:27.000000 trytond_timesheet-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.448552 trytond_timesheet-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_timesheet-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1387 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/doc/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.448552 trytond_timesheet-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/icons/tryton-timesheet.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-29 13:17:17.000000 trytond_timesheet-7.2.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11826 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14558 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.451885 trytond_timesheet-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9957 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9166 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11001 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10808 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9081 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9903 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11142 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9153 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10859 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9704 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8944 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9679 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10856 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9214 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10536 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9454 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10451 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10591 2024-04-29 13:17:17.000000 trytond_timesheet-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10099 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10216 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12208 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10331 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4582 2024-04-22 12:14:36.000000 trytond_timesheet-7.2.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2024-03-17 11:01:36.000000 trytond_timesheet-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.451885 trytond_timesheet-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_timesheet-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      146 2024-04-29 15:29:36.000000 trytond_timesheet-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2259 2024-04-29 15:53:44.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/user.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/hours_employee_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/hours_employee_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/hours_employee_monthly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/view/hours_employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/hours_employee_weekly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-09-12 21:17:04.000000 trytond_timesheet-7.2.0/view/line_enter_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/work_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      681 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/work_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_list_report.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6303 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5319 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3317 2024-05-01 09:51:43.000000 trytond_timesheet-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 09:51:43.000000 trytond_timesheet-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.332082 trytond_timesheet-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1387 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/doc/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.332082 trytond_timesheet-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/icons/tryton-timesheet.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11826 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14558 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9957 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9166 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11001 2024-04-30 17:21:59.000000 trytond_timesheet-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10808 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9081 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9903 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11142 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9153 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10859 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9704 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8944 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9679 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10856 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9214 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10536 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9457 2024-04-30 17:21:59.000000 trytond_timesheet-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10451 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10591 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10099 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10216 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12208 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10331 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4582 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      146 2024-04-30 17:21:06.000000 trytond_timesheet-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2259 2024-05-01 09:51:46.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:51:45.000000 trytond_timesheet-7.2.1/trytond_timesheet.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/user.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:46.335415 trytond_timesheet-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/hours_employee_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/hours_employee_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/hours_employee_monthly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/hours_employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/hours_employee_weekly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/line_enter_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/work_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      681 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/work_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/view/work_list_report.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6303 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5319 2024-04-30 17:21:00.000000 trytond_timesheet-7.2.1/work.xml
```

### Comparing `trytond_timesheet-7.2.0/CHANGELOG` & `trytond_timesheet-7.2.1/CHANGELOG`

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

### Comparing `trytond_timesheet-7.2.0/COPYRIGHT` & `trytond_timesheet-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/LICENSE` & `trytond_timesheet-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/PKG-INFO` & `trytond_timesheet-7.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with timesheets
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_timesheet-7.2.0/README.rst` & `trytond_timesheet-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/__init__.py` & `trytond_timesheet-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/doc/conf.py` & `trytond_timesheet-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/doc/index.rst` & `trytond_timesheet-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/doc/user_application.rst` & `trytond_timesheet-7.2.1/doc/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/icons/LICENSE` & `trytond_timesheet-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/ir.py` & `trytond_timesheet-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/line.py` & `trytond_timesheet-7.2.1/line.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/line.xml` & `trytond_timesheet-7.2.1/line.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/bg.po` & `trytond_timesheet-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/ca.po` & `trytond_timesheet-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/cs.po` & `trytond_timesheet-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/de.po` & `trytond_timesheet-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -294,19 +294,19 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
 msgstr "Alle Zeiterfassungspositionen"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Einstellungen"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
```

### Comparing `trytond_timesheet-7.2.0/locale/es.po` & `trytond_timesheet-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/es_419.po` & `trytond_timesheet-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/et.po` & `trytond_timesheet-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/fa.po` & `trytond_timesheet-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/fi.po` & `trytond_timesheet-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/fr.po` & `trytond_timesheet-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/hu.po` & `trytond_timesheet-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/id.po` & `trytond_timesheet-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/it.po` & `trytond_timesheet-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/lo.po` & `trytond_timesheet-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/lt.po` & `trytond_timesheet-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/nl.po` & `trytond_timesheet-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/pl.po` & `trytond_timesheet-7.2.1/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Raportowanie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 #, fuzzy
```

### Comparing `trytond_timesheet-7.2.0/locale/pt.po` & `trytond_timesheet-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/ro.po` & `trytond_timesheet-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/ru.po` & `trytond_timesheet-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/sl.po` & `trytond_timesheet-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/tr.po` & `trytond_timesheet-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/uk.po` & `trytond_timesheet-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/locale/zh_CN.po` & `trytond_timesheet-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/message.xml` & `trytond_timesheet-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/routes.py` & `trytond_timesheet-7.2.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/setup.py` & `trytond_timesheet-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/timesheet.xml` & `trytond_timesheet-7.2.1/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/tox.ini` & `trytond_timesheet-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/trytond_timesheet.egg-info/PKG-INFO` & `trytond_timesheet-7.2.1/trytond_timesheet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module with timesheets
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_timesheet-7.2.0/trytond_timesheet.egg-info/SOURCES.txt` & `trytond_timesheet-7.2.1/trytond_timesheet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/view/line_form.xml` & `trytond_timesheet-7.2.1/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/view/work_form.xml` & `trytond_timesheet-7.2.1/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/work.py` & `trytond_timesheet-7.2.1/work.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.2.0/work.xml` & `trytond_timesheet-7.2.1/work.xml`

 * *Files identical despite different names*

