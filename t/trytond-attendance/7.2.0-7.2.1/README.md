# Comparing `tmp/trytond_attendance-7.2.0.tar.gz` & `tmp/trytond_attendance-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_attendance-7.2.0.tar", last modified: Mon Apr 29 15:38:11 2024, max compression
+gzip compressed data, was "trytond_attendance-7.2.1.tar", last modified: Wed May  1 12:06:52 2024, max compression
```

## Comparing `trytond_attendance-7.2.0.tar` & `trytond_attendance-7.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-29 15:18:00.000000 trytond_attendance-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:17:59.000000 trytond_attendance-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35310 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-02-04 18:51:26.000000 trytond_attendance-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/attendance.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13717 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/attendance.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:04.000000 trytond_attendance-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/icons/tryton-attendance.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-29 13:17:17.000000 trytond_attendance-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6277 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6530 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6252 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6374 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5093 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6223 2024-04-29 13:17:17.000000 trytond_attendance-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6205 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5161 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4445 2024-03-17 11:01:36.000000 trytond_attendance-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2472 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance_sheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:04.000000 trytond_attendance-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:17:55.000000 trytond_attendance-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/trytond_attendance.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/attendance_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/attendance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_form_timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_list_timesheet.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.115157 trytond_attendance-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      921 2024-05-01 12:06:48.000000 trytond_attendance-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-05-01 12:06:48.000000 trytond_attendance-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35310 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-05-01 12:06:52.115157 trytond_attendance-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/attendance.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13717 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/attendance.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.111824 trytond_attendance-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.111824 trytond_attendance-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/icons/tryton-attendance.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.111824 trytond_attendance-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6277 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6530 2024-04-30 17:21:59.000000 trytond_attendance-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6252 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6374 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-30 17:21:59.000000 trytond_attendance-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5093 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6223 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6205 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5161 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:06:52.115157 trytond_attendance-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4445 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.111824 trytond_attendance-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/scenario_attendance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2472 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/scenario_attendance_sheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/scenario_attendance_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-30 17:21:06.000000 trytond_attendance-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.115157 trytond_attendance-7.2.1/trytond_attendance.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-05-01 12:06:52.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:06:51.000000 trytond_attendance-7.2.1/trytond_attendance.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:06:52.115157 trytond_attendance-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/attendance_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/attendance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_form_timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_attendance-7.2.1/view/sheet_list_timesheet.xml
```

### Comparing `trytond_attendance-7.2.0/CHANGELOG` & `trytond_attendance-7.2.1/CHANGELOG`

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

### Comparing `trytond_attendance-7.2.0/COPYRIGHT` & `trytond_attendance-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/LICENSE` & `trytond_attendance-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/PKG-INFO` & `trytond_attendance-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_attendance
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for recording employee attendance
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_attendance-7.2.0/__init__.py` & `trytond_attendance-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/attendance.py` & `trytond_attendance-7.2.1/attendance.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/attendance.xml` & `trytond_attendance-7.2.1/attendance.xml`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/doc/conf.py` & `trytond_attendance-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/doc/index.rst` & `trytond_attendance-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/icons/LICENSE` & `trytond_attendance-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/ir.py` & `trytond_attendance-7.2.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/bg.po` & `trytond_attendance-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/ca.po` & `trytond_attendance-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/cs.po` & `trytond_attendance-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/de.po` & `trytond_attendance-7.2.1/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -168,43 +168,43 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_admin"
 msgid "Any attendance"
 msgstr "Alle Anwesenheiten"
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_period_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet"
 msgid "Own attendance sheet"
 msgstr "Eigene Anwesenheitsliste"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_admin"
 msgid "Any attendance sheet"
 msgstr "Alle Anwesenheitslisten"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line"
 msgid "Own attendance sheet line"
 msgstr "Eigene Anwesenheitseinträge"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line_admin"
 msgid "Any attendance sheet line"
 msgstr "Alle Anwesenheitseinträge"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_attendance"
 msgid "Attendances"
 msgstr "Anwesenheiten"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
```

### Comparing `trytond_attendance-7.2.0/locale/es.po` & `trytond_attendance-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/es_419.po` & `trytond_attendance-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/et.po` & `trytond_attendance-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/fa.po` & `trytond_attendance-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/fi.po` & `trytond_attendance-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/fr.po` & `trytond_attendance-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/hu.po` & `trytond_attendance-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/id.po` & `trytond_attendance-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/it.po` & `trytond_attendance-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/lo.po` & `trytond_attendance-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/lt.po` & `trytond_attendance-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/nl.po` & `trytond_attendance-7.2.1/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -125,29 +125,29 @@
 msgctxt "model:ir.action,name:act_sheet"
 msgid "Sheets"
 msgstr "Staten"
 
 msgctxt "model:ir.message,text:msg_close_period_previous_open"
 msgid "To close period \"%(period)s\" you must first close \"%(other_period)s\"."
 msgstr ""
-"Om periode \"%(period)s\" te sluiten, moet u eerst \"% other_period)s\" "
+"Om periode \"%(period)s\" te sluiten, moet u eerst \"%(other_period)s\" "
 "sluiten."
 
 msgctxt "model:ir.message,text:msg_delete_period_close"
 msgid "To delete attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 "Om aanwezigheid \"%(attendance)s\" te verwijderen, moet u periode "
 "\"%(period)s\" opnieuw openen."
 
 msgctxt "model:ir.message,text:msg_draft_period_previous_closed"
 msgid ""
 "To change period \"%(period)s\" you must first change \"%(other_period)s\" "
 "to draft."
 msgstr ""
-"Om periode \"%(period)s\" te sluiten, moet u eerst \"% other_period)s\" "
+"Om periode \"%(period)s\" te sluiten, moet u eerst \"%(other_period)s\" "
 "terug in concept zetten."
 
 msgctxt "model:ir.message,text:msg_modify_period_close"
 msgid "To modify attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 "Om aanwezigheid \"%(attendance)s\" te wijzigen, moet u periode "
 "\"%(period)s\" opnieuw openen."
```

### Comparing `trytond_attendance-7.2.0/locale/pl.po` & `trytond_attendance-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/pt.po` & `trytond_attendance-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/ro.po` & `trytond_attendance-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/ru.po` & `trytond_attendance-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/sl.po` & `trytond_attendance-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/tr.po` & `trytond_attendance-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/uk.po` & `trytond_attendance-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/locale/zh_CN.po` & `trytond_attendance-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/message.xml` & `trytond_attendance-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/setup.py` & `trytond_attendance-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/tests/scenario_attendance.rst` & `trytond_attendance-7.2.1/tests/scenario_attendance.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/tests/scenario_attendance_sheet.rst` & `trytond_attendance-7.2.1/tests/scenario_attendance_sheet.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/tests/scenario_attendance_timesheet.rst` & `trytond_attendance-7.2.1/tests/scenario_attendance_timesheet.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/tox.ini` & `trytond_attendance-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.2.0/trytond_attendance.egg-info/PKG-INFO` & `trytond_attendance-7.2.1/trytond_attendance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_attendance
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for recording employee attendance
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_attendance-7.2.0/trytond_attendance.egg-info/SOURCES.txt` & `trytond_attendance-7.2.1/trytond_attendance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

