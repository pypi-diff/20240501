# Comparing `tmp/trytond_account_statement_rule-7.2.0.tar.gz` & `tmp/trytond_account_statement_rule-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_rule-7.2.0.tar", last modified: Mon Apr 29 15:36:13 2024, max compression
+gzip compressed data, was "trytond_account_statement_rule-7.2.1.tar", last modified: Wed May  1 12:15:41 2024, max compression
```

## Comparing `trytond_account_statement_rule-7.2.0.tar` & `trytond_account_statement_rule-7.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1125 2024-04-29 15:16:15.000000 trytond_account_statement_rule-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:16:14.000000 trytond_account_statement_rule-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15926 2024-01-27 09:58:52.000000 trytond_account_statement_rule-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5381 2024-04-27 16:30:39.000000 trytond_account_statement_rule-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_statement_rule-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:00.000000 trytond_account_statement_rule-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5079 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4673 2024-04-29 13:17:17.000000 trytond_account_statement_rule-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4088 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-27 16:43:21.000000 trytond_account_statement_rule-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2024-03-17 11:01:36.000000 trytond_account_statement_rule-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.072717 trytond_account_statement_rule-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3950 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keyword_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3484 2024-04-22 12:14:36.000000 trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keywords.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:00.000000 trytond_account_statement_rule-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-29 15:16:10.000000 trytond_account_statement_rule-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2139 2024-04-29 15:36:13.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:12.000000 trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:13.076050 trytond_account_statement_rule-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-02-04 18:51:26.000000 trytond_account_statement_rule-7.2.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1031 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_information_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_information_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-7.2.0/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1226 2024-05-01 12:15:38.000000 trytond_account_statement_rule-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 12:15:38.000000 trytond_account_statement_rule-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15926 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5381 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5079 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2024-04-30 17:21:59.000000 trytond_account_statement_rule-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4673 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4088 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3950 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keyword_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3484 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keywords.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-30 17:21:06.000000 trytond_account_statement_rule-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2139 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1031 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_information_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_information_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/statement_tree.xml
```

### Comparing `trytond_account_statement_rule-7.2.0/CHANGELOG` & `trytond_account_statement_rule-7.2.1/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_statement_rule-7.2.0/COPYRIGHT` & `trytond_account_statement_rule-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/LICENSE` & `trytond_account_statement_rule-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/PKG-INFO` & `trytond_account_statement_rule-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to automate statement import with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement_rule-7.2.0/README.rst` & `trytond_account_statement_rule-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/__init__.py` & `trytond_account_statement_rule-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/account.py` & `trytond_account_statement_rule-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/account.xml` & `trytond_account_statement_rule-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/doc/conf.py` & `trytond_account_statement_rule-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/doc/index.rst` & `trytond_account_statement_rule-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/bg.po` & `trytond_account_statement_rule-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/ca.po` & `trytond_account_statement_rule-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/cs.po` & `trytond_account_statement_rule-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/de.po` & `trytond_account_statement_rule-7.2.1/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 msgctxt "model:ir.model.button,string:statement_apply_rules_button"
 msgid "Apply Rules"
 msgstr "Regeln anwenden"
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Benutzer in Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
 msgstr "Regeln"
 
 msgctxt "view:account.statement.rule.information:"
 msgid "-"
```

### Comparing `trytond_account_statement_rule-7.2.0/locale/es.po` & `trytond_account_statement_rule-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/es_419.po` & `trytond_account_statement_rule-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/et.po` & `trytond_account_statement_rule-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/fa.po` & `trytond_account_statement_rule-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/fi.po` & `trytond_account_statement_rule-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/fr.po` & `trytond_account_statement_rule-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/hu.po` & `trytond_account_statement_rule-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/id.po` & `trytond_account_statement_rule-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/it.po` & `trytond_account_statement_rule-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/lo.po` & `trytond_account_statement_rule-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/lt.po` & `trytond_account_statement_rule-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/nl.po` & `trytond_account_statement_rule-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/pl.po` & `trytond_account_statement_rule-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/pt.po` & `trytond_account_statement_rule-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/ro.po` & `trytond_account_statement_rule-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/ru.po` & `trytond_account_statement_rule-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/sl.po` & `trytond_account_statement_rule-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/tr.po` & `trytond_account_statement_rule-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/uk.po` & `trytond_account_statement_rule-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/locale/zh_CN.po` & `trytond_account_statement_rule-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/setup.py` & `trytond_account_statement_rule-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule.rst` & `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keyword_bank_account.rst` & `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keyword_bank_account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/tests/scenario_account_statement_rule_keywords.rst` & `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keywords.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/tox.ini` & `trytond_account_statement_rule-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/PKG-INFO` & `trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to automate statement import with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement_rule-7.2.0/trytond_account_statement_rule.egg-info/SOURCES.txt` & `trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/view/rule_form.xml` & `trytond_account_statement_rule-7.2.1/view/rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.0/view/rule_information_form.xml` & `trytond_account_statement_rule-7.2.1/view/rule_information_form.xml`

 * *Files identical despite different names*

