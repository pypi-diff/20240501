# Comparing `tmp/trytond_account_receivable_rule-7.2.0.tar.gz` & `tmp/trytond_account_receivable_rule-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_receivable_rule-7.2.0.tar", last modified: Mon Apr 29 15:35:29 2024, max compression
+gzip compressed data, was "trytond_account_receivable_rule-7.2.1.tar", last modified: Wed May  1 12:17:02 2024, max compression
```

## Comparing `trytond_account_receivable_rule-7.2.0.tar` & `trytond_account_receivable_rule-7.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:15:39.000000 trytond_account_receivable_rule-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:39.000000 trytond_account_receivable_rule-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14181 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4381 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.790515 trytond_account_receivable_rule-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_receivable_rule-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.793848 trytond_account_receivable_rule-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3874 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3892 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3877 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3289 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4111 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3604 2024-04-29 13:17:17.000000 trytond_account_receivable_rule-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-27 16:43:21.000000 trytond_account_receivable_rule-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4731 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.793848 trytond_account_receivable_rule-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4496 2024-04-22 12:14:36.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3534 2024-04-22 12:14:36.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4028 2024-04-27 16:30:39.000000 trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_receivable_rule-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-29 15:15:35.000000 trytond_account_receivable_rule-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2170 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:29.000000 trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:29.797182 trytond_account_receivable_rule-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-02-04 18:51:26.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.039690 trytond_account_receivable_rule-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2024-05-01 12:16:58.000000 trytond_account_receivable_rule-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 12:16:58.000000 trytond_account_receivable_rule-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-05-01 12:17:02.036357 trytond_account_receivable_rule-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      893 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14181 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4381 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.033023 trytond_account_receivable_rule-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.036357 trytond_account_receivable_rule-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3874 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3893 2024-04-30 17:21:59.000000 trytond_account_receivable_rule-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3877 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3289 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4111 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3604 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:17:02.039690 trytond_account_receivable_rule-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4731 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.036357 trytond_account_receivable_rule-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4496 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3534 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4028 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-30 17:21:06.000000 trytond_account_receivable_rule-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.036357 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2170 2024-05-01 12:17:02.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:17:01.000000 trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:17:02.036357 trytond_account_receivable_rule-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/view/account_receivable_rule_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/view/account_receivable_rule_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/view/account_receivable_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:20:59.000000 trytond_account_receivable_rule-7.2.1/view/account_receivable_rule_list.xml
```

### Comparing `trytond_account_receivable_rule-7.2.0/CHANGELOG` & `trytond_account_receivable_rule-7.2.1/CHANGELOG`

 * *Files 13% similar despite different names*

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

### Comparing `trytond_account_receivable_rule-7.2.0/COPYRIGHT` & `trytond_account_receivable_rule-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/LICENSE` & `trytond_account_receivable_rule-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/PKG-INFO` & `trytond_account_receivable_rule-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_receivable_rule
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to enforce receivable rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_receivable_rule-7.2.0/__init__.py` & `trytond_account_receivable_rule-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/account.py` & `trytond_account_receivable_rule-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/account.xml` & `trytond_account_receivable_rule-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/doc/conf.py` & `trytond_account_receivable_rule-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/doc/design.rst` & `trytond_account_receivable_rule-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/bg.po` & `trytond_account_receivable_rule-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/ca.po` & `trytond_account_receivable_rule-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/cs.po` & `trytond_account_receivable_rule-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/de.po` & `trytond_account_receivable_rule-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 msgctxt "help:account.account.receivable.rule,overflow_account:"
 msgid ""
 "The account to move exceeded amount.\n"
 "Leave empty to keep it in the current account."
 msgstr ""
 "Das Konto auf das eine Überzahlung gebucht werden soll.\n"
-"Leer lassen um das aktuelle Konto zu verwenden."
+"Leer lassen, um das aktuelle Konto zu verwenden."
 
 msgctxt "help:account.account.receivable.rule.account,only_reconcile:"
 msgid "Distribute only to fully reconcile."
 msgstr "Nur bei vollständiger Abstimmung verteilen."
 
 msgctxt "model:account.account.receivable.rule,name:"
 msgid "Account Receivable Rule"
@@ -106,15 +106,15 @@
 msgctxt "model:ir.model.button,string:account_receivable_rule_apply_button"
 msgid "Apply"
 msgstr "Anwenden"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_account_receivable_rule_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_account_receivable_rule_form"
 msgid "Account Receivable Rules"
 msgstr "Konto Abstimmungsregeln"
 
 msgctxt "selection:account.account.receivable.rule,priorities:"
 msgid "Account, Maturity Date"
```

### Comparing `trytond_account_receivable_rule-7.2.0/locale/es.po` & `trytond_account_receivable_rule-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/es_419.po` & `trytond_account_receivable_rule-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/et.po` & `trytond_account_receivable_rule-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/fa.po` & `trytond_account_receivable_rule-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/fi.po` & `trytond_account_receivable_rule-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/fr.po` & `trytond_account_receivable_rule-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/hu.po` & `trytond_account_receivable_rule-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/id.po` & `trytond_account_receivable_rule-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/it.po` & `trytond_account_receivable_rule-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/lo.po` & `trytond_account_receivable_rule-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/lt.po` & `trytond_account_receivable_rule-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/nl.po` & `trytond_account_receivable_rule-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/pl.po` & `trytond_account_receivable_rule-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/pt.po` & `trytond_account_receivable_rule-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/ro.po` & `trytond_account_receivable_rule-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/ru.po` & `trytond_account_receivable_rule-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/sl.po` & `trytond_account_receivable_rule-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/tr.po` & `trytond_account_receivable_rule-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/uk.po` & `trytond_account_receivable_rule-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/locale/zh_CN.po` & `trytond_account_receivable_rule-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/message.xml` & `trytond_account_receivable_rule-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/setup.py` & `trytond_account_receivable_rule-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule.rst` & `trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_overflow.rst` & `trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule_overflow.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/tests/scenario_account_receivable_rule_statement.rst` & `trytond_account_receivable_rule-7.2.1/tests/scenario_account_receivable_rule_statement.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/tox.ini` & `trytond_account_receivable_rule-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/PKG-INFO` & `trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_receivable_rule
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to enforce receivable rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_receivable_rule-7.2.0/trytond_account_receivable_rule.egg-info/SOURCES.txt` & `trytond_account_receivable_rule-7.2.1/trytond_account_receivable_rule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_receivable_rule-7.2.0/view/account_receivable_rule_form.xml` & `trytond_account_receivable_rule-7.2.1/view/account_receivable_rule_form.xml`

 * *Files identical despite different names*

