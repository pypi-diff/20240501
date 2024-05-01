# Comparing `tmp/trytond_account_budget-7.2.0.tar.gz` & `tmp/trytond_account_budget-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_budget-7.2.0.tar", last modified: Mon Apr 29 15:31:53 2024, max compression
+gzip compressed data, was "trytond_account_budget-7.2.1.tar", last modified: Wed May  1 12:24:51 2024, max compression
```

## Comparing `trytond_account_budget-7.2.0.tar` & `trytond_account_budget-7.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:12:52.000000 trytond_account_budget-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-04-29 15:12:52.000000 trytond_account_budget-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30061 2024-02-04 18:51:26.000000 trytond_account_budget-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10485 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.459506 trytond_account_budget-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1610 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:50.000000 trytond_account_budget-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10307 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10644 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10348 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10248 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8370 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8278 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10356 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9670 2024-04-29 13:17:17.000000 trytond_account_budget-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9016 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-27 16:43:20.000000 trytond_account_budget-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1012 2024-02-04 18:51:26.000000 trytond_account_budget-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4644 2024-04-27 16:30:39.000000 trytond_account_budget-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5938 2024-04-22 12:14:36.000000 trytond_account_budget-7.2.0/tests/scenario_account_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:50.000000 trytond_account_budget-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-29 15:12:48.000000 trytond_account_budget-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2373 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:31:53.000000 trytond_account_budget-7.2.0/trytond_account_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:31:53.462840 trytond_account_budget-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      563 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-01-27 09:58:52.000000 trytond_account_budget-7.2.0/view/budget_line_period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-01-27 09:58:52.000000 trytond_account_budget-7.2.0/view/budget_line_period_list_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_budget-7.2.0/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.767404 trytond_account_budget-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-05-01 12:24:48.000000 trytond_account_budget-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2024-05-01 12:24:48.000000 trytond_account_budget-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-05-01 12:24:51.767404 trytond_account_budget-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30061 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10485 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.764071 trytond_account_budget-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1258 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.764071 trytond_account_budget-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10307 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10644 2024-04-30 17:21:59.000000 trytond_account_budget-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10348 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10248 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8370 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8278 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10356 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9670 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9016 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8190 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1012 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:24:51.767404 trytond_account_budget-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4644 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.764071 trytond_account_budget-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5938 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/tests/scenario_account_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-30 17:21:06.000000 trytond_account_budget-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.767404 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2870 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2373 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:24:51.000000 trytond_account_budget-7.2.1/trytond_account_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:24:51.767404 trytond_account_budget-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      563 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_period_list_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:20:59.000000 trytond_account_budget-7.2.1/view/budget_list.xml
```

### Comparing `trytond_account_budget-7.2.0/CHANGELOG` & `trytond_account_budget-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_budget-7.2.0/COPYRIGHT` & `trytond_account_budget-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/LICENSE` & `trytond_account_budget-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/PKG-INFO` & `trytond_account_budget-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_budget
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_budget-7.2.0/__init__.py` & `trytond_account_budget-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/account.py` & `trytond_account_budget-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/account.xml` & `trytond_account_budget-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/doc/conf.py` & `trytond_account_budget-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/doc/design.rst` & `trytond_account_budget-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/doc/reference.rst` & `trytond_account_budget-7.2.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/doc/usage.rst` & `trytond_account_budget-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/bg.po` & `trytond_account_budget-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/ca.po` & `trytond_account_budget-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/cs.po` & `trytond_account_budget-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/de.po` & `trytond_account_budget-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 
 msgctxt "model:ir.model.button,string:budget_update_lines_button"
 msgid "Update Lines"
 msgstr "Positionen aktualisieren"
 
 msgctxt "model:ir.rule.group,name:rule_group_budget_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_budget"
 msgid "Budgets"
 msgstr "Budgets"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_form"
 msgid "Budgets"
```

### Comparing `trytond_account_budget-7.2.0/locale/es.po` & `trytond_account_budget-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/es_419.po` & `trytond_account_budget-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/et.po` & `trytond_account_budget-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/fa.po` & `trytond_account_budget-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/fi.po` & `trytond_account_budget-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/fr.po` & `trytond_account_budget-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/hu.po` & `trytond_account_budget-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/id.po` & `trytond_account_budget-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/it.po` & `trytond_account_budget-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/lo.po` & `trytond_account_budget-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/lt.po` & `trytond_account_budget-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/nl.po` & `trytond_account_budget-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/pl.po` & `trytond_account_budget-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/pt.po` & `trytond_account_budget-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/ro.po` & `trytond_account_budget-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/ru.po` & `trytond_account_budget-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/sl.po` & `trytond_account_budget-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/tr.po` & `trytond_account_budget-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/uk.po` & `trytond_account_budget-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/locale/zh_CN.po` & `trytond_account_budget-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/message.xml` & `trytond_account_budget-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/setup.py` & `trytond_account_budget-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/tests/scenario_account_budget.rst` & `trytond_account_budget-7.2.1/tests/scenario_account_budget.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/tox.ini` & `trytond_account_budget-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/trytond_account_budget.egg-info/PKG-INFO` & `trytond_account_budget-7.2.1/trytond_account_budget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_budget
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_budget-7.2.0/trytond_account_budget.egg-info/SOURCES.txt` & `trytond_account_budget-7.2.1/trytond_account_budget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/view/budget_form.xml` & `trytond_account_budget-7.2.1/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/view/budget_line_form.xml` & `trytond_account_budget-7.2.1/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/view/budget_line_form_amount.xml` & `trytond_account_budget-7.2.1/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-7.2.0/view/budget_line_period_form.xml` & `trytond_account_budget-7.2.1/view/budget_line_period_form.xml`

 * *Files identical despite different names*
