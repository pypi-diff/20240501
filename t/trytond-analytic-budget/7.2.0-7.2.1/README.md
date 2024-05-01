# Comparing `tmp/trytond_analytic_budget-7.2.0.tar.gz` & `tmp/trytond_analytic_budget-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_budget-7.2.0.tar", last modified: Mon Apr 29 15:37:45 2024, max compression
+gzip compressed data, was "trytond_analytic_budget-7.2.1.tar", last modified: Wed May  1 12:07:40 2024, max compression
```

## Comparing `trytond_analytic_budget-7.2.0.tar` & `trytond_analytic_budget-7.2.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:17:39.000000 trytond_analytic_budget-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-29 15:17:39.000000 trytond_analytic_budget-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7903 2024-01-27 09:58:52.000000 trytond_analytic_budget-7.2.0/analytic_account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8405 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.410302 trytond_analytic_budget-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1336 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:03.000000 trytond_analytic_budget-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      948 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6125 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5869 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4916 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5876 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5023 2024-04-29 13:17:17.000000 trytond_analytic_budget-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4975 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-27 16:43:22.000000 trytond_analytic_budget-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:45.416968 trytond_analytic_budget-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4678 2024-04-27 16:30:39.000000 trytond_analytic_budget-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4419 2024-04-22 12:14:36.000000 trytond_analytic_budget-7.2.0/tests/scenario_analytic_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:03.000000 trytond_analytic_budget-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2024-04-29 15:17:35.000000 trytond_analytic_budget-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2042 2024-04-29 15:37:45.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      138 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:44.000000 trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:45.413635 trytond_analytic_budget-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      639 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_analytic_budget-7.2.0/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.407228 trytond_analytic_budget-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-05-01 12:07:37.000000 trytond_analytic_budget-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-05-01 12:07:36.000000 trytond_analytic_budget-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-05-01 12:07:40.407228 trytond_analytic_budget-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7903 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/analytic_account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8405 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.400561 trytond_analytic_budget-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1336 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      948 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.403895 trytond_analytic_budget-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6125 2024-04-30 17:21:59.000000 trytond_analytic_budget-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5869 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4916 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5876 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5023 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4975 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:07:40.407228 trytond_analytic_budget-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4678 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.403895 trytond_analytic_budget-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4419 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/tests/scenario_analytic_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2024-04-30 17:21:06.000000 trytond_analytic_budget-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.407228 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2915 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2042 2024-05-01 12:07:40.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      138 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:07:39.000000 trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:07:40.407228 trytond_analytic_budget-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      639 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-30 17:20:59.000000 trytond_analytic_budget-7.2.1/view/budget_list.xml
```

### Comparing `trytond_analytic_budget-7.2.0/CHANGELOG` & `trytond_analytic_budget-7.2.1/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_analytic_budget-7.2.0/COPYRIGHT` & `trytond_analytic_budget-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/LICENSE` & `trytond_analytic_budget-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/PKG-INFO` & `trytond_analytic_budget-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_budget
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_analytic_budget-7.2.0/__init__.py` & `trytond_analytic_budget-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/analytic_account.py` & `trytond_analytic_budget-7.2.1/analytic_account.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/analytic_account.xml` & `trytond_analytic_budget-7.2.1/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/doc/conf.py` & `trytond_analytic_budget-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/doc/design.rst` & `trytond_analytic_budget-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/doc/usage.rst` & `trytond_analytic_budget-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/bg.po` & `trytond_analytic_budget-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/ca.po` & `trytond_analytic_budget-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/cs.po` & `trytond_analytic_budget-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/de.po` & `trytond_analytic_budget-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 msgctxt "model:ir.model.button,string:budget_update_lines_button"
 msgid "Update Lines"
 msgstr "Positionen aktualisieren"
 
 msgctxt "model:ir.rule.group,name:rule_group_budget_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_form"
 msgid "Analytic Budgets"
 msgstr "Budgets Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_report"
 msgid "Analytic Budgets"
```

### Comparing `trytond_analytic_budget-7.2.0/locale/es.po` & `trytond_analytic_budget-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/es_419.po` & `trytond_analytic_budget-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/et.po` & `trytond_analytic_budget-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/fa.po` & `trytond_analytic_budget-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/fi.po` & `trytond_analytic_budget-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/fr.po` & `trytond_analytic_budget-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/hu.po` & `trytond_analytic_budget-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/id.po` & `trytond_analytic_budget-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/it.po` & `trytond_analytic_budget-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/lo.po` & `trytond_analytic_budget-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/lt.po` & `trytond_analytic_budget-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/nl.po` & `trytond_analytic_budget-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/pl.po` & `trytond_analytic_budget-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/pt.po` & `trytond_analytic_budget-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/ro.po` & `trytond_analytic_budget-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/ru.po` & `trytond_analytic_budget-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/sl.po` & `trytond_analytic_budget-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/tr.po` & `trytond_analytic_budget-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/uk.po` & `trytond_analytic_budget-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/locale/zh_CN.po` & `trytond_analytic_budget-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/setup.py` & `trytond_analytic_budget-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/tests/scenario_analytic_budget.rst` & `trytond_analytic_budget-7.2.1/tests/scenario_analytic_budget.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/tox.ini` & `trytond_analytic_budget-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/PKG-INFO` & `trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_budget
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_analytic_budget-7.2.0/trytond_analytic_budget.egg-info/SOURCES.txt` & `trytond_analytic_budget-7.2.1/trytond_analytic_budget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/view/budget_copy_start_form.xml` & `trytond_analytic_budget-7.2.1/view/budget_copy_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/view/budget_form.xml` & `trytond_analytic_budget-7.2.1/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/view/budget_line_form.xml` & `trytond_analytic_budget-7.2.1/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-7.2.0/view/budget_line_form_amount.xml` & `trytond_analytic_budget-7.2.1/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

