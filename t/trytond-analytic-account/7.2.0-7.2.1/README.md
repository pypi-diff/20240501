# Comparing `tmp/trytond_analytic_account-7.2.0.tar.gz` & `tmp/trytond_analytic_account-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_account-7.2.0.tar", last modified: Mon Apr 29 15:37:38 2024, max compression
+gzip compressed data, was "trytond_analytic_account-7.2.1.tar", last modified: Wed May  1 12:08:04 2024, max compression
```

## Comparing `trytond_analytic_account-7.2.0.tar` & `trytond_analytic_account-7.2.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.037161 trytond_analytic_account-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3596 2024-04-29 15:17:34.000000 trytond_analytic_account-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:17:34.000000 trytond_analytic_account-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17400 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8975 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.030495 trytond_analytic_account-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_analytic_account-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10602 2024-03-17 11:01:36.000000 trytond_analytic_account-7.2.0/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5436 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.030495 trytond_analytic_account-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8477 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7714 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8509 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7431 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8091 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8877 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7701 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8633 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8094 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7729 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8383 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8942 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7877 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8675 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7919 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8267 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8576 2024-04-29 13:17:17.000000 trytond_analytic_account-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8610 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8493 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7692 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7334 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7932 2024-04-27 16:43:22.000000 trytond_analytic_account-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-27 16:30:39.000000 trytond_analytic_account-7.2.0/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:38.037161 trytond_analytic_account-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-03-17 11:01:36.000000 trytond_analytic_account-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7642 2024-04-22 12:14:36.000000 trytond_analytic_account-7.2.0/tests/scenario_analytic_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11115 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_analytic_account-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-29 15:17:30.000000 trytond_analytic_account-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2483 2024-04-29 15:37:38.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:37.000000 trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:38.033828 trytond_analytic_account-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/account_distribution_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_distribution_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/analytic_account_entry_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/analytic_account_entry_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_analytic_account-7.2.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-02-04 18:51:26.000000 trytond_analytic_account-7.2.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_analytic_account-7.2.0/view/rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.913253 trytond_analytic_account-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2024-05-01 12:08:01.000000 trytond_analytic_account-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:08:01.000000 trytond_analytic_account-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-05-01 12:08:04.913253 trytond_analytic_account-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17400 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8975 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.903254 trytond_analytic_account-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10602 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5436 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.906587 trytond_analytic_account-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8477 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7714 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8643 2024-04-30 17:21:59.000000 trytond_analytic_account-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8509 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7431 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8091 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8877 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7701 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8633 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8094 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7729 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8383 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8942 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7877 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8675 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7919 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8267 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8576 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8610 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8493 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7692 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7334 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7932 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:08:04.913253 trytond_analytic_account-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.909920 trytond_analytic_account-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7642 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/tests/scenario_analytic_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11115 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2024-04-30 17:21:06.000000 trytond_analytic_account-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.909920 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2483 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:08:04.000000 trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:08:04.909920 trytond_analytic_account-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_distribution_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_distribution_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/analytic_account_entry_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/analytic_account_entry_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2024-04-30 17:20:59.000000 trytond_analytic_account-7.2.1/view/rule_list.xml
```

### Comparing `trytond_analytic_account-7.2.0/CHANGELOG` & `trytond_analytic_account-7.2.1/CHANGELOG`

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

### Comparing `trytond_analytic_account-7.2.0/COPYRIGHT` & `trytond_analytic_account-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/LICENSE` & `trytond_analytic_account-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/PKG-INFO` & `trytond_analytic_account-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_account
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for analytic accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_analytic_account-7.2.0/README.rst` & `trytond_analytic_account-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/__init__.py` & `trytond_analytic_account-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/account.py` & `trytond_analytic_account-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/account.xml` & `trytond_analytic_account-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/analytic_account.xml` & `trytond_analytic_account-7.2.1/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/doc/conf.py` & `trytond_analytic_account-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/doc/index.rst` & `trytond_analytic_account-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/line.py` & `trytond_analytic_account-7.2.1/line.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/line.xml` & `trytond_analytic_account-7.2.1/line.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/bg.po` & `trytond_analytic_account-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/ca.po` & `trytond_analytic_account-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/cs.po` & `trytond_analytic_account-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/de.po` & `trytond_analytic_account-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -249,27 +249,27 @@
 
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
 msgstr "Kostenstelle Regeln anwenden"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
 msgstr "Konten"
 
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
```

### Comparing `trytond_analytic_account-7.2.0/locale/es.po` & `trytond_analytic_account-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/es_419.po` & `trytond_analytic_account-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/et.po` & `trytond_analytic_account-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/fa.po` & `trytond_analytic_account-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/fi.po` & `trytond_analytic_account-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/fr.po` & `trytond_analytic_account-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/hu.po` & `trytond_analytic_account-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/id.po` & `trytond_analytic_account-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/it.po` & `trytond_analytic_account-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/lo.po` & `trytond_analytic_account-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/lt.po` & `trytond_analytic_account-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/nl.po` & `trytond_analytic_account-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/pl.po` & `trytond_analytic_account-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/pt.po` & `trytond_analytic_account-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/ro.po` & `trytond_analytic_account-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/ru.po` & `trytond_analytic_account-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/sl.po` & `trytond_analytic_account-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/tr.po` & `trytond_analytic_account-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/uk.po` & `trytond_analytic_account-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/locale/zh_CN.po` & `trytond_analytic_account-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/message.xml` & `trytond_analytic_account-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/rule.py` & `trytond_analytic_account-7.2.1/rule.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/rule.xml` & `trytond_analytic_account-7.2.1/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/setup.py` & `trytond_analytic_account-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/tests/scenario_analytic_account.rst` & `trytond_analytic_account-7.2.1/tests/scenario_analytic_account.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/tests/test_module.py` & `trytond_analytic_account-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/tox.ini` & `trytond_analytic_account-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/PKG-INFO` & `trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_account
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for analytic accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_analytic_account-7.2.0/trytond_analytic_account.egg-info/SOURCES.txt` & `trytond_analytic_account-7.2.1/trytond_analytic_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/view/account_form.xml` & `trytond_analytic_account-7.2.1/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/view/move_line_list.xml` & `trytond_analytic_account-7.2.1/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-7.2.0/view/rule_form.xml` & `trytond_analytic_account-7.2.1/view/rule_form.xml`

 * *Files identical despite different names*

