# Comparing `tmp/trytond_account_move_line_grouping-7.2.0.tar.gz` & `tmp/trytond_account_move_line_grouping-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_move_line_grouping-7.2.0.tar", last modified: Mon Apr 29 15:34:27 2024, max compression
+gzip compressed data, was "trytond_account_move_line_grouping-7.2.1.tar", last modified: Wed May  1 12:20:53 2024, max compression
```

## Comparing `trytond_account_move_line_grouping-7.2.0.tar` & `trytond_account_move_line_grouping-7.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.482145 trytond_account_move_line_grouping-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      861 2024-04-29 15:14:58.000000 trytond_account_move_line_grouping-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:14:57.000000 trytond_account_move_line_grouping-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2629 2024-04-29 15:34:27.482145 trytond_account_move_line_grouping-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10142 2024-02-04 18:51:26.000000 trytond_account_move_line_grouping-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5857 2024-01-27 09:58:52.000000 trytond_account_move_line_grouping-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.478812 trytond_account_move_line_grouping-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_account_move_line_grouping-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:56.000000 trytond_account_move_line_grouping-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.478812 trytond_account_move_line_grouping-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3619 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3648 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3620 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3671 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3135 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3639 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2024-04-29 13:17:17.000000 trytond_account_move_line_grouping-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-27 16:43:21.000000 trytond_account_move_line_grouping-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:27.482145 trytond_account_move_line_grouping-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4667 2024-04-27 16:30:39.000000 trytond_account_move_line_grouping-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.478812 trytond_account_move_line_grouping-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3755 2024-04-22 12:14:36.000000 trytond_account_move_line_grouping-7.2.0/tests/scenario_account_move_line_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:56.000000 trytond_account_move_line_grouping-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:14:53.000000 trytond_account_move_line_grouping-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.482145 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2629 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2077 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:27.000000 trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:27.482145 trytond_account_move_line_grouping-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2024-02-04 18:51:26.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2024-02-04 18:51:26.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_form_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-02-04 18:51:26.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-01-27 09:58:52.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-02-04 18:51:26.000000 trytond_account_move_line_grouping-7.2.0/view/move_line_group_list_payabale_receivable.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.826961 trytond_account_move_line_grouping-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-05-01 12:20:50.000000 trytond_account_move_line_grouping-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 12:20:50.000000 trytond_account_move_line_grouping-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2629 2024-05-01 12:20:53.826961 trytond_account_move_line_grouping-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10142 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5857 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.823628 trytond_account_move_line_grouping-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.823628 trytond_account_move_line_grouping-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3627 2024-04-30 17:21:59.000000 trytond_account_move_line_grouping-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3648 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3626 2024-04-30 17:21:59.000000 trytond_account_move_line_grouping-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3671 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3135 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3639 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3408 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:20:53.826961 trytond_account_move_line_grouping-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4667 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.823628 trytond_account_move_line_grouping-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3755 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/tests/scenario_account_move_line_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-30 17:21:06.000000 trytond_account_move_line_grouping-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.826961 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2629 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2077 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:20:53.000000 trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:20:53.826961 trytond_account_move_line_grouping-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      539 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_form_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-04-30 17:20:59.000000 trytond_account_move_line_grouping-7.2.1/view/move_line_group_list_payabale_receivable.xml
```

### Comparing `trytond_account_move_line_grouping-7.2.0/CHANGELOG` & `trytond_account_move_line_grouping-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_move_line_grouping-7.2.0/COPYRIGHT` & `trytond_account_move_line_grouping-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/LICENSE` & `trytond_account_move_line_grouping-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/PKG-INFO` & `trytond_account_move_line_grouping-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_move_line_grouping
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to display account move line grouped
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_move_line_grouping-7.2.0/__init__.py` & `trytond_account_move_line_grouping-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/account.py` & `trytond_account_move_line_grouping-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/account.xml` & `trytond_account_move_line_grouping-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/doc/conf.py` & `trytond_account_move_line_grouping-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/bg.po` & `trytond_account_move_line_grouping-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/ca.po` & `trytond_account_move_line_grouping-7.2.1/locale/ca.po`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
 msgstr "Import conciliat"
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Import moneda secundaria"
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
@@ -96,15 +96,15 @@
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr "Conciliat"
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
```

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/cs.po` & `trytond_account_move_line_grouping-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/de.po` & `trytond_account_move_line_grouping-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/es.po` & `trytond_account_move_line_grouping-7.2.1/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
 msgstr "Importe conciliado"
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Importe segunda moneda"
+msgstr "Importe moneda secundaria"
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
 msgstr "Empresa"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
@@ -96,15 +96,15 @@
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr "Conciliado"
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Segunda moneda"
+msgstr "Moneda secundaria"
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
```

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/es_419.po` & `trytond_account_move_line_grouping-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/et.po` & `trytond_account_move_line_grouping-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/fa.po` & `trytond_account_move_line_grouping-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/fi.po` & `trytond_account_move_line_grouping-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/fr.po` & `trytond_account_move_line_grouping-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/hu.po` & `trytond_account_move_line_grouping-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/id.po` & `trytond_account_move_line_grouping-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/it.po` & `trytond_account_move_line_grouping-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/lo.po` & `trytond_account_move_line_grouping-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/lt.po` & `trytond_account_move_line_grouping-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/nl.po` & `trytond_account_move_line_grouping-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/pl.po` & `trytond_account_move_line_grouping-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/pt.po` & `trytond_account_move_line_grouping-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/ro.po` & `trytond_account_move_line_grouping-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/ru.po` & `trytond_account_move_line_grouping-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/sl.po` & `trytond_account_move_line_grouping-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/tr.po` & `trytond_account_move_line_grouping-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/uk.po` & `trytond_account_move_line_grouping-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/locale/zh_CN.po` & `trytond_account_move_line_grouping-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/setup.py` & `trytond_account_move_line_grouping-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/tests/scenario_account_move_line_grouping.rst` & `trytond_account_move_line_grouping-7.2.1/tests/scenario_account_move_line_grouping.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/tox.ini` & `trytond_account_move_line_grouping-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/PKG-INFO` & `trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_move_line_grouping
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to display account move line grouped
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_move_line_grouping-7.2.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt` & `trytond_account_move_line_grouping-7.2.1/trytond_account_move_line_grouping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_form.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_line_group_form.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_line_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_line_group_form_move.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_line_group_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_line_group_form_payable_receivable.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_line_group_form_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_line_group_list.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_line_group_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-7.2.0/view/move_line_group_list_payabale_receivable.xml` & `trytond_account_move_line_grouping-7.2.1/view/move_line_group_list_payabale_receivable.xml`

 * *Files identical despite different names*

