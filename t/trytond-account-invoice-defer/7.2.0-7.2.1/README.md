# Comparing `tmp/trytond_account_invoice_defer-7.2.0.tar.gz` & `tmp/trytond_account_invoice_defer-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_defer-7.2.0.tar", last modified: Mon Apr 29 15:33:48 2024, max compression
+gzip compressed data, was "trytond_account_invoice_defer-7.2.1.tar", last modified: Wed May  1 12:21:17 2024, max compression
```

## Comparing `trytond_account_invoice_defer-7.2.0.tar` & `trytond_account_invoice_defer-7.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      828 2024-04-29 15:14:26.000000 trytond_account_invoice_defer-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:14:25.000000 trytond_account_invoice_defer-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18660 2024-03-17 11:01:36.000000 trytond_account_invoice_defer-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.969819 trytond_account_invoice_defer-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:55.000000 trytond_account_invoice_defer-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5844 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5849 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4801 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5896 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4856 2024-04-29 13:17:17.000000 trytond_account_invoice_defer-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-27 16:43:21.000000 trytond_account_invoice_defer-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4651 2024-04-27 16:30:39.000000 trytond_account_invoice_defer-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3862 2024-04-22 12:14:36.000000 trytond_account_invoice_defer-7.2.0/tests/scenario_account_invoice_defer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-01-27 09:58:52.000000 trytond_account_invoice_defer-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:55.000000 trytond_account_invoice_defer-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:14:20.000000 trytond_account_invoice_defer-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:33:48.000000 trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:33:48.973152 trytond_account_invoice_defer-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-02-04 18:51:26.000000 trytond_account_invoice_defer-7.2.0/view/invoice_deferred_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/invoice_deferred_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-7.2.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2024-05-01 12:21:14.000000 trytond_account_invoice_defer-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 12:21:14.000000 trytond_account_invoice_defer-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18660 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.819667 trytond_account_invoice_defer-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1844 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5844 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6117 2024-04-30 17:21:59.000000 trytond_account_invoice_defer-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5849 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4801 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5896 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4856 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4651 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3862 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tests/scenario_account_invoice_defer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-30 17:21:06.000000 trytond_account_invoice_defer-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:21:17.000000 trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:17.823000 trytond_account_invoice_defer-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/view/invoice_deferred_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/view/invoice_deferred_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_account_invoice_defer-7.2.1/view/invoice_line_form.xml
```

### Comparing `trytond_account_invoice_defer-7.2.0/CHANGELOG` & `trytond_account_invoice_defer-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_invoice_defer-7.2.0/COPYRIGHT` & `trytond_account_invoice_defer-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/LICENSE` & `trytond_account_invoice_defer-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/PKG-INFO` & `trytond_account_invoice_defer-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_defer
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_defer-7.2.0/__init__.py` & `trytond_account_invoice_defer-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/account.py` & `trytond_account_invoice_defer-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/account.xml` & `trytond_account_invoice_defer-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/doc/conf.py` & `trytond_account_invoice_defer-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/doc/design.rst` & `trytond_account_invoice_defer-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/bg.po` & `trytond_account_invoice_defer-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/ca.po` & `trytond_account_invoice_defer-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/cs.po` & `trytond_account_invoice_defer-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/de.po` & `trytond_account_invoice_defer-7.2.1/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 
 msgctxt "model:ir.message,text:msg_invoice_deferred_running_close_period"
 msgid ""
 "You cannot close period \"%(period)s\" because some invoices deferred "
 "\"%(deferrals)s\" do not have yet move for the period."
 msgstr ""
 "Der Buchungszeitraum \"%(period)s\" kann nicht geschlossen werden, da für "
-"einige Rechnungsabgrenzungsposten noch keine Buchungssätze erstellt wurden."
+"die Rechnungsabgrenzungsposten \"%(deferrals)s\" noch keine Buchungssätze "
+"für den Buchungszeitraum erstellt wurden."
 
 msgctxt "model:ir.message,text:msg_missing_deferred_account_expense"
 msgid "There is no deferred account expense configured."
 msgstr "Es wurde kein Konto für die aktive Rechnungsabgrenzung konfiguriert."
 
 msgctxt "model:ir.message,text:msg_missing_deferred_account_revenue"
 msgid "There is no deferred account revenue configured."
@@ -156,15 +157,15 @@
 
 msgctxt "model:ir.model.button,string:invoice_deferred_run_button"
 msgid "Run"
 msgstr "Ausführen"
 
 msgctxt "model:ir.rule.group,name:rule_group_invoice_deferred_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_deferred_create_moves"
 msgid "Create Invoices Deferred Moves"
 msgstr "Buchungssätze für Rechnungsabgrenzung erstellen"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_deferred_in_form"
 msgid "Supplier Invoices Deferred"
```

### Comparing `trytond_account_invoice_defer-7.2.0/locale/es.po` & `trytond_account_invoice_defer-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/es_419.po` & `trytond_account_invoice_defer-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/et.po` & `trytond_account_invoice_defer-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/fa.po` & `trytond_account_invoice_defer-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/fi.po` & `trytond_account_invoice_defer-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/fr.po` & `trytond_account_invoice_defer-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/hu.po` & `trytond_account_invoice_defer-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/id.po` & `trytond_account_invoice_defer-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/it.po` & `trytond_account_invoice_defer-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/lo.po` & `trytond_account_invoice_defer-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/lt.po` & `trytond_account_invoice_defer-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/nl.po` & `trytond_account_invoice_defer-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/pl.po` & `trytond_account_invoice_defer-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/pt.po` & `trytond_account_invoice_defer-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/ro.po` & `trytond_account_invoice_defer-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/ru.po` & `trytond_account_invoice_defer-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/sl.po` & `trytond_account_invoice_defer-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/tr.po` & `trytond_account_invoice_defer-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/uk.po` & `trytond_account_invoice_defer-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/locale/zh_CN.po` & `trytond_account_invoice_defer-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/message.xml` & `trytond_account_invoice_defer-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/setup.py` & `trytond_account_invoice_defer-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/tests/scenario_account_invoice_defer.rst` & `trytond_account_invoice_defer-7.2.1/tests/scenario_account_invoice_defer.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/tests/tools.py` & `trytond_account_invoice_defer-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/tox.ini` & `trytond_account_invoice_defer-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/PKG-INFO` & `trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_defer
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_defer-7.2.0/trytond_account_invoice_defer.egg-info/SOURCES.txt` & `trytond_account_invoice_defer-7.2.1/trytond_account_invoice_defer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-7.2.0/view/invoice_deferred_form.xml` & `trytond_account_invoice_defer-7.2.1/view/invoice_deferred_form.xml`

 * *Files identical despite different names*

